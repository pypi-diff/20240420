# Comparing `tmp/pan_ztp_patcher-0.2.5.tar.gz` & `tmp/pan_ztp_patcher-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pan_ztp_patcher-0.2.5.tar", max compression
+gzip compressed data, was "pan_ztp_patcher-0.2.6.tar", max compression
```

## Comparing `pan_ztp_patcher-0.2.5.tar` & `pan_ztp_patcher-0.2.6.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0     3912 2024-04-18 13:56:24.765685 pan_ztp_patcher-0.2.5/README.md
--rw-r--r--   0        0        0    13707 2024-04-19 10:27:15.254371 pan_ztp_patcher-0.2.5/pan_ztp_patcher/app.py
--rw-r--r--   0        0        0     1026 2024-04-18 15:55:37.498096 pan_ztp_patcher-0.2.5/pan_ztp_patcher/utils.py
--rw-r--r--   0        0        0    37113 2024-04-19 10:35:42.142804 pan_ztp_patcher-0.2.5/pan_ztp_patcher/ztp_patcher.py
--rw-r--r--   0        0        0      541 2024-04-19 11:01:49.890448 pan_ztp_patcher-0.2.5/pyproject.toml
--rw-r--r--   0        0        0     4650 1970-01-01 00:00:00.000000 pan_ztp_patcher-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0     3912 2024-04-19 23:12:26.253117 pan_ztp_patcher-0.2.6/README.md
+-rw-r--r--   0        0        0        0 2024-04-19 23:12:26.253117 pan_ztp_patcher-0.2.6/pan_ztp_patcher/__init__.py
+-rw-r--r--   0        0        0    13855 2024-04-19 23:12:26.253117 pan_ztp_patcher-0.2.6/pan_ztp_patcher/app.py
+-rw-r--r--   0        0        0     1026 2024-04-19 23:12:26.253117 pan_ztp_patcher-0.2.6/pan_ztp_patcher/utils.py
+-rw-r--r--   0        0        0    37511 2024-04-19 23:12:26.253117 pan_ztp_patcher-0.2.6/pan_ztp_patcher/ztp_patcher.py
+-rw-r--r--   0        0        0      597 2024-04-19 23:12:26.253117 pan_ztp_patcher-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0     4552 1970-01-01 00:00:00.000000 pan_ztp_patcher-0.2.6/PKG-INFO
```

### Comparing `pan_ztp_patcher-0.2.5/README.md` & `pan_ztp_patcher-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `pan_ztp_patcher-0.2.5/pan_ztp_patcher/app.py` & `pan_ztp_patcher-0.2.6/pan_ztp_patcher/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,15 +102,17 @@
     # Load environment variables from the specified .env file
     load_dotenv(args.env_file)
 
     # Firewall connection details
     pan_hostname = args.pan_hostname or os.getenv("PAN_HOSTNAME")
     pan_username = args.pan_username or os.getenv("PAN_USERNAME")
     pan_password_new = args.pan_password_new or os.getenv("PAN_PASSWORD")
-    pan_password_old = args.pan_password_old or os.getenv("PAN_PASSWORD_DEFAULT")
+    pan_password_old = args.pan_password_old or os.getenv(
+        "PAN_PASSWORD_DEFAULT"
+    )
 
     # Raspberry Pi connection details
     pi_hostname = args.pi_hostname or os.getenv("PI_HOSTNAME")
     pi_username = args.pi_username or os.getenv("PI_USERNAME")
     pi_password = args.pi_password or os.getenv("PI_PASSWORD")
     content_path = args.content_path or os.getenv("CONTENT_PATH")
     content_version = args.content_version or os.getenv("CONTENT_FILE")
@@ -193,18 +195,20 @@
                 pan_hostname=pan_hostname,
             )
 
             if jobs["result"]["download_panw"]:
                 logger.info(
                     "File downloaded successfully. Installing specific content from servers."
                 )
-                jobs["id"]["install_panw"] = install_specific_content_from_servers(
-                    api_key=api_key,
-                    content_version=content_version,
-                    pan_hostname=pan_hostname,
+                jobs["id"]["install_panw"] = (
+                    install_specific_content_from_servers(
+                        api_key=api_key,
+                        content_version=content_version,
+                        pan_hostname=pan_hostname,
+                    )
                 )
 
                 if jobs["id"]["install_panw"]:
                     logger.info(
                         f"Monitoring install job status for job ID: {jobs['id']['install_panw']}"
                     )
                     jobs["result"]["install_panw"] = monitor_job_status(
@@ -248,18 +252,20 @@
                 pan_hostname=pan_hostname,
             )
 
             if jobs["result"]["download_panw"]:
                 logger.info(
                     "File downloaded successfully. Installing specific content from servers."
                 )
-                jobs["id"]["install_panw"] = install_specific_content_from_servers(
-                    api_key=api_key,
-                    content_version=content_version,
-                    pan_hostname=pan_hostname,
+                jobs["id"]["install_panw"] = (
+                    install_specific_content_from_servers(
+                        api_key=api_key,
+                        content_version=content_version,
+                        pan_hostname=pan_hostname,
+                    )
                 )
 
                 if jobs["id"]["install_panw"]:
                     logger.info(
                         f"Monitoring install job status for job ID: {jobs['id']['install_panw']}"
                     )
                     jobs["result"]["install_panw"] = monitor_job_status(
@@ -292,15 +298,17 @@
         # if jobs["id"]["panw_latest"] is None, then log and increment attempt and continue
         if not jobs["id"]["panw_latest"]:
             logger.error("Failed to retrieve the job ID.")
             attempt += 1
             continue
 
         # Monitor the job status
-        logger.info(f"Monitoring job status for job ID: {jobs['id']['panw_latest']}")
+        logger.info(
+            f"Monitoring job status for job ID: {jobs['id']['panw_latest']}"
+        )
         jobs["result"]["panw_latest"] = monitor_job_status(
             api_key=api_key,
             job_id=jobs["id"]["panw_latest"],
             pan_hostname=pan_hostname,
         )
 
         # If the job was successful, break out of the loop
```

### Comparing `pan_ztp_patcher-0.2.5/pan_ztp_patcher/utils.py` & `pan_ztp_patcher-0.2.6/pan_ztp_patcher/utils.py`

 * *Files identical despite different names*

### Comparing `pan_ztp_patcher-0.2.5/pan_ztp_patcher/ztp_patcher.py` & `pan_ztp_patcher-0.2.6/pan_ztp_patcher/ztp_patcher.py`

 * *Files 2% similar despite different names*

```diff
@@ -169,25 +169,31 @@
                 filename_element = entry.find("filename")
 
                 # Check if the 'filename' element exists and matches the specified content version
                 if (
                     filename_element is not None
                     and filename_element.text == content_version
                 ):
-                    logger.info(f"Content version (filename) {content_version} found.")
+                    logger.info(
+                        f"Content version (filename) {content_version} found."
+                    )
                     return True
 
             # If the content version is not found in any entry
-            logger.info(f"Content version (filename) {content_version} not found.")
+            logger.info(
+                f"Content version (filename) {content_version} not found."
+            )
             return False
 
         else:
             error_message = root.find("./msg/line")
             if error_message is not None:
-                logger.error("API request failed: {}".format(error_message.text))
+                logger.error(
+                    "API request failed: {}".format(error_message.text)
+                )
             else:
                 logger.error("API request failed.")
             return False
 
     except urllib.error.URLError as url_error:
         logger.error("URL error occurred: {}".format(str(url_error)))
         return False
@@ -282,15 +288,17 @@
             logger.debug("Sending 'yes' to the prompt...")
             shell.send("yes\n")
             time.sleep(3)
             output = shell.recv(1024).decode("utf-8")
             logger.debug("Received output: {}".format(output))
 
         # Send the password for the Raspberry Pi
-        logger.debug("Sending password for {}@{}...".format(pi_username, pi_hostname))
+        logger.debug(
+            "Sending password for {}@{}...".format(pi_username, pi_hostname)
+        )
         time.sleep(3)
         shell.send(pi_password + "\n")
         time.sleep(3)
         output = shell.recv(1024).decode("utf-8")
         logger.debug("Received output: {}".format(output))
 
         # Wait for the completion prompt
@@ -361,15 +369,17 @@
     Raises:
         urllib.error.URLError: If a URL error occurs during the API request.
         xml.etree.ElementTree.ParseError: If an error occurs while parsing the XML response.
         Exception: If any other error occurs during the API request.
     """
 
     logger.info("=" * 79)
-    logger.info("Attempting to download software version: {}".format(content_version))
+    logger.info(
+        "Attempting to download software version: {}".format(content_version)
+    )
     logger.info("=" * 79)
 
     try:
         # Construct the API URL
         url = "https://{}/api/?type=op&cmd={}".format(
             pan_hostname,
             urllib.parse.quote_plus(
@@ -416,15 +426,17 @@
             else:
                 logger.error("Job ID not found in the response.")
                 return None
 
         else:
             error_message = root.find("./msg/line")
             if error_message is not None:
-                logger.error("API request failed: {}".format(error_message.text))
+                logger.error(
+                    "API request failed: {}".format(error_message.text)
+                )
             else:
                 logger.error("API request failed.")
             return None
 
     except urllib.error.URLError as url_error:
         logger.error("URL error occurred: {}".format(str(url_error)))
         return None
@@ -510,15 +522,17 @@
             else:
                 logger.error("Job ID not found in the response.")
                 return None
 
         else:
             error_message = root.find("./msg/line")
             if error_message is not None:
-                logger.error("API request failed: {}".format(error_message.text))
+                logger.error(
+                    "API request failed: {}".format(error_message.text)
+                )
             else:
                 logger.error("API request failed.")
             return None
 
     except urllib.error.URLError as url_error:
         logger.error("URL error occurred: {}".format(str(url_error)))
         return None
@@ -598,15 +612,17 @@
 
             # Log an error if the job ID is not found
             else:
                 logger.error("Job ID not found in the response.")
                 return None
 
         elif root.attrib.get("line") > 0:
-            logger.error("API request failed: {}".format(root.attrib.get("line")))
+            logger.error(
+                "API request failed: {}".format(root.attrib.get("line"))
+            )
             return None
 
         else:
             logger.error("API request failed.")
             return None
 
     except urllib.error.URLError as url_error:
@@ -641,15 +657,17 @@
     Raises:
         urllib.error.URLError: If a URL error occurs during the API request.
         xml.etree.ElementTree.ParseError: If an error occurs while parsing the XML response.
         Exception: If any other error occurs during the API request.
     """
 
     logger.info("=" * 79)
-    logger.info(f"Attempting to install specific content version: {content_version}")
+    logger.info(
+        f"Attempting to install specific content version: {content_version}"
+    )
     logger.info("=" * 79)
 
     try:
         # Construct the API URL
         url = "https://{}/api/?type=op&cmd={}".format(
             pan_hostname,
             urllib.parse.quote_plus(
@@ -694,15 +712,17 @@
             else:
                 logger.error("Job ID not found in the response.")
                 return None
 
         else:
             error_message = root.find("./msg/line")
             if error_message is not None:
-                logger.error("API request failed: {}".format(error_message.text))
+                logger.error(
+                    "API request failed: {}".format(error_message.text)
+                )
             else:
                 logger.error("API request failed.")
             return None
 
     except urllib.error.URLError as url_error:
         logger.error("URL error occurred: {}".format(str(url_error)))
         return None
@@ -813,15 +833,17 @@
 
             # Wait for 3 seconds before the next iteration
             time.sleep(3)
 
         except urllib.error.URLError as url_error:
             logger.error("URL error occurred: {}".format(str(url_error)))
         except ET.ParseError as parse_error:
-            logger.error("XML parsing error occurred: {}".format(str(parse_error)))
+            logger.error(
+                "XML parsing error occurred: {}".format(str(parse_error))
+            )
         except Exception as e:
             logger.error("An error occurred: {}".format(str(e)))
 
 
 def private_data_reset(
     api_key: str,
     pan_hostname: str,
@@ -884,15 +906,17 @@
             return True
 
         except urllib.error.URLError as url_error:
             logger.error("URL error occurred: {}".format(str(url_error)))
             return False
 
         except ET.ParseError as parse_error:
-            logger.error("XML parsing error occurred: {}".format(str(parse_error)))
+            logger.error(
+                "XML parsing error occurred: {}".format(str(parse_error))
+            )
             return False
 
         except Exception as e:
             logger.error("An error occurred: {}".format(str(e)))
             return False
 
 
@@ -995,15 +1019,17 @@
     logger.info("Retrieving licenses...")
     logger.info("=" * 79)
 
     try:
         # Construct the API URL for retrieving licenses
         url = "https://{}/api/?type=op&cmd={}".format(
             pan_hostname,
-            urllib.parse.quote_plus("<request><license><fetch/></license></request>"),
+            urllib.parse.quote_plus(
+                "<request><license><fetch/></license></request>"
+            ),
         )
         logger.debug("API URL: {}".format(url))
 
         # Create an HTTPS request with SSL verification disabled
         request = urllib.request.Request(url)
         request.add_header("X-PAN-KEY", api_key)
```

### Comparing `pan_ztp_patcher-0.2.5/pyproject.toml` & `pan_ztp_patcher-0.2.6/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 [tool.poetry]
 name = "pan-ztp-patcher"
-version = "0.2.5"
+version = "0.2.6"
 description = "Update content version on PAN-OS firewalls"
 authors = ["Calvin Remsburg <cremsburg.dev@gmail.com>"]
 license = "Apache2.0"
 readme = "README.md"
 
 [tool.poetry.scripts]
 ztp_patcher = "pan_ztp_patcher.app:main"
 
 [tool.poetry.dependencies]
-python = ">=3.7"
+python = ">=3.8.1"
 paramiko = "^3.4.0"
 python-dotenv = "0.21.1"
 
 [tool.poetry.group.dev.dependencies]
 ipdb = "^0.13.13"
+pytest = "^8.1.1"
+flake8 = "^7.0.0"
+black = "^24.4.0"
 
 [tool.black]
 line-length = 80
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `pan_ztp_patcher-0.2.5/PKG-INFO` & `pan_ztp_patcher-0.2.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 Metadata-Version: 2.1
 Name: pan-ztp-patcher
-Version: 0.2.5
+Version: 0.2.6
 Summary: Update content version on PAN-OS firewalls
 License: Apache2.0
 Author: Calvin Remsburg
 Author-email: cremsburg.dev@gmail.com
-Requires-Python: >=3.7
+Requires-Python: >=3.8.1
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: paramiko (>=3.4.0,<4.0.0)
 Requires-Dist: python-dotenv (==0.21.1)
 Description-Content-Type: text/markdown
```

