# Comparing `tmp/botasaurus2-1.4.5.tar.gz` & `tmp/botasaurus2-1.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botasaurus2-1.4.5.tar", max compression
+gzip compressed data, was "botasaurus2-1.4.6.tar", max compression
```

## Comparing `botasaurus2-1.4.5.tar` & `botasaurus2-1.4.6.tar`

### file list

```diff
@@ -1,51 +1,51 @@
--rw-r--r--   0        0        0      217 2024-03-15 22:38:58.098040 botasaurus2-1.4.5/AUTHORS
--rw-r--r--   0        0        0     1073 2024-03-15 22:38:58.098040 botasaurus2-1.4.5/LICENSE
--rw-r--r--   0        0        0    50976 2024-03-19 13:44:59.662333 botasaurus2-1.4.5/README.md
--rw-r--r--   0        0        0      854 2024-04-15 19:45:21.210506 botasaurus2-1.4.5/botasaurus/__init__.py
--rw-r--r--   0        0        0      211 2024-03-15 22:38:58.098040 botasaurus2-1.4.5/botasaurus/_id.py
--rw-r--r--   0        0        0     1034 2024-03-15 22:38:58.098040 botasaurus2-1.4.5/botasaurus/accept_google_cookies.py
--rw-r--r--   0        0        0    57750 2024-04-15 18:54:34.470840 botasaurus2-1.4.5/botasaurus/anti_detect_driver.py
--rw-r--r--   0        0        0     4485 2024-04-11 15:00:22.756112 botasaurus2-1.4.5/botasaurus/anti_detect_requests.py
--rw-r--r--   0        0        0     3549 2024-03-15 22:38:58.098040 botasaurus2-1.4.5/botasaurus/base_data.py
--rw-r--r--   0        0        0      800 2024-03-15 22:38:58.098040 botasaurus2-1.4.5/botasaurus/beep_utils.py
--rw-r--r--   0        0        0     2868 2024-04-12 14:30:05.866696 botasaurus2-1.4.5/botasaurus/botasaurus_storage.py
--rw-r--r--   0        0        0      944 2024-04-11 21:17:56.332972 botasaurus2-1.4.5/botasaurus/bt.py
--rw-r--r--   0        0        0     7486 2024-03-15 22:38:58.098040 botasaurus2-1.4.5/botasaurus/cache.py
--rw-r--r--   0        0        0     2114 2024-03-15 22:38:58.098040 botasaurus2-1.4.5/botasaurus/calc_max_parallel_browsers.py
--rw-r--r--   0        0        0    28154 2024-04-11 15:00:22.756112 botasaurus2-1.4.5/botasaurus/captcha.py
--rw-r--r--   0        0        0      566 2024-03-15 22:38:58.098040 botasaurus2-1.4.5/botasaurus/check_and_download_driver.py
--rw-r--r--   0        0        0      362 2024-03-15 22:38:58.098040 botasaurus2-1.4.5/botasaurus/chrome_launcher_adapter.py
--rw-r--r--   0        0        0    14871 2024-03-15 22:38:58.098040 botasaurus2-1.4.5/botasaurus/cl.py
--rw-r--r--   0        0        0      946 2024-03-15 22:38:58.098040 botasaurus2-1.4.5/botasaurus/close.py
--rw-r--r--   0        0        0      256 2024-03-20 15:48:31.573396 botasaurus2-1.4.5/botasaurus/constants.py
--rw-r--r--   0        0        0    15624 2024-04-17 10:36:48.584260 botasaurus2-1.4.5/botasaurus/create_driver_utils.py
--rw-r--r--   0        0        0    12609 2024-04-15 20:12:50.183439 botasaurus2-1.4.5/botasaurus/create_stealth_driver.py
--rw-r--r--   0        0        0     1820 2024-03-15 22:38:58.102041 botasaurus2-1.4.5/botasaurus/creators.py
--rw-r--r--   0        0        0     4130 2024-03-15 22:38:58.102041 botasaurus2-1.4.5/botasaurus/decorator_helpers.py
--rw-r--r--   0        0        0    39385 2024-04-15 21:45:09.835191 botasaurus2-1.4.5/botasaurus/decorators.py
--rw-r--r--   0        0        0      491 2024-03-15 22:38:58.102041 botasaurus2-1.4.5/botasaurus/decorators_utils.py
--rw-r--r--   0        0        0     1617 2024-03-15 22:38:58.102041 botasaurus2-1.4.5/botasaurus/download_driver.py
--rw-r--r--   0        0        0      459 2024-03-15 22:38:58.102041 botasaurus2-1.4.5/botasaurus/driver_about.py
--rw-r--r--   0        0        0       48 2024-03-15 22:38:58.102041 botasaurus2-1.4.5/botasaurus/exceptions.py
--rw-r--r--   0        0        0       84 2024-03-15 22:38:58.102041 botasaurus2-1.4.5/botasaurus/formats.py
--rw-r--r--   0        0        0    14839 2024-03-15 22:38:58.102041 botasaurus2-1.4.5/botasaurus/get_chrome_version.py
--rw-r--r--   0        0        0     8679 2024-04-11 15:00:22.756112 botasaurus2-1.4.5/botasaurus/got_adapter.py
--rw-r--r--   0        0        0     2438 2024-04-12 14:30:10.786777 botasaurus2-1.4.5/botasaurus/ip_utils.py
--rw-r--r--   0        0        0     1534 2024-03-15 22:38:58.102041 botasaurus2-1.4.5/botasaurus/list_utils.py
--rw-r--r--   0        0        0     3326 2024-04-11 20:48:02.911490 botasaurus2-1.4.5/botasaurus/local_storage.py
--rw-r--r--   0        0        0     1674 2024-03-15 22:38:58.102041 botasaurus2-1.4.5/botasaurus/local_storage_driver.py
--rw-r--r--   0        0        0       77 2024-03-15 22:38:58.102041 botasaurus2-1.4.5/botasaurus/opponent.py
--rw-r--r--   0        0        0     7343 2024-03-19 13:44:59.666333 botasaurus2-1.4.5/botasaurus/output.py
--rw-r--r--   0        0        0     4964 2024-04-12 14:01:33.922678 botasaurus2-1.4.5/botasaurus/profile.py
--rw-r--r--   0        0        0      352 2024-03-19 19:06:20.087339 botasaurus2-1.4.5/botasaurus/shortcuts.py
--rw-r--r--   0        0        0    22453 2024-03-15 22:38:58.102041 botasaurus2-1.4.5/botasaurus/sitemap.py
--rw-r--r--   0        0        0     2031 2024-03-19 13:44:59.666333 botasaurus2-1.4.5/botasaurus/str_utils.py
--rw-r--r--   0        0        0     6298 2024-03-15 22:38:58.102041 botasaurus2-1.4.5/botasaurus/temp_mail.py
--rw-r--r--   0        0        0       54 2024-03-15 22:38:58.102041 botasaurus2-1.4.5/botasaurus/usage.py
--rw-r--r--   0        0        0     7457 2024-03-15 22:38:58.102041 botasaurus2-1.4.5/botasaurus/user_agent.py
--rw-r--r--   0        0        0     4194 2024-03-15 22:38:58.102041 botasaurus2-1.4.5/botasaurus/user_generator.py
--rw-r--r--   0        0        0     8611 2024-04-15 14:50:43.118678 botasaurus2-1.4.5/botasaurus/utils.py
--rw-r--r--   0        0        0       57 2024-03-15 22:38:58.102041 botasaurus2-1.4.5/botasaurus/wait.py
--rw-r--r--   0        0        0     1183 2024-03-15 22:38:58.102041 botasaurus2-1.4.5/botasaurus/window_size.py
--rw-r--r--   0        0        0      848 2024-04-17 10:37:11.272301 botasaurus2-1.4.5/pyproject.toml
--rw-r--r--   0        0        0    52119 1970-01-01 00:00:00.000000 botasaurus2-1.4.5/PKG-INFO
+-rw-r--r--   0        0        0      217 2024-03-15 22:38:58.098040 botasaurus2-1.4.6/AUTHORS
+-rw-r--r--   0        0        0     1073 2024-03-15 22:38:58.098040 botasaurus2-1.4.6/LICENSE
+-rw-r--r--   0        0        0    50976 2024-03-19 13:44:59.662333 botasaurus2-1.4.6/README.md
+-rw-r--r--   0        0        0      854 2024-04-15 19:45:21.210506 botasaurus2-1.4.6/botasaurus/__init__.py
+-rw-r--r--   0        0        0      211 2024-03-15 22:38:58.098040 botasaurus2-1.4.6/botasaurus/_id.py
+-rw-r--r--   0        0        0     1034 2024-03-15 22:38:58.098040 botasaurus2-1.4.6/botasaurus/accept_google_cookies.py
+-rw-r--r--   0        0        0    57750 2024-04-15 18:54:34.470840 botasaurus2-1.4.6/botasaurus/anti_detect_driver.py
+-rw-r--r--   0        0        0     4485 2024-04-11 15:00:22.756112 botasaurus2-1.4.6/botasaurus/anti_detect_requests.py
+-rw-r--r--   0        0        0     3549 2024-03-15 22:38:58.098040 botasaurus2-1.4.6/botasaurus/base_data.py
+-rw-r--r--   0        0        0      800 2024-03-15 22:38:58.098040 botasaurus2-1.4.6/botasaurus/beep_utils.py
+-rw-r--r--   0        0        0     2868 2024-04-12 14:30:05.866696 botasaurus2-1.4.6/botasaurus/botasaurus_storage.py
+-rw-r--r--   0        0        0      944 2024-04-11 21:17:56.332972 botasaurus2-1.4.6/botasaurus/bt.py
+-rw-r--r--   0        0        0     7486 2024-03-15 22:38:58.098040 botasaurus2-1.4.6/botasaurus/cache.py
+-rw-r--r--   0        0        0     2114 2024-03-15 22:38:58.098040 botasaurus2-1.4.6/botasaurus/calc_max_parallel_browsers.py
+-rw-r--r--   0        0        0    28154 2024-04-11 15:00:22.756112 botasaurus2-1.4.6/botasaurus/captcha.py
+-rw-r--r--   0        0        0      566 2024-03-15 22:38:58.098040 botasaurus2-1.4.6/botasaurus/check_and_download_driver.py
+-rw-r--r--   0        0        0      362 2024-03-15 22:38:58.098040 botasaurus2-1.4.6/botasaurus/chrome_launcher_adapter.py
+-rw-r--r--   0        0        0    14871 2024-03-15 22:38:58.098040 botasaurus2-1.4.6/botasaurus/cl.py
+-rw-r--r--   0        0        0      946 2024-03-15 22:38:58.098040 botasaurus2-1.4.6/botasaurus/close.py
+-rw-r--r--   0        0        0      256 2024-03-20 15:48:31.573396 botasaurus2-1.4.6/botasaurus/constants.py
+-rw-r--r--   0        0        0    15623 2024-04-20 17:45:40.081352 botasaurus2-1.4.6/botasaurus/create_driver_utils.py
+-rw-r--r--   0        0        0    12641 2024-04-20 17:45:05.253739 botasaurus2-1.4.6/botasaurus/create_stealth_driver.py
+-rw-r--r--   0        0        0     1820 2024-03-15 22:38:58.102041 botasaurus2-1.4.6/botasaurus/creators.py
+-rw-r--r--   0        0        0     4130 2024-03-15 22:38:58.102041 botasaurus2-1.4.6/botasaurus/decorator_helpers.py
+-rw-r--r--   0        0        0    39495 2024-04-19 09:20:51.822788 botasaurus2-1.4.6/botasaurus/decorators.py
+-rw-r--r--   0        0        0      491 2024-03-15 22:38:58.102041 botasaurus2-1.4.6/botasaurus/decorators_utils.py
+-rw-r--r--   0        0        0     1617 2024-03-15 22:38:58.102041 botasaurus2-1.4.6/botasaurus/download_driver.py
+-rw-r--r--   0        0        0      459 2024-03-15 22:38:58.102041 botasaurus2-1.4.6/botasaurus/driver_about.py
+-rw-r--r--   0        0        0       48 2024-03-15 22:38:58.102041 botasaurus2-1.4.6/botasaurus/exceptions.py
+-rw-r--r--   0        0        0       84 2024-03-15 22:38:58.102041 botasaurus2-1.4.6/botasaurus/formats.py
+-rw-r--r--   0        0        0    14839 2024-03-15 22:38:58.102041 botasaurus2-1.4.6/botasaurus/get_chrome_version.py
+-rw-r--r--   0        0        0     8679 2024-04-11 15:00:22.756112 botasaurus2-1.4.6/botasaurus/got_adapter.py
+-rw-r--r--   0        0        0     2438 2024-04-12 14:30:10.786777 botasaurus2-1.4.6/botasaurus/ip_utils.py
+-rw-r--r--   0        0        0     1534 2024-03-15 22:38:58.102041 botasaurus2-1.4.6/botasaurus/list_utils.py
+-rw-r--r--   0        0        0     3326 2024-04-11 20:48:02.911490 botasaurus2-1.4.6/botasaurus/local_storage.py
+-rw-r--r--   0        0        0     1674 2024-03-15 22:38:58.102041 botasaurus2-1.4.6/botasaurus/local_storage_driver.py
+-rw-r--r--   0        0        0       77 2024-03-15 22:38:58.102041 botasaurus2-1.4.6/botasaurus/opponent.py
+-rw-r--r--   0        0        0     7343 2024-03-19 13:44:59.666333 botasaurus2-1.4.6/botasaurus/output.py
+-rw-r--r--   0        0        0     4964 2024-04-12 14:01:33.922678 botasaurus2-1.4.6/botasaurus/profile.py
+-rw-r--r--   0        0        0      352 2024-03-19 19:06:20.087339 botasaurus2-1.4.6/botasaurus/shortcuts.py
+-rw-r--r--   0        0        0    22453 2024-03-15 22:38:58.102041 botasaurus2-1.4.6/botasaurus/sitemap.py
+-rw-r--r--   0        0        0     2031 2024-03-19 13:44:59.666333 botasaurus2-1.4.6/botasaurus/str_utils.py
+-rw-r--r--   0        0        0     6298 2024-03-15 22:38:58.102041 botasaurus2-1.4.6/botasaurus/temp_mail.py
+-rw-r--r--   0        0        0       54 2024-03-15 22:38:58.102041 botasaurus2-1.4.6/botasaurus/usage.py
+-rw-r--r--   0        0        0     7457 2024-03-15 22:38:58.102041 botasaurus2-1.4.6/botasaurus/user_agent.py
+-rw-r--r--   0        0        0     4194 2024-03-15 22:38:58.102041 botasaurus2-1.4.6/botasaurus/user_generator.py
+-rw-r--r--   0        0        0     8611 2024-04-15 14:50:43.118678 botasaurus2-1.4.6/botasaurus/utils.py
+-rw-r--r--   0        0        0       57 2024-03-15 22:38:58.102041 botasaurus2-1.4.6/botasaurus/wait.py
+-rw-r--r--   0        0        0     1183 2024-03-15 22:38:58.102041 botasaurus2-1.4.6/botasaurus/window_size.py
+-rw-r--r--   0        0        0      848 2024-04-20 17:47:46.152103 botasaurus2-1.4.6/pyproject.toml
+-rw-r--r--   0        0        0    52119 1970-01-01 00:00:00.000000 botasaurus2-1.4.6/PKG-INFO
```

### Comparing `botasaurus2-1.4.5/LICENSE` & `botasaurus2-1.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.4.5/README.md` & `botasaurus2-1.4.6/README.md`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.4.5/botasaurus/__init__.py` & `botasaurus2-1.4.6/botasaurus/__init__.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.4.5/botasaurus/accept_google_cookies.py` & `botasaurus2-1.4.6/botasaurus/accept_google_cookies.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.4.5/botasaurus/anti_detect_driver.py` & `botasaurus2-1.4.6/botasaurus/anti_detect_driver.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.4.5/botasaurus/anti_detect_requests.py` & `botasaurus2-1.4.6/botasaurus/anti_detect_requests.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.4.5/botasaurus/base_data.py` & `botasaurus2-1.4.6/botasaurus/base_data.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.4.5/botasaurus/beep_utils.py` & `botasaurus2-1.4.6/botasaurus/beep_utils.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.4.5/botasaurus/botasaurus_storage.py` & `botasaurus2-1.4.6/botasaurus/botasaurus_storage.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.4.5/botasaurus/bt.py` & `botasaurus2-1.4.6/botasaurus/bt.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.4.5/botasaurus/cache.py` & `botasaurus2-1.4.6/botasaurus/cache.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.4.5/botasaurus/calc_max_parallel_browsers.py` & `botasaurus2-1.4.6/botasaurus/calc_max_parallel_browsers.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.4.5/botasaurus/captcha.py` & `botasaurus2-1.4.6/botasaurus/captcha.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.4.5/botasaurus/check_and_download_driver.py` & `botasaurus2-1.4.6/botasaurus/check_and_download_driver.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.4.5/botasaurus/cl.py` & `botasaurus2-1.4.6/botasaurus/cl.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.4.5/botasaurus/close.py` & `botasaurus2-1.4.6/botasaurus/close.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.4.5/botasaurus/create_driver_utils.py` & `botasaurus2-1.4.6/botasaurus/create_driver_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -237,15 +237,15 @@
     # Check if '--server' is in the list of command-line arguments
     return '--server' in argv
 
 def create_selenium_driver(options,
                            desired_capabilities,
                            attempt_download=True,
                            remote=False,
-                           remote_url="http://localhost:4444/wd/hub"):
+                           remote_url="http://selenoid:4444/wd/hub"):
 
     try:
         if desired_capabilities:
             for name, value in desired_capabilities.items():
                 options.set_capability(name, value)
         if remote:
             return AntiDetectDriverRemote(
```

### Comparing `botasaurus2-1.4.5/botasaurus/create_stealth_driver.py` & `botasaurus2-1.4.6/botasaurus/create_stealth_driver.py`

 * *Files 2% similar despite different names*

```diff
@@ -246,15 +246,15 @@
     except JavaScriptError as e:
         if "ECONNREFUSED" in e.js and not is_server_mode():
             add_server_args(options)
             print("Chrome failed to launch. Retrying with additional server options. To add server options by default, include '--server' in your launch command.")
             return launch_chrome(start_url, options._arguments)
         raise
 
-def do_create_stealth_driver(data, options, desired_capabilities, start_url, wait,  raise_exception,add_arguments, remote: bool = False):
+def do_create_stealth_driver(data, options, desired_capabilities, start_url, wait,  raise_exception,add_arguments, remote: bool = False, remote_url: str = "http://selenoid:4444/wd/hub"):
     options = clean_options(options)
     if add_arguments:
         add_arguments(data, options)
     remote_driver_options = options
     if not remote:
         remote_driver_options = Options()
         chrome = launch_server_safe_chrome(options, start_url)
@@ -265,16 +265,15 @@
                 print(f"Waiting {wait} seconds before connecting to Chrome...")
                 sleep(wait)
 
 
         remote_driver_options.add_experimental_option(
             "debuggerAddress", f"127.0.0.1:{debug_port}"
         )
-    logger.debug(remote_driver_options)
-    remote_driver = create_selenium_driver(remote_driver_options, desired_capabilities, remote=remote)
+    remote_driver = create_selenium_driver(remote_driver_options, desired_capabilities, remote=remote, remote_url=remote_url)
     if not remote:
         pid = chrome.pid
 
         remote_driver.kill_chrome_by_pid = lambda: kill_process_by_pid(pid)
 
         if not should_wait:
                 sleep(1) # Still do some wait to prevent exceptions
```

### Comparing `botasaurus2-1.4.5/botasaurus/creators.py` & `botasaurus2-1.4.6/botasaurus/creators.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.4.5/botasaurus/decorator_helpers.py` & `botasaurus2-1.4.6/botasaurus/decorator_helpers.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.4.5/botasaurus/decorators.py` & `botasaurus2-1.4.6/botasaurus/decorators.py`

 * *Files 1% similar despite different names*

```diff
@@ -442,15 +442,18 @@
             create_driver = kwargs.get("create_driver", create_driver)
             capabilities = kwargs.get("capabilities", capabilities)
             local_storage_dir = kwargs.get("local_storage_dir", local_storage_dir)
             remote = kwargs.get("remote", remote)
             remote_url = kwargs.get("remote_url", remote_url)
             
             local_storage = LocalStorageClass(local_storage_dir)
-            Profile = ProfileClass(local_storage_dir / Path('profiles'))
+            profile_path = None
+            if local_storage_dir:
+                profile_path = local_storage_dir / Path('profiles')
+            Profile = ProfileClass(profile_path)
             Profile.profile = profile
             fn_name = func.__name__
 
             if cache:
                 _create_cache_directory_if_not_exists(func)
 
             # # Pool to hold reusable drivers
```

### Comparing `botasaurus2-1.4.5/botasaurus/download_driver.py` & `botasaurus2-1.4.6/botasaurus/download_driver.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.4.5/botasaurus/get_chrome_version.py` & `botasaurus2-1.4.6/botasaurus/get_chrome_version.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.4.5/botasaurus/got_adapter.py` & `botasaurus2-1.4.6/botasaurus/got_adapter.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.4.5/botasaurus/ip_utils.py` & `botasaurus2-1.4.6/botasaurus/ip_utils.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.4.5/botasaurus/list_utils.py` & `botasaurus2-1.4.6/botasaurus/list_utils.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.4.5/botasaurus/local_storage.py` & `botasaurus2-1.4.6/botasaurus/local_storage.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.4.5/botasaurus/local_storage_driver.py` & `botasaurus2-1.4.6/botasaurus/local_storage_driver.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.4.5/botasaurus/output.py` & `botasaurus2-1.4.6/botasaurus/output.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.4.5/botasaurus/profile.py` & `botasaurus2-1.4.6/botasaurus/profile.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.4.5/botasaurus/sitemap.py` & `botasaurus2-1.4.6/botasaurus/sitemap.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.4.5/botasaurus/str_utils.py` & `botasaurus2-1.4.6/botasaurus/str_utils.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.4.5/botasaurus/temp_mail.py` & `botasaurus2-1.4.6/botasaurus/temp_mail.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.4.5/botasaurus/user_agent.py` & `botasaurus2-1.4.6/botasaurus/user_agent.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.4.5/botasaurus/user_generator.py` & `botasaurus2-1.4.6/botasaurus/user_generator.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.4.5/botasaurus/utils.py` & `botasaurus2-1.4.6/botasaurus/utils.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.4.5/botasaurus/window_size.py` & `botasaurus2-1.4.6/botasaurus/window_size.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.4.5/pyproject.toml` & `botasaurus2-1.4.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "botasaurus2"
-version = "1.4.5"
+version = "1.4.6"
 description = "Patching fork of botasaurus, The All in One Framework to build Awesome Scrapers."
 authors = ["Chetan Jain <chetan@omkar.cloud>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "botasaurus", from = "."}]
 
 [tool.poetry.dependencies]
```

### Comparing `botasaurus2-1.4.5/PKG-INFO` & `botasaurus2-1.4.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botasaurus2
-Version: 1.4.5
+Version: 1.4.6
 Summary: Patching fork of botasaurus, The All in One Framework to build Awesome Scrapers.
 License: MIT
 Author: Chetan Jain
 Author-email: chetan@omkar.cloud
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: botasaurus2 Version: 1.4.5 Summary: Patching fork
+Metadata-Version: 2.1 Name: botasaurus2 Version: 1.4.6 Summary: Patching fork
 of botasaurus, The All in One Framework to build Awesome Scrapers. License: MIT
 Author: Chetan Jain Author-email: chetan@omkar.cloud Requires-Python:
 >=3.10,<4.0 Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
 Programming Language :: Python :: 3.12 Requires-Dist: aigents (>=0.5.0,<0.6.0)
 Requires-Dist: beautifulsoup4 (>=4.11.2,<5.0.0) Requires-Dist: botasaurus-
```

