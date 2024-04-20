# Comparing `tmp/cmgr-0.0.4.tar.gz` & `tmp/cmgr-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cmgr-0.0.4.tar", last modified: Wed Mar  6 13:03:15 2024, max compression
+gzip compressed data, was "cmgr-0.0.7.tar", last modified: Sat Apr 20 05:10:07 2024, max compression
```

## Comparing `cmgr-0.0.4.tar` & `cmgr-0.0.7.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 kyan001    (501) staff       (20)        0 2024-03-06 13:03:15.023462 cmgr-0.0.4/
--rw-r--r--   0 kyan001    (501) staff       (20)     1491 2024-02-28 08:45:45.000000 cmgr-0.0.4/LICENSE
--rw-r--r--   0 kyan001    (501) staff       (20)     3035 2024-03-06 13:03:15.023141 cmgr-0.0.4/PKG-INFO
--rw-r--r--   0 kyan001    (501) staff       (20)      293 2024-02-29 15:50:18.000000 cmgr-0.0.4/README.md
-drwxr-xr-x   0 kyan001    (501) staff       (20)        0 2024-03-06 13:03:15.020738 cmgr-0.0.4/cmgr/
--rw-r--r--   0 kyan001    (501) staff       (20)     8706 2024-03-06 12:58:14.000000 cmgr-0.0.4/cmgr/__init__.py
--rw-r--r--   0 kyan001    (501) staff       (20)       79 2024-03-05 08:08:08.000000 cmgr-0.0.4/cmgr/__main__.py
--rw-r--r--   0 kyan001    (501) staff       (20)     2065 2024-03-05 08:08:08.000000 cmgr-0.0.4/cmgr/command_line.py
-drwxr-xr-x   0 kyan001    (501) staff       (20)        0 2024-03-06 13:03:15.022595 cmgr-0.0.4/cmgr.egg-info/
--rw-r--r--   0 kyan001    (501) staff       (20)     3035 2024-03-06 13:03:15.000000 cmgr-0.0.4/cmgr.egg-info/PKG-INFO
--rw-r--r--   0 kyan001    (501) staff       (20)      341 2024-03-06 13:03:15.000000 cmgr-0.0.4/cmgr.egg-info/SOURCES.txt
--rw-r--r--   0 kyan001    (501) staff       (20)        1 2024-03-06 13:03:15.000000 cmgr-0.0.4/cmgr.egg-info/dependency_links.txt
--rw-r--r--   0 kyan001    (501) staff       (20)       48 2024-03-06 13:03:15.000000 cmgr-0.0.4/cmgr.egg-info/entry_points.txt
--rw-r--r--   0 kyan001    (501) staff       (20)       63 2024-03-06 13:03:15.000000 cmgr-0.0.4/cmgr.egg-info/requires.txt
--rw-r--r--   0 kyan001    (501) staff       (20)       10 2024-03-06 13:03:15.000000 cmgr-0.0.4/cmgr.egg-info/top_level.txt
--rw-r--r--   0 kyan001    (501) staff       (20)     1316 2024-03-06 13:02:51.000000 cmgr-0.0.4/pyproject.toml
--rw-r--r--   0 kyan001    (501) staff       (20)       12 2024-03-06 13:02:42.000000 cmgr-0.0.4/requirements-dev.txt
--rw-r--r--   0 kyan001    (501) staff       (20)       44 2024-03-06 12:58:37.000000 cmgr-0.0.4/requirements.txt
--rw-r--r--   0 kyan001    (501) staff       (20)       38 2024-03-06 13:03:15.023517 cmgr-0.0.4/setup.cfg
-drwxr-xr-x   0 kyan001    (501) staff       (20)        0 2024-03-06 13:03:15.022229 cmgr-0.0.4/tests/
--rw-r--r--   0 kyan001    (501) staff       (20)     1217 2024-02-29 16:15:01.000000 cmgr-0.0.4/tests/test_cmgr.py
--rw-r--r--   0 kyan001    (501) staff       (20)      472 2024-02-29 16:18:14.000000 cmgr-0.0.4/tests/test_command_line.py
+drwxr-xr-x   0 kyan001    (501) staff       (20)        0 2024-04-20 05:10:07.293954 cmgr-0.0.7/
+-rw-r--r--   0 kyan001    (501) staff       (20)     1491 2024-02-28 08:45:45.000000 cmgr-0.0.7/LICENSE
+-rw-r--r--   0 kyan001    (501) staff       (20)     4452 2024-04-20 05:10:07.293764 cmgr-0.0.7/PKG-INFO
+-rw-r--r--   0 kyan001    (501) staff       (20)     1710 2024-03-07 12:15:50.000000 cmgr-0.0.7/README.md
+drwxr-xr-x   0 kyan001    (501) staff       (20)        0 2024-04-20 05:10:07.292374 cmgr-0.0.7/cmgr/
+-rw-r--r--   0 kyan001    (501) staff       (20)     8599 2024-04-20 05:08:09.000000 cmgr-0.0.7/cmgr/__init__.py
+-rw-r--r--   0 kyan001    (501) staff       (20)       79 2024-03-05 08:08:08.000000 cmgr-0.0.7/cmgr/__main__.py
+-rw-r--r--   0 kyan001    (501) staff       (20)     2204 2024-03-06 13:26:48.000000 cmgr-0.0.7/cmgr/command_line.py
+drwxr-xr-x   0 kyan001    (501) staff       (20)        0 2024-04-20 05:10:07.293433 cmgr-0.0.7/cmgr.egg-info/
+-rw-r--r--   0 kyan001    (501) staff       (20)     4452 2024-04-20 05:10:07.000000 cmgr-0.0.7/cmgr.egg-info/PKG-INFO
+-rw-r--r--   0 kyan001    (501) staff       (20)      341 2024-04-20 05:10:07.000000 cmgr-0.0.7/cmgr.egg-info/SOURCES.txt
+-rw-r--r--   0 kyan001    (501) staff       (20)        1 2024-04-20 05:10:07.000000 cmgr-0.0.7/cmgr.egg-info/dependency_links.txt
+-rw-r--r--   0 kyan001    (501) staff       (20)       48 2024-04-20 05:10:07.000000 cmgr-0.0.7/cmgr.egg-info/entry_points.txt
+-rw-r--r--   0 kyan001    (501) staff       (20)       63 2024-04-20 05:10:07.000000 cmgr-0.0.7/cmgr.egg-info/requires.txt
+-rw-r--r--   0 kyan001    (501) staff       (20)       10 2024-04-20 05:10:07.000000 cmgr-0.0.7/cmgr.egg-info/top_level.txt
+-rw-r--r--   0 kyan001    (501) staff       (20)     1316 2024-03-06 13:02:51.000000 cmgr-0.0.7/pyproject.toml
+-rw-r--r--   0 kyan001    (501) staff       (20)       12 2024-03-06 13:02:42.000000 cmgr-0.0.7/requirements-dev.txt
+-rw-r--r--   0 kyan001    (501) staff       (20)       44 2024-03-06 12:58:37.000000 cmgr-0.0.7/requirements.txt
+-rw-r--r--   0 kyan001    (501) staff       (20)       38 2024-04-20 05:10:07.293995 cmgr-0.0.7/setup.cfg
+drwxr-xr-x   0 kyan001    (501) staff       (20)        0 2024-04-20 05:10:07.293288 cmgr-0.0.7/tests/
+-rw-r--r--   0 kyan001    (501) staff       (20)     1217 2024-03-07 11:38:13.000000 cmgr-0.0.7/tests/test_cmgr.py
+-rw-r--r--   0 kyan001    (501) staff       (20)      694 2024-03-07 10:44:30.000000 cmgr-0.0.7/tests/test_command_line.py
```

### Comparing `cmgr-0.0.4/LICENSE` & `cmgr-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `cmgr-0.0.4/cmgr/__init__.py` & `cmgr-0.0.7/cmgr/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,53 +1,52 @@
 import os
 
 import consoleiotools as cit
 import consolecmdtools as cct
-for lib in (libs := ['tomllib', 'tomli', 'tomlkit']):
+for lib in (libs := ['tomllib', 'tomli']):
     try:
         toml_parser = __import__(lib)
         break
     except ImportError:
         pass
 else:
     raise ImportError("No TOML parser lib found in {libs}!")
 
 
-__version__ = "0.0.4"
+__version__ = "0.0.7"
 
 
 CMGR_PROFILE_FILENAME = 'cmgr.toml'  # Config Manager profile is the config file for cmgr itself.
 
 
-def _soft_raise(text: str):
-    """Print the error message, pause the program and exit."""
+def _raise(text: str):
+    """Print the error message and exit."""
     cit.err(text)
-    cit.pause()
-    cit.bye()
+    exit(1)
 
 
 def _parse_src_or_dst(path_or_cmd: str) -> cct.Path:
     """Parse the source or destination path or command.
 
     Args:
         path_or_cmd (str): The source or destination path or command.
 
     Returns:
         cct.Path: The parsed path.
     """
     if not path_or_cmd:
-        _soft_raise("The input of `_parse_src_or_dst()` is empty!")
+        _raise("The input of `_parse_src_or_dst()` is empty!")
     if os.path.isfile(path_or_cmd):  # path_or_cmd is a file
         return cct.get_path(path_or_cmd)
     if cct.is_cmd_exist(path_or_cmd):  # path_or_cmd is a command
         return cct.get_path(cct.read_cmd(path_or_cmd).strip())
     return cct.get_path(path_or_cmd)  # path_or_cmd is not a existing file or a valid command, guess it's a file path
 
 
-def print_profile_help():
+def print_profile_help() -> None:
     minimal_profile_url = "https://github.com/kyan001/PyConfigManager/raw/main/cmgr-minimal.toml"
     example_profile_url = "https://github.com/kyan001/PyConfigManager/raw/main/cmgr-example.toml"
     cit.info("Here is a minimal Config Manager profile example:")
     cit.print(cct.read_url(minimal_profile_url).decode())
     cit.info(f"For more details, visit: {example_profile_url}")
 
 
@@ -86,20 +85,19 @@
     Returns:
         dict: The Config Manager profile.
     """
     cmgr_profile_path = cct.get_path(path)
     if not cmgr_profile_path.exists:
         cit.warn(f"cmgr profile file `{path}` not found!")
         print_profile_help()
-        cit.pause()
-        cit.bye()
+        exit(1)
     with open(cmgr_profile_path, 'rb') as fl:
         cmgr_info = toml_parser.load(fl)
     if not cmgr_info:
-        _soft_raise(f"Bad cmgr config file `{path}`!")
+        _raise(f"Bad cmgr config file `{path}`!")
     cmgr_info['path'] = cmgr_profile_path  # add the path of the Config Manager profile to the Config Manager info.
     return make_configmanager(cmgr_info)
 
 
 def make_configmanager(info: dict) -> dict:
     """Validate and calibrate the Config Manager info.
 
@@ -114,29 +112,29 @@
     elif not info.get('name'):
         info['name'] = info['path'].parent.basename
     if not isinstance(info.get('path'), cct.Path):
         info['path'] = cct.get_path(info.get('path'))
     if info.get('install'):
         for package in info.get('install'):
             if not package.get('name'):
-                _soft_raise(f"Package name not found in {package}!")
+                _raise(f"Package name not found in {package}!")
             if not package.get('cmd'):
                 package['cmd'] = package['name']
     if info.get('config'):
         for config in info.get('config'):
             if not config.get('src'):
-                _soft_raise(f"Source config file path not found in {config}!")
+                _raise(f"Source config file path not found in {config}!")
             src = _parse_src_or_dst(config.get('src'))
             if not src.exists and not os.path.isabs(src):  # try to find the source file in the directory of the Config Manager profile.
                 src = cct.get_path(os.path.join(info.get('path').parent, config.get('src')))
             if not src.exists:
-                _soft_raise(f"Source config file not found: {src}!")
+                _raise(f"Source config file not found: {src}!")
             config['src'] = src
             if not config.get('dst'):
-                _soft_raise(f"Destination config file path not found in {config}!")
+                _raise(f"Destination config file path not found in {config}!")
             config['dst'] = cct.get_path(_parse_src_or_dst(config.get('dst')))
             if not config.get('name'):
                 config['name'] = src.basename
     if not info.get('name'):
         if info.get('config'):
             info['name'] = info['config'][0]['name']
         elif info.get('install'):
@@ -153,43 +151,43 @@
         filename (str): The filename of the Config Manager profile.
         root (str, optional): The directory to search. If not given, the directory of this script is used.
 
     Returns:
         list[str]: A list of Config Manager profile paths.
     """
     if not filename:
-        _soft_raise("The `filename` of Config Manager profile is empty!")
+        _raise("The `filename` of Config Manager profile is empty!")
     if not root:
         root = os.getcwd()
     if not isinstance(root, cct.Path):
         root = cct.get_path(root)
     cmgr_profiles: list[cct.Path] = []
     for path in cct.bfs_walk(root):
         path = cct.get_path(path)
         if path.basename == filename:
             cmgr_profiles.append(path)
     return cmgr_profiles
 
 
-def run_configmanager(config_manager: dict):
+def run_configmanager(config_manager: dict) -> None:
     """Run the config manager.
 
     Args:
         config_manager (dict): The Config Manager info.
     """
     cit.rule(f"Config Manager for {config_manager.get('name')}")
     cit.info(f"Path: {config_manager.get('path')}")
     if dependencies := config_manager.get('install'):
         cit.info(f"Dependencies: {[package.get('name') for package in dependencies]}")
     if configlets := config_manager.get("config"):
         cit.info(f"Configs: {[configlet.get('name') for configlet in configlets]}")
 
     # install dependencies
     if dependencies and not ensure_packages(dependencies):
-        _soft_raise("Failed to install dependencies!")
+        _raise("Failed to install dependencies!")
 
     # update config files
     if configlets:
         for configlet in configlets:
             cit.start()
             cit.title(f"Configurating {configlet.get('name')}")
             cit.info(f"Source: `{configlet.get('src')}`")
@@ -206,21 +204,20 @@
                         continue
                 else:
                     cit.info(f"Config file for `{configlet.get('name')}` is up-to-date!")
                     continue
             cct.copy_file(src, dst, backup=True, ensure=True, msgout=cit.info)
 
 
-def run_all_configmanager(filename: str = CMGR_PROFILE_FILENAME, root: str = cct.get_path(__file__).parent):
+def run_all_configmanager(filename: str = CMGR_PROFILE_FILENAME, root: str = cct.get_path(__file__).parent) -> None:
     avail_cmgr_profiles: list[cct.Path] = discover_cmgr_confs(filename, root)
     if len(avail_cmgr_profiles) == 0:
         cit.warn("No cmgr config file found!")
     elif len(avail_cmgr_profiles) == 1 and cct.get_path(avail_cmgr_profiles[0]).parent == root:
         config_manager = get_configmanager(avail_cmgr_profiles[0])
         run_configmanager(config_manager)
     else:
         cit.ask("Which cmgr to use?")
         cmgr_conf_paths = cit.get_choices(avail_cmgr_profiles, allable=True, exitable=True)
         for cmgr_conf_path in cmgr_conf_paths:
             config_manager = get_configmanager(cmgr_conf_path)
             run_configmanager(config_manager)
-    cit.pause()
```

### Comparing `cmgr-0.0.4/cmgr/command_line.py` & `cmgr-0.0.7/cmgr/command_line.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import cmgr
 
 
 @click.group(invoke_without_command=True)
 @click.option("-p", "--profile", "profile", default=None, help="The path of the cmgr profile file.")
 @click.option("-n", "--name", "filename", default=cmgr.CMGR_PROFILE_FILENAME, help="The filename of the cmgr profile file.")
 @click.option("-r", "--root", "root", default=os.getcwd(), help="The root directory to discover config manager conf files.")
+@click.version_option(version=cmgr.__version__)
 @click.pass_context
 def main(context: click.Context = None, profile: str = None, root: str = os.getcwd(), filename: str = cmgr.CMGR_PROFILE_FILENAME):
     if context.invoked_subcommand is None:
         if not profile:
             return cmgr.run_all_configmanager(root=root, filename=filename)
         else:
             return cmgr.run_configmanager(profile)
@@ -53,9 +54,15 @@
     }
     if name:
         cmgr_info["name"] = name
     config_manager = cmgr.make_configmanager(cmgr_info)
     return cmgr.run_configmanager(config_manager)
 
 
+@click.version_option()
+@click.command()
+def version():
+    click.echo(cmgr.__version__)
+
+
 if __name__ == "__main__":
     main()
```

### Comparing `cmgr-0.0.4/pyproject.toml` & `cmgr-0.0.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cmgr-0.0.4/tests/test_cmgr.py` & `cmgr-0.0.7/tests/test_cmgr.py`

 * *Files identical despite different names*

