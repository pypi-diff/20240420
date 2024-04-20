# Comparing `tmp/pyfineflow-1.1.1.tar.gz` & `tmp/pyfineflow-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfineflow-1.1.1.tar", last modified: Thu Apr 11 14:46:27 2024, max compression
+gzip compressed data, was "pyfineflow-1.1.2.tar", last modified: Sat Apr 20 11:15:53 2024, max compression
```

## Comparing `pyfineflow-1.1.1.tar` & `pyfineflow-1.1.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-04-11 14:46:27.611732 pyfineflow-1.1.1/
--rw-rw-rw-   0        0        0     1086 2024-02-03 16:31:19.000000 pyfineflow-1.1.1/LICENSE
--rw-rw-rw-   0        0        0     1277 2024-04-11 14:46:27.610732 pyfineflow-1.1.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-11 14:46:27.596926 pyfineflow-1.1.1/pyfineflow/
--rw-rw-rw-   0        0        0        0 2024-01-18 17:00:18.000000 pyfineflow-1.1.1/pyfineflow/__init__.py
--rw-rw-rw-   0        0        0     2110 2024-04-11 14:44:44.000000 pyfineflow-1.1.1/pyfineflow/__main__.py
--rw-rw-rw-   0        0        0    17560 2024-04-11 14:24:51.000000 pyfineflow-1.1.1/pyfineflow/core.py
--rw-rw-rw-   0        0        0     1222 2024-01-18 17:00:18.000000 pyfineflow-1.1.1/pyfineflow/log_conf.py
--rw-rw-rw-   0        0        0     3449 2024-01-18 17:00:18.000000 pyfineflow-1.1.1/pyfineflow/schemas.py
--rw-rw-rw-   0        0        0     4171 2024-04-07 14:08:33.000000 pyfineflow-1.1.1/pyfineflow/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-11 14:46:27.608664 pyfineflow-1.1.1/pyfineflow.egg-info/
--rw-rw-rw-   0        0        0     1277 2024-04-11 14:46:27.000000 pyfineflow-1.1.1/pyfineflow.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      352 2024-04-11 14:46:27.000000 pyfineflow-1.1.1/pyfineflow.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-11 14:46:27.000000 pyfineflow-1.1.1/pyfineflow.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2024-04-11 14:46:27.000000 pyfineflow-1.1.1/pyfineflow.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       22 2024-04-11 14:46:27.000000 pyfineflow-1.1.1/pyfineflow.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-04-11 14:46:27.000000 pyfineflow-1.1.1/pyfineflow.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-11 14:46:27.611732 pyfineflow-1.1.1/setup.cfg
--rw-rw-rw-   0        0        0      676 2024-04-11 14:46:22.000000 pyfineflow-1.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-20 11:15:53.306419 pyfineflow-1.1.2/
+-rw-rw-rw-   0        0        0     1086 2024-02-03 16:31:19.000000 pyfineflow-1.1.2/LICENSE
+-rw-rw-rw-   0        0        0     1265 2024-04-20 11:15:53.306419 pyfineflow-1.1.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-20 11:15:53.290891 pyfineflow-1.1.2/pyfineflow/
+-rw-rw-rw-   0        0        0        0 2024-01-18 17:00:18.000000 pyfineflow-1.1.2/pyfineflow/__init__.py
+-rw-rw-rw-   0        0        0     2123 2024-04-20 11:15:24.000000 pyfineflow-1.1.2/pyfineflow/__main__.py
+-rw-rw-rw-   0        0        0    17689 2024-04-20 11:14:46.000000 pyfineflow-1.1.2/pyfineflow/core.py
+-rw-rw-rw-   0        0        0     1222 2024-01-18 17:00:18.000000 pyfineflow-1.1.2/pyfineflow/log_conf.py
+-rw-rw-rw-   0        0        0     3449 2024-01-18 17:00:18.000000 pyfineflow-1.1.2/pyfineflow/schemas.py
+-rw-rw-rw-   0        0        0     4171 2024-04-07 14:08:33.000000 pyfineflow-1.1.2/pyfineflow/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-20 11:15:53.303891 pyfineflow-1.1.2/pyfineflow.egg-info/
+-rw-rw-rw-   0        0        0     1265 2024-04-20 11:15:53.000000 pyfineflow-1.1.2/pyfineflow.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      352 2024-04-20 11:15:53.000000 pyfineflow-1.1.2/pyfineflow.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-20 11:15:53.000000 pyfineflow-1.1.2/pyfineflow.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2024-04-20 11:15:53.000000 pyfineflow-1.1.2/pyfineflow.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       22 2024-04-20 11:15:53.000000 pyfineflow-1.1.2/pyfineflow.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-20 11:15:53.000000 pyfineflow-1.1.2/pyfineflow.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-20 11:15:53.307424 pyfineflow-1.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      676 2024-04-20 11:15:51.000000 pyfineflow-1.1.2/setup.py
```

### Comparing `pyfineflow-1.1.1/LICENSE` & `pyfineflow-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyfineflow-1.1.1/PKG-INFO` & `pyfineflow-1.1.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfineflow
-Version: 1.1.1
+Version: 1.1.2
 Summary: python nodes server for fineflow
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pyfineflow
 
 > fineflow的python节点后端
@@ -49,16 +49,16 @@
 
 @fine.node(category='数学运算', name="相减")
 def sub(num1: int, num2: int = 2) -> int:
     num = num1 - num2
     return num
 
 
-@fine.node(category='数学运算', name="原路返回")
-def sub(num1: int, num2: int = 2) -> (int, int):
+@fine.node(category='数学运算')
+def 原路返回(num1: int, num2: int = 2) -> (int, int):
     return num1, num2
 ```
 
 ```python
 # main.py
 from app import fine
```

### Comparing `pyfineflow-1.1.1/pyfineflow/__main__.py` & `pyfineflow-1.1.2/pyfineflow/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     class FuncReq(BaseModel):
         code: str
         params: dict
 
     @app.post(f'/{key}/func')
     def func(req: FuncReq):
         try:
-            vars = {'params': req.params}
+            vars = {'params': req.params,'help': help}
             exec(f"{req.code}\nres=func(params)", vars)
             return {'state': 1, 'msg': f'', 'data': vars['res']}
         except Exception as e:
             error_traceback = traceback.format_exc()
             # 将错误信息按行分割成列表
             traceback_lines = error_traceback.splitlines()
             # 获取最后五行的错误信息
```

### Comparing `pyfineflow-1.1.1/pyfineflow/core.py` & `pyfineflow-1.1.2/pyfineflow/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -177,15 +177,15 @@
         class FuncReq(BaseModel):
             code: str
             params: dict
 
         @router.post('/func')
         def func(req: FuncReq):
             try:
-                vars = {'params': req.params}
+                vars = {'params': req.params, 'help': help}
                 exec(f"{req.code}\nres=func(params)", vars)
                 return vars['res']
             except Exception as e:
                 error_traceback = traceback.format_exc()
                 # 将错误信息按行分割成列表
                 traceback_lines = error_traceback.splitlines()
                 # 获取最后五行的错误信息
@@ -250,14 +250,16 @@
         conf: Node = self.node_conf_map[node_key]
         func = self.node_func_map[node_key]
         kwargs = {}
         for key, item in params.items():
             user_server = item.get('useServer', False)
             value = item['value']
             if user_server:
+                if not value:
+                    raise Exception(f'input param:"{key}" is unset')
                 value = work.get_out_value_by_index(value)
             kwargs[key] = value
         func.ctx = NodeCtx(work_id, node_id, work)
         res = func(**kwargs)
         out_val_map = {}
         if len(conf['output']) == 1:
             key = conf['output'][0]['key']
@@ -305,15 +307,15 @@
         class FuncReq(BaseModel):
             code: str
             params: dict
 
         @router.post('/func')
         def func(req: FuncReq):
             try:
-                vars = {'params': req.params}
+                vars = {'params': req.params, 'help': help}
                 exec(f"{req.code}\nres=func(params)", vars)
                 return {'state': 1, 'msg': f'', 'data': vars['res']}
             except Exception as e:
                 error_traceback = traceback.format_exc()
                 # 将错误信息按行分割成列表
                 traceback_lines = error_traceback.splitlines()
                 # 获取最后五行的错误信息
```

### Comparing `pyfineflow-1.1.1/pyfineflow/log_conf.py` & `pyfineflow-1.1.2/pyfineflow/log_conf.py`

 * *Files identical despite different names*

### Comparing `pyfineflow-1.1.1/pyfineflow/schemas.py` & `pyfineflow-1.1.2/pyfineflow/schemas.py`

 * *Files identical despite different names*

### Comparing `pyfineflow-1.1.1/pyfineflow/utils.py` & `pyfineflow-1.1.2/pyfineflow/utils.py`

 * *Files identical despite different names*

### Comparing `pyfineflow-1.1.1/pyfineflow.egg-info/PKG-INFO` & `pyfineflow-1.1.2/pyfineflow.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfineflow
-Version: 1.1.1
+Version: 1.1.2
 Summary: python nodes server for fineflow
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pyfineflow
 
 > fineflow的python节点后端
@@ -49,16 +49,16 @@
 
 @fine.node(category='数学运算', name="相减")
 def sub(num1: int, num2: int = 2) -> int:
     num = num1 - num2
     return num
 
 
-@fine.node(category='数学运算', name="原路返回")
-def sub(num1: int, num2: int = 2) -> (int, int):
+@fine.node(category='数学运算')
+def 原路返回(num1: int, num2: int = 2) -> (int, int):
     return num1, num2
 ```
 
 ```python
 # main.py
 from app import fine
```

### Comparing `pyfineflow-1.1.1/setup.py` & `pyfineflow-1.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # --skip-existing 覆盖
 # python setup.py sdist bdist_wheel
 # twine upload dist/* --skip-existing
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 setup(
     name='pyfineflow',
-    version='1.1.1',
+    version='1.1.2',
     packages=find_packages(exclude=['__pycache__']),
     description='python nodes server for fineflow',
     long_description=long_description,
     long_description_content_type='text/markdown',
     install_requires=[
         'fastapi[all]~=0.110.1',
     ],
```

