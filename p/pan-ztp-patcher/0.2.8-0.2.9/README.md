# Comparing `tmp/pan_ztp_patcher-0.2.8.tar.gz` & `tmp/pan_ztp_patcher-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pan_ztp_patcher-0.2.8.tar", max compression
+gzip compressed data, was "pan_ztp_patcher-0.2.9.tar", max compression
```

## Comparing `pan_ztp_patcher-0.2.8.tar` & `pan_ztp_patcher-0.2.9.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    11357 2024-04-19 23:42:26.745535 pan_ztp_patcher-0.2.8/LICENSE
--rw-r--r--   0        0        0     3524 2024-04-19 23:42:26.745535 pan_ztp_patcher-0.2.8/README.md
--rw-r--r--   0        0        0        0 2024-04-19 23:42:26.745535 pan_ztp_patcher-0.2.8/pan_ztp_patcher/__init__.py
--rw-r--r--   0        0        0    13855 2024-04-19 23:42:26.745535 pan_ztp_patcher-0.2.8/pan_ztp_patcher/app.py
--rw-r--r--   0        0        0     1026 2024-04-19 23:42:26.745535 pan_ztp_patcher-0.2.8/pan_ztp_patcher/utils.py
--rw-r--r--   0        0        0    37511 2024-04-19 23:42:26.745535 pan_ztp_patcher-0.2.8/pan_ztp_patcher/ztp_patcher.py
--rw-r--r--   0        0        0      597 2024-04-19 23:42:26.745535 pan_ztp_patcher-0.2.8/pyproject.toml
--rw-r--r--   0        0        0     4164 1970-01-01 00:00:00.000000 pan_ztp_patcher-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-20 12:03:46.862488 pan_ztp_patcher-0.2.9/LICENSE
+-rw-r--r--   0        0        0     3524 2024-04-20 12:03:46.862488 pan_ztp_patcher-0.2.9/README.md
+-rw-r--r--   0        0        0        0 2024-04-20 12:03:46.862488 pan_ztp_patcher-0.2.9/pan_ztp_patcher/__init__.py
+-rw-r--r--   0        0        0    14846 2024-04-20 12:03:46.862488 pan_ztp_patcher-0.2.9/pan_ztp_patcher/app.py
+-rw-r--r--   0        0        0     1026 2024-04-20 12:03:46.862488 pan_ztp_patcher-0.2.9/pan_ztp_patcher/utils.py
+-rw-r--r--   0        0        0    43075 2024-04-20 12:03:46.862488 pan_ztp_patcher-0.2.9/pan_ztp_patcher/ztp_patcher.py
+-rw-r--r--   0        0        0      597 2024-04-20 12:03:46.862488 pan_ztp_patcher-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0     4164 1970-01-01 00:00:00.000000 pan_ztp_patcher-0.2.9/PKG-INFO
```

### Comparing `pan_ztp_patcher-0.2.8/LICENSE` & `pan_ztp_patcher-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pan_ztp_patcher-0.2.8/README.md` & `pan_ztp_patcher-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `pan_ztp_patcher-0.2.8/pan_ztp_patcher/app.py` & `pan_ztp_patcher-0.2.9/pan_ztp_patcher/app.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,22 +4,24 @@
 import os
 import sys
 
 from dotenv import load_dotenv
 from pan_ztp_patcher.utils import setup_logging
 from pan_ztp_patcher.ztp_patcher import (
     change_firewall_password,
+    check_content_installed,
     check_content_version,
     download_software,
     copy_content_via_scp,
     install_latest_content_from_servers,
     install_specific_content_from_servers,
     install_content_via_usb,
     monitor_job_status,
     private_data_reset,
+    reboot_firewall,
     retrieve_api_key,
     retrieve_license,
 )
 
 
 def main():
     """
@@ -129,29 +131,52 @@
         pan_password_new=pan_password_new,
         pan_password_old=pan_password_old,
         pan_username=pan_username,
     )
 
     if not changed_password:
         logger.error("Failed to change the firewall password.")
-        # sys.exit(1)
+        sys.exit(1)
 
     # Retrieve the API key
     api_key = retrieve_api_key(
         pan_hostname=pan_hostname,
         pan_password_new=pan_password_new,
         pan_username=pan_username,
     )
 
     if not api_key:
         logger.error("Failed to retrieve the API key.")
         sys.exit(1)
 
     logger.info("API key retrieved successfully.")
 
+    # -----------------------------------------------------------------------
+    # Check to see if the device has content installed already
+    # -----------------------------------------------------------------------
+    content_installed = check_content_installed(
+        api_key=api_key,
+        pan_hostname=pan_hostname,
+    )
+
+    # If content is already installed, reboot the firewall
+    if content_installed:
+        logger.info("Content already installed, rebooting the firewall.")
+        reboot = reboot_firewall(
+            api_key=api_key,
+            pan_hostname=pan_hostname,
+        )
+
+        if reboot:
+            logger.info("Firewall rebooted successfully.")
+            sys.exit(0)
+        else:
+            logger.error("Failed to reboot the firewall.")
+            sys.exit(1)
+
     # ------------------------------------------------------------------------
     # Retrieve License Workflow
     # ------------------------------------------------------------------------
     license_installed = retrieve_license(
         api_key=api_key,
         pan_hostname=pan_hostname,
     )
@@ -274,14 +299,15 @@
                         pan_hostname=pan_hostname,
                     )
 
                     if jobs["result"]["install_panw"]:
                         logger.info(
                             "Specific content installed successfully from servers."
                         )
+                        break
                     else:
                         logger.warning(
                             "Failed to install specific content from servers."
                         )
                 else:
                     logger.error("Failed to retrieve the install job ID.")
             else:
@@ -392,10 +418,14 @@
         if reset:
             logger.info("Firewall data successfully reset.")
             break
         else:
             logger.warning("Failed to reset the firewall data.")
             attempt += 1
 
+    if attempt > max_attempts:
+        logger.error("Failed to reset private data.")
+        sys.exit(1)
+
 
 if __name__ == "__main__":
     main()
```

### Comparing `pan_ztp_patcher-0.2.8/pan_ztp_patcher/utils.py` & `pan_ztp_patcher-0.2.9/pan_ztp_patcher/utils.py`

 * *Files identical despite different names*

### Comparing `pan_ztp_patcher-0.2.8/pan_ztp_patcher/ztp_patcher.py` & `pan_ztp_patcher-0.2.9/pan_ztp_patcher/ztp_patcher.py`

 * *Files 8% similar despite different names*

```diff
@@ -96,14 +96,101 @@
         return False
 
     except Exception as e:
         logger.error("An error occurred: {}".format(str(e)))
         return False
 
 
+def check_content_installed(
+    api_key: str,
+    pan_hostname: str,
+) -> bool:
+    """
+    Checks if content is installed on the PAN-OS firewall.
+
+    Args:
+        api_key (str): The API key for authentication.
+        pan_hostname (str): The hostname or IP address of the PAN-OS firewall.
+
+    Returns:
+        bool: True if content is installed, False otherwise.
+    """
+
+    logger.info("=" * 79)
+    logger.info("Checking if content is installed...")
+    logger.info("=" * 79)
+
+    try:
+        # Construct the API URL for checking installed content
+        url = "https://{}/api/?type=op&cmd={}".format(
+            pan_hostname,
+            urllib.parse.quote_plus(
+                "<request><content><upgrade><check/></upgrade></content></request>"
+            ),
+        )
+        logger.debug("API URL: {}".format(url))
+
+        # Create an HTTPS request with SSL verification disabled
+        request = urllib.request.Request(url)
+        request.add_header("X-PAN-KEY", api_key)
+
+        # Send the API request
+        logger.debug("Sending API request...")
+        response = urllib.request.urlopen(
+            request, context=urllib.request.ssl._create_unverified_context()
+        )
+
+        # Read the response content
+        logger.debug("Reading response content...")
+        response_content = response.read().decode("utf-8")
+        logger.debug("Received response: {}".format(response_content))
+
+        # Parse the XML response
+        logger.debug("Parsing XML response...")
+        root = ET.fromstring(response_content)
+        logger.debug("Root element: {}".format(root.tag))
+
+        # Check the response status
+        if root.attrib.get("status") == "success":
+            content_updates = root.find("./result/content-updates")
+
+            # Check if there are any <entry> elements within <content-updates>
+            if (
+                content_updates is not None
+                and len(content_updates.findall("./entry")) > 0
+            ):
+                logger.info("Content is installed.")
+                return True
+            else:
+                logger.info("No content installed.")
+                return False
+
+        else:
+            error_message = root.find("./msg/line")
+            if error_message is not None:
+                logger.error(
+                    "API request failed: {}".format(error_message.text)
+                )
+            else:
+                logger.error("API request failed.")
+            return False
+
+    except urllib.error.URLError as url_error:
+        logger.error("URL error occurred: {}".format(str(url_error)))
+        return False
+
+    except ET.ParseError as parse_error:
+        logger.error("XML parsing error occurred: {}".format(str(parse_error)))
+        return False
+
+    except Exception as e:
+        logger.error("An error occurred: {}".format(str(e)))
+        return False
+
+
 def check_content_version(
     api_key: str,
     content_version: str,
     pan_hostname: str,
 ) -> bool:
     """
     Checks if the specified content version (filename) is available from the PANW servers.
@@ -916,14 +1003,81 @@
             return False
 
         except Exception as e:
             logger.error("An error occurred: {}".format(str(e)))
             return False
 
 
+def reboot_firewall(
+    api_key: str,
+    pan_hostname: str,
+):
+    """_summary_
+
+    Args:
+        api_key (str): _description_
+        pan_hostname (str): _description_
+    """
+
+    logger.info("=" * 79)
+    logger.info("Rebooting the firewall...")
+    logger.info("=" * 79)
+
+    while True:
+        try:
+            # Construct the API URL for rebooting the firewall
+            url = "https://{}/api/?type=op&cmd={}".format(
+                pan_hostname,
+                urllib.parse.quote_plus(
+                    "<request><restart><system/></restart></request>"
+                ),
+            )
+            logger.debug("Reboot URL: {}".format(url))
+
+            # Create an HTTPS request with SSL verification disabled
+            request = urllib.request.Request(url)
+            request.add_header("X-PAN-KEY", api_key)
+
+            # Send the API request
+            logger.debug("Sending reboot request...")
+            response = urllib.request.urlopen(
+                request,
+                context=urllib.request.ssl._create_unverified_context(),
+            )
+
+            # Check the status code
+            if response.getcode() != 200:
+                raise ValueError(
+                    "HTTP request failed with status code: {}".format(
+                        response.getcode()
+                    )
+                )
+
+            # Read the response content
+            logger.debug("Reading response content...")
+            response_content = response.read().decode("utf-8")
+            logger.debug("Received response: {}".format(response_content))
+
+            return True
+
+        except urllib.error.URLError as url_error:
+            logger.error("URL error occurred: {}".format(str(url_error)))
+            return False
+
+        except ET.ParseError as parse_error:
+            logger.error(
+                "XML parsing error occurred: {}".format(str(parse_error))
+            )
+            return False
+
+        except Exception as e:
+            logger.error("An error occurred: {}".format(str(e)))
+            return False
+
+
 def retrieve_api_key(
     pan_hostname: str,
     pan_password_new: str,
     pan_username: str,
 ) -> Optional[str]:
     """
     Retrieves the API key from the PAN-OS firewall.
@@ -942,61 +1096,78 @@
         Exception: If any other error occurs during the API request.
     """
 
     logger.info("=" * 79)
     logger.info("Retrieving API key...")
     logger.info("=" * 79)
 
-    try:
-        # Construct the API URL
-        url = "https://{}/api/?type=keygen&user={}&password={}".format(
-            pan_hostname, pan_username, urllib.parse.quote(pan_password_new)
-        )
-        logger.debug("API URL: {}".format(url))
+    max_attempts = 3
+    timeout = 3
 
-        # Create an HTTPS request with SSL verification disabled
-        logger.debug("Retrieving API key...")
-        request = urllib.request.Request(url)
-        response = urllib.request.urlopen(
-            request, context=urllib.request.ssl._create_unverified_context()
-        )
+    for attempt in range(1, max_attempts + 1):
+        try:
+            # Construct the API URL
+            url = "https://{}/api/?type=keygen&user={}&password={}".format(
+                pan_hostname, pan_username, urllib.parse.quote(pan_password_new)
+            )
+            logger.debug("API URL: {}".format(url))
 
-        # Read the response content
-        logger.debug("Reading response content...")
-        response_content = response.read().decode("utf-8")
-        logger.debug("Received response: {}".format(response_content))
+            # Create an HTTPS request with SSL verification disabled
+            logger.debug("Retrieving API key (attempt {})...".format(attempt))
+            request = urllib.request.Request(url)
+            response = urllib.request.urlopen(
+                request,
+                context=urllib.request.ssl._create_unverified_context(),
+                timeout=timeout,
+            )
 
-        # Parse the XML response
-        logger.debug("Parsing XML response...")
-        root = ET.fromstring(response_content)
-        logger.debug("Root element: {}".format(root.tag))
+            # Read the response content
+            logger.debug("Reading response content...")
+            response_content = response.read().decode("utf-8")
+            logger.debug("Received response: {}".format(response_content))
 
-        # Extract the API key from the response
-        logger.debug("Extracting API key...")
-        api_key_element = root.find("./result/key")
-        if api_key_element is not None:
-            api_key = api_key_element.text
-            logger.debug("Retrieved API key: {}".format(api_key))
-            logger.info("Retrieved API key: {}".format(api_key))
-            return api_key
-        else:
-            logger.error("API key not found in the response.")
-            return None
+            # Parse the XML response
+            logger.debug("Parsing XML response...")
+            root = ET.fromstring(response_content)
+            logger.debug("Root element: {}".format(root.tag))
 
-    except urllib.error.URLError as url_error:
-        logger.error("URL error occurred: {}".format(str(url_error)))
-        return None
+            # Extract the API key from the response
+            logger.debug("Extracting API key...")
+            api_key_element = root.find("./result/key")
+            if api_key_element is not None:
+                api_key = api_key_element.text
+                logger.debug("Retrieved API key: {}".format(api_key))
+                logger.info("Retrieved API key: {}".format(api_key))
+                return api_key
+            else:
+                logger.error("API key not found in the response.")
 
-    except ET.ParseError as parse_error:
-        logger.error("XML parsing error occurred: {}".format(str(parse_error)))
-        return None
+        except urllib.error.URLError as url_error:
+            logger.error("URL error occurred: {}".format(str(url_error)))
 
-    except Exception as e:
-        logger.error("An error occurred: {}".format(str(e)))
-        return None
+        except ET.ParseError as parse_error:
+            logger.error(
+                "XML parsing error occurred: {}".format(str(parse_error))
+            )
+
+        except Exception as e:
+            logger.error("An error occurred: {}".format(str(e)))
+
+        logger.warning(
+            "Failed to retrieve API key (attempt {})".format(attempt)
+        )
+
+        if attempt < max_attempts:
+            logger.info("Retrying in {} seconds...".format(timeout))
+            time.sleep(timeout)
+
+    logger.error(
+        "Failed to retrieve API key after {} attempts".format(max_attempts)
+    )
+    return None
 
 
 def retrieve_license(
     api_key: str,
     pan_hostname: str,
 ) -> Optional[bool]:
     """
```

### Comparing `pan_ztp_patcher-0.2.8/pyproject.toml` & `pan_ztp_patcher-0.2.9/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pan-ztp-patcher"
-version = "0.2.8"
+version = "0.2.9"
 description = "Update content version on PAN-OS firewalls"
 authors = ["Calvin Remsburg <cremsburg.dev@gmail.com>"]
 license = "Apache2.0"
 readme = "README.md"
 
 [tool.poetry.scripts]
 ztp_patcher = "pan_ztp_patcher.app:main"
```

### Comparing `pan_ztp_patcher-0.2.8/PKG-INFO` & `pan_ztp_patcher-0.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pan-ztp-patcher
-Version: 0.2.8
+Version: 0.2.9
 Summary: Update content version on PAN-OS firewalls
 License: Apache2.0
 Author: Calvin Remsburg
 Author-email: cremsburg.dev@gmail.com
 Requires-Python: >=3.8.1
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

