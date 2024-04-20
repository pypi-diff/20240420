# Comparing `tmp/detect_advisor-1.0.4.tar.gz` & `tmp/detect_advisor-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "detect_advisor-1.0.4.tar", last modified: Mon Apr 15 11:25:57 2024, max compression
+gzip compressed data, was "detect_advisor-1.0.5.tar", last modified: Sat Apr 20 19:36:54 2024, max compression
```

## Comparing `detect_advisor-1.0.4.tar` & `detect_advisor-1.0.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:25:57.338917 detect_advisor-1.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-15 11:25:53.000000 detect_advisor-1.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    18374 2024-04-15 11:25:57.338917 detect_advisor-1.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    17807 2024-04-15 11:25:53.000000 detect_advisor-1.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:25:57.338917 detect_advisor-1.0.4/detect_advisor/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 11:25:53.000000 detect_advisor-1.0.4/detect_advisor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5175 2024-04-15 11:25:53.000000 detect_advisor-1.0.4/detect_advisor/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    24136 2024-04-15 11:25:53.000000 detect_advisor-1.0.4/detect_advisor/global_values.py
--rw-r--r--   0 runner    (1001) docker     (127)     3447 2024-04-15 11:25:53.000000 detect_advisor-1.0.4/detect_advisor/main.py
--rw-r--r--   0 runner    (1001) docker     (127)    11774 2024-04-15 11:25:53.000000 detect_advisor-1.0.4/detect_advisor/messages.py
--rw-r--r--   0 runner    (1001) docker     (127)    14503 2024-04-15 11:25:53.000000 detect_advisor-1.0.4/detect_advisor/output.py
--rw-r--r--   0 runner    (1001) docker     (127)    21418 2024-04-15 11:25:53.000000 detect_advisor-1.0.4/detect_advisor/process.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:25:57.338917 detect_advisor-1.0.4/detect_advisor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    18374 2024-04-15 11:25:57.000000 detect_advisor-1.0.4/detect_advisor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-15 11:25:57.000000 detect_advisor-1.0.4/detect_advisor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 11:25:57.000000 detect_advisor-1.0.4/detect_advisor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-15 11:25:57.000000 detect_advisor-1.0.4/detect_advisor.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-15 11:25:57.000000 detect_advisor-1.0.4/detect_advisor.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      699 2024-04-15 11:25:53.000000 detect_advisor-1.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 11:25:57.338917 detect_advisor-1.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 19:36:54.493340 detect_advisor-1.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-20 19:36:48.000000 detect_advisor-1.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    18374 2024-04-20 19:36:54.489340 detect_advisor-1.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    17807 2024-04-20 19:36:48.000000 detect_advisor-1.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 19:36:54.489340 detect_advisor-1.0.5/detect_advisor/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 19:36:48.000000 detect_advisor-1.0.5/detect_advisor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5175 2024-04-20 19:36:48.000000 detect_advisor-1.0.5/detect_advisor/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30270 2024-04-20 19:36:48.000000 detect_advisor-1.0.5/detect_advisor/global_values.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3447 2024-04-20 19:36:48.000000 detect_advisor-1.0.5/detect_advisor/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12469 2024-04-20 19:36:48.000000 detect_advisor-1.0.5/detect_advisor/messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14503 2024-04-20 19:36:48.000000 detect_advisor-1.0.5/detect_advisor/output.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22870 2024-04-20 19:36:48.000000 detect_advisor-1.0.5/detect_advisor/process.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 19:36:54.489340 detect_advisor-1.0.5/detect_advisor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    18374 2024-04-20 19:36:54.000000 detect_advisor-1.0.5/detect_advisor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-20 19:36:54.000000 detect_advisor-1.0.5/detect_advisor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 19:36:54.000000 detect_advisor-1.0.5/detect_advisor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-20 19:36:54.000000 detect_advisor-1.0.5/detect_advisor.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-20 19:36:54.000000 detect_advisor-1.0.5/detect_advisor.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-04-20 19:36:48.000000 detect_advisor-1.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 19:36:54.493340 detect_advisor-1.0.5/setup.cfg
```

### Comparing `detect_advisor-1.0.4/LICENSE` & `detect_advisor-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `detect_advisor-1.0.4/PKG-INFO` & `detect_advisor-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: detect_advisor
-Version: 1.0.4
+Version: 1.0.5
 Summary: Detect Advisor - prescan project folders to determine how to scan with Detect
 Author-email: Matthew Brady <mbrad@synopsys.com>
 Project-URL: Homepage, https://github.com/matthewb66/detect_advisor
 Project-URL: Issues, https://github.com/matthewb66/detect_advisor/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `detect_advisor-1.0.4/README.md` & `detect_advisor-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `detect_advisor-1.0.4/detect_advisor/config.py` & `detect_advisor-1.0.5/detect_advisor/config.py`

 * *Files identical despite different names*

### Comparing `detect_advisor-1.0.4/detect_advisor/global_values.py` & `detect_advisor-1.0.5/detect_advisor/global_values.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #
 # Constants
-advisor_version = "1.0.4"
+advisor_version = "1.0.5"
 detect_version = "9.X.0"
 
 ext_list = {
     'src': ['.4th', '.actionscript', '.ada', '.adb', '.ads', '.aidl', '.as', '.as8', '.asm', '.asp', '.aspx', '.aug',
             '.awk', '.bas', '.bash', '.bat', '.bf', '.bfpp', '.bi', '.bms', '.bmx', '.boo', '.c', '.c#', '.c++',
             '.cbl', '.cc', '.cfc', '.cfm', '.cgi', '.chai', '.clj', '.cljc', '.cljs', '.cls', '.cmd', '.com', '.cpp',
             '.cpy', '.cs', '.cu', '.cuh', '.cxx', '.d', '.dpk', '.dylan', '.e', '.ec', '.eh', '.el', '.erl', '.es',
@@ -34,34 +34,39 @@
 
 pm_dict = {
     'BAZEL':
         {
             'files': [],
             'exts': ['.bzl'],
             'execs': ['bazel'],
+            'exec_reqd': True,
+            'lock_files': [],
+            'lockfile_reqd': False,
             'accuracy': 'HIGH',
             'cli_options':
                 "--detect.bazel.path=PATH_TO_BAZEL\n" +
                 "    (OPTIONAL Path to bazel executable.)\n" +
                 "--detect.bazel.cquery.options='OPTION1,OPTION2'\n" +
                 "    (OPTIONAL List of additional options to pass to the bazel cquery command.)\n" +
                 "--detect.bazel.workspace.rules=<ALL, NONE, MAVEN_JAR, MAVEN_INSTALL, HASKELL_CABAL_LIBRARY, HTTP_ARCHIVE>\n" +
                 "    (OPTIONAL Bazel workspace external dependency rule: The Bazel workspace rule used to pull in external dependencies.\n" +
                 "    If not set, Detect will attempt to determine the rule from the contents of the WORKSPACE file (default: NONE).)\n",
             'cli_reqd':
                 "--detect.bazel.target='TARGET'\n" + \
                 "    (REQUIRED Bazel Target: The Bazel target (for example, //foo:foolib) for which dependencies are collected.)\n",
-
         },
     
     'BITBAKE':
         {
             'files': ['oe-init-build-env'],
             'exts': [],
             'execs': ['bitbake'],
+            'exec_reqd': True,
+            'lock_files': [],
+            'lockfile_reqd': False,
             'accuracy': 'HIGH',
             'linux_only': True,
             'cli_options':
                 "--detect.bitbake.package.names='PACKAGE1,PACKAGE2'\n" +
                 "    (OPTIONAL List of package names from which dependencies are extracted.)\n" +
                 "--detect.bitbake.search.depth=X\n" +
                 "    (OPTIONAL The depth at which Detect will search for the recipe-depends.dot or package-depends.dot files (default: 1).)\n" +
@@ -72,54 +77,69 @@
             'cli_reqd':
                 "--detect.bitbake.build.env.name=NAME\n" +
                 "    (REQUIRED BitBake Init Script Name: The name of the build environment init script (default: oe-init-build-env).)\n"
         },
     
     'CARGO':
         {
-            'files': ['Cargo.lock', 'Cargo.toml'],
+            'files': ['Cargo.toml'],
             'exts': [],
-            'execs': ['cargo'],
+            'execs': [],
+            'exec_reqd': False,
+            'lock_files': ['Cargo.lock'],
+            'lockfile_reqd': True,
             'accuracy': 'HIGH',
         },
     
     'CARTHAGE':
         {
-            'files': ['Cartfile', 'Cartfile.resolved'],
+            'files': ['Cartfile'],
             'exts': [],
-            'execs': ['carthage'],
+            'execs': [],
+            'exec_reqd': False,
+            'lock_files': ['Cartfile.resolved'],
+            'lockfile_reqd': True,
             'accuracy': 'HIGH',
         },
     
     'CLANG':
         {
             'files': ['compile_commands.json'],
             'exts': [],
             'execs': ['clang'],
+            'exec_reqd': True,
+            'lock_files': [],
+            'lockfile_reqd': False,
             'accuracy': 'HIGH',
             'linux_only': True,
             'cli_options':
                 "    Detect supports reading a compile_commands.json file generated by cmake.\n" +
                 "    However, it may be better to use the https://pypi.org/project/blackduck-c-cpp utility to scan C/C++ projects\n" +
                 "    which runs a full build scan\n",
         },
     
     'COCOAPODS':
         {
             'files': ['Podfile.lock'],
             'exts': [],
-            'execs': ['pod'],
+            'execs': [],
+            'exec_reqd': False,
+            'lock_files': ['Podfile.lock'],
+            'lockfile_reqd': True,
             'accuracy': 'HIGH',
         },
     
     'CONAN':
         {
-            'files': ['conanfile.txt', 'conanfile.py', 'conan.lock'],
+            'files': ['conanfile.txt', 'conanfile.py'],
             'exts': [],
             'execs': ['conan'],
+            'exec_reqd': False,
+            'lock_files': ['conan.lock'],
+            'lockfile_reqd': False,
             'accuracy': 'HIGH',
             'cli_options':
                 "--detect.conan.path=PATH_TO_CONAN\n" +
                 "    (OPTIONAL Path to conan executable.)\n" +
                 "--detect.bitbake.dependency.types.excluded=<NONE, BUILD>\n" +
                 "    (OPTIONAL Exclude dev dependencies - default NONE.)\n" +
                 "--detect.conan.arguments='ARG1 ARG2'\n" +
@@ -131,87 +151,172 @@
         },
     
     'CONDA':
         {
             'files': ['environment.yml'],
             'exts': [],
             'execs': ['conda'],
+            'lock_files': [],
+            'lockfile_reqd': False,
+            'exec_reqd': True,
             'accuracy': 'HIGH',
             'cli_options':
                 "--detect.conda.path=PATH_TO_CONDA\n" +
                 "    (OPTIONAL Path to conda executable)\n" +
                 "--detect.conda.environment.name=NAME\n" +
                 "    (OPTIONAL The name of the anaconda environment used by your project)\n",
         },
     
     'CPAN':
         {
             'files': ['Makefile.PL'],
             'exts': [],
             'execs': ['cpan', 'cpanm'],
+            'exec_reqd': True,
+            'lock_files': [],
+            'lockfile_reqd': False,
             'accuracy': 'HIGH',
             'cli_options':
                 "--detect.cpan.path=PATH_TO_CPAN\n" +
                 "    (OPTIONAL Path to cpan executable.)\n" +
                 "--detect.cpanm.path=PATH_TO_CPANM\n" +
                 "    (OPTIONAL Path to cpanm executable.)\n"
         },
     
     'CPP':
         {
             'files': ['makefile', 'CMakeLists.txt'],
             'exts': ['.mk'],
             'execs': ['cpp'],
+            'exec_reqd': False,
+            'lock_files': [],
+            'lockfile_reqd': False,
             'accuracy': 'HIGH',
             'cli_options':
                 "    C/C++ projects built using a compiler should be scanned using the blackduck_c_cpp utility.\n" + \
                 "    See https://pypi.org/project/blackduck-c-cpp.\n",
         },
     
     'CRAN':
         {
             'files': ['packrat.lock'],
             'exts': [],
-            'execs': ['cran'],
+            'execs': [],
+            'exec_reqd': False,
+            'lock_files': ['packrat.lock'],
+            'lockfile_reqd': True,
             'accuracy': 'HIGH',
         },
     
     'DART':
         {
-            'files': ['pubspec.yaml', 'pubspec.lock'],
+            'files': ['pubspec.yaml'],
             'exts': [],
             'execs': ['dart', 'flutter'],
+            'exec_reqd': False,
+            'lock_files': ['pubspec.lock'],
+            'lockfile_reqd': True,
             'accuracy': 'HIGH',
             'cli_options':
                 "--detect.dart.path=PATH_TO_DART\n" +
                 "    (OPTIONAL The path to the dart executable.)\n"
                 "--detect.flutter.path=PATH_TO_FLUTTER\n" +
                 "    (OPTIONAL The path to the flutter executable.)\n" +
                 "--detect.pub.dependency.types.excluded=<NONE, DEV>\n" +
                 "    (OPTIONAL Exclude dev dependencies - default NONE.)\n"
         },
     
-    'GO':
+    'GO_DEP':
+        {
+            'files': ['Gopkg.lock'],
+            'exts': [],
+            'execs': [],
+            'exec_reqd': False,
+            'lock_files': ['Gopkg.lock'],
+            'lockfile_reqd': True,
+            'accuracy': 'HIGH',
+            'cli_options':
+                "--detect.go.path=PATH_TO_GO\n" +
+                "    (OPTIONAL Path to the Go executable.)\n" +
+                "--detect.go.mod.dependency.types.excluded=<NONE, UNUSED, VENDORED>\n" +
+                "    (OPTIONAL Go Mod Dependency Types Excluded: Set this value to indicate which Go Mod dependency types Detect should exclude from the BOM.)\n"
+        },
+
+    'GO_GRADLE':
+        {
+            'files': ['gogradle.lock'],
+            'exts': [],
+            'execs': [],
+            'exec_reqd': False,
+            'lock_files': ['gogradle.lock'],
+            'lockfile_reqd': True,
+            'accuracy': 'HIGH',
+            'cli_options':
+                "--detect.go.path=PATH_TO_GO\n" +
+                "    (OPTIONAL Path to the Go executable.)\n" +
+                "--detect.go.mod.dependency.types.excluded=<NONE, UNUSED, VENDORED>\n" +
+                "    (OPTIONAL Go Mod Dependency Types Excluded: Set this value to indicate which Go Mod dependency types Detect should exclude from the BOM.)\n"
+        },
+
+    'GO_MOD':
         {
-            'files': ['Gopkg.lock', 'gogradle.lock', 'go.mod', 'vendor.json', 'vendor.conf'],
+            'files': ['go.mod'],
             'exts': [],
             'execs': ['go'],
+            'exec_reqd': True,
+            'lock_files': [],
+            'lockfile_reqd': False,
             'accuracy': 'HIGH',
             'cli_options':
                 "--detect.go.path=PATH_TO_GO\n" +
                 "    (OPTIONAL Path to the Go executable.)\n" +
                 "--detect.go.mod.dependency.types.excluded=<NONE, UNUSED, VENDORED>\n" +
                 "    (OPTIONAL Go Mod Dependency Types Excluded: Set this value to indicate which Go Mod dependency types Detect should exclude from the BOM.)\n"
         },
-    
+
+    'GO_VENDOR':
+        {
+            'files': ['vendor.json'],
+            'exts': [],
+            'execs': [],
+            'exec_reqd': False,
+            'lock_files': [],
+            'lockfile_reqd': False,
+            'accuracy': 'HIGH',
+            'cli_options':
+                "--detect.go.path=PATH_TO_GO\n" +
+                "    (OPTIONAL Path to the Go executable.)\n" +
+                "--detect.go.mod.dependency.types.excluded=<NONE, UNUSED, VENDORED>\n" +
+                "    (OPTIONAL Go Mod Dependency Types Excluded: Set this value to indicate which Go Mod dependency types Detect should exclude from the BOM.)\n"
+        },
+
+    'GO_VNDR':
+        {
+            'files': ['vendor.conf'],
+            'exts': [],
+            'execs': [],
+            'exec_reqd': False,
+            'lock_files': [],
+            'lockfile_reqd': False,
+            'accuracy': 'HIGH',
+            'cli_options':
+                "--detect.go.path=PATH_TO_GO\n" +
+                "    (OPTIONAL Path to the Go executable.)\n" +
+                "--detect.go.mod.dependency.types.excluded=<NONE, UNUSED, VENDORED>\n" +
+                "    (OPTIONAL Go Mod Dependency Types Excluded: Set this value to indicate which Go Mod dependency types Detect should exclude from the BOM.)\n"
+        },
+
     'GRADLE':
         {
             'files': ['build.gradle', 'build.gradle.kts'],
             'exts': [],
-            'execs': ['go'],
+            'execs': [],
+            'exec_reqd': False,
+            'lock_files': [],
+            'lockfile_reqd': False,
             'accuracy': 'LOW',
             'cli_options':
                 "--detect.gradle.path=PATH_TO_GRADLE\n" +
                 "    (OPTIONAL Path to the gradle or gradlew executable.)\n" +
                 "detect.gradle.configuration.types.excluded=<NONE, UNRESOLVED>\n" +
                 "    (OPTIONAL Gradle Configuration Types Excluded: Set this value to indicate which Gradle configuration types Detect should exclude from the BOM.)\n" +
                 "--detect.gradle.build.command='ARGUMENT1 ARGUMENT2'\n" +
@@ -229,33 +334,42 @@
         },
     
     'HEX':
         {
             'files': ['rebar.config'],
             'exts': [],
             'execs': ['rebar3'],
+            'exec_reqd': True,
+            'lock_files': [],
+            'lockfile_reqd': False,
             'accuracy': 'HIGH',
             'cli_options':
                 "--detect.hex.rebar3.path=PATH_TO_REBAR3\n" +
                 "    (OPTIONAL Path to the rebar3 executable.)\n"
         },
     
     'IVY':
         {
-            'files': ['ivy.xml', 'build.xml'],
+            'files': ['ivy.xml'],
             'exts': [],
-            'execs': ['ivy'],
+            'execs': [],
+            'exec_reqd': False,
+            'lock_files': [],
+            'lockfile_reqd': False,
             'accuracy': 'LOW',
         },
     
     'LERNA':
         {
             'files': ['lerna.json'],
             'exts': [],
             'execs': ['lerna'],
+            'exec_reqd': True,
+            'lock_files': ['package-lock.json', 'npm-shrinkwrap.json', 'yarn.lock'],
+            'lockfile_reqd': True,
             'accuracy': 'HIGH',
             'cli_options':
                 "--detect.lerna.path=PATH_TO_LERNA\n" +
                 "    (OPTIONAL Lerna Executable: Path of the lerna executable.)\n" +
                 "--detect.lerna.package.types.excluded=<NONE, PRIVATE>\n" +
                 "    (OPTIONAL Lerna Package Types Excluded: Set this value to indicate which Lerna package types Detect should exclude from the BOM.)\n" +
                 "--detect.lerna.excluded.packages=PACKAGE1,PACKAGE2\n" +
@@ -265,14 +379,17 @@
         },
     
     'MAVEN':
         {
             'files': ['pom.xml', 'pom.groovy'],
             'exts': [],
             'execs': ['mvn', 'mvnw'],
+            'exec_reqd': False,
+            'lock_files': [],
+            'lockfile_reqd': False,
             'accuracy': 'LOW',
             'cli_options':
                 "--detect.maven.path=PATH_TO_MAVEN\n" +
                 "    (OPTIONAL Path of the Maven executable.)\n" +
                 "--detect.maven.build.command='ARGUMENT1 ARGUMENT2'\n" +
                 "    (OPTIONAL Maven Build Command: Maven command line arguments to add to the mvn/mvnw command line.)\n" +
                 "--detect.maven.excluded.scopes='SCOPE1,SCOPE2'\n" +
@@ -283,17 +400,20 @@
                 "    (OPTIONAL Maven Modules Excluded: List of Maven modules (sub-projects) to exclude.)\n" +
                 "--detect.maven.included.modules='MODULE1,MODULE2'\n" +
                 "    (OPTIONAL Maven Modules Included: List of Maven modules (sub-projects) to include.)\n"
         },
     
     'NPM':
         {
-            'files': ['npm-shrinkwrap.json', 'package.json', 'package-lock.json'],
+            'files': ['package.json'],
             'exts': [],
             'execs': ['npm'],
+            'exec_reqd': False,
+            'lock_files': ['npm-shrinkwrap.json', 'package-lock.json'],
+            'lockfile_reqd': False,
             'accuracy': 'LOW',
             'cli_options':
                 "--detect.npm.path=PATH_TO_NPM\n" +
                 "    (OPTIONAL Path of the npm executable.)\n" +
                 "--detect.npm.arguments='ARG1 ARG2'\n" +
                 "    (OPTIONAL Additional arguments to add to the npm command line when running Detect against an NPM project.)\n" +
                 "--detect.npm.dependency.types.excluded=<NONE, DEV, PEER>\n" +
@@ -304,14 +424,17 @@
         {
             'files': [],
             'exts': ['.sln', '.csproj', '.fsproj', '.vbproj', '.asaproj', '.dcproj', '.shproj',
             '.ccproj', '.sfproj', '.njsproj', '.vcxproj', '.vcproj', '.xproj', '.pyproj',
             '.hiveproj', '.pigproj', '.jsproj', '.usqlproj', '.deployproj', '.msbuildproj',
             '.sqlproj', '.dbproj', '.rproj'],
             'execs': [],
+            'exec_reqd': False,
+            'lock_files': [],
+            'lockfile_reqd': False,
             'accuracy': 'LOW',
             'cli_options':
                 "--detect.nuget.config.path=PATH\n" + \
                 "    (OPTIONAL The path to the Nuget.Config file to supply to the nuget exe)\n" + \
                 "--detect.nuget.packages.repo.url=URL\n" + \
                 "    (OPTIONAL Nuget Packages Repository URL (default: https://api.nuget.org/v3/index.json).)\n" + \
                 "--detect.nuget.excluded.modules=PROJECT\n" + \
@@ -321,141 +444,171 @@
                 "--detect.nuget.included.modules=PROJECT\n" + \
                 "    (OPTIONAL Nuget Modules Included: The names of the projects in a solution to include (overrides exclude).)\n",
 
         },
     
     'PACKAGIST':
         {
-            'files': ['composer.lock', 'composer.json'],
+            'files': ['composer.json'],
             'exts': [],
-            'execs': ['composer'],
+            'execs': [],
+            'exec_reqd': False,
+            'lock_files': ['composer.lock'],
+            'lockfile_reqd': True,
             'accuracy': 'HIGH',
             'cli_options':
                 "--detect.packagist.include.dev.dependencies=false\n" + \
                 "    (OPTIONAL Include Packagist Development Dependencies: Set this value to false if you would like to exclude your dev requires dependencies.)\n",   
         },
     
     'PEAR':
         {
             'files': ['package.xml'],
             'exts': [],
             'execs': ['pear'],
+            'exec_reqd': True,
+            'lock_files': [],
+            'lockfile_reqd': False,
             'accuracy': 'HIGH',
             'cli_options':
                 "--detect.pear.only.required.deps=true\n" + \
                "    (OPTIONAL Include Only Required Pear Dependencies: Set to true if you would like to include only required packages.)\n",
  
         },
     
     'PIP':
         {
-            'files': ['pipfile', 'pipfile.lock', 'setup.py', 'pyproject.toml'],
+            'files': ['Pipfile','Pipfile.lock'],
             'exts': [],
-            'execs': ['python', 'python3', 'pipenv', 'pip', 'pip3'],
+            'execs': ['python', 'python3'],
+            'exec_reqd': False,
+            'lock_files': ['Pipfile.lock'],
+            'lockfile_reqd': True,
             'accuracy': 'HIGH',
             'cli_options':
                 "--detect.pip.only.project.tree=true\n" + \
                 "    (OPTIONAL PIP Include Only Project Tree: By default, pipenv includes all dependencies found in the graph. Set to true to only\n" + \
                 "    include dependencies found underneath the dependency that matches the provided pip project and version name.)\n" + \
                 "--detect.pip.project.name=NAME\n" + \
                 "    (OPTIONAL PIP Project Name: The name of your PIP project, to be used if your project's name cannot be correctly inferred from its setup.py file.)\n" + \
                 "--detect.pip.project.version.name=VERSION\n" + \
                 "    (OPTIONAL PIP Project Version Name: The version of your PIP project, to be used if your project's version name\n" + \
                 "    cannot be correctly inferred from its setup.py file.)\n"
         },
     
-    'PYTHON':
+    'PIP_REQTS':
         {
-            'files': ['requirements.txt'],
+            'files': ['requirements.txt', 'setup.py'],
             'exts': [],
-            'execs': ['python', 'python3'],
+            'execs': ['pip', 'pip3'],
+            'exec_reqd': False,
+            'lock_files': [],
+            'lockfile_reqd': False,
             'accuracy': 'LOW',
             'cli_options':
-                "--detect.pip.requirements.path='PATH1,PATH2'\n" + \
-                "    (OPTIONAL PIP Requirements Path: List of paths to requirements.txt files.)\n"
+                "--detect.pip.only.project.tree=true\n" + \
+                "    (OPTIONAL PIP Include Only Project Tree: By default, pipenv includes all dependencies found in the graph. Set to true to only\n" + \
+                "    include dependencies found underneath the dependency that matches the provided pip project and version name.)\n" + \
+                "--detect.pip.project.name=NAME\n" + \
+                "    (OPTIONAL PIP Project Name: The name of your PIP project, to be used if your project's name cannot be correctly inferred from its setup.py file.)\n" + \
+                "--detect.pip.project.version.name=VERSION\n" + \
+                "    (OPTIONAL PIP Project Version Name: The version of your PIP project, to be used if your project's version name\n" + \
+                "    cannot be correctly inferred from its setup.py file.)\n"
         },
-    
+
     'PNPM':
         {
             'files': ['pnpm-lock.yaml'],
             'exts': [],
-            'execs': ['pnpm'],
+            'execs': [],
+            'exec_reqd': False,
+            'lock_files': ['pnpm-lock.yaml'],
+            'lockfile_reqd': True,
             'accuracy': 'HIGH',
         },
     
     'POETRY':
         {
-            'files': ['Poetry.lock'],
+            'files': ['pyproject.toml', 'Poetry.lock'],
             'exts': [],
-            'execs': ['pypi'],
+            'execs': [],
+            'exec_reqd': False,
+            'lock_files': ['Poetry.lock'],
+            'lockfile_reqd': True,
             'accuracy': 'HIGH',
         },
     
     'RUBYGEMS':
         {
             'files': ['Gemfile.lock'],
             'exts': [],
-            'execs': ['gem'],
+            'execs': [],
+            'exec_reqd': False,
+            'lock_files': ['Gemfile.lock'],
+            'lockfile_reqd': False,
             'accuracy': 'HIGH',
             'cli_options':
                 "--detect.ruby.include.dev.dependencies=true\n" + \
                 "    (OPTIONAL Ruby Development Dependencies: If set to true, development dependencies will be included when parsing *.gemspec files.)\n" + \
                 "--detect.ruby.include.runtime.dependencies=false\n" + \
                 "    (OPTIONAL Ruby Runtime Dependencies: If set to false, runtime dependencies will not be included when parsing *.gemspec files.)\n",
         },
     
-    'GEMSPEC':
-        {
-            'files': [],
-            'exts': ['.gemspec'],
-            'execs': ['gem'],
-            'accuracy': 'LOW',
-        },
-    
     'SBT':
         {
             'files': ['build.sbt'],
             'exts': [],
-            'execs': ['sbt'],
+            'execs': [],
+            'exec_reqd': False,
+            'lock_files': [],
+            'lockfile_reqd': False,
             'accuracy': 'HIGH',
             'cli_options':
                 "--detect.sbt.report.search.depth\n" + \
                 "    (OPTIONAL SBT Report Search Depth: Depth the sbt detector will use to search for report files (default 3))\n" + \
                 "--detect.sbt.excluded.configurations='CONFIG'\n" + \
                 "    (OPTIONAL SBT Configurations Excluded: The names of the sbt configurations to exclude.)\n" + \
                 "--detect.sbt.included.configurations='CONFIG'\n" + \
                 "    (OPTIONAL SBT Configurations Included: The names of the sbt configurations to include.)\n",
         },
     
     'SWIFT':
         {
-            'files': ['Package.swift', 'Package.resolved'],
+            'files': ['Package.swift'],
             'exts': [],
             'execs': ['swift'],
+            'exec_reqd': False,
+            'lock_files': ['Package.resolved'],
+            'lockfile_reqd': False,
             'accuracy': 'HIGH',
         },
     
     'XCODE':
         {
             'files': [],
             'exts': ['.xcworkspace', '.xcodeproj'],
-            'execs': ['xcode'],
+            'execs': [],
+            'exec_reqd': False,
+            'lock_files': ['Package.resolved'],
+            'lockfile_reqd': False,
             'accuracy': 'HIGH',
         },
     
     'YARN':
         {
-            'files': ['yarn.lock'],
+            'files': ['package.json'],
             'exts': [],
-            'execs': ['yarn'],
+            'execs': [],
+            'exec_reqd': False,
+            'lock_files': ['yarn.lock'],
+            'lockfile_reqd': True,
             'accuracy': 'HIGH',
             'cli_options':
                 "--detect.yarn.prod.only=true\n" + \
                 "    (OPTIONAL Include Yarn Production Dependencies Only: Set this to true to only scan production dependencies.)\n"
-
         },
 }
 
 cli_msgs_dict = {
     'reqd': "--blackduck.url=https://YOURSERVER\n" + \
              "--blackduck.api.token=YOURTOKEN\n", 'proj': "--detect.project.name=PROJECT_NAME\n" + \
                                                           "--detect.project.version.name=VERSION_NAME\n" + \
@@ -465,15 +618,15 @@
      'detect_linux_proxy': " (You may need to configure a proxy to download and run the Detect script as follows)\n" + \
                            " export DETECT_CURL_OPTS='--proxy http://USER:PASSWORD@PROXYHOST:PROXYPORT'\n" + \
                            " bash <(curl -s -L ${DETECT_CURL_OPTS} https://detect.synopsys.com/detect9.sh)\n" + \
                            "--blackduck.proxy.host=PROXYHOST\n" + \
                            "--blackduck.proxy.port=PROXYPORT\n" + \
                            "--blackduck.proxy.username=USERNAME\n" + \
                            "--blackduck.proxy.password=PASSWORD\n",
-     'detect_win': " powershell \"[Net.ServicePointManager]::SecurityProtocol = 'tls12'; irm https://detect.synopsys.com/detec9.ps1?$(Get-Random) | iex; detect\"\n",
+     'detect_win': " powershell \"[Net.ServicePointManager]::SecurityProtocol = 'tls12'; irm https://detect.synopsys.com/detect9.ps1?$(Get-Random) | iex; detect\"\n",
      'detect_win_proxy': " (You may need to configure a proxy to download and run the Detect script as follows)\n" + \
                          "    ${Env:blackduck.proxy.host} = PROXYHOST\n" + \
                          "    ${Env:blackduck.proxy.port} = PROXYPORT\n" + \
                          "    ${Env:blackduck.proxy.password} = PROXYUSER\n" + \
                          "    ${Env:blackduck.proxy.username} = PROXYPASSWORD\n" + \
                          "    powershell \"[Net.ServicePointManager]::SecurityProtocol = 'tls12'; irm https://detect.synopsys.com/detect9.ps1?$(Get-Random) | iex; detect\"\n",
      'detect': '',
```

### Comparing `detect_advisor-1.0.4/detect_advisor/main.py` & `detect_advisor-1.0.5/detect_advisor/main.py`

 * *Files identical despite different names*

### Comparing `detect_advisor-1.0.4/detect_advisor/messages.py` & `detect_advisor-1.0.5/detect_advisor/messages.py`

 * *Files 3% similar despite different names*

```diff
@@ -160,48 +160,48 @@
         'desc': 'No package manager files found in project at all',
         'impact': 'No dependency scan will be performed',
         'action': 'This may be expected, but ensure you are scanning the correct project location',
     },
 
     'PACKAGES3': {
         'level': 'crit',
-        'desc': 'Package manager programs ({}) missing for package files in invocation folder',
+        'desc': 'Required package manager programs ({}) missing for dependency scan in invocation folder',
         'impact': 'Scan will fail',
         'action': 'Install required package manager programs',
     },
 
     'PACKAGES4': {
         'level': 'imp',
-        'desc': 'Package manager programs ({}) missing for package files in sub-folders',
+        'desc': 'Required package manager programs ({}) missing for dependency scan in sub-folders',
         'impact': 'The scan will fail if the scan depth is modified from the default level 0',
         'action': 'Install required package manager programs',
     },
 
     'PACKAGES5': {
         'level': 'imp',
         'desc': 'Package manager files found in archives',
         'impact': 'Dependency scan not performed for projects in archives',
         'action': 'Optionally extract zip archives and rescan',
     },
 
     'PACKAGES6': {
         'level': 'crit',
-        'desc': 'Package manager programs ({}) missing for package files in invocation folder',
-        'impact': 'Scan will fail',
-        'action': 'Either install required package manager programs or consider specifying --detect.accuracy.required=NONE (reduced accuracy scan)',
+        'desc': 'Missing lockfiles/PMs for package manager files in invocation folder',
+        'impact': 'Dependency scan will fail unless lockfiles created, PMs installed or --detect.accuracy.required=NONE specified',
+        'action': 'Either install required package manager programs, create lockfiles or specify --detect.accuracy.required=NONE (reduced accuracy scan)',
         'cli': 'reqd',
         'cli_search': 'detect.accuracy.required',
-        'cli_text': '--detect.accuracy.required=NONE (OR specify --detect.XXXX.path=<LOCATION> where XXX is package manager OR install package managers)',
+        'cli_text': '--detect.accuracy.required=NONE (OR specify --detect.XXXX.path=<LOCATION> where XXX is package manager OR install package managers OR create lockfiles)',
     },
 
     'PACKAGES7': {
         'level': 'imp',
-        'desc': 'Package manager programs ({}) missing for package files in sub-folders',
-        'impact': 'The scan will fail if the scan depth is modified from the default level 0',
-        'action': 'Either install required package manager programs or consider specifying --detect.accuracy.required=NONE (reduced accuracy scan)',
+        'desc': 'Missing lockfiles/PMs will cause scan to fail for package manager files in sub-folders',
+        'impact': 'Dependency scan will fail if scan depth > 0 unless lockfiles created, PMs installed or --detect.accuracy.required=NONE specified',
+        'action': 'Either install required package manager programs, create lockfiles or specify --detect.accuracy.required=NONE (reduced accuracy scan)',
         'cli': 'reqd',
         'cli_search': 'detect.accuracy.required',
         'cli_text': '--detect.accuracy.required=NONE (OR specify --detect.XXXX.path=<LOCATION> where XXX is package manager OR install package managers)',
     },
 
     'PACKAGES8': {
         'level': 'crit',
@@ -230,14 +230,28 @@
         'impact': 'JS packages will not be identified correctly',
         'action': "Run 'npm install' prior to scanning, or consider specifying --detect.accuracy.required=NONE (reduced accuracy scan)",
         'cli': 'reqd',
         'cli_search': 'detect.accuracy.required',
         'cli_text': '--detect.accuracy.required=NONE (OR install JS packages)',
     },
 
+    'PACKAGES12': {
+        'level': 'imp',
+        'desc': 'Lockfile(s) required for dependency scan missing in invocation folder',
+        'impact': 'Dependency scans will not be run',
+        'action': "Create lockfiles and rescan",
+    },
+
+    'PACKAGES13': {
+        'level': 'imp',
+        'desc': 'Lockfile(s) required for dependency scan missing in sub-folders',
+        'impact': 'Dependency scans will not be run',
+        'action': "Create lockfiles and rescan",
+    },
+
 }
 
 
 levtexts = {
     'crit': 'CRITICAL',
     'imp': 'IMPORTANT',
     'info': 'INFO',
```

### Comparing `detect_advisor-1.0.4/detect_advisor/output.py` & `detect_advisor-1.0.5/detect_advisor/output.py`

 * *Files identical despite different names*

### Comparing `detect_advisor-1.0.4/detect_advisor/process.py` & `detect_advisor-1.0.5/detect_advisor/process.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,27 +7,32 @@
 import hashlib
 
 from . import global_values
 from . import messages
 
 
 def process_pmdata():
-    pm_allfiles = {}
-    pm_allexts = {}
+    pm_all_files = {}
+    pm_all_exts = {}
+    # pm_all_locks = {}
 
     for pm in global_values.pm_dict.keys():
         if len(global_values.pm_dict[pm]['files']) > 0:
             for ffile in global_values.pm_dict[pm]['files']:
-                pm_allfiles[ffile] = pm
+                pm_all_files[ffile] = pm
 
         if len(global_values.pm_dict[pm]['exts']) > 0:
             for fext in global_values.pm_dict[pm]['exts']:
-                pm_allexts[fext] = pm
+                pm_all_exts[fext] = pm
 
-    return pm_allfiles, pm_allexts
+        # if len(global_values.pm_dict[pm]['lock_files']) > 0:
+        #     for ffile in global_values.pm_dict[pm]['lock_files']:
+        #         pm_all_locks[ffile] = pm
+
+    return pm_all_files, pm_all_exts
 
 
 def process_nested_zip(z, zippath, zipdepth, dirdepth):
     # global global_values.max_arc_depth
     # global global_values.global_values.messages
 
     zipdepth += 1
@@ -141,16 +146,16 @@
 
     if name in pm_allfiles.keys():
         if not in_archive:
             global_values.files_dict['det'][fhash] = {
                 'path': path,
                 'depth': dirdepth,
             }
-        # else:
-        #     global_values.file_list['arcs_pm'].append(path)
+        else:
+            global_values.file_list['arcs_pm'].append(path)
         ftype = 'det'
     elif os.path.basename(name) in global_values.ext_list['lic']:
         # global_values.file_list['other'].append(path)
         ftype = 'other'
         global_values.counts['lic'][global_values.notinarc] += 1
     elif ext != "":
         if ext in pm_allexts.keys():
@@ -402,104 +407,128 @@
     pm_allfiles, pm_allexts = process_pmdata()
 
     count = 0
     det_depth1 = 0
     det_other = 0
     det_max_depth = 0
     det_min_depth = 100
-    det_in_arc = 0
 
-    pm_dict = {}
+    pm_found_dict = {}
 
     det_files_by_depth = {}
     if len(global_values.files_dict['det']) > 0:
         for dethash in global_values.files_dict['det'].keys():
             command_exists = False
             detpath = global_values.files_dict['det'][dethash]['path']
             if det_excluded(detpath):
                 continue
             depth = global_values.files_dict['det'][dethash]['depth']
-            if detpath.find("##") > 0:
-                # in archive
-                det_in_arc += 1
-            else:
-                if depth == 1:
-                    det_depth1 += 1
-                elif depth > 1:
-                    det_other += 1
-                if depth > det_max_depth:
-                    det_max_depth = depth
-                if depth < det_min_depth:
-                    det_min_depth = depth
-
-                fname = os.path.basename(detpath)
-                pm = ''
-                if fname in pm_allfiles.keys():
-                    pm = pm_allfiles[fname]
-                elif os.path.splitext(fname)[1] in pm_allexts.keys():
-                    pm = pm_allexts[os.path.splitext(fname)[1]]
-                if pm != '':
-                    if depth not in det_files_by_depth.keys():
-                        det_files_by_depth[depth] = [detpath]
-                    else:
-                        det_files_by_depth[depth].append(detpath)
-
-                    # files_rep += detpath + '\n'
-                    if pm in pm_dict.keys():
-                        pm_dict[pm]['count'] += 1
-                        if depth < pm_dict[pm]['mindepth']:
-                            pm_dict[pm]['mindepth'] = depth
-                        if depth > pm_dict[pm]['maxdepth']:
-                            pm_dict[pm]['maxdepth'] = depth
-                    else:
-                        pm_dict[pm] = {
-                            'count': 1,
-                            'mindepth': depth,
-                            'maxdepth': depth,
-                            'exes_missing': False
-                        }
-                        exes = global_values.pm_dict[pm]['execs']
-                        # missing_cmds = ""
-                        all_missing = True
-                        for exe in exes:
-                            if shutil.which(exe) is not None:
-                                all_missing = False
-                                break
-                        if all_missing:
-                            pm_dict[pm]['exes_missing'] = True
-                        global_values.detectors_list.append(pm)
+            if depth == 1:
+                det_depth1 += 1
+            elif depth > 1:
+                det_other += 1
+            if depth > det_max_depth:
+                det_max_depth = depth
+            if depth < det_min_depth:
+                det_min_depth = depth
+
+            fname = os.path.basename(detpath)
+            pm = ''
+            if fname in pm_allfiles.keys():
+                pm = pm_allfiles[fname]
+            elif os.path.splitext(fname)[1] in pm_allexts.keys():
+                pm = pm_allexts[os.path.splitext(fname)[1]]
+
+            if pm != '':
+                # files_rep += detpath + '\n'
+                if pm in pm_found_dict.keys():
+                    pm_found_dict[pm]['count'] += 1
+                    if depth < pm_found_dict[pm]['mindepth']:
+                        pm_found_dict[pm]['mindepth'] = depth
+                    if depth > pm_found_dict[pm]['maxdepth']:
+                        pm_found_dict[pm]['maxdepth'] = depth
+                else:
+                    pm_found_dict[pm] = {
+                        'count': 1,
+                        'mindepth': depth,
+                        'maxdepth': depth,
+                        'exes_missing': False,
+                        'lockfound': True,
+                    }
+                    exes = global_values.pm_dict[pm]['execs']
+                    # missing_cmds = ""
+                    all_missing = True
+                    for exe in exes:
+                        if shutil.which(exe) is not None:
+                            all_missing = False
+                            break
+                    if all_missing:
+                        pm_found_dict[pm]['exes_missing'] = True
+                    global_values.detectors_list.append(pm)
+
+                # Check for lockfiles
+                lockfile_message = ''
+                if len(global_values.pm_dict[pm]['lock_files']) > 0:
+                    dir = os.path.dirname(detpath)
+                    found = False
+                    for entry in os.listdir(dir):
+                        if os.path.isfile(entry) and entry in global_values.pm_dict[pm]['lock_files']:
+                            found = True
+
+                    if not found:
+                        pm_found_dict[pm]['lockfound'] = False
+                        lockfile_message = ' *'
+
+                if depth not in det_files_by_depth.keys():
+                    det_files_by_depth[depth] = [detpath + lockfile_message]
+                else:
+                    det_files_by_depth[depth].append(detpath + lockfile_message)
 
         global_values.full_rep += "+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++\n" + \
-                                  "\nALL PACKAGE MANAGER CONFIG FILES FOUND (sorted by depth):"
+                                  "\nALL PACKAGE MANAGER CONFIG FILES FOUND (sorted by depth - * indicates missing lockfile):"
         for depth in sorted(det_files_by_depth.keys()):
-            global_values.full_rep += f"\nDepth {depth}:\n" + '\n'.join(det_files_by_depth[depth])
+            global_values.full_rep += f"\nDEPTH {depth}:\n- " + '\n- '.join(det_files_by_depth[depth])
 
         def pm_getter(item):
             return item[1]['mindepth']
 
         global_values.rep += ("\nPACKAGE MANAGER CONFIG FILE SUMMARY:\n\n"
                               "                MinDepth  MaxDepth    Count   Info\n")
-        for item in sorted(pm_dict.items(), key=pm_getter):
+        for item in sorted(pm_found_dict.items(), key=pm_getter):
             pm = item[0]
             info = ''
-            if item[1]['exes_missing']:
+
+            # Work out the pm scenario
+            lock_missing_reqd = False
+            if not item[1]['lockfound'] and global_values.pm_dict[pm]['lockfile_reqd']:
+                # Lockfile missing and required
+                info += '- Lockfile(s) required but not found '
+                if item[1]['mindepth'] == 1:
+                    messages.message('PACKAGES12', ','.join(exes)) #To do
+                else:
+                    messages.message('PACKAGES13', ','.join(exes)) #To do
+
+            # if item[1]['exes_missing']:
+            if item[1]['exes_missing'] and global_values.pm_dict[pm]['exec_reqd']:
                 exes = global_values.pm_dict[pm]['execs']
                 # info = "Missing package manager executables '{}'".format(','.join(exes))
-                info = 'Package Manager missing'
-                if global_values.pm_dict[pm]['accuracy'] == 'LOW':
-                    info += " - (buildless scan supported but not recommended - see recommendations)"
-                    if item[1]['mindepth'] == 1:
-                        messages.message('PACKAGES6', ','.join(exes))
-                    else:
-                        messages.message('PACKAGES7', ','.join(exes))
+                info = '- Package Manager missing and required '
+                if item[1]['mindepth'] == 1:
+                    messages.message('PACKAGES3', ','.join(exes))
                 else:
-                    if item[1]['mindepth'] == 1:
-                        messages.message('PACKAGES3', ','.join(exes))
-                    else:
-                        messages.message('PACKAGES4', ','.join(exes))
+                    messages.message('PACKAGES4', ','.join(exes))
+
+                if global_values.pm_dict[pm]['accuracy'] == 'LOW':
+                    if (global_values.pm_dict[pm]['exec_reqd'] and item[1]['exes_missing'] and
+                        not item[1]['lockfound'] and global_values.pm_dict[pm]['lockfile_reqd']):
+                        info += " - LOW accuracy scan due to missing PM/lockfiles"
+                        if item[1]['mindepth'] == 1:
+                            messages.message('PACKAGES6', ','.join(exes))
+                        else:
+                            messages.message('PACKAGES7', ','.join(exes))
 
             if platform.system() != "Linux" and 'linux_only' in global_values.pm_dict[pm] and global_values.pm_dict[pm]['linux_only']:
                 if item[1]['mindepth'] == 1:
                     messages.message('PLATFORM3', pm)
                 else:
                     messages.message('PLATFORM4', pm)
 
@@ -514,30 +543,31 @@
 
             global_values.rep += \
                 "  - {:11} {:>8d}  {:>8d}    {:>5,d}   {}\n".format(
                     item[0], item[1]['mindepth'], item[1]['maxdepth'], item[1]['count'], info)
 
         global_values.rep += "  TOTAL                               {:>5,d}\n".format(len(
             global_values.files_dict['det']))
-        global_values.rep += " (PM config files in archives         {:>5,d})\n".format(det_in_arc)
+        global_values.rep += " (PM config files in archives         {:>5,d})\n".format(
+            global_values.counts['det'][global_values.inarc])
 
     if det_depth1 == 0 and det_other > 0:
         messages.message('PACKAGES1', det_min_depth, det_max_depth)
 
     if det_depth1 == 0 and det_other == 0:
         messages.message('PACKAGES2')
 
     if global_values.counts['det'][global_values.inarc] > 0:
         messages.message('PACKAGES5')
 
     for pm in global_values.detectors_list:
-        if 'cli_options' in pm_dict[pm]:
+        if 'cli_options' in pm_found_dict[pm]:
             global_values.cli_msgs_dict['dep'] += (
                     f"For {pm}:\n" + global_values.pm_dict[pm]['cli_options'] + '\n')
-        if 'cli_reqd' in pm_dict[pm]:
+        if 'cli_reqd' in pm_found_dict[pm]:
             global_values.cli_msgs_dict['crit'] += (
                     f"For {pm}:\n" + global_values.pm_dict[pm]['cli_reqd'] + '\n')
 
     print(" Done")
 
     return
```

### Comparing `detect_advisor-1.0.4/detect_advisor.egg-info/PKG-INFO` & `detect_advisor-1.0.5/detect_advisor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: detect_advisor
-Version: 1.0.4
+Version: 1.0.5
 Summary: Detect Advisor - prescan project folders to determine how to scan with Detect
 Author-email: Matthew Brady <mbrad@synopsys.com>
 Project-URL: Homepage, https://github.com/matthewb66/detect_advisor
 Project-URL: Issues, https://github.com/matthewb66/detect_advisor/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `detect_advisor-1.0.4/pyproject.toml` & `detect_advisor-1.0.5/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "detect_advisor"
-version = "1.0.4"
+version = "1.0.5"
 authors = [
   { name="Matthew Brady", email="mbrad@synopsys.com" },
 ]
 description = "Detect Advisor - prescan project folders to determine how to scan with Detect"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

