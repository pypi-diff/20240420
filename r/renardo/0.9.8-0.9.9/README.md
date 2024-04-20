# Comparing `tmp/renardo-0.9.8.tar.gz` & `tmp/renardo-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "renardo-0.9.8.tar", last modified: Tue Feb 13 02:10:58 2024, max compression
+gzip compressed data, was "renardo-0.9.9.tar", last modified: Sat Apr 20 17:39:02 2024, max compression
```

## Comparing `renardo-0.9.8.tar` & `renardo-0.9.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 02:10:58.741278 renardo-0.9.8/
--rw-r--r--   0 runner    (1001) docker     (127)    12726 2024-02-13 02:10:58.741278 renardo-0.9.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12308 2024-02-13 02:10:44.000000 renardo-0.9.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 02:10:58.741278 renardo-0.9.8/renardo/
--rw-r--r--   0 runner    (1001) docker     (127)     3462 2024-02-13 02:10:44.000000 renardo-0.9.8/renardo/PulsarInstance.py
--rw-r--r--   0 runner    (1001) docker     (127)     3795 2024-02-13 02:10:44.000000 renardo-0.9.8/renardo/RenardoApp.py
--rw-r--r--   0 runner    (1001) docker     (127)     8002 2024-02-13 02:10:44.000000 renardo-0.9.8/renardo/RenardoTUI.py
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-02-13 02:10:44.000000 renardo-0.9.8/renardo/RenardoTUI.tcss
--rw-r--r--   0 runner    (1001) docker     (127)     5547 2024-02-13 02:10:44.000000 renardo-0.9.8/renardo/SCFilesHandling.py
--rw-r--r--   0 runner    (1001) docker     (127)     3251 2024-02-13 02:10:44.000000 renardo-0.9.8/renardo/SuperColliderInstance.py
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-02-13 02:10:44.000000 renardo-0.9.8/renardo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-02-13 02:10:44.000000 renardo-0.9.8/renardo/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 02:10:58.741278 renardo-0.9.8/renardo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12726 2024-02-13 02:10:58.000000 renardo-0.9.8/renardo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-02-13 02:10:58.000000 renardo-0.9.8/renardo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-13 02:10:58.000000 renardo-0.9.8/renardo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-02-13 02:10:58.000000 renardo-0.9.8/renardo.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-02-13 02:10:58.000000 renardo-0.9.8/renardo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-02-13 02:10:58.000000 renardo-0.9.8/renardo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-13 02:10:58.741278 renardo-0.9.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      944 2024-02-13 02:10:44.000000 renardo-0.9.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:39:02.231076 renardo-0.9.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    12726 2024-04-20 17:39:02.231076 renardo-0.9.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12308 2024-04-20 17:38:57.000000 renardo-0.9.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:39:02.231076 renardo-0.9.9/renardo/
+-rw-r--r--   0 runner    (1001) docker     (127)     3462 2024-04-20 17:38:57.000000 renardo-0.9.9/renardo/PulsarInstance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3795 2024-04-20 17:38:57.000000 renardo-0.9.9/renardo/RenardoApp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6934 2024-04-20 17:38:57.000000 renardo-0.9.9/renardo/RenardoTUI.py
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-20 17:38:57.000000 renardo-0.9.9/renardo/RenardoTUI.tcss
+-rw-r--r--   0 runner    (1001) docker     (127)     5547 2024-04-20 17:38:57.000000 renardo-0.9.9/renardo/SCFilesHandling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3251 2024-04-20 17:38:57.000000 renardo-0.9.9/renardo/SuperColliderInstance.py
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-20 17:38:57.000000 renardo-0.9.9/renardo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-20 17:38:57.000000 renardo-0.9.9/renardo/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:39:02.231076 renardo-0.9.9/renardo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12726 2024-04-20 17:39:02.000000 renardo-0.9.9/renardo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-20 17:39:02.000000 renardo-0.9.9/renardo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 17:39:02.000000 renardo-0.9.9/renardo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-20 17:39:02.000000 renardo-0.9.9/renardo.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-20 17:39:02.000000 renardo-0.9.9/renardo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-20 17:39:02.000000 renardo-0.9.9/renardo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 17:39:02.231076 renardo-0.9.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-04-20 17:38:57.000000 renardo-0.9.9/setup.py
```

### Comparing `renardo-0.9.8/PKG-INFO` & `renardo-0.9.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: renardo
-Version: 0.9.8
+Version: 0.9.9
 Summary: Launcher/config editor for Renardo livecoding environment
 Home-page: http://renardo.org/
 Author: Elie Gavoty
 Author-email: eliegavoty@free.fr
 License: cc-by-sa-4.0
 Description-Content-Type: text/markdown
-Requires-Dist: renardo-lib==0.9.8
-Requires-Dist: FoxDotEditor==0.9.8
+Requires-Dist: renardo-lib==0.9.9
+Requires-Dist: FoxDotEditor==0.9.9
 Requires-Dist: renardo_gatherer==0.1.3
 Requires-Dist: psutil
 Requires-Dist: textual
 
 Renardo v0.9 - FoxDot fork
 ===========================
```

### Comparing `renardo-0.9.8/README.md` & `renardo-0.9.9/README.md`

 * *Files identical despite different names*

### Comparing `renardo-0.9.8/renardo/PulsarInstance.py` & `renardo-0.9.9/renardo/PulsarInstance.py`

 * *Files identical despite different names*

### Comparing `renardo-0.9.8/renardo/RenardoApp.py` & `renardo-0.9.9/renardo/RenardoApp.py`

 * *Files identical despite different names*

### Comparing `renardo-0.9.8/renardo/RenardoTUI.py` & `renardo-0.9.9/renardo/RenardoTUI.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,101 +1,89 @@
-from textual.css.query import NoMatches
-
-from .SCFilesHandling import is_renardo_scfiles_installed, write_sc_renardo_files_in_user_config
-from textual import work
 from textual.app import App, ComposeResult
 from textual.reactive import reactive
-from textual.containers import Horizontal, Vertical
+from textual.binding import Binding
+from textual.css.query import NoMatches
+from renardo.SCFilesHandling import is_renardo_scfiles_installed, write_sc_renardo_files_in_user_config
+from renardo.widgets.Widgets import LeftPane
+from textual import work
 
+from textual.containers import Horizontal, Vertical
 from textual.widgets import (
     Header,
-    Label,
+    Footer,
     Button,
+    Label,
     TabbedContent,
     TabPane,
     Log,
-    Static,
-    ContentSwitcher,
+    RadioButton,
+    RadioSet,
+    TextArea,
+    MarkdownViewer
 )
 
-class StartRenardoBlock(Static):
-    def compose(self) -> ComposeResult:
-        #yield Label("Default samples pack downloaded and Renardo SuperCollider files installed")
-        yield Button("Start SuperCollider Backend", id="start-sc-btn")
-        yield Button("Start renardo Pulsar", id="start-pulsar-btn", disabled=True)
-        yield Button("Start renardo FoxDot editor", id="start-renardo-foxdot-editor-btn", disabled=True)
-        #yield Button("Start renardo pipe mode", id="start-renardo-pipe-btn", disabled=True)
-
-class SCNotReadyBlock(Static):
-    def compose(self) -> ComposeResult:
-        yield Label("SuperCollider seems not ready. Please install it in default location (see doc)")
-
-class DownloadRenardoSamplesBlock(Static):
-    def compose(self) -> ComposeResult:
-        yield Label("Default samples pack needs to be downloaded")
-        yield Button("Download renardo default samples pack", id="dl-renardo-samples-btn")
-
-class InitRenardoSCFilesBlock(Static):
-    def compose(self) -> ComposeResult:
-        yield Label("Renardo SuperCollider files need to be installed")
-        yield Button("Create renardo SC Class files and startup code", id="init-renardo-scfiles-btn")
-
-class LeftPane(ContentSwitcher):
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-
-    def compose(self) -> ComposeResult:
-        yield StartRenardoBlock(id="start-renardo")
-        yield SCNotReadyBlock(id="sc-not-ready")
-        yield InitRenardoSCFilesBlock(id="init-renardo-scfiles")
-        yield DownloadRenardoSamplesBlock(id="dl-renardo-samples")
-
 class RenardoTUI(App[None]):
     CSS_PATH = "RenardoTUI.tcss"
     left_pane_mode = reactive("start-renardo")
-    #BINDINGS = [
-    #    ("d", "toggle_dark", "Toggle dark mode"),
-    #    ("a", "add_stopwatch", "Add"),
-    #    ("r", "remove_stopwatch", "Remove"),
-    #]
+
+    BINDINGS = [
+        Binding("ctrl+q", "quit", "Quit", show=True, priority=True),
+    ]
+
     def __init__(self, renardo_app, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.renardo_app = renardo_app
         self.left_pane_mode = self.calculate_left_pane_mode()
 
     def calculate_left_pane_mode(self):
         if not self.renardo_app.sc_instance.supercollider_ready:
             return "sc-not-ready"
         if not is_renardo_scfiles_installed():
             return "init-renardo-scfiles"
         if not self.renardo_app.spack_manager.is_default_spack_initialized():
             return "dl-renardo-samples"
         return "start-renardo"
 
+    def watch_left_pane_mode(self): # This is a special method from textual that is not easy to move from the app
+        """watch function textual reactive param"""
+        try:
+            self.query_one(LeftPane).current = self.left_pane_mode
+        except NoMatches:
+            pass
+
     def compose(self) -> ComposeResult:
         yield Header()
-        with TabbedContent(initial="start-tab"):
-            with TabPane("Start", id="start-tab"):
+        with TabbedContent():
+            with TabPane("Welcome", id="welcome-tab"):
+                yield Label("Welcome to renardo terminal user interface (TUI) !!")
+                yield Label("Here you can configure (WIP), learn (WIP) renardo and start it's different modules")
+            with TabPane("Autostart", id="start-tab"):
                 with Horizontal():
                     with Vertical():
                         yield LeftPane(initial=self.calculate_left_pane_mode())
-                        yield Button("Quit", id="quit-btn")
                     with Vertical():
                         yield Log(id="log-output")
-            # with TabPane("Config", id="config-tab"):
-            #     with RadioSet():
-            #         yield Label("Boot SuperCollider audio backend at startup ?")
-            #         yield RadioButton("Yes (Still buggy but doesn't hurt to try)")
-            #         yield RadioButton("No (You should manually open SuperCollider and execute Renardo.start)", value=True)
-            #with TabPane("SuperCollider Boot", id="sc-boot"):
-            #    with Horizontal():
-            #        with Vertical():
-            #            yield Button("Start SC instance", id="start-sc-btn")
-            #        with Vertical():
-            #            yield Log(id="sc-log-output")
+#             with TabPane("Documentation", id="doc-tab"):
+#                 EXAMPLE_MARKDOWN = """\
+# # Markdown Viewer
+
+# This is an example of Textual's `MarkdownViewer` widget.
+
+# ## Features
+
+# Markdown syntax and extensions are supported.
+
+# - Typography *emphasis*, **strong**, `inline code` etc.
+# - Headers
+# - Lists (bullet and ordered)
+# - Syntax highlighted code blocks
+# - Tables!
+#                 """
+#                 yield MarkdownViewer(EXAMPLE_MARKDOWN)
+        yield Footer()
 
     @work(exclusive=True, thread=True)
     def dl_samples_background(self) -> None:
         log_output_widget = self.query_one("#log-output", Log)
         self.renardo_app.spack_manager.set_logger(log_output_widget)
         self.renardo_app.spack_manager.init_default_spack()
         self.left_pane_mode = self.calculate_left_pane_mode()
@@ -121,47 +109,40 @@
                 self.query_one("#start-pulsar-btn", Button).disabled = False
             else:
                 self.query_one("#start-pulsar-btn", Button).label = "Pulsar not ready"
 
             while True:
                 self.query_one("#log-output", Log).write_line(self.renardo_app.sc_instance.read_stdout_line())
         else:
-            self.query_one("#log-output", Log).write_line("Already started")
+            self.query_one("#log-output", Log).write_line("SuperCollider backend already started (sclang backend externally managed)\nIf you want to handle the backend manually you should ensure... \n...you executed Renardo.start; correctly in SuperCollider IDE")
+            self.query_one("#start-renardo-foxdot-editor-btn", Button).disabled = False
+            if self.renardo_app.pulsar_instance.pulsar_ready:
+                self.query_one("#start-pulsar-btn", Button).disabled = False
 
     @work(exclusive=True, thread=True)
     def start_pulsar_background(self) -> None:
         self.query_one("#log-output", Log).write_line("Launching Renardo SC module with SCLang...")
         self.renardo_app.pulsar_instance.start_pulsar_subprocess()
         while True:
             self.query_one("#log-output", Log).write_line(self.renardo_app.pulsar_instance.read_stdout_line())
 
     @work(exclusive=True, thread=True)
     def start_foxdoteditor_background(self) -> None:
         from renardo_lib import FoxDotCode
         # Open the GUI
         from FoxDotEditor.Editor import workspace
         FoxDot = workspace(FoxDotCode).run()
-        self.exit(0) # Exit renardo when editor is closed because there is a bug when relaunching editor
-
-    def watch_left_pane_mode(self):
-        """watch function textual reactive param"""
-        try:
-            self.query_one(LeftPane).current = self.left_pane_mode
-        except NoMatches:
-            pass
+        self.app.exit(0) # Exit renardo when editor is closed because there is a bug when relaunching editor
 
     # def on_radio_set_changed(self, event: RadioSet.Changed) -> None:
     #     self.renardo_app.args.boot = True if event.radio_set.pressed_index == 1 else False
 
     def on_button_pressed(self, event: Button.Pressed) -> None:
         """Event handler called when a button is pressed."""
         button_id = event.button.id
-        if button_id == "quit-btn":
-            #self.renardo_app.sc_instance.sclang_process.kill()
-            self.exit()
         if button_id == "dl-renardo-samples-btn":
             self.dl_samples_background()
         if button_id == "init-renardo-scfiles-btn":
             self.init_scfile_background()
         #if button_id == "start-renardo-pipe-btn":
         #    self.renardo_app.args.pipe = True
         #    self.exit()
@@ -171,7 +152,11 @@
             self.start_sc_background()
         if button_id == "start-renardo-foxdot-editor-btn":
             self.start_foxdoteditor_background()
 
     def on_mount(self) -> None:
         self.title = "Renardo"
         #self.query_one(RadioSet).focus()
+
+    def quit(self):
+        # self.renardo_app.sc_instance.sclang_process.kill()
+        self.exit()
```

### Comparing `renardo-0.9.8/renardo/SCFilesHandling.py` & `renardo-0.9.9/renardo/SCFilesHandling.py`

 * *Files identical despite different names*

### Comparing `renardo-0.9.8/renardo/SuperColliderInstance.py` & `renardo-0.9.9/renardo/SuperColliderInstance.py`

 * *Files identical despite different names*

### Comparing `renardo-0.9.8/renardo.egg-info/PKG-INFO` & `renardo-0.9.9/renardo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: renardo
-Version: 0.9.8
+Version: 0.9.9
 Summary: Launcher/config editor for Renardo livecoding environment
 Home-page: http://renardo.org/
 Author: Elie Gavoty
 Author-email: eliegavoty@free.fr
 License: cc-by-sa-4.0
 Description-Content-Type: text/markdown
-Requires-Dist: renardo-lib==0.9.8
-Requires-Dist: FoxDotEditor==0.9.8
+Requires-Dist: renardo-lib==0.9.9
+Requires-Dist: FoxDotEditor==0.9.9
 Requires-Dist: renardo_gatherer==0.1.3
 Requires-Dist: psutil
 Requires-Dist: textual
 
 Renardo v0.9 - FoxDot fork
 ===========================
```

### Comparing `renardo-0.9.8/setup.py` & `renardo-0.9.9/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -3,31 +3,31 @@
 from setuptools import setup
 
 with open("README.md", "r") as f:
     long_description=f.read()
 
 setup(
     name='renardo',
-    version="0.9.8",
+    version="0.9.9",
     description='Launcher/config editor for Renardo livecoding environment',
     author='Elie Gavoty',
     author_email='eliegavoty@free.fr',
     license='cc-by-sa-4.0',
     url='http://renardo.org/',
     packages=[
         'renardo',
     ],
     long_description=long_description,
     long_description_content_type="text/markdown",
     # entry_points={'gui_scripts' : ['FoxDotEditor = FoxDotEditor.__init__:main']},
     # data_files=[('', 'LICENSE')],
     package_data = {'renardo': ['RenardoTUI.tcss'],},
     install_requires=[
-        'renardo-lib==0.9.8',
-        'FoxDotEditor==0.9.8',
+        'renardo-lib==0.9.9',
+        'FoxDotEditor==0.9.9',
         'renardo_gatherer==0.1.3',
         'psutil',
         'textual',
     ],
     entry_points={
         'console_scripts': [
             'renardo = renardo:entrypoint',
```

