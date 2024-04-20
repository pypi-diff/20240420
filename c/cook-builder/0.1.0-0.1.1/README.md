# Comparing `tmp/cook_builder-0.1.0.tar.gz` & `tmp/cook_builder-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cook_builder-0.1.0.tar", last modified: Wed Apr 17 19:42:29 2024, max compression
+gzip compressed data, was "cook_builder-0.1.1.tar", last modified: Sat Apr 20 13:36:05 2024, max compression
```

## Comparing `cook_builder-0.1.0.tar` & `cook_builder-0.1.1.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxrwxr-x   0 seweryn   (1000) seweryn   (1000)        0 2024-04-17 19:42:29.190290 cook_builder-0.1.0/
--rw-rw-r--   0 seweryn   (1000) seweryn   (1000)     1072 2024-02-10 12:14:36.000000 cook_builder-0.1.0/LICENSE
--rw-r--r--   0 seweryn   (1000) seweryn   (1000)     2980 2024-04-17 19:42:29.190290 cook_builder-0.1.0/PKG-INFO
--rw-rw-r--   0 seweryn   (1000) seweryn   (1000)      851 2024-04-14 13:06:12.000000 cook_builder-0.1.0/README.md
-drwxrwxr-x   0 seweryn   (1000) seweryn   (1000)        0 2024-04-17 19:42:29.190290 cook_builder-0.1.0/cook/
--rw-rw-r--   0 seweryn   (1000) seweryn   (1000)      250 2024-04-17 17:21:28.000000 cook_builder-0.1.0/cook/__init__.py
--rw-rw-r--   0 seweryn   (1000) seweryn   (1000)      780 2024-04-15 19:53:48.000000 cook_builder-0.1.0/cook/build_server.py
--rw-rw-r--   0 seweryn   (1000) seweryn   (1000)     1619 2024-04-15 19:53:48.000000 cook_builder-0.1.0/cook/cli.py
--rw-rw-r--   0 seweryn   (1000) seweryn   (1000)     5827 2024-04-17 17:49:40.000000 cook_builder-0.1.0/cook/configuration.py
--rw-rw-r--   0 seweryn   (1000) seweryn   (1000)     2591 2024-04-17 17:35:46.000000 cook_builder-0.1.0/cook/cook.py
--rw-rw-r--   0 seweryn   (1000) seweryn   (1000)      150 2024-04-16 14:39:30.000000 cook_builder-0.1.0/cook/exception.py
--rw-rw-r--   0 seweryn   (1000) seweryn   (1000)     1988 2024-04-17 18:00:59.000000 cook_builder-0.1.0/cook/executors.py
--rw-rw-r--   0 seweryn   (1000) seweryn   (1000)      924 2024-04-13 11:15:16.000000 cook_builder-0.1.0/cook/logger.py
--rw-rw-r--   0 seweryn   (1000) seweryn   (1000)     1079 2024-04-17 17:21:33.000000 cook_builder-0.1.0/cook/main.py
--rw-rw-r--   0 seweryn   (1000) seweryn   (1000)     1030 2024-04-13 20:33:00.000000 cook_builder-0.1.0/cook/recipe.py
--rw-rw-r--   0 seweryn   (1000) seweryn   (1000)     3441 2024-04-17 17:42:46.000000 cook_builder-0.1.0/cook/rsync.py
--rw-rw-r--   0 seweryn   (1000) seweryn   (1000)      382 2024-04-13 14:06:50.000000 cook_builder-0.1.0/cook/watchers.py
-drwxrwxr-x   0 seweryn   (1000) seweryn   (1000)        0 2024-04-17 19:42:29.190290 cook_builder-0.1.0/cook_builder.egg-info/
--rw-r--r--   0 seweryn   (1000) seweryn   (1000)     2980 2024-04-17 19:42:29.000000 cook_builder-0.1.0/cook_builder.egg-info/PKG-INFO
--rw-rw-r--   0 seweryn   (1000) seweryn   (1000)      445 2024-04-17 19:42:29.000000 cook_builder-0.1.0/cook_builder.egg-info/SOURCES.txt
--rw-rw-r--   0 seweryn   (1000) seweryn   (1000)        1 2024-04-17 19:42:29.000000 cook_builder-0.1.0/cook_builder.egg-info/dependency_links.txt
--rw-rw-r--   0 seweryn   (1000) seweryn   (1000)       38 2024-04-17 19:42:29.000000 cook_builder-0.1.0/cook_builder.egg-info/entry_points.txt
--rw-rw-r--   0 seweryn   (1000) seweryn   (1000)       27 2024-04-17 19:42:29.000000 cook_builder-0.1.0/cook_builder.egg-info/requires.txt
--rw-rw-r--   0 seweryn   (1000) seweryn   (1000)        5 2024-04-17 19:42:29.000000 cook_builder-0.1.0/cook_builder.egg-info/top_level.txt
--rw-rw-r--   0 seweryn   (1000) seweryn   (1000)     1110 2024-04-17 19:42:03.000000 cook_builder-0.1.0/pyproject.toml
--rw-rw-r--   0 seweryn   (1000) seweryn   (1000)       38 2024-04-17 19:42:29.190290 cook_builder-0.1.0/setup.cfg
+drwxrwxr-x   0 seweryn   (1000) seweryn   (1000)        0 2024-04-20 13:36:05.090545 cook_builder-0.1.1/
+-rw-rw-r--   0 seweryn   (1000) seweryn   (1000)     1072 2024-02-10 12:14:36.000000 cook_builder-0.1.1/LICENSE
+-rw-r--r--   0 seweryn   (1000) seweryn   (1000)     3006 2024-04-20 13:36:05.090545 cook_builder-0.1.1/PKG-INFO
+-rw-rw-r--   0 seweryn   (1000) seweryn   (1000)      877 2024-04-19 18:55:28.000000 cook_builder-0.1.1/README.md
+drwxrwxr-x   0 seweryn   (1000) seweryn   (1000)        0 2024-04-20 13:36:05.090545 cook_builder-0.1.1/cook/
+-rw-rw-r--   0 seweryn   (1000) seweryn   (1000)       35 2024-04-20 08:35:09.000000 cook_builder-0.1.1/cook/__init__.py
+-rw-rw-r--   0 seweryn   (1000) seweryn   (1000)     1204 2024-04-20 08:24:26.000000 cook_builder-0.1.1/cook/build.py
+-rw-rw-r--   0 seweryn   (1000) seweryn   (1000)     1757 2024-04-20 11:07:01.000000 cook_builder-0.1.1/cook/cli.py
+-rw-rw-r--   0 seweryn   (1000) seweryn   (1000)     4851 2024-04-20 08:51:37.000000 cook_builder-0.1.1/cook/configuration.py
+-rw-rw-r--   0 seweryn   (1000) seweryn   (1000)     2762 2024-04-20 09:11:32.000000 cook_builder-0.1.1/cook/cook.py
+-rw-rw-r--   0 seweryn   (1000) seweryn   (1000)      150 2024-04-16 14:39:30.000000 cook_builder-0.1.1/cook/exception.py
+-rw-rw-r--   0 seweryn   (1000) seweryn   (1000)     2050 2024-04-20 09:06:17.000000 cook_builder-0.1.1/cook/executors.py
+-rw-rw-r--   0 seweryn   (1000) seweryn   (1000)      809 2024-04-20 09:16:35.000000 cook_builder-0.1.1/cook/logger.py
+-rw-rw-r--   0 seweryn   (1000) seweryn   (1000)     1129 2024-04-20 09:17:16.000000 cook_builder-0.1.1/cook/main.py
+-rw-rw-r--   0 seweryn   (1000) seweryn   (1000)     1030 2024-04-13 20:33:00.000000 cook_builder-0.1.1/cook/recipe.py
+-rw-rw-r--   0 seweryn   (1000) seweryn   (1000)     2146 2024-04-20 09:09:37.000000 cook_builder-0.1.1/cook/rsync.py
+-rw-rw-r--   0 seweryn   (1000) seweryn   (1000)     1383 2024-04-20 08:25:29.000000 cook_builder-0.1.1/cook/sync.py
+-rw-rw-r--   0 seweryn   (1000) seweryn   (1000)      381 2024-04-20 09:09:37.000000 cook_builder-0.1.1/cook/watchers.py
+drwxrwxr-x   0 seweryn   (1000) seweryn   (1000)        0 2024-04-20 13:36:05.090545 cook_builder-0.1.1/cook_builder.egg-info/
+-rw-r--r--   0 seweryn   (1000) seweryn   (1000)     3006 2024-04-20 13:36:05.000000 cook_builder-0.1.1/cook_builder.egg-info/PKG-INFO
+-rw-rw-r--   0 seweryn   (1000) seweryn   (1000)      451 2024-04-20 13:36:05.000000 cook_builder-0.1.1/cook_builder.egg-info/SOURCES.txt
+-rw-rw-r--   0 seweryn   (1000) seweryn   (1000)        1 2024-04-20 13:36:05.000000 cook_builder-0.1.1/cook_builder.egg-info/dependency_links.txt
+-rw-rw-r--   0 seweryn   (1000) seweryn   (1000)       38 2024-04-20 13:36:05.000000 cook_builder-0.1.1/cook_builder.egg-info/entry_points.txt
+-rw-rw-r--   0 seweryn   (1000) seweryn   (1000)       27 2024-04-20 13:36:05.000000 cook_builder-0.1.1/cook_builder.egg-info/requires.txt
+-rw-rw-r--   0 seweryn   (1000) seweryn   (1000)        5 2024-04-20 13:36:05.000000 cook_builder-0.1.1/cook_builder.egg-info/top_level.txt
+-rw-rw-r--   0 seweryn   (1000) seweryn   (1000)     1141 2024-04-20 13:35:33.000000 cook_builder-0.1.1/pyproject.toml
+-rw-rw-r--   0 seweryn   (1000) seweryn   (1000)       38 2024-04-20 13:36:05.090545 cook_builder-0.1.1/setup.cfg
```

### Comparing `cook_builder-0.1.0/LICENSE` & `cook_builder-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cook_builder-0.1.0/PKG-INFO` & `cook_builder-0.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cook_builder
-Version: 0.1.0
+Version: 0.1.1
 Summary: Build script aggregator and remote executor
 Author: Seweryn Rusecki
 License: MIT License
         
         Copyright (c) 2024 Seweryn Rusecki
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -80,7 +80,9 @@
 
 <!-- RELEASING
 1. Update version in pyproject.toml
 2. Build and upload wheels to PyPI:
     python3 -m build
     twine upload dist/*
 -->
+
+<!-- TODO: add tests -->
```

### Comparing `cook_builder-0.1.0/README.md` & `cook_builder-0.1.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -34,8 +34,10 @@
 ```
 
 <!-- RELEASING
 1. Update version in pyproject.toml
 2. Build and upload wheels to PyPI:
     python3 -m build
     twine upload dist/*
--->
+-->
+
+<!-- TODO: add tests -->
```

### Comparing `cook_builder-0.1.0/cook/cli.py` & `cook_builder-0.1.1/cook/cli.py`

 * *Files 7% similar despite different names*

```diff
@@ -28,14 +28,19 @@
 
     parser.add_argument('-p', '--recipe_path', default='.', help='Path to directory containing `recipe.py` file.')
     parser.add_argument('-b', '--build_server', help='Build server to use. Uses value of `default_build_server` if left unspecified.')
     parser.add_argument('-r', '--rich_output', action='store_true')
     parser.add_argument('project', nargs='?', help='Project to build. Uses value of `default_project` if left unspecified.')
     parser.add_argument('user_args', nargs='*', default=[], help='User arguments. Can be used in recipe file. Format: `key=value`')
 
+    # TODO: add dry run
+    # TODO: add quiet option
+    # TODO: add user flag args
+    # TODO: use better user args, e.g. --name latest
+
     args = parser.parse_args()
     settings.recipe_base_path = (pathlib.Path.cwd() / args.recipe_path).resolve()
     settings.build_server = args.build_server
     if args.project and '=' in args.project:
         settings.project = None
         args.user_args.insert(0, args.project)
     else:
```

### Comparing `cook_builder-0.1.0/cook/configuration.py` & `cook_builder-0.1.1/cook/configuration.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,36 +1,33 @@
+from copy import copy
 from enum import Enum, auto
 from pathlib import Path
 
-from .build_server import BuildServer
+from .build import BuildServer
+
+
+def get_nested_item(source_dict, *keys, default=None):
+    nested_item = source_dict
+    for key in keys:
+        if key not in nested_item:
+            return default
+        nested_item = nested_item[key]
+    return nested_item
 
 
 class ConfigurationError(Exception):
     pass
 
 
 class BuildType(Enum):
     LOCAL = auto()
     REMOTE = auto()
     COMPOSITE = auto()
 
 
-class BuildStep:
-    def __init__(self, workdir='.', command='', responders=None, expected_return_code=0, check=True):
-        self.command = command
-        self.workdir = workdir
-        self.expected_return_code = expected_return_code
-        self.check = check
-
-        if responders:
-            self.responders = responders
-        else:
-            self.responders = tuple()
-
-
 class Configuration:
     def __init__(self, recipe):
         self.projects = recipe.projects
 
         self.default_project = recipe.default_project
         self.default_build_server = recipe.default_build_server
 
@@ -46,21 +43,15 @@
 
         self._set_project(project)
         self._set_build_server(server)
 
         if not self._is_composite():
             self._update_paths()
 
-    def _get_nested_item(self, source_dict, *keys):
-        nested_item = source_dict
-        for key in keys:
-            if key not in nested_item:
-                return None
-            nested_item = nested_item[key]
-        return nested_item
+        # TODO: validate recipe contents and print warnings
 
     def _set_project(self, project):
         project_defined = project in self.projects
 
         if not project_defined:
             raise ConfigurationError(f'No such project {project}')
 
@@ -71,27 +62,27 @@
         if server_override is not None:
             build_server_name = server_override
 
         if self._is_composite():
             self.build_server = BuildServer(name=build_server_name)
             return
 
-        for build_server in self._get_nested_item(self.projects, self.project, 'build_servers'):
+        for build_server in get_nested_item(self.projects, self.project, 'build_servers'):
             if build_server.name == build_server_name:
                 self.build_server = build_server
                 break
         else:
             raise ConfigurationError(f'Build server {build_server_name} not defined for {self.project}')
 
         if self.build_server.skip == True:
             self.skip = True
             return
 
     def _get_build_server_override(self):
-        build_servers = self._get_nested_item(self.projects, self.project, 'build_servers')
+        build_servers = get_nested_item(self.projects, self.project, 'build_servers')
         if build_servers is None:
             return None
 
         overrides = []
         for build_server in build_servers:
             if build_server.override == True:
                 overrides.append(build_server.name)
@@ -132,58 +123,44 @@
     def get_build_server(self):
         return self.build_server.name
 
     def get_base_paths(self):
         return self.base_path.as_posix(), self.build_path.as_posix()
 
     def get_files_to_send(self):
-        files_to_send = self._get_nested_item(self.projects, self.project, 'send')
+        files_to_send = get_nested_item(self.projects, self.project, 'send')
 
         if files_to_send is None:
             return None
 
         return files_to_send
 
     def get_files_to_receive(self):
-        files_to_receive = self._get_nested_item(self.projects, self.project, 'receive')
+        files_to_receive = get_nested_item(self.projects, self.project, 'receive')
 
         if files_to_receive is None:
             return None
 
         return files_to_receive
 
     def get_build_steps(self):
         if self.skip == True:
             return None
 
-        build_steps = self._get_nested_item(self.projects, self.project, 'build_steps')
+        build_steps = get_nested_item(self.projects, self.project, 'build_steps')
 
         if build_steps is None:
             return None
 
         parsed_build_steps = []
 
         for step in build_steps:
-            if isinstance(step, str):
-                workdir = '.'
-                command = step
-                responders = None
-                expected_return_code = 0
-                check = True
-            elif isinstance(step, BuildStep):
-                workdir = step.workdir
-                command = step.command
-                responders = step.responders
-                expected_return_code = step.expected_return_code
-                check = step.check
-            else:
-                raise ConfigurationError(f'Expected build step to be of type str of BuildStep, was {type(step)}')
-
-            workdir = self.build_path / workdir
-            parsed_step = BuildStep(workdir=workdir, command=command, responders=responders, expected_return_code=expected_return_code, check=check)
+            # shallow copy is enough as only a str is modified but be careful
+            parsed_step = copy(step)
+            parsed_step.workdir = self.build_path / parsed_step.workdir
             parsed_build_steps.append(parsed_step)
 
         return parsed_build_steps
 
     def get_components(self):
-        components = self._get_nested_item(self.projects, self.project, 'components')
+        components = get_nested_item(self.projects, self.project, 'components')
         return components
```

### Comparing `cook_builder-0.1.0/cook/cook.py` & `cook_builder-0.1.1/cook/cook.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,80 +1,81 @@
 import subprocess
 
 import fabric
 
 from .configuration import BuildType, Configuration
 from .executors import LocalExecutor, RemoteExecutor
-from .logger import Logger
 from .rsync import Rsync
 
 
 class Cook:
-    def __init__(self, recipe, configuration, rich_output=False):
+    def __init__(self, recipe, configuration, logger):
         self.recipe = recipe
         self.configuration = configuration
-        self.rich_output = rich_output
+        self.logger = logger
 
     def cook(self):
         build_type = self.configuration.get_build_type()
+        self.build_server = self.configuration.get_build_server()
 
         if build_type == BuildType.LOCAL:
             self._local_build()
         elif build_type == BuildType.COMPOSITE:
             self._composite_build()
         elif build_type == BuildType.REMOTE:
             self._remote_build()
         else:
             raise RuntimeError(f'Unknown build type: {build_type}')
 
     def _local_build(self):
         build_steps = self.configuration.get_build_steps()
 
         if build_steps:
-            Logger().local('Running local build')
-            executor = LocalExecutor('local', Logger(), self.rich_output)
+            self.logger.print('local', 'Running local build')
+            executor = LocalExecutor('local', self.logger)
             executor.run_multiple(build_steps)
 
     def _remote_build(self):
         build_steps = self.configuration.get_build_steps()
         local_base, remote_base = self.configuration.get_base_paths()
         files_to_send = self.configuration.get_files_to_send()
         files_to_receive = self.configuration.get_files_to_receive()
 
-        ssh_name = self.configuration.get_build_server()
-
-        setup_rsync = bool(files_to_send or files_to_receive)
-
+        setup_rsync = files_to_send or files_to_receive
         if setup_rsync:
-            rsync = Rsync(ssh_name, local_base, remote_base, Logger())
+            rsync = Rsync(self.build_server, local_base, remote_base, self.logger)
 
         if files_to_send:
-            Logger().remote('Sending Files')
+            self.logger.print('remote', 'Sending Files')
             rsync.send(files_to_send)
 
         if build_steps:
-            Logger().remote('Running Remote Build')
-            executor = RemoteExecutor(ssh_name, Logger(), self.rich_output)
+            self.logger.print('remote', 'Running Remote Build')
+            executor = RemoteExecutor(self.build_server, self.logger)
             executor.run_multiple(build_steps)
 
         if files_to_receive:
-            Logger().remote('Receiving Files')
+            self.logger.print('remote', 'Receiving Files')
             rsync.receive(files_to_receive)
 
     def _composite_build(self):
         components = self.configuration.get_components()
 
         if not components:  # TODO required?
             return
 
-        Logger().local('Executing Components')
+        self.logger.print('local', 'Executing Components')
 
         for component in components:
-            Logger().local(f'Component: {component}')
+            self.logger.print('local', f'Component: {component}')
+            self._run_component(component)
 
+    def _run_component(self, component):
+        try:
             sub_configuration = Configuration(self.recipe)
+            sub_configuration.setup(component, self.build_server)
 
-            build_server = self.configuration.get_build_server()
-            sub_configuration.setup(component, build_server)
-
-            sub_cook = Cook(self.recipe, sub_configuration, self.rich_output)
+            sub_cook = Cook(self.recipe, sub_configuration, self.logger)
             sub_cook.cook()
+        except Exception as e:
+            self.logger.print('error', f'Component {component} failed!')
+            raise e
```

### Comparing `cook_builder-0.1.0/cook/executors.py` & `cook_builder-0.1.1/cook/executors.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,44 +20,47 @@
         self.name = name
         self.logger = logger
         self.rich_output = rich_output
 
     def run(self, context, step):
         run_args = {'watchers': []}
 
-        if self.rich_output:
+        if self.rich_output and self.logger:
             rich_printer = RichPrinter(self.logger)
             run_args['hide'] = 'both'
             run_args['watchers'].append(rich_printer)
 
         if step.responders:
             run_args['watchers'].extend(step.responders)
 
-        try:  # TODO: move this outside of run step
-            with context.cd(step.workdir):
-                result = context.run(step.command, warn=True, pty=True, **run_args)
-        except gaierror as e:
-            raise ExecutorError(e.strerror, self.name, e.errno)
+        with context.cd(step.workdir):
+            result = context.run(step.command, warn=True, pty=True, **run_args)
 
         return_code = result.return_code
         if step.check and return_code != step.expected_return_code:
             raise ProcessError(f'Encountered unexpected exit code {return_code}, expected {step.expected_return_code}', return_code)
 
 
 class LocalExecutor(Executor):
     def run_multiple(self, steps):
         context = invoke.context.Context()
         for step in steps:
             if self.logger:
-                self.logger.local(f'Local Workdir/Command: {step.workdir}: {step.command}')
+                self.logger.print('local', f'Local Workdir/Command: {step.workdir}: {step.command}')
 
             self.run(context, step)
 
 
 class RemoteExecutor(Executor):
+    def _execute_step(self, context, step):
+        if self.logger:
+            self.logger.print('remote', f'Remote Workdir/Command: {self.name}:{step.workdir}: {step.command}')
+
+        try:
+            self.run(context, step)
+        except gaierror as e:
+            raise ExecutorError(e.strerror, self.name, e.errno)
+
     def run_multiple(self, steps):
         with fabric.Connection(self.name) as context:
             for step in steps:
-                if self.logger:
-                    self.logger.remote(f'Remote Workdir/Command: {self.name}:{step.workdir}: {step.command}')
-
-                self.run(context, step)
+                self._execute_step(context, step)
```

### Comparing `cook_builder-0.1.0/cook/logger.py` & `cook_builder-0.1.1/cook/logger.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,37 +1,29 @@
 from rich.console import Console
 from rich.theme import Theme
 
-GREEN = '#00cc52'
-PURPLE = '#d849ff'
-RED = '#ff0000'
-
 
 class Logger:
-    def __init__(self):
+    GREEN = '#00cc52'
+    PURPLE = '#d849ff'
+
+    def __init__(self, log_rich_output):
         cook_console_theme = Theme(
             {
-                'local': GREEN,
-                'remote': PURPLE,
-                'error': RED,
+                'local': Logger.GREEN,
+                'remote': Logger.PURPLE,
+                'warning': 'dark_orange',
+                'error': 'red',
             }
         )
         self.console = Console(theme=cook_console_theme)
+        self.log_rich_output = log_rich_output
 
-    def _internal_message(self, message, style):
+    def print(self, style, message):
         message = '=== ' + str(message) + ' ==='
         self.console.print(message, style=style, highlight=False)
 
-    def local(self, message):
-        self._internal_message(message, 'local')
-
-    def remote(self, message):
-        self._internal_message(message, 'remote')
-
-    def error(self, message):
-        self._internal_message(message, 'error')
-
-    def rich(self, message):
-        self.console.print(message, end='')
-
-    def raw(self, message):
-        print(message, end='')
+    def log(self, message):
+        if self.log_rich_output:
+            self.console.print(message, end='')
+        else:
+            print(message, end='')
```

### Comparing `cook_builder-0.1.0/cook/main.py` & `cook_builder-0.1.1/cook/main.py`

 * *Files 23% similar despite different names*

```diff
@@ -17,28 +17,30 @@
 
 settings = Settings()
 
 
 def main():
     global settings
 
+    logger = Logger(settings.rich_output)
+
     try:
         recipe = Recipe(settings.recipe_base_path)
         recipe.load()
 
         configuration = Configuration(recipe)
         configuration.setup(settings.project, settings.build_server)
 
-        cook = Cook(recipe, configuration, settings.rich_output)
+        cook = Cook(recipe, configuration, logger)
         cook.cook()
 
     except (RecipeNotFound, RecipeError, ConfigurationError) as e:
-        Logger().error(e)
+        logger.print('error', e)
         exit(1)
 
     except ProcessError as e:
-        Logger().error(e)
+        logger.print('error', e)
         exit(e.return_code)
 
     except ExecutorError as e:
-        Logger().error(f'{e.name}: {e}')
+        logger.print('error', f'{e.name}: {e}')
         exit(e.return_code)
```

### Comparing `cook_builder-0.1.0/cook/recipe.py` & `cook_builder-0.1.1/cook/recipe.py`

 * *Files identical despite different names*

### Comparing `cook_builder-0.1.0/cook_builder.egg-info/PKG-INFO` & `cook_builder-0.1.1/cook_builder.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cook_builder
-Version: 0.1.0
+Version: 0.1.1
 Summary: Build script aggregator and remote executor
 Author: Seweryn Rusecki
 License: MIT License
         
         Copyright (c) 2024 Seweryn Rusecki
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -80,7 +80,9 @@
 
 <!-- RELEASING
 1. Update version in pyproject.toml
 2. Build and upload wheels to PyPI:
     python3 -m build
     twine upload dist/*
 -->
+
+<!-- TODO: add tests -->
```

### Comparing `cook_builder-0.1.0/pyproject.toml` & `cook_builder-0.1.1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cook_builder"
-version = "0.1.0"
+version = "0.1.1"
 dependencies = [
   "fabric==3.2.2",
   "rich==13.7.1",
 ]
 requires-python = ">=3.10"
 authors = [
   { name="Seweryn Rusecki" },
@@ -37,7 +37,10 @@
 cook = "cook.cli:cli"
 
 [tool.black]
 line-length = 140
 target-version = ['py310']
 skip-string-normalization = true
 extend-exclude = 'example/recipe.py'
+
+[tool.isort]
+profile = "black"
```

