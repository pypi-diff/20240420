# Comparing `tmp/fastlifeweb-0.3.1.tar.gz` & `tmp/fastlifeweb-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastlifeweb-0.3.1.tar", max compression
+gzip compressed data, was "fastlifeweb-0.4.0.tar", max compression
```

## Comparing `fastlifeweb-0.3.1.tar` & `fastlifeweb-0.4.0.tar`

### file list

```diff
@@ -1,63 +1,69 @@
--rw-r--r--   0        0        0     1504 2024-01-05 08:56:46.068218 fastlifeweb-0.3.1/LICENSE
--rw-r--r--   0        0        0      577 2024-03-29 07:03:39.775183 fastlifeweb-0.3.1/README.md
--rw-r--r--   0        0        0     1967 2024-03-29 07:20:30.908411 fastlifeweb-0.3.1/pyproject.toml
--rw-r--r--   0        0        0      312 2024-03-29 07:03:39.778516 fastlifeweb-0.3.1/src/fastlife/__init__.py
--rw-r--r--   0        0        0       91 2024-01-14 12:49:19.832886 fastlifeweb-0.3.1/src/fastlife/configurator/__init__.py
--rw-r--r--   0        0        0      216 2024-03-29 07:03:39.778516 fastlifeweb-0.3.1/src/fastlife/configurator/base.py
--rw-r--r--   0        0        0     5740 2024-03-29 07:03:45.239318 fastlifeweb-0.3.1/src/fastlife/configurator/configurator.py
--rw-r--r--   0        0        0     1449 2024-03-29 07:03:45.239318 fastlifeweb-0.3.1/src/fastlife/configurator/registry.py
--rw-r--r--   0        0        0     1387 2024-03-29 07:03:39.778516 fastlifeweb-0.3.1/src/fastlife/configurator/settings.py
--rw-r--r--   0        0        0        0 2023-09-22 06:52:58.847518 fastlifeweb-0.3.1/src/fastlife/py.typed
--rw-r--r--   0        0        0        0 2023-09-18 06:50:01.267211 fastlifeweb-0.3.1/src/fastlife/request/__init__.py
--rw-r--r--   0        0        0     3642 2024-03-29 07:03:45.242652 fastlifeweb-0.3.1/src/fastlife/request/form_data.py
--rw-r--r--   0        0        0        0 2024-01-14 12:49:19.832886 fastlifeweb-0.3.1/src/fastlife/security/__init__.py
--rw-r--r--   0        0        0     1025 2024-03-29 07:03:45.242652 fastlifeweb-0.3.1/src/fastlife/security/csrf.py
--rw-r--r--   0        0        0      509 2024-03-29 07:03:39.778516 fastlifeweb-0.3.1/src/fastlife/security/policy.py
--rw-r--r--   0        0        0      838 2024-03-29 07:03:39.778516 fastlifeweb-0.3.1/src/fastlife/session/__init__.py
--rw-r--r--   0        0        0     3049 2024-03-29 07:03:45.242652 fastlifeweb-0.3.1/src/fastlife/session/middleware.py
--rw-r--r--   0        0        0     1458 2024-03-29 07:03:39.778516 fastlifeweb-0.3.1/src/fastlife/session/serializer.py
--rw-r--r--   0        0        0        0 2024-03-29 07:03:39.778516 fastlifeweb-0.3.1/src/fastlife/shared_utils/__init__.py
--rw-r--r--   0        0        0      466 2023-11-25 15:57:32.200572 fastlifeweb-0.3.1/src/fastlife/shared_utils/infer.py
--rw-r--r--   0        0        0     1410 2024-03-29 07:03:45.242652 fastlifeweb-0.3.1/src/fastlife/shared_utils/resolver.py
--rw-r--r--   0        0        0      481 2024-03-29 07:03:39.778516 fastlifeweb-0.3.1/src/fastlife/templates/A.jinja
--rw-r--r--   0        0        0     1064 2024-03-29 07:03:39.778516 fastlifeweb-0.3.1/src/fastlife/templates/Button.jinja
--rw-r--r--   0        0        0       98 2024-03-29 07:03:39.778516 fastlifeweb-0.3.1/src/fastlife/templates/Checkbox.jinja
--rw-r--r--   0        0        0       80 2024-03-29 07:03:39.778516 fastlifeweb-0.3.1/src/fastlife/templates/CsrfToken.jinja
--rw-r--r--   0        0        0      147 2024-03-29 07:03:39.778516 fastlifeweb-0.3.1/src/fastlife/templates/Form.jinja
--rw-r--r--   0        0        0      151 2024-03-29 07:03:39.778516 fastlifeweb-0.3.1/src/fastlife/templates/H1.jinja
--rw-r--r--   0        0        0      151 2024-03-29 07:03:39.778516 fastlifeweb-0.3.1/src/fastlife/templates/H2.jinja
--rw-r--r--   0        0        0      120 2024-03-29 07:03:39.778516 fastlifeweb-0.3.1/src/fastlife/templates/Hidden.jinja
--rw-r--r--   0        0        0      612 2024-03-29 07:03:39.778516 fastlifeweb-0.3.1/src/fastlife/templates/Input.jinja
--rw-r--r--   0        0        0      147 2024-03-29 07:03:39.778516 fastlifeweb-0.3.1/src/fastlife/templates/Label.jinja
--rw-r--r--   0        0        0       65 2024-03-29 07:03:39.778516 fastlifeweb-0.3.1/src/fastlife/templates/Option.jinja
--rw-r--r--   0        0        0      654 2024-03-29 07:03:39.778516 fastlifeweb-0.3.1/src/fastlife/templates/Radio.jinja
--rw-r--r--   0        0        0      407 2024-03-29 07:03:39.778516 fastlifeweb-0.3.1/src/fastlife/templates/Select.jinja
--rw-r--r--   0        0        0        0 2024-03-29 07:03:39.778516 fastlifeweb-0.3.1/src/fastlife/templates/__init__.py
--rw-r--r--   0        0        0      279 2024-03-29 07:03:39.778516 fastlifeweb-0.3.1/src/fastlife/templates/pydantic_form/Boolean.jinja
--rw-r--r--   0        0        0      539 2024-03-29 07:03:39.778516 fastlifeweb-0.3.1/src/fastlife/templates/pydantic_form/Dropdown.jinja
--rw-r--r--   0        0        0       83 2024-03-29 07:03:39.778516 fastlifeweb-0.3.1/src/fastlife/templates/pydantic_form/Hidden.jinja
--rw-r--r--   0        0        0      493 2024-03-29 07:03:39.778516 fastlifeweb-0.3.1/src/fastlife/templates/pydantic_form/Model.jinja
--rw-r--r--   0        0        0     1409 2024-03-29 07:03:39.778516 fastlifeweb-0.3.1/src/fastlife/templates/pydantic_form/Sequence.jinja
--rw-r--r--   0        0        0      503 2024-03-29 07:03:39.778516 fastlifeweb-0.3.1/src/fastlife/templates/pydantic_form/Text.jinja
--rw-r--r--   0        0        0     1003 2024-03-29 07:03:39.778516 fastlifeweb-0.3.1/src/fastlife/templates/pydantic_form/Union.jinja
--rw-r--r--   0        0        0      287 2024-03-29 07:03:39.778516 fastlifeweb-0.3.1/src/fastlife/templates/pydantic_form/Widget.jinja
--rw-r--r--   0        0        0      220 2024-03-29 07:03:39.778516 fastlifeweb-0.3.1/src/fastlife/templating/__init__.py
--rw-r--r--   0        0        0     1907 2024-03-29 07:03:39.778516 fastlifeweb-0.3.1/src/fastlife/templating/binding.py
--rw-r--r--   0        0        0      156 2024-03-29 07:03:39.778516 fastlifeweb-0.3.1/src/fastlife/templating/renderer/__init__.py
--rw-r--r--   0        0        0      801 2024-03-29 07:03:39.778516 fastlifeweb-0.3.1/src/fastlife/templating/renderer/abstract.py
--rw-r--r--   0        0        0     2379 2024-03-29 07:03:45.242652 fastlifeweb-0.3.1/src/fastlife/templating/renderer/jinjax.py
--rw-r--r--   0        0        0        0 2023-12-02 23:16:17.801084 fastlifeweb-0.3.1/src/fastlife/templating/renderer/widgets/__init__.py
--rw-r--r--   0        0        0     2446 2024-03-29 07:03:39.778516 fastlifeweb-0.3.1/src/fastlife/templating/renderer/widgets/base.py
--rw-r--r--   0        0        0      454 2024-03-29 07:03:39.778516 fastlifeweb-0.3.1/src/fastlife/templating/renderer/widgets/boolean.py
--rw-r--r--   0        0        0      891 2024-03-29 07:03:39.778516 fastlifeweb-0.3.1/src/fastlife/templating/renderer/widgets/dropdown.py
--rw-r--r--   0        0        0     9626 2024-03-29 07:03:39.778516 fastlifeweb-0.3.1/src/fastlife/templating/renderer/widgets/factory.py
--rw-r--r--   0        0        0      317 2024-03-29 07:03:39.781850 fastlifeweb-0.3.1/src/fastlife/templating/renderer/widgets/hidden.py
--rw-r--r--   0        0        0      943 2024-03-29 07:03:39.781850 fastlifeweb-0.3.1/src/fastlife/templating/renderer/widgets/model.py
--rw-r--r--   0        0        0     1355 2024-03-29 07:03:39.781850 fastlifeweb-0.3.1/src/fastlife/templating/renderer/widgets/sequence.py
--rw-r--r--   0        0        0      782 2024-03-29 07:03:39.781850 fastlifeweb-0.3.1/src/fastlife/templating/renderer/widgets/text.py
--rw-r--r--   0        0        0     1658 2024-03-29 07:03:39.781850 fastlifeweb-0.3.1/src/fastlife/templating/renderer/widgets/union.py
--rw-r--r--   0        0        0       67 2023-09-16 21:42:04.218390 fastlifeweb-0.3.1/src/fastlife/testing/__init__.py
--rw-r--r--   0        0        0    13780 2024-03-29 07:03:39.781850 fastlifeweb-0.3.1/src/fastlife/testing/testclient.py
--rw-r--r--   0        0        0      154 2024-01-14 12:49:19.836219 fastlifeweb-0.3.1/src/fastlife/views/__init__.py
--rw-r--r--   0        0        0     1038 2024-03-29 07:03:39.781850 fastlifeweb-0.3.1/src/fastlife/views/pydantic_form.py
--rw-r--r--   0        0        0     1748 1970-01-01 00:00:00.000000 fastlifeweb-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1504 2024-01-05 08:56:46.068218 fastlifeweb-0.4.0/LICENSE
+-rw-r--r--   0        0        0      510 2024-04-13 13:57:35.096106 fastlifeweb-0.4.0/README.md
+-rw-r--r--   0        0        0     2090 2024-04-20 07:42:52.814451 fastlifeweb-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0      312 2024-03-30 15:07:08.088027 fastlifeweb-0.4.0/src/fastlife/__init__.py
+-rw-r--r--   0        0        0       91 2024-01-14 12:49:19.832886 fastlifeweb-0.4.0/src/fastlife/configurator/__init__.py
+-rw-r--r--   0        0        0      216 2024-03-29 07:03:39.778516 fastlifeweb-0.4.0/src/fastlife/configurator/base.py
+-rw-r--r--   0        0        0     5740 2024-03-30 15:07:08.088027 fastlifeweb-0.4.0/src/fastlife/configurator/configurator.py
+-rw-r--r--   0        0        0     1463 2024-04-13 13:57:35.099439 fastlifeweb-0.4.0/src/fastlife/configurator/registry.py
+-rw-r--r--   0        0        0     1489 2024-04-13 13:57:35.099439 fastlifeweb-0.4.0/src/fastlife/configurator/settings.py
+-rw-r--r--   0        0        0        0 2023-09-22 06:52:58.847518 fastlifeweb-0.4.0/src/fastlife/py.typed
+-rw-r--r--   0        0        0        0 2023-09-18 06:50:01.267211 fastlifeweb-0.4.0/src/fastlife/request/__init__.py
+-rw-r--r--   0        0        0     3642 2024-03-30 15:07:08.088027 fastlifeweb-0.4.0/src/fastlife/request/form_data.py
+-rw-r--r--   0        0        0        0 2024-01-14 12:49:19.832886 fastlifeweb-0.4.0/src/fastlife/security/__init__.py
+-rw-r--r--   0        0        0     1025 2024-03-30 15:07:08.088027 fastlifeweb-0.4.0/src/fastlife/security/csrf.py
+-rw-r--r--   0        0        0      509 2024-03-29 07:03:39.778516 fastlifeweb-0.4.0/src/fastlife/security/policy.py
+-rw-r--r--   0        0        0      838 2024-03-29 07:03:39.778516 fastlifeweb-0.4.0/src/fastlife/session/__init__.py
+-rw-r--r--   0        0        0     3049 2024-04-19 06:48:48.276132 fastlifeweb-0.4.0/src/fastlife/session/middleware.py
+-rw-r--r--   0        0        0     1458 2024-03-29 07:03:39.778516 fastlifeweb-0.4.0/src/fastlife/session/serializer.py
+-rw-r--r--   0        0        0        0 2024-03-30 15:07:08.088027 fastlifeweb-0.4.0/src/fastlife/shared_utils/__init__.py
+-rw-r--r--   0        0        0      466 2023-11-25 15:57:32.200572 fastlifeweb-0.4.0/src/fastlife/shared_utils/infer.py
+-rw-r--r--   0        0        0     1410 2024-03-30 15:07:08.088027 fastlifeweb-0.4.0/src/fastlife/shared_utils/resolver.py
+-rw-r--r--   0        0        0      677 2024-04-13 13:57:35.099439 fastlifeweb-0.4.0/src/fastlife/templates/A.jinja
+-rw-r--r--   0        0        0     1137 2024-04-13 13:57:35.099439 fastlifeweb-0.4.0/src/fastlife/templates/Button.jinja
+-rw-r--r--   0        0        0      366 2024-04-15 06:41:03.874701 fastlifeweb-0.4.0/src/fastlife/templates/Checkbox.jinja
+-rw-r--r--   0        0        0       59 2024-04-13 13:57:35.102773 fastlifeweb-0.4.0/src/fastlife/templates/CsrfToken.jinja
+-rw-r--r--   0        0        0      329 2024-04-14 07:07:54.763970 fastlifeweb-0.4.0/src/fastlife/templates/Form.jinja
+-rw-r--r--   0        0        0      196 2024-04-13 13:57:35.102773 fastlifeweb-0.4.0/src/fastlife/templates/H1.jinja
+-rw-r--r--   0        0        0      196 2024-04-13 13:57:35.102773 fastlifeweb-0.4.0/src/fastlife/templates/H2.jinja
+-rw-r--r--   0        0        0      195 2024-04-13 13:57:35.102773 fastlifeweb-0.4.0/src/fastlife/templates/H3.jinja
+-rw-r--r--   0        0        0      195 2024-04-13 13:57:35.102773 fastlifeweb-0.4.0/src/fastlife/templates/H4.jinja
+-rw-r--r--   0        0        0      193 2024-04-13 13:57:35.102773 fastlifeweb-0.4.0/src/fastlife/templates/H5.jinja
+-rw-r--r--   0        0        0      191 2024-04-13 13:57:35.102773 fastlifeweb-0.4.0/src/fastlife/templates/H6.jinja
+-rw-r--r--   0        0        0      120 2024-03-30 15:07:08.088027 fastlifeweb-0.4.0/src/fastlife/templates/Hidden.jinja
+-rw-r--r--   0        0        0      638 2024-04-14 21:06:08.222497 fastlifeweb-0.4.0/src/fastlife/templates/Input.jinja
+-rw-r--r--   0        0        0      170 2024-04-13 13:57:35.102773 fastlifeweb-0.4.0/src/fastlife/templates/Label.jinja
+-rw-r--r--   0        0        0      121 2024-04-15 06:29:06.881534 fastlifeweb-0.4.0/src/fastlife/templates/Option.jinja
+-rw-r--r--   0        0        0      164 2024-04-13 13:57:35.102773 fastlifeweb-0.4.0/src/fastlife/templates/P.jinja
+-rw-r--r--   0        0        0      723 2024-04-13 13:57:35.106106 fastlifeweb-0.4.0/src/fastlife/templates/Radio.jinja
+-rw-r--r--   0        0        0      427 2024-04-13 13:57:35.106106 fastlifeweb-0.4.0/src/fastlife/templates/Select.jinja
+-rw-r--r--   0        0        0        0 2024-03-30 15:07:08.088027 fastlifeweb-0.4.0/src/fastlife/templates/__init__.py
+-rw-r--r--   0        0        0      298 2024-04-15 06:38:03.760573 fastlifeweb-0.4.0/src/fastlife/templates/pydantic_form/Boolean.jinja
+-rw-r--r--   0        0        0      500 2024-04-15 06:29:02.724849 fastlifeweb-0.4.0/src/fastlife/templates/pydantic_form/Dropdown.jinja
+-rw-r--r--   0        0        0       83 2024-03-30 15:07:08.088027 fastlifeweb-0.4.0/src/fastlife/templates/pydantic_form/Hidden.jinja
+-rw-r--r--   0        0        0      123 2024-04-13 13:57:35.106106 fastlifeweb-0.4.0/src/fastlife/templates/pydantic_form/Hint.jinja
+-rw-r--r--   0        0        0      449 2024-04-13 13:57:35.106106 fastlifeweb-0.4.0/src/fastlife/templates/pydantic_form/Model.jinja
+-rw-r--r--   0        0        0     1380 2024-04-14 07:07:58.770652 fastlifeweb-0.4.0/src/fastlife/templates/pydantic_form/Sequence.jinja
+-rw-r--r--   0        0        0      402 2024-04-13 13:57:35.106106 fastlifeweb-0.4.0/src/fastlife/templates/pydantic_form/Text.jinja
+-rw-r--r--   0        0        0      950 2024-04-15 05:32:37.810352 fastlifeweb-0.4.0/src/fastlife/templates/pydantic_form/Union.jinja
+-rw-r--r--   0        0        0      287 2024-03-30 15:07:08.091360 fastlifeweb-0.4.0/src/fastlife/templates/pydantic_form/Widget.jinja
+-rw-r--r--   0        0        0      234 2024-04-13 13:57:35.106106 fastlifeweb-0.4.0/src/fastlife/templating/__init__.py
+-rw-r--r--   0        0        0     1378 2024-04-13 13:57:35.109439 fastlifeweb-0.4.0/src/fastlife/templating/binding.py
+-rw-r--r--   0        0        0      181 2024-04-13 13:57:35.109439 fastlifeweb-0.4.0/src/fastlife/templating/renderer/__init__.py
+-rw-r--r--   0        0        0      818 2024-04-13 13:57:35.109439 fastlifeweb-0.4.0/src/fastlife/templating/renderer/abstract.py
+-rw-r--r--   0        0        0     3206 2024-04-13 13:57:35.109439 fastlifeweb-0.4.0/src/fastlife/templating/renderer/jinjax.py
+-rw-r--r--   0        0        0        0 2023-12-02 23:16:17.801084 fastlifeweb-0.4.0/src/fastlife/templating/renderer/widgets/__init__.py
+-rw-r--r--   0        0        0     2769 2024-04-15 06:45:59.155931 fastlifeweb-0.4.0/src/fastlife/templating/renderer/widgets/base.py
+-rw-r--r--   0        0        0      468 2024-04-14 07:07:58.773985 fastlifeweb-0.4.0/src/fastlife/templating/renderer/widgets/boolean.py
+-rw-r--r--   0        0        0      901 2024-04-14 07:07:58.773985 fastlifeweb-0.4.0/src/fastlife/templating/renderer/widgets/dropdown.py
+-rw-r--r--   0        0        0    10335 2024-04-15 06:46:25.562707 fastlifeweb-0.4.0/src/fastlife/templating/renderer/widgets/factory.py
+-rw-r--r--   0        0        0      308 2024-04-14 07:07:58.773985 fastlifeweb-0.4.0/src/fastlife/templating/renderer/widgets/hidden.py
+-rw-r--r--   0        0        0      950 2024-04-14 07:07:58.773985 fastlifeweb-0.4.0/src/fastlife/templating/renderer/widgets/model.py
+-rw-r--r--   0        0        0     1347 2024-04-14 07:07:58.773985 fastlifeweb-0.4.0/src/fastlife/templating/renderer/widgets/sequence.py
+-rw-r--r--   0        0        0      819 2024-04-14 07:07:58.773985 fastlifeweb-0.4.0/src/fastlife/templating/renderer/widgets/text.py
+-rw-r--r--   0        0        0     1689 2024-04-14 07:07:58.777319 fastlifeweb-0.4.0/src/fastlife/templating/renderer/widgets/union.py
+-rw-r--r--   0        0        0       67 2023-09-16 21:42:04.218390 fastlifeweb-0.4.0/src/fastlife/testing/__init__.py
+-rw-r--r--   0        0        0    16404 2024-04-20 07:26:17.322149 fastlifeweb-0.4.0/src/fastlife/testing/testclient.py
+-rw-r--r--   0        0        0      154 2024-01-14 12:49:19.836219 fastlifeweb-0.4.0/src/fastlife/views/__init__.py
+-rw-r--r--   0        0        0     1092 2024-04-13 13:57:35.112773 fastlifeweb-0.4.0/src/fastlife/views/pydantic_form.py
+-rw-r--r--   0        0        0     1833 1970-01-01 00:00:00.000000 fastlifeweb-0.4.0/PKG-INFO
```

### Comparing `fastlifeweb-0.3.1/LICENSE` & `fastlifeweb-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fastlifeweb-0.3.1/pyproject.toml` & `fastlifeweb-0.4.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,36 +1,39 @@
 [tool.poetry]
 authors = ["Guillaume Gauvrit <guillaume@gauvr.it>"]
 description = "High-level web framework"
 name = "fastlifeweb"
 license = "BSD-derived"
 packages = [{include = "fastlife", from = "src"}]
+homepage = "https://github.com/mardiros/fastlife"
+repository = "https://github.com/mardiros/fastlife"
 readme = "README.md"
 classifiers = [
   "Development Status :: 4 - Beta",
   "Framework :: AsyncIO",
   "Intended Audience :: Developers",
   "License :: OSI Approved :: BSD License",
   "Topic :: Software Development :: Libraries :: Python Modules",
   "Topic :: Internet :: WWW/HTTP",
 ]
-version = "0.3.1"
+version = "0.4.0"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 beautifulsoup4 = {version = "^4.12.2", extras = ["testing"]}
 fastapi = "^0.110.0"
-jinjax = "^0.31"
+jinjax = "^0.32"
 pydantic = "^2.3.0"
 pydantic-settings = "^2.0.3"
 python-multipart = "^0.0.6"
 venusian = "^3.0.0"
 markupsafe = "^2.1.3"
 behave = "^1.2.6"
 itsdangerous = "^2.1.2"
+multidict = "^6.0.5"
 
 [tool.poetry.group.dev.dependencies]
 beautifulsoup4 = "^4.12.2"
 black = "^23.3.0"
 flake8 = "^6.1.0"
 httpx = "^0.25.0"
 mypy = "^1.4.0"
```

### Comparing `fastlifeweb-0.3.1/src/fastlife/configurator/configurator.py` & `fastlifeweb-0.4.0/src/fastlife/configurator/configurator.py`

 * *Files identical despite different names*

### Comparing `fastlifeweb-0.3.1/src/fastlife/configurator/registry.py` & `fastlifeweb-0.4.0/src/fastlife/configurator/registry.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 from fastapi import Depends
 
 from fastlife.security.policy import CheckPermission
 from fastlife.shared_utils.resolver import resolve
 
 if TYPE_CHECKING:
     from fastlife.templating.renderer import (  # coverage: ignore
-        AbstractTemplateRenderer,  # coverage: ignore
+        AbstractTemplateRendererFactory,  # coverage: ignore
     )  # coverage: ignore
 
 from .settings import Settings
 
 
 class AppRegistry:
     settings: Settings
-    renderer: "AbstractTemplateRenderer"
+    renderer: "AbstractTemplateRendererFactory"
     check_permission: CheckPermission
 
     def __init__(self, settings: Settings) -> None:
         # Abtract class resolved for dependency injection
         TemplateRenderer = resolve(settings.template_renderer_class)
 
         self.settings = settings
```

### Comparing `fastlifeweb-0.3.1/src/fastlife/configurator/settings.py` & `fastlifeweb-0.4.0/src/fastlife/configurator/settings.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,14 +13,17 @@
     registry_class: str = Field(default="fastlife.configurator.registry:AppRegistry")
     template_renderer_class: str = Field(
         default="fastlife.templating.renderer:JinjaxTemplateRenderer"
     )
     form_data_model_prefix: str = Field(default="payload")
     csrf_token_name: str = Field(default="csrf_token")
 
+    jinjax_use_cache: bool = Field(default=True)
+    jinjax_auto_reload: bool = Field(default=False)
+
     session_secret_key: str = Field(default="")
     session_cookie_name: str = Field(default="flsess")
     session_cookie_domain: str = Field(default="")
     session_cookie_path: str = Field(default="/")
     session_duration: timedelta = Field(default=timedelta(days=14))
     session_cookie_same_site: Literal["lax", "strict", "none"] = Field(default="lax")
     session_cookie_secure: bool = Field(default=False)
```

### Comparing `fastlifeweb-0.3.1/src/fastlife/request/form_data.py` & `fastlifeweb-0.4.0/src/fastlife/request/form_data.py`

 * *Files identical despite different names*

### Comparing `fastlifeweb-0.3.1/src/fastlife/security/csrf.py` & `fastlifeweb-0.4.0/src/fastlife/security/csrf.py`

 * *Files identical despite different names*

### Comparing `fastlifeweb-0.3.1/src/fastlife/session/__init__.py` & `fastlifeweb-0.4.0/src/fastlife/session/__init__.py`

 * *Files identical despite different names*

### Comparing `fastlifeweb-0.3.1/src/fastlife/session/middleware.py` & `fastlifeweb-0.4.0/src/fastlife/session/middleware.py`

 * *Files identical despite different names*

### Comparing `fastlifeweb-0.3.1/src/fastlife/session/serializer.py` & `fastlifeweb-0.4.0/src/fastlife/session/serializer.py`

 * *Files identical despite different names*

### Comparing `fastlifeweb-0.3.1/src/fastlife/shared_utils/resolver.py` & `fastlifeweb-0.4.0/src/fastlife/shared_utils/resolver.py`

 * *Files identical despite different names*

### Comparing `fastlifeweb-0.3.1/src/fastlife/templates/Input.jinja` & `fastlifeweb-0.4.0/src/fastlife/templates/Input.jinja`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,31 @@
-{# def name, value="", input_type="text", id="", aria_label="", placeholder="" #}
-{% set css = "bg-neutral-50 border border-neutral-300 text-neutral-900 text-base rounded-lg focus:ring-primary-500
-focus:border-primary-500 block w-full p-2.5 dark:bg-neutral-700 dark:border-neutral-600 dark:placeholder-neutral-400
-dark:text-white dark:focus:ring-primary-500 dark:focus:border-primary-500" %}
+{# def
+name,
+value="",
+type="text",
+id="",
+aria_label="",
+placeholder="",
+class_="""
+bg-neutral-50
+block
+border
+border-neutral-300
+p-2.5
+rounded-lg
+text-base
+text-neutral-900
+w-full
+dark:bg-neutral-700
+dark:border-neutral-600
+dark:focus:border-primary-500
+dark:focus:ring-primary-500
+dark:placeholder-neutral-400
+dark:text-white
+focus:border-primary-500
+focus:ring-primary-500
+"""
+#}
 
-<input name="{{name}}" value="{{value}}" type="{{input_type}}" id="{{id}}" {% if aria_label
+<input name="{{name}}" value="{{value}}" type="{{type}}" {% if id %}id="{{id}}" {% endif %}{% if aria_label
   %}aria-label="{{aria_label}}" {% endif %} {% if placeholder %}placeholder="{{placeholder}}" {% endif %}
-  class="{{css}}" />
+  class="{{attrs.class or class_}}" />
```

### Comparing `fastlifeweb-0.3.1/src/fastlife/templates/Radio.jinja` & `fastlifeweb-0.4.0/src/fastlife/templates/Radio.jinja`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,30 @@
-{# def label name id value checked=false disabled=false onclick="" #}
-<div class="flex items-center mb-4">
-  <input type="radio" name="{{name}}" id="{{id}}" {% if value %}value="{{value}}" {% endif %}{% if checked %}checked{%
-    endif %}
-    class="w-4 h-4 text-primary-600 bg-neutral-100 border-neutral-300 focus:ring-primary-500 dark:focus:ring-primary-600 dark:ring-offset-neutral-800 focus:ring-2 dark:bg-neutral-700 dark:border-neutral-600"
-    {% if onclick %}onclick="{{onclick}}" {% endif %} {%if disabled%}disabled{%endif%}>
-  <label for="{{id}}" class="ms-2 text-sm font-medium text-neutral-900 dark:text-neutral-300">{{label}}</label>
+{# def
+label,
+name,
+id,
+value,
+checked=false,
+disabled=false,
+onclick="",
+class_="""
+bg-neutral-100
+border-neutral-300
+w-4
+h-4
+text-primary-600
+focus:ring-2
+focus:ring-primary-500
+dark:bg-neutral-700
+dark:border-neutral-600
+dark:focus:ring-primary-600
+dark:ring-offset-neutral-800
+""",
+label_class="ms-2 text-sm font-medium text-neutral-900 dark:text-neutral-300",
+div_class="flex items-center mb-4"
+#}
+<div class="{{div_class}}">
+  <input type="radio" name="{{name}}" id="{{id}}" value="{{value}}" {% if checked %}checked{% endif %}
+    class="{{attrs.class or class_}}" {% if onclick %}onclick="{{onclick}}" {% endif %} {%if
+    disabled%}disabled{%endif%}>
+  <Label for={id} class={label_class}>{{label}}</Label>
 </div>
```

### Comparing `fastlifeweb-0.3.1/src/fastlife/templates/pydantic_form/Sequence.jinja` & `fastlifeweb-0.4.0/src/fastlife/templates/pydantic_form/Sequence.jinja`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 {# def widget, children_widgets, type #}
 
 <pydantic_form.Widget widget={widget} removable={widget.removable}>
   <details id="{{widget.id}}" open>
     <summary class="justify-between items-center font-medium cursor-pointer">
-      <h4 class="inline font-sans text-3xl font-bold">{{widget.title}}</h4>
+      <H3>{{widget.title}}</H3>
     </summary>
     <div>
       {% set fnGetName = "get" + widget.id.replace("-", "_") %}
       <script>
-        function {{fnGetName}}() {
+        function {{ fnGetName }} () {
           const el = document.getElementById("{{widget.id}}-content");
           const len = el.dataset.length;
           el.dataset.length = parseInt(len) + 1;
           return "{{type.name}}." + len;
         }
       </script>
 
@@ -24,14 +24,14 @@
         </div>
         {% endfor%}
       </div>
       <div>
         {% set container_id = "#" + widget.id + "-container" %}
         {% set add_id = widget.id + "-add" %}
         {% set vals = 'js:{"name": '+ fnGetName + '(), "token": "' + type.token + '", "removable": true}' %}
-        <Button type="button" target={container_id} swap="beforeend" id={add_id} vals={vals} get={type.url}>
+        <Button type="button" hx-target={container_id} hx-swap="beforeend" id={add_id} hx-vals={vals} hx-get={type.url}>
           Add
         </Button>
       </div>
     </div>
   </details>
 </pydantic_form.Widget>
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 {# def widget, children_widgets, type #}
-****** {{{{wwiiddggeett..ttiittllee}}}} ******
+******** {{{{wwiiddggeett..ttiittllee}}}} ********
 {% set fnGetName = "get" + widget.id.replace("-", "_") %}
 {% for child in children_widgets %} {% set container_id = widget.id + "-
 container" %}
 {{ child }}
 {% endfor%}
 {% set container_id = "#" + widget.id + "-container" %} {% set add_id =
 widget.id + "-add" %} {% set vals = 'js:{"name": '+ fnGetName + '(), "token":
```

### Comparing `fastlifeweb-0.3.1/src/fastlife/templates/pydantic_form/Union.jinja` & `fastlifeweb-0.4.0/src/fastlife/templates/pydantic_form/Union.jinja`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 {# def widget, child, types, parent_type #}
 
 <pydantic_form.Widget widget={widget}>
   <div id="{{widget.id}}">
     <details open>
       <summary class="justify-between items-center font-medium cursor-pointer">
-        <h4 class="inline font-sans text-3xl font-bold">{{widget.title}}</h4>
+        <H3>{{widget.title}}</H3>
       </summary>
       <div hx-sync="this" id="{{widget.id}}-child">
         {% if child %}
         {{ child }}
         {% else %}
         {% for typ in types %}
-        <Button type="button" target="closest div" get={typ.url} vals={typ.params|tojson}
-          id={typ.fullname + "-" + widget.token}
+        <Button type="button" hx-target="closest div" hx-get={typ.url} hx-vals={typ.params|tojson}
+          id={typ.id}
           onclick={"document.getElementById('" + widget.id +"-remove-btn').hidden=false"}>{{typ.title}}</Button>
         {% endfor %}
         {% endif %}
       </div>
-      <Button type="button" id={widget.id + "-remove-btn" } target={"#" + widget.id} vals={parent_type.params|tojson}
-        get={parent_type.url} hidden={not child}>
+      <Button type="button" id={widget.id + "-remove-btn" } hx-target={"#" + widget.id} hx-vals={parent_type.params|tojson}
+        hx-get={parent_type.url} hidden={not child}>
         Remove
       </Button>
     </details>
   </div>
 </pydantic_form.Widget>
```

### Comparing `fastlifeweb-0.3.1/src/fastlife/templating/renderer/abstract.py` & `fastlifeweb-0.4.0/src/fastlife/templating/renderer/abstract.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,19 +4,15 @@
 from fastapi import Request
 from markupsafe import Markup
 from pydantic.fields import FieldInfo
 
 
 class AbstractTemplateRenderer(abc.ABC):
     route_prefix: str
-    """Used to prefix url to fetch fast life widgets."""
-
-    @abc.abstractmethod
-    def render_page(self, request: Request, template: str, **params: Any) -> str:
-        ...
+    """Used to buid pydantic form"""
 
     @abc.abstractmethod
     def render_template(self, template: str, **params: Any) -> str:
         ...
 
     @abc.abstractmethod
     def pydantic_form(
@@ -25,7 +21,13 @@
         form_data: Mapping[str, Any] | None = None,
         name: str | None = None,
         token: str | None = None,
         removable: bool = False,
         field: FieldInfo | None = None,
     ) -> Markup:
         ...
+
+
+class AbstractTemplateRendererFactory(abc.ABC):
+    @abc.abstractmethod
+    def __call__(self, request: Request) -> AbstractTemplateRenderer:
+        ...
```

### Comparing `fastlifeweb-0.3.1/src/fastlife/templating/renderer/widgets/base.py` & `fastlifeweb-0.4.0/src/fastlife/templating/renderer/widgets/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 import abc
 import secrets
-from typing import Any, Mapping, Optional, Type
+from typing import Any, Generic, Mapping, Optional, Type, TypeVar
 
 from markupsafe import Markup
 
 from fastlife.shared_utils.infer import is_union
 from fastlife.templating.renderer.abstract import AbstractTemplateRenderer
 
+T = TypeVar("T")
+
 
 def get_title(typ: Type[Any]) -> str:
     return getattr(
         getattr(typ, "__meta__", None),
         "title",
         getattr(typ, "__name__", ""),
     )
 
 
-class Widget(abc.ABC):
+class Widget(abc.ABC, Generic[T]):
     name: str
     "variable name, nested variables have dots"
     title: str
     "Human title for the widget"
     aria_label: str
     "Non visible text alternative"
     token: str
@@ -28,20 +30,22 @@
     removable: bool
     "Indicate that the widget is removable from the dom"
 
     def __init__(
         self,
         name: str,
         *,
+        value: Optional[T] = None,
         title: Optional[str] = None,
         token: Optional[str] = None,
         aria_label: Optional[str] = None,
         removable: bool = False,
     ):
         self.name = name
+        self.value = value
         self.title = title or name.split(".")[-1]
         self.aria_label = aria_label or ""
         self.token = token or secrets.token_urlsafe(4).replace("_", "-")
         self.removable = removable
         self.id = f"{self.name}-{self.token}".replace("_", "-").replace(".", "-")
 
     @abc.abstractmethod
@@ -76,14 +80,20 @@
         self.token = token
 
     @property
     def fullname(self) -> str:
         return _get_fullname(self.typ)
 
     @property
+    def id(self) -> str:
+        name = self.name.replace("_", "-").replace(".", "-").replace(":", "-")
+        typ = self.typ.__name__.replace("_", "-")
+        return f"{name}-{typ}-{self.token}"
+
+    @property
     def params(self) -> Mapping[str, str]:
         return {"name": self.name, "token": self.token, "title": self.title}
 
     @property
     def url(self) -> str:
         ret = f"{self.route_prefix}/pydantic-form/widgets/{self.fullname}"
         return ret
```

### Comparing `fastlifeweb-0.3.1/src/fastlife/templating/renderer/widgets/dropdown.py` & `fastlifeweb-0.4.0/src/fastlife/templating/renderer/widgets/dropdown.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 from typing import Optional, Sequence, Tuple
 
 from .base import Widget
 
 
-class DropDownWidget(Widget):
+class DropDownWidget(Widget[str]):
     def __init__(
         self,
         name: str,
         *,
         title: Optional[str],
+        value: Optional[str] = None,
         options: Sequence[Tuple[str, str]] | Sequence[str],
         removable: bool = False,
-        value: str = "",
         token: Optional[str] = None,
-        help_text: Optional[str] = None,
+        hint: Optional[str] = None,
     ) -> None:
-        super().__init__(name, title=title, token=token, removable=removable)
+        super().__init__(
+            name, value=value, title=title, token=token, removable=removable
+        )
         self.options: list[dict[str, str]] = []
         for opt in options:
             if isinstance(opt, tuple):
                 self.options.append({"value": opt[0], "text": opt[1]})
             else:
                 self.options.append({"value": opt, "text": opt})
-        self.value = value
-        self.help_text = help_text
+        self.hint = hint
 
     def get_template(self) -> str:
         return "pydantic_form.Dropdown"
```

### Comparing `fastlifeweb-0.3.1/src/fastlife/templating/renderer/widgets/factory.py` & `fastlifeweb-0.4.0/src/fastlife/templating/renderer/widgets/factory.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import secrets
 from collections.abc import MutableSequence, Sequence
 from decimal import Decimal
 from types import NoneType
-from typing import Any, Literal, Mapping, Optional, Type, get_origin
+from typing import Any, Literal, Mapping, Optional, Type, cast, get_origin
 from uuid import UUID
 
 from markupsafe import Markup
 from pydantic import BaseModel, EmailStr, SecretStr, ValidationError
 from pydantic.fields import FieldInfo
 
 from fastlife.shared_utils.infer import is_complex_type, is_union
@@ -44,15 +44,15 @@
         self,
         base: Type[Any],
         form_data: Mapping[str, Any],
         *,
         prefix: str,
         removable: bool,
         field: FieldInfo | None = None,
-    ) -> Widget:
+    ) -> Widget[Any]:
         return self.build(
             base,
             value=form_data.get(prefix, {}),
             name=prefix,
             removable=removable,
             field=field,
         )
@@ -61,15 +61,30 @@
         self,
         typ: Type[Any],
         *,
         name: str = "",
         value: Any,
         removable: bool,
         field: FieldInfo | None = None,
-    ) -> Widget:
+    ) -> Widget[Any]:
+        if field and field.metadata:
+            for widget in field.metadata:
+                if issubclass(widget, Widget):
+                    return cast(
+                        Widget[Any],
+                        widget(
+                            name,
+                            value=value,
+                            removable=removable,
+                            title=field.title if field else "",
+                            aria_label=field.description if field else None,
+                            token=self.token,
+                        ),
+                    )
+
         type_origin = get_origin(typ)
         if type_origin:
             if is_union(typ):
                 return self.build_union(name, typ, field, value, removable)
 
             if (
                 type_origin is Sequence
@@ -83,63 +98,65 @@
 
         if issubclass(typ, BaseModel):  # if it raises here, the type_origin is unknown
             return self.build_model(name, typ, field, value or {}, removable)
 
         if issubclass(typ, bool):
             return self.build_boolean(name, typ, field, value or False, removable)
 
-        if issubclass(typ, EmailStr):
+        if issubclass(typ, EmailStr):  # type: ignore
             return self.build_emailtype(name, typ, field, value or "", removable)
 
         if issubclass(typ, SecretStr):
             return self.build_secretstr(name, typ, field, value or "", removable)
 
         if issubclass(typ, (int, str, float, Decimal, UUID)):
             return self.build_simpletype(name, typ, field, value or "", removable)
 
-        raise NotImplementedError(f"{typ} not implemented")
+        raise NotImplementedError(f"{typ} not implemented")  # coverage: ignore
 
     def build_model(
         self,
         field_name: str,
         typ: Type[BaseModel],
         field: Optional[FieldInfo],
         value: Mapping[str, Any],
         removable: bool,
-    ) -> Widget:
+    ) -> Widget[Any]:
         ret: dict[str, Any] = {}
         for key, field in typ.model_fields.items():
             child_key = f"{field_name}.{key}" if field_name else key
             if field.exclude:
                 continue
             if field.annotation is None:
-                raise ValueError(f"Missing annotation for {field} in {child_key}")
+                raise ValueError(  # coverage: ignore
+                    f"Missing annotation for {field} in {child_key}"
+                )
             ret[key] = self.build(
                 field.annotation,
                 name=child_key,
                 field=field,
                 value=value.get(key),
                 removable=False,
             )
         return ModelWidget(
             field_name,
-            children_widget=list(ret.values()),
+            value=list(ret.values()),
             removable=removable,
             title=get_title(typ),
             token=self.token,
         )
 
     def build_union(
         self,
         field_name: str,
         field_type: Type[Any],
         field: Optional[FieldInfo],
         value: Any,
         removable: bool,
-    ) -> Widget:
+    ) -> Widget[Any]:
         types: list[Type[Any]] = []
         # required = True
         for typ in field_type.__args__:  # type: ignore
             if typ is NoneType:
                 # required = False
                 continue
             types.append(typ)  # type: ignore
@@ -168,15 +185,15 @@
                         value=value,
                         removable=False,
                     )
 
         widget = UnionWidget(
             field_name,
             # we assume those types are BaseModel
-            child=child,
+            value=child,
             children_types=types,  # type: ignore
             title=field.title if field else "",
             token=self.token,
             removable=removable,
         )
 
         return widget
@@ -184,45 +201,45 @@
     def build_sequence(
         self,
         field_name: str,
         field_type: Type[Any],
         field: Optional[FieldInfo],
         value: Optional[Sequence[Any]],
         removable: bool,
-    ) -> Widget:
+    ) -> Widget[Any]:
         typ = field_type.__args__[0]  # type: ignore
         value = value or []
         items = [
             self.build(
                 typ,  # type: ignore
                 name=f"{field_name}.{idx}",
                 value=v,
                 field=field,
                 removable=True,
             )
             for idx, v in enumerate(value)
         ]
         return SequenceWidget(
             field_name,
-            help_text=field.description if field else "",
+            hint=field.description if field else "",
             title=field.title if field else "",
-            items=items,
+            value=items,
             item_type=typ,  # type: ignore
             token=self.token,
             removable=removable,
         )
 
     def build_boolean(
         self,
         field_name: str,
         field_type: Type[Any],
         field: FieldInfo | None,
         value: bool,
         removable: bool,
-    ) -> Widget:
+    ) -> Widget[Any]:
         return BooleanWidget(
             field_name,
             removable=removable,
             title=field.title if field else "",
             token=self.token,
             value=value,
         )
@@ -230,18 +247,18 @@
     def build_emailtype(
         self,
         field_name: str,
         field_type: Type[Any],
         field: FieldInfo | None,
         value: str | int | float,
         removable: bool,
-    ) -> Widget:
+    ) -> Widget[Any]:
         return TextWidget(
             field_name,
-            help_text=field.description if field else "",
+            hint=field.description if field else "",
             input_type="email",
             placeholder=str(field.examples[0]) if field and field.examples else None,
             removable=removable,
             title=field.title if field else "",
             token=self.token,
             value=str(value),
         )
@@ -249,18 +266,18 @@
     def build_secretstr(
         self,
         field_name: str,
         field_type: Type[Any],
         field: FieldInfo | None,
         value: SecretStr | str,
         removable: bool,
-    ) -> Widget:
+    ) -> Widget[Any]:
         return TextWidget(
             field_name,
-            help_text=field.description if field else "",
+            hint=field.description if field else "",
             input_type="password",
             placeholder=str(field.examples[0]) if field and field.examples else None,
             removable=removable,
             title=field.title if field else "",
             token=self.token,
             value=value.get_secret_value() if isinstance(value, SecretStr) else value,
         )
@@ -268,15 +285,15 @@
     def build_literal(
         self,
         field_name: str,
         field_type: Type[Any],  # a literal actually
         field: FieldInfo | None,
         value: str | int | float,
         removable: bool,
-    ) -> Widget:
+    ) -> Widget[Any]:
         choices: list[str] = field_type.__args__  # type: ignore
         if len(choices) == 1:
             return HiddenWidget(
                 field_name,
                 value=choices[0],
                 token=self.token,
             )
@@ -292,18 +309,18 @@
     def build_simpletype(
         self,
         field_name: str,
         field_type: Type[Any],
         field: FieldInfo | None,
         value: str | int | float,
         removable: bool,
-    ) -> Widget:
+    ) -> Widget[Any]:
         return TextWidget(
             field_name,
-            help_text=field.description if field else None,
+            hint=field.description if field else None,
             placeholder=str(field.examples[0]) if field and field.examples else None,
             aria_label=field.description if field else None,
             removable=removable,
             title=field.title if field else "",
             token=self.token,
             value=str(value),
         )
```

### Comparing `fastlifeweb-0.3.1/src/fastlife/templating/renderer/widgets/model.py` & `fastlifeweb-0.4.0/src/fastlife/templating/renderer/widgets/model.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,33 +1,34 @@
-from typing import Sequence
+from typing import Any, Sequence
 
 from markupsafe import Markup
 
 from fastlife.templating.renderer.abstract import AbstractTemplateRenderer
 
 from .base import Widget
 
 
-class ModelWidget(Widget):
+class ModelWidget(Widget[Sequence[Widget[Any]]]):
     def __init__(
         self,
         name: str,
         *,
-        children_widget: Sequence[Widget],
+        value: Sequence[Widget[Any]],
         removable: bool,
         title: str,
         token: str,
     ):
-        super().__init__(name, title=title, removable=removable, token=token)
-        self.children_widget = children_widget
+        super().__init__(
+            name, title=title, value=value, removable=removable, token=token
+        )
 
     def get_template(self) -> str:
         return "pydantic_form.Model"
 
     def to_html(self, renderer: AbstractTemplateRenderer) -> Markup:
         """Return the html version"""
-        children_widget = [child.to_html(renderer) for child in self.children_widget]
+        children_widget = [child.to_html(renderer) for child in self.value or []]
         kwargs = {
             "widget": self,
             "children_widget": children_widget,
         }
         return Markup(renderer.render_template(self.get_template(), **kwargs))
```

### Comparing `fastlifeweb-0.3.1/src/fastlife/templating/renderer/widgets/sequence.py` & `fastlifeweb-0.4.0/src/fastlife/templating/renderer/widgets/union.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,45 +1,54 @@
-from typing import Any, Optional, Sequence, Type
+from typing import Any, Optional, Sequence, Type, Union
 
 from markupsafe import Markup
+from pydantic import BaseModel
 
 from fastlife.templating.renderer.abstract import AbstractTemplateRenderer
 
 from .base import TypeWrapper, Widget
 
 
-class SequenceWidget(Widget):
-    items: Sequence[Widget]
-
+class UnionWidget(Widget[Widget[Any]]):
     def __init__(
         self,
         name: str,
         *,
         title: Optional[str],
-        help_text: Optional[str],
-        items: Optional[Sequence[Widget]],
-        item_type: Type[Any],
+        value: Optional[Widget[Any]],
+        children_types: Sequence[Type[BaseModel]],
         token: str,
         removable: bool,
     ):
-        super().__init__(name, title=title, token=token, removable=removable)
-        self.items = items or []
-        self.item_type = item_type
-        self.help_text = help_text
+        super().__init__(
+            name, value=value, title=title, token=token, removable=removable
+        )
+        self.children_types = children_types
+        self.parent_name = name
 
-    def get_template(self) -> str:
-        return "pydantic_form/Sequence"
+    def build_types(self, route_prefix: str) -> Sequence[TypeWrapper]:
+        return [
+            TypeWrapper(typ, route_prefix, self.name, self.token)
+            for typ in self.children_types
+        ]
 
-    def build_item_type(self, route_prefix: str) -> TypeWrapper:
-        return TypeWrapper(self.item_type, route_prefix, self.name, self.token)
+    def get_template(self) -> str:
+        return "pydantic_form.Union"
 
     def to_html(self, renderer: "AbstractTemplateRenderer") -> Markup:
         """Return the html version"""
-        children = [Markup(item.to_html(renderer)) for item in self.items]
+        child = Markup(self.value.to_html(renderer)) if self.value else ""
         return Markup(
             renderer.render_template(
                 self.get_template(),
                 widget=self,
-                type=self.build_item_type(renderer.route_prefix),
-                children_widgets=children,
+                types=self.build_types(renderer.route_prefix),
+                parent_type=TypeWrapper(
+                    Union[tuple(self.children_types)],  # type: ignore
+                    renderer.route_prefix,
+                    self.parent_name,
+                    self.token,
+                    title=self.title,
+                ),
+                child=child,
             )
         )
```

### Comparing `fastlifeweb-0.3.1/src/fastlife/templating/renderer/widgets/text.py` & `fastlifeweb-0.4.0/src/fastlife/templating/renderer/widgets/text.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,29 +1,33 @@
 from typing import Optional
 
 from .base import Widget
 
 
-class TextWidget(Widget):
+class TextWidget(Widget[str]):
     def __init__(
         self,
         name: str,
         *,
         title: Optional[str],
         aria_label: Optional[str] = None,
         placeholder: Optional[str] = None,
         removable: bool = False,
         value: str = "",
         token: Optional[str] = None,
-        help_text: Optional[str] = None,
+        hint: Optional[str] = None,
         input_type: str = "text"
     ) -> None:
         super().__init__(
-            name, title=title, aria_label=aria_label, token=token, removable=removable
+            name,
+            value=value,
+            title=title,
+            aria_label=aria_label,
+            token=token,
+            removable=removable,
         )
         self.placeholder = placeholder or ""
-        self.value = value
-        self.help_text = help_text
+        self.hint = hint
         self.input_type = input_type
 
     def get_template(self) -> str:
         return "pydantic_form.Text"
```

### Comparing `fastlifeweb-0.3.1/src/fastlife/testing/testclient.py` & `fastlifeweb-0.4.0/src/fastlife/testing/testclient.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,27 @@
 import re
 import time
 from collections.abc import MutableMapping
+from http.cookiejar import Cookie
 from typing import Any, Iterator, Literal, Mapping, Optional, Sequence
 from urllib.parse import urlencode
 
 import bs4
 import httpx
 from fastapi.testclient import TestClient
+from multidict import MultiDict
 from starlette.types import ASGIApp
 
 from fastlife.configurator.settings import Settings
 from fastlife.session.serializer import AbsractSessionSerializer
 from fastlife.shared_utils.resolver import resolve
 
+CookieTypes = httpx._types.CookieTypes  # type: ignore
+Cookies = httpx._models.Cookies  # type: ignore
+
 
 class Element:
     def __init__(self, client: "WebTestClient", tag: bs4.Tag):
         self._client = client
         self._tag = tag
 
     def click(self) -> "WebResponse":
@@ -31,28 +36,28 @@
         return self._tag.attrs
 
     @property
     def text(self) -> str:
         return self._tag.text.strip()
 
     @property
-    def form(self) -> "Element | None":
-        return Element(self._client, self._tag.form) if self._tag.form else None
-
-    @property
     def h1(self) -> "Element":
         nodes = self.by_node_name("h1")
         assert len(nodes) == 1, f"Should have 1 <h1>, got {len(nodes)} in {self}"
         return nodes[0]
 
     @property
     def h2(self) -> Sequence["Element"]:
         return self.by_node_name("h2")
 
     @property
+    def form(self) -> "Element | None":
+        return Element(self._client, self._tag.form) if self._tag.form else None
+
+    @property
     def hx_target(self) -> Optional[str]:
         el: bs4.Tag | None = self._tag
         while el:
             if "hx-target" in el.attrs:
                 ret = el.attrs["hx-target"]
                 if ret == "this":
                     ret = el.attrs["id"]
@@ -111,65 +116,138 @@
 
 class WebForm:
     def __init__(self, client: "WebTestClient", origin: str, form: Element):
         self._client = client
         self._form = form
         self._origin = origin
         self._formfields: dict[str, Element] = {}
-        self._formdata: dict[str, str] = {}
+        self._formdata: MultiDict[str] = MultiDict()
         inputs = self._form.by_node_name("input")
         for input in inputs:
             self._formfields[input.attrs["name"]] = input
             if input.attrs.get("type") == "checkbox" and "checked" not in input.attrs:
                 continue
-            self._formdata[input.attrs["name"]] = input.attrs.get("value", "")
+            self._formdata.add(input.attrs["name"], input.attrs.get("value", ""))
 
-        inputs = self._form.by_node_name("select")
-        for input in inputs:
-            self._formfields[input.attrs["name"]] = input
-            for option in input.by_node_name("options"):
-                if "selected" in option.attrs:
-                    self._formdata[input.attrs["name"]] = option.attrs.get(
-                        "value", option.text
+        selects = self._form.by_node_name("select")
+        for select in selects:
+            fieldname = select.attrs["name"]
+            self._formfields[fieldname] = select
+            options = select.by_node_name("option")
+            if "multiple" in select.attrs:
+                for option in options:
+                    if "selected" in option.attrs:
+                        self._formdata.add(
+                            fieldname, option.attrs.get("value", option.text)
+                        )
+            else:
+                if options:
+                    self._formdata[fieldname] = options[0].attrs.get(
+                        "value", options[0].text
                     )
+                    for option in options:
+                        if "selected" in option.attrs:
+                            self._formdata[fieldname] = option.attrs.get(
+                                "value", option.text
+                            )
+                            break
+
         # field textearea...
 
     def set(self, fieldname: str, value: str) -> Any:
         if fieldname not in self._formfields:
-            raise ValueError(f"{fieldname} does not exists")
+            raise ValueError(f'"{fieldname}" does not exists')
         if self._formfields[fieldname].node_name == "select":
-            raise RuntimeError(f"{fieldname} is a <select>, use select() instead")
+            raise ValueError(f'"{fieldname}" is a <select>, use select() instead')
+
+        if self._formfields[fieldname].attrs.get("type") == "checkbox":
+            self._formdata.add(fieldname, value)
+            return
+
+        if self._formfields[fieldname].attrs.get("type") == "radio":
+            radio = self._form.by_node_name(
+                "input", attrs={"type": "radio", "value": value}
+            )
+            if not radio:
+                raise ValueError(
+                    f'radio "{fieldname}" does not contains {value} option'
+                )
+
         self._formdata[fieldname] = value
 
+    def unset(self, fieldname: str, value: str) -> Any:
+        if fieldname not in self._formfields:
+            raise ValueError(f'"{fieldname}" does not exists')
+        if self._formfields[fieldname].node_name != "input":
+            raise ValueError(f'"{fieldname}" is not a checkbox')
+        if self._formfields[fieldname].attrs.get("type") != "checkbox":
+            raise ValueError(f'"{fieldname}" is not a checkbox')
+        values = self._formdata.popall(fieldname)
+        if value not in values:
+            raise ValueError(f'"{value}" not in "{fieldname}"')
+        for val in values:
+            if val != value:
+                self._formdata[fieldname] = val
+
     def select(self, fieldname: str, value: str) -> Any:
         if fieldname not in self._formfields:
-            raise ValueError(f"{fieldname} does not exists")
-        if self._formfields[fieldname].node_name != "select":
-            raise RuntimeError(
-                f"{fieldname} is a <{self._formfields[fieldname]}>, use set() instead"
+            raise ValueError(f'"{fieldname}" does not exists')
+        field = self._formfields[fieldname]
+        if field.node_name != "select":
+            raise ValueError(f"{fieldname} is a {repr(field)}, " "use set() instead")
+
+        for option in field.by_node_name("option"):
+            if option.text == value.strip():
+                if "multiple" in field.attrs:
+                    self._formdata.add(fieldname, value)
+                else:
+                    self._formdata[fieldname] = option.attrs.get("value", option.text)
+                break
+        else:
+            raise ValueError(f'No option {value} in <select name="{fieldname}">')
+
+    def unselect(self, fieldname: str, value: str) -> Any:
+        if fieldname not in self._formfields:
+            raise ValueError(f'"{fieldname}" does not exists')
+        field = self._formfields[fieldname]
+
+        if field.node_name != "select":
+            raise ValueError(
+                f"{fieldname} is a {repr(self._formfields[fieldname])}, "
+                "use unset() for checkbox instead"
             )
-        if "multiple" in self._formfields[fieldname].attrs:
-            raise NotImplementedError
+        if "multiple" not in field.attrs:
+            raise ValueError("only <select multiple> support unselect")
+
         for option in self._formfields[fieldname].by_node_name("option"):
             if option.text == value.strip():
-                self._formdata[fieldname] = option.attrs.get("value", option.text)
+                values = self._formdata.popall(fieldname)
+                if value not in values:
+                    raise ValueError(f'"{value}" not selected in "{fieldname}"')
+                for val in values:
+                    if val != value:
+                        self._formdata[fieldname] = val
                 break
         else:
             raise ValueError(f'No option {value} in <select name="{fieldname}">')
 
     def button(self, text: str, position: int = 0) -> "WebForm":
         buttons = self._form.get_all_by_text(text, node_name="button")
-        assert len(buttons) > position, f'Button "{text}" not found'
+        if position >= len(buttons):
+            pos = ""
+            if position > 0:
+                pos = f" at position {position}"
+            raise ValueError(f'Button "{text}" not found{pos}')
         button = buttons[position]
         if "name" in button.attrs:
             self._formdata[button.attrs["name"]] = button.attrs.get("value", "")
         return self
 
     def submit(self, follow_redirects: bool = True) -> "WebResponse":
-        headers = {}
+        headers: dict[str, str] = {}
         target = (
             self._form.attrs.get("hx-post")
             or self._form.attrs.get("post")
             or self._origin
         )
         if "hx-post" in self._form.attrs:
             if hx_target := self._form.hx_target:
@@ -195,20 +273,20 @@
         self._form: WebForm | None = None
 
     @property
     def status_code(self) -> int:
         return self._response.status_code
 
     @property
-    def is_redirect(self) -> int:
+    def is_redirect(self) -> bool:
         return 300 <= self._response.status_code < 400
 
     @property
     def content_type(self) -> str:
-        return self._response.headers["content-type"]
+        return self._response.headers.get("content-type", "").split(";").pop(0)
 
     @property
     def headers(self) -> httpx.Headers:
         return self._response.headers
 
     @property
     def text(self) -> str:
@@ -242,49 +320,36 @@
 
     def by_node_name(
         self, node_name: str, *, attrs: dict[str, str] | None = None
     ) -> list[Element]:
         return self.html.by_node_name(node_name, attrs=attrs)
 
 
-CookieTypes = httpx._types.CookieTypes  # type: ignore
-Cookies = httpx._models.Cookies  # type: ignore
-
-
 class Session(dict[str, Any]):
     def __init__(self, client: "WebTestClient"):
         self.client = client
-        if client.session_serializer is None:
-            raise RuntimeError(
-                "WebTestClient has not been initialize with the app settings, "
-                "can't decode session"
-            )
-
         self.srlz = client.session_serializer
-        settings = self.client.settings
-        assert settings is not None
-        self.settings = settings
+        self.settings = self.client.settings
         data: Mapping[str, Any]
-        self.has_session = settings.session_cookie_name in self.client.cookies
+        cookie_name = self.settings.session_cookie_name
+        self.has_session = cookie_name in self.client.cookies
         if self.has_session:
             data, error = self.srlz.deserialize(
-                self.client.cookies[settings.session_cookie_name].encode("utf-8")
+                self.client.cookies[cookie_name].encode("utf-8")
             )
             if error:
                 self.has_session = False
         else:
             data = {}
         super().__init__(data)
 
     def __setitem__(self, __key: Any, __value: Any) -> None:
         super().__setitem__(__key, __value)
         settings = self.settings
         data = self.serialize()
-        from http.cookiejar import Cookie
-
         self.client.cookies.jar.set_cookie(
             Cookie(
                 version=0,
                 name=settings.session_cookie_name,
                 value=data,
                 port=None,
                 port_specified=False,
@@ -326,29 +391,25 @@
         if settings is None:
             settings = Settings()
             settings.domain_name = settings.domain_name or "testserver.local"
         self.testclient = TestClient(
             app, base_url=f"http://{settings.domain_name}", cookies=cookies or {}
         )
         self.settings = settings
-        self.session_serializer: AbsractSessionSerializer | None = None
-        if settings:
-            self.session_serializer = resolve(settings.session_serializer)(
-                settings.session_secret_key,
-                int(settings.session_duration.total_seconds()),
-            )
+        self.session_serializer: AbsractSessionSerializer = resolve(
+            settings.session_serializer
+        )(
+            settings.session_secret_key,
+            int(settings.session_duration.total_seconds()),
+        )
 
     @property
     def cookies(self) -> Cookies:
         return self.testclient.cookies
 
-    @cookies.setter
-    def cookies(self, value: Cookies) -> None:
-        self.testclient.cookies = value
-
     @property
     def session(self) -> MutableMapping[str, Any]:
         return Session(self)
 
     def request(
         self,
         method: Literal["GET", "POST"],  # I am a browser
@@ -399,15 +460,15 @@
             url,
             max_redirects=int(follow_redirects) * 10,
         )
 
     def post(
         self,
         url: str,
-        data: Mapping[str, Any],
+        data: MultiDict[str],
         *,
         headers: Mapping[str, Any] | None = None,
         follow_redirects: bool = True,
     ) -> WebResponse:
         if headers is None:
             headers = {}
         return self.request(
```

### Comparing `fastlifeweb-0.3.1/src/fastlife/views/pydantic_form.py` & `fastlifeweb-0.4.0/src/fastlife/views/pydantic_form.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 from typing import Optional
 
-from fastapi import Query, Response
+from fastapi import Query, Request, Response
 from pydantic.fields import FieldInfo
 
 from fastlife import Configurator, configure
 from fastlife.configurator.registry import Registry
 from fastlife.shared_utils.resolver import resolve_extended
 
 
 async def show_widget(
     typ: str,
     reg: Registry,
+    request: Request,
     title: Optional[str] = Query(None),
     name: Optional[str] = Query(None),
     token: Optional[str] = Query(None),
     removable: bool = Query(False),
 ) -> Response:
     model_cls = resolve_extended(typ)
     field = None
     if title:
         field = FieldInfo(title=title)
-    data = reg.renderer.pydantic_form(model_cls, None, name, token, removable, field)
+    data = reg.renderer(request).pydantic_form(
+        model_cls, None, name, token, removable, field
+    )
     return Response(data, headers={"Content-Type": "text/html"})
 
 
 @configure
 def includeme(config: Configurator) -> None:
     route_prefix = config.registry.settings.fastlife_route_prefix
     config.add_route(
```

### Comparing `fastlifeweb-0.3.1/PKG-INFO` & `fastlifeweb-0.4.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: fastlifeweb
-Version: 0.3.1
+Version: 0.4.0
 Summary: High-level web framework
+Home-page: https://github.com/mardiros/fastlife
 License: BSD-derived
 Author: Guillaume Gauvrit
 Author-email: guillaume@gauvr.it
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: AsyncIO
 Classifier: Intended Audience :: Developers
@@ -16,20 +17,22 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: beautifulsoup4[testing] (>=4.12.2,<5.0.0)
 Requires-Dist: behave (>=1.2.6,<2.0.0)
 Requires-Dist: fastapi (>=0.110.0,<0.111.0)
 Requires-Dist: itsdangerous (>=2.1.2,<3.0.0)
-Requires-Dist: jinjax (>=0.31,<0.32)
+Requires-Dist: jinjax (>=0.32,<0.33)
 Requires-Dist: markupsafe (>=2.1.3,<3.0.0)
+Requires-Dist: multidict (>=6.0.5,<7.0.0)
 Requires-Dist: pydantic (>=2.3.0,<3.0.0)
 Requires-Dist: pydantic-settings (>=2.0.3,<3.0.0)
 Requires-Dist: python-multipart (>=0.0.6,<0.0.7)
 Requires-Dist: venusian (>=3.0.0,<4.0.0)
+Project-URL: Repository, https://github.com/mardiros/fastlife
 Description-Content-Type: text/markdown
 
 # Fastlife
 
 [![CI](https://github.com/mardiros/fastlife/actions/workflows/main.yml/badge.svg)](https://github.com/mardiros/fastlife/actions/workflows/main.yml)
 
 [![codecov](https://codecov.io/gh/mardiros/fastlife/graph/badge.svg?token=DTpi73d7mf)](https://codecov.io/gh/mardiros/fastlife)
@@ -40,9 +43,7 @@
 The intention is to prototype fast application.
 
 Under heavy development.
 
 
 The package is available on pypi with the name fastlifeweb.
 
-The name fastlife is squatted and I am tired of PEP 541 requests.
-
```

