# Comparing `tmp/glang-0.2.1.tar.gz` & `tmp/glang-0.4.0.tar.gz`

## Comparing `glang-0.2.1.tar` & `glang-0.4.0.tar`

### file list

```diff
@@ -1,65 +1,74 @@
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 glang-0.2.1/.gitattributes
--rw-r--r--   0        0        0    20717 2020-02-02 00:00:00.000000 glang-0.2.1/.pylintrc
--rwxr-xr-x   0        0        0     1879 2020-02-02 00:00:00.000000 glang-0.2.1/bootstrap.sh
--rw-r--r--   0        0        0     4095 2020-02-02 00:00:00.000000 glang-0.2.1/demo.c3
--rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 glang-0.2.1/glang.spec
--rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 glang-0.2.1/.vscode/launch.json
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 glang-0.2.1/.vscode/settings.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 glang-0.2.1/src/glang/__init__.py
--rw-r--r--   0        0        0     5558 2020-02-02 00:00:00.000000 glang-0.2.1/src/glang/driver.py
--rw-r--r--   0        0        0    37368 2020-02-02 00:00:00.000000 glang-0.2.1/src/glang/graphene_parser.py
--rw-r--r--   0        0        0     8524 2020-02-02 00:00:00.000000 glang-0.2.1/src/glang/target.py
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 glang-0.2.1/src/glang/bin/parser -> ../../../dist/parser
--rw-r--r--   0        0        0     1182 2020-02-02 00:00:00.000000 glang-0.2.1/src/glang/codegen/__init__.py
--rw-r--r--   0        0        0    17743 2020-02-02 00:00:00.000000 glang-0.2.1/src/glang/codegen/builtin_callables.py
--rw-r--r--   0        0        0    20742 2020-02-02 00:00:00.000000 glang-0.2.1/src/glang/codegen/builtin_types.py
--rw-r--r--   0        0        0    29450 2020-02-02 00:00:00.000000 glang-0.2.1/src/glang/codegen/expressions.py
--rw-r--r--   0        0        0    15510 2020-02-02 00:00:00.000000 glang-0.2.1/src/glang/codegen/generatable.py
--rw-r--r--   0        0        0     8837 2020-02-02 00:00:00.000000 glang-0.2.1/src/glang/codegen/interfaces.py
--rw-r--r--   0        0        0     2553 2020-02-02 00:00:00.000000 glang-0.2.1/src/glang/codegen/strings.py
--rw-r--r--   0        0        0     6880 2020-02-02 00:00:00.000000 glang-0.2.1/src/glang/codegen/translation_unit.py
--rw-r--r--   0        0        0    10204 2020-02-02 00:00:00.000000 glang-0.2.1/src/glang/codegen/type_conversions.py
--rw-r--r--   0        0        0    49492 2020-02-02 00:00:00.000000 glang-0.2.1/src/glang/codegen/type_resolution.py
--rw-r--r--   0        0        0    14800 2020-02-02 00:00:00.000000 glang-0.2.1/src/glang/codegen/user_facing_errors.py
--rw-r--r--   0        0        0     1362 2020-02-02 00:00:00.000000 glang-0.2.1/src/glang/lib/std/algorithms.c3
--rw-r--r--   0        0        0     4047 2020-02-02 00:00:00.000000 glang-0.2.1/src/glang/lib/std/arithmetic.c3
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 glang-0.2.1/src/glang/lib/std/assert.c3
--rw-r--r--   0        0        0     1403 2020-02-02 00:00:00.000000 glang-0.2.1/src/glang/lib/std/assignments.c3
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 glang-0.2.1/src/glang/lib/std/fcntl.c3
--rw-r--r--   0        0        0     5309 2020-02-02 00:00:00.000000 glang-0.2.1/src/glang/lib/std/format.c3
--rw-r--r--   0        0        0     3599 2020-02-02 00:00:00.000000 glang-0.2.1/src/glang/lib/std/io.c3
--rw-r--r--   0        0        0     2715 2020-02-02 00:00:00.000000 glang-0.2.1/src/glang/lib/std/iterators.c3
--rw-r--r--   0        0        0    13466 2020-02-02 00:00:00.000000 glang-0.2.1/src/glang/lib/std/json.c3
--rw-r--r--   0        0        0     2392 2020-02-02 00:00:00.000000 glang-0.2.1/src/glang/lib/std/logical.c3
--rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 glang-0.2.1/src/glang/lib/std/math.c3
--rw-r--r--   0        0        0     5518 2020-02-02 00:00:00.000000 glang-0.2.1/src/glang/lib/std/memory.c3
--rw-r--r--   0        0        0     3597 2020-02-02 00:00:00.000000 glang-0.2.1/src/glang/lib/std/span.c3
--rw-r--r--   0        0        0     3182 2020-02-02 00:00:00.000000 glang-0.2.1/src/glang/lib/std/string.c3
--rw-r--r--   0        0        0     2019 2020-02-02 00:00:00.000000 glang-0.2.1/src/glang/lib/std/type_traits.c3
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 glang-0.2.1/src/glang/lib/std/unistd.c3
--rw-r--r--   0        0        0     2414 2020-02-02 00:00:00.000000 glang-0.2.1/src/glang/lib/std/util.c3
--rw-r--r--   0        0        0     4346 2020-02-02 00:00:00.000000 glang-0.2.1/src/glang/lib/std/vector.c3
--rw-r--r--   0        0        0     3019 2020-02-02 00:00:00.000000 glang-0.2.1/src/glang/lib/std/wrappers.c3
--rw-r--r--   0        0        0     3239 2020-02-02 00:00:00.000000 glang-0.2.1/src/glang/lib/std/aarch64_linux/runtime.S
--rw-r--r--   0        0        0     2295 2020-02-02 00:00:00.000000 glang-0.2.1/src/glang/lib/std/aarch64_linux/syscalls.c3
--rw-r--r--   0        0        0     1940 2020-02-02 00:00:00.000000 glang-0.2.1/src/glang/lib/std/arm_linux/runtime.S
--rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 glang-0.2.1/src/glang/lib/std/arm_linux/syscalls.c3
--rw-r--r--   0        0        0     1273 2020-02-02 00:00:00.000000 glang-0.2.1/src/glang/lib/std/sys/mman.c3
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 glang-0.2.1/src/glang/lib/std/sys/types.c3
--rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 glang-0.2.1/src/glang/lib/std/sys/uio.c3
--rw-r--r--   0        0        0     3282 2020-02-02 00:00:00.000000 glang-0.2.1/src/glang/lib/std/x86_64_linux/runtime.S
--rw-r--r--   0        0        0     2016 2020-02-02 00:00:00.000000 glang-0.2.1/src/glang/lib/std/x86_64_linux/syscalls.c3
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 glang-0.2.1/src/glang/parser/__init__.py
--rw-r--r--   0        0        0     1347 2020-02-02 00:00:00.000000 glang-0.2.1/src/glang/parser/file_info.c3
--rw-r--r--   0        0        0     5650 2020-02-02 00:00:00.000000 glang-0.2.1/src/glang/parser/lexer_parser.py
--rw-r--r--   0        0        0    56284 2020-02-02 00:00:00.000000 glang-0.2.1/src/glang/parser/parser.c3
--rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 glang-0.2.1/src/glang/parser/self_hosted_parser.py
--rw-r--r--   0        0        0    26128 2020-02-02 00:00:00.000000 glang-0.2.1/src/glang/parser/syntax_tree.c3
--rw-r--r--   0        0        0     1285 2020-02-02 00:00:00.000000 glang-0.2.1/src/glang/targets/aarch64_linux.yml
--rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 glang-0.2.1/src/glang/targets/arm_linux.yml
--rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 glang-0.2.1/src/glang/targets/x86_64_linux.yml
--rw-r--r--   0        0        0     3150 2020-02-02 00:00:00.000000 glang-0.2.1/.gitignore
--rw-r--r--   0        0        0    34523 2020-02-02 00:00:00.000000 glang-0.2.1/LICENSE
--rw-r--r--   0        0        0      887 2020-02-02 00:00:00.000000 glang-0.2.1/hatch_build.py
--rw-r--r--   0        0        0     2204 2020-02-02 00:00:00.000000 glang-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 glang-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 glang-0.4.0/.gitattributes
+-rw-r--r--   0        0        0    20717 2020-02-02 00:00:00.000000 glang-0.4.0/.pylintrc
+-rwxr-xr-x   0        0        0     2256 2020-02-02 00:00:00.000000 glang-0.4.0/bootstrap.sh
+-rw-r--r--   0        0        0     4095 2020-02-02 00:00:00.000000 glang-0.4.0/demo.c3
+-rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 glang-0.4.0/glang.spec
+-rw-r--r--   0        0        0     2397 2020-02-02 00:00:00.000000 glang-0.4.0/printers.py
+-rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 glang-0.4.0/.vscode/launch.json
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 glang-0.4.0/.vscode/settings.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 glang-0.4.0/src/glang/__init__.py
+-rw-r--r--   0        0        0     5605 2020-02-02 00:00:00.000000 glang-0.4.0/src/glang/driver.py
+-rw-r--r--   0        0        0    40944 2020-02-02 00:00:00.000000 glang-0.4.0/src/glang/graphene_parser.py
+-rw-r--r--   0        0        0     8473 2020-02-02 00:00:00.000000 glang-0.4.0/src/glang/target.py
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 glang-0.4.0/src/glang/bin/parser -> ../../../dist/parser
+-rw-r--r--   0        0        0     2559 2020-02-02 00:00:00.000000 glang-0.4.0/src/glang/codegen/__init__.py
+-rw-r--r--   0        0        0    19637 2020-02-02 00:00:00.000000 glang-0.4.0/src/glang/codegen/builtin_callables.py
+-rw-r--r--   0        0        0    29459 2020-02-02 00:00:00.000000 glang-0.4.0/src/glang/codegen/builtin_types.py
+-rw-r--r--   0        0        0     8842 2020-02-02 00:00:00.000000 glang-0.4.0/src/glang/codegen/debug.py
+-rw-r--r--   0        0        0    30879 2020-02-02 00:00:00.000000 glang-0.4.0/src/glang/codegen/expressions.py
+-rw-r--r--   0        0        0     5160 2020-02-02 00:00:00.000000 glang-0.4.0/src/glang/codegen/floats.py
+-rw-r--r--   0        0        0    19928 2020-02-02 00:00:00.000000 glang-0.4.0/src/glang/codegen/generatable.py
+-rw-r--r--   0        0        0    11599 2020-02-02 00:00:00.000000 glang-0.4.0/src/glang/codegen/interfaces.py
+-rw-r--r--   0        0        0     5443 2020-02-02 00:00:00.000000 glang-0.4.0/src/glang/codegen/mangling.py
+-rw-r--r--   0        0        0     2566 2020-02-02 00:00:00.000000 glang-0.4.0/src/glang/codegen/strings.py
+-rw-r--r--   0        0        0    10429 2020-02-02 00:00:00.000000 glang-0.4.0/src/glang/codegen/translation_unit.py
+-rw-r--r--   0        0        0    10866 2020-02-02 00:00:00.000000 glang-0.4.0/src/glang/codegen/type_conversions.py
+-rw-r--r--   0        0        0    50601 2020-02-02 00:00:00.000000 glang-0.4.0/src/glang/codegen/type_resolution.py
+-rw-r--r--   0        0        0    15902 2020-02-02 00:00:00.000000 glang-0.4.0/src/glang/codegen/user_facing_errors.py
+-rw-r--r--   0        0        0     1362 2020-02-02 00:00:00.000000 glang-0.4.0/src/glang/lib/std/algorithms.c3
+-rw-r--r--   0        0        0     4595 2020-02-02 00:00:00.000000 glang-0.4.0/src/glang/lib/std/arithmetic.c3
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 glang-0.4.0/src/glang/lib/std/assert.c3
+-rw-r--r--   0        0        0     1403 2020-02-02 00:00:00.000000 glang-0.4.0/src/glang/lib/std/assignments.c3
+-rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 glang-0.4.0/src/glang/lib/std/fcntl.c3
+-rw-r--r--   0        0        0     4978 2020-02-02 00:00:00.000000 glang-0.4.0/src/glang/lib/std/format.c3
+-rw-r--r--   0        0        0     4067 2020-02-02 00:00:00.000000 glang-0.4.0/src/glang/lib/std/io.c3
+-rw-r--r--   0        0        0     2804 2020-02-02 00:00:00.000000 glang-0.4.0/src/glang/lib/std/iterators.c3
+-rw-r--r--   0        0        0    13342 2020-02-02 00:00:00.000000 glang-0.4.0/src/glang/lib/std/json.c3
+-rw-r--r--   0        0        0     2392 2020-02-02 00:00:00.000000 glang-0.4.0/src/glang/lib/std/logical.c3
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 glang-0.4.0/src/glang/lib/std/math.c3
+-rw-r--r--   0        0        0     5518 2020-02-02 00:00:00.000000 glang-0.4.0/src/glang/lib/std/memory.c3
+-rw-r--r--   0        0        0    15388 2020-02-02 00:00:00.000000 glang-0.4.0/src/glang/lib/std/rb_tree.c3
+-rw-r--r--   0        0        0     3597 2020-02-02 00:00:00.000000 glang-0.4.0/src/glang/lib/std/span.c3
+-rw-r--r--   0        0        0     3789 2020-02-02 00:00:00.000000 glang-0.4.0/src/glang/lib/std/string.c3
+-rw-r--r--   0        0        0     2261 2020-02-02 00:00:00.000000 glang-0.4.0/src/glang/lib/std/type_traits.c3
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 glang-0.4.0/src/glang/lib/std/unistd.c3
+-rw-r--r--   0        0        0     2597 2020-02-02 00:00:00.000000 glang-0.4.0/src/glang/lib/std/util.c3
+-rw-r--r--   0        0        0     4027 2020-02-02 00:00:00.000000 glang-0.4.0/src/glang/lib/std/vector.c3
+-rw-r--r--   0        0        0     3599 2020-02-02 00:00:00.000000 glang-0.4.0/src/glang/lib/std/wrappers.c3
+-rw-r--r--   0        0        0     3239 2020-02-02 00:00:00.000000 glang-0.4.0/src/glang/lib/std/aarch64_linux/runtime.S
+-rw-r--r--   0        0        0     2512 2020-02-02 00:00:00.000000 glang-0.4.0/src/glang/lib/std/aarch64_linux/syscalls.c3
+-rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 glang-0.4.0/src/glang/lib/std/aarch64_linux/sys/kstat.c3
+-rw-r--r--   0        0        0     1940 2020-02-02 00:00:00.000000 glang-0.4.0/src/glang/lib/std/arm_linux/runtime.S
+-rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 glang-0.4.0/src/glang/lib/std/arm_linux/syscalls.c3
+-rw-r--r--   0        0        0     1273 2020-02-02 00:00:00.000000 glang-0.4.0/src/glang/lib/std/sys/mman.c3
+-rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 glang-0.4.0/src/glang/lib/std/sys/stat.c3
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 glang-0.4.0/src/glang/lib/std/sys/types.c3
+-rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 glang-0.4.0/src/glang/lib/std/sys/uio.c3
+-rw-r--r--   0        0        0     3282 2020-02-02 00:00:00.000000 glang-0.4.0/src/glang/lib/std/x86_64_linux/runtime.S
+-rw-r--r--   0        0        0     2232 2020-02-02 00:00:00.000000 glang-0.4.0/src/glang/lib/std/x86_64_linux/syscalls.c3
+-rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 glang-0.4.0/src/glang/lib/std/x86_64_linux/sys/kstat.c3
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 glang-0.4.0/src/glang/parser/__init__.py
+-rw-r--r--   0        0        0     1347 2020-02-02 00:00:00.000000 glang-0.4.0/src/glang/parser/file_info.c3
+-rw-r--r--   0        0        0     5697 2020-02-02 00:00:00.000000 glang-0.4.0/src/glang/parser/lexer_parser.py
+-rw-r--r--   0        0        0    58452 2020-02-02 00:00:00.000000 glang-0.4.0/src/glang/parser/parser.c3
+-rw-r--r--   0        0        0     1016 2020-02-02 00:00:00.000000 glang-0.4.0/src/glang/parser/self_hosted_parser.py
+-rw-r--r--   0        0        0    26857 2020-02-02 00:00:00.000000 glang-0.4.0/src/glang/parser/syntax_tree.c3
+-rw-r--r--   0        0        0     1285 2020-02-02 00:00:00.000000 glang-0.4.0/src/glang/targets/aarch64_linux.yml
+-rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 glang-0.4.0/src/glang/targets/arm_linux.yml
+-rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 glang-0.4.0/src/glang/targets/x86_64_linux.yml
+-rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 glang-0.4.0/src/glang/utils/stack.py
+-rw-r--r--   0        0        0     3150 2020-02-02 00:00:00.000000 glang-0.4.0/.gitignore
+-rw-r--r--   0        0        0    34523 2020-02-02 00:00:00.000000 glang-0.4.0/LICENSE
+-rw-r--r--   0        0        0      933 2020-02-02 00:00:00.000000 glang-0.4.0/hatch_build.py
+-rw-r--r--   0        0        0     2182 2020-02-02 00:00:00.000000 glang-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 glang-0.4.0/PKG-INFO
```

### Comparing `glang-0.2.1/.pylintrc` & `glang-0.4.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `glang-0.2.1/bootstrap.sh` & `glang-0.4.0/bootstrap.sh`

 * *Files 14% similar despite different names*

```diff
@@ -2,34 +2,35 @@
 
 set -ex
 
 function checkout() {
     # Pass commit in $1. Output directory is returned.
     rpm_dir="GrapheneLang-${1/\//-}"
     if [ -d "$rpm_dir" ]; then
-        echo "$rpm_dir"
+        realpath "$rpm_dir"
     else
         dir="$(mktemp -d)"
         git archive "$1" --worktree-attributes ":(exclude)tests/" | tar -x -C "$dir"
-        echo "$dir"
+        realpath "$dir"
     fi
 }
 
 mkdir -p ./dist
 
-dest_dir="$(pwd)"
+dest_dir=$PWD
 stage_1_dir="$(checkout bootstrap/1)"
 stage_2_dir="$(checkout bootstrap/2)"
 stage_4_dir="$(checkout bootstrap/4)"
+stage_5_dir="$(checkout bootstrap/5)"
 
 # We can't have these inside the function, as the EXIT signal seems to be raised
 # when the functions returns... It also looks like a second call to trap
 # overwrites the first one.
 # shellcheck disable=SC2064
-trap "rm -rf $stage_1_dir; rm -rf $stage_2_dir; rm -rf $stage_4_dir" EXIT INT QUIT TERM
+trap "rm -rf $stage_1_dir; rm -rf $stage_2_dir; rm -rf $stage_4_dir; rm -rf $stage_5_dir" EXIT INT QUIT TERM
 
 # Stage 1; last commit where the Lark parser can parse the native parser.
 "$stage_1_dir/glang" "$stage_1_dir/parser/parser.c3" -o "$stage_2_dir/parser/parser" --bootstrap
 
 # Stage 2; last commit before the parser output format changes
 "$stage_2_dir/glang" "$stage_2_dir/parser/parser.c3" -o "$stage_2_dir/parser/parser"
 
@@ -37,12 +38,17 @@
 # available compiler. The location of the output has also changed.
 mkdir -p "$stage_4_dir/dist"
 "$stage_2_dir/glang" "$stage_4_dir/src/glang/parser/parser.c3" -o "$stage_4_dir/dist/parser"
 
 # Stage 4; we introduce `mut` syntax, first compile a commit where the parser
 # (but not the codegen) supports it. note: from this point forward we run as a
 # python module
-/usr/bin/env -C "$stage_4_dir" python3 -m src.glang.driver ./src/glang/parser/parser.c3 -o "$dest_dir/dist/parser"
+mkdir -p "$stage_5_dir/dist"
+env -C "$stage_4_dir" python3 -m src.glang.driver ./src/glang/parser/parser.c3 -o "$stage_5_dir/dist/parser"
+
+# Stage 5; we introduce floating point literal support, compile the last parser
+# that supports this before literals become required by the standard library.
+env -C "$stage_5_dir" python3 -m src.glang.driver ./src/glang/parser/parser.c3 -o "$dest_dir/dist/parser"
 
 # Final Stage; build the native parser from the working tree. Note that we need
 # to invoke the driver as a module.
-/usr/bin/env python3 -m src.glang.driver ./src/glang/parser/parser.c3 -o ./dist/parser -O3
+PYTHONPATH="$dest_dir/src:$PYTHONPATH" python3 -m src.glang.driver ./src/glang/parser/parser.c3 -o ./dist/parser -O3
```

### Comparing `glang-0.2.1/demo.c3` & `glang-0.4.0/demo.c3`

 * *Files identical despite different names*

### Comparing `glang-0.2.1/src/glang/driver.py` & `glang-0.4.0/src/glang/driver.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,24 @@
 import subprocess
 import sys
 from argparse import Action, ArgumentParser, Namespace
 from collections.abc import Sequence
 from os import getenv
 from pathlib import Path
-from typing import Any, Optional
+from typing import Any
 
 from tap import Tap
 
-from .graphene_parser import generate_ir_from_source
-from .target import get_host_target, get_target, get_target_triple, load_target_config
+from glang.graphene_parser import generate_ir_from_source
+from glang.target import (
+    get_host_target,
+    get_target,
+    get_target_triple,
+    load_target_config,
+)
 
 
 class PrintHostTargetAction(Action):
     def __call__(
         self,
         parser: ArgumentParser,
         namespace: Namespace,
@@ -26,15 +31,15 @@
         print(get_host_target())
         parser.exit()
 
 
 class DriverArguments(Tap):
     # TODO support multiple source files.
     input: Path
-    output: Optional[Path] = None
+    output: Path | None = None
 
     compile_to_object: bool = False
     """Do not run the linker, generate a target ".o" object file instead."""
 
     include_path: list[Path] = []
     """Add the specified directories to the search path for include files."""
 
@@ -108,15 +113,17 @@
     if args.output:
         if will_emit_binary:
             binary_output = args.output
         else:
             llvm_output = args.output
 
     # Compile to ir
-    ir = generate_ir_from_source(args.input, args.include_path, args.debug_compiler)
+    ir = generate_ir_from_source(
+        args.input, args.include_path, debug_compiler=args.debug_compiler
+    )
 
     if will_emit_llvm:
         with llvm_output.open("w", encoding="utf-8") as file:
             file.write(ir)
 
     if will_emit_llvm_to_stdout:
         sys.stdout.write(ir)
```

### Comparing `glang-0.2.1/src/glang/graphene_parser.py` & `glang-0.4.0/src/glang/graphene_parser.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,44 +1,49 @@
 import sys
 import traceback
+from collections.abc import Generator, Iterable
 from dataclasses import dataclass
 from pathlib import Path
-from typing import Any, Generator, Iterable, Optional, TypeGuard
+from typing import Any, TypeGuard
 from uuid import UUID
 
-from . import codegen as cg
-from .codegen.user_facing_errors import (
+from glang import codegen as cg
+from glang.codegen.user_facing_errors import (
     BorrowWithNoAddressError,
     CircularImportException,
     ErrorWithLineInfo,
     ErrorWithLocationInfo,
     FailedLookupError,
     FileDoesNotExistException,
     FileIsAmbiguousException,
     GenericHasGenericAnnotation,
     GrapheneError,
     MissingFunctionReturn,
+    NotInLoopStatementError,
     RepeatedGenericName,
     SourceLocation,
     StructMemberRedeclaration,
     VoidVariableDeclaration,
 )
-from .parser import lexer_parser as lp
+from glang.parser import lexer_parser as lp
 
 UnresolvedGenericMapping = dict[str, cg.UnresolvedSpecializationItem]
 
 
 class ResolvedPath(str):
+    # See https://docs.astral.sh/ruff/rules/no-slots-in-str-subclass/.
+    __slots__ = ()
+
     def __new__(cls, path: Path) -> "ResolvedPath":
         return str.__new__(cls, str(path.resolve()))
 
 
 def search_include_path_for_file(
     relative_file_path: str, include_path: list[Path]
-) -> Optional[ResolvedPath]:
+) -> ResolvedPath | None:
     matching_files: set[ResolvedPath] = set()
     for path in include_path:
         file_path = path / relative_file_path
         if file_path.exists():
             matching_files.add(ResolvedPath(file_path))
 
     if len(matching_files) == 0:
@@ -73,15 +78,15 @@
 
     def parse_constant(self, node: lp.CompileTimeConstant) -> cg.CompileTimeConstant:
         return self.parse(node, cg.CompileTimeConstant)
 
     def NumericGenericIdentifier(
         self, node: lp.NumericGenericIdentifier
     ) -> cg.CompileTimeConstant:
-        if not node.value in self._generic_args:
+        if node.value not in self._generic_args:
             raise FailedLookupError("numeric generic", f"[{node.value}, ...]")
 
         result = self._generic_args[node.value]
         assert isinstance(result, cg.CompileTimeConstant)
         return result
 
     def NumericIdentifier(self, node: lp.NumericIdentifier) -> cg.CompileTimeConstant:
@@ -207,56 +212,60 @@
         )
 
 
 class FunctionSignatureParser(lp.Interpreter):
     def __init__(self, program: cg.Program) -> None:
         super().__init__()
 
-        self._current_file: Optional[str] = None
-        self._include_hierarchy: Optional[tuple[str, ...]] = None
+        self._current_file: str | None = None
+        self._current_di_file: cg.DIFile | None = None
+        self._include_hierarchy: tuple[str, ...] | None = None
 
         self._program = program
         self._function_mapping: dict[UUID, lp.GenericFunctionDefinition] = {}
 
     def parse_file(
         self,
         file_name: str,
         include_hierarchy: list[str],
         top_level_features: list[lp.TopLevelFeature],
+        di_file: cg.DIFile,
     ) -> None:
         self._current_file = file_name
+        self._current_di_file = di_file
         self._include_hierarchy = tuple(include_hierarchy)
         for feature in top_level_features:
             if isinstance(feature, lp.FunctionDefinition):
                 self.parse(feature, None)
 
         self._current_file = None
         self._include_hierarchy = None
 
     def get_functions_to_codegen(
         self,
     ) -> Generator[
         tuple[
             cg.FunctionDeclaration,
             cg.FunctionSignature,
-            Optional[lp.GenericFunctionDefinition],
+            lp.GenericFunctionDefinition | None,
         ],
         None,
         None,
     ]:
         while to_generate := self._program.symbol_table.get_next_function_to_codegen():
             declaration, signature = to_generate
 
             body = None
             if not declaration.is_foreign:
                 body = self._function_mapping[declaration.uuid]
 
             yield declaration, signature, body
 
     def GenericFunctionDefinition(self, node: lp.GenericFunctionDefinition) -> None:
+        assert self._current_di_file is not None
         assert self._current_file is not None
         assert self._include_hierarchy is not None
 
         fn_name = (
             f"__builtin_{node.name}"
             if isinstance(node, lp.ImplicitFunction)
             else node.name
@@ -268,16 +277,16 @@
             self._include_hierarchy,
         )
 
         generic_mapping: UnresolvedGenericMapping = {}
         generic_definitions: list[cg.GenericArgument] = []
 
         # One for the type and one for the actual args.
-        variadic_type_pack_name: Optional[str] = None
-        variadic_args_pack_name: Optional[str] = None
+        variadic_type_pack_name: str | None = None
+        variadic_args_pack_name: str | None = None
 
         for generic in node.generic_definitions:
             if generic.is_packed:
                 # NOTE enforced by the grammar. We might want to relax this
                 # later and allow more than one pack per function.
                 assert variadic_type_pack_name is None
                 variadic_type_pack_name = generic.name
@@ -315,19 +324,22 @@
             tuple(specialization),
             tuple(arg_names),
             variadic_args_pack_name,
             tuple(arg_types),
             variadic_type_pack_name,
             unresolved_return,
             location,
+            node.meta,
+            self._current_di_file,
         )
         self._function_mapping[fn_declaration.uuid] = node
         self._program.symbol_table.add_function(fn_declaration)
 
     def ForeignFunction(self, node: lp.ForeignFunction) -> None:
+        assert self._current_di_file is not None
         assert self._current_file is not None
         assert self._include_hierarchy is not None
 
         parser = TypeParser({})
         fn_declaration = cg.FunctionDeclaration.construct(
             node.name,
             True,
@@ -337,14 +349,16 @@
             None,
             tuple(parser.parse_type(arg[1]) for arg in node.args),
             None,
             parser.parse_type(node.return_),
             SourceLocation(
                 node.meta.start.line, self._current_file, self._include_hierarchy
             ),
+            node.meta,
+            self._current_di_file,
         )
         self._program.symbol_table.add_function(fn_declaration)
 
 
 class ImportParser(lp.Interpreter):
     def __init__(
         self,
@@ -415,15 +429,15 @@
         return self
 
     def expression(self) -> cg.TypedExpression:
         assert isinstance(self.subexpressions[-1], cg.TypedExpression)
         return self.subexpressions[-1]
 
     def type(self) -> cg.Type:
-        return self.expression().underlying_type
+        return self.expression().result_type
 
 
 def is_flattened_expression_iterable(
     exprs: Iterable[Any],
 ) -> TypeGuard[Iterable[FlattenedExpression]]:
     # https://github.com/python/mypy/issues/3497#issuecomment-1083747764
     return all(isinstance(expr, FlattenedExpression) for expr in exprs)
@@ -444,70 +458,80 @@
         self._scope = scope
         self._generic_mapping = generic_mapping
 
     def parse_expr(self, expr: lp.Expression) -> FlattenedExpression:
         return self.parse(expr, FlattenedExpression)
 
     def HexConstant(self, node: lp.HexConstant) -> FlattenedExpression:
-        const_expr = cg.ConstantExpression(cg.UIntType(), node.value)
+        const_expr = cg.ConstantExpression(cg.UIntType(), node.value, node.meta)
         return FlattenedExpression([const_expr])
 
     def GenericIdentifierConstant(
         self, node: lp.GenericIdentifierConstant
     ) -> FlattenedExpression:
         argument = cg.GenericArgument(node.value, True)
         if argument not in self._generic_mapping.mapping:
             raise FailedLookupError("numeric generic", f"[{node.value}, ...]")
 
         mapped_value = self._generic_mapping.mapping[argument]
         assert isinstance(mapped_value, int)  # TODO: user facing error
-        const_expr = cg.ConstantExpression(cg.IntType(), str(mapped_value))
+        const_expr = cg.ConstantExpression(cg.IntType(), str(mapped_value), node.meta)
+        return FlattenedExpression([const_expr])
+
+    def FloatConstant(self, node: lp.FloatConstant) -> FlattenedExpression:
+        const_expr = cg.ConstantExpression(cg.IEEEFloat(32), node.value, node.meta)
         return FlattenedExpression([const_expr])
 
     def IntConstant(self, node: lp.IntConstant) -> FlattenedExpression:
         # TODO: the parser has already decoded this, why are we undoing it?
-        const_expr = cg.ConstantExpression(cg.IntType(), str(node.value))
+        const_expr = cg.ConstantExpression(cg.IntType(), str(node.value), node.meta)
         return FlattenedExpression([const_expr])
 
     def BoolConstant(self, node: lp.BoolConstant) -> FlattenedExpression:
         # TODO: the parser has already decoded this, why are we undoing it?
         value = "true" if node.value else "false"
-        const_expr = cg.ConstantExpression(cg.BoolType(), value)
+        const_expr = cg.ConstantExpression(cg.BoolType(), value, node.meta)
         return FlattenedExpression([const_expr])
 
     def StringConstant(self, node: lp.StringConstant) -> FlattenedExpression:
-        str_static_storage = self._program.add_static_string(node.value)
-        expr = FlattenedExpression([cg.VariableReference(str_static_storage)])
+        str_static_storage = self._program.add_static_string(node.value, node.meta)
+        expr = FlattenedExpression(
+            [cg.VariableReference(str_static_storage, node.meta)]
+        )
 
         # Implicitly take reference to string literal
-        return expr.add_parent(cg.BorrowExpression(expr.expression(), False))
+        return expr.add_parent(
+            cg.BorrowExpression(expr.expression(), cg.Type.Kind.CONST_REF, node.meta)
+        )
 
     def OperatorUse(self, node: lp.OperatorUse) -> FlattenedExpression:
         lhs = self.parse_expr(node.lhs)
         rhs = self.parse_expr(node.rhs)
 
         flattened_expr = FlattenedExpression([])
         flattened_expr.subexpressions.extend(lhs.subexpressions)
         flattened_expr.subexpressions.extend(rhs.subexpressions)
 
         call_expr = self._program.lookup_call_expression(
             node.name,
             [],  # Don't specialize operators
             [lhs.expression(), rhs.expression()],
+            node.meta,
         )
         return flattened_expr.add_parent(call_expr)
 
     def UnaryOperatorUse(self, node: lp.UnaryOperatorUse) -> FlattenedExpression:
         rhs = self.parse_expr(node.rhs)
 
         flattened_expr = FlattenedExpression(rhs.subexpressions)
         call_expr = self._program.lookup_call_expression(
             node.name,
             [],  # Don't specialize operators
             [rhs.expression()],
+            node.meta,
         )
         return flattened_expr.add_parent(call_expr)
 
     def LogicalOperatorUse(self, node: lp.LogicalOperatorUse) -> FlattenedExpression:
         lhs = self.parse_expr(node.lhs)
         rhs = self.parse_expr(node.rhs)
 
@@ -516,22 +540,24 @@
         return flattened_expr.add_parent(
             cg.LogicalOperator(
                 node.name,
                 self._function.get_next_label_id(),
                 lhs.expression(),
                 rhs.subexpressions[:-1],
                 rhs.expression(),
+                node.meta,
             )
         )
 
     def _function_call_inner(
         self,
         fn_name: str,
         fn_specialization: Iterable[lp.CompileTimeConstant | lp.Type],
         fn_args: Iterable[FlattenedExpression],
+        meta: lp.Meta,
     ) -> FlattenedExpression:
         fn_call_args = []
         flattened_expr = FlattenedExpression([])
         for arg in fn_args:
             fn_call_args.append(arg.expression())
             flattened_expr.subexpressions.extend(arg.subexpressions)
 
@@ -541,22 +567,22 @@
                 item,
                 self._generic_mapping,
             )
             for item in fn_specialization
         ]
 
         call_expr = self._program.lookup_call_expression(
-            fn_name, specialization, fn_call_args
+            fn_name, specialization, fn_call_args, meta
         )
         return flattened_expr.add_parent(call_expr)
 
     @staticmethod
     def _extract_parameter_pack(
         args: list[lp.Expression],
-    ) -> tuple[list[lp.Expression], Optional[str]]:
+    ) -> tuple[list[lp.Expression], str | None]:
         if len(args) == 0:
             return args, None
 
         if isinstance(args[-1], lp.PackExpansion):
             # TODO: support smarter expansions
             expansion = args[-1]
             assert isinstance(expansion.expression, lp.VariableAccess)
@@ -569,122 +595,146 @@
     ) -> FlattenedExpression:
         normal_args, pack_name = self._extract_parameter_pack(node.args)
         unresolved_args = [self.parse_expr(arg) for arg in normal_args]
 
         if pack_name:
             variadic_vars = self._scope.search_for_generic_pack(pack_name)
             unresolved_args.extend(
-                FlattenedExpression([cg.VariableReference(var)])
+                FlattenedExpression([cg.VariableReference(var, node.meta)])
                 for var in variadic_vars
             )
 
         # TODO perhaps we shouldn't always borrow this, although this is a bit
         # tricky as we haven't done overload resolution yet (which depends on
         # whether we borrow or not). A solution would be to borrow if we can,
         # otherwise pass an unborrowed/const-reference and let overload
         # resolution figure it out, although this isn't very explicit.
         if isinstance(node, lp.UFCS_Call):
             this_arg = self.parse_expr(node.expression)
             # TODO: should there be syntax for this? It seems a bit adhoc
-            indirection_kind = this_arg.expression().underlying_indirection_kind
-            if indirection_kind == cg.Type.Kind.CONST_REF:
-                this_arg.add_parent(cg.BorrowExpression(this_arg.expression(), False))
-            elif indirection_kind == cg.Type.Kind.MUTABLE_REF:
-                this_arg.add_parent(cg.BorrowExpression(this_arg.expression(), True))
-            elif indirection_kind == cg.Type.Kind.VALUE:
-                # (&a):fn(), (&mut a):fn(), or rvalue():fn();
-                # We do not allow the 3rd option
-                pure = this_arg.expression().get_equivalent_pure_type()
-                if pure.storage_kind == cg.Type.Kind.VALUE:
-                    raise BorrowWithNoAddressError(pure.format_for_output_to_user())
-            else:
-                assert False
+            match this_arg.expression().underlying_indirection_kind:
+                case cg.Type.Kind.CONST_REF:
+                    this_arg.add_parent(
+                        cg.BorrowExpression(
+                            this_arg.expression(), cg.Type.Kind.CONST_REF, node.meta
+                        )
+                    )
+                case cg.Type.Kind.MUTABLE_REF:
+                    this_arg.add_parent(
+                        cg.BorrowExpression(
+                            this_arg.expression(),
+                            cg.Type.Kind.MUTABLE_OR_CONST_REF,
+                            node.meta,
+                        )
+                    )
+                case cg.Type.Kind.VALUE:
+                    # (&a):fn(), (&mut a):fn(), or rvalue():fn();
+                    # We do not allow the 3rd option
+                    possible = this_arg.expression().result_type_as_if_borrowed
+                    if possible.storage_kind == cg.Type.Kind.VALUE:
+                        raise BorrowWithNoAddressError(
+                            possible.format_for_output_to_user()
+                        )
+                case _:
+                    # cg.Type.Kind.MUTABLE_OR_CONST_REF shouldn't be possible.
+                    raise AssertionError
 
             unresolved_args.insert(0, this_arg)
 
         return self._function_call_inner(
-            node.name, node.specialization, unresolved_args
+            node.name, node.specialization, unresolved_args, node.meta
         )
 
     def FunctionCall(self, node: lp.FunctionCall) -> FlattenedExpression:
         return self._function_call_outer(node)
 
     def UFCS_Call(self, node: lp.FunctionCall) -> FlattenedExpression:
         return self._function_call_outer(node)
 
     def VariableAccess(self, node: lp.VariableAccess) -> FlattenedExpression:
         var = self._scope.search_for_variable(node.name)
         if var is None:
             raise FailedLookupError("variable", node.name)
 
-        return FlattenedExpression([cg.VariableReference(var)])
+        return FlattenedExpression([cg.VariableReference(var, node.meta)])
 
     def _ensure_pointer_is_available(
-        self, expr: FlattenedExpression
+        self, expr: FlattenedExpression, meta: lp.Meta
     ) -> FlattenedExpression:
         # Copy expression to stack if it is not a pointer
         if expr.expression().has_address:
             return expr
 
-        temp_var = cg.StackVariable("", expr.type(), True, True)  # FIXME
+        temp_var = cg.StackVariable(
+            "", expr.type(), True, True, meta, self._function._di_file
+        )  # FIXME
         self._scope.add_variable(temp_var)
 
-        expr.subexpressions.append(cg.VariableInitialize(temp_var, expr.expression()))
-        return expr.add_parent(cg.VariableReference(temp_var))
+        expr.subexpressions.append(
+            cg.VariableInitialize(temp_var, expr.expression(), meta)
+        )
+        return expr.add_parent(cg.VariableReference(temp_var, meta))
 
     def ArrayIndexAccess(self, node: lp.ArrayIndexAccess) -> FlattenedExpression:
         index_exprs = [self.parse_expr(item) for item in node.indexes]
-        lhs = self._ensure_pointer_is_available(self.parse_expr(node.expression))
+        lhs = self._ensure_pointer_is_available(
+            self.parse_expr(node.expression), node.meta
+        )
         lhs_expr = lhs.expression()
 
         cg_indices: list[cg.TypedExpression] = []
         for index_expr in index_exprs:
             cg_indices.append(index_expr.expression())
             lhs.subexpressions.extend(index_expr.subexpressions)
 
-        return lhs.add_parent(cg.ArrayIndexAccess(lhs_expr, cg_indices))
+        return lhs.add_parent(cg.ArrayIndexAccess(lhs_expr, cg_indices, node.meta))
 
     def StructIndexAccess(self, node: lp.StructIndexAccess) -> FlattenedExpression:
         lhs = self.parse_expr(node.expression)
-        struct_access = cg.StructMemberAccess(lhs.expression(), node.member)
+        struct_access = cg.StructMemberAccess(lhs.expression(), node.member, node.meta)
         return lhs.add_parent(struct_access)
 
     def Borrow(self, node: lp.Borrow) -> FlattenedExpression:
         lhs = self.parse_expr(node.expression)
-        # TODO: make this const-correct
-        # I've temporarily disabled this so we can parse the parser as it
-        #  transitions to using the new syntax
-        return lhs.add_parent(cg.BorrowExpression(lhs.expression(), node.is_mut))
+        return lhs.add_parent(
+            cg.BorrowExpression(
+                lhs.expression(),
+                cg.Type.Kind.MUTABLE_REF if node.is_mut else cg.Type.Kind.CONST_REF,
+                node.meta,
+            )
+        )
 
     def UnnamedInitializerList(
         self, node: lp.UnnamedInitializerList
     ) -> FlattenedExpression:
         arg_exprs: list[cg.TypedExpression] = []
         combined_flattened = FlattenedExpression([])
         for arg in node.args:
             arg_expr = self.parse_expr(arg)
             combined_flattened.subexpressions.extend(arg_expr.subexpressions)
             arg_exprs.append(arg_expr.expression())
 
-        return combined_flattened.add_parent(cg.UnnamedInitializerList(arg_exprs))
+        return combined_flattened.add_parent(
+            cg.UnnamedInitializerList(arg_exprs, node.meta)
+        )
 
     def NamedInitializerList(
         self, node: lp.NamedInitializerList
     ) -> FlattenedExpression:
         names: list[str] = []
         member_exprs: list[cg.TypedExpression] = []
         combined_flattened = FlattenedExpression([])
         for name, expression in node.args:
             names.append(name)
             expr = self.parse_expr(expression)
             combined_flattened.subexpressions.extend(expr.subexpressions)
             member_exprs.append(expr.expression())
 
         return combined_flattened.add_parent(
-            cg.NamedInitializerList(member_exprs, names)
+            cg.NamedInitializerList(member_exprs, names, node.meta)
         )
 
 
 def generate_standalone_expression(
     program: cg.Program,
     function: cg.Function,
     scope: cg.Scope,
@@ -699,24 +749,26 @@
 def generate_return_statement(
     program: cg.Program,
     function: cg.Function,
     scope: cg.Scope,
     node: lp.Return,
     generic_mapping: cg.GenericMapping,
 ) -> None:
+    return_type = function.get_signature().return_type
+
     if node.expression is None:
-        scope.add_generatable(cg.ReturnStatement(cg.VoidType()))
+        scope.add_generatable(cg.ReturnStatement(return_type, node.meta))
         return
 
     parser = ExpressionParser(program, function, scope, generic_mapping)
     flattened_expr = parser.parse_expr(node.expression)
     scope.add_generatable(flattened_expr.subexpressions)
 
     expr = cg.ReturnStatement(
-        function.get_signature().return_type, flattened_expr.expression()
+        return_type, node.meta, returned_expr=flattened_expr.expression()
     )
     scope.add_generatable(expr)
 
 
 def generate_variable_declaration(
     program: cg.Program,
     function: cg.Function,
@@ -732,46 +784,55 @@
     var_type = TypeParser.parse_and_resolve(program, node.type_, generic_mapping)
     assert isinstance(var_type, cg.Type)
     if var_type.definition.is_void:
         raise VoidVariableDeclaration(
             "variable", node.variable, var_type.format_for_output_to_user()
         )
 
-    var = cg.StackVariable(node.variable, var_type, node.is_mut, rhs is not None)
+    var = cg.StackVariable(
+        node.variable,
+        var_type,
+        node.is_mut,
+        rhs is not None,
+        node.meta,
+        function._di_file,
+    )
     scope.add_variable(var)
 
     if rhs is None:
         return
 
     scope.add_generatable(rhs.subexpressions)
-    scope.add_generatable(cg.VariableInitialize(var, rhs.expression()))
+    scope.add_generatable(cg.VariableInitialize(var, rhs.expression(), node.meta))
 
 
 def generate_if_statement(
     program: cg.Program,
     function: cg.Function,
     scope: cg.Scope,
     node: lp.If,
     generic_mapping: cg.GenericMapping,
 ) -> None:
     parser = ExpressionParser(program, function, scope, generic_mapping)
     condition_expr = parser.parse_expr(node.condition)
 
     scope.add_generatable(condition_expr.subexpressions)
 
-    if_scope = cg.Scope(function.get_next_scope_id(), scope)
+    if_scope = cg.Scope(function.get_next_scope_id(), node.meta, scope)
     generate_body(program, function, if_scope, node.if_scope, generic_mapping)
 
     # Note: this looks like a redundant scope when the else branch is empty but I've
     #       chosen to explicitly codegen it here so we can generate destructors in
     #       the else branch (eg. if it was moved in the if)
-    else_scope = cg.Scope(function.get_next_scope_id(), scope)
+    else_scope = cg.Scope(function.get_next_scope_id(), node.else_scope.meta, scope)
     generate_body(program, function, else_scope, node.else_scope, generic_mapping)
 
-    if_statement = cg.IfElseStatement(condition_expr.expression(), if_scope, else_scope)
+    if_statement = cg.IfElseStatement(
+        condition_expr.expression(), if_scope, else_scope, node.meta
+    )
     scope.add_generatable(if_statement)
 
 
 def generate_while_statement(
     program: cg.Program,
     function: cg.Function,
     scope: cg.Scope,
@@ -779,83 +840,128 @@
     generic_mapping: cg.GenericMapping,
 ) -> None:
     parser = ExpressionParser(program, function, scope, generic_mapping)
     condition_expr = parser.parse_expr(node.condition)
 
     while_scope_id = function.get_next_scope_id()
 
-    inner_scope = cg.Scope(function.get_next_scope_id(), scope)
+    inner_scope = cg.Scope(
+        function.get_next_scope_id(), node.scope.meta, scope, is_inside_loop=True
+    )
     generate_body(program, function, inner_scope, node.scope, generic_mapping)
 
     scope.add_generatable(
         cg.WhileStatement(
             while_scope_id,
             condition_expr.expression(),
             condition_expr.subexpressions,
             inner_scope,
+            node.meta,
         )
     )
 
 
 def generate_for_statement(
     program: cg.Program,
     function: cg.Function,
     scope: cg.Scope,
     node: lp.For,
     generic_mapping: cg.GenericMapping,
 ) -> None:
     # Outer scope
-    outer_scope = cg.Scope(function.get_next_scope_id(), scope)
+    outer_scope = cg.Scope(function.get_next_scope_id(), node.meta, outer_scope=scope)
 
     #    Produce the iterator
     parser = ExpressionParser(program, function, scope, generic_mapping)
     iter_expr = parser.parse_expr(node.iterator)
 
     #    Save the iterator onto the stack (for referencing)
     store_in_mutable = not iter_expr.type().storage_kind.is_reference()
     iter_variable = cg.StackVariable(
-        f"__for_iter_{outer_scope.id}", iter_expr.type(), store_in_mutable, True
+        f"__for_iter_{outer_scope.id}",
+        iter_expr.type(),
+        store_in_mutable,
+        True,
+        node.meta,
+        function._di_file,
     )
     outer_scope.add_variable(iter_variable)
     outer_scope.add_generatable(iter_expr.subexpressions)
     outer_scope.add_generatable(
-        cg.VariableInitialize(iter_variable, iter_expr.expression())
+        cg.VariableInitialize(iter_variable, iter_expr.expression(), node.meta)
+    )
+    var_ref = cg.VariableReference(iter_variable, node.meta)
+    borrowed_iter_expr = cg.BorrowExpression(
+        var_ref, cg.Type.Kind.MUTABLE_REF, node.meta
     )
-    var_ref = cg.VariableReference(iter_variable)
-    borrowed_iter_expr = cg.BorrowExpression(var_ref, True)
     outer_scope.add_generatable([var_ref, borrowed_iter_expr])
 
     # Inner scope
-    inner_scope = cg.Scope(function.get_next_scope_id(), outer_scope)
+    inner_scope = cg.Scope(
+        function.get_next_scope_id(), node.scope.meta, outer_scope, is_inside_loop=True
+    )
 
     has_next_expr = program.lookup_call_expression(
-        "__builtin_has_next", [], [borrowed_iter_expr]
+        "__builtin_has_next", [], [borrowed_iter_expr], node.scope.meta
     )
     get_next_expr = program.lookup_call_expression(
-        "__builtin_get_next", [], [borrowed_iter_expr]
+        "__builtin_get_next", [], [borrowed_iter_expr], node.scope.meta
     )
     inner_scope.add_generatable(get_next_expr)
 
     iter_result_variable = cg.StackVariable(
-        node.variable, get_next_expr.underlying_type, False, True
+        node.variable,
+        get_next_expr.result_type,
+        False,
+        True,
+        node.meta,
+        function._di_file,
     )
     inner_scope.add_variable(iter_result_variable)
     inner_scope.add_generatable(
-        cg.VariableInitialize(iter_result_variable, get_next_expr)
+        cg.VariableInitialize(iter_result_variable, get_next_expr, node.scope.meta)
     )
 
     # For loop is just syntax sugar for a while loop
     generate_body(program, function, inner_scope, node.scope, generic_mapping)
 
     outer_scope.add_generatable(
-        cg.WhileStatement(inner_scope.id, has_next_expr, [has_next_expr], inner_scope)
+        cg.WhileStatement(
+            inner_scope.id, has_next_expr, [has_next_expr], inner_scope, node.meta
+        )
     )
     scope.add_generatable(outer_scope)
 
 
+def generate_continue_statement(
+    program: cg.Program,
+    function: cg.Function,
+    scope: cg.Scope,
+    node: lp.Return,
+    generic_mapping: cg.GenericMapping,
+) -> None:
+    if not scope.is_inside_loop():
+        raise NotInLoopStatementError("continue")
+
+    scope.add_generatable(cg.ContinueStatement(node.meta))
+
+
+def generate_break_statement(
+    program: cg.Program,
+    function: cg.Function,
+    scope: cg.Scope,
+    node: lp.Return,
+    generic_mapping: cg.GenericMapping,
+) -> None:
+    if not scope.is_inside_loop():
+        raise NotInLoopStatementError("break")
+
+    scope.add_generatable(cg.BreakStatement(node.meta))
+
+
 def generate_assignment(
     program: cg.Program,
     function: cg.Function,
     scope: cg.Scope,
     node: lp.Assignment,
     generic_mapping: cg.GenericMapping,
 ) -> None:
@@ -863,46 +969,52 @@
     lhs = parser.parse_expr(node.lhs)
     rhs = parser.parse_expr(node.rhs)
 
     scope.add_generatable(lhs.subexpressions)
     scope.add_generatable(rhs.subexpressions)
 
     if node.operator == "=":
-        scope.add_generatable(cg.Assignment(lhs.expression(), rhs.expression()))
+        scope.add_generatable(
+            cg.Assignment(lhs.expression(), rhs.expression(), node.meta)
+        )
     else:
-        borrowed_lhs = cg.BorrowExpression(lhs.expression(), True)
+        borrowed_lhs = cg.BorrowExpression(
+            lhs.expression(), cg.Type.Kind.MUTABLE_REF, node.meta
+        )
         scope.add_generatable(borrowed_lhs)
         scope.add_generatable(
             program.lookup_call_expression(
-                node.operator, [], [borrowed_lhs, rhs.expression()]
+                node.operator, [], [borrowed_lhs, rhs.expression()], node.meta
             )
         )
 
 
 def generate_scope_body(
     program: cg.Program,
     function: cg.Function,
     outer_scope: cg.Scope,
     node: lp.Scope,
     generic_mapping: cg.GenericMapping,
 ) -> None:
-    inner_scope = cg.Scope(function.get_next_scope_id(), outer_scope)
+    inner_scope = cg.Scope(function.get_next_scope_id(), node.meta, outer_scope)
     generate_body(program, function, inner_scope, node, generic_mapping)
     outer_scope.add_generatable(inner_scope)
 
 
 def generate_body(
     program: cg.Program,
     function: cg.Function,
     scope: cg.Scope,
     body: lp.Scope,
     generic_mapping: cg.GenericMapping,
 ) -> None:
     generators = {
         "Assignment": generate_assignment,
+        "Break": generate_break_statement,
+        "Continue": generate_continue_statement,
         "Expression": generate_standalone_expression,
         "For": generate_for_statement,
         "If": generate_if_statement,
         "Return": generate_return_statement,
         "Scope": generate_scope_body,
         "VariableDeclaration": generate_variable_declaration,
         "While": generate_while_statement,
@@ -911,15 +1023,15 @@
     for line in body.lines:
         try:
             for candidate in type(line).mro():
                 name = candidate.__name__
                 if name in generators:
                     break
             else:
-                assert False
+                raise AssertionError
 
             generators[name](program, function, scope, line, generic_mapping)
         except GrapheneError as exc:
             # TODO: more granular error messages
             raise ErrorWithLineInfo(
                 exc.message,
                 line.meta.start.line,
@@ -927,33 +1039,45 @@
             ) from exc
 
 
 def generate_function(
     program: cg.Program,
     declaration: cg.FunctionDeclaration,
     signature: cg.FunctionSignature,
-    body: Optional[lp.GenericFunctionDefinition],
+    body: lp.GenericFunctionDefinition | None,
 ) -> None:
     try:
-        fn = cg.Function(declaration.arg_names, signature, declaration.pack_type_name)
-    except GrapheneError as e:
+        fn = cg.Function(
+            declaration.arg_names,
+            signature,
+            declaration.pack_type_name,
+            declaration.di_file,
+            program.di_compile_unit,
+            declaration.meta,
+        )
+    except GrapheneError as err:
         assert isinstance(declaration.loc, SourceLocation)
-        raise ErrorWithLineInfo(e.message, declaration.loc.line, "function declaration")
+        raise ErrorWithLineInfo(
+            err.message, declaration.loc.line, "function declaration"
+        ) from err
 
     if body is None:
         assert declaration.is_foreign
         return
 
     generate_body(program, fn, fn.top_level_scope, body.scope, declaration.mapping)
 
     # We cannot omit the "ret" instruction from LLVM IR. If the function returns
     # void, then we can add it ourselves, otherwise the user needs to fix it.
     if not fn.top_level_scope.is_return_guaranteed():
         if fn.get_signature().return_type.definition.is_void:
-            fn.top_level_scope.add_generatable(cg.ReturnStatement(cg.VoidType()))
+            # FIXME the meta here should come from the last } of the function.
+            fn.top_level_scope.add_generatable(
+                cg.ReturnStatement(cg.VoidType(), declaration.meta)
+            )
         else:
             raise MissingFunctionReturn(
                 fn.get_signature().user_facing_name,
                 body.meta.end.line,
             )
 
     program.add_function_body(fn)
@@ -962,60 +1086,64 @@
 def append_file_to_program(
     program: cg.Program,
     function_parser: FunctionSignatureParser,
     file_path: ResolvedPath,
     include_path: list[Path],
     included_from: list[ResolvedPath],
     already_processed: set[ResolvedPath],
+    di_file: cg.DIFile | None = None,
 ) -> None:
     already_processed.add(file_path)
+    if di_file is None:
+        di_file = program.add_secondary_file(Path(file_path))
 
     try:
         top_level_features = lp.run_lexer_parser(Path(file_path))
 
         ImportParser(
             program,
             function_parser,
-            include_path + [Path(file_path).parent],
-            included_from + [file_path],
+            [*include_path, Path(file_path).parent],
+            [*included_from, file_path],
             already_processed,
         ).parse_file(top_level_features)
 
         TypeDefinitionsParser(
             str(file_path), list(map(str, included_from)), program
         ).parse_file(top_level_features)
 
         function_parser.parse_file(
-            str(file_path), list(map(str, included_from)), top_level_features
+            str(file_path), list(map(str, included_from)), top_level_features, di_file
         )
         program.symbol_table.resolve_all_non_generics()
     except ErrorWithLineInfo as exc:
         raise ErrorWithLocationInfo(
             exc.message,
             SourceLocation(exc.line, str(file_path), tuple(map(str, included_from))),
             exc.context,
         ) from exc
 
 
 def generate_ir_from_source(
-    file_path: Path, include_path: list[Path], debug_compiler: bool = False
+    file_path: Path, include_path: list[Path], *, debug_compiler: bool = False
 ) -> str:
-    program = cg.Program()
+    program = cg.Program(file_path)
     try:
         # Initial pass resolves all builtin types
         program.symbol_table.resolve_all_non_generics()
 
         fn_parser = FunctionSignatureParser(program)
         append_file_to_program(
             program,
             fn_parser,
             ResolvedPath(file_path),
             include_path,
             [],
             set(),
+            program.di_files[0],
         )
 
         for declaration, signature, body in fn_parser.get_functions_to_codegen():
             try:
                 generate_function(program, declaration, signature, body)
             except ErrorWithLineInfo as exc:
                 assert isinstance(declaration.loc, SourceLocation)
@@ -1038,8 +1166,8 @@
                 print(file=sys.stderr)
 
             for file in reversed(exc.loc.include_hierarchy):
                 print(f"Included from file '{file}'", file=sys.stderr)
 
         sys.exit(1)
 
-    return "\n".join(program.generate_ir())
+    return program.generate_ir()
```

### Comparing `glang-0.2.1/src/glang/target.py` & `glang-0.4.0/src/glang/target.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import platform
 from dataclasses import dataclass
 from enum import Enum
 from pathlib import Path
 from sys import exit as sys_exit
 from sys import stderr
-from typing import Optional
 
 import yaml
 
 
 class Endianess(Enum):
     BIG = 0
     LITTLE = 1
@@ -25,27 +24,27 @@
 class ManglingStyle(Enum):
     ELF = 0
 
     @property
     def llvm_datalayout_spec(self) -> str:
         if self == self.ELF:
             return "m:e"
-        raise NotImplementedError()
+        raise NotImplementedError
 
     @property
     def private_symbol_prefix(self) -> str:
         if self == self.ELF:
             return ".L"
-        raise NotImplementedError()
+        raise NotImplementedError
 
     @classmethod
     def from_str(cls, string: str) -> "ManglingStyle":
         if string == "elf":
             return cls.ELF
-        raise NotImplementedError()
+        raise NotImplementedError
 
 
 class ABI(Enum):
     SYSTEMV_AMD64 = 0
     ARM_EABI = 1
     AAPCS64 = 2
 
@@ -79,15 +78,15 @@
         for member_size, member_align in zip(member_sizes, member_aligns, strict=True):
             # Add padding to ensure each member is aligned
             struct_size += compute_padding(struct_size, member_align)
 
             # Append member to the struct
             struct_size += member_size
 
-        # The size of any object is always a multiple of the object‘s alignment.
+        # The size of any object is always a multiple of the object's alignment.
         struct_size += compute_padding(
             struct_size, self.compute_struct_alignment(member_aligns)
         )
 
         return struct_size
 
     def compute_struct_alignment(self, member_aligns: list[int]) -> int:
@@ -109,26 +108,26 @@
             return member_align if array_size < 16 else max(member_align, 16)
 
         if self == self.AAPCS64:
             # The alignment of an array shall be the alignment of its base type.
             # https://github.com/ARM-software/abi-aa/blob/main/aapcs64/aapcs64.rst#593arrays
             return member_align
 
-        raise NotImplementedError()
+        raise NotImplementedError
 
     @classmethod
     def from_str(cls, string: str) -> "ABI":
         if string == "SystemV_AMD64":
             return cls.SYSTEMV_AMD64
         if string == "arm_eabi":
             # FIXME actually implement the ABI...
             return cls.ARM_EABI
         if string == "aapcs64":
             return cls.AAPCS64
-        raise NotImplementedError()
+        raise NotImplementedError
 
 
 @dataclass(frozen=True, slots=True)
 class Size:
     in_bytes: int
 
     @property
@@ -181,16 +180,16 @@
         self.int_type = TypeInfo(**int_type)
         self.llvm_target_triple = llvm_target_triple
         self.llvm_types = {t: TypeInfo(**d) for t, d in llvm_types.items()}
 
 
 TARGETS_DIR = Path(__file__).parent / "targets"
 
-_target: Optional[str] = None
-_target_config: Optional[TargetConfig] = None
+_target: str | None = None
+_target_config: TargetConfig | None = None
 
 
 def load_target_config(target: str) -> None:
     global _target, _target_config
 
     # Should only call this once.
     assert _target is None
@@ -246,15 +245,15 @@
         f"{type_name}:{type_info.align.in_bits}"
         for type_name, type_info in config.llvm_types.items()
         if type_name != "ptr"
     )
 
     # Native integer widths.
     specs.append(
-        "n" + str.join(":", map(lambda w: str(w.in_bits), config.arch_native_widths))
+        "n" + str.join(":", (str(w.in_bits) for w in config.arch_native_widths))
     )
 
     # Alignment of the stack.
     specs.append(f"S{config.stack_align.in_bits}")
 
     return str.join("-", specs)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `glang-0.2.1/src/glang/codegen/builtin_callables.py` & `glang-0.4.0/src/glang/codegen/builtin_callables.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,197 +1,240 @@
 from abc import abstractmethod
-from typing import Iterator
 
-from .builtin_types import (
+from glang.codegen.builtin_types import (
     BoolDefinition,
     BoolType,
     GenericIntType,
+    IEEEFloatDefinition,
     IntegerDefinition,
     IPtrType,
     SizeType,
 )
-from .expressions import ConstantExpression
-from .interfaces import SpecializationItem, Type, TypedExpression
-from .type_conversions import do_implicit_conversion
-from .user_facing_errors import OperandError
+from glang.codegen.expressions import ConstantExpression, StaticTypedExpression
+from glang.codegen.interfaces import (
+    IRContext,
+    IROutput,
+    SpecializationItem,
+    Type,
+    TypedExpression,
+)
+from glang.codegen.type_conversions import do_implicit_conversion
+from glang.codegen.user_facing_errors import OperandError
+from glang.parser.lexer_parser import Meta
+
+NUMERIC_TYPES = (IntegerDefinition, BoolDefinition, IEEEFloatDefinition)
 
 
-class BuiltinCallable(TypedExpression):
+class BuiltinCallable(StaticTypedExpression):
     @abstractmethod
     def __init__(
-        self, specialization: list[SpecializationItem], arguments: list[TypedExpression]
+        self,
+        specialization: list[SpecializationItem],
+        arguments: list[TypedExpression],
+        meta: Meta,
     ) -> None:
         pass
 
 
-class UnaryIntegerExpression(BuiltinCallable):
+class UnaryExpression(BuiltinCallable):
     IR_FORMAT_STR = ""
     USER_FACING_NAME = ""
+    EXPECTED_TYPES = ()
 
     def __init__(
-        self, specialization: list[SpecializationItem], arguments: list[TypedExpression]
+        self,
+        specialization: list[SpecializationItem],
+        arguments: list[TypedExpression],
+        meta: Meta,
     ) -> None:
         (self._arg,) = arguments
 
         assert self.IR_FORMAT_STR is not None
         assert len(specialization) == 0
 
-        definition = self._arg.underlying_type.definition
-        assert isinstance(definition, (IntegerDefinition, BoolDefinition))
+        definition = self._arg.result_type.definition
+        assert isinstance(definition, self.EXPECTED_TYPES)
 
-        self._arg_type = self._arg.underlying_type.convert_to_value_type()
-        TypedExpression.__init__(self, self._arg_type, Type.Kind.VALUE)
+        self._arg_type = self._arg.result_type.convert_to_value_type()
+        StaticTypedExpression.__init__(self, self._arg_type, Type.Kind.VALUE, meta)
 
     def __repr__(self) -> str:
         return f"{self.__class__.__name__}({self._arg})"
 
-    def generate_ir(self, reg_gen: Iterator[int]) -> list[str]:
+    def generate_ir(self, ctx: IRContext) -> IROutput:
         # https://llvm.org/docs/LangRef.html#add-instruction (and below)
         conv, extra_exprs = do_implicit_conversion(self._arg, self._arg_type)
 
-        ir_lines: list[str] = []
-        ir_lines.extend(self.expand_ir(extra_exprs, reg_gen))
+        ir_output = IROutput()
+        ir_output.extend(self.expand_ir(extra_exprs, ctx))
 
-        self.result_reg = next(reg_gen)
+        self.result_reg = next(ctx.reg_gen)
 
         op = self.IR_FORMAT_STR.format_map(
             {
                 "type": self._arg_type.ir_type,
                 "arg": conv.ir_ref_without_type_annotation,
             }
         )
 
-        ir_lines.append(f"%{self.result_reg} = {op}")
-        return ir_lines
+        dbg = self.add_di_location(ctx, ir_output)
+
+        ir_output.lines.append(f"%{self.result_reg} = {op}, {dbg}")
+        return ir_output
 
     @property
     def ir_ref_without_type_annotation(self) -> str:
         return f"%{self.result_reg}"
 
     def assert_can_read_from(self) -> None:
         pass
 
     def assert_can_write_to(self) -> None:
         raise OperandError(f"cannot assign to `{self.USER_FACING_NAME}(..., ...)`")
 
 
-class BitwiseNotExpression(UnaryIntegerExpression):
+class BitwiseNotExpression(UnaryExpression):
+    EXPECTED_TYPES = (IntegerDefinition, BoolDefinition)
     USER_FACING_NAME = "__builtin_bitwise_not"
     IR_FORMAT_STR = "xor {type} -1, {arg}"
 
 
-class UnaryMinusExpression(UnaryIntegerExpression):
+class UnaryIntegerMinusExpression(UnaryExpression):
+    EXPECTED_TYPES = IntegerDefinition
     USER_FACING_NAME = "__builtin_minus"
     IR_FORMAT_STR = "sub {type} 0, {arg}"
 
 
-class BasicIntegerExpression(BuiltinCallable):
-    SIGNED_IR = ""
-    UNSIGNED_IR = ""
-    USER_FACING_NAME = ""
+class UnaryFloatingMinusExpression(UnaryExpression):
+    EXPECTED_TYPES = IEEEFloatDefinition
+    USER_FACING_NAME = "__builtin_fminus"
+    IR_FORMAT_STR = "fneg {type} {arg}"
+
+
+class BasicNumericExpression(BuiltinCallable):
+    FLOATING_POINT_IR = None
+    SIGNED_IR = None
+    UNSIGNED_IR = None
+    USER_FACING_NAME = None
 
     @staticmethod
     @abstractmethod
     def get_result_type(arguments: list[TypedExpression]) -> Type:
         pass
 
     def __init__(
-        self, specialization: list[SpecializationItem], arguments: list[TypedExpression]
+        self,
+        specialization: list[SpecializationItem],
+        arguments: list[TypedExpression],
+        meta: Meta,
     ) -> None:
         lhs, rhs = arguments
         # This is not a user-facing function, we don't need sensible error messages
-        assert self.SIGNED_IR is not None
-        assert self.UNSIGNED_IR is not None
+        assert self.USER_FACING_NAME is not None
+
         assert len(specialization) == 0
-        lhs_definition = lhs.underlying_type.definition
-        rhs_definition = rhs.underlying_type.definition
-        assert isinstance(lhs_definition, (IntegerDefinition, BoolDefinition))
-        assert isinstance(rhs_definition, (IntegerDefinition, BoolDefinition))
-        assert lhs.underlying_type == rhs.underlying_type
+        lhs_definition = lhs.result_type.definition
+        rhs_definition = rhs.result_type.definition
+        assert isinstance(lhs_definition, NUMERIC_TYPES)
+        assert isinstance(rhs_definition, NUMERIC_TYPES)
+        assert lhs.result_type == rhs.result_type
 
-        TypedExpression.__init__(self, self.get_result_type(arguments), Type.Kind.VALUE)
+        StaticTypedExpression.__init__(
+            self, self.get_result_type(arguments), Type.Kind.VALUE, meta
+        )
 
-        self._arg_type = lhs.underlying_type.convert_to_value_type()
+        self._arg_type = lhs.result_type.convert_to_value_type()
         self._lhs = lhs
         self._rhs = rhs
 
     def __repr__(self) -> str:
         return f"{self.__class__.__name__}({self._lhs}, {self._rhs})"
 
-    def generate_ir(self, reg_gen: Iterator[int]) -> list[str]:
+    def generate_ir(self, ctx: IRContext) -> IROutput:
         # https://llvm.org/docs/LangRef.html#add-instruction (and below)
         conv_lhs, extra_exprs_lhs = do_implicit_conversion(self._lhs, self._arg_type)
         conv_rhs, extra_exprs_rhs = do_implicit_conversion(self._rhs, self._arg_type)
 
-        ir_lines: list[str] = []
-        ir_lines.extend(self.expand_ir(extra_exprs_lhs, reg_gen))
-        ir_lines.extend(self.expand_ir(extra_exprs_rhs, reg_gen))
-
-        self.result_reg = next(reg_gen)
-
-        if isinstance(self._arg_type.definition, IntegerDefinition):
+        ir_output = IROutput()
+        ir_output.extend(self.expand_ir(extra_exprs_lhs, ctx))
+        ir_output.extend(self.expand_ir(extra_exprs_rhs, ctx))
+
+        self.result_reg = ctx.next_reg()
+
+        if isinstance(self._arg_type.definition, IEEEFloatDefinition):
+            ir = self.FLOATING_POINT_IR
+        elif isinstance(self._arg_type.definition, IntegerDefinition):
             ir = (
                 self.SIGNED_IR
                 if self._arg_type.definition.is_signed
                 else self.UNSIGNED_IR
             )
         else:
             assert isinstance(self._arg_type.definition, BoolDefinition)
             ir = self.UNSIGNED_IR
 
+        assert ir is not None
+        dbg = self.add_di_location(ctx, ir_output)
+
         # eg. for addition
         # <result> = add [nuw] [nsw] <ty> <op1>, <op2>  ; yields ty:result
-        ir_lines.append(
+        ir_output.lines.append(
             f"%{self.result_reg} = {ir} {conv_lhs.ir_ref_with_type_annotation}, "
-            f"{conv_rhs.ir_ref_without_type_annotation}"
+            f"{conv_rhs.ir_ref_without_type_annotation}, {dbg}"
         )
-        return ir_lines
+
+        return ir_output
 
     @property
     def ir_ref_without_type_annotation(self) -> str:
         return f"%{self.result_reg}"
 
     def assert_can_read_from(self) -> None:
         pass
 
     def assert_can_write_to(self) -> None:
         raise OperandError(f"cannot assign to `{self.USER_FACING_NAME}(..., ...)`")
 
 
-class ArithmeticExpression(BasicIntegerExpression):
+class ArithmeticExpression(BasicNumericExpression):
     @staticmethod
     def get_result_type(arguments: list[TypedExpression]) -> Type:
-        return arguments[0].underlying_type.convert_to_value_type()
+        return arguments[0].result_type.convert_to_value_type()
 
 
 class AddExpression(ArithmeticExpression):
+    FLOATING_POINT_IR = "fadd"
     SIGNED_IR = "add nsw"
     UNSIGNED_IR = "add nuw"
     USER_FACING_NAME = "__builtin_add"
 
 
 class SubExpression(ArithmeticExpression):
+    FLOATING_POINT_IR = "fsub"
     SIGNED_IR = "sub nsw"
     UNSIGNED_IR = "sub nuw"
     USER_FACING_NAME = "__builtin_subtract"
 
 
 class MultiplyExpression(ArithmeticExpression):
+    FLOATING_POINT_IR = "fmul"
     SIGNED_IR = "mul nsw"
     UNSIGNED_IR = "mul nuw"
     USER_FACING_NAME = "__builtin_multiply"
 
 
 class DivideExpression(ArithmeticExpression):
+    FLOATING_POINT_IR = "fdiv"
     SIGNED_IR = "sdiv"
     UNSIGNED_IR = "udiv"
     USER_FACING_NAME = "__builtin_divide"
 
 
 class RemainderExpression(ArithmeticExpression):
+    FLOATING_POINT_IR = "frem"
     SIGNED_IR = "srem"
     UNSIGNED_IR = "urem"
     USER_FACING_NAME = "__builtin_remainder"
 
 
 class ShiftLeftExpression(ArithmeticExpression):
     SIGNED_IR = "shl"
@@ -221,60 +264,66 @@
 
 class BitwiseXorExpression(ArithmeticExpression):
     SIGNED_IR = "xor"
     UNSIGNED_IR = "xor"
     USER_FACING_NAME = "__builtin_bitwise_xor"
 
 
-class CompareExpression(BasicIntegerExpression):
+class CompareExpression(BasicNumericExpression):
     @staticmethod
     def get_result_type(arguments: list[TypedExpression]) -> Type:
         return BoolType()
 
 
 class IsEqualExpression(CompareExpression):
+    FLOATING_POINT_IR = "fcmp ueq"  # Ordered and equal (can we relax this?)
     SIGNED_IR = "icmp eq"
     UNSIGNED_IR = "icmp eq"
     USER_FACING_NAME = "__builtin_is_equal"
 
 
 class IsGreaterThanExpression(CompareExpression):
+    FLOATING_POINT_IR = "fcmp ugt"
     SIGNED_IR = "icmp sgt"
     UNSIGNED_IR = "icmp ugt"
     USER_FACING_NAME = "__builtin_is_greater_than"
 
 
 class IsLessThanExpression(CompareExpression):
+    FLOATING_POINT_IR = "fcmp ult"
     SIGNED_IR = "icmp slt"
     UNSIGNED_IR = "icmp ult"
     USER_FACING_NAME = "__builtin_is_less_than"
 
 
 class AlignOfExpression(BuiltinCallable):
     def __init__(
         self,
         specialization: list[SpecializationItem],
         arguments: list[TypedExpression],
+        meta: Meta,
     ) -> None:
         assert len(arguments) == 0
         assert len(specialization) == 1
         (self._argument_type,) = specialization
         assert isinstance(self._argument_type, Type)
 
         self._result = ConstantExpression(
-            SizeType(), str(self._argument_type.alignment)
+            SizeType(), str(self._argument_type.alignment), meta
         )
 
-        TypedExpression.__init__(self, self._result.underlying_type, Type.Kind.VALUE)
+        StaticTypedExpression.__init__(
+            self, self._result.underlying_type, Type.Kind.VALUE, meta
+        )
 
     def __repr__(self) -> str:
         return f"AlignOf({self._argument_type})"
 
-    def generate_ir(self, reg_gen: Iterator[int]) -> list[str]:
-        return self._result.generate_ir(reg_gen)
+    def generate_ir(self, ctx: IRContext) -> IROutput:
+        return self._result.generate_ir(ctx)
 
     @property
     def ir_ref_without_type_annotation(self) -> str:
         return self._result.ir_ref_without_type_annotation
 
     def assert_can_read_from(self) -> None:
         pass
@@ -284,29 +333,34 @@
 
 
 class SizeOfExpression(BuiltinCallable):
     def __init__(
         self,
         specialization: list[SpecializationItem],
         arguments: list[TypedExpression],
+        meta: Meta,
     ) -> None:
         assert len(arguments) == 0
         assert len(specialization) == 1
         (self._argument_type,) = specialization
         assert isinstance(self._argument_type, Type)
 
-        self._result = ConstantExpression(SizeType(), str(self._argument_type.size))
+        self._result = ConstantExpression(
+            SizeType(), str(self._argument_type.size), meta
+        )
 
-        TypedExpression.__init__(self, self._result.underlying_type, Type.Kind.VALUE)
+        StaticTypedExpression.__init__(
+            self, self._result.underlying_type, Type.Kind.VALUE, meta
+        )
 
     def __repr__(self) -> str:
         return f"SizeOf({self._argument_type})"
 
-    def generate_ir(self, reg_gen: Iterator[int]) -> list[str]:
-        return self._result.generate_ir(reg_gen)
+    def generate_ir(self, ctx: IRContext) -> IROutput:
+        return self._result.generate_ir(ctx)
 
     @property
     def ir_ref_without_type_annotation(self) -> str:
         return self._result.ir_ref_without_type_annotation
 
     def assert_can_read_from(self) -> None:
         pass
@@ -316,224 +370,256 @@
 
 
 class NarrowExpression(BuiltinCallable):
     def __init__(
         self,
         specialization: list[SpecializationItem],
         arguments: list[TypedExpression],
+        meta: Meta,
     ) -> None:
         (self._argument,) = arguments
         (return_type,) = specialization
         assert isinstance(return_type, Type)
 
-        self._arg_value_type = self._argument.underlying_type.convert_to_value_type()
+        self._arg_value_type = self._argument.result_type.convert_to_value_type()
 
         to_definition = return_type.definition
         from_definition = self._arg_value_type.definition
         assert isinstance(to_definition, IntegerDefinition)
         assert isinstance(from_definition, IntegerDefinition)
 
         assert from_definition.bits > to_definition.bits
         assert from_definition.is_signed == to_definition.is_signed
 
-        TypedExpression.__init__(self, return_type, Type.Kind.VALUE)
+        StaticTypedExpression.__init__(self, return_type, Type.Kind.VALUE, meta)
 
     def __repr__(self) -> str:
         return f"Narrow({self._argument} to {self.underlying_type})"
 
-    def generate_ir(self, reg_gen: Iterator[int]) -> list[str]:
+    def generate_ir(self, ctx: IRContext) -> IROutput:
         conv_arg, extra_exprs_arg = do_implicit_conversion(
             self._argument, self._arg_value_type
         )
-        ir_lines: list[str] = self.expand_ir(extra_exprs_arg, reg_gen)
+        ir_output = self.expand_ir(extra_exprs_arg, ctx)
+
+        dbg = self.add_di_location(ctx, ir_output)
+
+        self.result_reg = ctx.next_reg()
 
-        self.result_reg = next(reg_gen)
-        return [
-            *ir_lines,
+        ir_output.lines.append(
             f"%{self.result_reg} = trunc {conv_arg.ir_ref_with_type_annotation}"
-            f" to {self.underlying_type.ir_type}",
-        ]
+            f" to {self.underlying_type.ir_type}, {dbg}"
+        )
+
+        return ir_output
 
     @property
     def ir_ref_without_type_annotation(self) -> str:
         return f"%{self.result_reg}"
 
     def assert_can_read_from(self) -> None:
         pass
 
     def assert_can_write_to(self) -> None:
         raise OperandError("cannot assign to `__builtin_narrow<...>(...)`")
 
 
 class PtrToIntExpression(BuiltinCallable):
     def __init__(
-        self, specialization: list[SpecializationItem], arguments: list[TypedExpression]
+        self,
+        specialization: list[SpecializationItem],
+        arguments: list[TypedExpression],
+        meta: Meta,
     ) -> None:
         assert len(specialization) == 0
         assert len(arguments) == 1
 
         # We don't attempt to dereference this at all. src_expr shouldn't have
         # more than one layer of indirection.
         (self._src_expr,) = arguments
         assert self._src_expr.has_address
 
-        TypedExpression.__init__(self, IPtrType(), Type.Kind.VALUE)
+        StaticTypedExpression.__init__(self, IPtrType(), Type.Kind.VALUE, meta)
 
     def __repr__(self) -> str:
         return f"PtrToInt({self._src_expr} to {self.underlying_type})"
 
-    def generate_ir(self, reg_gen: Iterator[int]) -> list[str]:
+    def generate_ir(self, ctx: IRContext) -> IROutput:
         # Implicit conversions do not apply.
+        ir_output = IROutput()
+
+        self.result_reg = ctx.next_reg()
 
-        self.result_reg = next(reg_gen)
+        dbg = self.add_di_location(ctx, ir_output)
 
         # <result> = ptrtoint <ty> <value> to <ty2>
-        return [
+        ir_output.lines.append(
             f"%{self.result_reg} = ptrtoint {self._src_expr.ir_ref_with_type_annotation}"
-            f" to {self.underlying_type.ir_type}"
-        ]
+            f" to {self.underlying_type.ir_type}, {dbg}"
+        )
+
+        return ir_output
 
     @property
     def ir_ref_without_type_annotation(self) -> str:
         return f"%{self.result_reg}"
 
     def assert_can_read_from(self) -> None:
         pass
 
     def assert_can_write_to(self) -> None:
         raise OperandError("Cannot assign to `__builtin_ptr_to_int()`")
 
 
 class IntToPtrExpression(BuiltinCallable):
     def __init__(
-        self, specialization: list[SpecializationItem], arguments: list[TypedExpression]
+        self,
+        specialization: list[SpecializationItem],
+        arguments: list[TypedExpression],
+        meta: Meta,
     ) -> None:
         assert len(specialization) == 1
         assert len(arguments) == 1
 
         (self._ptr_type,) = specialization
         assert isinstance(self._ptr_type, Type)
         assert self._ptr_type.storage_kind.is_reference()
 
         (self._src_expr,) = arguments
-        assert isinstance(self._src_expr.underlying_type, GenericIntType)
+        assert isinstance(self._src_expr.result_type, GenericIntType)
 
-        TypedExpression.__init__(
-            self, self._ptr_type.convert_to_value_type(), self._ptr_type.storage_kind
+        StaticTypedExpression.__init__(
+            self,
+            self._ptr_type.convert_to_value_type(),
+            self._ptr_type.storage_kind,
+            meta,
         )
 
     def __repr__(self) -> str:
         return f"IntToPtr({self._src_expr} to {self.underlying_type})"
 
-    def generate_ir(self, reg_gen: Iterator[int]) -> list[str]:
+    def generate_ir(self, ctx: IRContext) -> IROutput:
         # Remove any indirect references
         conv_src_expr, extra_exprs = do_implicit_conversion(
-            self._src_expr, self._src_expr.underlying_type
+            self._src_expr, self._src_expr.result_type
         )
 
-        ir = self.expand_ir(extra_exprs, reg_gen)
+        ir = self.expand_ir(extra_exprs, ctx)
 
-        self.result_reg = next(reg_gen)
+        self.result_reg = ctx.next_reg()
+
+        dbg = self.add_di_location(ctx, ir)
 
         # <result> = inttoptr <ty> <value> to <ty2>
-        return ir + [
+        ir.lines.append(
             f"%{self.result_reg} = inttoptr {conv_src_expr.ir_ref_with_type_annotation}"
-            f" to {self.ir_type_annotation}",
-        ]
+            f" to {self.ir_type_annotation}, {dbg}"
+        )
+
+        return ir
 
     @property
     def ir_ref_without_type_annotation(self) -> str:
         return f"%{self.result_reg}"
 
     def assert_can_read_from(self) -> None:
         pass
 
     def assert_can_write_to(self) -> None:
         pass
 
 
 class BitcastExpression(BuiltinCallable):
     def __init__(
-        self, specialization: list[SpecializationItem], arguments: list[TypedExpression]
+        self,
+        specialization: list[SpecializationItem],
+        arguments: list[TypedExpression],
+        meta: Meta,
     ) -> None:
         assert len(specialization) == 1
         assert len(arguments) == 1
 
         self.result_ref = None
 
         (self._src_expr,) = arguments
         (self._target_type,) = specialization
         assert isinstance(self._target_type, Type)
 
-        src_type = self._src_expr.underlying_type
+        src_type = self._src_expr.result_type
 
         # We can bitcast from ptr->ptr or non-aggregate->non-aggregate
         #  We can also bitcast away const
         assert (
             self._target_type.storage_kind.is_reference()
             == src_type.storage_kind.is_reference()
         )
 
         # TODO: support floats, support references
         assert isinstance(self._target_type, GenericIntType)
         assert isinstance(src_type, GenericIntType)
 
         assert self._target_type.size == src_type.size
 
-        TypedExpression.__init__(
+        StaticTypedExpression.__init__(
             self,
             self._target_type.convert_to_value_type(),
             self._target_type.storage_kind,
+            meta,
         )
 
     def __repr__(self) -> str:
         return f"Bitcast({self._src_expr} to {self.underlying_type})"
 
-    def generate_ir(self, reg_gen: Iterator[int]) -> list[str]:
+    def generate_ir(self, ctx: IRContext) -> IROutput:
         # Remove any indirect references
         conv_src_expr, extra_exprs = do_implicit_conversion(
-            self._src_expr, self._src_expr.underlying_type
+            self._src_expr, self._src_expr.result_type
         )
 
-        ir = self.expand_ir(extra_exprs, reg_gen)
+        ir = self.expand_ir(extra_exprs, ctx)
 
         if self.ir_type_annotation == conv_src_expr.ir_type_annotation:
             # Type is already correct, nothing to do
             self.result_ref = conv_src_expr.ir_ref_without_type_annotation
             return ir
 
-        self.result_ref = f"%{next(reg_gen)}"
+        self.result_ref = f"%{ctx.next_reg()}"
+
+        dbg = self.add_di_location(ctx, ir)
 
         # <result> = bitcast <ty> <value> to <ty2>
-        return ir + [
+        ir.lines.append(
             f"{self.result_ref} = bitcast {conv_src_expr.ir_ref_with_type_annotation}"
-            f" to {self.ir_type_annotation}",
-        ]
+            f" to {self.ir_type_annotation}, {dbg}",
+        )
+
+        return ir
 
     @property
     def ir_ref_without_type_annotation(self) -> str:
         assert self.result_ref is not None
         return self.result_ref
 
     def assert_can_read_from(self) -> None:
         pass
 
     def assert_can_write_to(self) -> None:
         self._src_expr.assert_can_write_to()
 
 
 def get_builtin_callables() -> dict[str, type[BuiltinCallable]]:
-    def get_integer_builtin(
-        expression_class: type[BasicIntegerExpression | UnaryIntegerExpression],
+    def get_arithmetic_builtin(
+        expression_class: type[BasicNumericExpression | UnaryExpression],
     ):
+        assert expression_class.USER_FACING_NAME is not None
         return (expression_class.USER_FACING_NAME, expression_class)
 
     integer_instructions = dict(
         map(
-            get_integer_builtin,
+            get_arithmetic_builtin,
             [
                 AddExpression,
                 SubExpression,
                 MultiplyExpression,
                 DivideExpression,
                 RemainderExpression,
                 ShiftLeftExpression,
@@ -541,15 +627,16 @@
                 BitwiseAndExpression,
                 BitwiseOrExpression,
                 BitwiseXorExpression,
                 # NOTE: I haven't added the redundant compare equal/ not equal instructions here
                 IsEqualExpression,
                 IsGreaterThanExpression,
                 IsLessThanExpression,
-                UnaryMinusExpression,
+                UnaryIntegerMinusExpression,
+                UnaryFloatingMinusExpression,
                 BitwiseNotExpression,
             ],
         )
     )
 
     return {
         **integer_instructions,
```

### Comparing `glang-0.2.1/src/glang/codegen/expressions.py` & `glang-0.4.0/src/glang/codegen/expressions.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,43 +1,51 @@
 from abc import abstractmethod
-from typing import Iterator, Optional
 
-from .builtin_types import (
+from glang.codegen.builtin_types import (
+    AnonymousType,
     BoolType,
     FunctionSignature,
     HeapArrayDefinition,
     IntType,
     SizeType,
     StackArrayDefinition,
     StructDefinition,
     format_array_dims_for_ir,
 )
-from .interfaces import Generatable, Type, TypedExpression, Variable
-from .type_conversions import (
+from glang.codegen.interfaces import (
+    Generatable,
+    IRContext,
+    IROutput,
+    StaticTypedExpression,
+    Type,
+    TypedExpression,
+    Variable,
+)
+from glang.codegen.type_conversions import (
     assert_is_implicitly_convertible,
     do_implicit_conversion,
     get_implicit_conversion_cost,
 )
-from .user_facing_errors import (
+from glang.codegen.user_facing_errors import (
     ArrayIndexCount,
     BorrowWithNoAddressError,
     CannotAssignToInitializerList,
     DoubleBorrowError,
     InvalidInitializerListConversion,
-    InvalidInitializerListDeduction,
     InvalidInitializerListLength,
     MutableBorrowOfNonMutable,
     OperandError,
     TypeCheckerError,
 )
+from glang.parser.lexer_parser import Meta
 
 
-class ConstantExpression(TypedExpression):
-    def __init__(self, cst_type: Type, value: str) -> None:
-        super().__init__(cst_type, Type.Kind.VALUE)
+class ConstantExpression(StaticTypedExpression):
+    def __init__(self, cst_type: Type, value: str, meta: Meta) -> None:
+        super().__init__(cst_type, Type.Kind.VALUE, meta)
 
         self.value = cst_type.definition.graphene_literal_to_ir_constant(value)
 
     def __repr__(self) -> str:
         return f"ConstantExpression({self.underlying_type}, {self.value})"
 
     @property
@@ -49,16 +57,16 @@
         pass
 
     def assert_can_write_to(self) -> None:
         # Can never write to a constant expression (an rvalue).
         raise OperandError(f"cannot modify the constant {self.value}")
 
 
-class VariableReference(TypedExpression):
-    def __init__(self, variable: Variable) -> None:
+class VariableReference(StaticTypedExpression):
+    def __init__(self, variable: Variable, meta: Meta) -> None:
         # Calculate the constness
         # 1) If the variable refers to a reference, the storage MUST be const,
         #     the reference inherits its constness from the reference type
         if variable.type.storage_kind.is_reference():
             assert not variable.is_mutable
             indirection_kind = variable.type.storage_kind
 
@@ -68,19 +76,20 @@
                 Type.Kind.MUTABLE_REF if variable.is_mutable else Type.Kind.CONST_REF
             )
 
         # A variable with a reference type needs borrowing before it becomes a true reference
         super().__init__(
             variable.type.convert_to_value_type(),
             indirection_kind,
-            variable.type.storage_kind.is_reference(),
+            meta,
+            was_reference_type_at_any_point=variable.type.storage_kind.is_reference(),
         )
 
         self.variable = variable
-        self._ir_ref: Optional[str] = None
+        self._ir_ref: str | None = None
 
     def __repr__(self) -> str:
         return (
             f"VariableReference({self.variable.user_facing_name}: {self.variable.type})"
         )
 
     @property
@@ -90,27 +99,27 @@
 
     def assert_can_read_from(self) -> None:
         self.variable.assert_can_read_from()
 
     def assert_can_write_to(self) -> None:
         self.variable.assert_can_write_to()
 
-    def generate_ir(self, reg_gen: Iterator[int]) -> list[str]:
+    def generate_ir(self, ctx: IRContext) -> IROutput:
         self._ir_ref = self.variable.ir_ref_without_type_annotation
 
-        ir = []
+        ir = IROutput()
         if self.variable.type.storage_kind.is_reference():
-            self._ir_ref = f"%{self.dereference_double_indirection(reg_gen, ir)}"
+            self._ir_ref = f"%{self.dereference_double_indirection(ctx, ir)}"
 
         return ir
 
 
-class FunctionParameter(TypedExpression):
-    def __init__(self, expr_type: Type) -> None:
-        super().__init__(expr_type, Type.Kind.VALUE)
+class FunctionParameter(StaticTypedExpression):
+    def __init__(self, expr_type: Type, meta: Meta) -> None:
+        super().__init__(expr_type, Type.Kind.VALUE, meta)
 
     def __repr__(self) -> str:
         return f"FunctionParameter({self.underlying_type})"
 
     def set_reg(self, reg: int) -> None:
         self.result_reg = reg
 
@@ -121,60 +130,62 @@
 
     def assert_can_read_from(self) -> None:
         pass
 
     def assert_can_write_to(self) -> None:
         # We should only write to the implicit stack variable
         #   Writing directly to a parameter is a codegen error
-        assert False
+        raise AssertionError
 
 
-class FunctionCallExpression(TypedExpression):
+class FunctionCallExpression(StaticTypedExpression):
     def __init__(
-        self, signature: FunctionSignature, args: list[TypedExpression]
+        self, signature: FunctionSignature, args: list[TypedExpression], meta: Meta
     ) -> None:
         super().__init__(
             signature.return_type.convert_to_value_type(),
             signature.return_type.storage_kind,
-            signature.return_type.storage_kind.is_reference(),
+            meta,
+            was_reference_type_at_any_point=signature.return_type.storage_kind.is_reference(),
         )
 
         for arg, arg_type in zip(args, signature.arguments, strict=True):
             arg.assert_can_read_from()
             # We do check this during overload resolution, but you can never be
             # too careful.
             assert_is_implicitly_convertible(arg, arg_type, "function call")
 
         self.signature = signature
         self.args = args
 
-    def generate_ir(self, reg_gen: Iterator[int]) -> list[str]:
+    def generate_ir(self, ctx: IRContext) -> IROutput:
         # https://llvm.org/docs/LangRef.html#call-instruction
 
-        ir_lines: list[str] = []
+        ir = IROutput()
+        dbg = self.add_di_location(ctx, ir)
         conv_args: list[TypedExpression] = []
 
         for arg, arg_type in zip(self.args, self.signature.arguments, strict=True):
             conv_arg, extra_exprs = do_implicit_conversion(arg, arg_type)
 
-            ir_lines += self.expand_ir(extra_exprs, reg_gen)
+            ir.extend(self.expand_ir(extra_exprs, ctx))
             conv_args.append(conv_arg)
 
         args_ir = map(lambda arg: arg.ir_ref_with_type_annotation, conv_args)
 
-        call_expr = f"call {self.signature.ir_ref}({str.join(', ', args_ir)})"
+        call_expr = f"call {self.signature.ir_ref}({str.join(', ', args_ir)}), {dbg}"
 
         # We cannot assign `void` to a register.
         if not self.signature.return_type.definition.is_void:
-            self.result_reg = next(reg_gen)
+            self.result_reg = ctx.next_reg()
             call_expr = f"%{self.result_reg} = {call_expr}"
 
-        ir_lines.append(call_expr)
+        ir.lines.append(call_expr)
 
-        return ir_lines
+        return ir
 
     def __repr__(self) -> str:
         return f"FunctionCallExpression({self.signature})"
 
     @property
     def ir_ref_without_type_annotation(self) -> str:
         return f"%{self.result_reg}"
@@ -185,69 +196,77 @@
 
     def assert_can_write_to(self) -> None:
         # TODO: Maybe the error message could be better? Atm we have:
         #   Error: cannot assign to non-reference 'int' since it does not have an address
         pass
 
 
-class BorrowExpression(TypedExpression):
-    def __init__(self, expr: TypedExpression, is_explicitly_mutable: bool) -> None:
+class BorrowExpression(StaticTypedExpression):
+    def __init__(
+        self, expr: TypedExpression, borrow_kind: Type.Kind, meta: Meta
+    ) -> None:
         self._expr = expr
 
-        if expr.underlying_type.storage_kind.is_reference():
-            raise DoubleBorrowError(expr.underlying_type.format_for_output_to_user())
+        rhs_type = expr.result_type
+        if rhs_type.storage_kind.is_reference():
+            raise DoubleBorrowError(rhs_type.format_for_output_to_user())
 
         if not expr.underlying_indirection_kind.is_reference():
-            raise BorrowWithNoAddressError(
-                expr.underlying_type.format_for_output_to_user()
-            )
+            raise BorrowWithNoAddressError(rhs_type.format_for_output_to_user())
 
-        if expr.underlying_indirection_kind == Type.Kind.CONST_REF:
-            # TODO: should a mutable borrow of a constant value give a constant borrow?
-            if is_explicitly_mutable:
-                # TODO: is this error message sufficient?
-                raise MutableBorrowOfNonMutable(
-                    expr.get_equivalent_pure_type().format_for_output_to_user()
-                )
+        # NOTE we are kinda abusing Type.Kind here.
+        assert borrow_kind.is_reference()
 
-        self._is_mut = is_explicitly_mutable
+        if (
+            borrow_kind == Type.Kind.MUTABLE_REF
+            and not expr.underlying_indirection_kind.is_mutable_reference()
+        ):
+            # TODO: is this error message sufficient?
+            raise MutableBorrowOfNonMutable(
+                expr.result_type_as_if_borrowed.format_for_output_to_user()
+            )
+
+        self._is_mut = (
+            borrow_kind.is_mutable_reference()
+            and expr.underlying_indirection_kind.is_mutable_reference()
+        )
 
-        storage_type = Type.Kind.MUTABLE_REF if self._is_mut else Type.Kind.CONST_REF
+        storage_type = borrow_kind if self._is_mut else Type.Kind.CONST_REF
 
         # TODO: this is a bit more permissive that I'd like, but we (need)? to support
         #       indirect initialization by first assigning to a reference
         if self._is_mut:
             expr.assert_can_write_to()
 
         super().__init__(
-            expr.underlying_type.convert_to_storage_type(storage_type), Type.Kind.VALUE
+            rhs_type.convert_to_storage_type(storage_type), Type.Kind.VALUE, meta
         )
 
     def __repr__(self) -> str:
-        return f"BorrowExpression(is_mut={self._is_mut}, {repr(self._expr)})"
+        return f"BorrowExpression(is_mut={self._is_mut}, {self._expr!r})"
 
     @property
     def ir_ref_without_type_annotation(self) -> str:
         return self._expr.ir_ref_without_type_annotation
 
     def assert_can_read_from(self) -> None:
         self._expr.assert_can_read_from()
 
     def assert_can_write_to(self) -> None:
         # TODO: can this assert be reached by a user?
         assert self._is_mut
         self._expr.assert_can_write_to()
 
 
-class StructMemberAccess(TypedExpression):
-    def __init__(self, lhs: TypedExpression, member_name: str) -> None:
+class StructMemberAccess(StaticTypedExpression):
+    def __init__(self, lhs: TypedExpression, member_name: str, meta: Meta) -> None:
         self._member_name = member_name
         self._lhs = lhs
 
-        self._struct_type = lhs.underlying_type.convert_to_value_type()
+        self._struct_type = lhs.result_type.convert_to_value_type()
         underlying_definition = self._struct_type.definition
         if not isinstance(underlying_definition, StructDefinition):
             raise TypeCheckerError(
                 "struct member access",
                 self._struct_type.format_for_output_to_user(),
                 "{...}",
             )
@@ -260,64 +279,73 @@
         # 1) If the member is a reference
         #      - We take its storage type (even if the parent struct is constant)
         # 2) If the member is a value type
         #      - We take the storage type of the parent struct
         if self._member_type.storage_kind.is_reference():
             storage_kind = self._member_type.storage_kind
         else:
-            storage_kind = lhs.get_equivalent_pure_type().storage_kind
+            storage_kind = lhs.result_type_as_if_borrowed.storage_kind
 
-        super().__init__(self._member_type.convert_to_value_type(), storage_kind)
+        super().__init__(self._member_type.convert_to_value_type(), storage_kind, meta)
 
-    def generate_ir_from_known_address(self, reg_gen: Iterator[int]) -> list[str]:
+    def generate_ir_from_known_address(self, ctx: IRContext) -> IROutput:
         # https://llvm.org/docs/LangRef.html#getelementptr-instruction
 
         # In llvm structs behind a pointer are treated like an array
-        pointer_offset = ConstantExpression(IntType(), "0")
-        index = ConstantExpression(IntType(), str(self._index))
-
-        self.result_reg = next(reg_gen)
+        assert self.meta is not None
+        pointer_offset = ConstantExpression(IntType(), "0", self.meta)
+        index = ConstantExpression(IntType(), str(self._index), self.meta)
+
+        self.result_reg = ctx.next_reg()
+        ir = IROutput()
+        dbg = self.add_di_location(ctx, ir)
 
         # <result> = getelementptr inbounds <ty>, ptr <ptrval>{, [inrange] <ty> <idx>}*
-        ir = [
+        ir.lines.append(
             f"%{self.result_reg} = getelementptr inbounds {self._struct_type.ir_type},"
             f" {self._lhs.ir_ref_with_type_annotation}, "
-            f"{pointer_offset.ir_ref_with_type_annotation}, {index.ir_ref_with_type_annotation}",
-        ]
+            f"{pointer_offset.ir_ref_with_type_annotation}, {index.ir_ref_with_type_annotation},"
+            f" {dbg}"
+        )
 
         # Prevent double indirection, dereference the element pointer to get the
         # underlying reference
         if self._member_type.storage_kind.is_reference():
-            self.result_reg = self.dereference_double_indirection(reg_gen, ir)
+            self.result_reg = self.dereference_double_indirection(ctx, ir)
 
         return ir
 
-    def generate_ir_without_known_address(self, reg_gen: Iterator[int]) -> list[str]:
+    def generate_ir_without_known_address(self, ctx: IRContext) -> IROutput:
         # https://llvm.org/docs/LangRef.html#insertvalue-instruction
 
         # <result> = extractvalue <aggregate type> <val>, <idx>{, <idx>}*
-        self.result_reg = next(reg_gen)
-        return [
+        self.result_reg = ctx.next_reg()
+        ir = IROutput()
+        dbg = self.add_di_location(ctx, ir)
+
+        ir.lines.append(
             f"%{self.result_reg} = extractvalue {self._lhs.ir_ref_with_type_annotation},"
-            f" {self._index}"
-        ]
+            f" {self._index}, {dbg}"
+        )
+
+        return ir
 
-    def generate_ir(self, reg_gen: Iterator[int]) -> list[str]:
+    def generate_ir(self, ctx: IRContext) -> IROutput:
         if self._lhs.has_address:
-            return self.generate_ir_from_known_address(reg_gen)
+            return self.generate_ir_from_known_address(ctx)
         else:
-            return self.generate_ir_without_known_address(reg_gen)
+            return self.generate_ir_without_known_address(ctx)
 
     @property
     def ir_ref_without_type_annotation(self) -> str:
         return f"%{self.result_reg}"
 
     def __repr__(self) -> str:
         return (
-            f"StructMemberAccess({self.underlying_type.format_for_output_to_user()}"
+            f"StructMemberAccess({self._struct_type.format_for_output_to_user()}"
             f".{self._member_name}: {self.underlying_type})"
         )
 
     def assert_can_read_from(self) -> None:
         # TODO: can we check if the members are initialized?
         self._lhs.assert_can_read_from()
 
@@ -326,99 +354,101 @@
         if not self.has_address:
             raise OperandError("cannot modify temporary struct")
 
         self._lhs.assert_can_write_to()
         # TODO: check if the reference is const
 
 
-class ArrayIndexAccess(TypedExpression):
+class ArrayIndexAccess(StaticTypedExpression):
     def __init__(
-        self, array_ptr: TypedExpression, indices: list[TypedExpression]
+        self, array_ptr: TypedExpression, indices: list[TypedExpression], meta: Meta
     ) -> None:
         # NOTE: needs address since getelementptr must be used for runtime indexing
         assert array_ptr.has_address
 
-        self._type_of_array: Type = array_ptr.underlying_type.convert_to_value_type()
+        self._type_of_array: Type = array_ptr.result_type.convert_to_value_type()
         self._array_ptr = array_ptr
 
         array_definition = self._type_of_array.definition
-        if not isinstance(
-            array_definition, (StackArrayDefinition, HeapArrayDefinition)
-        ):
+        if not isinstance(array_definition, StackArrayDefinition | HeapArrayDefinition):
             raise TypeCheckerError(
                 "array index access",
-                array_ptr.underlying_type.format_for_output_to_user(),
+                array_ptr.format_for_output_to_user(),
                 "T[...]",
             )
 
         if isinstance(array_definition, StackArrayDefinition):
             if len(array_definition.dimensions) != len(indices):
                 raise ArrayIndexCount(
                     self._type_of_array.format_for_output_to_user(),
                     len(indices),
                     len(array_definition.dimensions),
                 )
-        else:
-            if len(indices) != 1 + len(array_definition.known_dimensions):
-                raise ArrayIndexCount(
-                    self._type_of_array.format_for_output_to_user(), len(indices), 1
-                )
+        elif len(indices) != 1 + len(array_definition.known_dimensions):
+            raise ArrayIndexCount(
+                self._type_of_array.format_for_output_to_user(), len(indices), 1
+            )
 
         self._element_type: Type = array_definition.member
         self._conversion_exprs: list[TypedExpression] = []
 
         # Now convert all the indices into integers using standard implicit rules
         self._indices: list[TypedExpression] = []
         for index in indices:
             index_expr, conversions = do_implicit_conversion(
                 index, SizeType(), "array index access"
             )
             self._indices.append(index_expr)
             self._conversion_exprs.extend(conversions)
 
-        pure_type = array_ptr.get_equivalent_pure_type()
+        result_type = array_ptr.result_type_as_if_borrowed
         super().__init__(
-            self._element_type.convert_to_value_type(), pure_type.storage_kind
+            self._element_type.convert_to_value_type(), result_type.storage_kind, meta
         )
 
-    def generate_ir(self, reg_gen: Iterator[int]) -> list[str]:
+    def generate_ir(self, ctx: IRContext) -> IROutput:
         # https://llvm.org/docs/LangRef.html#getelementptr-instruction
         array_def = self._type_of_array.definition
-        assert isinstance(array_def, (StackArrayDefinition, HeapArrayDefinition))
+        assert isinstance(array_def, StackArrayDefinition | HeapArrayDefinition)
 
-        conversion_ir = self.expand_ir(self._conversion_exprs, reg_gen)
+        ir = self.expand_ir(self._conversion_exprs, ctx)
 
         # To access a stack array, we need to dereference the pointer returend
         # by `alloca` to get the address of the first element, and then we can
         # index into it. For heap arrays, we already have its address so we can
         # index it immediately.
         if isinstance(array_def, StackArrayDefinition):
+            assert self.meta is not None
             indices_ir = [
-                ConstantExpression(SizeType(), "0").ir_ref_with_type_annotation
+                ConstantExpression(
+                    SizeType(), "0", self.meta
+                ).ir_ref_with_type_annotation
             ]
             gep_type_ir = self._type_of_array.ir_type
         else:
             indices_ir = []
             gep_type_ir = format_array_dims_for_ir(
                 array_def.known_dimensions, array_def.member
             )
 
         for index in self._indices:
             indices_ir.append(index.ir_ref_with_type_annotation)
 
+        self.result_reg = ctx.next_reg()
+        dbg = self.add_di_location(ctx, ir)
+
         # <result> = getelementptr inbounds <ty>, ptr <ptrval>{, [inrange] <ty> <idx>}*
-        self.result_reg = next(reg_gen)
-        ir = [
-            *conversion_ir,
+        ir.lines.append(
             f"%{self.result_reg} = getelementptr inbounds {gep_type_ir},"
-            f" {self._array_ptr.ir_ref_with_type_annotation}, {', '.join(indices_ir)}",
-        ]
+            f" {self._array_ptr.ir_ref_with_type_annotation}, {', '.join(indices_ir)},"
+            f" {dbg}",
+        )
 
         if self._element_type.storage_kind.is_reference():
-            self.result_reg = self.dereference_double_indirection(reg_gen, ir)
+            self.result_reg = self.dereference_double_indirection(ctx, ir)
 
         return ir
 
     @property
     def ir_ref_without_type_annotation(self) -> str:
         return f"%{self.result_reg}"
 
@@ -430,52 +460,55 @@
         # TODO: can we check if the individual members are initialized?
         self._array_ptr.assert_can_read_from()
 
     def assert_can_write_to(self) -> None:
         self._array_ptr.assert_can_write_to()
 
 
-class ArrayInitializer(TypedExpression):
-    def __init__(self, array_type: Type, element_exprs: list[TypedExpression]) -> None:
+class ArrayInitializer(StaticTypedExpression):
+    def __init__(
+        self, array_type: Type, element_exprs: list[TypedExpression], meta: Meta
+    ) -> None:
         assert array_type.storage_kind == Type.Kind.VALUE
         assert isinstance(array_type.definition, StackArrayDefinition)
         # TODO support for multidimensional arrays?
         assert len(array_type.definition.dimensions) == 1
         assert len(element_exprs) == array_type.definition.dimensions[0]
 
-        self._result_ref: Optional[str] = None
+        self._result_ref: str | None = None
         self._elements: list[TypedExpression] = []
         self._conversion_exprs: list[TypedExpression] = []
         self.implicit_conversion_cost = 0
-        self.result_ref: Optional[str] = None
+        self.result_ref: str | None = None
 
         target_type = array_type.definition.member
         for member_expr in element_exprs:
             member, extra_exprs = do_implicit_conversion(
                 member_expr, target_type, "array initialization"
             )
 
             conversion_cost = get_implicit_conversion_cost(member_expr, target_type)
             assert conversion_cost is not None
 
             self._elements.append(member)
             self._conversion_exprs.extend(extra_exprs)
             self.implicit_conversion_cost += conversion_cost
 
-        super().__init__(array_type, Type.Kind.VALUE)
+        super().__init__(array_type, Type.Kind.VALUE, meta)
 
-    def generate_ir(self, reg_gen: Iterator[int]) -> list[str]:
-        ir: list[str] = self.expand_ir(self._conversion_exprs, reg_gen)
+    def generate_ir(self, ctx: IRContext) -> IROutput:
+        ir = self.expand_ir(self._conversion_exprs, ctx)
+        dbg = self.add_di_location(ctx, ir)
 
         previous_ref = "undef"
         for index, value in enumerate(self._elements):
-            current_ref = f"%{next(reg_gen)}"
-            ir.append(
-                f"{current_ref} = insertvalue {self.underlying_type.ir_type} {previous_ref}, "
-                f"{value.ir_ref_with_type_annotation}, {index}"
+            current_ref = f"%{ctx.next_reg()}"
+            ir.lines.append(
+                f"{current_ref} = insertvalue {self.ir_type_annotation} {previous_ref}, "
+                f"{value.ir_ref_with_type_annotation}, {index}, {dbg}"
             )
 
             previous_ref = current_ref
 
         self.result_ref = previous_ref
         return ir
 
@@ -490,25 +523,27 @@
     def assert_can_read_from(self) -> None:
         pass
 
     def assert_can_write_to(self) -> None:
         raise OperandError("cannot modify temporary array")
 
 
-class StructInitializer(TypedExpression):
-    def __init__(self, struct_type: Type, member_exprs: list[TypedExpression]) -> None:
+class StructInitializer(StaticTypedExpression):
+    def __init__(
+        self, struct_type: Type, member_exprs: list[TypedExpression], meta: Meta
+    ) -> None:
         assert struct_type.storage_kind == Type.Kind.VALUE
         assert isinstance(struct_type.definition, StructDefinition)
         assert len(member_exprs) == len(struct_type.definition.members)
 
-        self._result_ref: Optional[str] = None
+        self._result_ref: str | None = None
         self._members: list[TypedExpression] = []
         self._conversion_exprs: list[TypedExpression] = []
         self.implicit_conversion_cost = 0
-        self.result_ref: Optional[str] = None
+        self.result_ref: str | None = None
 
         for (_, target_type), member_expr in zip(
             struct_type.definition.members, member_exprs, strict=True
         ):
             member, extra_exprs = do_implicit_conversion(
                 member_expr, target_type, "struct initializer"
             )
@@ -516,25 +551,26 @@
             conversion_cost = get_implicit_conversion_cost(member_expr, target_type)
             assert conversion_cost is not None
 
             self._members.append(member)
             self._conversion_exprs.extend(extra_exprs)
             self.implicit_conversion_cost += conversion_cost
 
-        super().__init__(struct_type, Type.Kind.VALUE)
+        super().__init__(struct_type, Type.Kind.VALUE, meta)
 
-    def generate_ir(self, reg_gen: Iterator[int]) -> list[str]:
-        ir: list[str] = self.expand_ir(self._conversion_exprs, reg_gen)
+    def generate_ir(self, ctx: IRContext) -> IROutput:
+        ir = self.expand_ir(self._conversion_exprs, ctx)
+        dbg = self.add_di_location(ctx, ir)
 
         previous_ref = "undef"
         for index, value in enumerate(self._members):
-            current_ref = f"%{next(reg_gen)}"
-            ir.append(
-                f"{current_ref} = insertvalue {self.underlying_type.ir_type} {previous_ref}, "
-                f"{value.ir_ref_with_type_annotation}, {index}"
+            current_ref = f"%{ctx.next_reg()}"
+            ir.lines.append(
+                f"{current_ref} = insertvalue {self.ir_type_annotation} {previous_ref}, "
+                f"{value.ir_ref_with_type_annotation}, {index}, {dbg}"
             )
 
             previous_ref = current_ref
 
         self.result_ref = previous_ref
         return ir
 
@@ -550,28 +586,25 @@
         pass
 
     def assert_can_write_to(self) -> None:
         raise OperandError("cannot modify temporary struct")
 
 
 class InitializerList(TypedExpression):
-    @abstractmethod
-    def format_for_output_to_user(self) -> str:
-        pass
-
-    def get_equivalent_pure_type(self) -> Type:
-        assert False
+    @property
+    def has_address(self) -> bool:
+        return False
 
     @property
-    def underlying_type(self) -> Type:
-        raise InvalidInitializerListDeduction(self.format_for_output_to_user())
+    def ir_type_annotation(self) -> str:
+        raise AssertionError
 
     @property
     def ir_ref_without_type_annotation(self) -> str:
-        assert False
+        raise AssertionError
 
     def assert_can_read_from(self) -> None:
         pass
 
     def assert_can_write_to(self) -> None:
         raise CannotAssignToInitializerList()
 
@@ -582,28 +615,37 @@
     def try_convert_to_type(self, other: Type) -> tuple[int, list[TypedExpression]]:
         if not isinstance(other.definition, StructDefinition):
             raise InvalidInitializerListConversion(
                 other.format_for_output_to_user(True), self.format_for_output_to_user()
             )
 
         ordered_members = self.get_ordered_members(other)
-        struct_initializer = StructInitializer(other, ordered_members)
+        assert self.meta is not None
+        struct_initializer = StructInitializer(other, ordered_members, self.meta)
         return struct_initializer.implicit_conversion_cost, [struct_initializer]
 
 
 class NamedInitializerList(InitializerList):
-    def __init__(self, members: list[TypedExpression], names: list[str]) -> None:
-        super().__init__(None, Type.Kind.VALUE)
-
+    def __init__(
+        self, members: list[TypedExpression], names: list[str], meta: Meta
+    ) -> None:
+        super().__init__(Type.Kind.VALUE, meta)
         self._members = dict(zip(names, members, strict=True))
 
+    @property
+    def result_type(self) -> Type:
+        struct_items = [
+            (name, expr.result_type) for name, expr in self._members.items()
+        ]
+        return AnonymousType(StructDefinition(struct_items))
+
     def format_for_output_to_user(self) -> str:
         members = [
-            f"{name}: {type_name.underlying_type.format_for_output_to_user()}"
-            for name, type_name in self._members.items()
+            f"{name}: {expr.format_for_output_to_user()}"
+            for name, expr in self._members.items()
         ]
         return "{" + ", ".join(members) + "}"
 
     def __repr__(self) -> str:
         return f"InitializerList({list(self._members.items())})"
 
     def get_ordered_members(self, other: Type) -> list[TypedExpression]:
@@ -623,31 +665,35 @@
                 )
             ordered_members.append(self._members[member_name])
 
         return ordered_members
 
 
 class UnnamedInitializerList(InitializerList):
-    def __init__(self, members: list[TypedExpression]) -> None:
-        super().__init__(None, Type.Kind.VALUE)
+    def __init__(self, members: list[TypedExpression], meta: Meta) -> None:
+        super().__init__(Type.Kind.VALUE, meta)
 
         self._members = members
 
-    def format_for_output_to_user(self) -> str:
-        type_names = [
-            member.underlying_type.format_for_output_to_user()
-            for member in self._members
+    @property
+    def result_type(self) -> Type:
+        struct_items = [
+            (str(index), expr.result_type) for index, expr in enumerate(self._members)
         ]
+        return AnonymousType(StructDefinition(struct_items))
+
+    def format_for_output_to_user(self) -> str:
+        type_names = [member.format_for_output_to_user() for member in self._members]
         return "{" + ", ".join(type_names) + "}"
 
     def __repr__(self) -> str:
         return f"InitializerList({self._members})"
 
     def get_ordered_members(self, other: Type) -> list[TypedExpression]:
-        assert isinstance(other.definition, (StructDefinition, StackArrayDefinition))
+        assert isinstance(other.definition, StructDefinition | StackArrayDefinition)
 
         if isinstance(other.definition, StructDefinition):
             if len(other.definition.members) != len(self._members):
                 raise InvalidInitializerListLength(
                     len(self._members), len(other.definition.members), "a struct"
                 )
         else:
@@ -664,58 +710,61 @@
 
         return self._members
 
     def try_convert_to_type(self, other: Type) -> tuple[int, list[TypedExpression]]:
         # Unnamed initializer lists can also be converted to stack arrays.
         if isinstance(other.definition, StackArrayDefinition):
             ordered_members = self.get_ordered_members(other)
-            array_initializer = ArrayInitializer(other, ordered_members)
+            assert self.meta is not None
+            array_initializer = ArrayInitializer(other, ordered_members, self.meta)
             return array_initializer.implicit_conversion_cost, [array_initializer]
 
         # If other is not a stack array, then delegate to the parent class. It
         # can handle all other cases.
         return super().try_convert_to_type(other)
 
 
-class LogicalOperator(TypedExpression):
+class LogicalOperator(StaticTypedExpression):
     def __init__(
         self,
         operator: str,
         label_id: int,
         lhs_expression: TypedExpression,
         rhs_generatables: list[Generatable],
         rhs_expression: TypedExpression,
+        meta: Meta,
     ) -> None:
-        super().__init__(BoolType(), Type.Kind.VALUE)
+        super().__init__(BoolType(), Type.Kind.VALUE, meta)
 
         assert operator in ("and", "or")
 
         # FIXME these errors are not great.
         lhs_expression.assert_can_read_from()
         assert_is_implicitly_convertible(
             lhs_expression, BoolType(), f"logical {operator}"
         )
 
         rhs_expression.assert_can_read_from()
         assert_is_implicitly_convertible(
             rhs_expression, BoolType(), f"logical {operator}"
         )
 
-        self.result_reg: Optional[int] = None
+        self.result_reg: int | None = None
 
         self.operator = operator
         self.label_id = label_id
         self.lhs_expression = lhs_expression
         self.rhs_generatables = rhs_generatables
         self.rhs_expression = rhs_expression
 
-    def generate_ir(self, reg_gen: Iterator[int]) -> list[str]:
+    def generate_ir(self, ctx: IRContext) -> IROutput:
         # https://llvm.org/docs/LangRef.html#br-instruction
         # https://llvm.org/docs/LangRef.html#phi-instruction
-        ir: list[str] = []
+        ir = IROutput()
+        dbg = self.add_di_location(ctx, ir)
 
         lhs_label = f"l{self.operator}{self.label_id}.lhs"
         rhs_start_label = f"l{self.operator}{self.label_id}.rhs_start"
         rhs_end_label = f"l{self.operator}{self.label_id}.rhs_end"
         end_label = f"l{self.operator}{self.label_id}.end"
 
         # Logical and evaluates the RHS condition only if the LHS evaluates to
@@ -724,62 +773,63 @@
         label_if_true = rhs_start_label if self.operator == "and" else end_label
         label_if_false = end_label if self.operator == "and" else rhs_start_label
 
         # Start by branching to a known label name. This would have been
         # entirely unnecessary if we knew what the current label name was, but
         # we don't!
         # br label <dest>
-        ir.append(f"br label %{lhs_label}")
+        ir.lines.append(f"br label %{lhs_label}, {dbg}")
 
         # lhs body.
-        ir.append(f"{lhs_label}:")
+        ir.lines.append(f"{lhs_label}:")
 
         # Cast lhs to bool.
         conv_lhs, extra_lhs_exprs = do_implicit_conversion(
             self.lhs_expression, BoolType()
         )
-        ir.extend(self.expand_ir(extra_lhs_exprs, reg_gen))
+        ir.extend(self.expand_ir(extra_lhs_exprs, ctx))
 
         # Jump to either rhs_label or end_label.
         # br i1 <cond>, label <iftrue>, label <iffalse>
-        ir.append(
+        ir.lines.append(
             f"br {conv_lhs.ir_ref_with_type_annotation}, "
-            f"label %{label_if_true}, label %{label_if_false}"
+            f"label %{label_if_true}, label %{label_if_false}, {dbg}"
         )
 
         # rhs body.
-        ir.append(f"{rhs_start_label}:")
-        ir.extend(self.expand_ir(self.rhs_generatables, reg_gen))
-        ir.extend(self.rhs_expression.generate_ir(reg_gen))
+        ir.lines.append(f"{rhs_start_label}:")
+        ir.extend(self.expand_ir(self.rhs_generatables, ctx))
+        ir.extend(self.rhs_expression.generate_ir(ctx))
 
         # Cast rhs to bool.
         conv_rhs, extra_rhs_exprs = do_implicit_conversion(
             self.rhs_expression, BoolType()
         )
-        ir.extend(self.expand_ir(extra_rhs_exprs, reg_gen))
+        ir.extend(self.expand_ir(extra_rhs_exprs, ctx))
 
         # The rhs may generate its own labels. Due to this, we do not know which
         #  label contains `self.rhs_expression`. Since Phi needs control flow
         #  information, we generate a label and branch directly to phi.
         # TODO: we can generate cleaner IR be recording expressions' labels
-        ir.append(f"br label %{rhs_end_label}")
-        ir.append(f"{rhs_end_label}:")
+        ir.lines.append(f"br label %{rhs_end_label}, {dbg}")
+        ir.lines.append(f"{rhs_end_label}:")
 
         # phi's block: all control flows branch into this label
-        ir.append(f"br label %{end_label}")
-        ir.append(f"{end_label}:")
+        ir.lines.append(f"br label %{end_label}, {dbg}")
+        ir.lines.append(f"{end_label}:")
 
         # The IR is in SSA form, so we need a phi node to obtain the result of
         # the operator in a single register.
-        self.result_reg = next(reg_gen)
+        self.result_reg = ctx.next_reg()
         # <result> = phi [fast-math-flags] <ty> [ <val0>, <label0> ], ...
-        ir.append(
+        ir.lines.append(
             f"{self.ir_ref_without_type_annotation} = phi {self.ir_type_annotation} "
             f"[ {conv_lhs.ir_ref_without_type_annotation}, %{lhs_label} ], "
-            f"[ {conv_rhs.ir_ref_without_type_annotation}, %{rhs_end_label} ]"
+            f"[ {conv_rhs.ir_ref_without_type_annotation}, %{rhs_end_label} ], "
+            f"{dbg}"
         )
 
         return ir
 
     def __repr__(self) -> str:
         return (
             f"LogicalOperator({self.operator}, {self.label_id}, "
@@ -792,8 +842,8 @@
         return f"%{self.result_reg}"
 
     def assert_can_read_from(self) -> None:
         pass
 
     def assert_can_write_to(self) -> None:
         # TODO user-facing error.
-        assert False
+        raise AssertionError
```

### Comparing `glang-0.2.1/src/glang/codegen/generatable.py` & `glang-0.4.0/src/glang/codegen/generatable.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,50 +1,100 @@
-from typing import Iterable, Iterator, Optional
+from __future__ import annotations
 
-from .builtin_types import BoolType, CharArrayDefinition, VoidType
-from .interfaces import Generatable, Type, TypedExpression, Variable
-from .type_conversions import assert_is_implicitly_convertible, do_implicit_conversion
-from .user_facing_errors import (
+from collections.abc import Iterable
+
+from glang.codegen.builtin_types import BoolType, CharArrayDefinition, VoidType
+from glang.codegen.debug import DIFile, DILocalVariable, DILocation, DIType
+from glang.codegen.interfaces import (
+    Generatable,
+    IRContext,
+    IROutput,
+    LoopInfo,
+    Type,
+    TypedExpression,
+    Variable,
+)
+from glang.codegen.type_conversions import (
+    assert_is_implicitly_convertible,
+    do_implicit_conversion,
+)
+from glang.codegen.user_facing_errors import (
     AssignmentToBorrowedReference,
     AssignmentToNonPointerError,
     CannotAssignToAConstant,
     FailedLookupError,
     OperandError,
     RedefinitionError,
+    TypeCheckerError,
 )
+from glang.parser.lexer_parser import Meta
 
 
 class StackVariable(Variable):
     def __init__(
-        self, name: str, var_type: Type, is_mutable: bool, initialized: bool
+        self,
+        name: str,
+        var_type: Type,
+        is_mutable: bool,
+        initialized: bool,
+        meta: Meta,
+        di_file: DIFile,
     ) -> None:
-        super().__init__(name, var_type, is_mutable)
+        super().__init__(name, var_type, is_mutable, meta, di_file)
 
         self.initialized = initialized
 
     @property
     def ir_ref_without_type_annotation(self) -> str:
         assert self.ir_reg is not None
 
         return f"%{self.ir_reg}"
 
     @property
     def ir_ref(self) -> str:
         # alloca returns a pointer.
         return f"ptr {self.ir_ref_without_type_annotation}"
 
-    def generate_ir(self, reg_gen: Iterator[int]) -> list[str]:
+    def generate_ir(self, ctx: IRContext) -> IROutput:
         assert self.ir_reg is None
-        self.ir_reg = next(reg_gen)
+        self.ir_reg = ctx.next_reg()
+        ir = IROutput()
 
         # <result> = alloca [inalloca] <type> [, <ty> <NumElements>]
         #            [, align <alignment>] [, addrspace(<num>)]
-        return [
+        ir.lines.append(
             f"%{self.ir_reg} = alloca {self.type.ir_type}, align {self.type.alignment}"
-        ]
+        )
+
+        metadata = self.type.to_di_type(ctx.metadata_gen)
+        ir.metadata.update(metadata)
+        assert isinstance(metadata[-1], DIType)
+
+        di_local_variable = DILocalVariable(
+            ctx.next_meta(),
+            self._name,
+            None,  # FIXME specify arg for function arguments.
+            ctx.scope,
+            self._di_file,
+            self._meta.start.line,
+            metadata[-1],
+        )
+        ir.metadata.add(di_local_variable)
+
+        di_location = DILocation(
+            ctx.next_meta(), self._meta.start.line, self._meta.start.column, ctx.scope
+        )
+        ir.metadata.add(di_location)
+
+        ir.lines.append(
+            f"call void @llvm.dbg.declare(metadata {self.ir_ref}, metadata !{di_local_variable.id},"
+            f" metadata !DIExpression()), !dbg !{di_location.id}"
+        )
+
+        return ir
 
     def assert_can_read_from(self) -> None:
         # Can ready any initialized variable.
         if not self.initialized:
             raise OperandError(
                 f"cannot use uninitialized variable '{self.user_facing_name}'"
             )
@@ -53,32 +103,38 @@
         # TODO: this is kinda hacky, we aught to rename this function to
         # something like: `promise_will_write_to()``
         self.initialized = True
 
 
 class StaticVariable(Variable):
     def __init__(
-        self, name: str, var_type: Type, is_mutable: bool, graphene_literal: str
+        self,
+        name: str,
+        var_type: Type,
+        is_mutable: bool,
+        graphene_literal: str,
+        meta: Meta,
+        di_file: DIFile,
     ) -> None:
         assert var_type.storage_kind == Type.Kind.VALUE
         self._graphene_literal = graphene_literal
-        super().__init__(name, var_type, is_mutable)
+        super().__init__(name, var_type, is_mutable, meta, di_file)
 
     @property
     def ir_ref_without_type_annotation(self) -> str:
         assert self.ir_reg is not None
         if isinstance(self.type.definition, CharArrayDefinition):
             return f"@.str.{self.ir_reg}"
         return f"@.{self.ir_reg}"
 
     @property
     def ir_ref(self) -> str:
         return f"{self.type.ir_type} {self.ir_ref_without_type_annotation}"
 
-    def generate_ir(self, reg_gen: Iterator[int]) -> list[str]:
+    def generate_ir(self, ctx: IRContext) -> IROutput:
         additional_prefix = "global" if self.is_mutable else "unnamed_addr constant"
 
         literal = self.type.definition.graphene_literal_to_ir_constant(
             self._graphene_literal
         )
         # @<GlobalVarName> = [Linkage] [PreemptionSpecifier] [Visibility]
         #            [DLLStorageClass] [ThreadLocal]
@@ -86,39 +142,48 @@
         #            [ExternallyInitialized]
         #            <global | constant> <Type> [<InitializerConstant>]
         #            [, section "name"] [, partition "name"]
         #            [, comdat [($name)]] [, align <Alignment>]
         #            [, no_sanitize_address] [, no_sanitize_hwaddress]
         #            [, sanitize_address_dyninit] [, sanitize_memtag]
         #            (, !name !N)*
-        self.ir_reg = next(reg_gen)
-        return [
-            f"{self.ir_ref_without_type_annotation} = private {additional_prefix} "
-            f"{self.type.ir_type} {literal}"
-        ]
+        self.ir_reg = ctx.next_reg()
+        return IROutput(
+            [
+                f"{self.ir_ref_without_type_annotation} = private {additional_prefix} "
+                f"{self.type.ir_type} {literal}"
+            ]
+        )
 
     def assert_can_read_from(self) -> None:
         pass
 
     def assert_can_write_to(self) -> None:
         pass
 
 
 class Scope(Generatable):
-    def __init__(self, scope_id: int, outer_scope: Optional["Scope"] = None) -> None:
-        super().__init__()
+    def __init__(
+        self,
+        scope_id: int,
+        meta: Meta,
+        outer_scope: Scope | None = None,
+        is_inside_loop: bool = False,
+    ) -> None:
+        super().__init__(meta)
 
         assert scope_id >= 0
         self.id = scope_id
 
-        self._outer_scope: Optional[Scope] = outer_scope
+        self._outer_scope: Scope | None = outer_scope
         self._variables: dict[str, StackVariable] = {}
         self._lines: list[Generatable] = []
-        self._generic_pack: Optional[tuple[str, int]] = None
+        self._generic_pack: tuple[str, int] | None = None
         self._allocations: list[StackVariable] = []
+        self._is_inside_loop: bool = is_inside_loop
 
     def _record_allocation(self, var: StackVariable) -> None:
         self._allocations.append(var)
 
         if self._outer_scope is not None:
             self._outer_scope._record_allocation(var)
 
@@ -133,15 +198,15 @@
         # must be unique in a single scope.
         if var.user_facing_name in self._variables:
             raise RedefinitionError("variable", var.user_facing_name)
 
         self._record_allocation(var)
         self._variables[var.user_facing_name] = var
 
-    def search_for_variable(self, var_name: str) -> Optional[StackVariable]:
+    def search_for_variable(self, var_name: str) -> StackVariable | None:
         # Search this scope first.
         if var_name in self._variables:
             return self._variables[var_name]
 
         # Then move up the stack.
         if self._outer_scope:
             return self._outer_scope.search_for_variable(var_name)
@@ -169,25 +234,25 @@
     def start_label(self) -> str:
         return f"scope_{self.id}_begin"
 
     @property
     def end_label(self) -> str:
         return f"scope_{self.id}_end"
 
-    def generate_ir(self, reg_gen: Iterator[int]) -> list[str]:
-        contained_ir = []
+    def generate_ir(self, ctx: IRContext) -> IROutput:
+        contained_ir = IROutput()
 
         # Variables are allocated at the function scope (not in inner-scopes)
         #   This prevents a large loop causing a stack overflow
         if self._outer_scope is None:
             for variable in self._allocations:
-                contained_ir.extend(variable.generate_ir(reg_gen))
+                contained_ir.extend(variable.generate_ir(ctx))
 
         for line in self._lines:
-            contained_ir.extend(line.generate_ir(reg_gen))
+            contained_ir.extend(line.generate_ir(ctx))
             if line.is_return_guaranteed():
                 # Avoid generating dead instructions
                 # TODO: warn about unreachable code
                 break
 
         return contained_ir
 
@@ -197,255 +262,364 @@
     def is_return_guaranteed(self) -> bool:
         for line in self._lines:
             if line.is_return_guaranteed():
                 # TODO: it would be nice if we could give a dead code warning here
                 return True
         return False
 
+    def is_jump_guaranteed(self) -> bool:
+        for line in self._lines:
+            if line.is_jump_guaranteed():
+                # TODO: it would be nice if we could give a dead code warning here
+                return True
+        return False
+
+    def is_inside_loop(self) -> bool:
+        if self._is_inside_loop:
+            return True
+
+        if self._outer_scope:
+            return self._outer_scope.is_inside_loop()
+
+        return False
+
     def __repr__(self) -> str:
         return f"{{{','.join(map(repr, self._lines))}}}"
 
 
 class IfElseStatement(Generatable):
     def __init__(
         self,
         condition: TypedExpression,
         if_scope: Scope,
         else_scope: Scope,
+        meta: Meta,
     ) -> None:
-        super().__init__()
+        super().__init__(meta)
 
         condition.assert_can_read_from()
         assert_is_implicitly_convertible(condition, BoolType(), "if condition")
 
         self.condition = condition
         self.if_scope = if_scope
         self.else_scope = else_scope
 
-    def generate_ir(self, reg_gen: Iterator[int]) -> list[str]:
+    def generate_ir(self, ctx: IRContext) -> IROutput:
         # https://llvm.org/docs/LangRef.html#br-instruction
         need_label_after_statement = False
 
         conv_condition, extra_exprs = do_implicit_conversion(self.condition, BoolType())
 
-        ir = self.expand_ir(extra_exprs, reg_gen)
+        ir = self.expand_ir(extra_exprs, ctx)
+
+        dbg = self.add_di_location(ctx, ir)
 
         # br i1 <cond>, label <iftrue>, label <iffalse>
-        ir.append(
+        ir.lines.append(
             f"br {conv_condition.ir_ref_with_type_annotation}, "
-            f"label %{self.if_scope.start_label}, label %{self.else_scope.start_label}"
+            f"label %{self.if_scope.start_label}, label %{self.else_scope.start_label}, "
+            f"{dbg}"
         )
 
         # If body
-        ir.append(f"{self.if_scope.start_label}:")
-        ir.extend(self.if_scope.generate_ir(reg_gen))
+        ir.lines.append(f"{self.if_scope.start_label}:")
+        ir.extend(self.if_scope.generate_ir(ctx))
 
-        if not self.if_scope.is_return_guaranteed():
+        if not self.if_scope.is_jump_guaranteed():
             # Jump to the end of the if/else statement.
-            ir.append(f"br label %{self.else_scope.end_label}")
+            ir.lines.append(f"br label %{self.else_scope.end_label}, {dbg}")
             need_label_after_statement = True
 
         # Else body
-        ir.append(f"{self.else_scope.start_label}:")
-        ir.extend(self.else_scope.generate_ir(reg_gen))
+        ir.lines.append(f"{self.else_scope.start_label}:")
+        ir.extend(self.else_scope.generate_ir(ctx))
 
-        if not self.else_scope.is_return_guaranteed():
+        if not self.else_scope.is_jump_guaranteed():
             # Jump to the end of the if/else statement.
-            ir.append(f"br label %{self.else_scope.end_label}")
+            ir.lines.append(f"br label %{self.else_scope.end_label}, {dbg}")
             need_label_after_statement = True
 
         if need_label_after_statement:
             # LLVM will complain if this is empty.
-            ir.append(f"{self.else_scope.end_label}:")
+            ir.lines.append(f"{self.else_scope.end_label}:")
 
         return ir
 
     def is_return_guaranteed(self) -> bool:
         return (
             self.if_scope.is_return_guaranteed()
             and self.else_scope.is_return_guaranteed()
         )
 
+    def is_jump_guaranteed(self) -> bool:
+        return (
+            self.if_scope.is_jump_guaranteed() and self.else_scope.is_jump_guaranteed()
+        )
+
     def __repr__(self) -> str:
         return f"IfElseStatement({self.condition} {self.if_scope} {self.else_scope})"
 
 
 class WhileStatement(Generatable):
     def __init__(
         self,
         new_scope_id: int,
         condition: TypedExpression,
         condition_generatable: list[Generatable],
         inner_scope: Scope,
+        meta: Meta,
     ) -> None:
-        super().__init__()
+        super().__init__(meta)
 
         condition.assert_can_read_from()
         assert_is_implicitly_convertible(condition, BoolType(), "while condition")
 
-        self.start_label = f"while_{new_scope_id}_begin"
-        self.end_label = f"while_{new_scope_id}_end"
+        self.info = LoopInfo(f"while_{new_scope_id}_begin", f"while_{new_scope_id}_end")
 
         self.condition = condition
         self.condition_generatable = condition_generatable
         self.inner_scope = inner_scope
 
-    def generate_ir(self, reg_gen: Iterator[int]) -> list[str]:
+    def generate_ir(self, ctx: IRContext) -> IROutput:
         # https://llvm.org/docs/LangRef.html#br-instruction
 
         conv_condition, extra_exprs = do_implicit_conversion(self.condition, BoolType())
 
+        ir = IROutput()
+        dbg = self.add_di_location(ctx, ir)
+
+        # br label <dest>
+        ir.lines.extend(
+            [
+                f"br label %{self.info.start_label}, {dbg}",
+                f"{self.info.start_label}:",
+            ]
+        )
+        # Evaluate condition
+        ir.extend(self.expand_ir(self.condition_generatable, ctx))
+        ir.extend(self.expand_ir(extra_exprs, ctx))
         # br i1 <cond>, label <iftrue>, label <iffalse>
-        return [
-            f"br label %{self.start_label}",
-            f"{self.start_label}:",
-            # Evaluate condition
-            *self.expand_ir(self.condition_generatable, reg_gen),
-            *self.expand_ir(extra_exprs, reg_gen),
-            (
-                f"br {conv_condition.ir_ref_with_type_annotation}, label "
-                f"%{self.inner_scope.start_label}, label %{self.end_label}"
-            ),
-            # Loop body
-            f"{self.inner_scope.start_label}:",
-            *self.inner_scope.generate_ir(reg_gen),
-            f"br label %{self.start_label}",  # Loop
-            f"{self.end_label}:",
-        ]
+        ir.lines.append(
+            f"br {conv_condition.ir_ref_with_type_annotation}, label "
+            f"%{self.inner_scope.start_label}, label %{self.info.end_label}, {dbg}"
+        )
+        # Loop body
+        ir.lines.append(f"{self.inner_scope.start_label}:")
+        ctx.loop_stack.push(self.info)  # TODO clean up with a context manager?
+        ir.extend(self.inner_scope.generate_ir(ctx))
+        ctx.loop_stack.pop()
+
+        # e.g. if the scope includes continue statements in all code paths.
+        if not self.inner_scope.is_jump_guaranteed():
+            ir.lines.append(f"br label %{self.info.start_label}, {dbg}")
+
+        ir.lines.append(f"{self.info.end_label}:")
+
+        return ir
 
     def is_return_guaranteed(self) -> bool:
         return False
 
     def __repr__(self) -> str:
         return f"While({self.condition} {self.inner_scope})"
 
 
 class ReturnStatement(Generatable):
     def __init__(
-        self, return_type: Type, returned_expr: Optional[TypedExpression] = None
+        self,
+        return_type: Type,
+        meta: Meta,
+        returned_expr: TypedExpression | None = None,
     ) -> None:
-        super().__init__()
+        super().__init__(meta)
 
         if returned_expr is not None:
             returned_expr.assert_can_read_from()
             assert_is_implicitly_convertible(
                 returned_expr, return_type, "return statement"
             )
+        elif return_type != VoidType():
+            raise TypeCheckerError(
+                "return statement",
+                return_type.format_for_output_to_user(),
+                VoidType().format_for_output_to_user(),
+                maybe_missing_borrow=False,
+            )
 
         self.return_type = return_type
         self.returned_expr = returned_expr
 
-    def generate_ir(self, reg_gen: Iterator[int]) -> list[str]:
+    def generate_ir(self, ctx: IRContext) -> IROutput:
         # https://llvm.org/docs/LangRef.html#i-ret
 
+        ir = IROutput()
+        dbg = self.add_di_location(ctx, ir)
+
         # We have to use return_type instead of returned_expr.underlying_type,
         # as returned_expr might be an initializer list, which throws when its
         # type is accesssed.
         if self.returned_expr is None or self.return_type == VoidType():
             # ret void; Return from void function
-            return ["ret void"]
+            ir.lines.append(f"ret void, {dbg}")
+            return ir
 
         conv_returned_expr, extra_exprs = do_implicit_conversion(
             self.returned_expr, self.return_type
         )
 
-        ir_lines = self.expand_ir(extra_exprs, reg_gen)
+        ir.extend(self.expand_ir(extra_exprs, ctx))
 
         # ret <type> <value>; Return a value from a non-void function
-        ir_lines.append(f"ret {conv_returned_expr.ir_ref_with_type_annotation}")
+        ir.lines.append(f"ret {conv_returned_expr.ir_ref_with_type_annotation}, {dbg}")
 
-        return ir_lines
+        return ir
 
     def is_return_guaranteed(self) -> bool:
         return True
 
     def __repr__(self) -> str:
         return f"ReturnStatement({self.returned_expr})"
 
 
+class ContinueStatement(Generatable):
+    def __init__(self, meta: Meta) -> None:
+        super().__init__(meta)
+
+    def generate_ir(self, ctx: IRContext) -> IROutput:
+        # https://llvm.org/docs/LangRef.html#br-instruction
+
+        assert not ctx.loop_stack.empty()
+
+        ir = IROutput()
+        dbg = self.add_di_location(ctx, ir)
+
+        # br label <dest>
+        ir.lines.append(f"br label %{ctx.loop_stack.peek().start_label}, {dbg}")
+
+        return ir
+
+    def is_return_guaranteed(self) -> bool:
+        return False
+
+    def is_jump_guaranteed(self) -> bool:
+        return True
+
+    def __repr__(self) -> str:
+        return "ContinueStatement()"
+
+
+class BreakStatement(Generatable):
+    def __init__(self, meta: Meta) -> None:
+        super().__init__(meta)
+
+    def generate_ir(self, ctx: IRContext) -> IROutput:
+        # https://llvm.org/docs/LangRef.html#br-instruction
+
+        assert not ctx.loop_stack.empty()
+
+        ir = IROutput()
+        dbg = self.add_di_location(ctx, ir)
+
+        # br label <dest>
+        ir.lines.append(f"br label %{ctx.loop_stack.peek().end_label}, {dbg}")
+
+        return ir
+
+    def is_return_guaranteed(self) -> bool:
+        return False
+
+    def is_jump_guaranteed(self) -> bool:
+        return True
+
+    def __repr__(self) -> str:
+        return "BreakStatement()"
+
+
 class VariableInitialize(Generatable):
-    def __init__(self, variable: StackVariable, value: TypedExpression) -> None:
-        super().__init__()
+    def __init__(
+        self, variable: StackVariable, value: TypedExpression, meta: Meta
+    ) -> None:
+        super().__init__(meta)
 
         value.assert_can_read_from()
         assert_is_implicitly_convertible(value, variable.type, "variable assignment")
 
         self.variable = variable
         self.value = value
 
-    def generate_ir(self, reg_gen: Iterator[int]) -> list[str]:
+    def generate_ir(self, ctx: IRContext) -> IROutput:
         # https://llvm.org/docs/LangRef.html#store-instruction
 
         conv_value, extra_exprs = do_implicit_conversion(self.value, self.variable.type)
 
-        ir_lines = self.expand_ir(extra_exprs, reg_gen)
+        ir = self.expand_ir(extra_exprs, ctx)
+
+        dbg = self.add_di_location(ctx, ir)
 
         # store [volatile] <ty> <value>, ptr <pointer>[, align <alignment>]...
-        ir_lines += [
+        ir.lines.append(
             f"store {conv_value.ir_ref_with_type_annotation}, {self.variable.ir_ref}, "
-            f"align {conv_value.get_equivalent_pure_type().alignment}"
-        ]
+            f"align {conv_value.result_type_as_if_borrowed.alignment}, {dbg}"
+        )
 
-        return ir_lines
+        return ir
 
     def is_return_guaranteed(self) -> bool:
         return False
 
     def __repr__(self) -> str:
         return (
             f"VariableAssignment({self.variable.user_facing_name}:"
             f" {self.variable.type})"
         )
 
 
 class Assignment(Generatable):
-    def __init__(self, dst: TypedExpression, src: TypedExpression) -> None:
-        super().__init__()
+    def __init__(self, dst: TypedExpression, src: TypedExpression, meta: Meta) -> None:
+        super().__init__(meta)
 
-        if dst.underlying_type.storage_kind != Type.Kind.VALUE:
-            raise AssignmentToBorrowedReference(
-                dst.underlying_type.format_for_output_to_user()
-            )
+        if dst.result_type.storage_kind.is_reference():
+            raise AssignmentToBorrowedReference(dst.format_for_output_to_user())
 
         dst.assert_can_write_to()
         src.assert_can_read_from()
 
-        storage_kind = dst.get_equivalent_pure_type().storage_kind
+        storage_kind = dst.result_type_as_if_borrowed.storage_kind
 
         if not storage_kind.is_reference():
-            raise AssignmentToNonPointerError(
-                dst.underlying_type.format_for_output_to_user()
-            )
+            raise AssignmentToNonPointerError(dst.format_for_output_to_user())
 
-        if storage_kind == Type.Kind.CONST_REF:
+        if not storage_kind.is_mutable_reference():
             raise CannotAssignToAConstant(
-                dst.get_equivalent_pure_type().format_for_output_to_user()
+                dst.result_type_as_if_borrowed.format_for_output_to_user()
             )
 
         self._dst = dst
         self._src = src
 
-        self._target_type = dst.underlying_type
+        self._target_type = dst.result_type
         assert_is_implicitly_convertible(self._src, self._target_type, "assignment")
 
-    def generate_ir(self, reg_gen: Iterator[int]) -> list[str]:
+    def generate_ir(self, ctx: IRContext) -> IROutput:
         # https://llvm.org/docs/LangRef.html#store-instruction
         converted_src, src_conversions = do_implicit_conversion(
             self._src, self._target_type, "assignment"
         )
 
-        conversion_ir: list[str] = []
-        conversion_ir.extend(self.expand_ir(src_conversions, reg_gen))
+        ir = self.expand_ir(src_conversions, ctx)
+
+        dbg = self.add_di_location(ctx, ir)
 
         # store [volatile] <ty> <value>, ptr <pointer>[, align <alignment>]...
-        return [
-            *conversion_ir,
+        ir.lines.append(
             f"store {converted_src.ir_ref_with_type_annotation}, "
             f"{self._dst.ir_ref_with_type_annotation}, "
-            f"align {self._dst.get_equivalent_pure_type().alignment}",
-        ]
+            f"align {self._dst.result_type_as_if_borrowed.alignment}, {dbg}"
+        )
+
+        return ir
 
     def is_return_guaranteed(self) -> bool:
         return False
 
     def __repr__(self) -> str:
         return f"Assignment({self._dst} = {self._src})"
```

### Comparing `glang-0.2.1/src/glang/codegen/interfaces.py` & `glang-0.4.0/src/glang/codegen/interfaces.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 from abc import ABC, abstractmethod
-from dataclasses import dataclass
+from collections.abc import Iterable, Iterator
+from dataclasses import dataclass, field
 from enum import Enum
-from typing import Any, Iterable, Iterator, Optional
+from typing import Any
 
-from .user_facing_errors import MutableVariableContainsAReference
+from glang.codegen.debug import DIFile, DILocation, DIScope, Metadata
+from glang.codegen.user_facing_errors import MutableVariableContainsAReference
+from glang.parser.lexer_parser import Meta
+from glang.utils.stack import Stack
 
 
 class TypeDefinition(ABC):
     def graphene_literal_to_ir_constant(self, value: str) -> str:
-        assert False
+        raise AssertionError
 
     @abstractmethod
     def are_equivalent(self, other: "TypeDefinition") -> bool:
         pass
 
     @abstractmethod
     def format_for_output_to_user(self) -> str:
@@ -51,33 +55,42 @@
     def is_void(self) -> bool:
         return False
 
     @property
     def storage_kind(self) -> "Type.Kind":
         return Type.Kind.VALUE
 
+    @abstractmethod
+    def to_di_type(self, metadata_gen: Iterator[int]) -> list[Metadata]:
+        pass
+
     def __repr__(self) -> str:
         return f"TypeDefinition({self.format_for_output_to_user()})"
 
 
 class Type(ABC):
     class Kind(Enum):
         VALUE = 1
         MUTABLE_REF = 2
         CONST_REF = 3
+        # Mutable reference, but implicitly convertible to a const reference.
+        MUTABLE_OR_CONST_REF = 4
 
         def is_reference(self) -> bool:
             return self != Type.Kind.VALUE
 
+        def is_mutable_reference(self) -> bool:
+            return self in (self.MUTABLE_REF, self.MUTABLE_OR_CONST_REF)
+
     def __init__(self, definition: TypeDefinition) -> None:
         self.definition = definition
 
         self._visited_in_finite_resolution = False
 
-    def __eq__(self, other: Any) -> bool:
+    def __eq__(self, other: object) -> bool:
         assert isinstance(other, Type)
         return self.definition.are_equivalent(other.definition)
 
     @property
     def is_finite(self) -> bool:
         if self._visited_in_finite_resolution:
             return False
@@ -116,34 +129,71 @@
         pass
 
     @property
     @abstractmethod
     def ir_type(self) -> str:
         pass
 
+    def to_di_type(self, metadata_gen: Iterator[int]) -> list[Metadata]:
+        return self.definition.to_di_type(metadata_gen)
+
     def __repr__(self) -> str:
         return f"Type({self.format_for_output_to_user(True)})"
 
 
+@dataclass
+class IROutput:
+    lines: list[str] = field(default_factory=list)
+    metadata: set[Metadata] = field(default_factory=set)
+
+    def extend(self, other: "IROutput") -> None:
+        self.lines.extend(other.lines)
+        self.metadata.update(other.metadata)
+
+
+@dataclass
+class LoopInfo:
+    start_label: str
+    end_label: str
+
+
+@dataclass
+class IRContext:
+    reg_gen: Iterator[int]
+    metadata_gen: Iterator[int]
+    scope: DIScope
+    loop_stack: Stack[LoopInfo]
+
+    def next_reg(self) -> int:
+        return next(self.reg_gen)
+
+    def next_meta(self) -> int:
+        return next(self.metadata_gen)
+
+
 class Variable(ABC):
-    def __init__(self, name: str, var_type: Type, is_mutable: bool) -> None:
+    def __init__(
+        self, name: str, var_type: Type, is_mutable: bool, meta: Meta, di_file: DIFile
+    ) -> None:
         super().__init__()
 
         self._name = name
         self.type = var_type
         self.is_mutable = is_mutable
+        self._meta = meta
+        self._di_file = di_file
 
         # We cannot store references in mutable variables. Since there is no
         #  syntax to reassign the reference
         if self.type.storage_kind.is_reference() and self.is_mutable:
             raise MutableVariableContainsAReference(
                 self._name, self.type.format_for_output_to_user(True)
             )
 
-        self.ir_reg: Optional[int] = None
+        self.ir_reg: int | None = None
 
     @property
     def user_facing_name(self) -> str:
         return self._name
 
     @property
     @abstractmethod
@@ -152,126 +202,132 @@
 
     @property
     @abstractmethod
     def ir_ref(self) -> str:
         pass
 
     @abstractmethod
-    def generate_ir(self, reg_gen: Iterator[int]) -> list[str]:
+    def generate_ir(self, ctx: IRContext) -> IROutput:
         pass
 
     def __repr__(self) -> str:
-        return f"{self.__class__.__name__}({self._name}: {repr(self.type)}, is_mut: {self.is_mutable})"
+        return f"{self.__class__.__name__}({self._name}: {self.type!r}, is_mut: {self.is_mutable})"
 
     @abstractmethod
     def assert_can_read_from(self) -> None:
         pass
 
     @abstractmethod
     def assert_can_write_to(self) -> None:
         pass
 
 
 class Generatable(ABC):
-    def generate_ir(self, _: Iterator[int]) -> list[str]:
-        return []
+    def __init__(self, meta: Meta | None) -> None:
+        super().__init__()
+
+        self.meta = meta
+
+    def generate_ir(self, ctx: IRContext) -> IROutput:
+        return IROutput()
 
     @abstractmethod
     def is_return_guaranteed(self) -> bool:
         pass
 
+    def is_jump_guaranteed(self) -> bool:
+        return self.is_return_guaranteed()
+
     @abstractmethod
     def __repr__(self) -> str:
         pass
 
     @staticmethod
-    def expand_ir(
-        generatables: Iterable["Generatable"], reg_gen: Iterator[int]
-    ) -> list[str]:
-        ir_lines: list[str] = []
+    def expand_ir(generatables: Iterable["Generatable"], ctx: IRContext) -> IROutput:
+        ir_output = IROutput()
 
         for generatable in generatables:
-            ir_lines.extend(generatable.generate_ir(reg_gen))
+            ir_output.extend(generatable.generate_ir(ctx))
+
+        return ir_output
 
-        return ir_lines
+    def add_di_location(self, ctx: IRContext, ir: IROutput) -> str:
+        assert self.meta is not None
+
+        di_location = DILocation(
+            ctx.next_meta(),
+            self.meta.start.line,
+            self.meta.start.column,
+            ctx.scope,
+        )
+        ir.metadata.add(di_location)
+
+        return f"!dbg !{di_location.id}"
 
 
 class TypedExpression(Generatable):
     def __init__(
-        self,
-        expr_type: Optional[Type],
-        underlying_indirection_kind: Type.Kind,
-        was_reference_type_at_any_point: bool = False,
+        self, underlying_indirection_kind: Type.Kind, meta: Meta | None
     ) -> None:
-        super().__init__()
-        # It is the callers responsibility to escape double indirections
-        if expr_type is not None and expr_type.storage_kind.is_reference():
-            assert not underlying_indirection_kind.is_reference()
-
-        self._underlying_type = expr_type
+        super().__init__(meta)
         self.underlying_indirection_kind = underlying_indirection_kind
-
-        # Used for better error messages
-        self.was_reference_type_at_any_point = was_reference_type_at_any_point
-
-        self.result_reg: Optional[int] = None
+        self.result_reg: int | None = None
 
     @property
-    def underlying_type(self) -> Type:
-        assert self._underlying_type is not None
-        return self._underlying_type
+    @abstractmethod
+    def result_type(self) -> Type:
+        pass
 
-    def get_equivalent_pure_type(self) -> Type:
+    @property
+    def result_type_as_if_borrowed(self) -> Type:
         if self.underlying_indirection_kind.is_reference():
-            return self.underlying_type.convert_to_storage_type(
+            return self.result_type.convert_to_storage_type(
                 self.underlying_indirection_kind
             )
-        return self.underlying_type
+        return self.result_type
 
     @property
+    @abstractmethod
     def has_address(self) -> bool:
-        return (
-            self.underlying_type.storage_kind.is_reference()
-            or self.underlying_indirection_kind.is_reference()
-        )
+        pass
 
     def is_return_guaranteed(self) -> bool:
         # At the moment no TypedExpression can return
         return False
 
     @property
     def ir_ref_with_type_annotation(self) -> str:
         assert self.ir_ref_without_type_annotation is not None
         return f"{self.ir_type_annotation} {self.ir_ref_without_type_annotation}"
 
     @property
+    @abstractmethod
     def ir_type_annotation(self) -> str:
-        if self.underlying_indirection_kind.is_reference():
-            return "ptr"
-
-        return self.underlying_type.ir_type
+        pass
 
-    def dereference_double_indirection(
-        self, reg_gen: Iterator[int], ir: list[str]
-    ) -> int:
+    def dereference_double_indirection(self, ctx: IRContext, ir: IROutput) -> int:
         # Converts a double indirection eg. address of reference into a reference
         assert self.has_address
 
-        store_at = next(reg_gen)
-        ir.append(
+        dbg = self.add_di_location(ctx, ir)
+
+        store_at = ctx.next_reg()
+        ir.lines.append(
             f"%{store_at} = load ptr, {self.ir_ref_with_type_annotation}, "
-            f"align {self.get_equivalent_pure_type().alignment}"
+            f"align {self.result_type_as_if_borrowed.alignment}, {dbg}"
         )
         return store_at
 
+    @abstractmethod
     def format_for_output_to_user(self) -> str:
-        return self.underlying_type.format_for_output_to_user()
+        pass
 
+    @abstractmethod
     def try_convert_to_type(self, type: Type) -> tuple[int, list["TypedExpression"]]:
-        return (0, [])
+        pass
 
     @property
     @abstractmethod
     def ir_ref_without_type_annotation(self) -> str:
         pass
 
     @abstractmethod
@@ -279,36 +335,83 @@
         pass
 
     @abstractmethod
     def assert_can_write_to(self) -> None:
         pass
 
 
+class StaticTypedExpression(TypedExpression):
+    def __init__(
+        self,
+        expr_type: Type,
+        underlying_indirection_kind: Type.Kind,
+        meta: Meta | None,
+        was_reference_type_at_any_point: bool = False,
+    ) -> None:
+        # It is the caller's responsibility to escape double indirections
+        if expr_type.storage_kind.is_reference():
+            assert not underlying_indirection_kind.is_reference()
+
+        self.underlying_type = expr_type
+
+        self.was_reference_type_at_any_point = was_reference_type_at_any_point
+        super().__init__(underlying_indirection_kind, meta)
+
+    @property
+    def result_type(self) -> Type:
+        return self.underlying_type
+
+    @property
+    def has_address(self) -> bool:
+        return (
+            self.underlying_type.storage_kind.is_reference()
+            or self.underlying_indirection_kind.is_reference()
+        )
+
+    def format_for_output_to_user(self) -> str:
+        return self.underlying_type.format_for_output_to_user()
+
+    def try_convert_to_type(self, type: Type) -> tuple[int, list[TypedExpression]]:
+        return (0, [])
+
+    @property
+    def ir_type_annotation(self) -> str:
+        if self.underlying_indirection_kind.is_reference():
+            return "ptr"
+
+        return self.underlying_type.ir_type
+
+
 SpecializationItem = Type | int
 
 
 @dataclass(frozen=True)
 class GenericArgument:
     name: str
     is_value_arg: bool
 
 
 @dataclass
 class GenericMapping:
     mapping: dict[GenericArgument, SpecializationItem]
     pack: list[Type]
 
+    def __add__(self, other: Any) -> "GenericMapping":
+        assert isinstance(other, GenericMapping)
+        assert len(self.pack) == 0 or len(other.pack) == 0
+        return GenericMapping({**self.mapping, **other.mapping}, self.pack + other.pack)
+
 
 def do_specializations_match(
     s1: list[SpecializationItem], s2: list[SpecializationItem]
 ) -> bool:
     if len(s1) != len(s2):
         return False
 
-    for item1, item2 in zip(s1, s2):
+    for item1, item2 in zip(s1, s2, strict=True):
         if isinstance(item1, Type) != isinstance(item2, Type):
             return False
 
         if item1 != item2:
             return False
 
     return True
@@ -326,15 +429,15 @@
 
 
 def format_arguments(args: Iterable[Type] | Iterable[TypedExpression]) -> str:
     items = ", ".join(item.format_for_output_to_user() for item in args)
     return f"({items})"
 
 
-def format_generics(args: Iterable[GenericArgument], pack_name: Optional[str]) -> str:
+def format_generics(args: Iterable[GenericArgument], pack_name: str | None) -> str:
     formatted_generics = [item.name for item in args]
     if pack_name is not None:
         formatted_generics.append(pack_name)
 
     if len(formatted_generics) == 0:
         return ""
```

### Comparing `glang-0.2.1/src/glang/codegen/strings.py` & `glang-0.4.0/src/glang/codegen/strings.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from .user_facing_errors import InvalidEscapeSequence
+from glang.codegen.user_facing_errors import InvalidEscapeSequence
 
 # Based on https://en.cppreference.com/w/cpp/language/escape.
 # We omit \' because we don't have single-quoted strings, and \? because
 # we don't have trigraphs.
 _ESCAPE_SEQUENCES_TABLE = {
     '"': chr(0x22),
     "\\": chr(0x5C),
```

### Comparing `glang-0.2.1/src/glang/codegen/type_conversions.py` & `glang-0.4.0/src/glang/codegen/type_conversions.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,125 +1,128 @@
-from functools import cached_property
-from typing import Iterator, Optional
+from glang.codegen.builtin_types import (
+    HeapArrayDefinition,
+    IEEEFloatDefinition,
+    IntegerDefinition,
+    StackArrayDefinition,
+)
+from glang.codegen.interfaces import (
+    IRContext,
+    IROutput,
+    StaticTypedExpression,
+    Type,
+    TypedExpression,
+)
+from glang.codegen.user_facing_errors import OperandError, TypeCheckerError
 
-from .builtin_types import HeapArrayDefinition, IntegerDefinition, StackArrayDefinition
-from .interfaces import Type, TypedExpression
-from .user_facing_errors import OperandError, TypeCheckerError
 
-
-class SquashIntoUnderlyingType(TypedExpression):
+class RemoveIndirection(StaticTypedExpression):
     def __init__(self, ref: TypedExpression) -> None:
-        # Converts a TypedExpression into an underlying type with no indirection
-        super().__init__(ref.underlying_type, Type.Kind.VALUE)
-
+        super().__init__(ref.result_type, Type.Kind.VALUE, ref.meta)
         self.ref = ref
 
-    def generate_ir(self, reg_gen: Iterator[int]) -> list[str]:
+    def generate_ir(self, ctx: IRContext) -> IROutput:
         # https://llvm.org/docs/LangRef.html#load-instruction
+        self.result_reg = ctx.next_reg()
+        return_type_ir = self.ref.result_type.ir_type
 
-        self.result_reg = next(reg_gen)
-        return_type_ir = self.ref.underlying_type.ir_type
+        ir = IROutput()
+        dbg = self.add_di_location(ctx, ir)
 
         # <result> = load [volatile] <ty>, ptr <pointer>[, align <alignment>]...
-        return [
+        ir.lines.append(
             f"%{self.result_reg} = load {return_type_ir}, "
             f"{self.ref.ir_ref_with_type_annotation}, "
-            f"align {self.get_equivalent_pure_type().alignment}"
-        ]
+            f"align {self.result_type_as_if_borrowed.alignment}, {dbg}"
+        )
 
-    @cached_property
+        return ir
+
+    @property
     def ir_ref_without_type_annotation(self) -> str:
         return f"%{self.result_reg}"
 
     def __repr__(self) -> str:
         return f"SquashIntoUnderlyingType({self.ref})"
 
     def assert_can_read_from(self) -> None:
         self.ref.assert_can_read_from()
 
     def assert_can_write_to(self) -> None:
         raise OperandError("cannot modify a squashed value")
 
 
-class PromoteInteger(TypedExpression):
+class PromoteNumeric(StaticTypedExpression):
     def __init__(self, src: TypedExpression, dest_type: Type) -> None:
-        src_definition = src.underlying_type.definition
+        super().__init__(dest_type, Type.Kind.VALUE, src.meta)
+
+        src_definition = src.result_type.definition
 
         assert not src.has_address
         assert dest_type.storage_kind == Type.Kind.VALUE
-        assert isinstance(src_definition, IntegerDefinition)
-        assert isinstance(dest_type.definition, IntegerDefinition)
-        assert src_definition.is_signed == dest_type.definition.is_signed
-        assert src_definition.bits < dest_type.definition.bits
+        assert src_definition.size < dest_type.size
 
-        super().__init__(dest_type, Type.Kind.VALUE)
+        if isinstance(src_definition, IntegerDefinition):
+            assert isinstance(dest_type.definition, IntegerDefinition)
+            assert src_definition.is_signed == dest_type.definition.is_signed
+            self.instruction = "sext" if src_definition.is_signed else "zext"
+        else:
+            assert isinstance(src_definition, IEEEFloatDefinition)
+            assert isinstance(dest_type.definition, IEEEFloatDefinition)
+            self.instruction = "fpext"
 
         self.src = src
-        self.is_signed = src_definition.is_signed
 
-    def generate_ir(self, reg_gen: Iterator[int]) -> list[str]:
+    def generate_ir(self, ctx: IRContext) -> IROutput:
         # https://llvm.org/docs/LangRef.html#sext-to-instruction
         # https://llvm.org/docs/LangRef.html#zext-to-instruction
+        # https://llvm.org/docs/LangRef.html#fpext-to-instruction
 
-        self.result_reg = next(reg_gen)
-
-        instruction = "sext" if self.is_signed else "zext"
+        self.result_reg = ctx.next_reg()
+        ir = IROutput()
+        dbg = self.add_di_location(ctx, ir)
+
+        # <result> = {s,z,fp}ext <ty> <value> to <ty2> ; yields ty2
+        ir.lines.append(
+            f"%{self.result_reg} = {self.instruction} "
+            f"{self.src.ir_ref_with_type_annotation} to {self.underlying_type.ir_type}, "
+            f"{dbg}"
+        )
 
-        # <result> = {s,z}ext <ty> <value> to <ty2> ; yields ty2
-        return [
-            f"%{self.result_reg} = {instruction} "
-            f"{self.src.ir_ref_with_type_annotation} to {self.underlying_type.ir_type}"
-        ]
+        return ir
 
     @property
     def ir_ref_without_type_annotation(self) -> str:
         return f"%{self.result_reg}"
 
     def __repr__(self) -> str:
-        return f"PromoteInteger({self.src.underlying_type} to {self.underlying_type})"
+        return f"PromoteNumeric({self.src} to {self.underlying_type})"
 
     def assert_can_read_from(self) -> None:
         self.src.assert_can_read_from()
 
     def assert_can_write_to(self) -> None:
         # TODO this isn't very helpful.
         raise OperandError("cannot modify promoted integers")
 
 
-class Reinterpret(TypedExpression):
+class Reinterpret(StaticTypedExpression):
     def __init__(self, src: TypedExpression, dest_type: Type) -> None:
-        # Bit cast between anything
-        super().__init__(dest_type, Type.Kind.VALUE)
-
-        self._src = src
-        self._no_conversion_needed = (
-            self._src.get_equivalent_pure_type().ir_type
-            == self.get_equivalent_pure_type().ir_type
-        )
+        assert src.has_address and not src.underlying_indirection_kind.is_reference()
+        assert dest_type.storage_kind.is_reference()
 
-    def generate_ir(self, reg_gen: Iterator[int]) -> list[str]:
-        # https://llvm.org/docs/LangRef.html#bitcast-to-instruction
+        super().__init__(dest_type, Type.Kind.VALUE, src.meta)
 
-        if self._no_conversion_needed:
-            return []
-
-        self.result_reg = next(reg_gen)
-        return [
-            f"%{self.result_reg} = bitcast {self._src.ir_ref_with_type_annotation} "
-            f"to {self.get_equivalent_pure_type().ir_type}"
-        ]
+        self._src = src
 
     @property
     def ir_ref_without_type_annotation(self) -> str:
-        if self._no_conversion_needed:
-            return self._src.ir_ref_without_type_annotation
-        return f"%{self.result_reg}"
+        return self._src.ir_ref_without_type_annotation
 
     def __repr__(self) -> str:
-        return f"Reinterpret({self._src.underlying_type} to {self.underlying_type})"
+        return f"Reinterpret({self._src} to {self.underlying_type})"
 
     def assert_can_read_from(self) -> None:
         self._src.assert_can_read_from()
 
     def assert_can_write_to(self) -> None:
         self._src.assert_can_write_to()
 
@@ -152,60 +155,82 @@
     """
     expr_list = [src]
 
     def last_expr() -> TypedExpression:
         return expr_list[-1]
 
     def last_type() -> Type:
-        return expr_list[-1].underlying_type
+        return expr_list[-1].result_type
 
     promotion_cost: int = 0
 
     # Always dereference implicit addresses
     if src.underlying_indirection_kind.is_reference():
-        expr_list.append(SquashIntoUnderlyingType(src))
+        expr_list.append(RemoveIndirection(src))
 
     # Initializer lists (+ anything else that depends on the TypedExpression)
     additional_cost, exprs = src.try_convert_to_type(dest_type)
     promotion_cost += additional_cost
     expr_list.extend(exprs)
 
-    # We never implicitly dereferenced
-    if last_type().storage_kind != dest_type.storage_kind:
-        maybe_missing_borrow = False
-        if src.underlying_type == dest_type.convert_to_storage_type(Type.Kind.VALUE):
-            maybe_missing_borrow = src.was_reference_type_at_any_point
-
-        raise TypeCheckerError(
-            context,
-            src.underlying_type.format_for_output_to_user(True),
-            dest_type.format_for_output_to_user(True),
-            maybe_missing_borrow,
-        )
+    match (last_type().storage_kind, dest_type.storage_kind):
+        case Type.Kind.MUTABLE_OR_CONST_REF, dest_kind if dest_kind.is_reference():
+            expr_list.append(
+                Reinterpret(
+                    last_expr(),
+                    last_type().convert_to_storage_type(dest_kind),
+                )
+            )
+            # Preferentially select the mutable overload.
+            if dest_kind == Type.Kind.CONST_REF:
+                promotion_cost += 1
+        case a, b if a != b:
+            # We never implicitly dereference.
+            maybe_missing_borrow = (
+                last_type() == dest_type.convert_to_storage_type(Type.Kind.VALUE)
+                and isinstance(src, StaticTypedExpression)
+                and src.was_reference_type_at_any_point
+            )
+
+            raise TypeCheckerError(
+                context,
+                src.format_for_output_to_user(),
+                dest_type.format_for_output_to_user(True),
+                maybe_missing_borrow,
+            )
 
     # Integer promotion.
     last_def = last_type().definition
     dest_def = dest_type.definition
     if (
         isinstance(last_def, IntegerDefinition)
         and isinstance(dest_def, IntegerDefinition)
         and last_def.is_signed == dest_def.is_signed
-        and last_def.bits < dest_def.bits
+        and last_def.size < dest_def.size
     ):
-        promotion_cost += dest_def.bits // last_def.bits
-        expr_list.append(PromoteInteger(last_expr(), dest_type))
+        promotion_cost += dest_def.size // last_def.size
+        expr_list.append(PromoteNumeric(last_expr(), dest_type))
+
+    # Floating point promotion
+    if (
+        isinstance(last_def, IEEEFloatDefinition)
+        and isinstance(dest_def, IEEEFloatDefinition)
+        and last_def.size < dest_def.size
+    ):
+        promotion_cost += dest_def.size // last_def.size
+        expr_list.append(PromoteNumeric(last_expr(), dest_type))
 
     # Array reference equivalence
     last_array_def = last_type().convert_to_value_type().definition
     dest_array_def = dest_type.convert_to_value_type().definition
     if (
         last_type().storage_kind.is_reference()
         and last_type().storage_kind == dest_type.storage_kind
-        and isinstance(last_array_def, (HeapArrayDefinition, StackArrayDefinition))
-        and isinstance(dest_array_def, (HeapArrayDefinition, StackArrayDefinition))
+        and isinstance(last_array_def, HeapArrayDefinition | StackArrayDefinition)
+        and isinstance(dest_array_def, HeapArrayDefinition | StackArrayDefinition)
         and last_array_def.member == dest_array_def.member
     ):
         if (
             isinstance(last_array_def, HeapArrayDefinition)
             and isinstance(dest_array_def, HeapArrayDefinition)
             and last_array_def.known_dimensions == dest_array_def.known_dimensions
         ):
@@ -224,20 +249,18 @@
             and isinstance(dest_array_def, StackArrayDefinition)
             and last_array_def.dimensions[1:] == dest_array_def.dimensions[1:]
             and last_array_def.dimensions[0] >= dest_array_def.dimensions[0]
         ):
             # TODO: promotion cost going from known size to smaller/ unknown size
             expr_list.append(Reinterpret(last_expr(), dest_type))
 
-    # TODO float promotion.
-
     if last_type() != dest_type:
         raise TypeCheckerError(
             context,
-            src.underlying_type.format_for_output_to_user(),
+            src.format_for_output_to_user(),
             dest_type.format_for_output_to_user(),
         )
 
     return promotion_cost, expr_list
 
 
 def do_implicit_conversion(
@@ -254,22 +277,22 @@
     # Just discard the return value. It will throw if the conversion fails.
     # TODO maybe we could cache the result for later.
     implicit_conversion_impl(expr, target, context)
 
 
 def get_implicit_conversion_cost(
     src: Type | TypedExpression, dest_type: Type
-) -> Optional[int]:
-    class Wrapper(TypedExpression):
+) -> int | None:
+    class Wrapper(StaticTypedExpression):
         def __init__(self, expr_type: Type) -> None:
-            super().__init__(expr_type, Type.Kind.VALUE)
+            super().__init__(expr_type, Type.Kind.VALUE, None)
 
         @property
         def ir_ref_without_type_annotation(self) -> str:
-            assert False
+            raise AssertionError
 
         def assert_can_read_from(self) -> None:
             pass
 
         def assert_can_write_to(self) -> None:
             pass
```

### Comparing `glang-0.2.1/src/glang/codegen/type_resolution.py` & `glang-0.4.0/src/glang/codegen/type_resolution.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 from abc import abstractmethod
 from collections import defaultdict
+from collections.abc import Callable, Iterable
 from dataclasses import dataclass
 from functools import partial
 from itertools import groupby
-from typing import Callable, Iterable, Optional
 from uuid import UUID, uuid4
 
-from .builtin_types import (
+from glang.codegen.builtin_types import (
     AnonymousType,
     FunctionSignature,
     HeapArrayDefinition,
     NamedType,
     PlaceholderDefinition,
     PrimitiveType,
     StackArrayDefinition,
     StructDefinition,
 )
-from .expressions import InitializerList
-from .interfaces import (
+from glang.codegen.debug import DIFile
+from glang.codegen.interfaces import (
     GenericArgument,
     GenericMapping,
     SpecializationItem,
     Type,
     TypedExpression,
     do_specializations_match,
     format_arguments,
     format_generics,
     format_specialization,
 )
-from .type_conversions import get_implicit_conversion_cost
-from .user_facing_errors import (
+from glang.codegen.type_conversions import get_implicit_conversion_cost
+from glang.codegen.user_facing_errors import (
     AmbiguousFunctionCall,
     BuiltinSourceLocation,
     DoubleReferenceError,
     ErrorWithLocationInfo,
     FailedLookupError,
     GrapheneError,
     IncorrectSpecializationCount,
@@ -43,14 +43,15 @@
     OverloadResolutionError,
     PatternMatchDeductionFailure,
     RedeclarationWithIncorrectSpecializationCount,
     RedefinitionError,
     SpecializationFailed,
     SubstitutionFailure,
 )
+from glang.parser.lexer_parser import Meta
 
 
 def get_cost_at_pattern_match_depth(depth: int) -> int:
     # TODO: maybe this should be a list for infinite precision?
     # ATM. only 16 generic deductions/ nested levels are allowed
     return 16 ** (16 - depth)
 
@@ -72,15 +73,15 @@
     @abstractmethod
     def get_generics_taking_part_in_pattern_match(self) -> set[GenericArgument]:
         pass
 
     @abstractmethod
     def pattern_match(
         self, target: Type, out: GenericMapping, depth: int
-    ) -> Optional[int]:
+    ) -> int | None:
         pass
 
 
 @dataclass(frozen=True)
 class CompileTimeConstant:
     @abstractmethod
     def format_for_output_to_user(self) -> str:
@@ -97,17 +98,15 @@
         pass
 
     @abstractmethod
     def get_generics_taking_part_in_pattern_match(self) -> set[GenericArgument]:
         pass
 
     @abstractmethod
-    def pattern_match(
-        self, target: int, out: GenericMapping, depth: int
-    ) -> Optional[int]:
+    def pattern_match(self, target: int, out: GenericMapping, depth: int) -> int | None:
         pass
 
 
 UnresolvedSpecializationItem = UnresolvedType | CompileTimeConstant
 
 
 @dataclass(frozen=True)
@@ -122,17 +121,15 @@
 
     def resolve(self) -> int:
         return self.value
 
     def get_generics_taking_part_in_pattern_match(self) -> set[GenericArgument]:
         return set()
 
-    def pattern_match(
-        self, target: int, _: GenericMapping, depth: int
-    ) -> Optional[int]:
+    def pattern_match(self, target: int, _: GenericMapping, depth: int) -> int | None:
         if target != self.value:
             return None
         return 0
 
 
 @dataclass(frozen=True)
 class GenericValueReference(CompileTimeConstant):
@@ -142,34 +139,33 @@
     def argument(self) -> GenericArgument:
         return GenericArgument(self.name, True)
 
     def format_for_output_to_user(self) -> str:
         return self.name
 
     def produce_specialized_copy(self, generics: GenericMapping) -> CompileTimeConstant:
-        assert self.argument in generics.mapping
+        if self.argument not in generics.mapping:
+            return self
 
         specialized_value = generics.mapping[self.argument]
         if not isinstance(specialized_value, int):
             raise SpecializationFailed(
                 self.format_for_output_to_user(),
                 specialized_value.format_for_output_to_user(),
             )
 
         return NumericLiteralConstant(specialized_value)
 
     def resolve(self) -> int:
-        assert False
+        raise AssertionError
 
     def get_generics_taking_part_in_pattern_match(self) -> set[GenericArgument]:
         return {self.argument}
 
-    def pattern_match(
-        self, target: int, out: GenericMapping, depth: int
-    ) -> Optional[int]:
+    def pattern_match(self, target: int, out: GenericMapping, depth: int) -> int | None:
         if self.argument in out.mapping:
             # TODO: user facing error
             if out.mapping[self.argument] != target:
                 return None
             return 0
 
         out.mapping[self.argument] = target
@@ -190,15 +186,15 @@
         return self.resolved_type
 
     def get_generics_taking_part_in_pattern_match(self) -> set[GenericArgument]:
         return set()
 
     def pattern_match(
         self, target: Type, out: GenericMapping, depth: int
-    ) -> Optional[int]:
+    ) -> int | None:
         if self.resolved_type != target:
             return None
         return 0
 
 
 @dataclass(frozen=True)
 class UnresolvedNamedType(UnresolvedType):
@@ -211,53 +207,56 @@
 
         specialization_format = ", ".join(
             arg.format_for_output_to_user() for arg in self.specialization
         )
         return f"{self.name}<{specialization_format}>"
 
     def produce_specialized_copy(self, generics: GenericMapping) -> UnresolvedType:
-        specialization: list[UnresolvedSpecializationItem] = []
-        for item in self.specialization:
-            specialization.append(item.produce_specialized_copy(generics))
-
-        return UnresolvedNamedType(self.name, tuple(specialization))
+        return UnresolvedNamedType(
+            self.name,
+            tuple(
+                item.produce_specialized_copy(generics) for item in self.specialization
+            ),
+        )
 
     def resolve(self, lookup: Callable[[str, list[SpecializationItem]], Type]) -> Type:
         resolved_specialization = []
         for specialization in self.specialization:
             if isinstance(specialization, UnresolvedType):
                 resolved_specialization.append(specialization.resolve(lookup))
             else:
                 assert isinstance(specialization, CompileTimeConstant)
                 resolved_specialization.append(specialization.resolve())
 
         return lookup(self.name, resolved_specialization)
 
     def _pattern_match_impl(
         self, target: Type, mapping_out: GenericMapping, depth: int
-    ) -> Optional[int]:
+    ) -> int | None:
         if not isinstance(target, NamedType):
             return None
 
         # If our name doesn't match, recurse into the target's alias
         if target.name != self.name:
             if target.alias is None:
                 return None
 
             return self.pattern_match(target.alias, mapping_out, depth)
 
         if len(self.specialization) != len(target.specialization):
             return None
 
         cost = 0
-        for this_arg, target_arg in zip(self.specialization, target.specialization):
+        for this_arg, target_arg in zip(
+            self.specialization, target.specialization, strict=True
+        ):
             if isinstance(this_arg, CompileTimeConstant) != isinstance(target_arg, int):
                 return None
 
-            result: Optional[int] = None
+            result: int | None = None
             if isinstance(this_arg, CompileTimeConstant):
                 assert isinstance(target_arg, int)
                 result = this_arg.pattern_match(target_arg, mapping_out, depth + 1)
 
             if isinstance(this_arg, UnresolvedType):
                 assert isinstance(target_arg, Type)
                 result = this_arg.pattern_match(target_arg, mapping_out, depth + 1)
@@ -275,15 +274,15 @@
                 item.get_generics_taking_part_in_pattern_match()
                 for item in self.specialization
             )
         )
 
     def pattern_match(
         self, target: Type, out: GenericMapping, depth: int
-    ) -> Optional[int]:
+    ) -> int | None:
         curr = target
 
         while curr:
             curr_mapping = GenericMapping(out.mapping.copy(), out.pack.copy())
             result = self._pattern_match_impl(curr, curr_mapping, depth)
 
             if result is not None:
@@ -304,33 +303,34 @@
     def argument(self) -> GenericArgument:
         return GenericArgument(self.name, False)
 
     def format_for_output_to_user(self) -> str:
         return self.name
 
     def produce_specialized_copy(self, generics: GenericMapping) -> UnresolvedType:
-        assert self.argument in generics.mapping
+        if self.argument not in generics.mapping:
+            return self
 
         specialized_type = generics.mapping[self.argument]
         if not isinstance(specialized_type, Type):
             raise SpecializationFailed(
                 self.format_for_output_to_user(), str(specialized_type)
             )
 
         return UnresolvedTypeWrapper(specialized_type)
 
     def resolve(self, _: Callable[[str, list[SpecializationItem]], Type]) -> Type:
-        assert False
+        raise AssertionError
 
     def get_generics_taking_part_in_pattern_match(self) -> set[GenericArgument]:
         return {self.argument}
 
     def pattern_match(
         self, target: Type, out: GenericMapping, depth: int
-    ) -> Optional[int]:
+    ) -> int | None:
         if self.argument in out.mapping:
             if target != out.mapping[self.argument]:
                 return None
             return 0
 
         out.mapping[self.argument] = target
         return get_cost_at_pattern_match_depth(depth)
@@ -347,32 +347,35 @@
 
     def produce_specialized_copy(self, generics: GenericMapping) -> UnresolvedType:
         return UnresolvedReferenceType(
             self.value_type.produce_specialized_copy(generics), self.is_mutable
         )
 
     def resolve(self, lookup: Callable[[str, list[SpecializationItem]], Type]) -> Type:
-        # TODO: support circular references
         resolved_value = self.value_type.resolve(lookup)
         if resolved_value.storage_kind.is_reference():
             raise DoubleReferenceError(resolved_value.format_for_output_to_user(True))
 
         storage = Type.Kind.MUTABLE_REF if self.is_mutable else Type.Kind.CONST_REF
         return resolved_value.convert_to_storage_type(storage)
 
     def get_generics_taking_part_in_pattern_match(self) -> set[GenericArgument]:
         return self.value_type.get_generics_taking_part_in_pattern_match()
 
     def pattern_match(
         self, target: Type, out: GenericMapping, depth: int
-    ) -> Optional[int]:
+    ) -> int | None:
         if target.storage_kind == Type.Kind.VALUE:
             return None
 
-        if (target.storage_kind == Type.Kind.MUTABLE_REF) != self.is_mutable:
+        if (
+            target.storage_kind.is_reference()
+            and target.storage_kind != Type.Kind.MUTABLE_OR_CONST_REF
+            and (target.storage_kind == Type.Kind.MUTABLE_REF) != self.is_mutable
+        ):
             return None
 
         if isinstance(target.definition, HeapArrayDefinition):
             return None
 
         return self.value_type.pattern_match(
             target.convert_to_value_type(), out, depth + 1
@@ -414,16 +417,36 @@
         return set().union(
             *(
                 member[1].get_generics_taking_part_in_pattern_match()
                 for member in self.members
             )
         )
 
-    def pattern_match(self, _1: Type, _2: GenericMapping, _3: int) -> Optional[int]:
-        assert False  # TODO
+    def pattern_match(
+        self, target: Type, generics: GenericMapping, depth: int
+    ) -> int | None:
+        if not isinstance(target.definition, StructDefinition):
+            return None
+
+        cost = 0
+        for our_member, target_member in zip(
+            self.members, target.definition.members, strict=True
+        ):
+            if our_member[0] != target_member[0]:
+                return None  # Struct member names don't match
+
+            if len(our_member[1].get_generics_taking_part_in_pattern_match()) == 0:
+                continue  # No need to pattern match, use type equality
+
+            result = our_member[1].pattern_match(target_member[1], generics, depth + 1)
+            if result is None:
+                return None
+            cost += result
+
+        return cost
 
 
 @dataclass(frozen=True)
 class UnresolvedStackArrayType(UnresolvedType):
     member_type: UnresolvedType
     dimensions: tuple[CompileTimeConstant, ...]
 
@@ -437,17 +460,15 @@
     def produce_specialized_copy(self, generics: GenericMapping) -> UnresolvedType:
         return UnresolvedStackArrayType(
             self.member_type.produce_specialized_copy(generics),
             tuple(dim.produce_specialized_copy(generics) for dim in self.dimensions),
         )
 
     def resolve(self, lookup: Callable[[str, list[SpecializationItem]], Type]) -> Type:
-        resolved_dimensions = []
-        for dimension in self.dimensions:
-            resolved_dimensions.append(dimension.resolve())
+        resolved_dimensions = [dimension.resolve() for dimension in self.dimensions]
 
         resolved_member = self.member_type.resolve(lookup)
         return AnonymousType(StackArrayDefinition(resolved_member, resolved_dimensions))
 
     def get_generics_taking_part_in_pattern_match(self) -> set[GenericArgument]:
         return set().union(
             self.member_type.get_generics_taking_part_in_pattern_match(),
@@ -455,23 +476,25 @@
                 dim.get_generics_taking_part_in_pattern_match()
                 for dim in self.dimensions
             ),
         )
 
     def pattern_match(
         self, target: Type, out: GenericMapping, depth: int
-    ) -> Optional[int]:
+    ) -> int | None:
         if not isinstance(target.definition, StackArrayDefinition):
             return None
 
         if len(self.dimensions) != len(target.definition.dimensions):
             return None
 
         cost = 0
-        for target_dim, our_dim in zip(target.definition.dimensions, self.dimensions):
+        for target_dim, our_dim in zip(
+            target.definition.dimensions, self.dimensions, strict=True
+        ):
             result = our_dim.pattern_match(target_dim, out, depth + 1)
             if result is None:
                 return None
             cost += result
 
         result = self.member_type.pattern_match(
             target.definition.member, out, depth + 1
@@ -526,28 +549,31 @@
                 dim.get_generics_taking_part_in_pattern_match()
                 for dim in self.known_dimensions
             ),
         )
 
     def pattern_match(
         self, target: Type, out: GenericMapping, depth: int
-    ) -> Optional[int]:
+    ) -> int | None:
         if not isinstance(target.definition, HeapArrayDefinition):
             return None
 
-        # TODO: do we pattern match mutable refs into constant refs?
-        if (target.storage_kind == Type.Kind.MUTABLE_REF) != self.is_mutable:
+        if (
+            target.storage_kind.is_reference()
+            and target.storage_kind != Type.Kind.MUTABLE_OR_CONST_REF
+            and (target.storage_kind == Type.Kind.MUTABLE_REF) != self.is_mutable
+        ):
             return None
 
         if len(self.known_dimensions) != len(target.definition.known_dimensions):
             return None
 
         cost = 0
         for target_dim, our_dim in zip(
-            target.definition.known_dimensions, self.known_dimensions
+            target.definition.known_dimensions, self.known_dimensions, strict=True
         ):
             result = our_dim.pattern_match(target_dim, out, depth + 1)
             if result is None:
                 return None
 
         result = self.member_type.pattern_match(
             target.definition.member, out, depth + 1
@@ -568,15 +594,15 @@
     uuid: UUID
 
     def format_name_for_output_to_user(self) -> str:
         if len(self.expanded_specialization) == 0:
             return self.name
 
         specializations_fmt = ", ".join(
-            (item.format_for_output_to_user() for item in self.expanded_specialization)
+            item.format_for_output_to_user() for item in self.expanded_specialization
         )
         return f"{self.name}<{specializations_fmt}>"
 
     def format_for_output_to_user(self) -> str:
         generics_fmt = format_generics(self.generics, None)
         name_fmt = self.format_name_for_output_to_user()
         aliased_fmt = self.aliased.format_for_output_to_user()
@@ -615,28 +641,28 @@
             name, generics, tuple(expanded_specialization), aliased, loc, uuid4()
         )
 
     def pattern_match(
         self,
         target_specialization: list[SpecializationItem],
         mapping_out: GenericMapping,
-    ) -> Optional[int]:
+    ) -> int | None:
         cost = 0
         for item, target in zip(
             self.expanded_specialization, target_specialization, strict=True
         ):
             if isinstance(item, CompileTimeConstant) != isinstance(target, int):
                 return None
 
             if len(item.get_generics_taking_part_in_pattern_match()) == 0:
                 # Nothing to match, we rely on type equality instead
                 # This costs nothing
                 continue
 
-            result: Optional[int] = None
+            result: int | None = None
             if isinstance(item, CompileTimeConstant):
                 assert isinstance(target, int)
                 result = item.pattern_match(target, mapping_out, 1)
 
             if isinstance(item, UnresolvedType):
                 assert isinstance(target, Type)
                 result = item.pattern_match(target, mapping_out, 1)
@@ -652,35 +678,34 @@
         new_specialization = tuple(
             item.produce_specialized_copy(generics)
             for item in self.expanded_specialization
         )
         new_alias = self.aliased.produce_specialized_copy(generics)
 
         return Typedef(
-            self.name, tuple(), new_specialization, new_alias, self.loc, self.uuid
+            self.name, (), new_specialization, new_alias, self.loc, self.uuid
         )
 
 
 @dataclass(frozen=True)
 class UnresolvedFunctionSignature:
     name: str
     expanded_specialization: tuple[UnresolvedSpecializationItem, ...]
     arguments: tuple[UnresolvedType, ...]
-    parameter_pack_argument_name: Optional[str]
+    parameter_pack_argument_name: str | None
     return_type: UnresolvedType
 
-    def collapse_into_type(self, arg: TypedExpression | Type) -> Type:
-        if isinstance(arg, InitializerList):
-            raise NotImplementedError()
+    @staticmethod
+    def collapse_into_type(arg: TypedExpression | Type) -> Type:
         if isinstance(arg, TypedExpression):
-            return arg.underlying_type
+            return arg.result_type
         if isinstance(arg, Type):
             return arg
 
-        assert False
+        raise AssertionError
 
     def format_for_output_to_user(self) -> str:
         specialization_str = ""
         if len(self.expanded_specialization) != 0:
             specialization_list = ", ".join(
                 (
                     item.format_for_output_to_user()
@@ -705,145 +730,140 @@
             )
         )
 
     def produce_specialized_copy(
         self,
         generics: GenericMapping,
     ) -> "UnresolvedFunctionSignature":
-        unmatched_generics = (
-            self.get_generics_taking_part_in_pattern_match() - generics.mapping.keys()
-        )
-        if len(unmatched_generics) != 0:
-            raise PatternMatchDeductionFailure(
-                self.format_for_output_to_user(), unmatched_generics.pop().name
-            )
-
         if self.parameter_pack_argument_name is None:
             assert len(generics.pack) == 0
 
-        new_specialization: list[UnresolvedSpecializationItem] = []
-        for item in self.expanded_specialization:
-            new_specialization.append(item.produce_specialized_copy(generics))
-
-        arguments: list[UnresolvedType] = []
-        for arg in self.arguments:
-            arguments.append(arg.produce_specialized_copy(generics))
+        new_specialization: list[UnresolvedSpecializationItem] = [
+            item.produce_specialized_copy(generics)
+            for item in self.expanded_specialization
+        ]
+
+        arguments: list[UnresolvedType] = [
+            arg.produce_specialized_copy(generics) for arg in self.arguments
+        ]
 
         unresolved_packed_types = [
             UnresolvedTypeWrapper(pack_type) for pack_type in generics.pack
         ]
         arguments.extend(unresolved_packed_types)
         new_specialization.extend(unresolved_packed_types)
 
         return UnresolvedFunctionSignature(
             self.name,
             tuple(new_specialization),
             tuple(arguments),
-            None,  # We have just expanded the parameter pack
+            self.parameter_pack_argument_name if len(generics.pack) == 0 else None,
             self.return_type.produce_specialized_copy(generics),
         )
 
-    def pattern_match(
+    def pattern_match_specialization(
         self,
-        target_args: list[TypedExpression] | list[Type],
         target_specialization: list[SpecializationItem],
         out: GenericMapping,
         depth: int,
-    ) -> Optional[int]:
+    ) -> int | None:
         cost = 0
-
-        # Match the specialization
         for target_item, item in zip(
-            target_specialization, self.expanded_specialization
+            target_specialization, self.expanded_specialization, strict=False
         ):
             if isinstance(item, CompileTimeConstant) != isinstance(target_item, int):
-                return False
+                return None
 
             if len(item.get_generics_taking_part_in_pattern_match()) == 0:
                 continue  # Allow for implicit conversions + type equivalency
 
-            result: Optional[int] = None
+            result: int | None = None
             if isinstance(item, CompileTimeConstant):
                 assert isinstance(target_item, int)
                 result = item.pattern_match(target_item, out, depth + 1)
 
             if isinstance(item, UnresolvedType):
                 assert isinstance(target_item, Type)
                 result = item.pattern_match(target_item, out, depth + 1)
 
             if result is None:
                 return None
 
             cost += result
+        return cost
+
+    def pattern_match_args(
+        self,
+        target_args: list[TypedExpression] | list[Type],
+        out: GenericMapping,
+        depth: int,
+    ) -> int | None:
+        cost = 0
 
         # Check the argument count
         if self.parameter_pack_argument_name is None:
             if len(self.arguments) != len(target_args):
                 return None
         else:
             if len(self.arguments) >= len(target_args):
                 return None
 
         # Match the (non-packed) arguments
         for target_arg, unresolved_arg in zip(
-            target_args[: len(self.arguments)], self.arguments
+            target_args[: len(self.arguments)], self.arguments, strict=True
         ):
             if len(unresolved_arg.get_generics_taking_part_in_pattern_match()) == 0:
                 continue  # Allow for implicit conversions + type equivalency
 
-            if isinstance(target_arg, InitializerList):
-                # See: `docs/types_overview.c3`
-                # TODO: we should convert this to an anonymous struct
-                #   for now we just ignore initializer lists
-                continue
-
             arg_type = self.collapse_into_type(target_arg)
             result = unresolved_arg.pattern_match(arg_type, out, depth + 1)
             if result is None:
                 return None
 
             cost += result
 
         # Match the packed arguments
         if self.parameter_pack_argument_name is not None:
             assert len(out.pack) == 0
             out.pack.extend(
-                (
-                    self.collapse_into_type(arg)
-                    for arg in target_args[len(self.arguments) :]
-                )
+                self.collapse_into_type(arg)
+                for arg in target_args[len(self.arguments) :]
             )
             cost += get_cost_at_pattern_match_depth(depth + 1) * len(out.pack)
 
         return cost
 
 
 @dataclass
 class FunctionDeclaration:
     is_foreign: bool
     arg_names: tuple[str, ...]
-    pack_type_name: Optional[str]
+    pack_type_name: str | None
     generics: tuple[GenericArgument, ...]
     signature: UnresolvedFunctionSignature
     mapping: GenericMapping
     loc: Location
+    meta: Meta
+    di_file: DIFile
     uuid: UUID
 
     @staticmethod
     def construct(
         name: str,
         is_foreign: bool,
         generics: tuple[GenericArgument, ...],
         specialization: Iterable[UnresolvedSpecializationItem],
         arg_names: tuple[str, ...],
-        pack_type_name: Optional[str],
+        pack_type_name: str | None,
         arg_types: tuple[UnresolvedType, ...],
-        parameter_pack_argument_name: Optional[str],
+        parameter_pack_argument_name: str | None,
         return_type: UnresolvedType,
         location: Location,
+        meta: Meta,
+        di_file: DIFile,
     ):
         explicitly_matched_generics = set().union(
             *(
                 item.get_generics_taking_part_in_pattern_match()
                 for item in specialization
             )
         )
@@ -872,42 +892,56 @@
             is_foreign,
             arg_names,
             pack_type_name,
             generics,
             signature,
             GenericMapping({}, []),
             location,
+            meta,
+            di_file,
             uuid4(),
         )
 
     def format_for_output_to_user(self) -> str:
         prefix = "foreign" if self.is_foreign else "function"
         generic_format = format_generics(self.generics, self.pack_type_name)
         return f"{prefix}{generic_format} {self.signature.format_for_output_to_user()}"
 
-    def pattern_match(
+    def pattern_match_specialization(
         self,
-        target_args: list[TypedExpression] | list[Type],
         target_specialization: list[SpecializationItem],
         out: GenericMapping,
-    ) -> Optional[int]:
-        return self.signature.pattern_match(target_args, target_specialization, out, 0)
+    ) -> int | None:
+        return self.signature.pattern_match_specialization(
+            target_specialization, out, 0
+        )
+
+    def pattern_match_args(
+        self,
+        target_args: list[TypedExpression] | list[Type],
+        out: GenericMapping,
+    ) -> int | None:
+        return self.signature.pattern_match_args(target_args, out, 0)
 
     def produce_specialized_copy(
         self, generics: GenericMapping
     ) -> "FunctionDeclaration":
-        assert len(self.mapping.mapping) == 0 and len(self.mapping.pack) == 0
+        assert len(self.mapping.pack) == 0
+
+        remaining_generics = set(self.generics) - set(generics.mapping)
         return FunctionDeclaration(
             self.is_foreign,
             self.arg_names,
             self.pack_type_name,
-            tuple(),
+            tuple(remaining_generics),
             self.signature.produce_specialized_copy(generics),
-            generics,
+            self.mapping + generics,
             self.loc,
+            self.meta,
+            self.di_file,
             self.uuid,
         )
 
 
 class SymbolTable:
     """
     Definitions:
@@ -939,15 +973,17 @@
         # Lookup cache
         self._resolved_types: dict[UUID, list[NamedType]] = defaultdict(list)
         self._resolved_functions: dict[UUID, list[FunctionSignature]] = defaultdict(
             list
         )
 
         # Remember which functions need codegen
-        self._already_codegened: dict[UUID, list[FunctionSignature]] = defaultdict(list)
+        self._already_codegened: dict[
+            UUID, list[tuple[FunctionDeclaration, FunctionSignature]]
+        ] = defaultdict(list)
         self._remaining_to_codegen: list[
             tuple[FunctionDeclaration, FunctionSignature]
         ] = []
 
     def resolve_specialization_item(
         self, unresolved: UnresolvedSpecializationItem
     ) -> SpecializationItem:
@@ -1024,23 +1060,23 @@
         return result
 
     def select_function_with_least_implicit_conversion_cost(
         self,
         fn_name: str,
         candidate_functions: list[tuple[FunctionSignature, FunctionDeclaration]],
         fn_args: list[TypedExpression] | list[Type],
-    ) -> Optional[tuple[FunctionSignature, FunctionDeclaration]]:
+    ) -> tuple[FunctionSignature, FunctionDeclaration] | None:
         functions_by_cost: list[tuple[int, FunctionSignature, FunctionDeclaration]] = []
 
         for function, declaration in candidate_functions:
             total_cost = 0
             if len(fn_args) != len(function.arguments):
                 continue
 
-            for src_expr, dest_type in zip(fn_args, function.arguments):
+            for src_expr, dest_type in zip(fn_args, function.arguments, strict=True):
                 cost = get_implicit_conversion_cost(src_expr, dest_type)
                 if cost is not None:
                     total_cost += cost
                 else:
                     break  # Conversion failed!
             else:
                 # Discard this candidate if conversion fails
@@ -1063,77 +1099,94 @@
             f"{fn_name}{format_arguments(fn_args)}",
             [(fn.format_for_output_to_user(), fn.loc) for _, fn in best_functions],
         )
 
     def add_function_to_codegen(
         self, declaration: FunctionDeclaration, signature: FunctionSignature
     ) -> None:
-        for other in self._already_codegened[declaration.uuid]:
-            if (
-                do_specializations_match(other.specialization, signature.specialization)
-                and other.arguments == signature.arguments
-                and other.return_type == signature.return_type
+        for other_def, other_sig in self._already_codegened[declaration.uuid]:
+            if declaration.uuid == other_def.uuid and do_specializations_match(
+                other_sig.specialization, signature.specialization
             ):
                 return  # Already codegened
 
-        self._already_codegened[declaration.uuid].append(signature)
+        self._already_codegened[declaration.uuid].append((declaration, signature))
         self._remaining_to_codegen.append((declaration, signature))
 
     def lookup_function(
         self,
         name: str,
         given_specialization: list[SpecializationItem],
         args: list[TypedExpression] | list[Type],
+        *,
         evaluated_context: bool,
     ) -> tuple[FunctionSignature, FunctionDeclaration]:
         # Specializes and resolves the function corresponding to the correct definition
         # There are two types of function definition:
         #   1) function [T] fn : ...            (pure generic)
         #   2a) function [T] fn<Thing<T>> : ... (pattern match a)
         #   2b) function [T] fn : (a : T) ...   (pattern match b)
         #
         # The first (pure generic) is syntax sugar for the following:
         #     function [T] fn  ==> function [T] fn<T>
         #
         # A function may deduce its specialization based on its arguments
         #   For now, either the full specialization must be given or none at all
-        #   TODO: relax this requirement
         #
         # We choose which function gets priority based on the following criteria:
         #   1) When initialized the signature MUST not create a substitution failure
         #   2) All parameter implicit conversions MUST succeed
         #   3) Minimize the number of top level generic deductions
         #   4) Minimize the number of 2nd level generic deductions
         #   N) Minimize the number of N level generic deductions
         #   N+1) Minimize the cost of implicit conversion
 
         if name not in self._unresolved_fndefs:
             # Substitution impossible
             raise FailedLookupError(
-                "function", f"function {name}{format_arguments(args)}"
+                "function", f"function {name} : {format_arguments(args)}"
             )
 
         all_candidates: list[tuple[int, FunctionDeclaration]] = []
         for candidate in self._unresolved_fndefs[name]:
+            # The user provides a partial specialization
             generics = GenericMapping({}, [])
-            cost = candidate.pattern_match(args, given_specialization, generics)
-            if cost is None:
+            cost1 = candidate.pattern_match_specialization(
+                given_specialization, generics
+            )
+            if cost1 is None:
+                continue
+
+            partially_specialized = candidate.produce_specialized_copy(generics)
+
+            # Deduce any remaining generics
+            generics = GenericMapping({}, [])
+            cost2 = partially_specialized.pattern_match_args(args, generics)
+            if cost2 is None:
                 continue
 
             # We've matched the pattern, now we specialize the candidate
-            # TODO: catch these errors
-            specialized = candidate.produce_specialized_copy(generics)
-            all_candidates.append((cost, specialized))
+            specialized = partially_specialized.produce_specialized_copy(generics)
+            unmatched_generics = (
+                specialized.signature.get_generics_taking_part_in_pattern_match()
+            )
+            if len(unmatched_generics) != 0:
+                raise PatternMatchDeductionFailure(
+                    specialized.format_for_output_to_user(),
+                    unmatched_generics.pop().name,
+                )
+
+            all_candidates.append((cost1 + cost2, specialized))
 
         # Find the cheapest valid candidate (doing overload resolution if cost is the same)
         all_candidates.sort(key=lambda item: item[0])
         for _, candidates in groupby(all_candidates, key=lambda item: item[0]):
-            resolved_candidates: list[
-                tuple[FunctionSignature, FunctionDeclaration]
-            ] = []
+            resolved_candidates: list[tuple[FunctionSignature, FunctionDeclaration]] = (
+                []
+            )
             for _, candidate in candidates:
                 try:
                     resolved = self.resolve_function(candidate)
                     if do_specializations_match(
                         resolved.specialization[: len(given_specialization)],
                         given_specialization,
                     ):
@@ -1208,15 +1261,14 @@
             generics = GenericMapping({}, [])
             cost = candidate.pattern_match(specialization, generics)
 
             if cost is None:
                 continue
 
             # We've matched the pattern, now we specialize the candidate
-            # TODO: catch these errors
             specialized = candidate.produce_specialized_copy(generics)
             all_candidates.append((cost, specialized))
 
         # Find the cheapest valid candidate (doing overload resolution if cost is the same)
         all_candidates.sort(key=lambda item: item[0])
         for _, candidates in groupby(all_candidates, key=lambda item: item[0]):
             resolved_candidates: list[tuple[Type, Location]] = []
@@ -1263,17 +1315,17 @@
 
         matched_functions.append(fn_to_add)
         self._newly_added_unresolved_functions.append(fn_to_add)
 
     def add_builtin_type(self, type_to_add: PrimitiveType) -> None:
         typedef = Typedef(
             type_to_add.name,
-            tuple(),
-            tuple(),
-            UnresolvedNamedType(type_to_add.name, tuple()),
+            (),
+            (),
+            UnresolvedNamedType(type_to_add.name, ()),
             BuiltinSourceLocation(),
             uuid4(),
         )
         self._resolved_types[typedef.uuid].append(type_to_add)
         self.add_type(typedef)
 
     def add_type(self, to_add: Typedef) -> None:
@@ -1311,35 +1363,27 @@
                 raise ErrorWithLocationInfo(e.message, typedef.loc, "typedef") from e
 
         for fn in self._newly_added_unresolved_functions:
             if len(fn.generics) != 0 or fn.pack_type_name is not None:
                 continue
 
             try:
-                resolved_specialization = [
-                    self.resolve_specialization_item(item)
-                    for item in fn.signature.expanded_specialization
-                ]
-                resolved_args = [
-                    self.resolve_type(item) for item in fn.signature.arguments
-                ]
-                self.lookup_function(
-                    fn.signature.name, resolved_specialization, resolved_args, True
-                )
+                signature = self.resolve_function(fn)
+                self.add_function_to_codegen(fn, signature)
             except GrapheneError as e:
                 raise ErrorWithLocationInfo(
                     e.message, fn.loc, "function declaration"
                 ) from e
 
         self._newly_added_unresolved_typedefs.clear()
         self._newly_added_unresolved_functions.clear()
 
     def get_next_function_to_codegen(
         self,
-    ) -> Optional[tuple[FunctionDeclaration, FunctionSignature]]:
+    ) -> tuple[FunctionDeclaration, FunctionSignature] | None:
         try:
             return self._remaining_to_codegen.pop()
         except IndexError:
             return None
 
     def get_ir_for_initialization(self) -> list[str]:
         ir: list[str] = []
```

### Comparing `glang-0.2.1/src/glang/codegen/user_facing_errors.py` & `glang-0.4.0/src/glang/codegen/user_facing_errors.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,10 @@
+from collections.abc import Iterable
 from dataclasses import dataclass
-from typing import Iterable, Literal, Optional
+from typing import Literal
 
 
 @dataclass(frozen=True)
 class Location:
     pass
 
 
@@ -39,28 +40,28 @@
 
     @property
     def message(self) -> str:
         return str(self)
 
 
 class ErrorWithLineInfo(ValueError):
-    def __init__(self, message: str, line: int, context: Optional[str] = None) -> None:
+    def __init__(self, message: str, line: int, context: str | None = None) -> None:
         super().__init__(message)
 
         self.line = line
         self.context = context
 
     @property
     def message(self) -> str:
         return str(self)
 
 
 class ErrorWithLocationInfo(ValueError):
     def __init__(
-        self, message: str, location: Location, context: Optional[str] = None
+        self, message: str, location: Location, context: str | None = None
     ) -> None:
         super().__init__(message)
 
         self.loc = location
         self.context = context
 
     @property
@@ -124,15 +125,15 @@
         )
 
 
 class PatternMatchDeductionFailure(GrapheneError):
     def __init__(self, fn_name: str, unmatched_generic: str) -> None:
         super().__init__(
             f"Error: cannot deduce generic type '{unmatched_generic}' "
-            f"in function '{fn_name}', manual specialization is required"
+            f"in '{fn_name}', manual specialization is required"
         )
 
 
 class NonDeterminableSize(GrapheneError):
     def __init__(self, type_name: str) -> None:
         super().__init__(
             f"Error: cannot construct recursive type '{type_name}' since it "
@@ -205,14 +206,53 @@
     ) -> None:
         super().__init__(
             f"Error: {type_name} cannot store value {actual_value}, permitted range"
             f" [{expected_lower}, {expected_upper})"
         )
 
 
+class InvalidFloatLiteralTooLarge(GrapheneError):
+    def __init__(
+        self,
+        type_name: str,
+        actual_value: str,
+        max_representable_with_rounding: int,
+        min_unrepresentable_without_rounding: int,
+    ) -> None:
+        max_str = str(max_representable_with_rounding)
+        min_str = str(min_unrepresentable_without_rounding)
+        assert len(max_str) == len(min_str)
+
+        first_diff = next(
+            i
+            for i, (char1, char2) in enumerate(zip(max_str, min_str, strict=True))
+            if char1 != char2
+        )
+
+        upper_truncated = f"{max_str[0]}.{max_str[1:first_diff+1]}e+{len(max_str)-1}"
+
+        super().__init__(
+            f"Error: '{type_name}' cannot represent '{actual_value}' since it is "
+            "too large and would be truncated to +infty. Only values below "
+            f"{upper_truncated} can be represented."
+        )
+
+
+class InvalidFloatLiteralPrecision(GrapheneError):
+    def __init__(
+        self,
+        type_name: str,
+        actual_value: str,
+    ) -> None:
+        super().__init__(
+            f"Error: '{type_name}' cannot represent '{actual_value}' since there "
+            f"is insufficient precision for a normalized representation."
+        )
+
+
 class ArrayIndexCount(GrapheneError):
     def __init__(self, type_name: str, actual: int, expected: int) -> None:
         super().__init__(
             f"Error: array type '{type_name}' expects {expected} indices but received {actual}"
         )
 
 
@@ -331,22 +371,14 @@
     def __init__(self, struct_type: str, init_list_name: str) -> None:
         super(GrapheneError, self).__init__(
             f"Error: initializer list of the form '{init_list_name}' cannot be "
             f"converted to '{struct_type}'"
         )
 
 
-class InvalidInitializerListDeduction(TypeCheckerError):
-    def __init__(self, init_list_name: str) -> None:
-        super(GrapheneError, self).__init__(
-            "Error: cannot deduce the destination type for initializer list "
-            f"'{init_list_name}' without a strongly typed context"
-        )
-
-
 class CannotAssignToInitializerList(GrapheneError):
     def __init__(self) -> None:
         super().__init__("Error: cannot assign to an initializer list")
 
 
 class FileDoesNotExistException(GrapheneError):
     def __init__(self, file_name: str) -> None:
@@ -466,7 +498,12 @@
         # TODO would be nice if we could print the struct's name (if available).
         super().__init__(
             f"Error: redeclaration of struct member `{name}` (previous "
             f"declaration `{name}: {previous_type}`)",
             line,
             "struct definition",
         )
+
+
+class NotInLoopStatementError(GrapheneError):
+    def __init__(self, statement: str) -> None:
+        super().__init__(f"'{statement}' is not inside a loop")
```

### Comparing `glang-0.2.1/src/glang/lib/std/algorithms.c3` & `glang-0.4.0/src/glang/lib/std/algorithms.c3`

 * *Files identical despite different names*

### Comparing `glang-0.2.1/src/glang/lib/std/arithmetic.c3` & `glang-0.4.0/src/glang/lib/std/arithmetic.c3`

 * *Files 24% similar despite different names*

```diff
@@ -1,32 +1,50 @@
 @require_once "assignments.c3"
 @require_once "logical.c3"
 @require_once "type_traits.c3"
 
-typedef [U, V] CommonArithmeticType: TypeIf<U, Both<IsIntegral<U>, IsIntegral<V>>>
-typedef CommonArithmeticType<i8, i16> : i16
-typedef CommonArithmeticType<i8, i32> : i32
-typedef CommonArithmeticType<i8, i64> : i64
-typedef CommonArithmeticType<i8, i128> : i128
-typedef CommonArithmeticType<i16, i32> : i32
-typedef CommonArithmeticType<i16, i64> : i64
+typedef [U, V] AreCompatibleArithmeticTypes :
+    Either<
+        Both<IsIntegral<U>, IsIntegral<V>>,
+        Both<IsFloating<U>, IsFloating<V>>,
+    >
+
+typedef [U, V] CommonArithmeticType: TypeIf<U, AreCompatibleArithmeticTypes<U, V>>
+
+typedef CommonArithmeticType<i8, i16>   : i16
+typedef CommonArithmeticType<i8, i32>   : i32
+typedef CommonArithmeticType<i8, i64>   : i64
+typedef CommonArithmeticType<i8, i128>  : i128
+typedef CommonArithmeticType<i16, i32>  : i32
+typedef CommonArithmeticType<i16, i64>  : i64
 typedef CommonArithmeticType<i16, i128> : i128
-typedef CommonArithmeticType<i32, i64> : i64
+typedef CommonArithmeticType<i32, i64>  : i64
 typedef CommonArithmeticType<i32, i128> : i128
 typedef CommonArithmeticType<i64, i128> : i128
 
-typedef [U, V] ArithmeticCompareResult : TypeIf<bool, Both<IsIntegral<U>, IsIntegral<V>>>
-typedef [T] RegisterHasTrivialAssignments<Override<T>> : TypeIf<TrueType, IsIntegral<T>>
+typedef CommonArithmeticType<f16, f32>  : f32
+typedef CommonArithmeticType<f16, f64>  : f64
+typedef CommonArithmeticType<f16, f128> : f128
+typedef CommonArithmeticType<f32, f64>  : f64
+typedef CommonArithmeticType<f32, f128> : f128
+typedef CommonArithmeticType<f64, f128> : f128
+
+typedef [U, V] ArithmeticCompareResult : TypeIf<bool, AreCompatibleArithmeticTypes<U, V>>
+typedef [T] RegisterHasTrivialAssignments<Override<T>> : TypeIf<TrueType, IsArithmetic<T>>
 
-@operator [T] + : (value: T) -> TypeIf<T, IsIntegral<T>> = { return value; }
+@operator [T] + : (value: T) -> TypeIf<T, IsArithmetic<T>> = { return value; }
 
 @operator [T] - : (value: T) -> TypeIf<T, IsIntegral<T>> = {
     return __builtin_minus(value);
 }
 
+@operator [T] - : (value: T) -> TypeIf<T, IsFloating<T>> = {
+    return __builtin_fminus(value);
+}
+
 @operator [U, V] + : (lhs: U, rhs : V) -> CommonArithmeticType<U, V> = {
     let lhs_widen: CommonArithmeticType<U, V> = lhs;
     let rhs_widen: CommonArithmeticType<U, V> = rhs;
     return __builtin_add(lhs_widen, rhs_widen);
 }
 
 @operator [U, V] - : (lhs: U, rhs : V) -> CommonArithmeticType<U, V> = {
```

### Comparing `glang-0.2.1/src/glang/lib/std/assignments.c3` & `glang-0.4.0/src/glang/lib/std/assignments.c3`

 * *Files identical despite different names*

### Comparing `glang-0.2.1/src/glang/lib/std/fcntl.c3` & `glang-0.4.0/src/glang/lib/std/fcntl.c3`

 * *Files identical despite different names*

### Comparing `glang-0.2.1/src/glang/lib/std/format.c3` & `glang-0.4.0/src/glang/lib/std/format.c3`

 * *Files 6% similar despite different names*

```diff
@@ -1,41 +1,39 @@
 @require_once "io.c3"
 @require_once "string.c3"
 @require_once "type_traits.c3"
 @require_once "util.c3"
 
-function [IO] write : (io : IO mut&, char : UTF32Codepoint) -> TypeIf<StringView, IsStreamableTextIO<IO>> = {
-    return io:write_char(char.codepoint);
+function [IO] write : (io : IO mut&, char : UTF32Codepoint) -> TypeIf<void, IsStreamableTextIO<IO>> = {
+    io:write_char(char.codepoint);
 }
 
-function [IO, @Len] write : (io : IO mut&, string : u8[@Len]&) -> TypeIf<StringView, IsStreamableTextIO<IO>> = {
-    return io:write(sv(&string));
+function [IO, @Len] write : (io : IO mut&, string : u8[@Len]&) -> TypeIf<void, IsStreamableTextIO<IO>> = {
+    io:write(sv(&string));
 }
 
-function [IO] write : (io : IO mut&, string : StringView) -> TypeIf<StringView, IsStreamableTextIO<IO>> = {
+function [IO] write : (io : IO mut&, string : StringView) -> TypeIf<void, IsStreamableTextIO<IO>> = {
     let buffer : Span<u8> = io:request_buffer(string:length());
 
-    // TODO: remave this assumption
+    // TODO: remove this assumption
     // TODO: maybe stream large strings directly
     runtime_assert(buffer.length == string:length());
     for index in range(string:length()) {
         buffer.data[index] = string.buffer.data[index];
     }
     io:consume_length(buffer.length);
-    return make<StringView>(buffer:to_view());
 }
 
-function [IO] write : (io : IO mut&, number : isize) -> TypeIf<StringView, IsStreamableTextIO<IO>> = {
+function [IO] write : (io : IO mut&, number : isize) -> TypeIf<void, IsStreamableTextIO<IO>> = {
     let buffer : Span<u8> = io:request_buffer(21); // len(INT_64_MIN) == 21
     if number == 0 {
         buffer.data[0] = "0"[0];
         io:consume_length(1);
 
-        // BUG: WE CAN RETURN VOID??
-        return {make<View<u8>>(&buffer.data, 1)};
+        return;
     }
 
     let is_negative : bool = number < 0;
     mut current_number : isize = number;
     mut length : isize = 0;
     while current_number != 0 {
         let next_digit: u8 = as_logical(__builtin_narrow<i8>(abs(current_number % 10) + as_arithmetic("0"[0])));
@@ -50,24 +48,23 @@
         buffer.data[length] = "-"[0];
         length += 1;
     }
 
     let result : Span<u8> = make<Span<u8>>(&mut buffer.data, length);
     result:reverse();
     io:consume_length(length);
-    return {result:to_view()};
 }
 
-function [IO] write : (io : IO mut&, number : u32) -> TypeIf<StringView, IsStreamableTextIO<IO>> = {
+function [IO] write : (io : IO mut&, number : u32) -> TypeIf<void, IsStreamableTextIO<IO>> = {
     // TODO: support u64
     let buffer : Span<u8> = io:request_buffer(8); // 4 bytes
 
     if number == 0x00 {
         buffer.data[0] = "0"[0];
-        return {make<View<u8>>(&buffer.data, 1)};
+        return;
     }
 
     let lookup_table : u8[16] = {
         "0"[0], "1"[0], "2"[0], "3"[0], "4"[0], "5"[0], "6"[0], "7"[0], "8"[0], "9"[0], "A"[0], "B"[0], "C"[0], "D"[0], "E"[0], "F"[0]
     };
 
     mut remaining_number : u32 = number;
@@ -78,30 +75,28 @@
         remaining_number >>= 4;
         length += 1;
     }
 
     let result : Span<u8> = buffer:slice_to(length);
     result:reverse();
     io:consume_length(length);
-    return {result:to_view()};
 }
 
-function [IO] write : (io : IO mut&, value : bool) -> TypeIf<StringView, IsStreamableTextIO<IO>> = {
+function [IO] write : (io : IO mut&, value : bool) -> TypeIf<void, IsStreamableTextIO<IO>> = {
     if value {
-        return io:write(sv("true"));
+        io:write(sv("true"));
     } else {
-        return io:write(sv("false"));
+        io:write(sv("false"));
     }
 }
 
-function [IO] write_char : (io : IO mut&, char : u8) -> TypeIf<StringView, IsStreamableTextIO<IO>> = {
+function [IO] write_char : (io : IO mut&, char : u8) -> TypeIf<void, IsStreamableTextIO<IO>> = {
     let buffer : Span<u8> = io:request_buffer(1);
     buffer.data[0] = char;
     io:consume_length(1);
-    return make<StringView>(buffer:to_view());
 }
 
 function [Args...] print : (args : Args...) -> void = {
     mut io : BufferedFile = get_stdout_io();
     io:print_impl(args...);
     io:write(sv("\n"));
     io:flush();
```

### Comparing `glang-0.2.1/src/glang/lib/std/io.c3` & `glang-0.4.0/src/glang/lib/std/io.c3`

 * *Files 19% similar despite different names*

```diff
@@ -1,69 +1,90 @@
 @require_once "algorithms.c3"
 @require_once "arithmetic.c3"
 @require_once "assert.c3"
 @require_once "fcntl.c3"
 @require_once "iterators.c3"
 @require_once "math.c3"
 @require_once "string.c3"
+@require_once "sys/mman.c3"
+@require_once "sys/stat.c3"
 @require_once "sys/uio.c3"
 @require_once "syscalls.c3"
 @require_once "wrappers.c3"
 
-typedef UnbufferedFile : { fd : int }
+typedef File : { fd : int }
+typedef MappedFile : { underlying : File, buffer : View<u8> }
 
-function write : (file : UnbufferedFile&, buffer : View<u8>) -> void = {
+function write : ( file : File&, buffer : View<u8> ) -> void = {
     sys_write(file.fd, &buffer.data, buffer.length);
 }
 
-function read : (file : UnbufferedFile&, buffer: Span<u8>) -> View<u8> = {
+function read : ( file : File&, buffer: Span<u8> ) -> View<u8> = {
     let bytes_read: isize = sys_read(file.fd, &mut buffer.data, buffer.length);
     return {&buffer.data, bytes_read};
 }
 
-function close : (file : UnbufferedFile&) -> void = {
+function close : ( file : File& ) -> void = {
     if file.fd >= 3 {
         // Don't close std{in,out,err}
-        runtime_assert(sys_close(file.fd) > 0);
+        runtime_assert(sys_close(file.fd) == 0);
     }
 }
 
-function open : (file_path: CString, mode: u32) -> UnbufferedFile = {
-    // BUG: try removing the '&' here... the error message is nonsense
+function open : ( file_path: CString, mode: u32 ) -> Optional<File> = {
     let fd : int = sys_open(&file_path.data, mode, 0x00);
-    runtime_assert(fd > 0);
-    return {fd};
+    if fd < 0 {
+        return make<Optional<File>>();
+    }
+    return make<Optional<File>>({fd});
+}
+
+function read : ( file : File& ) -> Optional<MappedFile> = {
+    let stat : Optional<stat_t> = stat( file.fd );
+    if !stat:has_value() {
+        return make<Optional<MappedFile>>();
+    }
+    let size : isize = stat:data().st_size;
+
+    let buffer : iptr = mmap(0, size, SYS_PROT_READ(), SYS_MAP_PRIVATE(), file.fd, 0);
+    return make<Optional<MappedFile>>({
+        file,
+        { &addr_to_heap_array<u8>(buffer), size }
+    });
 }
 
+function unmap : ( file : MappedFile& ) -> void = {
+    munmap(ref_to_addr(&file.buffer.data), file.buffer.length);
+}
 
 typedef RegisterIsStreamableTextIO<Override<BufferedFile>> : TrueType
 typedef BufferedFile : {
-    underlying_file : UnbufferedFile,
+    underlying : File,
     buffer : u8[1024],
     buffer_pointer : isize,
 }
 
 function get_stdout_io : () -> BufferedFile = {
     mut result : BufferedFile;
-    result.underlying_file = {1 /* stdout */};
+    result.underlying = {1 /* stdout */};
     result.buffer_pointer = 0;
     return result;
 }
 
 function flush : (io : BufferedFile mut&) -> void = {
     let data_to_write : View<u8> = {&io.buffer, io.buffer_pointer};
     let string_to_write : StringView = {data_to_write};
     // UFCS where `write` takes a `T&` and we have a `T mut&`
-    (&io.underlying_file):write(data_to_write);
+    io.underlying:write(data_to_write);
     io.buffer_pointer = 0;
 }
 
 function close : (io : BufferedFile mut&) -> void = {
     io:flush();
-    (&io.underlying_file):close();
+    io.underlying:close();
 }
 
 function request_buffer : (io : BufferedFile mut&, length : isize) -> Span<u8> = {
     // TODO: this syntax for calling const length is kinda dumb
     runtime_assert(length <= io.buffer:length());
 
     if io.buffer_pointer + length < io.buffer:length() {
@@ -77,18 +98,14 @@
     return {&mut io.buffer, length};
 }
 
 function consume_length : (io : BufferedFile mut&, length : isize) -> void = {
     io.buffer_pointer += length;
 }
 
-function read : (file : BufferedFile&, buffer: Span<u8>) -> View<u8> = {
-    return file.underlying_file:read(buffer);
-}
-
 function EOF : () -> int = {
     // EOF - end-of-file return value
     // An integer constant expression with type int and a negative value.
     return -1;
 }
 
 function puts : (str : StringView) -> int = {
```

### Comparing `glang-0.2.1/src/glang/lib/std/iterators.c3` & `glang-0.4.0/src/glang/lib/std/iterators.c3`

 * *Files 2% similar despite different names*

```diff
@@ -57,15 +57,19 @@
 @implicit [T] get_next : (range: Range<T> mut&) -> T = {
     let next : T = range.lower;
     range.lower += range.step;
     return next;
 }
 
 @implicit [T] has_next : (range : Range<T> mut&) -> bool = {
-    return range.lower < range.upper;
+    if range.step > 0 {
+        return range.lower < range.upper;
+    } else {
+        return range.lower > range.upper;
+    }
 }
 
 // ContiguousContainerIter
 // TODO: NO ITERATOR FUNCTIONS ARE CONSTANT!!
 //   This hurts the const-correctness of functions taking iterators directly
 @implicit [T, R] has_next : (iter : ContiguousContainerIter<T, R> mut&) -> bool = {
     return iter.current_index < iter.container:length();
```

### Comparing `glang-0.2.1/src/glang/lib/std/json.c3` & `glang-0.4.0/src/glang/lib/std/json.c3`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,14 @@
     if cursor.iter:has_next() {
         return make<Optional<u8>>(cursor.iter:__builtin_get_next());
     }
 
     return make<Optional<u8>>();
 }
 
-function position : (cursor : Cursor mut&) -> isize = { return (&cursor):position();}
 function position : (cursor : Cursor&) -> isize = {
     // Looking into the iterator like this is sorta cursed
     return cursor.iter.current_index;
 }
 
 function slice_between : (cursor: Cursor&, start_offset : iptr, end_offset : isize) -> StringView = {
     // Looking into the iterator like this is sorta cursed
@@ -270,15 +269,15 @@
     mut string : Vector<u8> = make<Vector<u8>>(&mut cursor.allocator);
 
     while cursor:has_next() {
         if !in_escape_seq and cursor:eat(char("\"")) {
             mut node : JSON_Node = new_json_node(/* string */ 3, &mut cursor.allocator);
 
             // TODO: https://github.com/DaveDuck321/GrapheneLang/issues/124
-            let value: StringView = {(&string):view()};
+            let value: StringView = {string:view()};
             node.value = make<Optional<StringView>>(value);
 
             return make<Optional<JSON_Node>>(node);
         }
 
         let char_opt : Optional<u8> = cursor:next();
         runtime_assert(char_opt:has_value());
@@ -354,15 +353,15 @@
     let end_pos : isize = cursor:position();
 
     if !is_valid {
         return make<Optional<JSON_Node>>();
     }
 
     mut node : JSON_Node = new_json_node(/* string */ 4, &mut cursor.allocator);
-    node.value = make<Optional<StringView>>((&cursor):slice_between(start_pos, end_pos));
+    node.value = make<Optional<StringView>>(cursor:slice_between(start_pos, end_pos));
 
     return make<Optional<JSON_Node>>(node);
 }
 
 // TODO this and write below should be the only public functions.
 function json_parse : (source : StringView) -> Optional<JSON_Node> = {
     // FIXME memory safety, memory leaks.
@@ -383,15 +382,15 @@
     if !cursor:has_next() {
         return result;
     }
 
     return make<Optional<JSON_Node>>();
 }
 
-function [IO] write : (io : IO mut&, node : JSON_Node) -> TypeIf<StringView, IsStreamableTextIO<IO>> = {
+function [IO] write : (io : IO mut&, node : JSON_Node) -> TypeIf<void, IsStreamableTextIO<IO>> = {
     // null
     if node.type == 0 {
         return io:write(sv("null"));
     }
 
     // true
     if node.type == 1 {
@@ -413,15 +412,15 @@
             buffer.data[0] = char("\"");
             buffer.data[buffer.length - 1] = char("\"");
             for i in range(string:length()) {
                 buffer.data[i + 1] = string.buffer.data[i];
             }
 
             io:consume_length(buffer.length);
-            return {buffer:to_view()};
+            return;
         }
     }
 
     // number (which we can just echo back!)
     if node.type == 4 {
         // Allowed to fail.
         if node.value:has_value() {
@@ -467,9 +466,9 @@
             }
             flag ^= true;
         }
 
         return io:write(sv("}"));
     }
 
-    return io:write(sv("<invalid node>"));
+    io:write(sv("<invalid node>"));
 }
```

### Comparing `glang-0.2.1/src/glang/lib/std/logical.c3` & `glang-0.4.0/src/glang/lib/std/logical.c3`

 * *Files identical despite different names*

### Comparing `glang-0.2.1/src/glang/lib/std/memory.c3` & `glang-0.4.0/src/glang/lib/std/memory.c3`

 * *Files identical despite different names*

### Comparing `glang-0.2.1/src/glang/lib/std/span.c3` & `glang-0.4.0/src/glang/lib/std/span.c3`

 * *Files identical despite different names*

### Comparing `glang-0.2.1/src/glang/lib/std/string.c3` & `glang-0.4.0/src/glang/lib/std/string.c3`

 * *Files 10% similar despite different names*

```diff
@@ -27,25 +27,35 @@
     return { make<View<u8>>(&cstr.data, cstr:length()) };
 }
 
 function length : (sv : StringView&) -> isize = {
     return sv.buffer:length();
 }
 
-function length : (sv : StringView mut&) -> isize = { return (&sv):length(); }
-
 // TODO: return `UTF32Codepoint` here
 function get_iter : (sv : StringView&) -> ContiguousContainerIter<View<u8>&, u8&> = {
     return sv.buffer:get_iter();
 }
 
 @operator == : (lhs : StringView, rhs : StringView) -> bool = {
     return lhs.buffer == rhs.buffer;
 }
 
+function slice_to : (sv : StringView&, end : isize) -> StringView = {
+    return { sv.buffer:slice_to(end) };
+}
+
+function slice_from : (sv : StringView&, start : isize) -> StringView = {
+    return { sv.buffer:slice_from(start) };
+}
+
+function slice_between : (sv : StringView&, start : isize, end : isize) -> StringView = {
+    return { sv.buffer:slice_between(start, end) };
+}
+
 // CString
 function length : (str: CString&) -> isize = {
     mut len : isize = 0;
     while str.data[len] != char("\0") {
         len = len + 1;
     }
     return len;
@@ -108,7 +118,19 @@
     return false;
 }
 
 function char : (literal : u8[1]&) -> u8 = {
     // TODO: add char literals
     return literal[0];
 }
+
+function[Int] unstringify : (view : StringView) -> TypeIf<Int, IsIntegral<Int>> = {
+    mut result : Int = 0;
+
+    for char in view:get_iter() {
+        runtime_assert(ascii_is_digit(char));
+        result *= 10;
+        result += as_arithmetic(char) - as_arithmetic(char("0"));
+    }
+
+    return result;
+}
```

### Comparing `glang-0.2.1/src/glang/lib/std/type_traits.c3` & `glang-0.4.0/src/glang/lib/std/type_traits.c3`

 * *Files 8% similar despite different names*

```diff
@@ -44,14 +44,22 @@
 typedef [T] IsIntegral : FalseType
 typedef IsIntegral<i8> : TrueType
 typedef IsIntegral<i16> : TrueType
 typedef IsIntegral<i32> : TrueType
 typedef IsIntegral<i64> : TrueType
 typedef IsIntegral<i128> : TrueType
 
+typedef [T] IsFloating : FalseType
+typedef IsFloating<f16> : TrueType
+typedef IsFloating<f32> : TrueType
+typedef IsFloating<f64> : TrueType
+typedef IsFloating<f128> : TrueType
+
+typedef [T] IsArithmetic : Either<IsIntegral<T>, IsFloating<T>>
+
 typedef [T] IsLogical : FalseType
 typedef IsLogical<bool> : TrueType
 typedef IsLogical<u8> : TrueType
 typedef IsLogical<u16> : TrueType
 typedef IsLogical<u32> : TrueType
 typedef IsLogical<u64> : TrueType
 typedef IsLogical<u128> : TrueType
```

### Comparing `glang-0.2.1/src/glang/lib/std/util.c3` & `glang-0.4.0/src/glang/lib/std/util.c3`

 * *Files 5% similar despite different names*

```diff
@@ -41,14 +41,20 @@
 
 function [T, AddrT] addr_to_mut_heap_array : (address : AddrT)
     -> TypeIf<T[mut&], AreEquivalent<AddrT, iptr>> =
 {
     return &mut __builtin_int_to_ptr<T[mut&]>(address);
 }
 
+function [TRef, BRef] reinterpret_addr : (base : BRef)
+    -> TypeIf<TRef, Both<IsRef<TRef>, IsRef<BRef>>> =
+{
+    return &__builtin_int_to_ptr<TRef>(__builtin_ptr_to_int(&base));
+}
+
 function as_arithmetic : (value : u8)   -> i8   = { return __builtin_bitcast<i8>(value); }
 function as_arithmetic : (value : u16)  -> i16  = { return __builtin_bitcast<i16>(value); }
 function as_arithmetic : (value : u32)  -> i32  = { return __builtin_bitcast<i32>(value); }
 function as_arithmetic : (value : u64)  -> i64  = { return __builtin_bitcast<i64>(value); }
 function as_arithmetic : (value : u128) -> i128 = { return __builtin_bitcast<i128>(value); }
 
 function as_logical : (value : i8)   -> u8   = { return __builtin_bitcast<u8>(value); }
```

### Comparing `glang-0.2.1/src/glang/lib/std/vector.c3` & `glang-0.4.0/src/glang/lib/std/vector.c3`

 * *Files 3% similar despite different names*

```diff
@@ -85,15 +85,15 @@
 }
 
 function [T] capacity : (self : Vector<T> mut&) -> isize = {
     return self.memory.length;
 }
 
 function [T] data : (self : Vector<T> mut&) -> Span<T> = {
-    return (&self.memory):slice_to(self.length);
+    return self.memory:slice_to(self.length);
 }
 
 function [T] data : (self : Vector<T>&) -> Span<T> = {
     // TODO: we can extract the mutable data from a constant vector... Do I like this?
     return self.memory:slice_to(self.length);
 }
 
@@ -105,27 +105,18 @@
 
 function [T] view : (self : Vector<T>&) -> View<T> = {
     // TODO: take value types as const reference
     let data : Span<T> = self:data();
     return data:to_view();
 }
 
-function [T] get_iter : (vec : Vector<T> mut&) -> ContiguousContainerIter<Vector<T>&, T mut&> = {
-    return (&vec):get_iter();
-}
-
 function [T] get_iter : (vec : Vector<T>&) -> ContiguousContainerIter<Vector<T>&, T mut&> = {
     return { .container = &vec, .current_index = 0 };
 }
 
-// TODO: remove this... maybe use const value semantics?
-function [T] get_citer : (vec : Vector<T> mut&) -> ContiguousContainerIter<Vector<T>&, T&> = {
-    return (&vec):get_iter();
-}
-
 function [T] get_citer : (vec : Vector<T>&) -> ContiguousContainerIter<Vector<T>&, T&> = {
     return { .container = &vec, .current_index = 0 };
 }
 
 function [T] clear : (self : Vector<T> mut&) -> void = {
     // TODO: destructor support (if we add destructors)
     self.length = 0;
```

### Comparing `glang-0.2.1/src/glang/lib/std/wrappers.c3` & `glang-0.4.0/src/glang/lib/std/wrappers.c3`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 @require_once "type_traits.c3"
 
 typedef [T] Ptr : { data : T& }
+typedef [T] MutPtr : { data : T mut& }
 typedef [T] MaybeNullPtr : Optional<Ptr<T>>
 
 // Maybe FIXME: this isn't really ergonomic, this SFINAE avoids &/ mut& code duplication
 typedef [T] Optional : { _value : TypeIf<T, Not<IsRef<T>>>, _has_value : bool}
 typedef [T] Optional<T&> : { _ptr : iptr } // Nullptr optimization
 typedef [T] Optional<T mut&> : { _ptr : iptr } // Duplicated
 
@@ -13,14 +14,23 @@
     return &self.data;
 }
 
 function [T] data : (self : Ptr<T> mut&) -> T& = {
     return &self.data;
 }
 
+// MutPtr
+function [T] data : (self : MutPtr<T>&) -> T mut& = {
+    return &mut self.data;
+}
+
+function [T] data : (self : MutPtr<T> mut&) -> T mut& = {
+    return &mut self.data;
+}
+
 // Generic Optional
 function [T] make<Optional<T>> : () -> Optional<T> = {
     mut result : Optional<T>;
     result._has_value = false;
     return result;
 }
 
@@ -51,32 +61,44 @@
     return &mut self._value;
 }
 
 function [T] has_value : (self : Optional<T>&) -> bool = {
     return self._has_value;
 }
 
+function [IO, T] write : (
+    io : IO mut&, optional : Optional<T>
+) -> TypeIf<void, IsStreamableTextIO<IO>> = {
+    if optional:has_value() {
+        return io:write(optional:data());
+    }
+
+    io:write("<empty>");
+}
+
+
 // Optional<T&>
-function [T] make<T&> : (value : T&) -> Optional<T&> = {
-    return { ref_to_addr(&value) };
+function [T] make<Optional<T&>> : () -> Optional<T&> = {
+    return { 0 };
 }
 
-function [T] make<T&> : (value : T&) -> Optional<T&> = {
+function [T] make<Optional<T&>> : (value : T&) -> Optional<T&> = {
     return { ref_to_addr(&value) };
 }
 
 function [T] store : (self : Optional<T&> mut&, value : T&) -> void = {
     self._ptr = ref_to_addr(&value);
 }
 
 function [T] erase : (self : Optional<T&> mut&) -> void = {
     self._ptr = 0;
 }
 
 function [T] data : (self : Optional<T&>&) -> T& = {
+    runtime_assert(self:has_value());
     return &addr_to_ref<T>(self._ptr);
 }
 
 function [T] data : (self : Optional<T&> mut&) -> T& = {
     return &addr_to_ref<T>(self._ptr);
 }
 
@@ -88,30 +110,34 @@
 function [T] has_value : (self : Optional<T&> mut&) -> bool = {
     return self._ptr != 0;
 }
 
 
 // HUGE DUPLICATION FOR MUTABLE REFERENCE
 // Optional<T&>
-function [T] make<T&> : (value : T mut&) -> Optional<T mut&> = {
-    return { ref_to_addr(&value) };
+function [T] make<Optional<T mut&>> : () -> Optional<T mut&> = {
+    return { 0 };
 }
 
-function [T] make<T&> : (value : T mut&) -> Optional<T mut&> = {
+function [T] make<Optional<T mut&>> : (value : T mut&) -> Optional<T mut&> = {
     return { ref_to_addr(&value) };
 }
 
 function [T] store : (self : Optional<T mut&> mut&, value : T mut&) -> void = {
     self._ptr = ref_to_addr(&value);
 }
 
 function [T] erase : (self : Optional<T mut&> mut&) -> void = {
     self._ptr = 0;
 }
 
+function [T] data : (self : Optional<T mut&>&) -> T mut& = {
+    return &mut addr_to_mut_ref<T>(self._ptr);
+}
+
 function [T] data : (self : Optional<T mut&> mut&) -> T mut& = {
     return &mut addr_to_mut_ref<T>(self._ptr);
 }
 
 function [T] has_value : (self : Optional<T mut&>&) -> bool = {
     return self._ptr != 0;
 }
```

### Comparing `glang-0.2.1/src/glang/lib/std/aarch64_linux/runtime.S` & `glang-0.4.0/src/glang/lib/std/aarch64_linux/runtime.S`

 * *Files identical despite different names*

### Comparing `glang-0.2.1/src/glang/lib/std/aarch64_linux/syscalls.c3` & `glang-0.4.0/src/glang/lib/std/aarch64_linux/syscalls.c3`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 @require_once "../util.c3"
 @require_once "../sys/uio.c3"
 @require_once "../sys/types.c3"
 @require_once "../fcntl.c3"
+@require_once "sys/kstat.c3"
 
 foreign _syscall_0 : (syscall_number: i32) -> i64
 foreign _syscall_1 : (a: i64, syscall_number: i32) -> i64
 foreign _syscall_2 : (a: i64, b: i64, syscall_number: i32) -> i64
 foreign _syscall_3 : (a: i64, b: i64, c: i64, syscall_number: i32) -> i64
 foreign _syscall_4 : (a: i64, b: i64, c: i64, d: i64, syscall_number: i32) -> i64
 foreign _syscall_6 : (a: i64, b: i64, c: i64, d: i64, e: i64, f: i64, syscall_number: i32) -> i64
@@ -33,14 +34,19 @@
     return sys_openat(AT_FDCWD(), &filename, flags, mode);
 }
 
 function sys_close : (fd : int) -> int = {
     return Narrow<int>(_syscall_1(fd, /* close */ 57));
 }
 
+function sys_fstat : (fd: int, out : stat_t mut&) -> int = {
+    let buf_addr : iptr = __builtin_ptr_to_int(&mut out);
+    return Narrow<int>(_syscall_2(fd, buf_addr, /* fstat */ 80));
+}
+
 function sys_writev : (fd: int, iov: iovec[&], iovcnt: int) -> isize = {
     let iov_addr : iptr = __builtin_ptr_to_int(iov);
 
     return _syscall_3(fd, iov_addr, iovcnt, /* writev */ 66);
 }
 
 function sys_mmap : (
```

### Comparing `glang-0.2.1/src/glang/lib/std/arm_linux/runtime.S` & `glang-0.4.0/src/glang/lib/std/arm_linux/runtime.S`

 * *Files identical despite different names*

### Comparing `glang-0.2.1/src/glang/lib/std/sys/mman.c3` & `glang-0.4.0/src/glang/lib/std/sys/mman.c3`

 * *Files identical despite different names*

### Comparing `glang-0.2.1/src/glang/lib/std/x86_64_linux/runtime.S` & `glang-0.4.0/src/glang/lib/std/x86_64_linux/runtime.S`

 * *Files identical despite different names*

### Comparing `glang-0.2.1/src/glang/lib/std/x86_64_linux/syscalls.c3` & `glang-0.4.0/src/glang/lib/std/x86_64_linux/syscalls.c3`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 @require_once "../util.c3"
 @require_once "../sys/mman.c3"
 @require_once "../sys/uio.c3"
 @require_once "../sys/types.c3"
+@require_once "sys/kstat.c3"
 
 foreign _syscall_0 : (syscall_number: i64) -> i64
 foreign _syscall_1 : (a: i64, syscall_number: i64) -> i64
 foreign _syscall_2 : (a: i64, b: i64, syscall_number: i64) -> i64
 foreign _syscall_3 : (a: i64, b: i64, c: i64, syscall_number: i64) -> i64
 foreign _syscall_6 : (a: i64, b: i64, c: i64, d: i64, e: i64, f: i64, syscall_number: i64) -> i64
 
@@ -22,14 +23,19 @@
 function sys_open : (filename: u8[&], flags: u32, mode: u32) -> int = {
     let filename_addr : iptr = __builtin_ptr_to_int(filename);
     let result : i64 =  _syscall_3(filename_addr, as_arithmetic(flags),
                                      as_arithmetic(mode), /* open */ 2);
     return Narrow<int>(result);
 }
 
+function sys_fstat : (fd: int, out : stat_t mut&) -> int = {
+    let buf_addr : iptr = __builtin_ptr_to_int(&mut out);
+    return Narrow<int>(_syscall_2(fd, buf_addr, /* fstat */ 5));
+}
+
 function sys_close : (fd : int) -> int = {
     return Narrow<int>(_syscall_1(fd, /* close */ 3));
 }
 
 function sys_writev : (fd: int, iov: iovec[&], iovcnt: int) -> isize = {
     let iov_addr : iptr = __builtin_ptr_to_int(iov);
     return _syscall_3(fd, iov_addr, iovcnt, /* writev */ 20);
```

### Comparing `glang-0.2.1/src/glang/parser/file_info.c3` & `glang-0.4.0/src/glang/parser/file_info.c3`

 * *Files identical despite different names*

### Comparing `glang-0.2.1/src/glang/parser/lexer_parser.py` & `glang-0.4.0/src/glang/parser/lexer_parser.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 import json
 from dataclasses import dataclass
 from pathlib import Path
-from typing import Any, Optional
-from typing import Type as PyType
-from typing import TypeVar
+from typing import Any, TypeVar
 
-from .self_hosted_parser import parse
+from glang.parser.self_hosted_parser import parse
 
 # Mirrors the data structures in `syntax_tree.c3`
 # TODO: python bindings to automate this :-D
 
 
 @dataclass
 class FilePosition:
@@ -197,30 +195,40 @@
     variable: str
     iterator: Expression
     scope: Scope
 
 
 @dataclass
 class Return(LineOfCode):
-    expression: Optional[Expression]
+    expression: Expression | None
+
+
+@dataclass
+class Break(LineOfCode):
+    pass
+
+
+@dataclass
+class Continue(LineOfCode):
+    pass
 
 
 @dataclass
 class Assignment(LineOfCode):
     lhs: Expression
     operator: str
     rhs: Expression
 
 
 @dataclass
 class VariableDeclaration(LineOfCode):
     is_mut: bool
     variable: str
     type_: Type
-    expression: Optional[Expression]
+    expression: Expression | None
 
 
 @dataclass
 class OperatorUse(Expression):
     name: str
     lhs: Expression
     rhs: Expression
@@ -326,21 +334,21 @@
     expression: Expression
     member: str
 
 
 class Interpreter:
     T = TypeVar("T")
 
-    def parse(self, thing: ParsedNode, ret_type: PyType[T] | None) -> T:
+    def parse(self, thing: ParsedNode, ret_type: type[T] | None) -> T:
         for fn_type in type(thing).mro():
             if hasattr(self, fn_type.__name__):
                 fn = getattr(self, fn_type.__name__)
                 break
         else:
-            assert False, f"{self} could not dispatch '{thing}'"
+            raise AssertionError(f"{self} could not dispatch '{thing}'")
 
         result = fn(thing)
         if ret_type is not None:
             assert isinstance(result, ret_type)
 
         return result
```

### Comparing `glang-0.2.1/src/glang/parser/parser.c3` & `glang-0.4.0/src/glang/parser/parser.c3`

 * *Files 2% similar despite different names*

```diff
@@ -9,57 +9,51 @@
 
 typedef Cursor : {
     program : StringView,
     position : isize,
     allocator: Allocator mut&, // TODO: this should be somewhere else?
 }
 
-// TODO: should be `Cursor&`
-function get_sv : (cursor : Cursor mut&, slice : ProgramSlice) -> StringView = {
+function get_sv : (cursor : Cursor&, slice : ProgramSlice) -> StringView = {
     return { slice_between(&cursor.program.buffer, slice.start_offset, slice.end_offset) };
 }
 
-// TODO: should be `Cursor&`
-function slice : (cursor : Cursor mut&, length : isize) -> ProgramSlice = {
+function slice : (cursor : Cursor&, length : isize) -> ProgramSlice = {
     return {cursor.position, cursor.position + length};
 }
 
 function ascii_is_text_token_start_char : (char : u8) -> bool = {
     return ascii_is_alpha(char) or char == "_"[0];
 }
 
 function ascii_is_text_token_char : (char : u8) -> bool = {
     return ascii_is_alphanumeric(char) or char == "_"[0];
 }
 
-// TODO: should be `Cursor&`
-function get_char : (cursor : Cursor mut&) -> u8 = {
+function get_char : (cursor : Cursor&) -> u8 = {
     return cursor:get_char_at_offset(0);
 }
 
-// TODO: should be `Cursor&`
-function get_char_at_offset : (cursor : Cursor mut&, offset : isize) -> u8 = {
+function get_char_at_offset : (cursor : Cursor&, offset : isize) -> u8 = {
     if cursor.position + offset >= cursor.program:length() {
         return "\0"[0];
     }
     // TODO: allow direct indexing into a stringview
     return cursor.program.buffer.data[cursor.position + offset];
 }
 
 function meta : (start : isize, end : isize) -> Meta = {
     return {start, end};
 }
 
-// TODO: should be `Cursor&`
-function [@Len] is_next : (cursor : Cursor mut&, token : u8[@Len]&) -> bool = {
+function [@Len] is_next : (cursor : Cursor&, token : u8[@Len]&) -> bool = {
     return cursor:is_next(sv(&token));
 }
 
-// TODO: should be `Cursor&`
-function is_next : (cursor : Cursor mut&, token : StringView) -> bool = {
+function is_next : (cursor : Cursor&, token : StringView) -> bool = {
     for i in range(token:length()) {
         if cursor:get_char_at_offset(i) != token.buffer.data[i] {
             return false;
         }
     }
 
     if ascii_is_text_token_start_char(token.buffer.data[0]) {
@@ -252,43 +246,85 @@
         return {start_offset, start_offset + true_str:length()};
     } else {
         runtime_assert(cursor:try_skip_next_and_surrounding_white_space(false_str));
         return {start_offset, start_offset + false_str:length()};
     }
 }
 
-function get_next_decimal_token : (cursor : Cursor mut&) -> ProgramSlice = {
+// TODO: merge constant and compile time constant
+typedef NumericToken : {
+    data : ProgramSlice,
+    type : int, // 1: float, 2: int, 5: hex (matching `Constant`)
+}
+
+function get_next_numeric_token : (cursor : Cursor mut&) -> NumericToken = {
+    // TODO: binary/ octal
+    if cursor:is_next("0x") {
+        return {cursor:get_next_hex_token(), 5 /* Hex */};
+    }
+
+    // Parse floating point and integer constants
+    mut has_seen_decimal_point : bool = false;
+    mut has_seen_exponent : bool = false;
+
     mut token : ProgramSlice = cursor:slice(0);
     if cursor:try_skip_next("-") {
         token.end_offset += 1;
     }
 
     while !cursor:is_end_of_token() {
         let next_char : u8 = cursor:get_char();
         if ascii_is_digit(next_char) {
             cursor.position += 1;
             token.end_offset += 1;
+
+            if cursor:get_char() == char(".") {
+                if has_seen_decimal_point {
+                    syntax_error(&mut cursor, sv("cannot have two decimal points in a floating point constant"));
+                }
+                if has_seen_exponent {
+                    syntax_error(&mut cursor, sv("cannot have decimal place in floating point exponent"));
+                }
+                has_seen_decimal_point = true;
+
+                cursor.position += 1;
+                token.end_offset += 1;
+            }
+
+            if ascii_to_upper(cursor:get_char()) == char("E") {
+                if has_seen_exponent {
+                    syntax_error(&mut cursor, sv("cannot have two exponents in a floating point constant"));
+                }
+                has_seen_exponent = true;
+
+                cursor.position += 1;
+                token.end_offset += 1;
+
+                if cursor:get_char() == char("-") or cursor:get_char() == char("+") {
+                    cursor.position += 1;
+                    token.end_offset += 1;
+                }
+
+                if !ascii_is_digit(cursor:get_char()) {
+                    syntax_error(&mut cursor, sv("illegal digit '%' in floating constant"), decode_utf8(next_char));
+                }
+            }
         } else {
             // Otherwise its a syntax error
             syntax_error(&mut cursor, sv("illegal digit '%' in decimal constant"), decode_utf8(next_char));
         }
     }
     if token.end_offset - token.start_offset == 0 {
         syntax_error(&mut cursor, sv("expected decimal constant"));
     }
 
-    return token;
-}
-
-function get_next_numeric_token : (cursor : Cursor mut&) -> ProgramSlice = {
-    // TODO: binary/ octal
-    if cursor:is_next("0x") {
-        return cursor:get_next_hex_token();
+    if has_seen_decimal_point or has_seen_exponent {
+        return {token, 1 /* Floating point */};
     } else {
-        return cursor:get_next_decimal_token();
+        return {token, 2 /* Int */};
     }
 }
 
 function get_next_string_literal_token : (cursor : Cursor mut&) -> ProgramSlice = {
     runtime_assert(cursor:try_skip_next("\""));
     let start_offset : isize = cursor.position;
 
@@ -478,16 +514,19 @@
 function parse_compile_time_constant : (cursor : Cursor mut&) -> CompileTimeConstant = {
     runtime_assert(cursor:is_at_start_of_compile_time_constant());
 
     if cursor:is_next("@") {
         let identifier : ProgramSlice = cursor:get_next_at_identifier();
         return {true, identifier};
     } else {
-        let number : ProgramSlice = cursor:get_next_numeric_token();
-        return {false, number};
+        let number : NumericToken = cursor:get_next_numeric_token();
+        if number.type == 1 {
+            syntax_error(&mut cursor, sv("floating point literals cannot be used as a compile time constant"));
+        }
+        return {false, number.data};
     }
 }
 
 function parse_compile_time_constant_list : (cursor : Cursor mut&) -> Vector<CompileTimeConstant> = {
     // TODO: return some meta here
     // TODO: lets avoid this duplicate logic
     // Maybe we need function pointers
@@ -603,24 +642,19 @@
         is_heap_array = true;
         cursor:expect_next_skipping_ws("&");
     } else {
         is_heap_array = cursor:try_skip_next_and_surrounding_white_space("&");
     }
 
     mut sizes : Vector<CompileTimeConstant>;
-    // TODO: this would be cleaner with a short-circuit `and`
-    if is_heap_array {
-        // A heap array may/ may not have further dimensions specified
-        // TODO: I'm using `if ... {full} else {allocate empty}` pattern a lot... is there a nicer way
-        if cursor:try_skip_next_and_surrounding_white_space(",") {
-            sizes = cursor:parse_compile_time_constant_list();
-        } else {
-            sizes = make<Vector<CompileTimeConstant>>(&mut cursor.allocator);
-            cursor:expect_next_skipping_ws("]");
-        }
+    // A heap array may/ may not have further dimensions specified
+    // TODO: I'm using `if ... {full} else {allocate empty}` pattern a lot... is there a nicer way
+    if is_heap_array and !cursor:try_skip_next_and_surrounding_white_space(",") {
+        sizes = make<Vector<CompileTimeConstant>>(&mut cursor.allocator);
+        cursor:expect_next_skipping_ws("]");
     } else {
         // A stack array must have a known size
         sizes = cursor:parse_compile_time_constant_list();
     }
 
     let meta : Meta = {prefix.meta.start_offset, cursor.position};
     let array : ArrayType mut& = &mut cursor.allocator:allocate<ArrayType>();
@@ -898,23 +932,19 @@
 
     // Constants
     if cursor:is_next("true") or cursor:is_next("false") {
         let constant : Constant mut& = &mut cursor.allocator:allocate<Constant>();
         constant = {3, cursor:get_next_bool_token()};
         return {1, ref_to_addr(&constant), get_meta(constant.value)};
     }
-    if cursor:is_next("0x") {
-        let constant : Constant mut& = &mut cursor.allocator:allocate<Constant>();
-        constant = {5, cursor:get_next_hex_token()};
-        return {1, ref_to_addr(&constant), get_meta(constant.value)};
-    }
     if ascii_is_digit(cursor:get_char()) {
-        // TODO: float support
         let constant : Constant mut& = &mut cursor.allocator:allocate<Constant>();
-        constant = {2, cursor:get_next_decimal_token()};
+
+        let token : NumericToken = cursor:get_next_numeric_token();
+        constant = {token.type, token.data};
         return {1, ref_to_addr(&constant), get_meta(constant.value)};
     }
     if cursor:is_next("\"") {
         let constant : Constant mut& = &mut cursor.allocator:allocate<Constant>();
         constant = {0, cursor:get_next_string_literal_token()};
         return {1, ref_to_addr(&constant), get_meta(constant.value)};
     }
@@ -1140,14 +1170,30 @@
     }
 
     let expression : Expression = cursor:parse_expression();
     cursor:expect_next(";");
     return {make<Optional<Expression>>(expression), meta(start_offset, cursor:skip_ws_return_offset())};
 }
 
+function parse_continue : (cursor : Cursor mut&) -> Continue = {
+    let start_offset : isize = cursor.position;
+    runtime_assert(cursor:try_skip_next_and_surrounding_white_space("continue"));
+
+    cursor:expect_next(";");
+    return {meta(start_offset, cursor:skip_ws_return_offset())};
+}
+
+function parse_break : (cursor : Cursor mut&) -> Break = {
+    let start_offset : isize = cursor.position;
+    runtime_assert(cursor:try_skip_next_and_surrounding_white_space("break"));
+
+    cursor:expect_next(";");
+    return {meta(start_offset, cursor:skip_ws_return_offset())};
+}
+
 function parse_line : (cursor : Cursor mut&) -> Line = {
     // TODO: this should be templated?
     cursor:try_skip_white_space();
     if cursor:is_next("if") {
         let pointer : If mut& = &mut cursor.allocator:allocate<If>();
         pointer = cursor:parse_if();
         return {3, ref_to_addr(&pointer), pointer.meta};
@@ -1163,14 +1209,24 @@
         return {5, ref_to_addr(&pointer), pointer.meta};
     }
     if cursor:is_next("return") {
         let pointer : Return mut& = &mut cursor.allocator:allocate<Return>();
         pointer = cursor:parse_return();
         return {2, ref_to_addr(&pointer), pointer.meta};
     }
+    if cursor:is_next("continue") {
+        let pointer : Continue mut& = &mut cursor.allocator:allocate<Continue>();
+        pointer = cursor:parse_continue();
+        return {8, ref_to_addr(&pointer), pointer.meta};
+    }
+    if cursor:is_next("break") {
+        let pointer : Break mut& = &mut cursor.allocator:allocate<Break>();
+        pointer = cursor:parse_break();
+        return {9, ref_to_addr(&pointer), pointer.meta};
+    }
     if cursor:is_next("{") {
         let pointer : Scope mut& = &mut cursor.allocator:allocate<Scope>();
         pointer = cursor:parse_scope();
         return {6, ref_to_addr(&pointer), pointer.meta};
     }
     if cursor:is_next("let") {
         let pointer : VariableDeclaration mut& = &mut cursor.allocator:allocate<VariableDeclaration>();
@@ -1351,35 +1407,33 @@
     }
 
     syntax_error(&mut cursor, sv("expected one of the following top level program features:\\n - typedef\\n - @require_once\\n - function\\n - foreign\\n - @implicit\\n - @assignment\\n - @operator"));
     return {0, 0, meta(0, 0)};
 }
 
 function main : (argc: int, argv: u8[&][&]) -> int = {
-    let file_to_parse : CString = {&argv[1]};
-    let file : UnbufferedFile = open(file_to_parse, O_RDONLY());
-
-
-    mut allocator : Allocator = initialize_allocator();
-    mut file_contents : Vector<u8> = make<Vector<u8>>(&mut allocator);
-
     // 1) Read the entire file
-    {
-        mut read_buffer : u8[1024];
+    let file_to_parse : CString = {&argv[1]};
+    let file : Optional<File> = open(file_to_parse, O_RDONLY());
+    if !file:has_value() {
+        printf(sv("Error: could not open file '%'"), make<StringView>(file_to_parse));
+        return 1;
+    }
 
-        // TODO: `do while` to avoid temp value? Or `break` to make this prettier
-        mut read_data : View<u8> = make<View<u8>>("uninitialized");
-        while read_data:length() != 0 {
-            read_data = file:read(make<Span<u8>>(&mut read_buffer));
-            file_contents:extend_back(read_data:get_iter());
-        }
+    let maybe_map : Optional<MappedFile> = file:data():read();
+    file:data():close();  // fd no longer needed
+    if !maybe_map:has_value() {
+        printf(sv("Error: could not map file '%'"), make<StringView>(file_to_parse));
+        return 1;
     }
-    let program_text : StringView = { file_contents:view() };
+    let file_mapping : MappedFile& = &maybe_map:data();
+    let program_text : StringView = { file_mapping.buffer };
 
     // 2) Start parsing!!
+    mut allocator : Allocator = initialize_allocator();
     mut program : Vector<TopLevelFeature> = make<Vector<TopLevelFeature>>(&mut allocator);
     {
         mut cursor : Cursor = {program_text, 0, &mut allocator};
         cursor:try_skip_white_space();
 
         while !cursor:is_next("\0") {
             program:push_back(cursor:parse_next_top_level_feature());
@@ -1394,10 +1448,11 @@
             .file = get_stdout_io(),
         };
         json_output:write_json_value(&program);
         json_output:close();
     }
 
     // 4) Cleanup
-    file_contents:deallocate();
+    file_mapping:unmap();
+
     return 0;
 }
```

### Comparing `glang-0.2.1/src/glang/parser/self_hosted_parser.py` & `glang-0.4.0/src/glang/parser/self_hosted_parser.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import json
 import subprocess
 from pathlib import Path
 
-from ..codegen.user_facing_errors import InvalidSyntax
+from glang.codegen.user_facing_errors import InvalidSyntax
 
 PARSER_PATH = (Path(__file__).parent.parent / "bin" / "parser").resolve()
 
 
 def is_whitespace(string: str) -> bool:
     return len(string) == 0 or string.isspace()
```

### Comparing `glang-0.2.1/src/glang/parser/syntax_tree.c3` & `glang-0.4.0/src/glang/parser/syntax_tree.c3`

 * *Files 2% similar despite different names*

```diff
@@ -84,15 +84,15 @@
     alias : Type,
     meta : Meta,
 }
 
 typedef Scope : { lines : Vector<Line>, meta : Meta }
 typedef Line : {
     // TODO: enum
-    type : int, // 0: expression, 1: assignment, 2: return, 3: if, 4: while, 5: for, 6: scope, 7: declaration
+    type : int, // 0: expression, 1: assignment, 2: return, 3: if, 4: while, 5: for, 6: scope, 7: declaration, 8: continue, 9: break
     pointer : iptr,
     meta : Meta,
 }
 
 typedef If : {
     condition : Expression,
     if_scope : Scope,
@@ -111,14 +111,18 @@
     iterator : Expression,
     scope : Scope,
     meta : Meta,
 }
 
 typedef Return : { expression : Optional<Expression>, meta : Meta }
 
+typedef Continue : { meta : Meta }
+
+typedef Break : { meta : Meta }
+
 typedef Assignment : {
     lhs : Expression,
     operator : ProgramSlice,
     rhs : Expression,
     meta : Meta,
 }
 
@@ -368,16 +372,16 @@
         stream:write(",");
         stream:write_json_value(&value);
     }
     stream:write("]");
 }
 
 function write_json_value : (stream : JSON_Stream mut&, meta : Meta&) -> void = {
-    let start_position : FilePosition = (&stream.line_number_lookup):lookup_position(meta.start_offset);
-    let end_position : FilePosition = (&stream.line_number_lookup):lookup_position(meta.end_offset);
+    let start_position : FilePosition = stream.line_number_lookup:lookup_position(meta.start_offset);
+    let end_position : FilePosition = stream.line_number_lookup:lookup_position(meta.end_offset);
 
     mut object : JSON_Object = stream:new_object();
     object
         :add("__type__", sv("Meta"))
         :add("start", start_position)
         :add("end", end_position)
         :end();
@@ -630,14 +634,22 @@
         stream:write_json_value(&addr_to_ref<Scope>(line.pointer));
         return;
     }
     if line.type == 7 {
         stream:write_json_value(&addr_to_ref<VariableDeclaration>(line.pointer));
         return;
     }
+    if line.type == 8 {
+        stream:write_json_value(&addr_to_ref<Continue>(line.pointer));
+        return;
+    }
+    if line.type == 9 {
+        stream:write_json_value(&addr_to_ref<Break>(line.pointer));
+        return;
+    }
     runtime_assert(false);
 }
 
 function write_json_value : (stream : JSON_Stream mut&, node : If&) -> void = {
     mut object : JSON_Object = stream:new_object();
     object
         :add_meta("If", node.meta)
@@ -670,14 +682,28 @@
     mut object : JSON_Object = stream:new_object();
     object
         :add_meta("Return", node.meta)
         :add("expression", node.expression)
         :end();
 }
 
+function write_json_value : (stream : JSON_Stream mut&, node : Continue&) -> void = {
+    mut object : JSON_Object = stream:new_object();
+    object
+        :add_meta("Continue", node.meta)
+        :end();
+}
+
+function write_json_value : (stream : JSON_Stream mut&, node : Break&) -> void = {
+    mut object : JSON_Object = stream:new_object();
+    object
+        :add_meta("Break", node.meta)
+        :end();
+}
+
 function write_json_value : (stream : JSON_Stream mut&, node : Assignment&) -> void = {
     mut object : JSON_Object = stream:new_object();
     object
         :add_meta("Assignment", node.meta)
         :add("lhs", node.lhs)
         :add("rhs", node.rhs)
         :add("operator", node.operator)
```

### Comparing `glang-0.2.1/src/glang/targets/aarch64_linux.yml` & `glang-0.4.0/src/glang/targets/aarch64_linux.yml`

 * *Files identical despite different names*

### Comparing `glang-0.2.1/src/glang/targets/arm_linux.yml` & `glang-0.4.0/src/glang/targets/arm_linux.yml`

 * *Files identical despite different names*

### Comparing `glang-0.2.1/.gitignore` & `glang-0.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `glang-0.2.1/LICENSE` & `glang-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `glang-0.2.1/hatch_build.py` & `glang-0.4.0/hatch_build.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from pathlib import Path
+from subprocess import run
 from typing import Any
 
-from hatch.utils.platform import Platform
 from hatchling.builders.hooks.plugin.interface import BuildHookInterface
 
 
 class CustomBuildHook(BuildHookInterface):
     def clean(self, versions: list[str]):
         build_dir = Path(self.directory)
         parser_bin = build_dir / "parser"
@@ -14,15 +14,17 @@
             parser_bin.unlink()
 
         return super().clean(versions)
 
     def initialize(self, version: str, build_data: dict[str, Any]):
         self.app.display_waiting("Bootstrapping parser")
 
-        Platform().check_command(["./bootstrap.sh"], shell=False)
+        rc = run(["./bootstrap.sh"], check=False).returncode
+        if rc:
+            self.app.abort("Bootstrap failed", rc)
 
         self.app.display_success("Done!")
 
         build_data["force_include"]["dist/parser"] = "glang/bin/parser"
 
         build_data["pure_python"] = False
         build_data["infer_tag"] = True
```

### Comparing `glang-0.2.1/pyproject.toml` & `glang-0.4.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,56 +1,49 @@
 [build-system]
-requires = ["hatchling"]
+requires = ["hatchling~=1.21"]
 build-backend = "hatchling.build"
 
 
 [project]
 name = "glang"
-version = "0.2.1"
+version = "0.4.0"
 authors = [
   { name = "Antros Economides", email = "antroseconomides@hotmail.co.uk" },
   { name = "Tom Grant", email = "thomas.grant.mail@gmail.com" },
 ]
 description = "A Graphene front-end for LLVM"
 # TODO readme = "README.md"
 license = "AGPL-3.0-only"
-requires-python = ">=3.10"
+requires-python = ">=3.12"
 classifiers = [
   "Development Status :: 3 - Alpha",
   "License :: OSI Approved :: GNU Affero General Public License v3",
   "Operating System :: POSIX :: Linux",
   "Programming Language :: Python :: 3",
   "Topic :: Software Development :: Compilers",
 ]
-dependencies = ["PyYAML~=6.0.0", "typed-argument-parser>=1.8.1,<1.10.0"]
+dependencies = ["PyYAML~=6.0", "typed-argument-parser~=1.8"]
 
 [project.urls]
 "Homepage" = "https://github.com/DaveDuck321/GrapheneLang/"
 "Bug Tracker" = "https://github.com/DaveDuck321/GrapheneLang/issues"
 
 [project.scripts]
 glang = "glang.driver:main"
 
 
 # Development environment to be used with your IDE. Just set the venv path to
 # the output of `hatch env find dev`.
 [tool.hatch.envs.dev]
-dependencies = ["hatch~=1.7.0", "interegular~=0.3.2", "lark~=1.1.7", "pylint"]
+dependencies = ["interegular~=0.3", "lark~=1.1"]
 
 [tool.hatch.envs.dev.scripts]
 bootstrap = "./bootstrap.sh"
-lint = ["pylint $(git ls-files \\*.py)"]
-
-
-# Test environment.
-[tool.hatch.envs.test]
-dependencies = ["interegular~=0.3.2", "lark~=1.1.7"]
-
-[tool.hatch.envs.test.scripts]
-run = "python tests/run_tests.py"
+parser = "glang ./src/glang/parser/parser.c3 -o ./dist/parser -O3"
+test = "python tests/run_tests.py {args}"
 
 
 # Style environment. Does not depend on the project.
 [tool.hatch.envs.style]
 detached = true
 skip-install = true
 dependencies = ["black", "isort"]
@@ -64,20 +57,21 @@
 
 
 # Build configuration. Need a bunch of dependencies because the build process
 # bootstraps the compiler.
 [tool.hatch.build]
 # Exclude symlinks used for editable installs.
 exclude = ["src/glang/bin"]
-dependencies = [
-  "hatch~=1.7.0",
-  "lark~=1.1.7",
-  "PyYAML~=6.0.0",
-  "typed-argument-parser>=1.8.1,<1.10.0",
-]
+dependencies = ["lark~=1.1", "PyYAML~=6.0", "typed-argument-parser~=1.8"]
 
 [tool.hatch.build.targets.sdist]
 exclude = [".github", "docs", "tests"]
 
 [tool.hatch.build.targets.wheel]
 packages = ["src/glang"]
 hooks.custom.path = "hatch_build.py"
+
+[tool.ruff]
+# hatch sets this to 120 by default. 88 is what black uses.
+line-length = 88
+# Disable all rules without automatic fixes.
+fix-only = true
```

### Comparing `glang-0.2.1/PKG-INFO` & `glang-0.4.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: glang
-Version: 0.2.1
+Version: 0.4.0
 Summary: A Graphene front-end for LLVM
 Project-URL: Homepage, https://github.com/DaveDuck321/GrapheneLang/
 Project-URL: Bug Tracker, https://github.com/DaveDuck321/GrapheneLang/issues
 Author-email: Antros Economides <antroseconomides@hotmail.co.uk>, Tom Grant <thomas.grant.mail@gmail.com>
 License-Expression: AGPL-3.0-only
 License-File: LICENSE
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Compilers
-Requires-Python: >=3.10
-Requires-Dist: pyyaml~=6.0.0
-Requires-Dist: typed-argument-parser<1.10.0,>=1.8.1
+Requires-Python: >=3.12
+Requires-Dist: pyyaml~=6.0
+Requires-Dist: typed-argument-parser~=1.8
```

