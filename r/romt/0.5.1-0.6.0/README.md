# Comparing `tmp/romt-0.5.1.tar.gz` & `tmp/romt-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "romt-0.5.1.tar", max compression
+gzip compressed data, was "romt-0.6.0.tar", max compression
```

## Comparing `romt-0.5.1.tar` & `romt-0.6.0.tar`

### file list

```diff
@@ -1,25 +1,27 @@
--rw-r--r--   0        0        0    11198 2024-03-05 10:44:03.573648 romt-0.5.1/CHANGES.rst
--rw-r--r--   0        0        0     1122 2022-03-27 00:55:58.237668 romt-0.5.1/LICENSE.rst
--rw-r--r--   0        0        0    65899 2024-03-02 18:56:09.843788 romt-0.5.1/README.rst
--rw-r--r--   0        0        0     2149 2024-02-29 08:50:17.419836 romt-0.5.1/maintainer.rst
--rwxr-xr-x   0        0        0      315 2024-02-29 08:50:17.419836 romt-0.5.1/make-exec-darwin.sh
--rwxr-xr-x   0        0        0      249 2024-02-29 08:50:17.419836 romt-0.5.1/make-exec-linux.sh
--rw-r--r--   0        0        0      246 2024-02-29 08:50:17.419836 romt-0.5.1/make-exec-windows.bat
--rw-r--r--   0        0        0     3722 2024-03-05 10:33:46.116058 romt-0.5.1/pyproject.toml
--rwxr-xr-x   0        0        0       57 2022-03-27 00:55:58.237668 romt-0.5.1/romt-wrapper.py
--rw-r--r--   0        0        0        0 2022-03-27 00:55:58.241668 romt-0.5.1/src/romt/__init__.py
--rw-r--r--   0        0        0     1614 2024-02-29 08:50:17.423836 romt-0.5.1/src/romt/base.py
--rw-r--r--   0        0        0     5614 2024-02-29 08:50:17.423836 romt-0.5.1/src/romt/cli.py
--rw-r--r--   0        0        0     5503 2024-02-29 08:50:17.423836 romt-0.5.1/src/romt/common.py
--rw-r--r--   0        0        0    36373 2024-02-29 08:50:17.423836 romt-0.5.1/src/romt/crate.py
--rw-r--r--   0        0        0     2616 2024-02-29 08:50:17.423836 romt-0.5.1/src/romt/dist.py
--rw-r--r--   0        0        0     8216 2024-02-29 08:50:17.423836 romt-0.5.1/src/romt/download.py
--rw-r--r--   0        0        0     2314 2024-02-29 08:50:17.423836 romt-0.5.1/src/romt/error.py
--rw-r--r--   0        0        0     2049 2024-02-29 08:50:17.423836 romt-0.5.1/src/romt/integrity.py
--rw-r--r--   0        0        0     6900 2024-02-29 08:50:17.423836 romt-0.5.1/src/romt/manifest.py
--rw-r--r--   0        0        0       93 2024-02-29 08:50:17.423836 romt-0.5.1/src/romt/py.typed
--rw-r--r--   0        0        0    17677 2024-02-29 08:50:17.427836 romt-0.5.1/src/romt/rustup.py
--rw-r--r--   0        0        0     6406 2024-02-29 08:50:17.427836 romt-0.5.1/src/romt/serve.py
--rw-r--r--   0        0        0     7457 2024-02-29 08:50:17.427836 romt-0.5.1/src/romt/signature.py
--rw-r--r--   0        0        0    26142 2024-03-02 18:46:58.786858 romt-0.5.1/src/romt/toolchain.py
--rw-r--r--   0        0        0    67077 1970-01-01 00:00:00.000000 romt-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0    11692 2024-04-20 17:40:16.132832 romt-0.6.0/CHANGES.rst
+-rw-r--r--   0        0        0     1122 2022-03-27 00:55:58.237668 romt-0.6.0/LICENSE.rst
+-rw-r--r--   0        0        0    69410 2024-04-20 17:41:12.944064 romt-0.6.0/README.rst
+-rw-r--r--   0        0        0     2149 2024-02-29 08:50:17.419836 romt-0.6.0/maintainer.rst
+-rwxr-xr-x   0        0        0      315 2024-02-29 08:50:17.419836 romt-0.6.0/make-exec-darwin.sh
+-rwxr-xr-x   0        0        0      249 2024-04-20 13:18:31.896068 romt-0.6.0/make-exec-linux.sh
+-rw-r--r--   0        0        0      246 2024-02-29 08:50:17.419836 romt-0.6.0/make-exec-windows.bat
+-rw-r--r--   0        0        0    90538 2024-04-20 13:18:31.896068 romt-0.6.0/poetry.lock
+-rw-r--r--   0        0        0     3815 2024-04-20 13:18:31.896068 romt-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     9162 2024-04-20 19:25:11.631664 romt-0.6.0/requirements.txt
+-rwxr-xr-x   0        0        0       57 2022-03-27 00:55:58.237668 romt-0.6.0/romt-wrapper.py
+-rw-r--r--   0        0        0        0 2022-03-27 00:55:58.241668 romt-0.6.0/src/romt/__init__.py
+-rw-r--r--   0        0        0     1614 2024-02-29 08:50:17.423836 romt-0.6.0/src/romt/base.py
+-rw-r--r--   0        0        0     5614 2024-02-29 08:50:17.423836 romt-0.6.0/src/romt/cli.py
+-rw-r--r--   0        0        0     5503 2024-02-29 08:50:17.423836 romt-0.6.0/src/romt/common.py
+-rw-r--r--   0        0        0    36373 2024-02-29 08:50:17.423836 romt-0.6.0/src/romt/crate.py
+-rw-r--r--   0        0        0     2616 2024-02-29 08:50:17.423836 romt-0.6.0/src/romt/dist.py
+-rw-r--r--   0        0        0     8216 2024-02-29 08:50:17.423836 romt-0.6.0/src/romt/download.py
+-rw-r--r--   0        0        0     2314 2024-02-29 08:50:17.423836 romt-0.6.0/src/romt/error.py
+-rw-r--r--   0        0        0     2049 2024-02-29 08:50:17.423836 romt-0.6.0/src/romt/integrity.py
+-rw-r--r--   0        0        0     6900 2024-02-29 08:50:17.423836 romt-0.6.0/src/romt/manifest.py
+-rw-r--r--   0        0        0       93 2024-02-29 08:50:17.423836 romt-0.6.0/src/romt/py.typed
+-rw-r--r--   0        0        0    17677 2024-02-29 08:50:17.427836 romt-0.6.0/src/romt/rustup.py
+-rw-r--r--   0        0        0     7383 2024-04-20 16:03:02.608214 romt-0.6.0/src/romt/serve.py
+-rw-r--r--   0        0        0     7457 2024-02-29 08:50:17.427836 romt-0.6.0/src/romt/signature.py
+-rw-r--r--   0        0        0    26142 2024-03-02 18:46:58.786858 romt-0.6.0/src/romt/toolchain.py
+-rw-r--r--   0        0        0    70588 1970-01-01 00:00:00.000000 romt-0.6.0/PKG-INFO
```

### Comparing `romt-0.5.1/CHANGES.rst` & `romt-0.6.0/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,25 @@
 *******
 History
 *******
 
+Version 0.6.0
+=============
+
+- Include ``poetry.lock`` and ``requirements.txt`` in the generated
+  ``romt-x.y.z.tar.gz`` source archive.  This allows explicit use of locked
+  versions for all dependencies when installing from PyPI.
+
+- Extend ``romt serve`` to support the "sparse" index protocol.  This requires
+  adjustments to the ``.cargo/config.toml`` file; see the ``README.rst`` file
+  for details.
+
+- Document how to use ``nxingx`` to serve the "sparse" ``crates.io-index``
+  protocol.
+
 Version 0.5.1
 =============
 
 - Remove extraneous artifacts from the built ``romt-x.y.z-*.whl`` file.  In the
   absence of a specified ``format`` option, these should have been present only
   in the source distribution file ``romt-x.y.z.tar.gz`` according to the Poetry
   documentation (https://python-poetry.org/docs/pyproject/#include-and-exclude).
```

### Comparing `romt-0.5.1/LICENSE.rst` & `romt-0.6.0/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `romt-0.5.1/README.rst` & `romt-0.6.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 Romt (Rust Offline Mirror Tool) aids in using the Rust programming language in
 an offline context.  Instructions and tooling are provided for:
 
 - Mirroring of Rust ecosystem artifacts:
 
   - Toolchains (Rustc, Cargo, libraries, etc.)
   - Rustup (toolchain multiplexer)
-  - Crates.io (community-supplied Crates)
+  - Crates.io (community-supplied Crates) with "sparse" index support.
 
 - Incremental artifact downloading (with a configurable number of simultaneous
   download jobs).
 
 - Incremental artifact transfer to offline network.
 
 - Artifact serving in offline context (offline computer, disconnected network).
@@ -83,65 +83,86 @@
 The simplest method of installation is to use a pre-built self-contained
 executable from the Github release area:
 https://github.com/drmikehenry/romt/releases
 
 Option 2: Install from Python Package Index
 -------------------------------------------
 
-Romt is also available in the Python Package Index (PyPI).  For machines with
-direct Internet access, installation is straightforward; for machines on a
-disconnected network, more steps are required.
+Romt is also available in the Python Package Index (PyPI).
 
-First ensure that the ``PATH`` contains the directory that holds installed
-Python packages::
+- Download ``romt`` source and all dependencies on a host with direct Internet
+  access:
 
-    # For Linux:
-    ~/.local/bin
+  - Prepare ``romt`` download area:
 
-    # For Windows with Python version X.Y:
-    %APPDATA%\Python\PythonXY\Scripts
+    .. code-block:: sh
+
+      mkdir romt
+      cd romt
 
-Next, choose installation method based on access to the Internet:
+  - Download poetry and dependencies:
 
-- With direct Internet access:
+    .. code-block:: sh
+
+      pip download poetry
 
-  - Install directly from PyPI:
+  - Download the ``romt`` source:
 
     .. code-block:: sh
 
-      pip install --user romt
+      pip download --no-binary :all: --no-deps romt
 
-- On a disconnected Network:
+  - Unpack the ``romt`` source tarball ``romt-*.tar.gz``:
+
+    .. code-block:: sh
 
-  - Download ``romt`` with dependencies (from Internet-connected machine):
+      # Example for Linux:
+      tar -zxf romt-*.tar.gz
+
+  - Download the dependencies from ``requirements.txt``:
 
     .. code-block:: sh
 
-      mkdir romt
-      cd romt
-      pip download romt
+      pip download -r romt-*/requirements.txt
 
-  - Transfer the ``romt`` directory to a machine on the disconnected network.
+- If installing to an offline host, transfer the entire ``romt/`` download area
+  to that host.
 
-  - Install from the ``romt`` directory:
+- Ensure that the ``PATH`` contains the directory that holds installed Python
+  packages::
 
-    .. code-block:: sh
+      # For Linux:
+      ~/.local/bin
 
-      cd romt
-      pip install --user --no-index --find-links . romt
+      # For Windows with Python version X.Y:
+      %APPDATA%\Python\PythonXY\Scripts
+
+- Install ``romt`` from the current directory of sources (ensuring the current
+  working directory is the ``romt/`` download area):
+
+  .. code-block:: sh
+
+    pip install --user --no-index --find-links . romt
 
 Option 3: Work with source
 --------------------------
 
 If desired, the source may be cloned from Github and installed into a virtual
 environment.
 
 - Install Poetry globally as described in the documentation:
   https://python-poetry.org/docs/#installation
 
+  Include the ``poetry-plugin-export`` plugin as well.  Assuming ``pipx`` was
+  used for installation of poetry itself, this is done via::
+
+    pipx inject poetry poetry-plugin-export
+
+  This plugin is needed for generating a ``requirements.txt`` file.
+
 - Clone source:
 
   .. code-block:: sh
 
     git clone https://github.com/drmikehenry/romt
     cd romt
 
@@ -430,40 +451,56 @@
 
 - Try out some rustup commands::
 
     rustup self update
     rustup component add rust-src
 
 - Create the text file ``~/.cargo/config.toml``
-  (``%USERPROFILE%\.cargo\config.toml`` on Windows) with the following content::
-
-    [source.crates-io]
-    registry = 'http://localhost:8000/git/crates.io-index'
-
-    # Disable cert revocation checking (necessary only on Windows):
-    [http]
-    check-revoke = false
-
-    # For greatly improved performance, have Cargo use the Git command-line
-    # client to acquire `crates.io-index` repository. See
-    # https://github.com/rust-lang/cargo/issues/9167 for details.
-    [net]
-    git-fetch-with-cli = true
+  (``%USERPROFILE%\.cargo\config.toml`` on Windows) to use ``romt serve``. With
+  a Rust toolchain from 2022-06-20 or later, the "sparse" protocol may be used.
+  This is significantly faster than the older Git-based method.
+
+  - For the sparse index method, use the following contents for the
+    ``config.toml`` file::
+
+      [source.crates-io]
+      registry = 'sparse+http://localhost:8000/crates-index/'
+
+      # Disable cert revocation checking (necessary only on Windows):
+      [http]
+      check-revoke = false
+
+  - For the older Git-based index method, use the following contents for the
+    ``config.toml`` file::
+
+      [source.crates-io]
+      registry = 'http://localhost:8000/git/crates.io-index'
+
+      # Disable cert revocation checking (necessary only on Windows):
+      [http]
+      check-revoke = false
+
+      # For greatly improved performance, have Cargo use the Git command-line
+      # client to acquire `crates.io-index` repository. See
+      # https://github.com/rust-lang/cargo/issues/9167 for details.
+      [net]
+      git-fetch-with-cli = true
 
 - Create a sample project to demonstrate crate usage:
 
   .. code-block:: sh
 
     cargo new rand_test
     cd rand_test
 
-- Append the following line to ``Cargo.toml`` (just below the
-  ``[dependencies]`` line)::
+- Add the ``rand`` crate to the build:
 
-    rand = ""
+  .. code-block:: sh
+
+    cargo add rand
 
 - Fetch ``rand`` and its dependencies::
 
     cargo fetch
 
 Upgrading from Romt versions before 0.4.0
 =========================================
@@ -1764,14 +1801,21 @@
 Rust artifacts may optionally be served via the nginx web server.  A simple
 example for Ubuntu Linux is shown below.  If you change host or port values
 below, configure the index repository via:
 .. code-block:: sh
 
   romt crate config --server-url <SERVER_URL>
 
+``nginx`` with Perl support and ``fcgiwrap`` are required.  On Ubuntu, these may
+be installed via:
+
+.. code-block:: sh
+
+  apt install nginx-extras fcgiwrap
+
 Below is a sample nginx configuration.
 
 Place the following content into ``/etc/nginx/sites-available/rust``.  Make
 adjustments as indicated by each ``TODO``.  These instructions assume crates
 are stored using lowercase prefixes; if using mixed-case prefixes, adjust as
 directed by the ``TODO`` comments::
 
@@ -1797,14 +1841,29 @@
       include       fastcgi_params;
       fastcgi_pass  unix:/var/run/fcgiwrap.socket;
       fastcgi_param SCRIPT_FILENAME     /usr/lib/git-core/git-http-backend;
       fastcgi_param GIT_HTTP_EXPORT_ALL "";
       fastcgi_param PATH_INFO           $1;
     }
 
+    # Support "sparse" `crates.io-index` protocol.
+    location ~ /crates-index/(.*) {
+
+      # TODO: Change to absolute path to mirror/git directory:
+      fastcgi_param CRATE_INDEX_ROOT    /ABSOLUTE/PATH/TO/mirror/git/crates.io-index;
+
+      include       fastcgi_params;
+      fastcgi_pass  unix:/var/run/fcgiwrap.socket;
+      # TODO: Adjust path to `cgi-crates-index` CGI script as needed:
+      fastcgi_param SCRIPT_FILENAME     /usr/lib/cgi-bin/cgi-crates-index;
+      fastcgi_param GIT_HTTP_EXPORT_ALL "";
+      fastcgi_param PATH_INFO           $1;
+    }
+
+
     # Rewrite URLs like /crates/{crate}/{crate}-{version}.crate to use
     # a prefix based on the crate name.  Special cases for crate names
     # with 1, 2, 3, and 4-or-more characters:
     #   a/a-{version}.crate         -> 1/a/a-{version}.crate
     #   ab/ab-{version}.crate       -> 2/aa/ab-{version}.crate
     #   abc/abc-{version}.crate     -> 3/a/abc/abc-{version}.crate
     #   abcd*/abcd*-{version}.crate -> ab/cd/abcd*-{version}.crate
@@ -1816,14 +1875,84 @@
     # rewrite "^/crates/([^/])/([^/]+)$"                     "/crates/1/$1/$2"  last;
     # rewrite "^/crates/([^/]{2})/([^/]+)$"                  "/crates/2/$1/$2"  last;
     # rewrite "^/crates/([^/])([^/]{2})/([^/]+)$"            "/crates/3/$1/$1$2/$3"  last;
     # rewrite "^/crates/([^/]{2})([^/]{2})([^/]*)/([^/]+)$"  "/crates/$1/$2/$1$2$3/$4" last;
 
   }
 
+Serving the ``crates.io-index`` with the "sparse" protocol requires the creation
+of the following ``cgi-crates-index`` CGI script.  On Ubuntu, such scripts live
+in ``/usr/lib/cgi-bin``; e.g.:
+
+- Create ``/usr/lib/cgi-bin`` directory if necessary:
+
+.. code-block:: sh
+
+  mkdir -p /usr/lib/cgi-bin
+
+- Create ``/usr/lib/cgi-bin/cgi-crates-index`` with contents:
+
+  .. code-block:: perl
+
+    #!/usr/bin/perl
+
+    use strict;
+    use warnings;
+
+    sub send_content {
+        my ($content_type, $body) = @_;
+        my $content_length = length($body);
+        print "Content-Type: $content_type\r\n";
+        print "Content-Length: $content_length\r\n";
+        print "\r\n";
+        print "$body"
+    }
+
+    sub send_404 {
+        print "Status: 404 Not Found\r\n";
+        send_content('text/html', <<'END');
+    <html>
+    <head><title>404 Not Found</title></head>
+    <body>
+    <h1>404 Not Found</h1>
+    </body>
+    </html>
+    END
+    }
+
+    my $repo = $ENV{CRATE_INDEX_ROOT};
+    my $path_info = $ENV{PATH_INFO} || "config.json";
+
+    my $pipe;
+    if (open($pipe, '-|', "git -C $repo show master:$path_info")) {
+        my $body;
+        {
+            local $/; # Slurp mode.
+            $body = <$pipe>;
+        }
+        if (close($pipe)) {
+            send_content('application/octet-stream', $body);
+        } else {
+            send_404();
+        }
+    } else {
+        send_404();
+    }
+
+  Note that the user running the CGI script must own the ``crates.io-index``
+  tree or else Git may throw errors such as::
+
+    fatal: detected dubious ownership in repository at '/.../crates.io-index'
+
+- Make ``/usr/lib/cgi-bin/cgi-crates-index`` executable:
+
+  .. code-block:: sh
+
+    chmod +x /usr/lib/cgi-bin/cgi-crates-index
+
 Serving crates with lowercase prefixes requires Perl support in nginx (on
 Ubuntu, this requires the package ``nginx-extras`` instead of ``nginx-full``);
 Perl support is not required for mixed-case prefixes.  To serve crates with
 lowercase prefixes, create the file ``/etc/nginx/conf.d/perl.conf`` with the
 below contents::
 
   # Reference: https://nginx.org/en/docs/http/ngx_http_perl_module.html
```

### Comparing `romt-0.5.1/maintainer.rst` & `romt-0.6.0/maintainer.rst`

 * *Files identical despite different names*

### Comparing `romt-0.5.1/pyproject.toml` & `romt-0.6.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 [tool.poetry]
 name = "romt"
-version = "0.5.1"
+version = "0.6.0"
 include = [
   { path = "CHANGES.rst", format="sdist" },
   { path = "LICENSE.rst", format="sdist" },
   { path = "README.rst", format="sdist" },
   { path = "maintainer.rst", format="sdist" },
   { path = "make-exec-darwin.sh", format="sdist" },
   { path = "make-exec-linux.sh", format="sdist" },
   { path = "make-exec-windows.bat", format="sdist" },
+  { path = "poetry.lock", format="sdist" },
+  { path = "requirements.txt", format="sdist" },
   { path = "romt-wrapper.py", format="sdist" },
 ]
 description = """\
   Romt (Rust Offline Mirror Tool) enables mirroring of Rust \
   programming language tools and crates for use in an offline context.\
 """
 keywords = ["Rust", "mirror", "toolchain", "crates"]
```

### Comparing `romt-0.5.1/src/romt/base.py` & `romt-0.6.0/src/romt/base.py`

 * *Files identical despite different names*

### Comparing `romt-0.5.1/src/romt/cli.py` & `romt-0.6.0/src/romt/cli.py`

 * *Files identical despite different names*

### Comparing `romt-0.5.1/src/romt/common.py` & `romt-0.6.0/src/romt/common.py`

 * *Files identical despite different names*

### Comparing `romt-0.5.1/src/romt/crate.py` & `romt-0.6.0/src/romt/crate.py`

 * *Files identical despite different names*

### Comparing `romt-0.5.1/src/romt/dist.py` & `romt-0.6.0/src/romt/dist.py`

 * *Files identical despite different names*

### Comparing `romt-0.5.1/src/romt/download.py` & `romt-0.6.0/src/romt/download.py`

 * *Files identical despite different names*

### Comparing `romt-0.5.1/src/romt/error.py` & `romt-0.6.0/src/romt/error.py`

 * *Files identical despite different names*

### Comparing `romt-0.5.1/src/romt/integrity.py` & `romt-0.6.0/src/romt/integrity.py`

 * *Files identical despite different names*

### Comparing `romt-0.5.1/src/romt/manifest.py` & `romt-0.6.0/src/romt/manifest.py`

 * *Files identical despite different names*

### Comparing `romt-0.5.1/src/romt/rustup.py` & `romt-0.6.0/src/romt/rustup.py`

 * *Files identical despite different names*

### Comparing `romt-0.5.1/src/romt/serve.py` & `romt-0.6.0/src/romt/serve.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import argparse
+import http
 import http.server
 import os
 from pathlib import Path
+import subprocess
 from typing import Optional
 
 import romt.crate
 from romt import common
 
 description = """\
 Serve Rust artifacts via http.
@@ -104,21 +106,45 @@
                 os.path.basename(path),
             )
 
         if self.path != path:
             common.iprint(f"Rewrite URL: {self.path} -> {path}")
             self.path = path
 
+    def _git_show(self, path: str) -> bytes:
+        body = subprocess.check_output(
+            ["git", "-C", "git/crates.io-index", "show", f"master:{path}"]
+        )
+        return body
+
+    def _handle_sparse_index(self, *, with_body: bool) -> bool:
+        prefix = "/crates-index/"
+        if not self.path.startswith(prefix):
+            return False
+        try:
+            body = self._git_show(self.path[len(prefix) :])
+        except subprocess.CalledProcessError:
+            self.send_error(http.HTTPStatus.NOT_FOUND, "File not found")
+            return True
+        self.send_response(http.HTTPStatus.OK)
+        self.send_header("Content-Type", "application/octet-stream")
+        self.send_header("Content-Length", str(len(body)))
+        self.end_headers()
+
+        if with_body:
+            self.wfile.write(body)
+        return True
+
     def do_get(self) -> None:
         self._rewrite_path()
-        super().do_GET()
+        self._handle_sparse_index(with_body=True) or super().do_GET()
 
     def do_head(self) -> None:
         self._rewrite_path()
-        super().do_HEAD()
+        self._handle_sparse_index(with_body=False) or super().do_HEAD()
 
     def do_post(self) -> None:
         self._rewrite_path()
         super().do_POST()
 
 
 # Work-around for non-compliant do_ALLCAPS functions.
```

### Comparing `romt-0.5.1/src/romt/signature.py` & `romt-0.6.0/src/romt/signature.py`

 * *Files identical despite different names*

### Comparing `romt-0.5.1/src/romt/toolchain.py` & `romt-0.6.0/src/romt/toolchain.py`

 * *Files identical despite different names*

### Comparing `romt-0.5.1/PKG-INFO` & `romt-0.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: romt
-Version: 0.5.1
+Version: 0.6.0
 Summary: Romt (Rust Offline Mirror Tool) enables mirroring of Rust programming language tools and crates for use in an offline context.
 Home-page: https://github.com/drmikehenry/romt
 License: MIT
 Keywords: Rust,mirror,toolchain,crates
 Author: Michael Henry
 Author-email: drmikehenry@drmikehenry.com
 Requires-Python: >=3.8,<3.13
@@ -34,15 +34,15 @@
 Romt (Rust Offline Mirror Tool) aids in using the Rust programming language in
 an offline context.  Instructions and tooling are provided for:
 
 - Mirroring of Rust ecosystem artifacts:
 
   - Toolchains (Rustc, Cargo, libraries, etc.)
   - Rustup (toolchain multiplexer)
-  - Crates.io (community-supplied Crates)
+  - Crates.io (community-supplied Crates) with "sparse" index support.
 
 - Incremental artifact downloading (with a configurable number of simultaneous
   download jobs).
 
 - Incremental artifact transfer to offline network.
 
 - Artifact serving in offline context (offline computer, disconnected network).
@@ -112,65 +112,86 @@
 The simplest method of installation is to use a pre-built self-contained
 executable from the Github release area:
 https://github.com/drmikehenry/romt/releases
 
 Option 2: Install from Python Package Index
 -------------------------------------------
 
-Romt is also available in the Python Package Index (PyPI).  For machines with
-direct Internet access, installation is straightforward; for machines on a
-disconnected network, more steps are required.
+Romt is also available in the Python Package Index (PyPI).
 
-First ensure that the ``PATH`` contains the directory that holds installed
-Python packages::
+- Download ``romt`` source and all dependencies on a host with direct Internet
+  access:
 
-    # For Linux:
-    ~/.local/bin
+  - Prepare ``romt`` download area:
 
-    # For Windows with Python version X.Y:
-    %APPDATA%\Python\PythonXY\Scripts
+    .. code-block:: sh
+
+      mkdir romt
+      cd romt
 
-Next, choose installation method based on access to the Internet:
+  - Download poetry and dependencies:
 
-- With direct Internet access:
+    .. code-block:: sh
+
+      pip download poetry
 
-  - Install directly from PyPI:
+  - Download the ``romt`` source:
 
     .. code-block:: sh
 
-      pip install --user romt
+      pip download --no-binary :all: --no-deps romt
 
-- On a disconnected Network:
+  - Unpack the ``romt`` source tarball ``romt-*.tar.gz``:
+
+    .. code-block:: sh
 
-  - Download ``romt`` with dependencies (from Internet-connected machine):
+      # Example for Linux:
+      tar -zxf romt-*.tar.gz
+
+  - Download the dependencies from ``requirements.txt``:
 
     .. code-block:: sh
 
-      mkdir romt
-      cd romt
-      pip download romt
+      pip download -r romt-*/requirements.txt
 
-  - Transfer the ``romt`` directory to a machine on the disconnected network.
+- If installing to an offline host, transfer the entire ``romt/`` download area
+  to that host.
 
-  - Install from the ``romt`` directory:
+- Ensure that the ``PATH`` contains the directory that holds installed Python
+  packages::
 
-    .. code-block:: sh
+      # For Linux:
+      ~/.local/bin
 
-      cd romt
-      pip install --user --no-index --find-links . romt
+      # For Windows with Python version X.Y:
+      %APPDATA%\Python\PythonXY\Scripts
+
+- Install ``romt`` from the current directory of sources (ensuring the current
+  working directory is the ``romt/`` download area):
+
+  .. code-block:: sh
+
+    pip install --user --no-index --find-links . romt
 
 Option 3: Work with source
 --------------------------
 
 If desired, the source may be cloned from Github and installed into a virtual
 environment.
 
 - Install Poetry globally as described in the documentation:
   https://python-poetry.org/docs/#installation
 
+  Include the ``poetry-plugin-export`` plugin as well.  Assuming ``pipx`` was
+  used for installation of poetry itself, this is done via::
+
+    pipx inject poetry poetry-plugin-export
+
+  This plugin is needed for generating a ``requirements.txt`` file.
+
 - Clone source:
 
   .. code-block:: sh
 
     git clone https://github.com/drmikehenry/romt
     cd romt
 
@@ -459,40 +480,56 @@
 
 - Try out some rustup commands::
 
     rustup self update
     rustup component add rust-src
 
 - Create the text file ``~/.cargo/config.toml``
-  (``%USERPROFILE%\.cargo\config.toml`` on Windows) with the following content::
-
-    [source.crates-io]
-    registry = 'http://localhost:8000/git/crates.io-index'
-
-    # Disable cert revocation checking (necessary only on Windows):
-    [http]
-    check-revoke = false
-
-    # For greatly improved performance, have Cargo use the Git command-line
-    # client to acquire `crates.io-index` repository. See
-    # https://github.com/rust-lang/cargo/issues/9167 for details.
-    [net]
-    git-fetch-with-cli = true
+  (``%USERPROFILE%\.cargo\config.toml`` on Windows) to use ``romt serve``. With
+  a Rust toolchain from 2022-06-20 or later, the "sparse" protocol may be used.
+  This is significantly faster than the older Git-based method.
+
+  - For the sparse index method, use the following contents for the
+    ``config.toml`` file::
+
+      [source.crates-io]
+      registry = 'sparse+http://localhost:8000/crates-index/'
+
+      # Disable cert revocation checking (necessary only on Windows):
+      [http]
+      check-revoke = false
+
+  - For the older Git-based index method, use the following contents for the
+    ``config.toml`` file::
+
+      [source.crates-io]
+      registry = 'http://localhost:8000/git/crates.io-index'
+
+      # Disable cert revocation checking (necessary only on Windows):
+      [http]
+      check-revoke = false
+
+      # For greatly improved performance, have Cargo use the Git command-line
+      # client to acquire `crates.io-index` repository. See
+      # https://github.com/rust-lang/cargo/issues/9167 for details.
+      [net]
+      git-fetch-with-cli = true
 
 - Create a sample project to demonstrate crate usage:
 
   .. code-block:: sh
 
     cargo new rand_test
     cd rand_test
 
-- Append the following line to ``Cargo.toml`` (just below the
-  ``[dependencies]`` line)::
+- Add the ``rand`` crate to the build:
 
-    rand = ""
+  .. code-block:: sh
+
+    cargo add rand
 
 - Fetch ``rand`` and its dependencies::
 
     cargo fetch
 
 Upgrading from Romt versions before 0.4.0
 =========================================
@@ -1793,14 +1830,21 @@
 Rust artifacts may optionally be served via the nginx web server.  A simple
 example for Ubuntu Linux is shown below.  If you change host or port values
 below, configure the index repository via:
 .. code-block:: sh
 
   romt crate config --server-url <SERVER_URL>
 
+``nginx`` with Perl support and ``fcgiwrap`` are required.  On Ubuntu, these may
+be installed via:
+
+.. code-block:: sh
+
+  apt install nginx-extras fcgiwrap
+
 Below is a sample nginx configuration.
 
 Place the following content into ``/etc/nginx/sites-available/rust``.  Make
 adjustments as indicated by each ``TODO``.  These instructions assume crates
 are stored using lowercase prefixes; if using mixed-case prefixes, adjust as
 directed by the ``TODO`` comments::
 
@@ -1826,14 +1870,29 @@
       include       fastcgi_params;
       fastcgi_pass  unix:/var/run/fcgiwrap.socket;
       fastcgi_param SCRIPT_FILENAME     /usr/lib/git-core/git-http-backend;
       fastcgi_param GIT_HTTP_EXPORT_ALL "";
       fastcgi_param PATH_INFO           $1;
     }
 
+    # Support "sparse" `crates.io-index` protocol.
+    location ~ /crates-index/(.*) {
+
+      # TODO: Change to absolute path to mirror/git directory:
+      fastcgi_param CRATE_INDEX_ROOT    /ABSOLUTE/PATH/TO/mirror/git/crates.io-index;
+
+      include       fastcgi_params;
+      fastcgi_pass  unix:/var/run/fcgiwrap.socket;
+      # TODO: Adjust path to `cgi-crates-index` CGI script as needed:
+      fastcgi_param SCRIPT_FILENAME     /usr/lib/cgi-bin/cgi-crates-index;
+      fastcgi_param GIT_HTTP_EXPORT_ALL "";
+      fastcgi_param PATH_INFO           $1;
+    }
+
+
     # Rewrite URLs like /crates/{crate}/{crate}-{version}.crate to use
     # a prefix based on the crate name.  Special cases for crate names
     # with 1, 2, 3, and 4-or-more characters:
     #   a/a-{version}.crate         -> 1/a/a-{version}.crate
     #   ab/ab-{version}.crate       -> 2/aa/ab-{version}.crate
     #   abc/abc-{version}.crate     -> 3/a/abc/abc-{version}.crate
     #   abcd*/abcd*-{version}.crate -> ab/cd/abcd*-{version}.crate
@@ -1845,14 +1904,84 @@
     # rewrite "^/crates/([^/])/([^/]+)$"                     "/crates/1/$1/$2"  last;
     # rewrite "^/crates/([^/]{2})/([^/]+)$"                  "/crates/2/$1/$2"  last;
     # rewrite "^/crates/([^/])([^/]{2})/([^/]+)$"            "/crates/3/$1/$1$2/$3"  last;
     # rewrite "^/crates/([^/]{2})([^/]{2})([^/]*)/([^/]+)$"  "/crates/$1/$2/$1$2$3/$4" last;
 
   }
 
+Serving the ``crates.io-index`` with the "sparse" protocol requires the creation
+of the following ``cgi-crates-index`` CGI script.  On Ubuntu, such scripts live
+in ``/usr/lib/cgi-bin``; e.g.:
+
+- Create ``/usr/lib/cgi-bin`` directory if necessary:
+
+.. code-block:: sh
+
+  mkdir -p /usr/lib/cgi-bin
+
+- Create ``/usr/lib/cgi-bin/cgi-crates-index`` with contents:
+
+  .. code-block:: perl
+
+    #!/usr/bin/perl
+
+    use strict;
+    use warnings;
+
+    sub send_content {
+        my ($content_type, $body) = @_;
+        my $content_length = length($body);
+        print "Content-Type: $content_type\r\n";
+        print "Content-Length: $content_length\r\n";
+        print "\r\n";
+        print "$body"
+    }
+
+    sub send_404 {
+        print "Status: 404 Not Found\r\n";
+        send_content('text/html', <<'END');
+    <html>
+    <head><title>404 Not Found</title></head>
+    <body>
+    <h1>404 Not Found</h1>
+    </body>
+    </html>
+    END
+    }
+
+    my $repo = $ENV{CRATE_INDEX_ROOT};
+    my $path_info = $ENV{PATH_INFO} || "config.json";
+
+    my $pipe;
+    if (open($pipe, '-|', "git -C $repo show master:$path_info")) {
+        my $body;
+        {
+            local $/; # Slurp mode.
+            $body = <$pipe>;
+        }
+        if (close($pipe)) {
+            send_content('application/octet-stream', $body);
+        } else {
+            send_404();
+        }
+    } else {
+        send_404();
+    }
+
+  Note that the user running the CGI script must own the ``crates.io-index``
+  tree or else Git may throw errors such as::
+
+    fatal: detected dubious ownership in repository at '/.../crates.io-index'
+
+- Make ``/usr/lib/cgi-bin/cgi-crates-index`` executable:
+
+  .. code-block:: sh
+
+    chmod +x /usr/lib/cgi-bin/cgi-crates-index
+
 Serving crates with lowercase prefixes requires Perl support in nginx (on
 Ubuntu, this requires the package ``nginx-extras`` instead of ``nginx-full``);
 Perl support is not required for mixed-case prefixes.  To serve crates with
 lowercase prefixes, create the file ``/etc/nginx/conf.d/perl.conf`` with the
 below contents::
 
   # Reference: https://nginx.org/en/docs/http/ngx_http_perl_module.html
```

