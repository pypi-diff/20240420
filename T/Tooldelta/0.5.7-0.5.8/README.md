# Comparing `tmp/tooldelta-0.5.7.tar.gz` & `tmp/tooldelta-0.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tooldelta-0.5.7.tar", max compression
+gzip compressed data, was "tooldelta-0.5.8.tar", max compression
```

## Comparing `tooldelta-0.5.7.tar` & `tooldelta-0.5.8.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rwxr-xr-x   0        0        0     1497 2024-04-19 14:07:38.946065 tooldelta-0.5.7/LICENSE
--rwxr-xr-x   0        0        0     2504 2024-04-19 14:07:38.946065 tooldelta-0.5.7/README.md
--rwxr-xr-x   0        0        0      973 2024-04-19 14:07:46.998008 tooldelta-0.5.7/pyproject.toml
--rwxr-xr-x   0        0        0      360 2024-04-19 14:07:38.950065 tooldelta-0.5.7/tooldelta/__init__.py
--rw-r--r--   0        0        0     4979 2024-04-19 14:07:38.950065 tooldelta-0.5.7/tooldelta/auths.py
--rwxr-xr-x   0        0        0    19961 2024-04-19 14:07:38.950065 tooldelta-0.5.7/tooldelta/builtins.py
--rwxr-xr-x   0        0        0    12365 2024-04-19 14:07:38.950065 tooldelta-0.5.7/tooldelta/cfg.py
--rwxr-xr-x   0        0        0    10889 2024-04-19 14:07:38.950065 tooldelta-0.5.7/tooldelta/color_print.py
--rw-r--r--   0        0        0     1884 2024-04-19 14:07:38.950065 tooldelta-0.5.7/tooldelta/constants.py
--rw-r--r--   0        0        0     5870 2024-04-19 14:07:38.950065 tooldelta-0.5.7/tooldelta/fb_conn/fbconn.py
--rwxr-xr-x   0        0        0    30100 2024-04-19 14:07:38.950065 tooldelta-0.5.7/tooldelta/frame.py
--rwxr-xr-x   0        0        0     4644 2024-04-19 14:07:38.950065 tooldelta-0.5.7/tooldelta/game_texts.py
--rwxr-xr-x   0        0        0      476 2024-04-19 14:07:38.950065 tooldelta-0.5.7/tooldelta/get_tool_delta_version.py
--rwxr-xr-x   0        0        0    20525 2024-04-19 14:07:38.950065 tooldelta-0.5.7/tooldelta/launch_cli.py
--rwxr-xr-x   0        0        0     1276 2024-04-19 14:07:38.950065 tooldelta-0.5.7/tooldelta/launch_options.py
--rwxr-xr-x   0        0        0     2425 2024-04-19 14:07:38.950065 tooldelta-0.5.7/tooldelta/logger.py
--rw-r--r--   0        0        0    30151 2024-04-19 14:07:38.950065 tooldelta-0.5.7/tooldelta/neo_conn.py
--rwxr-xr-x   0        0        0     1292 2024-04-19 14:07:38.950065 tooldelta-0.5.7/tooldelta/packets.py
--rwxr-xr-x   0        0        0    15769 2024-04-19 14:07:38.950065 tooldelta-0.5.7/tooldelta/plugin_load/PluginGroup.py
--rwxr-xr-x   0        0        0     3118 2024-04-19 14:07:38.950065 tooldelta-0.5.7/tooldelta/plugin_load/__init__.py
--rwxr-xr-x   0        0        0     7341 2024-04-19 14:07:38.950065 tooldelta-0.5.7/tooldelta/plugin_load/classic_plugin/__init__.py
--rwxr-xr-x   0        0        0      450 2024-04-19 14:07:38.950065 tooldelta-0.5.7/tooldelta/plugin_load/funcs.py
--rwxr-xr-x   0        0        0     9975 2024-04-19 14:07:38.950065 tooldelta-0.5.7/tooldelta/plugin_load/injected_plugin/__init__.py
--rwxr-xr-x   0        0        0     9146 2024-04-19 14:07:38.950065 tooldelta-0.5.7/tooldelta/plugin_load/injected_plugin/movent.py
--rwxr-xr-x   0        0        0    16934 2024-04-19 14:07:38.950065 tooldelta-0.5.7/tooldelta/plugin_manager.py
--rwxr-xr-x   0        0        0    16769 2024-04-19 14:07:38.950065 tooldelta-0.5.7/tooldelta/plugin_market.py
--rw-r--r--   0        0        0     1774 2024-04-19 14:07:38.950065 tooldelta-0.5.7/tooldelta/starter.py
--rwxr-xr-x   0        0        0      808 2024-04-19 14:07:38.950065 tooldelta-0.5.7/tooldelta/sys_args.py
--rwxr-xr-x   0        0        0     9071 2024-04-19 14:07:38.950065 tooldelta-0.5.7/tooldelta/urlmethod.py
--rw-r--r--   0        0        0     3743 1970-01-01 00:00:00.000000 tooldelta-0.5.7/PKG-INFO
+-rwxr-xr-x   0        0        0     1497 2024-04-19 14:15:54.468505 tooldelta-0.5.8/LICENSE
+-rwxr-xr-x   0        0        0     2504 2024-04-19 14:15:54.468505 tooldelta-0.5.8/README.md
+-rwxr-xr-x   0        0        0      973 2024-04-19 14:16:02.764524 tooldelta-0.5.8/pyproject.toml
+-rwxr-xr-x   0        0        0      360 2024-04-19 14:15:54.472505 tooldelta-0.5.8/tooldelta/__init__.py
+-rw-r--r--   0        0        0     4979 2024-04-19 14:15:54.472505 tooldelta-0.5.8/tooldelta/auths.py
+-rwxr-xr-x   0        0        0    19961 2024-04-19 14:15:54.472505 tooldelta-0.5.8/tooldelta/builtins.py
+-rwxr-xr-x   0        0        0    12365 2024-04-19 14:15:54.472505 tooldelta-0.5.8/tooldelta/cfg.py
+-rwxr-xr-x   0        0        0    10889 2024-04-19 14:15:54.472505 tooldelta-0.5.8/tooldelta/color_print.py
+-rw-r--r--   0        0        0     1884 2024-04-19 14:15:54.472505 tooldelta-0.5.8/tooldelta/constants.py
+-rw-r--r--   0        0        0     5870 2024-04-19 14:15:54.472505 tooldelta-0.5.8/tooldelta/fb_conn/fbconn.py
+-rwxr-xr-x   0        0        0    30098 2024-04-19 14:15:54.472505 tooldelta-0.5.8/tooldelta/frame.py
+-rwxr-xr-x   0        0        0     4644 2024-04-19 14:15:54.472505 tooldelta-0.5.8/tooldelta/game_texts.py
+-rwxr-xr-x   0        0        0      476 2024-04-19 14:15:54.472505 tooldelta-0.5.8/tooldelta/get_tool_delta_version.py
+-rwxr-xr-x   0        0        0    20525 2024-04-19 14:15:54.472505 tooldelta-0.5.8/tooldelta/launch_cli.py
+-rwxr-xr-x   0        0        0     1276 2024-04-19 14:15:54.472505 tooldelta-0.5.8/tooldelta/launch_options.py
+-rwxr-xr-x   0        0        0     2425 2024-04-19 14:15:54.472505 tooldelta-0.5.8/tooldelta/logger.py
+-rw-r--r--   0        0        0    30151 2024-04-19 14:15:54.472505 tooldelta-0.5.8/tooldelta/neo_conn.py
+-rwxr-xr-x   0        0        0     1292 2024-04-19 14:15:54.472505 tooldelta-0.5.8/tooldelta/packets.py
+-rwxr-xr-x   0        0        0    15769 2024-04-19 14:15:54.472505 tooldelta-0.5.8/tooldelta/plugin_load/PluginGroup.py
+-rwxr-xr-x   0        0        0     3118 2024-04-19 14:15:54.472505 tooldelta-0.5.8/tooldelta/plugin_load/__init__.py
+-rwxr-xr-x   0        0        0     7341 2024-04-19 14:15:54.472505 tooldelta-0.5.8/tooldelta/plugin_load/classic_plugin/__init__.py
+-rwxr-xr-x   0        0        0      450 2024-04-19 14:15:54.472505 tooldelta-0.5.8/tooldelta/plugin_load/funcs.py
+-rwxr-xr-x   0        0        0     9975 2024-04-19 14:15:54.472505 tooldelta-0.5.8/tooldelta/plugin_load/injected_plugin/__init__.py
+-rwxr-xr-x   0        0        0     9146 2024-04-19 14:15:54.472505 tooldelta-0.5.8/tooldelta/plugin_load/injected_plugin/movent.py
+-rwxr-xr-x   0        0        0    16934 2024-04-19 14:15:54.472505 tooldelta-0.5.8/tooldelta/plugin_manager.py
+-rwxr-xr-x   0        0        0    16769 2024-04-19 14:15:54.472505 tooldelta-0.5.8/tooldelta/plugin_market.py
+-rw-r--r--   0        0        0     1774 2024-04-19 14:15:54.472505 tooldelta-0.5.8/tooldelta/starter.py
+-rwxr-xr-x   0        0        0      808 2024-04-19 14:15:54.472505 tooldelta-0.5.8/tooldelta/sys_args.py
+-rwxr-xr-x   0        0        0     9071 2024-04-19 14:15:54.472505 tooldelta-0.5.8/tooldelta/urlmethod.py
+-rw-r--r--   0        0        0     3743 1970-01-01 00:00:00.000000 tooldelta-0.5.8/PKG-INFO
```

### Comparing `tooldelta-0.5.7/LICENSE` & `tooldelta-0.5.8/LICENSE`

 * *Files identical despite different names*

### Comparing `tooldelta-0.5.7/README.md` & `tooldelta-0.5.8/README.md`

 * *Files identical despite different names*

### Comparing `tooldelta-0.5.7/pyproject.toml` & `tooldelta-0.5.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "Tooldelta"
-version = "0.5.7" # This field is automatically set to the value in the version file
+version = "0.5.8" # This field is automatically set to the value in the version file
 description = "Plugin Loader for NeteaseRentalServer on Panel"
 authors = ["SuperScript-PRC"]
 license = ""
 
 readme = "README.md"
 homepage = "https://github.com/SuperScript-PRC/ToolDelta"
 repository = "https://github.com/SuperScript-PRC/ToolDelta"
```

### Comparing `tooldelta-0.5.7/tooldelta/auths.py` & `tooldelta-0.5.8/tooldelta/auths.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.5.7/tooldelta/builtins.py` & `tooldelta-0.5.8/tooldelta/builtins.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.5.7/tooldelta/cfg.py` & `tooldelta-0.5.8/tooldelta/cfg.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.5.7/tooldelta/color_print.py` & `tooldelta-0.5.8/tooldelta/color_print.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.5.7/tooldelta/constants.py` & `tooldelta-0.5.8/tooldelta/constants.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.5.7/tooldelta/fb_conn/fbconn.py` & `tooldelta-0.5.8/tooldelta/fb_conn/fbconn.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.5.7/tooldelta/frame.py` & `tooldelta-0.5.8/tooldelta/frame.py`

 * *Files 0% similar despite different names*

```diff
@@ -105,15 +105,15 @@
             # 配置文件有误
             r = self.upgrade_cfg()
             if r:
                 Print.print_war("配置文件未升级, 已自动升级, 请重启 ToolDelta")
             else:
                 Print.print_err(f"ToolDelta基本配置有误, 需要更正: {err}")
             raise SystemExit from err
-        if self.serverNumber == "0":
+        if self.serverNumber == 0:
             while 1:
                 try:
                     self.serverNumber = int(input(
                         Print.fmt_info("请输入租赁服号: ", "§b 输入 ")
                     ))
                     self.serverPasswd = (
                         getpass.getpass(
```

### Comparing `tooldelta-0.5.7/tooldelta/game_texts.py` & `tooldelta-0.5.8/tooldelta/game_texts.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.5.7/tooldelta/launch_cli.py` & `tooldelta-0.5.8/tooldelta/launch_cli.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -191,20 +191,20 @@
         Args:
             serverNumber (int): 服务器号
             password (str): 服务器密码
             fbToken (str): 验证服务器Token
             auth_server (str): 验证服务器地址
         """
         super().__init__(serverNumber, password, fbToken, auth_server)
-        neo_conn.load_lib()
         self.status = SysStatus.LOADING
         self.launch_event = threading.Event()
         self.omega: Optional[neo_conn.ThreadOmega] = None
         self.neomg_proc = None
         self.download_libs()
+        neo_conn.load_lib()
         self.status = SysStatus.LAUNCHING
         self.secret_exit_key = ""
 
     def set_omega(self, openat_port: int) -> None:
         """设置 Omega 连接
 
         Args:
```

### Comparing `tooldelta-0.5.7/tooldelta/launch_options.py` & `tooldelta-0.5.8/tooldelta/launch_options.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.5.7/tooldelta/logger.py` & `tooldelta-0.5.8/tooldelta/logger.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.5.7/tooldelta/neo_conn.py` & `tooldelta-0.5.8/tooldelta/neo_conn.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.5.7/tooldelta/packets.py` & `tooldelta-0.5.8/tooldelta/packets.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.5.7/tooldelta/plugin_load/PluginGroup.py` & `tooldelta-0.5.8/tooldelta/plugin_load/PluginGroup.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.5.7/tooldelta/plugin_load/__init__.py` & `tooldelta-0.5.8/tooldelta/plugin_load/__init__.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.5.7/tooldelta/plugin_load/classic_plugin/__init__.py` & `tooldelta-0.5.8/tooldelta/plugin_load/classic_plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.5.7/tooldelta/plugin_load/injected_plugin/__init__.py` & `tooldelta-0.5.8/tooldelta/plugin_load/injected_plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.5.7/tooldelta/plugin_load/injected_plugin/movent.py` & `tooldelta-0.5.8/tooldelta/plugin_load/injected_plugin/movent.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.5.7/tooldelta/plugin_manager.py` & `tooldelta-0.5.8/tooldelta/plugin_manager.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.5.7/tooldelta/plugin_market.py` & `tooldelta-0.5.8/tooldelta/plugin_market.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.5.7/tooldelta/starter.py` & `tooldelta-0.5.8/tooldelta/starter.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.5.7/tooldelta/sys_args.py` & `tooldelta-0.5.8/tooldelta/sys_args.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.5.7/tooldelta/urlmethod.py` & `tooldelta-0.5.8/tooldelta/urlmethod.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.5.7/PKG-INFO` & `tooldelta-0.5.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Tooldelta
-Version: 0.5.7
+Version: 0.5.8
 Summary: Plugin Loader for NeteaseRentalServer on Panel
 Home-page: https://github.com/SuperScript-PRC/ToolDelta
 Author: SuperScript-PRC
 Requires-Python: >=3.9,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: Tooldelta Version: 0.5.7 Summary: Plugin Loader for
+Metadata-Version: 2.1 Name: Tooldelta Version: 0.5.8 Summary: Plugin Loader for
 NeteaseRentalServer on Panel Home-page: https://github.com/SuperScript-PRC/
 ToolDelta Author: SuperScript-PRC Requires-Python: >=3.9,<3.13 Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Programming Language ::
 Python :: 3.12 Requires-Dist: aiohttp (>=3.9.3,<4.0.0) Requires-Dist: colorama
 (>=0.4.6,<0.5.0) Requires-Dist: flask (>=3.0.2,<4.0.0) Requires-Dist: mido
```

