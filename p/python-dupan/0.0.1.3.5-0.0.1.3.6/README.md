# Comparing `tmp/python_dupan-0.0.1.3.5.tar.gz` & `tmp/python_dupan-0.0.1.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_dupan-0.0.1.3.5.tar", max compression
+gzip compressed data, was "python_dupan-0.0.1.3.6.tar", max compression
```

## Comparing `python_dupan-0.0.1.3.5.tar` & `python_dupan-0.0.1.3.6.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rwxr-xr-x   0        0        0     1100 2023-12-31 13:16:43.902936 python_dupan-0.0.1.3.5/LICENSE
--rw-r--r--   0        0        0    97504 2024-04-08 06:45:01.992933 python_dupan-0.0.1.3.5/dupan/__init__.py
--rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 python_dupan-0.0.1.3.5/dupan/py.typed
--rw-r--r--   0        0        0       61 2024-01-01 10:28:23.372962 python_dupan-0.0.1.3.5/dupan/util/__init__.py
--rw-r--r--   0        0        0    13103 2024-01-19 04:25:53.949786 python_dupan-0.0.1.3.5/dupan/util/file.py
--rw-r--r--   0        0        0     1795 2023-12-14 11:01:07.350145 python_dupan-0.0.1.3.5/dupan/util/property.py
--rw-r--r--   0        0        0     2751 2023-12-29 05:26:01.836028 python_dupan-0.0.1.3.5/dupan/util/response.py
--rw-r--r--   0        0        0     6295 2024-01-16 04:33:26.963104 python_dupan-0.0.1.3.5/dupan/util/text.py
--rw-r--r--   0        0        0     2114 2023-12-10 10:45:36.285664 python_dupan-0.0.1.3.5/dupan/util/urlopen.py
--rw-r--r--   0        0        0     1249 2024-04-08 06:45:59.111697 python_dupan-0.0.1.3.5/pyproject.toml
--rw-r--r--   0        0        0    10836 2024-01-17 04:31:26.628554 python_dupan-0.0.1.3.5/readme.md
--rw-r--r--   0        0        0    12069 1970-01-01 00:00:00.000000 python_dupan-0.0.1.3.5/PKG-INFO
+-rwxr-xr-x   0        0        0     1100 2023-12-31 13:16:43.902936 python_dupan-0.0.1.3.6/LICENSE
+-rw-r--r--   0        0        0    96106 2024-04-20 12:24:08.768698 python_dupan-0.0.1.3.6/dupan/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 python_dupan-0.0.1.3.6/dupan/py.typed
+-rw-r--r--   0        0        0       61 2024-01-01 10:28:23.372962 python_dupan-0.0.1.3.6/dupan/util/__init__.py
+-rw-r--r--   0        0        0    13103 2024-01-19 04:25:53.949786 python_dupan-0.0.1.3.6/dupan/util/file.py
+-rw-r--r--   0        0        0     1795 2023-12-14 11:01:07.350145 python_dupan-0.0.1.3.6/dupan/util/property.py
+-rw-r--r--   0        0        0     2751 2023-12-29 05:26:01.836028 python_dupan-0.0.1.3.6/dupan/util/response.py
+-rw-r--r--   0        0        0     6295 2024-01-16 04:33:26.963104 python_dupan-0.0.1.3.6/dupan/util/text.py
+-rw-r--r--   0        0        0     2114 2023-12-10 10:45:36.285664 python_dupan-0.0.1.3.6/dupan/util/urlopen.py
+-rw-r--r--   0        0        0     1249 2024-04-20 12:25:13.879064 python_dupan-0.0.1.3.6/pyproject.toml
+-rw-r--r--   0        0        0    10836 2024-01-17 04:31:26.628554 python_dupan-0.0.1.3.6/readme.md
+-rw-r--r--   0        0        0    12069 1970-01-01 00:00:00.000000 python_dupan-0.0.1.3.6/PKG-INFO
```

### Comparing `python_dupan-0.0.1.3.5/LICENSE` & `python_dupan-0.0.1.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `python_dupan-0.0.1.3.5/dupan/__init__.py` & `python_dupan-0.0.1.3.6/dupan/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -905,21 +905,24 @@
         self.url = url
         self.shorturl = shorturl
         self.password = password
         session = self.session = Session()
         session.headers["Referer"] = url
 
     def __iter__(self, /) -> Iterator[dict]:
-        dq = deque("/")
+        dq: deque[tuple[str, str]] = deque()
         get, put = dq.popleft, dq.append
+        put(("", ""))
         while dq:
-            for file in self.iterdir(get()):
+            dir, dir_relpath = get()
+            for file in self.iterdir(dir):
+                relpath = file["relpath"] = joinpath(dir_relpath, file["server_filename"])
                 yield file
                 if file["isdir"]:
-                    put(file["path"])
+                    put((file["path"], relpath))
 
     @staticmethod
     def _extract_from_url(url: str, /) -> tuple[str, str]:
         urlp = urlparse(url)
         if urlp.scheme and urlp.scheme not in ("http", "https"):
             raise ValueError(f"url 协议只接受 'http' 和 'https'，收到 {urlp.scheme!r}，")
         if urlp.netloc and urlp.netloc != "pan.baidu.com":
@@ -1014,51 +1017,55 @@
                 if not errno:
                     break
                 if errno == -62:
                     data.update(cast(dict[str, str], decaptcha()))
                 else:
                     raise OSError(json)
 
-    def iterdir(self, /, dir="/") -> Iterator[dict]:
+    def iterdir(self, /, dir: str = "/", page: int = 1, num: int = 0) -> Iterator[dict]:
         if dir in ("", "/"):
-            yield from self.list_index()
+            data = self.list_index()
+            if num <= 0 or page <= 0:
+                yield from data
+            else:
+                yield from data[(page-1)*num:page*num]
             return
         if not hasattr(self, "share_uk"):
             self.list_index()
         if not dir.startswith("/"):
             dir = self.root + "/" + dir
-            start_inx = len(dir) + 1
-        elif dir == self.root or dir.startswith(self.root + "/"):
-            start_inx = len(self.root) + 1
-        elif dir == self.root2 or dir.startswith(self.root2 + "/"):
-            start_inx = len(self.root2) + 1
-        else:
-            raise FileNotFoundError(errno.ENOENT, dir)
         api = "https://pan.baidu.com/share/list"
         params = {
             "uk": self.share_uk, 
             "shareid": self.share_id, 
             "order": "other", 
             "desc": 1, 
             "showempty": 0, 
             "clienttype": 0, 
             "web": 1, 
             "page": 1, 
             "num": 100, 
             "dir": dir, 
         }
         get = self.session.get
-        while True:
-            ls = Error.check(get(api, params=params).json())["list"]
-            for file in ls:
-                file["relpath"] = file["path"][start_inx:]
-            yield from ls
-            if len(ls) < 100:
-                return
-            params["page"] += 1
+        if num <= 0 or page <= 0:
+            if num > 0:
+                params["num"] = num
+            else:
+                num = params["num"]
+            while True:
+                ls = Error.check(get(api, params=params).json())["list"]
+                yield from ls
+                if len(ls) < num:
+                    break
+                params["page"] += 1
+        else:
+            params["page"] = page
+            params["num"] = num
+            yield from Error.check(get(api, params=params).json())["list"]
 
     def list_index(self, /, try_times: int = 5) -> list[dict]:
         url = self.url
         password = self.password
         session = self.session
         if try_times <= 0:
             it: Iterator[int] = count()
@@ -1095,68 +1102,19 @@
                         root2 = root2, 
                         share_uk = data["share_uk"], 
                         share_id = data["shareid"], 
                     )
                     return file_list
         raise RuntimeError("too many attempts")
 
-    def listdir(self, /, dir="/", page=1, num=0) -> list[str]:
-        return [a["server_filename"] for a in self.listdir_attr(dir, page, num)]
+    def listdir(self, /, dir: str = "/", page: int = 1, num: int = 0) -> list[str]:
+        return [attr["server_filename"] for attr in self.iterdir(dir, page, num)]
 
-    def listdir_attr(self, /, dir="/", page=1, num=0) -> list[dict]:
-        if dir in ("", "/"):
-            data = self.list_index()
-            if num <= 0:
-                return data
-            if page < 1:
-                page = 1
-            return data[(page-1)*num:page*num]
-        if not hasattr(self, "share_uk"):
-            self.list_index()
-        if not dir.startswith("/"):
-            dir = self.root + "/" + dir
-            start_inx = len(dir) + 1
-        elif dir == self.root or dir.startswith(self.root + "/"):
-            start_inx = len(self.root) + 1
-        elif dir == self.root2 or dir.startswith(self.root2 + "/"):
-            start_inx = len(self.root2) + 1
-        else:
-            raise FileNotFoundError(errno.ENOENT, dir)
-        api = "https://pan.baidu.com/share/list"
-        params = {
-            "uk": self.share_uk, 
-            "shareid": self.share_id, 
-            "order": "other", 
-            "desc": 1, 
-            "showempty": 0, 
-            "clienttype": 0, 
-            "web": 1, 
-            "page": 1, 
-            "num": 100, 
-            "dir": dir, 
-        }
-        session = self.session
-        if num <= 0:
-            ls_all = []
-            while True:
-                ls = Error.check(session.get(api, params=params).json())["list"]
-                ls_all.extend(ls)
-                if len(ls) < 100:
-                    for file in ls_all:
-                        file["relpath"] = file["path"][start_inx:]
-                    return ls_all
-                params["page"] += 1
-        if page > 0:
-            params["page"] = page
-        if num < 100:
-            params["num"] = 100
-        ls = Error.check(session.get(api, params=params).json())["list"]
-        for file in ls:
-            file["relpath"] = file["path"][start_inx:]
-        return ls
+    def listdir_attr(self, /, dir: str = "/", page: int = 1, num: int = 0) -> list[dict]:
+        return list(self.iterdir(dir, page, num))
 
 
 class DuPanPath:
     fs: DuPanFileSystem
     path: str
 
     def __init__(
```

### Comparing `python_dupan-0.0.1.3.5/dupan/util/file.py` & `python_dupan-0.0.1.3.6/dupan/util/file.py`

 * *Files identical despite different names*

### Comparing `python_dupan-0.0.1.3.5/dupan/util/property.py` & `python_dupan-0.0.1.3.6/dupan/util/property.py`

 * *Files identical despite different names*

### Comparing `python_dupan-0.0.1.3.5/dupan/util/response.py` & `python_dupan-0.0.1.3.6/dupan/util/response.py`

 * *Files identical despite different names*

### Comparing `python_dupan-0.0.1.3.5/dupan/util/text.py` & `python_dupan-0.0.1.3.6/dupan/util/text.py`

 * *Files identical despite different names*

### Comparing `python_dupan-0.0.1.3.5/dupan/util/urlopen.py` & `python_dupan-0.0.1.3.6/dupan/util/urlopen.py`

 * *Files identical despite different names*

### Comparing `python_dupan-0.0.1.3.5/pyproject.toml` & `python_dupan-0.0.1.3.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-dupan"
-version = "0.0.1.3.5"
+version = "0.0.1.3.6"
 description = "Python wrapper for `baidu webdisk <https://pan.baidu.com>`."
 authors = ["ChenyangGao <wosiwujm@gmail.com>"]
 license = "MIT"
 readme = "readme.md"
 homepage = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-dupan-client"
 repository = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-dupan-client"
 keywords = ["nas", "dupan", "百度网盘"]
```

### Comparing `python_dupan-0.0.1.3.5/readme.md` & `python_dupan-0.0.1.3.6/readme.md`

 * *Files identical despite different names*

### Comparing `python_dupan-0.0.1.3.5/PKG-INFO` & `python_dupan-0.0.1.3.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-dupan
-Version: 0.0.1.3.5
+Version: 0.0.1.3.6
 Summary: Python wrapper for `baidu webdisk <https://pan.baidu.com>`.
 Home-page: https://github.com/ChenyangGao/web-mount-packs/tree/main/python-dupan-client
 License: MIT
 Keywords: nas,dupan,百度网盘
 Author: ChenyangGao
 Author-email: wosiwujm@gmail.com
 Requires-Python: >=3.10,<4.0
```

