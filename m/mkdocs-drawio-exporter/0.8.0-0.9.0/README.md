# Comparing `tmp/mkdocs-drawio-exporter-0.8.0.tar.gz` & `tmp/mkdocs_drawio_exporter-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs-drawio-exporter-0.8.0.tar", last modified: Sun May  9 10:25:21 2021, max compression
+gzip compressed data, was "mkdocs_drawio_exporter-0.9.0.tar", max compression
```

## Comparing `mkdocs-drawio-exporter-0.8.0.tar` & `mkdocs_drawio_exporter-0.9.0.tar`

### file list

```diff
@@ -1,16 +1,9 @@
-drwxr-xr-x   0 lukecarrier   (501) staff       (20)        0 2021-05-09 10:25:21.100883 mkdocs-drawio-exporter-0.8.0/
--rw-r--r--   0 lukecarrier   (501) staff       (20)     6650 2021-05-09 10:25:21.100441 mkdocs-drawio-exporter-0.8.0/PKG-INFO
--rw-r--r--   0 lukecarrier   (501) staff       (20)     4901 2021-05-09 10:06:44.000000 mkdocs-drawio-exporter-0.8.0/README.md
-drwxr-xr-x   0 lukecarrier   (501) staff       (20)        0 2021-05-09 10:25:21.098956 mkdocs-drawio-exporter-0.8.0/mkdocs_drawio_exporter.egg-info/
--rw-r--r--   0 lukecarrier   (501) staff       (20)     6650 2021-05-09 10:25:21.000000 mkdocs-drawio-exporter-0.8.0/mkdocs_drawio_exporter.egg-info/PKG-INFO
--rw-r--r--   0 lukecarrier   (501) staff       (20)      393 2021-05-09 10:25:21.000000 mkdocs-drawio-exporter-0.8.0/mkdocs_drawio_exporter.egg-info/SOURCES.txt
--rw-r--r--   0 lukecarrier   (501) staff       (20)        1 2021-05-09 10:25:21.000000 mkdocs-drawio-exporter-0.8.0/mkdocs_drawio_exporter.egg-info/dependency_links.txt
--rw-r--r--   0 lukecarrier   (501) staff       (20)       78 2021-05-09 10:25:21.000000 mkdocs-drawio-exporter-0.8.0/mkdocs_drawio_exporter.egg-info/entry_points.txt
--rw-r--r--   0 lukecarrier   (501) staff       (20)        7 2021-05-09 10:25:21.000000 mkdocs-drawio-exporter-0.8.0/mkdocs_drawio_exporter.egg-info/requires.txt
--rw-r--r--   0 lukecarrier   (501) staff       (20)       21 2021-05-09 10:25:21.000000 mkdocs-drawio-exporter-0.8.0/mkdocs_drawio_exporter.egg-info/top_level.txt
-drwxr-xr-x   0 lukecarrier   (501) staff       (20)        0 2021-05-09 10:25:21.099956 mkdocs-drawio-exporter-0.8.0/mkdocsdrawioexporter/
--rw-r--r--   0 lukecarrier   (501) staff       (20)       86 2021-05-02 10:25:00.000000 mkdocs-drawio-exporter-0.8.0/mkdocsdrawioexporter/__init__.py
--rw-r--r--   0 lukecarrier   (501) staff       (20)    11679 2021-05-09 10:03:50.000000 mkdocs-drawio-exporter-0.8.0/mkdocsdrawioexporter/exporter.py
--rw-r--r--   0 lukecarrier   (501) staff       (20)     3693 2021-05-09 10:03:50.000000 mkdocs-drawio-exporter-0.8.0/mkdocsdrawioexporter/plugin.py
--rw-r--r--   0 lukecarrier   (501) staff       (20)       38 2021-05-09 10:25:21.101034 mkdocs-drawio-exporter-0.8.0/setup.cfg
--rw-r--r--   0 lukecarrier   (501) staff       (20)      805 2021-05-09 10:21:19.000000 mkdocs-drawio-exporter-0.8.0/setup.py
+-rw-r--r--   0        0        0     1088 2022-05-28 16:23:43.820835 mkdocs_drawio_exporter-0.9.0/LICENSE.md
+-rw-r--r--   0        0        0     5162 2024-04-20 13:34:58.570127 mkdocs_drawio_exporter-0.9.0/README.md
+-rw-r--r--   0        0        0       86 2024-04-03 12:37:18.104252 mkdocs_drawio_exporter-0.9.0/mkdocs_drawio_exporter/__init__.py
+-rw-r--r--   0        0        0    13942 2024-04-20 13:34:58.570948 mkdocs_drawio_exporter-0.9.0/mkdocs_drawio_exporter/exporter.py
+-rw-r--r--   0        0        0     3422 2024-04-20 13:16:29.256842 mkdocs_drawio_exporter-0.9.0/mkdocs_drawio_exporter/plugin.py
+-rw-r--r--   0        0        0       36 2024-04-03 12:37:18.105168 mkdocs_drawio_exporter-0.9.0/mkdocs_drawio_exporter/tests/__init__.py
+-rw-r--r--   0        0        0    12808 2024-04-20 13:16:29.257645 mkdocs_drawio_exporter-0.9.0/mkdocs_drawio_exporter/tests/exporter.py
+-rw-r--r--   0        0        0     1916 2024-04-20 13:34:58.571241 mkdocs_drawio_exporter-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     6924 1970-01-01 00:00:00.000000 mkdocs_drawio_exporter-0.9.0/PKG-INFO
```

### Comparing `mkdocs-drawio-exporter-0.8.0/README.md` & `mkdocs_drawio_exporter-0.9.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 For the default configuration, just add the plugin to the `plugins` key:
 
 ```yaml
 plugins:
     - drawio-exporter
 ```
 
-You can override the default configuration:
+You can override the default configuration; values shown are defaults:
 
 ```yaml
 plugins:
     - drawio-exporter:
         # Diagrams are cached to speed up site generation. The default path is
         # drawio-exporter, relative to the documentation directory.
         cache_dir: 'drawio-exporter'
@@ -40,22 +40,26 @@
         #   * drawio on Linux
         #   * draw.io on macOS
         #   * or draw.io.exe on Windows
         # We'll look for it on your system's PATH, then default installation
         # paths. If we can't find it we'll warn you.
         drawio_executable: null
         # Additional Draw.io CLI args
+        #   * --embed-svg-images will embed external images in SVGS, if format is "svg".
         drawio_args: []
         # Output format (see draw.io --help | grep format)
         format: svg
         # Embed format
         #   * The default is to embed via the <img> tag, only rewriting the
         #     value of the src attribute.
         #   * Consider <object type="image/svg+xml" data="{img_src}"></object>
         #     to enable interactive elements (like hyperlinks) in SVGs.
+        #   * Consider {content} to inline SVGs into documents directly, useful
+        #     for styling with CSS, preserving interactivity, and improving
+        #     search by indexing diagram text.
         embed_format: '{img_open}{img_src}{img_close}'
         # Glob pattern for matching source files
         sources: '*.drawio'
 ```
 
 ## Usage
 
@@ -69,14 +73,18 @@
 
 ```markdown
 ![Page 1](my-diagram.drawio#0)
 ```
 
 The plugin will export the diagram to the `format` specified in your configuration and will rewrite the `<img>` tag in the generated page to match. To speed up your documentation rebuilds, the generated output will be placed into `cache_dir` and then copied to the desired destination. The cached images will only be updated if the source diagram's modification date is newer than the cached export. Thus, bear in mind caching works per file - with large multi-page documents a change to one page will rebuild all pages, which will be slower than separate files per page.
 
+### GitHub Actions
+
+See [this guide](./docs/github-actions.md).
+
 ### Headless usage
 
 In addition to the above, if you're running in a headless environment (e.g. in integration, or inside a Docker container), you may need to ensure a display server is running and that the necessary dependencies are installed.
 
 On Debian and Ubuntu, the following should install the dependencies:
 
 ```console
@@ -107,67 +115,59 @@
 ```
 
 ## Hacking
 
 To get completion working in your editor, set up a virtual environment in the root of this repository and install MkDocs:
 
 ```
-$ pip3 install --user --upgrade setuptools twine wheel
-$ python3 -m venv venv
-$ . venv/bin/activate
-$ pip install -r requirements.txt
+$ pip3 install --user --upgrade wheel
+$ pipx install twine
+$ poetry install
 ```
 
 To install the plugin onto a local MkDocs site in editable form:
 
 ```
-$ pip install --editable /path/to/mkdocs-drawio-exporter
+$ poetry add --editable /path/to/mkdocs-drawio-exporter
 ```
 
-Note that you'll need to repeat this step if you make any changes to the `entry_points` listed in `setup.py`.
+Note that you'll need to repeat this step if you make any changes to the `[tool.poetry.plugins.*]` sections listed in `pyproject.toml`.
 
-Run the tests with the Python `unittest` module:
+Run the tests with the `test` script:
 
 ```
-$ python -m unittest mkdocsdrawioexporter.tests
+$ poetry run test
 ```
 
 ## Upgrading dependencies
 
-To upgrade the dependencies, install `pip-upgrader`:
+To upgrade the dependencies, first make any necessary changes to the constraints expressed in the `[tool.poetry.dependencies]` section of `pyproject.toml`, then have Poetry update them:
 
-```console
-. venv/bin/activate
-pip install -r requirements.dev.txt
 ```
-
-Then proceed to update the dependencies:
-
-```console
-pip-upgrade requirements.dev.txt
+$ poetry update
 ```
 
 ## Releasing
 
 Build the distributable package:
 
 ```
-$ python3 setup.py sdist bdist_wheel
+$ poetry build
 ```
 
 Push it to the PyPI test instance:
 
 ```
-$ python3 -m twine upload --repository-url https://test.pypi.org/legacy/ dist/*
+$ twine upload --repository-url https://test.pypi.org/legacy/ dist/*
 ```
 
 Test it inside a virtual environment:
 
 ```
 $ pip install --index-url https://test.pypi.org/simple/ --no-deps mkdocs-drawio-exporter
 ```
 
 Let's go live:
 
 ```
-$ python3 -m twine upload dist/*
+$ twine upload dist/*
 ```
```

### Comparing `mkdocs-drawio-exporter-0.8.0/mkdocsdrawioexporter/exporter.py` & `mkdocs_drawio_exporter-0.9.0/mkdocs_drawio_exporter/exporter.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,36 @@
 import fnmatch
 import hashlib
 import os.path
 import re
 import shutil
 import subprocess
 import sys
+from typing import TypedDict
+import urllib.parse
 
 
-IMAGE_RE = re.compile('(<img[^>]+src=")([^">]+)("\s*\/?>)')
+IMAGE_RE = re.compile('(<img[^>]+src=")([^">]+)("\\s*\\/?>)')
+
+
+class Configuration(TypedDict):
+    """Draw.io Exporter MkDocs plugin configuration.
+
+    Contains the resolved configuration values, including defaults and any
+    computed values (such as paths to binaries).
+
+    Seems ugly to shadow BasePlugin.config_scheme, but improves type hints and
+    allows us to more easily pass configuration around."""
+
+    cache_dir: str
+    drawio_executable: str
+    drawio_args: list[str]
+    format: str
+    embed_format: str
+    sources: str
 
 
 class ConfigurationError(Exception):
     """Configuration exception.
 
     Used to signal that MkDocs should exit, as the plugin configuration is
     invalid and we'll be unable to export diagrams.
@@ -41,16 +60,15 @@
         """
         self.key = key
         self.value = value
         self.message = message
         Exception.__init__(self, self.message)
 
     def __str__(self):
-        return 'drawio-exporter: value "{}" for key "{}" is invalid: {}'.format(
-                self.value, self.key, self.message)
+        return f'drawio-exporter: value "{self.value}" for key "{self.key}" is invalid: {self.message}'
 
     def drawio_executable(value, message):
         """Raise an error for a misconfigured Draw.io path.
 
         :param str value: Configured Draw.io executable path.
         :param str message: Explanatory message describing the problem.
         """
@@ -98,22 +116,26 @@
 
     def __hash__(self):
         return hash((
             'source_rel', self.source_rel,
             'page_index', self.page_index,
         ))
 
+    def __repr__(self):
+        return f"Source({self.source_embed}, {self.page_index}, {self.source_rel})"
+
     def resolve_rel_path(self, page_dest_path):
         """Resolve the path of the source, relative to the documentation directory.
 
         :param str page_dest_path: The destination path of the parent page.
         """
+        unescaped_source_embed = urllib.parse.unquote(self.source_embed)
         self.source_rel = os.path.normpath(os.path.join(
                 os.path.dirname(page_dest_path),
-                self.source_embed))
+                unescaped_source_embed))
 
 
 class DrawIoExporter:
     """Draw.io Exporter.
 
     The logic for the export process lives here. The bindings to the MkDocs
     plugin events is kept separate to ease testing.
@@ -121,20 +143,28 @@
 
     log = None
     """Log.
 
     :type: logging.Logger
     """
 
-    def __init__(self, log):
+    docs_dir = None
+    """Draw.io docs_dir.
+
+    :type str:
+    """
+
+    def __init__(self, log, docs_dir):
         """Initialise.
 
         :param logging.Logger log: Where to log.
+        :param str docs_dir: MkDocs docs_dir.
         """
         self.log = log
+        self.docs_dir = docs_dir
 
     DRAWIO_EXECUTABLE_NAMES = ['drawio', 'draw.io']
     """Draw.io executable names."""
 
     def drawio_executable_paths(self, platform):
         """Get the Draw.io executable paths for the platform.
 
@@ -155,27 +185,27 @@
             return ['/opt/draw.io/drawio']
         elif platform == 'win32':
             program_files = [os.environ['ProgramFiles']]
             if 'ProgramFiles(x86)' in os.environ:
                 program_files.append(os.environ['ProgramFiles(x86)'])
             return [os.path.join(dir, 'draw.io', 'draw.io.exe') for dir in program_files]
         else:
-            self.log.warn('Draw.io executable paths not known for platform "{}"'.format(platform))
+            self.log.warning(f'Draw.io executable paths not known for platform "{platform}"')
 
-    def prepare_cache_dir(self, cache_dir, docs_dir):
+    def prepare_cache_dir(self, cache_dir):
         """Ensure the cache path is set, absolute and exists.
 
         :param str cache_dir: Configured cache directory.
         :param str docs_dir: Docs directory, in which to base relative cache directories.
         :return str: Final cache directory.
         """
         if not cache_dir:
            cache_dir = 'drawio-exporter'
         if not os.path.isabs(cache_dir):
-            cache_dir = os.path.join(docs_dir, cache_dir)
+            cache_dir = os.path.join(self.docs_dir, cache_dir)
         return cache_dir
 
     def prepare_drawio_executable(self, executable, executable_names, platform_executable_paths):
         """Ensure the Draw.io executable path is configured, or guess it.
 
         :param str executable: Configured Draw.io executable.
         :param list(str) executable_names: Candidate executable names to seek on PATH.
@@ -187,31 +217,42 @@
                 raise ConfigurationError.drawio_executable(
                         executable, "executable didn't exist")
             return executable
 
         for name in executable_names:
             executable = shutil.which(name)
             if executable:
-                self.log.debug('Found Draw.io executable "{}" at "{}"'.format(name, executable))
+                self.log.debug(f'Found Draw.io executable "{name}" at "{executable}"')
                 return executable
 
         candidates = platform_executable_paths
-        self.log.debug('Trying paths {} for platform "{}"'.format(candidates, sys.platform))
+        self.log.debug(f'Trying paths {candidates} for platform "{sys.platform}"')
         for candidate in candidates:
             if os.path.isfile(candidate):
-                self.log.debug('Found Draw.io executable for platform "{}" at "{}"'.format(
-                        sys.platform, candidate))
+                self.log.debug(f'Found Draw.io executable for platform "{sys.platform}" at "{candidate}"')
                 return candidate
 
         raise ConfigurationError.drawio_executable(
                 None, 'Unable to find Draw.io executable; ensure it\'s on PATH or set drawio_executable option')
 
-    def rewrite_image_embeds(self, output_content, sources, format, embed_format):
+    def validate_config(self, config: Configuration):
+        """Validate the configuration.
+
+        :param dict config: Configuration.
+        :return bool: True if configuration is valid.
+        """
+        if '{content}' in config['embed_format'] and config['format'] != 'svg':
+            raise ConfigurationError(
+                    'embed_format', config['embed_format'],
+                    'cannot inline content of non-SVG format')
+
+    def rewrite_image_embeds(self, page_dest_path, output_content, config: Configuration):
         """Rewrite image embeds.
 
+        :param str page_dest_path: Destination path.
         :param str output_content: Content to rewrite.
         :param str sources: Glob to match Draw.io diagram filenames.
         :param str format: Desired export format.
         :param str embed_format: Format string to rewrite <img> tags with.
         :return str: Rewritten content.
         """
         content_sources = []
@@ -219,21 +260,42 @@
         def replace(match):
             try:
                 filename, page_index = match.group(2).rsplit('#', 1)
             except ValueError:
                 filename = match.group(2)
                 page_index = 0
 
-            if fnmatch.fnmatch(filename, sources):
-                content_sources.append(Source(filename, page_index))
-                img_src = "{}-{}.{}".format(filename, page_index, format)
+            if fnmatch.fnmatch(filename, config["sources"]):
+                source = Source(filename, page_index)
+                source.resolve_rel_path(page_dest_path)
+                content_sources.append(source)
+                img_src = f"{filename}-{page_index}.{config["format"]}"
+
+                # Cache the file on-demand and read file content only if we
+                # need to inline the file's content.
+                content = None
+                if "{content}" in config["embed_format"]:
+                    img_path = self.make_cache_filename(
+                            source.source_rel, page_index, config['cache_dir'])
+
+                    abs_src_path = os.path.join(self.docs_dir, source.source_rel)
+                    _, exit_status = self.ensure_file_cached(
+                            abs_src_path, source.source_rel, source.page_index,
+                            config)
+
+                    if exit_status not in (None, 0):
+                        self.log.error(f'Export failed with exit status {exit_status}; skipping rewrite')
+                        return match.group(0)
+
+                    with open(img_path, "r") as f:
+                        content = f.read()
 
-                return embed_format.format(
+                return config["embed_format"].format(
                         img_open=match.group(1), img_close=match.group(3),
-                        img_src=img_src)
+                        img_src=img_src, content=content)
             else:
                 return match.group(0)
         output_content = IMAGE_RE.sub(replace, output_content)
 
         return (output_content, content_sources)
 
     def filter_cache_files(self, files, cache_dir):
@@ -241,83 +303,82 @@
 
         :param list(mkdocs.structure.File): Files to filter.
         :param str cache_dir: Cache directory.
         :return list(mkdocs.structure.File): Filtered files.
         """
         return [f for f in files if not f.abs_src_path.startswith(cache_dir)]
 
-    def ensure_file_cached(self, source, source_rel, page_index, drawio_executable, drawio_args, cache_dir, format):
+    def ensure_file_cached(self, source, source_rel, page_index, config: Configuration):
         """Ensure cached copy of output exists.
 
         :param str source: Source path, absolute.
         :param str source_rel: Source path, relative to docs directory.
         :param int page_index: Page index, numbered from zero.
         :param str drawio_executable: Path to the configured Draw.io executable.
         :param list(str) drawio_args: Additional arguments to append to the Draw.io export command.
         :param str cache_dir: Export cache directory.
         :param str format: Desired export format.
         :return tuple(str, int): Cached export filename.
         """
-        cache_filename = self.make_cache_filename(source_rel, page_index, cache_dir)
+        cache_filename = self.make_cache_filename(source_rel, page_index, config['cache_dir'])
         exit_status = None
 
         if self.use_cached_file(source, cache_filename):
-            self.log.debug('Source file appears unchanged; using cached copy from "{}"'.format(cache_filename))
+            self.log.debug(f'Source file appears unchanged; using cached copy from "{cache_filename}"')
         else:
-            if not drawio_executable:
-                self.log.warn('Skipping export of "{}" as Draw.io executable not available'.format(source))
+            if not config['drawio_executable']:
+                self.log.warning(f'Skipping export of "{source}" as Draw.io executable not available')
                 return (None, exit_status)
 
-            self.log.debug('Exporting "{}" to "{}"'.format(source, cache_filename))
+            self.log.debug(f'Exporting "{source}" to "{cache_filename}"')
             exit_status = self.export_file(
-                    source, page_index, cache_filename,
-                    drawio_executable, drawio_args, format)
+                    source, page_index, cache_filename, config)
 
         return (cache_filename, exit_status)
 
     def make_cache_filename(self, source, page_index, cache_dir):
         """Make the cached filename.
 
         :param str source: Source path, relative to the docs directory.
         :param int page_index: Page index, numbered from zero.
         :param str cache_dir: Export cache directory.
         :return str: Resulting filename.
         """
-        basename = '{}-{}'.format(
-                hashlib.sha1(source.encode('utf-8')).hexdigest(), page_index)
+        filename_hash = hashlib.sha1(source.encode('utf-8')).hexdigest()
+        basename = f'{filename_hash}-{page_index}'
         return os.path.join(cache_dir, basename)
 
     def use_cached_file(self, source, cache_filename):
         """Is the cached copy up to date?
 
         :param str source: Source path, relative to the docs directory.
         :param str cache_filename: Export cache filename.
         :return bool: True if cache is up to date, else False.
         """
         return os.path.exists(cache_filename) \
                 and os.path.getmtime(cache_filename) >= os.path.getmtime(source)
 
-    def export_file(self, source, page_index, dest, drawio_executable, drawio_args, format):
+    def export_file(self, source, page_index, dest, config: Configuration):
         """Export an individual file.
 
         :param str source: Source path, absolute.
         :param int page_index: Page index, numbered from zero.
         :param str dest: Destination path, within cache.
         :param str drawio_executable: Path to the configured Draw.io executable.
         :param list(str) drawio_args: Additional arguments to append to the Draw.io export command.
         :param str format: Desired export format.
         :return int: The Draw.io exit status.
         """
         cmd = [
-            drawio_executable,
+            config['drawio_executable'],
             '--export', source,
             '--page-index', str(page_index),
             '--output', dest,
-            '--format', format,
+            '--format', config['format'],
         ]
-        cmd += drawio_args
+        cmd += config['drawio_args']
 
         try:
-            self.log.debug('Using export command {}'.format(cmd))
+            self.log.debug(f'Using export command {cmd}')
             return subprocess.call(cmd)
         except:
             self.log.exception('Subprocess raised exception')
```

### Comparing `mkdocs-drawio-exporter-0.8.0/mkdocsdrawioexporter/plugin.py` & `mkdocs_drawio_exporter-0.9.0/mkdocs_drawio_exporter/plugin.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 import mkdocs
 from mkdocs.config import config_options
 import mkdocs.plugins
 from mkdocs.structure.files import Files
 from mkdocs.utils import copy_file
 
-from .exporter import ConfigurationError, DrawIoExporter, Source
+from .exporter import ConfigurationError, DrawIoExporter, Configuration
 
 
 log = mkdocs.plugins.log.getChild('drawio-exporter')
 
 
 class DrawIoExporterPlugin(mkdocs.plugins.BasePlugin):
     """Draw.io Exporter MkDocs plugin.
@@ -30,65 +30,61 @@
     )
 
     exporter = None
 
     sources = []
 
     def on_config(self, config):
-        self.exporter = DrawIoExporter(log)
+        self.exporter = DrawIoExporter(log, config['docs_dir'])
 
         self.config['cache_dir'] = self.exporter.prepare_cache_dir(
-                self.config['cache_dir'], config['docs_dir'])
+                self.config['cache_dir'])
         try:
             self.config['drawio_executable'] = self.exporter.prepare_drawio_executable(
                     self.config['drawio_executable'],
                     DrawIoExporter.DRAWIO_EXECUTABLE_NAMES,
                     self.exporter.drawio_executable_paths(sys.platform))
+            self.exporter.validate_config(self.config)
         except ConfigurationError as e:
             raise mkdocs.exceptions.ConfigurationError(str(e))
 
         os.makedirs(self.config['cache_dir'], exist_ok=True)
 
-        log.debug('Using Draw.io executable "{}", arguments {} and cache directory "{}"'.format(
-                self.config['drawio_executable'], self.config['drawio_args'],
-                self.config['cache_dir']))
+        log.debug(f'Using Draw.io executable "{self.config['drawio_executable']}", '
+                f'arguments {self.config['drawio_args']} and '
+                f'cache directory "{self.config['cache_dir']}"')
 
     def on_post_page(self, output_content, page, **kwargs):
         output_content, content_sources = self.exporter.rewrite_image_embeds(
-                output_content, self.config['sources'],
-                self.config['format'], self.config['embed_format'])
+                page.file.dest_path, output_content, self.config)
 
-        for source in content_sources:
-            source.resolve_rel_path(page.file.dest_path)
         self.sources += content_sources
 
         return output_content
 
     def on_files(self, files, config):
         keep = self.exporter.filter_cache_files(files, self.config['cache_dir'])
-        log.debug('{} files left after excluding cache'.format(len(keep)))
+        log.debug(f'{len(keep)} files left after excluding cache')
 
         return Files(keep)
 
     def on_post_build(self, config):
         sources = set(self.sources)
-        log.debug('Found {} unique sources in {} total embeds'.format(len(sources), len(self.sources)))
+        log.debug(f'Found {len(sources)} unique sources in {len(self.sources)} total embeds')
         self.sources = []
 
         for source in sources:
-            dest_rel_path = '{}-{}.{}'.format(
-                    source.source_rel, source.page_index, self.config['format'])
+            dest_rel_path = f'{source.source_rel}-{source.page_index}.{self.config['format']}'
             abs_src_path = os.path.join(config['docs_dir'], source.source_rel)
             abs_dest_path = os.path.join(config['site_dir'], dest_rel_path)
             cache_filename, exit_status = self.exporter.ensure_file_cached(
                     abs_src_path, source.source_rel, source.page_index,
-                    self.config['drawio_executable'], self.config['drawio_args'],
-                    self.config['cache_dir'], self.config['format'])
+                    self.config)
 
             if exit_status not in (None, 0):
-                log.error('Export failed with exit status {}; skipping copy'.format(exit_status))
+                log.error(f'Export failed with exit status {exit_status}; skipping copy')
                 continue
 
             try:
                 copy_file(cache_filename, abs_dest_path)
             except FileNotFoundError:
-                log.warn('Export successful, but wrote no output file')
+                log.warning('Export successful, but wrote no output file')
```

