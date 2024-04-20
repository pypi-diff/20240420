# Comparing `tmp/python_115-0.0.6.1.tar.gz` & `tmp/python_115-0.0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_115-0.0.6.1.tar", max compression
+gzip compressed data, was "python_115-0.0.6.2.tar", max compression
```

## Comparing `python_115-0.0.6.1.tar` & `python_115-0.0.6.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rwxr-xr-x   0        0        0     1100 2023-10-11 13:48:41.987287 python_115-0.0.6.1/LICENSE
--rwxr-xr-x   0        0        0   269684 2024-04-19 15:54:42.968152 python_115-0.0.6.1/p115/__init__.py
--rwxr-xr-x   0        0        0      115 2024-04-19 15:21:20.677842 python_115-0.0.6.1/p115/__main__.py
--rwxr-xr-x   0        0        0      161 2024-04-19 14:59:47.539120 python_115-0.0.6.1/p115/cmd/__init__.py
--rwxr-xr-x   0        0        0      336 2024-04-19 15:07:36.047405 python_115-0.0.6.1/p115/cmd/init.py
--rwxr-xr-x   0        0        0     6742 2024-04-19 15:25:32.941526 python_115-0.0.6.1/p115/cmd/iterdir.py
--rwxr-xr-x   0        0        0     1405 2024-04-19 15:22:56.504224 python_115-0.0.6.1/p115/cmd/qrcode.py
--rw-r--r--   0        0        0      179 2023-12-22 08:44:22.766732 python_115-0.0.6.1/p115/exception.py
--rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 python_115-0.0.6.1/p115/py.typed
--rw-r--r--   0        0        0       87 2023-12-19 14:25:03.149217 python_115-0.0.6.1/p115/util/__init__.py
--rw-r--r--   0        0        0     4329 2023-11-24 07:50:22.455279 python_115-0.0.6.1/p115/util/_init_mimetypes.py
--rw-r--r--   0        0        0      360 2024-02-08 06:48:55.081770 python_115-0.0.6.1/p115/util/args.py
--rw-r--r--   0        0        0     7920 2023-12-14 11:02:29.316261 python_115-0.0.6.1/p115/util/cipher.py
--rw-r--r--   0        0        0     5671 2024-04-03 04:46:18.484632 python_115-0.0.6.1/p115/util/concurrent.py
--rw-r--r--   0        0        0    12120 2024-04-03 04:46:18.485585 python_115-0.0.6.1/p115/util/download.py
--rw-r--r--   0        0        0    15103 2024-04-03 05:18:09.304611 python_115-0.0.6.1/p115/util/file.py
--rw-r--r--   0        0        0     4507 2023-12-08 06:07:31.193403 python_115-0.0.6.1/p115/util/hash.py
--rw-r--r--   0        0        0    10070 2024-01-12 05:37:18.775493 python_115-0.0.6.1/p115/util/ignore.py
--rw-r--r--   0        0        0     2822 2024-02-13 03:37:52.593362 python_115-0.0.6.1/p115/util/iter.py
--rw-r--r--   0        0        0     4562 2024-01-16 05:10:10.057134 python_115-0.0.6.1/p115/util/path.py
--rw-r--r--   0        0        0     1794 2024-01-15 14:50:38.503730 python_115-0.0.6.1/p115/util/property.py
--rw-r--r--   0        0        0     3190 2024-01-29 10:59:02.879730 python_115-0.0.6.1/p115/util/response.py
--rw-r--r--   0        0        0     6122 2024-01-15 15:35:49.895519 python_115-0.0.6.1/p115/util/retry.py
--rw-r--r--   0        0        0     6785 2024-02-09 07:54:09.097617 python_115-0.0.6.1/p115/util/text.py
--rw-r--r--   0        0        0       43 2024-04-03 05:08:27.538028 python_115-0.0.6.1/p115/util/upload.py
--rw-r--r--   0        0        0    10029 2024-01-29 10:52:22.271824 python_115-0.0.6.1/p115/util/urlopen.py
--rw-r--r--   0        0        0     1272 2024-04-19 17:10:12.938195 python_115-0.0.6.1/pyproject.toml
--rw-r--r--   0        0        0    34641 2024-01-05 10:56:58.191328 python_115-0.0.6.1/readme.md
--rw-r--r--   0        0        0    35896 1970-01-01 00:00:00.000000 python_115-0.0.6.1/PKG-INFO
+-rwxr-xr-x   0        0        0     1100 2023-10-11 13:48:41.987287 python_115-0.0.6.2/LICENSE
+-rwxr-xr-x   0        0        0   273345 2024-04-20 16:48:30.143243 python_115-0.0.6.2/p115/__init__.py
+-rwxr-xr-x   0        0        0      115 2024-04-19 15:21:20.677842 python_115-0.0.6.2/p115/__main__.py
+-rwxr-xr-x   0        0        0      161 2024-04-19 14:59:47.539120 python_115-0.0.6.2/p115/cmd/__init__.py
+-rwxr-xr-x   0        0        0      336 2024-04-19 15:07:36.047405 python_115-0.0.6.2/p115/cmd/init.py
+-rwxr-xr-x   0        0        0     6742 2024-04-19 15:25:32.941526 python_115-0.0.6.2/p115/cmd/iterdir.py
+-rwxr-xr-x   0        0        0     1405 2024-04-19 15:22:56.504224 python_115-0.0.6.2/p115/cmd/qrcode.py
+-rw-r--r--   0        0        0      179 2023-12-22 08:44:22.766732 python_115-0.0.6.2/p115/exception.py
+-rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 python_115-0.0.6.2/p115/py.typed
+-rw-r--r--   0        0        0       87 2023-12-19 14:25:03.149217 python_115-0.0.6.2/p115/util/__init__.py
+-rw-r--r--   0        0        0     4329 2023-11-24 07:50:22.455279 python_115-0.0.6.2/p115/util/_init_mimetypes.py
+-rw-r--r--   0        0        0      360 2024-02-08 06:48:55.081770 python_115-0.0.6.2/p115/util/args.py
+-rw-r--r--   0        0        0     7920 2023-12-14 11:02:29.316261 python_115-0.0.6.2/p115/util/cipher.py
+-rw-r--r--   0        0        0     5671 2024-04-03 04:46:18.484632 python_115-0.0.6.2/p115/util/concurrent.py
+-rw-r--r--   0        0        0    12120 2024-04-03 04:46:18.485585 python_115-0.0.6.2/p115/util/download.py
+-rw-r--r--   0        0        0    15103 2024-04-03 05:18:09.304611 python_115-0.0.6.2/p115/util/file.py
+-rw-r--r--   0        0        0     4507 2023-12-08 06:07:31.193403 python_115-0.0.6.2/p115/util/hash.py
+-rw-r--r--   0        0        0    10070 2024-01-12 05:37:18.775493 python_115-0.0.6.2/p115/util/ignore.py
+-rw-r--r--   0        0        0     2822 2024-02-13 03:37:52.593362 python_115-0.0.6.2/p115/util/iter.py
+-rw-r--r--   0        0        0     4562 2024-01-16 05:10:10.057134 python_115-0.0.6.2/p115/util/path.py
+-rw-r--r--   0        0        0     1794 2024-01-15 14:50:38.503730 python_115-0.0.6.2/p115/util/property.py
+-rw-r--r--   0        0        0     3190 2024-01-29 10:59:02.879730 python_115-0.0.6.2/p115/util/response.py
+-rw-r--r--   0        0        0     6122 2024-01-15 15:35:49.895519 python_115-0.0.6.2/p115/util/retry.py
+-rw-r--r--   0        0        0     6785 2024-02-09 07:54:09.097617 python_115-0.0.6.2/p115/util/text.py
+-rw-r--r--   0        0        0       43 2024-04-03 05:08:27.538028 python_115-0.0.6.2/p115/util/upload.py
+-rw-r--r--   0        0        0    10029 2024-01-29 10:52:22.271824 python_115-0.0.6.2/p115/util/urlopen.py
+-rw-r--r--   0        0        0     1272 2024-04-20 16:48:36.360398 python_115-0.0.6.2/pyproject.toml
+-rw-r--r--   0        0        0    34641 2024-01-05 10:56:58.191328 python_115-0.0.6.2/readme.md
+-rw-r--r--   0        0        0    35896 1970-01-01 00:00:00.000000 python_115-0.0.6.2/PKG-INFO
```

### Comparing `python_115-0.0.6.1/LICENSE` & `python_115-0.0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `python_115-0.0.6.1/p115/__init__.py` & `python_115-0.0.6.2/p115/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python3
 # encoding: utf-8
 
 from __future__ import annotations
 
 __author__ = "ChenyangGao <https://chenyanggao.github.io>"
-__version__ = (0, 0, 5)
+__version__ = (0, 0, 6)
 __all__ = [
     "P115Client", "P115Path", "P115FileSystem", "P115SharePath", "P115ShareFileSystem", 
     "P115ZipPath", "P115ZipFileSystem", "P115Offline", "P115Recyclebin", "P115Sharing", 
 ]
 
 import errno
 
@@ -94,31 +94,58 @@
 ECDH_ENCODER: Final = P115ECDHCipher()
 
 if not hasattr(Response, "__del__"):
     Response.__del__ = Response.close # type: ignore
 
 
 def check_response(fn: RequestVarT, /) -> RequestVarT:
-    if isinstance(fn, dict):
-        resp = fn
-        if not resp.get("state", True):
+    def check(resp: dict):
+        if resp.get("state"):
+            return resp
+        if "errno" in resp:
+            match resp["errno"]:
+                # {'state': False, 'error': '该目录名称已存在。', 'errno': 20004, 'errtype': 'war'}
+                case 20004:
+                    raise FileExistsError(resp)
+                # {'state': False, 'error': '父目录不存在。', 'errno': 20009, 'errtype': 'war'}
+                case 20009:
+                    raise FileNotFoundError(resp)
+                # {'state': False, 'error': '不能将文件复制到自身或其子目录下。', 'errno': 91002, 'errtype': 'war'}
+                case 91002:
+                    raise OSError(errno.ENOTSUP, resp)
+                # {'state': False, 'error': '操作的文件(夹)数量超过5万个', 'errno': 91004, 'errtype': 'war'}
+                case 91004:
+                    raise OSError(errno.ENOTSUP, resp)
+                # {'state': False, 'error': '空间不足，复制失败。', 'errno': 91005, 'errtype': 'war'}
+                case 91005:
+                    raise OSError(errno.ENOSPC, resp)
+                # {'state': False, 'error': '文件（夹）不存在或已经删除。', 'errno': 90008, 'errtype': 'war'}
+                case 90008:
+                    raise FileNotFoundError(resp)
+                # {'state': False, 'error': '文件已删除，请勿重复操作', 'errno': 231011, 'errtype': 'war'}
+                case 231011:
+                    raise FileNotFoundError(resp)
+                # {'state': False, 'error': '删除[...]操作尚未执行完成，请稍后再试！', 'errno': 990009, 'errtype': 'war'}
+                # {'state': False, 'error': '还原[...]操作尚未执行完成，请稍后再试！', 'errno': 990009, 'errtype': 'war'}
+                # {'state': False, 'error': '复制[...]操作尚未执行完成，请稍后再试！', 'errno': 990009, 'errtype': 'war'}
+                # {'state': False, 'error': '移动[...]操作尚未执行完成，请稍后再试！', 'errno': 990009, 'errtype': 'war'}
+                case 990009:
+                    raise OSError(errno.EBUSY, resp)
+                # {'state': False, 'error': '操作的文件(夹)数量超过5万个', 'errno': 990023, 'errtype': ''}
+                case 990023:
+                    raise OSError(errno.ENOTSUP, resp)
             raise OSError(errno.EIO, resp)
-        return fn
+    if isinstance(fn, dict):
+        return check(fn)
     elif iscoroutinefunction(fn):
         async def wrapper(*args, **kwds):
-            resp = await fn(*args, **kwds)
-            if not resp.get("state", True):
-                raise OSError(errno.EIO, resp)
-            return resp
+            return check(await fn(*args, **kwds))
     elif callable(fn):
         def wrapper(*args, **kwds):
-            resp = fn(*args, **kwds)
-            if not resp.get("state", True):
-                raise OSError(errno.EIO, resp)
-            return resp
+            return check(fn(*args, **kwds))
     else:
         raise TypeError
     return update_wrapper(wrapper, fn)
 
 
 def console_qrcode(text: str) -> None:
     qr = qrcode.QRCode(border=1)
@@ -645,116 +672,127 @@
         POST https://webapi.115.com/user/space_summury
         """
         api = "https://webapi.115.com/user/space_summury"
         return self.request(api, "POST", async_=async_, **request_kwargs)
 
     def fs_batch_copy(
         self, 
-        payload: dict, 
+        payload: dict | Iterable[int | str], 
         /, 
+        pid: int = 0, 
         async_: bool = False, 
         **request_kwargs, 
     ) -> dict:
         """复制文件或文件夹
         POST https://webapi.115.com/files/copy
         payload:
             - pid: int | str
             - fid[0]: int | str
             - fid[1]: int | str
             - ...
         """
         api = "https://webapi.115.com/files/copy"
+        if isinstance(payload, dict):
+            payload = {"pid": pid, **payload}
+        else:
+            payload = {f"fid[{fid}]": fid for i, fid in enumerate(payload)}
+            if not payload:
+                return {"state": False, "message": "no op"}
+            payload["pid"] = pid
         return self.request(api, "POST", data=payload, async_=async_, **request_kwargs)
 
     def fs_batch_delete(
         self, 
-        payload: dict, 
+        payload: dict | Iterable[int | str], 
         /, 
         async_: bool = False, 
         **request_kwargs, 
     ) -> dict:
         """删除文件或文件夹
         POST https://webapi.115.com/rb/delete
         payload:
             - fid[0]: int | str
             - fid[1]: int | str
             - ...
         """
         api = "https://webapi.115.com/rb/delete"
+        if not isinstance(payload, dict):
+            payload = {f"fid[{i}]": fid for i, fid in enumerate(payload)}
+        if not payload:
+            return {"state": False, "message": "no op"}
         return self.request(api, "POST", data=payload, async_=async_, **request_kwargs)
 
     def fs_batch_move(
         self, 
-        payload: dict, 
+        payload: dict | Iterable[int | str], 
         /, 
+        pid: int = 0, 
         async_: bool = False, 
         **request_kwargs, 
     ) -> dict:
         """移动文件或文件夹
         POST https://webapi.115.com/files/move
         payload:
             - pid: int | str
             - fid[0]: int | str
             - fid[1]: int | str
             - ...
         """
         api = "https://webapi.115.com/files/move"
+        if isinstance(payload, dict):
+            payload = {"pid": pid, **payload}
+        else:
+            payload = {f"fid[{i}]": fid for i, fid in enumerate(payload)}
+            if not payload:
+                return {"state": False, "message": "no op"}
+            payload["pid"] = pid
         return self.request(api, "POST", data=payload, async_=async_, **request_kwargs)
 
     def fs_batch_rename(
         self, 
-        payload: dict, 
+        payload: dict | Iterable[tuple[int | str, str]], 
         /, 
         async_: bool = False, 
         **request_kwargs, 
     ) -> dict:
         """重命名文件或文件夹
         POST https://webapi.115.com/files/batch_rename
         payload:
             - files_new_name[{file_id}]: str # 值为新的文件名（basename）
         """
         api = "https://webapi.115.com/files/batch_rename"
+        if not isinstance(payload, dict):
+            payload = {f"files_new_name[{fid}]": name for fid, name in payload}
+        if not payload:
+            return {"state": False, "message": "no op"}
         return self.request(api, "POST", data=payload, async_=async_, **request_kwargs)
 
     def fs_copy(
         self, 
-        fids: int | str | Iterable[int | str], 
+        id: int | str, 
         /, 
-        pid: int, 
+        pid: int = 0, 
         async_: bool = False, 
         **request_kwargs, 
     ) -> dict:
         """复制文件或文件夹，此接口是对 `fs_batch_copy` 的封装
         """
-        if isinstance(fids, (int, str)):
-            payload = {"fid[0]": fids}
-        else:
-            payload = {f"fid[{fid}]": fid for i, fid in enumerate(fids)}
-            if not payload:
-                return {"state": False, "message": "no op"}
-        payload["pid"] = pid
-        return self.fs_batch_copy(payload, async_=async_, **request_kwargs)
+        return self.fs_batch_copy({"fid[0]": id, "pid": pid}, async_=async_, **request_kwargs)
 
     def fs_delete(
         self, 
-        fids: int | str | Iterable[int | str], 
+        id: int | str, 
         /, 
         async_: bool = False, 
         **request_kwargs, 
     ) -> dict:
         """删除文件或文件夹，此接口是对 `fs_batch_delete` 的封装
         """
         api = "https://webapi.115.com/rb/delete"
-        if isinstance(fids, (int, str)):
-            payload = {"fid[0]": fids}
-        else:
-            payload = {f"fid[{i}]": fid for i, fid in enumerate(fids)}
-            if not payload:
-                return {"state": False, "message": "no op"}
-        return self.fs_batch_delete(payload, async_=async_, **request_kwargs)
+        return self.fs_batch_delete({"fid[0]": id}, async_=async_, **request_kwargs)
 
     def fs_file(
         self, 
         payload: int | str | dict, 
         /, 
         async_: bool = False, 
         **request_kwargs, 
@@ -1063,42 +1101,35 @@
             payload = {"pid": 0, "cname": payload}
         else:
             payload = {"pid": 0, **payload}
         return self.request(api, "POST", data=payload, async_=async_, **request_kwargs)
 
     def fs_move(
         self, 
-        fids: int | str | Iterable[int | str], 
+        id: int | str, 
         /, 
         pid: int = 0, 
         async_: bool = False, 
         **request_kwargs, 
     ) -> dict:
         """移动文件或文件夹，此接口是对 `fs_batch_move` 的封装
         """
-        if isinstance(fids, (int, str)):
-            payload = {"fid[0]": fids}
-        else:
-            payload = {f"fid[{i}]": fid for i, fid in enumerate(fids)}
-            if not payload:
-                return {"state": False, "message": "no op"}
-        payload["pid"] = pid
-        return self.fs_batch_move(payload, async_=async_, **request_kwargs)
+        return self.fs_batch_move({"fid[0]": id, "pid": pid}, async_=async_, **request_kwargs)
 
     def fs_rename(
         self, 
-        fid_name_pairs: Iterable[tuple[int | str, str]], 
+        id: int, 
+        name: str, 
         /, 
         async_: bool = False, 
         **request_kwargs, 
     ) -> dict:
         """重命名文件或文件夹，此接口是对 `fs_batch_rename` 的封装
         """
-        payload = {f"files_new_name[{fid}]": name for fid, name in fid_name_pairs}
-        return self.fs_batch_rename(payload, async_=async_, **request_kwargs)
+        return self.fs_batch_rename({f"files_new_name[{id}]": name}, async_=async_, **request_kwargs)
 
     def fs_search(
         self, 
         payload: str | dict, 
         /, 
         async_: bool = False, 
         **request_kwargs, 
@@ -5606,22 +5637,82 @@
         app: str = "web", 
         **kwargs, 
     ) -> Self:
         kwargs["client"] = P115Client(cookie, login_app=app)
         return cls(**kwargs)
 
     @check_response
-    def _copy(self, id: int, pid: int = 0, /) -> dict:
+    def fs_mkdir(self, name: str, /, pid: int = 0) -> dict:
+        return self.client.fs_mkdir({"cname": name, "pid": pid})
+
+    @check_response
+    def fs_copy(self, id: int, /, pid: int = 0) -> dict:
         return self.client.fs_copy(id, pid)
 
     @check_response
-    def _delete(self, id: int, /) -> dict:
+    def fs_delete(self, id: int, /) -> dict:
         return self.client.fs_delete(id)
 
-    def _files(
+    @check_response
+    def fs_move(self, id: int, /, pid: int = 0) -> dict:
+        return self.client.fs_move(id, pid)
+
+    @check_response
+    def fs_rename(self, id: int, name: str, /) -> dict:
+        return self.client.fs_rename(id, name)
+
+    @check_response
+    def fs_batch_copy(
+        self, 
+        payload: dict | Iterable[int | str], 
+        /, 
+        pid: int = 0, 
+    ) -> dict:
+        return self.client.fs_batch_copy(payload, pid)
+
+    @check_response
+    def fs_batch_delete(
+        self, 
+        payload: dict | Iterable[int | str], 
+        /, 
+    ) -> dict:
+        return self.client.fs_batch_delete(payload)
+
+    @check_response
+    def fs_batch_move(
+        self, 
+        payload: dict | Iterable[int | str], 
+        /, 
+        pid: int = 0, 
+    ) -> dict:
+        return self.client.fs_batch_move(payload, pid)
+
+    @check_response
+    def fs_batch_rename(
+        self, 
+        payload: dict | Iterable[tuple[int | str, str]], 
+        /, 
+    ) -> dict:
+        return self.client.fs_batch_rename(payload)
+
+    def fs_info(self, id: int, /) -> dict:
+        result = self.client.fs_info({"file_id": id})
+        if result["state"]:
+            return result
+        match result["code"]:
+            # {'state': False, 'code': 20018, 'message': '文件不存在或已删除。'}
+            case 20018:
+                raise FileNotFoundError(result)
+            # {'state': False, 'code': 990002, 'message': '参数错误。'}
+            case 990002:
+                raise OSError(errno.EINVAL, result)
+            case _:
+                raise OSError(errno.EIO, result)
+
+    def fs_files(
         self, 
         /, 
         id: int = 0, 
         limit: int = 32, 
         offset: int = 0, 
     ) -> dict:
         resp = check_response(self.client.fs_files({
@@ -5631,31 +5722,15 @@
             "show_dir": 1, 
         }))
         if id and int(resp["path"][-1]["cid"]) != id:
             raise NotADirectoryError(errno.ENOTDIR, f"{id} is not a directory")
         return resp
 
     @check_response
-    def _info(self, id: int, /) -> dict:
-        return self.client.fs_info({"file_id": id})
-
-    @check_response
-    def _mkdir(self, name: str, pid: int = 0, /) -> dict:
-        return self.client.fs_mkdir({"cname": name, "pid": pid})
-
-    @check_response
-    def _move(self, id: int, pid: int = 0, /) -> dict:
-        return self.client.fs_move(id, pid)
-
-    @check_response
-    def _rename(self, id: int, name: str, /) -> dict:
-        return self.client.fs_rename([(id, name)])
-
-    @check_response
-    def _search(self, payload: dict, /) -> dict:
+    def fs_search(self, payload: str | dict, /) -> dict:
         return self.client.fs_search(payload)
 
     @check_response
     def space_summury(self, /) -> dict:
         return self.client.fs_space_summury()
 
     def _upload(self, file, name, pid: int = 0) -> dict:
@@ -5666,22 +5741,22 @@
                 pass
             else:
                 resp = self.client.upload_file(file, name, pid)
                 name = resp["data"]["file_name"]
                 try:
                     return self._attr_path([name], pid)
                 except FileNotFoundError:
-                    self._files(pid, 1)
+                    self.fs_files(pid, 1)
                     return self._attr_path([name], pid)
         resp = check_response(self.client.upload_file_sample)(file, name, pid)
         id = int(resp["data"]["file_id"])
         try:
             return self._attr(id)
         except FileNotFoundError:
-            self._files(pid, 1)
+            self.fs_files(pid, 1)
             return self._attr(id)
 
     def _clear_cache(self, attr: dict, /):
         attr_cache = self.attr_cache
         if attr_cache is None:
             return
         id = attr["id"]
@@ -5848,15 +5923,15 @@
                                 try:
                                     del path_to_id[old_attr["path"]]
                                 except LookupError:
                                     pass
                             old_attr.update(attr)
                 return attr
             def iterdir():
-                get_files = self._files
+                get_files = self.fs_files
                 resp = get_files(id, limit=pagesize)
                 dirname = joins(("", *(a["name"] for a in resp["path"][1:])))
                 if path_to_id is not None:
                     path_to_id[dirname] = id
                 last_update = datetime.now()
                 count = resp["count"]
                 for attr in resp["data"]:
@@ -5896,15 +5971,15 @@
         if attr_cache is None:
             attrs = None
         else:
             attrs = attr_cache.get(id)
         if attrs and "attr" in attrs and get_version is None:
             return attrs["attr"]
         try:
-            data = self._info(id)["data"][0]
+            data = self.fs_info(id)["data"][0]
         except OSError as e:
             raise FileNotFoundError(errno.ENOENT, f"no such id: {id!r}") from e
         attr = normalize_info(data, fs=self, last_update=datetime.now())
         pid = attr["parent_id"]
         attr_old = None
         if attr_cache is not None:
             if get_version is None:
@@ -6077,40 +6152,40 @@
             elif overwrite_or_ignore is None:
                 raise FileExistsError(
                     errno.EEXIST, 
                     f"destination already exists: {src_fullpath!r} -> {dst_fullpath!r}", 
                 )
             elif not overwrite_or_ignore:
                 return None
-            self._delete(dst_attr["id"])
+            self.fs_delete(dst_attr["id"])
             dst_pid = dst_attr["parent_id"]
         src_id = src_attr["id"]
         if splitext(src_name)[1] != splitext(dst_name)[1]:
             dst_name = check_response(self.client.upload_file_init)(
                 dst_name, 
                 filesize=src_attr["size"], 
                 file_sha1=src_attr["sha1"], 
                 read_range_bytes_or_hash=lambda rng: self.read_bytes_range(src_id, rng), 
                 pid=dst_pid, 
             )["data"]["file_name"]
             return self.attr([dst_name], dst_pid)
         elif src_name == dst_name:
-            self._copy(src_id, dst_pid)
+            self.fs_copy(src_id, dst_pid)
             return self.attr([src_name], dst_pid)
         else:
-            tempdir_id = int(self._mkdir(str(uuid4()))["cid"])
+            tempdir_id = int(self.fs_mkdir(str(uuid4()))["cid"])
             try:
-                self._copy(src_id, tempdir_id)
+                self.fs_copy(src_id, tempdir_id)
                 dst_id = self.attr([src_name], tempdir_id)["id"]
-                resp = self._rename(dst_id, dst_name)
+                resp = self.fs_rename(dst_id, dst_name)
                 if resp["data"]:
                     dst_name = resp["data"][str(dst_id)]
-                self._move(dst_id, dst_pid)
+                self.fs_move(dst_id, dst_pid)
             finally:
-                self._delete(tempdir_id)
+                self.fs_delete(tempdir_id)
             return self.attr(dst_id)
 
     def copytree(
         self, 
         /, 
         src_path: IDOrPathType, 
         dst_path: IDOrPathType = "", 
@@ -6140,15 +6215,15 @@
             if len(dst_patht) == 1:
                 dst_attr = self.attr(0)
                 dst_id = 0
             else:
                 dst_attr = self.makedirs(dst_patht[:-1], exist_ok=True)
                 dst_id = dst_attr["id"]
                 if src_name == dst_patht[-1]:
-                    self._copy(src_id, dst_id)
+                    self.fs_copy(src_id, dst_id)
                     return self.attr([src_name], dst_id)
                 dst_attr = self.makedirs([src_name], dst_id, exist_ok=True)
                 dst_id = dst_attr["id"]
         else:
             dst_id = dst_attr["id"]
             dst_fullpath = dst_attr["path"]
             if src_fullpath == dst_fullpath:
@@ -6192,15 +6267,15 @@
         return self.attr(dst_attr["id"])
 
     def _dir_get_ancestors(self, id: int, /) -> list[dict]:
         ls = [{"name": "", "id": 0, "parent_id": 0, "is_directory": True}]
         if id:
             ls.extend(
                 {"name": p["name"], "id": int(p["cid"]), "parent_id": int(p["pid"]), "is_directory": True} 
-                for p in self._files(id, limit=1)["path"][1:]
+                for p in self.fs_files(id, limit=1)["path"][1:]
             )
         return ls
 
     def get_ancestors(
         self, 
         id_or_path: IDOrPathType = "", 
         /, 
@@ -6213,15 +6288,15 @@
 
     def get_directory_capacity(
         self, 
         id_or_path: IDOrPathType, 
         /, 
         pid: Optional[int] = None, 
     ) -> int:
-        return self._files(self.get_id(id_or_path, pid), limit=1)["count"]
+        return self.fs_files(self.get_id(id_or_path, pid), limit=1)["count"]
 
     def get_id_from_pickcode(self, /, pickcode: str = "") -> int:
         if not pickcode:
             return 0
         data = self.get_info_from_pickcode(pickcode)
         for fid in data:
             return int(fid)
@@ -6309,15 +6384,15 @@
             return get_attr(0)
         exists = False
         for name in patht:
             try:
                 attr = get_attr([name], pid)
             except FileNotFoundError:
                 exists = False
-                resp = self._mkdir(name, pid)
+                resp = self.fs_mkdir(name, pid)
                 pid = int(resp["cid"])
                 attr = get_attr(pid)
             else:
                 exists = True
                 if not attr["is_directory"]:
                     raise NotADirectoryError(errno.ENOTDIR, f"{path!r} (in {pid!r}): there is a superior non-directory")
                 pid = attr["id"]
@@ -6354,15 +6429,15 @@
                 if not attr["is_directory"]:
                     raise NotADirectoryError(errno.ENOTDIR, f"{attr['id']!r} ({name!r} in {pid!r}) not a directory")
                 pid = attr["id"]
         else:
             raise FileExistsError(errno.EEXIST, f"{path!r} (in {pid!r}) already exists")
         if i < len(patht):
             raise FileNotFoundError(errno.ENOENT, f"{path!r} (in {pid!r}) missing superior directory")
-        resp = self._mkdir(name, pid)
+        resp = self.fs_mkdir(name, pid)
         return self.attr(int(resp["cid"]))
 
     def move(
         self, 
         /, 
         src_path: IDOrPathType, 
         dst_path: IDOrPathType, 
@@ -6379,15 +6454,15 @@
             return None
         if any(a["id"] == src_id for a in self.get_ancestors(dst_id)):
             raise PermissionError(errno.EPERM, f"move a path to its subordinate path is not allowed: {src_id!r} -> {dst_id!r}")
         if dst_attr["is_directory"]:
             name = src_attr["name"]
             if self.exists([name], dst_id):
                 raise FileExistsError(errno.EEXIST, f"destination {name!r} (in {dst_id!r}) already exists")
-            self._move(src_id, dst_id)
+            self.fs_move(src_id, dst_id)
             new_attr = self.attr(src_id)
             self._update_cache_path(src_attr, new_attr)
             return new_attr
         raise FileExistsError(errno.EEXIST, f"destination {dst_id!r} already exists")
 
     # TODO: 由于 115 网盘不支持删除里面有超过 5 万个文件等文件夹，因此需要增加参数，支持在失败后，拆分任务，返回一个 Future 对象，可以获取已完成和未完成，并且可以随时取消
     def remove(
@@ -6402,18 +6477,18 @@
         clear_cache = self._clear_cache
         if attr["is_directory"]:
             if not recursive:
                 raise IsADirectoryError(errno.EISDIR, f"{id_or_path!r} (in {pid!r}) is a directory")
             if id == 0:
                 for subattr in self.iterdir(0):
                     cid = subattr["id"]
-                    self._delete(cid)
+                    self.fs_delete(cid)
                     clear_cache(subattr)
                 return attr
-        self._delete(id)
+        self.fs_delete(id)
         clear_cache(attr)
         return attr
 
     def removedirs(
         self, 
         id_or_path: IDOrPathType, 
         /, 
@@ -6424,30 +6499,30 @@
         except FileNotFoundError:
             return None
         if not attr["is_directory"]:
             raise NotADirectoryError(errno.ENOTDIR, f"{attr['path']!r} (id={attr['id']!r}) is not a directory")
         delid = 0
         pid = attr["id"]
         pattr = attr
-        get_files = self._files
+        get_files = self.fs_files
         while pid:
             files = get_files(pid, limit=1)
             if files["count"] > 1:
                 break
             delid = pid
             pid = int(files["path"][-1]["pid"])
             pattr = {
                 "id": delid, 
                 "parent_id": pid, 
                 "is_directory": True, 
                 "path": "/" + joins([p["name"] for p in files["path"][1:]]), 
             }
         if delid == 0:
             return None
-        self._delete(delid)
+        self.fs_delete(delid)
         self._clear_cache(pattr)
         return attr
 
     # TODO: 支持 dst_path 从 src_path 开始的相对路径
     def rename(
         self, 
         /, 
@@ -6479,63 +6554,63 @@
                 self._update_cache_path(src_attr, new_attr)
                 return new_attr
             return None
         try:
             dst_attr = self.attr(dst_path, pid)
         except FileNotFoundError:
             if src_dirt == dst_dirt and (src_attr["is_directory"] or src_ext == dst_ext):
-                return get_result(self._rename(src_id, dst_name))
+                return get_result(self.fs_rename(src_id, dst_name))
             destdir_attr = self.attr(dst_dirt)
             if not destdir_attr["is_directory"]:
                 raise NotADirectoryError(errno.ENOTDIR, f"parent path {joins(dst_dirt)!r} is not directory: {src_fullpath!r} -> {dst_fullpath!r}")
             dst_pid = destdir_attr["id"]
         else:
             if replace:
                 if src_attr["is_directory"]:
                     if dst_attr["is_directory"]:
                         if self.get_directory_capacity(dst_attr["id"]):
                             raise OSError(errno.ENOTEMPTY, f"source is directory, but destination is non-empty directory: {src_fullpath!r} -> {dst_fullpath!r}")
                     else:
                         raise NotADirectoryError(errno.ENOTDIR, f"source is directory, but destination is not a directory: {src_fullpath!r} -> {dst_fullpath!r}")
                 elif dst_attr["is_directory"]:
                     raise IsADirectoryError(errno.EISDIR, f"source is file, but destination is directory: {src_fullpath!r} -> {dst_fullpath!r}")
-                self._delete(dst_attr["id"])
+                self.fs_delete(dst_attr["id"])
             else:
                 raise FileExistsError(errno.EEXIST, f"destination already exists: {src_fullpath!r} -> {dst_fullpath!r}")
             dst_pid = dst_attr["parent_id"]
         if not (src_attr["is_directory"] or src_ext == dst_ext):
             name = check_response(self.client.upload_file_init)(
                 dst_name, 
                 filesize=src_attr["size"], 
                 file_sha1=src_attr["sha1"], 
                 read_range_bytes_or_hash=lambda rng: self.read_bytes_range(src_id, rng), 
                 pid=dst_pid, 
             )["data"]["file_name"]
-            self._delete(src_id)
+            self.fs_delete(src_id)
             new_attr = self._attr_path([name], dst_pid)
             self._update_cache_path(src_attr, new_attr)
             return new_attr
         if src_name == dst_name:
-            self._move(src_id, dst_pid)
+            self.fs_move(src_id, dst_pid)
             new_attr = self._attr(src_id)
             self._update_cache_path(src_attr, new_attr)
             return new_attr
         elif src_dirt == dst_dirt:
-            return get_result(self._rename(src_id, dst_name))
+            return get_result(self.fs_rename(src_id, dst_name))
         else:
-            self._rename(src_id, str(uuid4()))
+            self.fs_rename(src_id, str(uuid4()))
             try:
-                self._move(src_id, dst_pid)
+                self.fs_move(src_id, dst_pid)
                 try:
-                    return get_result(self._rename(src_id, dst_name))
+                    return get_result(self.fs_rename(src_id, dst_name))
                 except:
-                    self._move(src_id, src_attr["parent_id"])
+                    self.fs_move(src_id, src_attr["parent_id"])
                     raise
             except:
-                self._rename(src_id, src_name)
+                self.fs_rename(src_id, src_name)
                 raise
 
     def renames(
         self, 
         /, 
         src_path: IDOrPathType, 
         dst_path: IDOrPathType, 
@@ -6564,17 +6639,17 @@
     ) -> dict:
         attr = self.attr(id_or_path, pid)
         id = attr["id"]
         if id == 0:
             raise PermissionError(errno.EPERM, "remove the root directory is not allowed")
         elif not attr["is_directory"]:
             raise NotADirectoryError(errno.ENOTDIR, f"{id_or_path!r} (in {pid!r}) is not a directory")
-        elif self._files(id, limit=1)["count"]:
+        elif self.fs_files(id, limit=1)["count"]:
             raise OSError(errno.ENOTEMPTY, f"directory is not empty: {id_or_path!r} (in {pid!r})")
-        self._delete(id)
+        self.fs_delete(id)
         self._clear_cache(attr) 
         return attr
 
     def rmtree(
         self, 
         id_or_path: IDOrPathType, 
         /, 
@@ -6599,15 +6674,15 @@
             "limit": page_size, 
             "offset": offset, 
             **kwargs, 
         }
         def wrap(attr):
             attr = normalize_info(attr, fs=self, last_update=last_update)
             return P115Path(attr)
-        search = self._search
+        search = self.fs_search
         while True:
             resp = search(payload)
             last_update = datetime.now()
             if resp["offset"] != offset:
                 break
             data = resp["data"]
             if not data:
@@ -6698,15 +6773,15 @@
             else:
                 if overwrite_or_ignore is None:
                     raise FileExistsError(errno.EEXIST, f"{path!r} (in {pid!r}) exists")
                 elif attr["is_directory"]:
                     raise IsADirectoryError(errno.EISDIR, f"{path!r} (in {pid!r}) is a directory")
                 elif not overwrite_or_ignore:
                     return attr
-                self._delete(attr["id"])
+                self.fs_delete(attr["id"])
         return self._upload(fio, name, pid)
 
     # TODO: 为了提升速度，之后会支持多线程上传，以及直接上传不做检查
     # TODO: 返回上传任务的迭代器，包含进度相关信息，以及最终的响应信息
     # TODO: 增加参数，onerror, predicate, submit 等
     def upload_tree(
         self, 
@@ -6850,15 +6925,15 @@
     ) -> Self:
         return cls(P115Client(cookie, login_app=app), share_link)
 
     def set_receive_code(self, code: str, /):
         self.__dict__["receive_code"] = code
 
     @check_response
-    def _files(
+    def fs_files(
         self, 
         /, 
         id: int = 0, 
         limit: int = 32, 
         offset: int = 0, 
     ) -> dict:
         return self.client.share_snap({
@@ -6879,15 +6954,15 @@
 
     @cached_property
     def create_time(self, /) -> datetime:
         return datetime.fromtimestamp(int(self.shareinfo["create_time"]))
 
     @property
     def sharedata(self, /) -> dict:
-        return self._files(limit=1)["data"]
+        return self.fs_files(limit=1)["data"]
 
     @property
     def shareinfo(self, /) -> dict:
         return self.sharedata["shareinfo"]
 
     def _attr(self, id: int = 0, /) -> AttrDict:
         try:
@@ -7019,15 +7094,15 @@
         id = attr["id"]
         try:
             return iter(self.attr_cache[id])
         except KeyError:
             dirname = attr["path"]
             def iterdir():
                 page_size = 1 << 10
-                get_files = self._files
+                get_files = self.fs_files
                 path_to_id = self.path_to_id
                 data = get_files(id, page_size)["data"]
                 last_update = datetime.now()
                 for attr in map(normalize_info, data["list"]):
                     attr["fs"] = self
                     attr["last_update"] = last_update
                     path = attr["path"] = joinpath(dirname, escape(attr["name"]))
@@ -7275,15 +7350,15 @@
         id_or_pickcode: int | str, 
         cookie = None, 
         app: str = "web", 
     ) -> Self:
         return cls(P115Client(cookie, login_app=app), id_or_pickcode)
 
     @check_response
-    def _files(
+    def fs_files(
         self, 
         /, 
         path: str = "", 
         next_marker: str = "", 
     ) -> dict:
         return self.client.extract_list(
             path=path, 
@@ -7428,15 +7503,15 @@
         id = attr["id"]
         try:
             return iter(self.attr_cache[id])
         except KeyError:
             nextid = self.__dict__["_nextid"]
             dirname = attr["path"]
             def iterdir():
-                get_files = self._files
+                get_files = self.fs_files
                 path_to_id = self.path_to_id
                 data = get_files(dirname)["data"]
                 last_update = datetime.now()
                 for attr in map(normalize_info, data["list"]):
                     attr["last_update"] = last_update
                     path = joinpath(dirname, escape(attr["name"]))
                     attr.update(id=nextid(), parent_id=id, path=path)
```

### Comparing `python_115-0.0.6.1/p115/cmd/iterdir.py` & `python_115-0.0.6.2/p115/cmd/iterdir.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.6.1/p115/cmd/qrcode.py` & `python_115-0.0.6.2/p115/cmd/qrcode.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.6.1/p115/util/_init_mimetypes.py` & `python_115-0.0.6.2/p115/util/_init_mimetypes.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.6.1/p115/util/cipher.py` & `python_115-0.0.6.2/p115/util/cipher.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.6.1/p115/util/concurrent.py` & `python_115-0.0.6.2/p115/util/concurrent.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.6.1/p115/util/download.py` & `python_115-0.0.6.2/p115/util/download.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.6.1/p115/util/file.py` & `python_115-0.0.6.2/p115/util/file.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.6.1/p115/util/hash.py` & `python_115-0.0.6.2/p115/util/hash.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.6.1/p115/util/ignore.py` & `python_115-0.0.6.2/p115/util/ignore.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.6.1/p115/util/iter.py` & `python_115-0.0.6.2/p115/util/iter.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.6.1/p115/util/path.py` & `python_115-0.0.6.2/p115/util/path.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.6.1/p115/util/property.py` & `python_115-0.0.6.2/p115/util/property.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.6.1/p115/util/response.py` & `python_115-0.0.6.2/p115/util/response.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.6.1/p115/util/retry.py` & `python_115-0.0.6.2/p115/util/retry.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.6.1/p115/util/text.py` & `python_115-0.0.6.2/p115/util/text.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.6.1/p115/util/urlopen.py` & `python_115-0.0.6.2/p115/util/urlopen.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.6.1/pyproject.toml` & `python_115-0.0.6.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-115"
-version = "0.0.6.1"
+version = "0.0.6.2"
 description = "Python wrapper for 115 webdisk."
 authors = ["ChenyangGao <wosiwujm@gmail.com>"]
 license = "MIT"
 readme = "readme.md"
 homepage = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-115-client"
 repository = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-115-client"
 keywords = ["nas", "115"]
```

### Comparing `python_115-0.0.6.1/readme.md` & `python_115-0.0.6.2/readme.md`

 * *Files identical despite different names*

### Comparing `python_115-0.0.6.1/PKG-INFO` & `python_115-0.0.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-115
-Version: 0.0.6.1
+Version: 0.0.6.2
 Summary: Python wrapper for 115 webdisk.
 Home-page: https://github.com/ChenyangGao/web-mount-packs/tree/main/python-115-client
 License: MIT
 Keywords: nas,115
 Author: ChenyangGao
 Author-email: wosiwujm@gmail.com
 Requires-Python: >=3.11,<4.0
```

