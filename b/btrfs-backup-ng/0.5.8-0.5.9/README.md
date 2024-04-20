# Comparing `tmp/btrfs-backup-ng-0.5.8.tar.gz` & `tmp/btrfs-backup-ng-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "btrfs-backup-ng-0.5.8.tar", last modified: Mon Jan 29 22:21:30 2024, max compression
+gzip compressed data, was "btrfs-backup-ng-0.5.9.tar", last modified: Sun Feb 18 19:09:37 2024, max compression
```

## Comparing `btrfs-backup-ng-0.5.8.tar` & `btrfs-backup-ng-0.5.9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 berrym    (1000) berrym    (1000)        0 2024-01-29 22:21:30.622501 btrfs-backup-ng-0.5.8/
--rw-r--r--   0 berrym    (1000) berrym    (1000)     1227 2024-01-25 04:44:42.000000 btrfs-backup-ng-0.5.8/LICENSE
--rw-r--r--   0 berrym    (1000) berrym    (1000)    15576 2024-01-29 22:21:30.622501 btrfs-backup-ng-0.5.8/PKG-INFO
--rw-r--r--   0 berrym    (1000) berrym    (1000)    15080 2024-01-29 22:17:12.000000 btrfs-backup-ng-0.5.8/README.md
--rw-r--r--   0 berrym    (1000) berrym    (1000)      713 2024-01-29 22:16:25.000000 btrfs-backup-ng-0.5.8/pyproject.toml
--rw-r--r--   0 berrym    (1000) berrym    (1000)       38 2024-01-29 22:21:30.622501 btrfs-backup-ng-0.5.8/setup.cfg
--rw-r--r--   0 berrym    (1000) berrym    (1000)       38 2024-01-25 04:44:42.000000 btrfs-backup-ng-0.5.8/setup.py
-drwxr-xr-x   0 berrym    (1000) berrym    (1000)        0 2024-01-29 22:21:30.620501 btrfs-backup-ng-0.5.8/src/
-drwxr-xr-x   0 berrym    (1000) berrym    (1000)        0 2024-01-29 22:21:30.620501 btrfs-backup-ng-0.5.8/src/btrfs_backup_ng/
--rw-r--r--   0 berrym    (1000) berrym    (1000)       74 2024-01-29 22:16:36.000000 btrfs-backup-ng-0.5.8/src/btrfs_backup_ng/__init__.py
--rw-r--r--   0 berrym    (1000) berrym    (1000)    25603 2024-01-29 22:06:21.000000 btrfs-backup-ng-0.5.8/src/btrfs_backup_ng/__main__.py
-drwxr-xr-x   0 berrym    (1000) berrym    (1000)        0 2024-01-29 22:21:30.622501 btrfs-backup-ng-0.5.8/src/btrfs_backup_ng/endpoint/
--rw-r--r--   0 berrym    (1000) berrym    (1000)     2414 2024-01-25 04:44:42.000000 btrfs-backup-ng-0.5.8/src/btrfs_backup_ng/endpoint/__init__.py
--rw-r--r--   0 berrym    (1000) berrym    (1000)    13764 2024-01-28 00:41:30.000000 btrfs-backup-ng-0.5.8/src/btrfs_backup_ng/endpoint/common.py
--rw-r--r--   0 berrym    (1000) berrym    (1000)     1635 2024-01-28 00:41:30.000000 btrfs-backup-ng-0.5.8/src/btrfs_backup_ng/endpoint/local.py
--rw-r--r--   0 berrym    (1000) berrym    (1000)      599 2024-01-25 04:44:42.000000 btrfs-backup-ng-0.5.8/src/btrfs_backup_ng/endpoint/shell.py
--rw-r--r--   0 berrym    (1000) berrym    (1000)     5647 2024-01-28 00:41:30.000000 btrfs-backup-ng-0.5.8/src/btrfs_backup_ng/endpoint/ssh.py
--rw-r--r--   0 berrym    (1000) berrym    (1000)     9571 2024-01-28 00:41:30.000000 btrfs-backup-ng-0.5.8/src/btrfs_backup_ng/util.py
-drwxr-xr-x   0 berrym    (1000) berrym    (1000)        0 2024-01-29 22:21:30.622501 btrfs-backup-ng-0.5.8/src/btrfs_backup_ng.egg-info/
--rw-r--r--   0 berrym    (1000) berrym    (1000)    15576 2024-01-29 22:21:30.000000 btrfs-backup-ng-0.5.8/src/btrfs_backup_ng.egg-info/PKG-INFO
--rw-r--r--   0 berrym    (1000) berrym    (1000)      585 2024-01-29 22:21:30.000000 btrfs-backup-ng-0.5.8/src/btrfs_backup_ng.egg-info/SOURCES.txt
--rw-r--r--   0 berrym    (1000) berrym    (1000)        1 2024-01-29 22:21:30.000000 btrfs-backup-ng-0.5.8/src/btrfs_backup_ng.egg-info/dependency_links.txt
--rw-r--r--   0 berrym    (1000) berrym    (1000)       66 2024-01-29 22:21:30.000000 btrfs-backup-ng-0.5.8/src/btrfs_backup_ng.egg-info/entry_points.txt
--rw-r--r--   0 berrym    (1000) berrym    (1000)        5 2024-01-29 22:21:30.000000 btrfs-backup-ng-0.5.8/src/btrfs_backup_ng.egg-info/requires.txt
--rw-r--r--   0 berrym    (1000) berrym    (1000)       16 2024-01-29 22:21:30.000000 btrfs-backup-ng-0.5.8/src/btrfs_backup_ng.egg-info/top_level.txt
+drwxr-xr-x   0 berrym    (1000) berrym    (1000)        0 2024-02-18 19:09:37.406484 btrfs-backup-ng-0.5.9/
+-rw-r--r--   0 berrym    (1000) berrym    (1000)     1227 2024-01-25 04:44:42.000000 btrfs-backup-ng-0.5.9/LICENSE
+-rw-r--r--   0 berrym    (1000) berrym    (1000)    15576 2024-02-18 19:09:37.406484 btrfs-backup-ng-0.5.9/PKG-INFO
+-rw-r--r--   0 berrym    (1000) berrym    (1000)    15081 2024-02-18 19:09:22.000000 btrfs-backup-ng-0.5.9/README.md
+-rw-r--r--   0 berrym    (1000) berrym    (1000)      704 2024-02-18 19:09:22.000000 btrfs-backup-ng-0.5.9/pyproject.toml
+-rw-r--r--   0 berrym    (1000) berrym    (1000)       38 2024-02-18 19:09:37.406484 btrfs-backup-ng-0.5.9/setup.cfg
+-rw-r--r--   0 berrym    (1000) berrym    (1000)       38 2024-01-25 04:44:42.000000 btrfs-backup-ng-0.5.9/setup.py
+drwxr-xr-x   0 berrym    (1000) berrym    (1000)        0 2024-02-18 19:09:37.404484 btrfs-backup-ng-0.5.9/src/
+drwxr-xr-x   0 berrym    (1000) berrym    (1000)        0 2024-02-18 19:09:37.404484 btrfs-backup-ng-0.5.9/src/btrfs_backup_ng/
+-rw-r--r--   0 berrym    (1000) berrym    (1000)       74 2024-02-18 19:09:22.000000 btrfs-backup-ng-0.5.9/src/btrfs_backup_ng/__init__.py
+-rw-r--r--   0 berrym    (1000) berrym    (1000)    25836 2024-02-18 19:09:22.000000 btrfs-backup-ng-0.5.9/src/btrfs_backup_ng/__main__.py
+drwxr-xr-x   0 berrym    (1000) berrym    (1000)        0 2024-02-18 19:09:37.406484 btrfs-backup-ng-0.5.9/src/btrfs_backup_ng/endpoint/
+-rw-r--r--   0 berrym    (1000) berrym    (1000)     2414 2024-01-25 04:44:42.000000 btrfs-backup-ng-0.5.9/src/btrfs_backup_ng/endpoint/__init__.py
+-rw-r--r--   0 berrym    (1000) berrym    (1000)    13830 2024-02-16 17:47:20.000000 btrfs-backup-ng-0.5.9/src/btrfs_backup_ng/endpoint/common.py
+-rw-r--r--   0 berrym    (1000) berrym    (1000)     1695 2024-02-16 17:47:20.000000 btrfs-backup-ng-0.5.9/src/btrfs_backup_ng/endpoint/local.py
+-rw-r--r--   0 berrym    (1000) berrym    (1000)      599 2024-01-25 04:44:42.000000 btrfs-backup-ng-0.5.9/src/btrfs_backup_ng/endpoint/shell.py
+-rw-r--r--   0 berrym    (1000) berrym    (1000)     5780 2024-02-16 17:47:20.000000 btrfs-backup-ng-0.5.9/src/btrfs_backup_ng/endpoint/ssh.py
+-rw-r--r--   0 berrym    (1000) berrym    (1000)     9709 2024-02-16 17:47:20.000000 btrfs-backup-ng-0.5.9/src/btrfs_backup_ng/util.py
+drwxr-xr-x   0 berrym    (1000) berrym    (1000)        0 2024-02-18 19:09:37.406484 btrfs-backup-ng-0.5.9/src/btrfs_backup_ng.egg-info/
+-rw-r--r--   0 berrym    (1000) berrym    (1000)    15576 2024-02-18 19:09:37.000000 btrfs-backup-ng-0.5.9/src/btrfs_backup_ng.egg-info/PKG-INFO
+-rw-r--r--   0 berrym    (1000) berrym    (1000)      585 2024-02-18 19:09:37.000000 btrfs-backup-ng-0.5.9/src/btrfs_backup_ng.egg-info/SOURCES.txt
+-rw-r--r--   0 berrym    (1000) berrym    (1000)        1 2024-02-18 19:09:37.000000 btrfs-backup-ng-0.5.9/src/btrfs_backup_ng.egg-info/dependency_links.txt
+-rw-r--r--   0 berrym    (1000) berrym    (1000)       66 2024-02-18 19:09:37.000000 btrfs-backup-ng-0.5.9/src/btrfs_backup_ng.egg-info/entry_points.txt
+-rw-r--r--   0 berrym    (1000) berrym    (1000)        5 2024-02-18 19:09:37.000000 btrfs-backup-ng-0.5.9/src/btrfs_backup_ng.egg-info/requires.txt
+-rw-r--r--   0 berrym    (1000) berrym    (1000)       16 2024-02-18 19:09:37.000000 btrfs-backup-ng-0.5.9/src/btrfs_backup_ng.egg-info/top_level.txt
```

### Comparing `btrfs-backup-ng-0.5.8/LICENSE` & `btrfs-backup-ng-0.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `btrfs-backup-ng-0.5.8/PKG-INFO` & `btrfs-backup-ng-0.5.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: btrfs-backup-ng
-Version: 0.5.8
+Version: 0.5.9
 Summary: Intelligent, feature-rich backups for btrfs
 Author-email: Michael Berry <trismegustis@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/berrym/btrfs-backup-ng
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
@@ -40,15 +40,15 @@
 written by Chris Lawrence. Since then, most of the code has been
 refactored and many new features were added before this repository has
 been transferred to Robert Schindler. Many thanks to Chris for his work. The old code
 base has been tagged with `legacy`. If, for any reason, you want to
 continue using it and miss the new features, you can check that out.
 
 Latest release  
-v0.5.8
+v0.5.9
 
 Downloads  
 <http://pypi.python.org/pypi/btrfs_backup_ng>
 
 Source  
 <https://github.com/berrym/btrfs-backup-ng>
 
@@ -122,15 +122,15 @@
 Note: This package now uses a pyproject.toml based build as outlined in
 PEP 517 and PEP 621.
 
 Clone this git repository
 
     $ git clone https://github.com/berrym/btrfs-backup-ng.git
     $ cd btrfs-backup-ng
-    $ git checkout tags/v0.5.8  # optionally checkout a specific version
+    $ git checkout tags/v0.5.9  # optionally checkout a specific version
     $ python3 -m venv /path/to/btrfs-backup-ng/venv # optionally use venv
     $ sh /path/to/btrfs-backup-ng/venv/bin/activate # using venv
     $ python3 -m build
     # using venv
     $ python3 -m pip install .
     # or 
     $ sudo python3 -m pip install .
```

### Comparing `btrfs-backup-ng-0.5.8/README.md` & `btrfs-backup-ng-0.5.9/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 written by Chris Lawrence. Since then, most of the code has been
 refactored and many new features were added before this repository has
 been transferred to Robert Schindler. Many thanks to Chris for his work. The old code
 base has been tagged with `legacy`. If, for any reason, you want to
 continue using it and miss the new features, you can check that out.
 
 Latest release  
-v0.5.8
+v0.5.9
 
 Downloads  
 <http://pypi.python.org/pypi/btrfs_backup_ng>
 
 Source  
 <https://github.com/berrym/btrfs-backup-ng>
 
@@ -107,15 +107,15 @@
 Note: This package now uses a pyproject.toml based build as outlined in
 PEP 517 and PEP 621.
 
 Clone this git repository
 
     $ git clone https://github.com/berrym/btrfs-backup-ng.git
     $ cd btrfs-backup-ng
-    $ git checkout tags/v0.5.8  # optionally checkout a specific version
+    $ git checkout tags/v0.5.9  # optionally checkout a specific version
     $ python3 -m venv /path/to/btrfs-backup-ng/venv # optionally use venv
     $ sh /path/to/btrfs-backup-ng/venv/bin/activate # using venv
     $ python3 -m build
     # using venv
     $ python3 -m pip install .
     # or 
     $ sudo python3 -m pip install .
@@ -403,8 +403,8 @@
 Copyright © 2023 Michael Berry <trismegustis@gmail.com>\
 Copyright © 2017 Robert Schindler <r.schindler@efficiosoft.com>\
 Copyright © 2014 Chris Lawrence <lawrencc@debian.org>
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![build result](https://build.opensuse.org/projects/home:berrym/packages/btrfs-backup-ng/badge.svg?type=default)](https://build.opensuse.org/package/show/home:berrym/btrfs-backup-ng)
-[![Copr build status](https://copr.fedorainfracloud.org/coprs/mberry/btrfs-backup-ng/package/btrfs-backup-ng/status_image/last_build.png)](https://copr.fedorainfracloud.org/coprs/mberry/btrfs-backup-ng/package/btrfs-backup-ng/)
+[![Copr build status](https://copr.fedorainfracloud.org/coprs/mberry/btrfs-backup-ng/package/btrfs-backup-ng/status_image/last_build.png)](https://copr.fedorainfracloud.org/coprs/mberry/btrfs-backup-ng/package/btrfs-backup-ng/)
```

### Comparing `btrfs-backup-ng-0.5.8/src/btrfs_backup_ng/__main__.py` & `btrfs-backup-ng-0.5.9/src/btrfs_backup_ng/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,33 +26,37 @@
 ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
 CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
 
 import concurrent.futures
 import logging
-import multiprocessing
+
 import os
 import sys
 import time
 from math import inf
 
-from rich import progress
+from rich.console import Console, Group
+from rich.live import Live
+from rich.logging import RichHandler
+from rich.panel import Panel
+from rich.progress import BarColumn, Progress, SpinnerColumn, TimeElapsedColumn
 
 from . import endpoint
 from . import util
 
 
-def send_snapshot(
-    snapshot, destination_endpoint, parent=None, clones=None, no_progress=False
-):
+console = Console()
+
+
+def send_snapshot(snapshot, destination_endpoint, parent=None, clones=None):
     """
     Sends snapshot to destination endpoint, using given parent and clones.
-    It connects the pipes of source and destination together and shows
-    progress data using the pv command.
+    It connects the pipes of source and destination together.
     """
 
     # Now we need to send the snapshot (incrementally, if possible)
     logging.info("Sending %s ...", snapshot)
     if parent:
         logging.info("  Using parent: %s", parent)
     else:
@@ -181,15 +185,16 @@
                 destination_endpoint,
                 parent=parent,
                 clones=clones,
                 **kwargs,
             )
         except util.SnapshotTransferError:
             logging.info(
-                "Keeping %s locked to prevent it from getting removed.", best_snapshot
+                "Keeping %s locked to prevent it from getting removed.",
+                best_snapshot,
             )
         else:
             source_endpoint.set_lock(best_snapshot, destination_id, False)
             if parent:
                 source_endpoint.set_lock(parent, destination_id, False, parent=True)
             destination_endpoint.add_snapshot(best_snapshot)
             destination_snapshots = destination_endpoint.list_snapshots()
@@ -416,27 +421,26 @@
             file=sys.stderr,
         )
         raise util.AbortError()
 
     return options
 
 
-def run_task(task):
+def run_task(options):
     """Create a list of tasks to run."""
 
-    options = parse_options(task)
     logging.basicConfig(
-        format="%(asctime)s  [%(levelname)-5s]  %(message)s",
+        format="%(message)s",
         datefmt="%H:%M:%S",
         level=options["verbosity"].upper(),
+        handlers=[RichHandler(console=console)],
     )
 
     # applying shortcuts
     if "quiet" in options:
-        options["no_progress"] = True
         options["verbosity"] = "warning"
     if "latest_only" in options:
         options["num_snapshots"] = 1
 
     logging.info(util.log_heading(f"Started at {time.ctime()}"))
 
     logging.debug(util.log_heading("Settings"))
@@ -447,30 +451,30 @@
 
     if "snapshot_prefix" in options:
         snapshot_prefix = options["snapshot_prefix"]
     else:
         snapshot_prefix = ""
 
     logging.debug("Enable btrfs debugging: %r", options["btrfs_debug"])
-    logging.debug("Don't display progress: %r", options["no_progress"])
     logging.debug("Don't take a new snapshot: %r", options["no_snapshot"])
     logging.debug("Number of snapshots to keep: %d", options["num_snapshots"])
     logging.debug(
         "Number of backups to keep: %s",
         (str(options["num_backups"]) if options["num_backups"] > 0 else "Any"),
     )
     logging.debug("Snapshot folder: %s", snapshot_directory)
     logging.debug("Snapshot prefix: %s", snapshot_prefix if snapshot_prefix else None)
     logging.debug("Don't transfer snapshots: %r", options["no_transfer"])
     logging.debug("Don't send incrementally: %r", options["no_incremental"])
     logging.debug("Extra SSH config options: %s", options["ssh_opt"])
     logging.debug("Use sudo at SSH remote host: %r", options["ssh_sudo"])
     logging.debug("Run 'btrfs subvolume sync' afterwards: %r", options["sync"])
     logging.debug(
-        "Convert subvolumes to read-write before deletion: %r", options["convert_rw"]
+        "Convert subvolumes to read-write before deletion: %r",
+        options["convert_rw"],
     )
     logging.debug("Remove locks for given destinations: %r", options["remove_locks"])
     logging.debug("Skip filesystem checks: %r", options["skip_fs_checks"])
     logging.debug("Auto add locked destinations: %r", options["locked_destinations"])
 
     # kwargs that are common between all endpoints
     endpoint_kwargs = {
@@ -549,15 +553,14 @@
         for destination_endpoint in destination_endpoints:
             try:
                 sync_snapshots(
                     source_endpoint,
                     destination_endpoint,
                     keep_num_backups=options["num_backups"],
                     no_incremental=options["no_incremental"],
-                    no_progress=options["no_progress"],
                 )
             except util.AbortError as e:
                 logging.error(
                     "Aborting snapshot transfer to %s due to exception.",
                     destination_endpoint,
                 )
                 logging.debug("Exception was: %s", e)
@@ -606,65 +609,90 @@
     """Main function."""
     command_line = ""
     for arg in sys.argv[1:]:
         command_line += f"{arg}  "  # Assume no space => no quotes
 
     tasks = [task.split() for task in command_line.split(":")]
 
+    task_options = []
+
     # make sure we have at least one valid task to complete
-    if len(tasks) == 1:
-        _ = parse_options(tasks[0])
+    for task in tasks:
+        task_options.append(parse_options(task))
 
     # make sure we have root privileges
     elevate_privileges()
 
+    overall_progress = Progress(
+        "[progress.description]{task.description}",
+        BarColumn(),
+        "[progress.percentage]{task.percentage:>3.0f}%",
+        SpinnerColumn(),
+        TimeElapsedColumn(),
+        refresh_per_second=4,
+    )
+
+    tasks_progress = Progress(
+        "{task.description}",
+        BarColumn(),
+        SpinnerColumn(),
+        TimeElapsedColumn(),
+        refresh_per_second=4,
+    )
+
+    progress_group = Group(Panel(tasks_progress), Panel(overall_progress))
+
     try:
-        with progress.Progress(
-            "[progress.description]{task.description}",
-            progress.BarColumn(),
-            "[progress.percentage]{task.percentage:>3.0f}%",
-            progress.TimeRemainingColumn(),
-            progress.TimeElapsedColumn(),
-            refresh_per_second=1,  # bit slower updates
-        ) as progress_bars:
-            futures = []  # keep track of the jobs
-            with multiprocessing.Manager() as manager:
-                # this is the key - we share some state between our
-                # main process and our worker functions
-                _progress = manager.dict()
-                overall_progress_task = progress_bars.add_task(
-                    "[green]All jobs progress:"
+        with Live(progress_group, console=console, refresh_per_second=4):
+            futures = []  # keep track of the concurrent futures
+            task_numbers = []
+            futures_id_map = {}
+
+            with concurrent.futures.ProcessPoolExecutor(max_workers=8) as executor:
+                for n, _ in enumerate(tasks):
+                    futures.append(executor.submit(run_task, task_options[n]))
+
+                    task_id = tasks_progress.add_task(
+                        f"[red]task {n}: [cyan]{task_options[n]['source']} -> {task_options[n]['destinations']}",
+                        total=None,
+                        visible=True,
+                    )
+                    task_numbers.append(task_id)
+                    futures_id_map[futures[n]] = task_id
+
+                # Total count of completed tasks
+                total_tasks = len(task_numbers)
+                # tasks_completed = 0
+
+                overall_task_id = overall_progress.add_task(
+                    "[green]All jobs progress:",
+                    total=total_tasks,
+                    visible=True,
                 )
 
-                with concurrent.futures.ProcessPoolExecutor() as executor:
-                    futures = {executor.submit(run_task, task): task for task in tasks}
-
-                    for n in range(len(tasks)):  # iterate over the tasks we need to run
-                        # set visible false, so we don't have a lot of bars all at once:
-                        task_id = progress_bars.add_task(f"task {n}", total=None)
-
-                    # monitor the progress:
-                    while (
-                        tasks_completed := sum([future.done() for future in futures])
-                    ) < len(futures):
-                        progress_bars.update(
-                            overall_progress_task,
-                            completed=tasks_completed,
-                            total=len(futures),
-                        )
-                        for task_id, update_data in _progress.items():
-                            latest = update_data["progress"]
-                            total = update_data["total"]
-                            # update the progress bar for this task:
-                            progress_bars.update(
-                                task_id,
-                                completed=latest,
-                                total=total,
-                                visible=latest < total,
-                            )
-
-                    for future in concurrent.futures.as_completed(futures):
-                        task = futures[future]
-                        result = future.result()
-                        print(f"{task}\nResult: {result}")
+                # monitor the progress
+                for future in concurrent.futures.as_completed(futures):
+                    result = future.result()
+                    task_id = futures_id_map[future]
+                    logging.info(
+                        "Task %d has completed, result: %s",
+                        task_id,
+                        result,
+                    )
+                    tasks_progress.update(
+                        task_id,
+                        description=f"[red]Task {task_id}: [bold yellow]Completed!",
+                        total=1,
+                        completed=1,
+                    )
+                    overall_progress.update(
+                        overall_task_id,
+                        advance=1,
+                    )
+
+            overall_progress.update(
+                overall_task_id,
+                description="[bold yellow]All tasks have finished!",
+                completed=total_tasks,
+            )
     except (util.AbortError, KeyboardInterrupt):
         sys.exit(1)
```

### Comparing `btrfs-backup-ng-0.5.8/src/btrfs_backup_ng/endpoint/__init__.py` & `btrfs-backup-ng-0.5.9/src/btrfs_backup_ng/endpoint/__init__.py`

 * *Files identical despite different names*

### Comparing `btrfs-backup-ng-0.5.8/src/btrfs_backup_ng/endpoint/common.py` & `btrfs-backup-ng-0.5.9/src/btrfs_backup_ng/endpoint/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,15 +57,17 @@
         """Takes a snapshot and returns the created object."""
 
         snapshot = util.Snapshot(self.path, self.snap_prefix, self)
         snapshot_path = snapshot.get_path()
         logging.info("%s -> %s", self.source, snapshot_path)
 
         commands = [
-            self._build_snapshot_cmd(self.source, snapshot_path, readonly=readonly)
+            self._build_snapshot_cmd(
+                self.source, snapshot_path, readonly=readonly
+            )
         ]
 
         # sync disks
         if sync:
             commands.append(self._build_sync_command())
 
         for cmd in self._collapse_commands(commands, abort_on_failure=True):
@@ -86,15 +88,17 @@
         """Calls 'btrfs receive', setting the given pipe as its stdin.
         The receiving process's Popen object is returned."""
 
         cmd = self._build_receive_command(self.path)
         # from WARNING level onwards, hide stdout
         loglevel = logging.getLogger().getEffectiveLevel()
         stdout = subprocess.DEVNULL if loglevel >= logging.WARNING else None
-        return self._exec_command(cmd, method="Popen", stdin=stdin, stdout=stdout)
+        return self._exec_command(
+            cmd, method="Popen", stdin=stdin, stdout=stdout
+        )
 
     def list_snapshots(self, flush_cache=False):
         """Returns a list with all snapshots found at ``self.path``.
         If ``flush_cache`` is not set, cached results will be used
         if available."""
 
         if self.__cached_snapshots is not None and not flush_cache:
@@ -287,15 +291,17 @@
         return cmd
 
     def _build_receive_command(self, destination):
         """Should return a command to receive a snapshot to ``dest``.
         The stream is piped into stdin when the command is running."""
         return ["btrfs", "receive"] + self.btrfs_flags + [destination]
 
-    def _build_deletion_commands(self, snapshots, convert_rw=None, subvolume_sync=None):
+    def _build_deletion_commands(
+        self, snapshots, convert_rw=None, subvolume_sync=None
+    ):
         """Should return a list of commands that, when executed in order,
         delete the given ``snapshots``. ``convert_rw`` and
         ``subvolume_sync`` should be regarded as well."""
 
         if convert_rw is None:
             convert_rw = self.convert_rw
         if subvolume_sync is None:
```

### Comparing `btrfs-backup-ng-0.5.8/src/btrfs_backup_ng/endpoint/local.py` & `btrfs-backup-ng-0.5.9/src/btrfs_backup_ng/endpoint/local.py`

 * *Files 5% similar despite different names*

```diff
@@ -40,12 +40,16 @@
                     raise util.AbortError()
 
         if (
             self.source is not None
             and self.fs_checks
             and not util.is_subvolume(self.source)
         ):
-            logging.error("%s does not seem to be a btrfs subvolume", self.source)
+            logging.error(
+                "%s does not seem to be a btrfs subvolume", self.source
+            )
             raise util.AbortError()
         if self.fs_checks and not util.is_btrfs(self.path):
-            logging.error("%s does not seem to be on a btrfs filesystem", self.path)
+            logging.error(
+                "%s does not seem to be on a btrfs filesystem", self.path
+            )
             raise util.AbortError()
```

### Comparing `btrfs-backup-ng-0.5.8/src/btrfs_backup_ng/endpoint/shell.py` & `btrfs-backup-ng-0.5.9/src/btrfs_backup_ng/endpoint/shell.py`

 * *Files identical despite different names*

### Comparing `btrfs-backup-ng-0.5.8/src/btrfs_backup_ng/endpoint/ssh.py` & `btrfs-backup-ng-0.5.9/src/btrfs_backup_ng/endpoint/ssh.py`

 * *Files 3% similar despite different names*

```diff
@@ -52,15 +52,18 @@
 
     def _prepare(self):
         # check whether ssh is available
         logging.debug("Checking for ssh ...")
         cmd = ["ssh"]
         try:
             util.exec_subprocess(
-                cmd, method="call", stdout=subprocess.DEVNULL, stderr=subprocess.DEVNULL
+                cmd,
+                method="call",
+                stdout=subprocess.DEVNULL,
+                stderr=subprocess.DEVNULL,
             )
         except FileNotFoundError as e:
             logging.debug("  -> got exception: %s", e)
             logging.info("ssh command is not available")
             raise util.AbortError()
 
         logging.debug("  -> ssh is available")
@@ -76,15 +79,17 @@
         cmd = ["sshfs"]
         if self.port:
             cmd += ["-p", str(self.port)]
         for opt in self.sshfs_opts:
             cmd += ["-o", opt]
         cmd += [f"{self._build_connect_string()}:/", mount_point]
         try:
-            util.exec_subprocess(cmd, method="check_call", stdout=subprocess.DEVNULL)
+            util.exec_subprocess(
+                cmd, method="check_call", stdout=subprocess.DEVNULL
+            )
         except FileNotFoundError as e:
             logging.debug("  -> got exception: %s", e)
             if self.source:
                 # we need that for the locks
                 logging.info(
                     "  The sshfs command is not available but it is "
                     "mandatory for sourcing from SSH."
@@ -102,15 +107,17 @@
         if self.sshfs:
             for d in dirs:
                 if not os.path.isdir(self._path_to_sshfs(d)):
                     logging.info("Creating directory: %s", d)
                     try:
                         os.makedirs(self._path_to_sshfs(d))
                     except OSError as e:
-                        logging.error("Error creating new location %s: %s", d, e)
+                        logging.error(
+                            "Error creating new location %s: %s", d, e
+                        )
                         raise util.AbortError()
         else:
             cmd = ["mkdir", "-p"] + dirs
             self._exec_command(cmd)
 
     def _collapse_commands(self, commands, abort_on_failure=True):
         """Concatenates all given commands, ';' is inserted as separator."""
```

### Comparing `btrfs-backup-ng-0.5.8/src/btrfs_backup_ng/util.py` & `btrfs-backup-ng-0.5.9/src/btrfs_backup_ng/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -121,22 +121,24 @@
     best_match = ""
     best_match_fs_type = ""
     logging.debug("  Reading mounts file: %s", MOUNTS_FILE)
     for line in open(MOUNTS_FILE, encoding="utf-8"):
         try:
             mount_point, fs_type = line.split(" ")[1:3]
         except ValueError as e:
-            logging.debug("  Couldn't split line, skipping: %s\nCaught: %s", line, e)
+            logging.debug(
+                "  Couldn't split line, skipping: %s\nCaught: %s", line, e
+            )
             continue
         mount_point_prefix = mount_point
         if not mount_point_prefix.endswith(os.sep):
             mount_point_prefix += os.sep
-        if (path == mount_point or path.startswith(mount_point_prefix)) and len(
-            mount_point
-        ) > len(best_match):
+        if (
+            path == mount_point or path.startswith(mount_point_prefix)
+        ) and len(mount_point) > len(best_match):
             best_match = mount_point
             best_match_fs_type = fs_type
             logging.debug(
                 "  New best_match with filesystem type %s: %s",
                 best_match_fs_type,
                 best_match,
             )
@@ -218,15 +220,17 @@
                 try:
                     with open(arg_string[1:], encoding="utf-8") as args_file:
                         for arg_line in args_file.read().splitlines():
                             for arg in self.convert_arg_line_to_args(arg_line):
                                 # make nested includes relative to their parent
                                 if (
                                     self.fromfile_prefix_chars is not None
-                                    and arg.startswith(self.fromfile_prefix_chars)
+                                    and arg.startswith(
+                                        self.fromfile_prefix_chars
+                                    )
                                 ):
                                     dir_name = os.path.dirname(arg_string[1:])
                                     path = os.path.join(dir_name, arg[1:])
                                     # eliminate ../foo/../foo constructs
                                     path = os.path.normpath(path)
                                     arg = arg[0] + path
                                 arg_strings.append(arg)
@@ -260,9 +264,11 @@
         if text.startswith("N|"):
             _lines = text[2:].splitlines()
         else:
             _lines = [text]
         lines = []
         for line in _lines:
             # this is the RawTextHelpFormatter._split_lines
-            lines.extend(argparse.HelpFormatter._split_lines(self, line, width))
+            lines.extend(
+                argparse.HelpFormatter._split_lines(self, line, width)
+            )
         return lines
```

### Comparing `btrfs-backup-ng-0.5.8/src/btrfs_backup_ng.egg-info/PKG-INFO` & `btrfs-backup-ng-0.5.9/src/btrfs_backup_ng.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: btrfs-backup-ng
-Version: 0.5.8
+Version: 0.5.9
 Summary: Intelligent, feature-rich backups for btrfs
 Author-email: Michael Berry <trismegustis@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/berrym/btrfs-backup-ng
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
@@ -40,15 +40,15 @@
 written by Chris Lawrence. Since then, most of the code has been
 refactored and many new features were added before this repository has
 been transferred to Robert Schindler. Many thanks to Chris for his work. The old code
 base has been tagged with `legacy`. If, for any reason, you want to
 continue using it and miss the new features, you can check that out.
 
 Latest release  
-v0.5.8
+v0.5.9
 
 Downloads  
 <http://pypi.python.org/pypi/btrfs_backup_ng>
 
 Source  
 <https://github.com/berrym/btrfs-backup-ng>
 
@@ -122,15 +122,15 @@
 Note: This package now uses a pyproject.toml based build as outlined in
 PEP 517 and PEP 621.
 
 Clone this git repository
 
     $ git clone https://github.com/berrym/btrfs-backup-ng.git
     $ cd btrfs-backup-ng
-    $ git checkout tags/v0.5.8  # optionally checkout a specific version
+    $ git checkout tags/v0.5.9  # optionally checkout a specific version
     $ python3 -m venv /path/to/btrfs-backup-ng/venv # optionally use venv
     $ sh /path/to/btrfs-backup-ng/venv/bin/activate # using venv
     $ python3 -m build
     # using venv
     $ python3 -m pip install .
     # or 
     $ sudo python3 -m pip install .
```

### Comparing `btrfs-backup-ng-0.5.8/src/btrfs_backup_ng.egg-info/SOURCES.txt` & `btrfs-backup-ng-0.5.9/src/btrfs_backup_ng.egg-info/SOURCES.txt`

 * *Files identical despite different names*

