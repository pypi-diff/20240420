# Comparing `tmp/snapshooter-1.0.7.tar.gz` & `tmp/snapshooter-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snapshooter-1.0.7.tar", last modified: Wed Apr 17 09:04:27 2024, max compression
+gzip compressed data, was "snapshooter-1.0.8.tar", last modified: Fri Apr 19 21:39:22 2024, max compression
```

## Comparing `snapshooter-1.0.7.tar` & `snapshooter-1.0.8.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:04:27.846211 snapshooter-1.0.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-17 09:04:09.000000 snapshooter-1.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4764 2024-04-17 09:04:27.846211 snapshooter-1.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4281 2024-04-17 09:04:09.000000 snapshooter-1.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 09:04:27.846211 snapshooter-1.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      986 2024-04-17 09:04:09.000000 snapshooter-1.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:04:27.846211 snapshooter-1.0.7/snapshooter/
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-17 09:04:18.000000 snapshooter-1.0.7/snapshooter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8239 2024-04-17 09:04:09.000000 snapshooter-1.0.7/snapshooter/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     4537 2024-04-17 09:04:09.000000 snapshooter-1.0.7/snapshooter/fsspec_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      714 2024-04-17 09:04:09.000000 snapshooter-1.0.7/snapshooter/jsonl_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-17 09:04:09.000000 snapshooter-1.0.7/snapshooter/logging_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    35326 2024-04-17 09:04:09.000000 snapshooter-1.0.7/snapshooter/snapshooter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:04:27.846211 snapshooter-1.0.7/snapshooter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4764 2024-04-17 09:04:27.000000 snapshooter-1.0.7/snapshooter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-17 09:04:27.000000 snapshooter-1.0.7/snapshooter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 09:04:27.000000 snapshooter-1.0.7/snapshooter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-17 09:04:27.000000 snapshooter-1.0.7/snapshooter.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-17 09:04:27.000000 snapshooter-1.0.7/snapshooter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-17 09:04:27.000000 snapshooter-1.0.7/snapshooter.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:04:27.846211 snapshooter-1.0.7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 09:04:09.000000 snapshooter-1.0.7/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-17 09:04:09.000000 snapshooter-1.0.7/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     6417 2024-04-17 09:04:09.000000 snapshooter-1.0.7/tests/test_fsspec_snapshooter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-17 09:04:09.000000 snapshooter-1.0.7/tests/test_fsspec_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:39:22.589535 snapshooter-1.0.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-19 21:39:06.000000 snapshooter-1.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4764 2024-04-19 21:39:22.589535 snapshooter-1.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4281 2024-04-19 21:39:06.000000 snapshooter-1.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 21:39:22.589535 snapshooter-1.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-04-19 21:39:06.000000 snapshooter-1.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:39:22.589535 snapshooter-1.0.8/snapshooter/
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-19 21:39:14.000000 snapshooter-1.0.8/snapshooter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9614 2024-04-19 21:39:06.000000 snapshooter-1.0.8/snapshooter/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4537 2024-04-19 21:39:06.000000 snapshooter-1.0.8/snapshooter/fsspec_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-04-19 21:39:06.000000 snapshooter-1.0.8/snapshooter/jsonl_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-19 21:39:06.000000 snapshooter-1.0.8/snapshooter/logging_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36137 2024-04-19 21:39:06.000000 snapshooter-1.0.8/snapshooter/snapshooter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-19 21:39:06.000000 snapshooter-1.0.8/snapshooter/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:39:22.589535 snapshooter-1.0.8/snapshooter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4764 2024-04-19 21:39:22.000000 snapshooter-1.0.8/snapshooter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-19 21:39:22.000000 snapshooter-1.0.8/snapshooter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 21:39:22.000000 snapshooter-1.0.8/snapshooter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-19 21:39:22.000000 snapshooter-1.0.8/snapshooter.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-19 21:39:22.000000 snapshooter-1.0.8/snapshooter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-19 21:39:22.000000 snapshooter-1.0.8/snapshooter.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:39:22.589535 snapshooter-1.0.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 21:39:06.000000 snapshooter-1.0.8/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-19 21:39:06.000000 snapshooter-1.0.8/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6485 2024-04-19 21:39:06.000000 snapshooter-1.0.8/tests/test_fsspec_snapshooter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-19 21:39:06.000000 snapshooter-1.0.8/tests/test_fsspec_utils.py
```

### Comparing `snapshooter-1.0.7/LICENSE` & `snapshooter-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `snapshooter-1.0.7/PKG-INFO` & `snapshooter-1.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snapshooter
-Version: 1.0.7
+Version: 1.0.8
 Summary: Provides a set of utilities for comparing and backing up data on different filesystems
 Home-page: https://github.com/jeromerg/snapshooter
 Author: jeromerg
 Author-email: jeromerg@gmx.net
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `snapshooter-1.0.7/README.md` & `snapshooter-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `snapshooter-1.0.7/setup.py` & `snapshooter-1.0.8/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -22,14 +22,15 @@
         "Operating System :: OS Independent",
     ],
     install_requires=[
         'fsspec',
         'pandas',
         'tabulate',
         'typer[all]',
+        'colorlog',
         'tzlocal',
     ],
     entry_points={
         'console_scripts': [
             'snapshooter=snapshooter.cli:main_cli',
         ],
     },
```

### Comparing `snapshooter-1.0.7/snapshooter/cli.py` & `snapshooter-1.0.8/snapshooter/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,56 @@
 import json
 import logging
+import sys
 from dataclasses import dataclass
 from datetime import datetime
 from enum import Enum
-from typing import List
+from typing import List, Literal
+import colorlog
 
 import fsspec
 import typer
 from typing_extensions import Annotated
-
 from snapshooter import Heap, Snapshooter, convert_snapshot_to_df, compare_snapshots as compare_snapshots_
+from snapshooter.fsspec_utils import natural_sort_key
+
+
+class LogLevel(str, Enum):
+    CRITICAL = "CRITICAL"
+    ERROR    = "ERROR"
+    WARNING  = "WARNING"
+    INFO     = "INFO"
+    DEBUG    = "DEBUG"
+    NONE     = "NONE"
+    
+
+def setup_logging(loglevel: LogLevel = "INFO"):    
+    if loglevel == "NONE":
+        return
+    
+    loglevel_value = getattr(logging, loglevel.upper())
+    
+    formatter = colorlog.ColoredFormatter(
+        '%(log_color)s%(asctime)s %(levelname)-8s %(name)s - %(message)s', 
+        datefmt="%H:%M:%S",
+        stream=sys.stderr
+    )
+    handler = logging.StreamHandler()
+    logger = logging.getLogger()
+    handler.setFormatter(formatter)
+    logger.addHandler(handler)
+    logger.setLevel(loglevel_value)
+    handler.setLevel(loglevel_value)
+
+    # shift logging for azure.core.pipeline.policies.http_logging_policy (if root logger is set to INFO, then set this to WARNING and so one)
+    logging.getLogger("azure.core.pipeline.policies.http_logging_policy").setLevel(loglevel_value + 10)
+
 
-logging.basicConfig(
-    level=logging.INFO, 
-    # format: HH:MM:SS (UTC) - level - name - message
-    format="%(asctime)s (%(levelname)s) - %(name)s - %(message)s",
-)
-                    
 log = logging.getLogger(__name__)
 
-# get root logger
-root_logger = logging.getLogger()
-# shift logging for azure.core.pipeline.policies.http_logging_policy (if root logger is set to INFO, then set this to WARNING and so one)
-logging.getLogger("azure.core.pipeline.policies.http_logging_policy").setLevel(root_logger.getEffectiveLevel() + 10)
 
 main_cli = typer.Typer()
 
 
 @dataclass
 class SharedConfig:
     root_dir             : str
@@ -47,15 +71,18 @@
     heap_storage_options    : Annotated[str, typer.Option(envvar="HEAP_STORAGE_OPTIONS"    , help="Additional storage options to pass to fsspec heap_dir file system. expected JSON string")] = None,
     snap_storage_options    : Annotated[str, typer.Option(envvar="SNAP_STORAGE_OPTIONS"    , help="Additional storage options to pass to fsspec snap_dir file system. expected JSON string")] = None,
     parallel_copy_to_heap   : Annotated[int, typer.Option(envvar="PARALLEL_COPY_TO_HEAP"   , help="Number of parallel threads to use for copying files to heap")] = 20,
     parallel_copy_to_file   : Annotated[int, typer.Option(envvar="PARALLEL_COPY_TO_FILE"   , help="Number of parallel threads to use for copying files to file")] = 20,
     parallel_delete_in_file : Annotated[int, typer.Option(envvar="PARALLEL_DELETE_IN_FILE" , help="Number of parallel threads to use for deleting files in file")] = 20,
     parallel_listing        : Annotated[int, typer.Option(envvar="PARALLEL_LISTING"        , help="Number of parallel threads to use for listing files in file")] = 20,
     parallel_heap_listing   : Annotated[int, typer.Option(envvar="PARALLEL_HEAP_LISTING"   , help="Number of parallel threads to use for listing files in heap")] = 20,
+    loglevel                : Annotated[LogLevel, typer.Option(envvar="LOGLEVEL"           , help="The log level to use. Default is INFO.")] = "INFO",
 ):
+    setup_logging(loglevel)
+    
     file_storage_options_dict = json.loads(file_storage_options or "{}")
     heap_storage_options_dict = json.loads(heap_storage_options or "{}")
     snap_storage_options_dict = json.loads(snap_storage_options or "{}")
 
     file_fs, file_root = fsspec.url_to_fs(file_root, **file_storage_options_dict)
     heap_fs, heap_root = fsspec.url_to_fs(heap_root, **heap_storage_options_dict)
     snap_fs, snap_root = fsspec.url_to_fs(snap_root, **snap_storage_options_dict)
@@ -84,46 +111,59 @@
 @main_cli.command()
 def make_snapshot(
     ctx                    : typer.Context,
     save_snapshot          : Annotated[bool, typer.Option(help="Whether to save the snapshot or not. If False, the snapshot is not saved, but the snapshot is returned as a list of dictionaries. Default is True.")] = True,
     download_missing_files : Annotated[bool, typer.Option(help="Whether to download missing files or not. If True, missing files are downloaded. Remark: files with unknown md5 will still be required to be downloaded. Default is True.")] = True,
 ):
     snapshooter: Snapshooter = ctx.obj
-    snapshooter.make_snapshot(
+    snap, ts, path = snapshooter.make_snapshot(
         save_snapshot=save_snapshot,
         download_missing_files=download_missing_files
     )
+    print(path)
 
 
 @main_cli.command()
 def restore_snapshot(
     ctx                  : typer.Context,
-    path                 : Annotated[str, typer.Argument(help="The path to the snapshot file to restore. If not set, then it will look for the latest snapshot available, that fulfills the --latest timestamp if provided")] = None,
-    latest               : Annotated[str, typer.Argument(help="If set, then look for the latest snapshot before or at this timestamp. Expected format is 'YYYY-MM-DD' or 'YYYY-MM-DDTHH:MM:SS[offset]'.")] = None,
+    path                 : Annotated[str, typer.Option(help="The path to the snapshot file to restore. If not set, then it will look for the latest snapshot available, that fulfills the --latest timestamp if provided")] = None,
+    latest               : Annotated[str, typer.Option(help="If set, then look for the latest snapshot before or at this timestamp. Expected format is 'YYYY-MM-DD' or 'YYYY-MM-DDTHH:MM:SS[offset]'.")] = None,
     save_snapshot_before : Annotated[bool, typer.Option(help="Whether to save the current state into a 'backup' snapshot or not. Default is True.")] = True,
     save_snapshot_after  : Annotated[bool, typer.Option(help="Whether to save the restored state into a 'backup' snapshot or not. Default is True.")] = False,
 ):
     snapshooter: Snapshooter = ctx.obj
     latest_timestamp = datetime.fromisoformat(latest) if latest is not None else None
     snapshooter.restore_snapshot(
         snapshot_to_restore=path,
         latest_timestamp=latest_timestamp,
         save_snapshot_before=save_snapshot_before,
         save_snapshot_after=save_snapshot_after,
     )
 
 
+class SortOrder(str, Enum):
+    ASC  = "asc"
+    DESC = "desc"
+
+
 @main_cli.command()
 def list_snapshots(
     ctx: typer.Context,
+    limit: Annotated[int, typer.Option(help="The number of snapshots to list. Default is 10.")] = 10,
+    offset: Annotated[int, typer.Option(help="The offset to start listing snapshots. Default is 0.")] = 0,
+    order: Annotated[SortOrder, typer.Option(help="The order to list snapshots. Default is 'desc'.")] = "desc"
 ):
     snapshooter: Snapshooter = ctx.obj
     snapshot_paths = snapshooter.get_snapshot_paths()
+    snapshot_paths = sorted(snapshot_paths, key=natural_sort_key, reverse=(order == "desc"))
+    snapshot_paths = snapshot_paths[offset:offset+limit]
     for snapshot_path in snapshot_paths:
-        typer.echo(snapshot_path)
+        print(snapshot_path)
+    if offset + limit < len(snapshot_paths):
+        print("...")
 
 
 class DiffState(Enum):
     ONLY_LEFT = "only_left"
     ONLY_RIGHT = "only_right"
     DIFFERENT = "different"
     EQUAL = "equal"
```

### Comparing `snapshooter-1.0.7/snapshooter/fsspec_utils.py` & `snapshooter-1.0.8/snapshooter/fsspec_utils.py`

 * *Files identical despite different names*

### Comparing `snapshooter-1.0.7/snapshooter/jsonl_utils.py` & `snapshooter-1.0.8/snapshooter/jsonl_utils.py`

 * *Files identical despite different names*

### Comparing `snapshooter-1.0.7/snapshooter/snapshooter.py` & `snapshooter-1.0.8/snapshooter/snapshooter.py`

 * *Files 2% similar despite different names*

```diff
@@ -125,25 +125,36 @@
         """ Create a new Snapshooter instance.
 
         :param heap_fs: The file system of the heap files.
         :param heap_root: The root directory of the heap files.
         """
         self.heap_fs   = _coerce_fs(heap_fs)
         self.heap_root = _coerce_root_dir(heap_fs, heap_root)
-        # Get all heap files
-        log.info(f"List out heap files in {self.heap_root}")
-        lister = ParallelLister(
-            fs=self.heap_fs,
-            root=self.heap_root,
-            parallel_file_listing=parallel_listing,
-        )
-        heap_file_paths = [fi["name"] for fi in lister.list_files()]
-        # basename WITHOUT EXTENSION corresponds to the md5
-        self.heap_md5s = set([os.path.basename(p).split(".")[0] for p in heap_file_paths])
-        log.info(f"Heap initialized: Found {len(self.heap_md5s)} files in heap")
+        self.parallel_listing = parallel_listing
+        self._heap_md5s : Set[str] | None = None
+
+    def load_md5s_if_not_yet_loaded(self):
+        # this call triggers the initialization of the heap_md5s if not done yet
+        dummy = self.heap_md5s
+        
+    @property
+    def heap_md5s(self) -> Set[str]:        
+        if self._heap_md5s is None:
+            # Get all heap files
+            log.info(f"List out heap files in {self.heap_root}")
+            lister = ParallelLister(
+                fs=self.heap_fs,
+                root=self.heap_root,
+                parallel_file_listing=self.parallel_listing,
+            )
+            heap_file_paths = [fi["name"] for fi in lister.list_files()]
+            # basename WITHOUT EXTENSION corresponds to the md5
+            self._heap_md5s = set([os.path.basename(p).split(".")[0] for p in heap_file_paths])
+            log.info(f"Heap initialized: Found {len(self._heap_md5s)} files in heap")
+        return self._heap_md5s
 
     def add_file_to_heap(self, f: BufferedReader, check_interrupted_fn: Callable) -> str:
         temp_file_path = f"{self.heap_root}/temp/{uuid.uuid4()}.gz"
         self.heap_fs.makedirs(f"{self.heap_root}/temp", exist_ok=True)
         md5_digester = hashlib.md5()
         try:
             with (
@@ -256,15 +267,15 @@
     def get_snapshot_paths(self) -> list[str]:
         """ Get all snapshot paths from the snapshot file system.
 
         :return: The paths of all snapshots sorted by path name (descending).
         """
         snap_glob      = FMT_PLACEHOLDER_REGEX.sub("*", SNAP_PATH_FMT)
         snapshot_files = self.snap_fs.glob(f"{self.snap_root}/{snap_glob}")
-        return snapshot_files
+        return list(reversed(snapshot_files))
 
     def try_get_snapshot_path(
         self, 
         latest_timestamp: datetime.datetime | None = None
     ) -> str | None:
         """ Tries to get the latest snapshot path from the snapshot file system. If before is given, tries to get the latest snapshot path which was created before or at the given timestamp.
 
@@ -381,15 +392,17 @@
             if md5 is not None:
                 src_file_info["md5"] = md5
 
     def make_snapshot(
         self,
         save_snapshot: bool = True,
         download_missing_files: bool = True
-    ) -> tuple[List[dict], datetime.datetime]:
+    ) -> tuple[List[dict], datetime.datetime, str | None]:
+        self.heap.load_md5s_if_not_yet_loaded()  # cleaner logging if done here
+        
         timestamp = datetime.datetime.now(datetime.timezone.utc)
         log.info(f"Making Snapshot with timestamp = '{timestamp}'")
 
         _create_folder_if_not_exists(self.file_fs, self.file_root, "root folder")
         _create_folder_if_not_exists(self.snap_fs, self.snap_root, "snapshot root folder")
         
         log.info(f"Retrieving prior snapshot to optimize download...")
@@ -425,17 +438,18 @@
                 heap                   = self.heap,
                 parallelization        = self.parallel_copy_to_heap,
                 snapshot_files_by_name = snapshot_files_by_name,
             )
             downloader.process_files()
 
         if save_snapshot:
-            self._save_snapshot(snapshot, timestamp)
-
-        return snapshot, timestamp
+            snapshot_filepath = self._save_snapshot(snapshot, timestamp)
+        else:
+            snapshot_filepath = None
+        return snapshot, timestamp, snapshot_filepath
 
     def _save_snapshot(
         self,
         snapshot: List[dict],
         snapshot_timestamp: datetime
     ) -> str:
         """Save the given snapshot to the snapshot file system.
@@ -457,14 +471,16 @@
     def restore_snapshot(
         self,
         snapshot_to_restore  : str | List[dict] | pd.DataFrame | None = None,
         latest_timestamp     : datetime.datetime = None,
         save_snapshot_before : bool = True,
         save_snapshot_after  : bool = False,
     ):
+        self.heap.load_md5s_if_not_yet_loaded()  # cleaner logging if done here
+
         log.info("Loading snapshot to restore")
         # read snapshot depending on the type of snapshot_to_restore
         if snapshot_to_restore is None:
             snap = self.read_snapshot(latest_timestamp=latest_timestamp)
             df_snapshot_to_restore = convert_snapshot_to_df(snap)
         elif isinstance(snapshot_to_restore, str):
             snap = self.read_snapshot(snapshot_path=snapshot_to_restore)
@@ -474,15 +490,15 @@
         elif isinstance(snapshot_to_restore, pd.DataFrame):
             df_snapshot_to_restore = snapshot_to_restore
         else:
             raise Exception(f"restore_snapshot: Unknown type {type(snapshot_to_restore)} for snapshot_to_restore. Expected: pd.DataFrame, List[dict]")
         log.info(f"Snapshot to restore loaded")
 
         log.info("Making current snapshot to apply diff to")
-        current_snapshot, _ = self.make_snapshot(save_snapshot=save_snapshot_before, download_missing_files=True)
+        current_snapshot, _, _ = self.make_snapshot(save_snapshot=save_snapshot_before, download_missing_files=True)
         log.info(f"Current snapshot made")
         df_current_snapshot = convert_snapshot_to_df(current_snapshot)
 
         df_diff = compare_snapshots(df_snapshot_to_restore, df_current_snapshot)
 
         if df_diff["status"].eq("equal").all():
             log.info(f"No files to restore, all {len(df_diff)} files are equal")
@@ -497,14 +513,16 @@
         # Remark: There is space for optimization, because the snapshot 
         # could be built from the snapshot before and the diff + missing file metadata for
         # the files that were not in the snapshot before.
         if save_snapshot_after:
             self.make_snapshot(save_snapshot=True, download_missing_files=True)
 
     def apply_diff(self, df_diff: pd.DataFrame):
+        self.heap.load_md5s_if_not_yet_loaded()  # cleaner logging if done here
+
         if not isinstance(df_diff, pd.DataFrame):
             raise Exception(f"apply_diff: Unknown type {type(df_diff)} for diff. Expected: pd.DataFrame")
 
         relative_path_only_left  = set(df_diff[df_diff["status"] == "only_left"].index)
         relative_path_only_right = set(df_diff[df_diff["status"] == "only_right"].index)
         relative_path_different  = set(df_diff[df_diff["status"] == "different"].index)
```

### Comparing `snapshooter-1.0.7/snapshooter.egg-info/PKG-INFO` & `snapshooter-1.0.8/snapshooter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snapshooter
-Version: 1.0.7
+Version: 1.0.8
 Summary: Provides a set of utilities for comparing and backing up data on different filesystems
 Home-page: https://github.com/jeromerg/snapshooter
 Author: jeromerg
 Author-email: jeromerg@gmx.net
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `snapshooter-1.0.7/tests/test_fsspec_snapshooter.py` & `snapshooter-1.0.8/tests/test_fsspec_snapshooter.py`

 * *Files 5% similar despite different names*

```diff
@@ -49,17 +49,18 @@
     snapshooter = Snapshooter(
         file_fs   = fs,
         file_root = original_file_root,
         snap_fs   = fs,
         snap_root = snap_root,
         heap      = heap,
     )
-    snap, timestamp = snapshooter.make_snapshot()
+    snap, timestamp, path = snapshooter.make_snapshot()
     assert timestamp is not None
     assert snap is not None
+    assert path is not None
     assert isinstance(timestamp, datetime)
     assert isinstance(snap, list)
     assert len(snap) == 3
     # result is expected to be sorted by name (relative path to root)
     assert snap[0]["name"] == "empty_file.txt"
     assert snap[1]["name"] == "subfolder/another_text_file.txt"
     assert snap[2]["name"] == "text_file.txt"
@@ -121,17 +122,18 @@
     snapshooter = Snapshooter(
         file_fs   = fs,
         file_root = changed_file_root,
         snap_fs   = fs,
         snap_root = snap_root,
         heap      = heap,
     )
-    snap, timestamp = snapshooter.make_snapshot()
+    snap, timestamp, path = snapshooter.make_snapshot()
     assert timestamp is not None
     assert snap is not None
+    assert path is not None
     assert isinstance(timestamp, datetime)
     assert isinstance(snap, list)
     assert len(snap) == 3
     # result is expected to be sorted by name (relative path to root)
     assert snap[0]["name"] == "empty_file.txt"
     assert snap[1]["name"] == "subfolder/another_text_file.txt"
     assert snap[2]["name"] == "text_file_added.txt"
```

### Comparing `snapshooter-1.0.7/tests/test_fsspec_utils.py` & `snapshooter-1.0.8/tests/test_fsspec_utils.py`

 * *Files identical despite different names*

