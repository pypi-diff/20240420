# Comparing `tmp/wikiteam3-4.2.5.tar.gz` & `tmp/wikiteam3-4.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wikiteam3-4.2.5.tar", max compression
+gzip compressed data, was "wikiteam3-4.2.6.tar", max compression
```

## Comparing `wikiteam3-4.2.5.tar` & `wikiteam3-4.2.6.tar`

### file list

```diff
@@ -1,65 +1,65 @@
--rw-r--r--   0        0        0    35121 2024-03-06 03:04:21.649498 wikiteam3-4.2.5/LICENSE
--rw-r--r--   0        0        0    16107 2024-03-10 09:50:28.696990 wikiteam3-4.2.5/README.md
--rw-r--r--   0        0        0     2043 2024-04-08 13:47:32.033662 wikiteam3-4.2.5/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-06 03:04:22.145501 wikiteam3-4.2.5/wikiteam3/__init__.py
--rwxr-xr-x   0        0        0      155 2024-03-06 03:04:22.145501 wikiteam3-4.2.5/wikiteam3/dumpgenerator/__init__.py
--rw-r--r--   0        0        0       94 2024-03-06 03:04:22.145501 wikiteam3-4.2.5/wikiteam3/dumpgenerator/__main__.py
--rw-r--r--   0        0        0      193 2024-03-06 03:04:22.145501 wikiteam3-4.2.5/wikiteam3/dumpgenerator/api/__init__.py
--rw-r--r--   0        0        0     5233 2024-03-06 03:04:22.145501 wikiteam3-4.2.5/wikiteam3/dumpgenerator/api/api.py
--rw-r--r--   0        0        0      415 2024-04-08 12:30:05.560295 wikiteam3-4.2.5/wikiteam3/dumpgenerator/api/get_json.py
--rw-r--r--   0        0        0     1110 2024-03-06 03:04:22.145501 wikiteam3-4.2.5/wikiteam3/dumpgenerator/api/handle_status_code.py
--rw-r--r--   0        0        0     3019 2024-03-06 03:04:22.145501 wikiteam3-4.2.5/wikiteam3/dumpgenerator/api/index_check.py
--rw-r--r--   0        0        0     3483 2024-04-08 13:47:16.853117 wikiteam3-4.2.5/wikiteam3/dumpgenerator/api/namespaces.py
--rw-r--r--   0        0        0     9971 2024-03-06 03:04:22.145501 wikiteam3-4.2.5/wikiteam3/dumpgenerator/api/page_titles.py
--rw-r--r--   0        0        0     5480 2024-03-06 03:04:22.145501 wikiteam3-4.2.5/wikiteam3/dumpgenerator/api/wiki_check.py
--rw-r--r--   0        0        0       91 2024-03-06 03:04:22.145501 wikiteam3-4.2.5/wikiteam3/dumpgenerator/cli/__init__.py
--rw-r--r--   0        0        0    22478 2024-04-08 13:18:29.425069 wikiteam3-4.2.5/wikiteam3/dumpgenerator/cli/cli.py
--rw-r--r--   0        0        0     1948 2024-03-06 03:04:22.145501 wikiteam3-4.2.5/wikiteam3/dumpgenerator/cli/delay.py
--rw-r--r--   0        0        0      980 2024-03-06 03:04:22.145501 wikiteam3-4.2.5/wikiteam3/dumpgenerator/cli/greeter.py
--rw-r--r--   0        0        0     3092 2024-04-08 12:43:00.924209 wikiteam3-4.2.5/wikiteam3/dumpgenerator/config.py
--rw-r--r--   0        0        0       37 2024-03-06 03:04:22.145501 wikiteam3-4.2.5/wikiteam3/dumpgenerator/dump/__init__.py
--rw-r--r--   0        0        0    12817 2024-04-08 12:46:20.286521 wikiteam3-4.2.5/wikiteam3/dumpgenerator/dump/generator.py
--rw-r--r--   0        0        0        0 2024-03-06 03:04:22.145501 wikiteam3-4.2.5/wikiteam3/dumpgenerator/dump/image/__init__.py
--rw-r--r--   0        0        0     2576 2024-03-06 03:04:22.145501 wikiteam3-4.2.5/wikiteam3/dumpgenerator/dump/image/html_regexs.py
--rw-r--r--   0        0        0     4620 2024-03-06 03:04:22.145501 wikiteam3-4.2.5/wikiteam3/dumpgenerator/dump/image/html_regexs_test.py
--rw-r--r--   0        0        0    32910 2024-04-08 12:59:53.869416 wikiteam3-4.2.5/wikiteam3/dumpgenerator/dump/image/image.py
--rw-r--r--   0        0        0        0 2024-03-06 03:04:22.145501 wikiteam3-4.2.5/wikiteam3/dumpgenerator/dump/misc/__init__.py
--rw-r--r--   0        0        0      879 2024-03-06 03:04:22.145501 wikiteam3-4.2.5/wikiteam3/dumpgenerator/dump/misc/index_php.py
--rw-r--r--   0        0        0     2638 2024-04-08 12:19:09.606864 wikiteam3-4.2.5/wikiteam3/dumpgenerator/dump/misc/site_info.py
--rw-r--r--   0        0        0      505 2024-03-06 03:04:22.145501 wikiteam3-4.2.5/wikiteam3/dumpgenerator/dump/misc/site_info_test.py
--rw-r--r--   0        0        0     1007 2024-03-06 03:04:22.145501 wikiteam3-4.2.5/wikiteam3/dumpgenerator/dump/misc/special_logs.py
--rw-r--r--   0        0        0     1009 2024-03-06 03:04:22.145501 wikiteam3-4.2.5/wikiteam3/dumpgenerator/dump/misc/special_version.py
--rw-r--r--   0        0        0        0 2024-03-06 03:04:22.145501 wikiteam3-4.2.5/wikiteam3/dumpgenerator/dump/page/__init__.py
--rw-r--r--   0        0        0        0 2024-03-06 03:04:22.145501 wikiteam3-4.2.5/wikiteam3/dumpgenerator/dump/page/xmlexport/__init__.py
--rw-r--r--   0        0        0      498 2024-03-06 03:04:22.145501 wikiteam3-4.2.5/wikiteam3/dumpgenerator/dump/page/xmlexport/page_xml.py
--rw-r--r--   0        0        0    13522 2024-03-06 03:04:22.145501 wikiteam3-4.2.5/wikiteam3/dumpgenerator/dump/page/xmlexport/page_xml_api.py
--rw-r--r--   0        0        0     8991 2024-03-06 03:04:22.145501 wikiteam3-4.2.5/wikiteam3/dumpgenerator/dump/page/xmlexport/page_xml_export.py
--rw-r--r--   0        0        0        0 2024-03-06 03:04:22.145501 wikiteam3-4.2.5/wikiteam3/dumpgenerator/dump/page/xmlrev/__init__.py
--rw-r--r--   0        0        0    22245 2024-03-06 03:04:22.145501 wikiteam3-4.2.5/wikiteam3/dumpgenerator/dump/page/xmlrev/xml_revisions.py
--rw-r--r--   0        0        0     4783 2024-03-06 03:04:22.145501 wikiteam3-4.2.5/wikiteam3/dumpgenerator/dump/page/xmlrev/xml_revisions_page.py
--rw-r--r--   0        0        0        0 2024-03-06 03:04:22.145501 wikiteam3-4.2.5/wikiteam3/dumpgenerator/dump/xmldump/__init__.py
--rw-r--r--   0        0        0     5780 2024-03-06 03:04:22.145501 wikiteam3-4.2.5/wikiteam3/dumpgenerator/dump/xmldump/xml_dump.py
--rw-r--r--   0        0        0     5240 2024-03-06 03:04:22.145501 wikiteam3-4.2.5/wikiteam3/dumpgenerator/dump/xmldump/xml_header.py
--rw-r--r--   0        0        0      277 2024-03-06 03:04:22.145501 wikiteam3-4.2.5/wikiteam3/dumpgenerator/dump/xmldump/xml_integrity.py
--rw-r--r--   0        0        0     2487 2024-03-06 03:04:22.145501 wikiteam3-4.2.5/wikiteam3/dumpgenerator/dump/xmldump/xml_truncate.py
--rw-r--r--   0        0        0     1144 2024-03-06 03:04:22.145501 wikiteam3-4.2.5/wikiteam3/dumpgenerator/exceptions.py
--rw-r--r--   0        0        0       33 2024-03-06 03:04:22.145501 wikiteam3-4.2.5/wikiteam3/dumpgenerator/log/__init__.py
--rw-r--r--   0        0        0      485 2024-03-06 03:04:22.145501 wikiteam3-4.2.5/wikiteam3/dumpgenerator/log/log_error.py
--rw-r--r--   0        0        0       65 2024-04-08 13:47:44.397985 wikiteam3-4.2.5/wikiteam3/dumpgenerator/version.py
--rw-r--r--   0        0        0       83 2024-03-06 03:04:22.149502 wikiteam3-4.2.5/wikiteam3/uploader/__init__.py
--rw-r--r--   0        0        0       83 2024-03-06 03:04:22.149502 wikiteam3-4.2.5/wikiteam3/uploader/__main__.py
--rw-r--r--   0        0        0     9212 2024-03-08 17:33:56.605131 wikiteam3-4.2.5/wikiteam3/uploader/compresser.py
--rw-r--r--   0        0        0     1733 2024-03-06 03:04:22.149502 wikiteam3-4.2.5/wikiteam3/uploader/socketLock.py
--rw-r--r--   0        0        0    23068 2024-03-08 17:35:52.503064 wikiteam3-4.2.5/wikiteam3/uploader/uploader.py
--rw-r--r--   0        0        0      377 2024-03-06 03:04:22.149502 wikiteam3-4.2.5/wikiteam3/utils/__init__.py
--rw-r--r--   0        0        0     3255 2024-03-06 03:04:22.149502 wikiteam3-4.2.5/wikiteam3/utils/ia_checker.py
--rw-r--r--   0        0        0     3422 2024-03-06 03:04:22.149502 wikiteam3-4.2.5/wikiteam3/utils/identifier.py
--rw-r--r--   0        0        0     1471 2024-03-06 03:04:22.149502 wikiteam3-4.2.5/wikiteam3/utils/login/__init__.py
--rw-r--r--   0        0        0     2380 2024-03-06 03:04:22.149502 wikiteam3-4.2.5/wikiteam3/utils/login/api.py
--rw-r--r--   0        0        0     2157 2024-03-06 03:04:22.149502 wikiteam3-4.2.5/wikiteam3/utils/login/index.py
--rw-r--r--   0        0        0     7701 2024-04-08 13:33:10.207323 wikiteam3-4.2.5/wikiteam3/utils/monkey_patch.py
--rw-r--r--   0        0        0      341 2024-03-06 03:04:22.149502 wikiteam3-4.2.5/wikiteam3/utils/uprint.py
--rw-r--r--   0        0        0    38659 2024-03-06 03:04:22.149502 wikiteam3-4.2.5/wikiteam3/utils/user_agent.py
--rw-r--r--   0        0        0     4686 2024-03-06 03:04:22.149502 wikiteam3-4.2.5/wikiteam3/utils/util.py
--rw-r--r--   0        0        0      779 2024-04-08 12:19:44.152101 wikiteam3-4.2.5/wikiteam3/utils/wiki_avoid.py
--rw-r--r--   0        0        0    18092 1970-01-01 00:00:00.000000 wikiteam3-4.2.5/PKG-INFO
+-rw-r--r--   0        0        0    35121 2024-03-06 03:04:21.649498 wikiteam3-4.2.6/LICENSE
+-rw-r--r--   0        0        0    15951 2024-04-16 09:08:54.076329 wikiteam3-4.2.6/README.md
+-rw-r--r--   0        0        0     2043 2024-04-20 09:16:56.490748 wikiteam3-4.2.6/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-03-06 03:04:22.145501 wikiteam3-4.2.6/wikiteam3/__init__.py
+-rwxr-xr-x   0        0        0      155 2024-04-16 08:42:20.855948 wikiteam3-4.2.6/wikiteam3/dumpgenerator/__init__.py
+-rw-r--r--   0        0        0       94 2024-03-06 03:04:22.145501 wikiteam3-4.2.6/wikiteam3/dumpgenerator/__main__.py
+-rw-r--r--   0        0        0      193 2024-04-12 14:34:34.797759 wikiteam3-4.2.6/wikiteam3/dumpgenerator/api/__init__.py
+-rw-r--r--   0        0        0     5233 2024-04-16 08:42:20.855948 wikiteam3-4.2.6/wikiteam3/dumpgenerator/api/api.py
+-rw-r--r--   0        0        0      415 2024-04-12 14:34:34.797759 wikiteam3-4.2.6/wikiteam3/dumpgenerator/api/get_json.py
+-rw-r--r--   0        0        0     1110 2024-04-12 14:34:34.797759 wikiteam3-4.2.6/wikiteam3/dumpgenerator/api/handle_status_code.py
+-rw-r--r--   0        0        0     3019 2024-04-12 14:34:34.797759 wikiteam3-4.2.6/wikiteam3/dumpgenerator/api/index_check.py
+-rw-r--r--   0        0        0     3483 2024-04-20 09:18:04.969071 wikiteam3-4.2.6/wikiteam3/dumpgenerator/api/namespaces.py
+-rw-r--r--   0        0        0     9971 2024-04-12 14:34:34.797759 wikiteam3-4.2.6/wikiteam3/dumpgenerator/api/page_titles.py
+-rw-r--r--   0        0        0     5480 2024-04-16 08:42:20.855948 wikiteam3-4.2.6/wikiteam3/dumpgenerator/api/wiki_check.py
+-rw-r--r--   0        0        0       91 2024-04-12 14:34:34.797759 wikiteam3-4.2.6/wikiteam3/dumpgenerator/cli/__init__.py
+-rw-r--r--   0        0        0    22238 2024-04-16 11:59:36.759685 wikiteam3-4.2.6/wikiteam3/dumpgenerator/cli/cli.py
+-rw-r--r--   0        0        0     1948 2024-04-16 08:42:20.855948 wikiteam3-4.2.6/wikiteam3/dumpgenerator/cli/delay.py
+-rw-r--r--   0        0        0      980 2024-04-16 08:42:20.855948 wikiteam3-4.2.6/wikiteam3/dumpgenerator/cli/greeter.py
+-rw-r--r--   0        0        0     3197 2024-04-16 12:02:46.643738 wikiteam3-4.2.6/wikiteam3/dumpgenerator/config.py
+-rw-r--r--   0        0        0       37 2024-03-06 03:04:22.145501 wikiteam3-4.2.6/wikiteam3/dumpgenerator/dump/__init__.py
+-rw-r--r--   0        0        0    12158 2024-04-16 08:42:20.855948 wikiteam3-4.2.6/wikiteam3/dumpgenerator/dump/generator.py
+-rw-r--r--   0        0        0        0 2024-03-06 03:04:22.145501 wikiteam3-4.2.6/wikiteam3/dumpgenerator/dump/image/__init__.py
+-rw-r--r--   0        0        0     2576 2024-04-12 14:34:34.801759 wikiteam3-4.2.6/wikiteam3/dumpgenerator/dump/image/html_regexs.py
+-rw-r--r--   0        0        0     4620 2024-04-16 08:42:20.855948 wikiteam3-4.2.6/wikiteam3/dumpgenerator/dump/image/html_regexs_test.py
+-rw-r--r--   0        0        0    32910 2024-04-16 08:42:20.855948 wikiteam3-4.2.6/wikiteam3/dumpgenerator/dump/image/image.py
+-rw-r--r--   0        0        0        0 2024-03-06 03:04:22.145501 wikiteam3-4.2.6/wikiteam3/dumpgenerator/dump/misc/__init__.py
+-rw-r--r--   0        0        0      879 2024-04-12 14:34:34.801759 wikiteam3-4.2.6/wikiteam3/dumpgenerator/dump/misc/index_php.py
+-rw-r--r--   0        0        0     2638 2024-04-16 08:42:20.855948 wikiteam3-4.2.6/wikiteam3/dumpgenerator/dump/misc/site_info.py
+-rw-r--r--   0        0        0      505 2024-04-16 08:42:20.855948 wikiteam3-4.2.6/wikiteam3/dumpgenerator/dump/misc/site_info_test.py
+-rw-r--r--   0        0        0     1007 2024-04-12 14:34:34.801759 wikiteam3-4.2.6/wikiteam3/dumpgenerator/dump/misc/special_logs.py
+-rw-r--r--   0        0        0     1009 2024-04-12 14:34:34.801759 wikiteam3-4.2.6/wikiteam3/dumpgenerator/dump/misc/special_version.py
+-rw-r--r--   0        0        0        0 2024-03-06 03:04:22.145501 wikiteam3-4.2.6/wikiteam3/dumpgenerator/dump/page/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-06 03:04:22.145501 wikiteam3-4.2.6/wikiteam3/dumpgenerator/dump/page/xmlexport/__init__.py
+-rw-r--r--   0        0        0      498 2024-04-12 14:34:34.801759 wikiteam3-4.2.6/wikiteam3/dumpgenerator/dump/page/xmlexport/page_xml.py
+-rw-r--r--   0        0        0    13540 2024-04-16 09:08:54.080329 wikiteam3-4.2.6/wikiteam3/dumpgenerator/dump/page/xmlexport/page_xml_api.py
+-rw-r--r--   0        0        0     8991 2024-04-12 14:34:34.801759 wikiteam3-4.2.6/wikiteam3/dumpgenerator/dump/page/xmlexport/page_xml_export.py
+-rw-r--r--   0        0        0        0 2024-03-06 03:04:22.145501 wikiteam3-4.2.6/wikiteam3/dumpgenerator/dump/page/xmlrev/__init__.py
+-rw-r--r--   0        0        0    24136 2024-04-16 11:43:03.544270 wikiteam3-4.2.6/wikiteam3/dumpgenerator/dump/page/xmlrev/xml_revisions.py
+-rw-r--r--   0        0        0     4841 2024-04-16 12:16:42.470155 wikiteam3-4.2.6/wikiteam3/dumpgenerator/dump/page/xmlrev/xml_revisions_page.py
+-rw-r--r--   0        0        0        0 2024-03-06 03:04:22.145501 wikiteam3-4.2.6/wikiteam3/dumpgenerator/dump/xmldump/__init__.py
+-rw-r--r--   0        0        0     5780 2024-04-16 08:42:20.859948 wikiteam3-4.2.6/wikiteam3/dumpgenerator/dump/xmldump/xml_dump.py
+-rw-r--r--   0        0        0     5240 2024-04-12 14:34:34.801759 wikiteam3-4.2.6/wikiteam3/dumpgenerator/dump/xmldump/xml_header.py
+-rw-r--r--   0        0        0      277 2024-04-12 14:34:34.801759 wikiteam3-4.2.6/wikiteam3/dumpgenerator/dump/xmldump/xml_integrity.py
+-rw-r--r--   0        0        0     2487 2024-04-12 14:34:34.801759 wikiteam3-4.2.6/wikiteam3/dumpgenerator/dump/xmldump/xml_truncate.py
+-rw-r--r--   0        0        0     2265 2024-04-16 11:54:19.674306 wikiteam3-4.2.6/wikiteam3/dumpgenerator/exceptions.py
+-rw-r--r--   0        0        0       33 2024-04-12 14:34:34.801759 wikiteam3-4.2.6/wikiteam3/dumpgenerator/log/__init__.py
+-rw-r--r--   0        0        0      485 2024-04-16 08:42:20.859948 wikiteam3-4.2.6/wikiteam3/dumpgenerator/log/log_error.py
+-rw-r--r--   0        0        0       65 2024-04-20 09:17:02.202942 wikiteam3-4.2.6/wikiteam3/dumpgenerator/version.py
+-rw-r--r--   0        0        0       83 2024-04-12 14:34:34.809759 wikiteam3-4.2.6/wikiteam3/uploader/__init__.py
+-rw-r--r--   0        0        0       83 2024-04-12 14:34:34.809759 wikiteam3-4.2.6/wikiteam3/uploader/__main__.py
+-rw-r--r--   0        0        0     9212 2024-04-16 08:42:20.859948 wikiteam3-4.2.6/wikiteam3/uploader/compresser.py
+-rw-r--r--   0        0        0     1733 2024-04-12 14:34:34.809759 wikiteam3-4.2.6/wikiteam3/uploader/socketLock.py
+-rw-r--r--   0        0        0    23068 2024-04-16 08:42:20.859948 wikiteam3-4.2.6/wikiteam3/uploader/uploader.py
+-rw-r--r--   0        0        0      377 2024-04-12 14:34:34.809759 wikiteam3-4.2.6/wikiteam3/utils/__init__.py
+-rw-r--r--   0        0        0     3255 2024-04-12 14:34:34.809759 wikiteam3-4.2.6/wikiteam3/utils/ia_checker.py
+-rw-r--r--   0        0        0     3422 2024-04-12 14:34:34.809759 wikiteam3-4.2.6/wikiteam3/utils/identifier.py
+-rw-r--r--   0        0        0     1471 2024-04-12 14:34:34.809759 wikiteam3-4.2.6/wikiteam3/utils/login/__init__.py
+-rw-r--r--   0        0        0     2380 2024-04-12 14:34:34.809759 wikiteam3-4.2.6/wikiteam3/utils/login/api.py
+-rw-r--r--   0        0        0     2157 2024-04-12 14:34:34.809759 wikiteam3-4.2.6/wikiteam3/utils/login/index.py
+-rw-r--r--   0        0        0     7701 2024-04-16 08:42:20.859948 wikiteam3-4.2.6/wikiteam3/utils/monkey_patch.py
+-rw-r--r--   0        0        0      341 2024-04-12 14:34:34.809759 wikiteam3-4.2.6/wikiteam3/utils/uprint.py
+-rw-r--r--   0        0        0    38659 2024-04-12 14:34:34.809759 wikiteam3-4.2.6/wikiteam3/utils/user_agent.py
+-rw-r--r--   0        0        0     4497 2024-04-16 09:08:54.080329 wikiteam3-4.2.6/wikiteam3/utils/util.py
+-rw-r--r--   0        0        0      779 2024-04-16 08:42:20.859948 wikiteam3-4.2.6/wikiteam3/utils/wiki_avoid.py
+-rw-r--r--   0        0        0    17936 1970-01-01 00:00:00.000000 wikiteam3-4.2.6/PKG-INFO
```

### Comparing `wikiteam3-4.2.5/LICENSE` & `wikiteam3-4.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `wikiteam3-4.2.5/README.md` & `wikiteam3-4.2.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -37,21 +37,20 @@
 
 ```bash
 usage: wikiteam3dumpgenerator [-h] [-v] [--cookies cookies.txt] [--delay 1.5]
                               [--retries 5] [--path PATH] [--resume] [--force]
                               [--user USER] [--pass PASSWORD]
                               [--http-user HTTP_USER]
                               [--http-pass HTTP_PASSWORD] [--insecure]
-                              [--verbose] [--stdout-log-file STDOUT_LOG_PATH]
-                              [--api_chunksize 50] [--api API] [--index INDEX]
-                              [--index-check-threshold 0.80] [--xml]
-                              [--curonly] [--xmlapiexport] [--xmlrevisions]
-                              [--xmlrevisions_page] [--namespaces 1,2,3]
-                              [--exnamespaces 1,2,3] [--images]
-                              [--bypass-cdn-image-compression]
+                              [--verbose] [--api_chunksize 50] [--api API]
+                              [--index INDEX] [--index-check-threshold 0.80]
+                              [--xml] [--curonly] [--xmlapiexport]
+                              [--xmlrevisions] [--xmlrevisions_page]
+                              [--namespaces 1,2,3] [--exnamespaces 1,2,3]
+                              [--images] [--bypass-cdn-image-compression]
                               [--image-timestamp-interval 2019-01-02T01:36:06Z/2023-08-12T10:36:06Z]
                               [--ia-wbm-booster {0,1,2,3}]
                               [--assert-max-pages 123]
                               [--assert-max-edits 123]
                               [--assert-max-images 123]
                               [--assert-max-images-bytes 123]
                               [--get-wiki-engine] [--failfast] [--upload]
@@ -75,16 +74,14 @@
   --pass PASSWORD       Password if MediaWiki authentication is required.
   --http-user HTTP_USER
                         Username if HTTP authentication is required.
   --http-pass HTTP_PASSWORD
                         Password if HTTP authentication is required.
   --insecure            Disable SSL certificate verification
   --verbose
-  --stdout-log-file STDOUT_LOG_PATH
-                        Path to copy stdout to
   --api_chunksize 50    Chunk size for MediaWiki API (arvlimit, ailimit, etc.)
 
   wiki                  URL to wiki (e.g. http://wiki.domain.org), auto
                         detects API and index.php
   --api API             URL to API (e.g. http://wiki.domain.org/w/api.php)
   --index INDEX         URL to index.php (e.g.
                         http://wiki.domain.org/w/index.php), (not supported
@@ -116,15 +113,15 @@
 Image dump options:
   Options for image dump (--images)
 
   --bypass-cdn-image-compression
                         Bypass CDN image compression. (CloudFlare Polish,
                         etc.)
   --image-timestamp-interval 2019-01-02T01:36:06Z/2023-08-12T10:36:06Z
-                        [BETA] Only download images uploaded in the given time
+                        Only download images uploaded in the given time
                         interval. [format: ISO 8601 UTC interval] (only works
                         with api)
   --ia-wbm-booster {0,1,2,3}
                         Download images from Internet Archive Wayback Machine
                         if possible, reduce the bandwidth usage of the wiki.
                         [0: disabled (default), 1: use earliest snapshot, 2:
                         use latest snapshot, 3: the closest snapshot to the
```

### Comparing `wikiteam3-4.2.5/pyproject.toml` & `wikiteam3-4.2.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "wikiteam3"
-version = "4.2.5"
+version = "4.2.6"
 description = "Tools for downloading and preserving MediaWikis. We archive MediaWikis, from Wikipedia to tiniest wikis."
 license = "GPL-3.0-or-later"
 # authors = ["WikiTeam Contributors"] # FIXME: it's not an valid author name
 authors = ["yzqzss <yzqzss@yandex.com>"]
 maintainers = [
     # "saveweb wikiteam3 maintainers", #FIXME
     # "mediawiki-scarper maintainers",
```

### Comparing `wikiteam3-4.2.5/wikiteam3/dumpgenerator/api/api.py` & `wikiteam3-4.2.6/wikiteam3/dumpgenerator/api/api.py`

 * *Files identical despite different names*

### Comparing `wikiteam3-4.2.5/wikiteam3/dumpgenerator/api/handle_status_code.py` & `wikiteam3-4.2.6/wikiteam3/dumpgenerator/api/handle_status_code.py`

 * *Files identical despite different names*

### Comparing `wikiteam3-4.2.5/wikiteam3/dumpgenerator/api/index_check.py` & `wikiteam3-4.2.6/wikiteam3/dumpgenerator/api/index_check.py`

 * *Files identical despite different names*

### Comparing `wikiteam3-4.2.5/wikiteam3/dumpgenerator/api/namespaces.py` & `wikiteam3-4.2.6/wikiteam3/dumpgenerator/api/namespaces.py`

 * *Files identical despite different names*

### Comparing `wikiteam3-4.2.5/wikiteam3/dumpgenerator/api/page_titles.py` & `wikiteam3-4.2.6/wikiteam3/dumpgenerator/api/page_titles.py`

 * *Files identical despite different names*

### Comparing `wikiteam3-4.2.5/wikiteam3/dumpgenerator/api/wiki_check.py` & `wikiteam3-4.2.6/wikiteam3/dumpgenerator/api/wiki_check.py`

 * *Files identical despite different names*

### Comparing `wikiteam3-4.2.5/wikiteam3/dumpgenerator/cli/cli.py` & `wikiteam3-4.2.6/wikiteam3/dumpgenerator/cli/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,17 +79,14 @@
         # help="User-Agent to use for requests (default: wikiteam3/<version> ...)",
         help=argparse.SUPPRESS, # private option
     )
     parser.add_argument(
         "--verbose", action="store_true", help=""
     )
     parser.add_argument(
-        "--stdout-log-file", dest="stdout_log_path", default=None, help="Path to copy stdout to",
-    )
-    parser.add_argument(
         "--api_chunksize", metavar="50", default=50, help="Chunk size for MediaWiki API (arvlimit, ailimit, etc.)"
     )
 
     # URL params
     group_WikiOrAPIOrIndex = parser.add_argument_group()
     group_WikiOrAPIOrIndex.add_argument(
         "wiki", default="", nargs="?", help="URL to wiki (e.g. http://wiki.domain.org), auto detects API and index.php"
@@ -511,42 +508,40 @@
             if ns.lower() == "all":
                 print("You cannot exclude all namespaces.")
                 sys.exit(1)
             else:
                 exnamespaces = [int(i) for i in ns.split(",")]
 
 
-    config = new_config({
-        "curonly": args.curonly,
-        "date": datetime.datetime.utcnow().strftime("%Y%m%d"),
-        "api": api,
-        "failfast": args.failfast,
-        "http_method": "POST",
-        "api_chunksize": int(args.api_chunksize),
-        "index": index,
-        "images": args.images,
-        "logs": False,
-        "xml": args.xml,
-        "xmlapiexport": args.xmlapiexport,
-        "xmlrevisions": args.xmlrevisions or args.xmlrevisions_page,
-        "xmlrevisions_page": args.xmlrevisions_page,
-        "namespaces": namespaces,
-        "exnamespaces": exnamespaces,
-        "path": args.path and os.path.normpath(args.path) or "",
-        "cookies": args.cookies or "",
-        "delay": args.delay,
-        "retries": int(args.retries),
-    })
+    config = Config(
+        curonly = args.curonly,
+        date = datetime.datetime.utcnow().strftime("%Y%m%d"),
+        api = api,
+        failfast = args.failfast,
+        http_method = "POST",
+        api_chunksize = int(args.api_chunksize),
+        index = index,
+        images = args.images,
+        logs = False,
+        xml = args.xml,
+        xmlapiexport = args.xmlapiexport,
+        xmlrevisions = args.xmlrevisions or args.xmlrevisions_page,
+        xmlrevisions_page = args.xmlrevisions_page,
+        namespaces = namespaces,
+        exnamespaces = exnamespaces,
+        path = args.path and os.path.normpath(args.path) or "",
+        delay = args.delay,
+        retries = int(args.retries),
+    )
 
 
     other = OtherConfig(
         resume = args.resume,
         force = args.force,
         session = session,
-        stdout_log_path = args.stdout_log_path,
         bypass_cdn_image_compression = args.bypass_cdn_image_compression,
         add_referer_header = args.add_referer_header,
         image_timestamp_interval = args.image_timestamp_interval,
         ia_wbm_booster = args.ia_wbm_booster,
 
         assert_max_pages = args.assert_max_pages,
         assert_max_edits = args.assert_max_edits,
```

### Comparing `wikiteam3-4.2.5/wikiteam3/dumpgenerator/cli/delay.py` & `wikiteam3-4.2.6/wikiteam3/dumpgenerator/cli/delay.py`

 * *Files identical despite different names*

### Comparing `wikiteam3-4.2.5/wikiteam3/dumpgenerator/cli/greeter.py` & `wikiteam3-4.2.6/wikiteam3/dumpgenerator/cli/greeter.py`

 * *Files identical despite different names*

### Comparing `wikiteam3-4.2.5/wikiteam3/dumpgenerator/config.py` & `wikiteam3-4.2.6/wikiteam3/dumpgenerator/config.py`

 * *Files 17% similar despite different names*

```diff
@@ -11,68 +11,69 @@
     else:
         ret = klass_or_obj
     for k,v in d.items():
         if hasattr(ret, k):
             setattr(ret, k, v)
     return ret
 
-'''
-config = {
-        "curonly": args.curonly,
-        "date": datetime.datetime.utcnow().strftime("%Y%m%d"),
-        "api": api,
-        "failfast": args.failfast,
-        "http_method": "POST",
-        "index": index,
-        "images": args.images,
-        "logs": False,
-        "xml": args.xml,
-        "xmlrevisions": args.xmlrevisions,
-        "namespaces": namespaces,
-        "exnamespaces": exnamespaces,
-        "path": args.path and os.path.normpath(args.path) or "",
-        "cookies": args.cookies or "",
-        "delay": args.delay,
-        "retries": int(args.retries),
-    }
-'''
+
 @dataclasses.dataclass
 class Config:
     def asdict(self):
         return dataclasses.asdict(self)
 
     # General params
     delay: float = 0.0
+    """ Delay between requests """
     retries: int = 0
+    """ Number of retries """
     path: str = ''
+    """ Path to save the wikidump """
     logs: bool = False
+    """
+    Save MediaWiki logs #NOTE: this feature is not implemented yet
+    https://www.mediawiki.org/wiki/Manual:Logging_table
+    """
     date: str = False
+    """
+    Date of the dump
+    `datetime.datetime.utcnow().strftime("%Y%m%d")`
+    """
 
     # URL params
     index: str = ''
     api: str = ''
 
     # Download params
     xml: bool = False
     curonly: bool = False
     xmlapiexport: bool = False
     xmlrevisions: bool = False
     xmlrevisions_page: bool = False
     images: bool = False
     namespaces: List[int] = None
     exnamespaces: List[int] = None
+    """ save images """
 
     api_chunksize: int = 0  # arvlimit, ailimit, etc
-    export: str = '' # Special:Export page name
+    export: str = ''
+    """ `Special:Export` page name """
     http_method: str = ''
+    """ GET/POST """
 
     # Meta info params
     failfast: bool = False
 
-    templates: bool = False
+    templates: bool = False # TODO: rename to `xml_export_include_templates`
+    """
+    Whether to include `&templates=1` parameter in the `Special:Export` (--xml) export action.
+    https://www.mediawiki.org/wiki/Manual:Parameters_to_Special:Export#Available_parameters
+
+    NOTE: this config is not used to control the export of templates namespace (--namespaces).
+    """
 
 def new_config(configDict) -> Config:
     return _dataclass_from_dict(Config, configDict)
 
 def load_config(config: Config, config_filename: str):
     """Load config file"""
 
@@ -96,15 +97,14 @@
 
 
 @dataclasses.dataclass
 class OtherConfig:
     resume: bool
     force: bool 
     session: requests.Session 
-    stdout_log_path: Optional[str] 
     bypass_cdn_image_compression: bool 
     add_referer_header: Optional[str] 
     '''None, "auto", {URL}'''
     image_timestamp_interval: Optional[str]
     ''' 2019-01-02T01:36:06Z/2023-08-12T10:36:06Z '''
     ia_wbm_booster: int
```

### Comparing `wikiteam3-4.2.5/wikiteam3/dumpgenerator/dump/generator.py` & `wikiteam3-4.2.6/wikiteam3/dumpgenerator/dump/generator.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,48 +19,26 @@
 from wikiteam3.dumpgenerator.dump.xmldump.xml_dump import generate_XML_dump
 from wikiteam3.dumpgenerator.dump.xmldump.xml_integrity import check_XML_integrity
 from wikiteam3.dumpgenerator.log import log_error
 from wikiteam3.utils import url2prefix_from_config, undo_HTML_entities, avoid_WikiMedia_projects
 from wikiteam3.utils.ia_checker import any_recent_ia_item_exists
 from wikiteam3.utils.util import ALL_DUMPED_MARK, int_or_zero, mark_as_done, underscore
 
-# From https://stackoverflow.com/a/57008707
-class Tee(object):
-    def __init__(self, filename):
-        self.file = open(filename, 'w', encoding="utf-8")
-        self.stdout = sys.stdout
-
-    def __enter__(self):
-        sys.stdout = self
-
-    def __exit__(self, exc_type, exc_value, tb):
-        sys.stdout = self.stdout
-        if exc_type is not None:
-            self.file.write(traceback.format_exc())
-        self.file.close()
-
-    def write(self, data):
-        self.file.write(data)
-        self.stdout.write(data)
-
-    def flush(self):
-        self.file.flush()
-        self.stdout.flush()
 
 class DumpGenerator:
     configfilename = "config.json"
 
     @staticmethod
     def __init__(params=None):
         """Main function"""
         config_filename = DumpGenerator.configfilename
         config, other = get_parameters(params=params)
         avoid_WikiMedia_projects(config=config, other=other)
 
-        with (Tee(other.stdout_log_path) if other.stdout_log_path else contextlib.nullcontext()):
+        with contextlib.nullcontext():
             print(welcome())
             print("Analysing %s" % (config.api if config.api else config.index))
 
             # do not enter if resume is requested from begining
             while not other.resume and os.path.isdir(config.path):
                 print('\nWarning!: "%s" path exists' % (config.path))
                 reply = "y" if config.failfast else ""
```

### Comparing `wikiteam3-4.2.5/wikiteam3/dumpgenerator/dump/image/html_regexs.py` & `wikiteam3-4.2.6/wikiteam3/dumpgenerator/dump/image/html_regexs.py`

 * *Files identical despite different names*

### Comparing `wikiteam3-4.2.5/wikiteam3/dumpgenerator/dump/image/html_regexs_test.py` & `wikiteam3-4.2.6/wikiteam3/dumpgenerator/dump/image/html_regexs_test.py`

 * *Files identical despite different names*

### Comparing `wikiteam3-4.2.5/wikiteam3/dumpgenerator/dump/image/image.py` & `wikiteam3-4.2.6/wikiteam3/dumpgenerator/dump/image/image.py`

 * *Files identical despite different names*

### Comparing `wikiteam3-4.2.5/wikiteam3/dumpgenerator/dump/misc/index_php.py` & `wikiteam3-4.2.6/wikiteam3/dumpgenerator/dump/misc/index_php.py`

 * *Files identical despite different names*

### Comparing `wikiteam3-4.2.5/wikiteam3/dumpgenerator/dump/misc/site_info.py` & `wikiteam3-4.2.6/wikiteam3/dumpgenerator/dump/misc/site_info.py`

 * *Files identical despite different names*

### Comparing `wikiteam3-4.2.5/wikiteam3/dumpgenerator/dump/misc/special_logs.py` & `wikiteam3-4.2.6/wikiteam3/dumpgenerator/dump/misc/special_logs.py`

 * *Files identical despite different names*

### Comparing `wikiteam3-4.2.5/wikiteam3/dumpgenerator/dump/misc/special_version.py` & `wikiteam3-4.2.6/wikiteam3/dumpgenerator/dump/misc/special_version.py`

 * *Files identical despite different names*

### Comparing `wikiteam3-4.2.5/wikiteam3/dumpgenerator/dump/page/xmlexport/page_xml_api.py` & `wikiteam3-4.2.6/wikiteam3/dumpgenerator/dump/page/xmlexport/page_xml_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 import requests
 
 from wikiteam3.dumpgenerator.api import handle_StatusCode
 from wikiteam3.dumpgenerator.config import Config
 from wikiteam3.dumpgenerator.exceptions import PageMissingError, ExportAbortedError
 from wikiteam3.dumpgenerator.log import log_error
+from wikiteam3.utils.util import underscore
 
 
 def reconstructRevisions(root: ET.Element):
     #print ET.tostring(rev)
     page = ET.Element('stub')
     edits = 0
 
@@ -147,16 +148,15 @@
 
 
 def getXMLPageWithApi(config: Config, title="", verbose=True, *, session: requests.Session):
     """ Get the full history (or current only) of a page using API:Query
         if params['curonly'] is set, then using export&exportwrap to export
     """
 
-    title_ = title
-    title_ = re.sub(' ', '_', title_)
+    title_ = underscore(title)
     # do not convert & into %26, title_ = re.sub('&', '%26', title_)
     # action=query&rvlimit=50&format=xml&prop=revisions&titles=TITLE_HERE
     # &rvprop=timestamp%7Cuser%7Ccomment%7Ccontent%7Cids%7Cuserid%7Csha1%7Csize
     # print 'current:%s' % (title_)
     if not config.curonly:
         params = {'titles': title_, 'action': 'query', 'format': 'xml',
                   'prop': 'revisions',
```

### Comparing `wikiteam3-4.2.5/wikiteam3/dumpgenerator/dump/page/xmlexport/page_xml_export.py` & `wikiteam3-4.2.6/wikiteam3/dumpgenerator/dump/page/xmlexport/page_xml_export.py`

 * *Files identical despite different names*

### Comparing `wikiteam3-4.2.5/wikiteam3/dumpgenerator/dump/page/xmlrev/xml_revisions.py` & `wikiteam3-4.2.6/wikiteam3/dumpgenerator/dump/page/xmlrev/xml_revisions.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,16 @@
 from urllib.parse import urlparse
 import lxml.etree
 
 import mwclient
 import mwclient.errors
 import requests
 
-from wikiteam3.dumpgenerator.exceptions import PageMissingError
+from wikiteam3.dumpgenerator.cli.delay import Delay
+from wikiteam3.dumpgenerator.exceptions import MWUnknownContentModelException, PageMissingError
 from wikiteam3.dumpgenerator.log import log_error
 from wikiteam3.dumpgenerator.api.namespaces import getNamespacesAPI
 from wikiteam3.dumpgenerator.api.page_titles import read_titles
 from wikiteam3.dumpgenerator.dump.page.xmlrev.xml_revisions_page import \
     make_xml_from_page, make_xml_page_from_raw
 from wikiteam3.dumpgenerator.config import Config
 
@@ -56,33 +57,62 @@
         if _arvcontinue_input is not None:
             arv_params['arvcontinue'] = _arvcontinue_input
 
         if not config.curonly:
             # We have to build the XML manually...
             # Skip flags, presumably needed to add <minor/> which is in the schema.
             # Also missing: parentid and contentformat.
+            ARV_PROP = "ids|timestamp|user|userid|size|sha1|contentmodel|comment|content|flags"
             arv_params[
                 "arvprop"
-            ] = "ids|timestamp|user|userid|size|sha1|contentmodel|comment|content|flags"
+            ] = ARV_PROP
             print(
                 "Trying to get wikitext from the allrevisions API and to build the XML"
             )
             while True:
                 print("[arvcontinue]:", arv_params.get("arvcontinue", ""))
                 try:
                     allrevs_response = site.api(
                         http_method=config.http_method, **arv_params
                     )
+                    # reset params if the response is OK
+                    arv_params["arvprop"] = ARV_PROP
+                    if arv_params["arvlimit"] != config.api_chunksize:
+                        arv_params["arvlimit"] = min(arv_params["arvlimit"] * 2, config.api_chunksize)
+                        print(f"INFO: response is OK, increasing arvlimit to {arv_params['arvlimit']}")
+                except mwclient.errors.APIError as e:
+                    if e.code == MWUnknownContentModelException.error_code:
+                        if arv_params['arvlimit'] != 1:
+                            # let's retry with arvlimit=1 to retrieve good revisions as much as possible
+                            print("WARNING: API returned MWUnknownContentModelException. retrying with arvlimit=1 (revision by revision)")
+                            arv_params["arvlimit"] = 1
+                            Delay(config=config)
+                            continue
+                        elif '|content' in arv_params["arvprop"]:
+                            log_error(config=config, to_stdout=True,
+                                text=f"ERROR: API returned MWUnknownContentModelException on arvcontinue={arv_params.get('arvcontinue', '')}, " +
+                                "retried with arvlimit=1 and still failed. retrying without arvprop=content. " +
+                                '(wikiteam3 would mark the revision as "<text deleted="deletetd"> in the xmldump)'
+                            )
+                            arv_params["arvprop"] = ARV_PROP.replace('|content', '')
+                            Delay(config=config)
+                            continue
+                        else:
+                            assert False, "This should not happen"
+                    else:
+                        raise
+
                 except requests.exceptions.HTTPError as e:
                     if (
                             e.response.status_code == 405
                             and config.http_method == "POST"
                     ):
                         print("POST request to the API failed, retrying with GET")
                         config.http_method = "GET"
+                        Delay(config=config)
                         continue
                     else:
                         raise
                 except requests.exceptions.ReadTimeout as err:
                     # Hopefully temporary, just wait a bit and continue with the same request.
                     # No point putting a limit to retries, we'd need to abort everything.
                     # TODO: reuse the retry logic of the checkAPI phase? Or force mwclient
@@ -94,14 +124,15 @@
                 except mwclient.errors.InvalidResponse as e:
                     if (
                         e.response_text.startswith("<!DOCTYPE html>") # type: ignore
                         and config.http_method == "POST"
                     ):
                         print("POST request to the API failed (got HTML), retrying with GET")
                         config.http_method = "GET"
+                        Delay(config=config)
                         continue
                     else:
                         raise
 
                 for page in allrevs_response["query"]["allrevisions"]:
                     yield make_xml_from_page(page, arv_params.get("arvcontinue", ""))
 
@@ -373,16 +404,14 @@
             if c % 10 == 0:
                 print(f"\n->  Downloaded {c} pages\n")
 
 
 def getXMLRevisions(config: Config, session: requests.Session, lastPage=None, useAllrevision=True):
     # FIXME: actually figure out the various strategies for each MediaWiki version
     apiurl = urlparse(config.api)
-    # FIXME: force the protocol we asked for! Or don't verify SSL if we asked HTTP?
-    # https://github.com/WikiTeam/wikiteam/issues/358
     site = mwclient.Site(
         apiurl.netloc, apiurl.path.replace("api.php", ""), scheme=apiurl.scheme, pool=session
     )
 
     if useAllrevision:
         # Find last title
         if lastPage is not None:
```

### Comparing `wikiteam3-4.2.5/wikiteam3/dumpgenerator/dump/page/xmlrev/xml_revisions_page.py` & `wikiteam3-4.2.6/wikiteam3/dumpgenerator/dump/page/xmlrev/xml_revisions_page.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,15 +52,15 @@
                 size = 0
 
             # Create rev object
             revision = [E.id(str(rev["revid"])),
                 E.timestamp(rev["timestamp"]),]
 
             # The text, user, comment, sha1 may be deleted/suppressed
-            if (('texthidden' in rev) or ('textmissing' in rev)):
+            if (('texthidden' in rev) or ('textmissing' in rev)) or ('*' not in rev):
                 print("Warning: text missing/hidden in pageid %d revid %d" % (page['pageid'], rev['revid']))
                 revision.append(E.text(**{
                     'bytes': str(size),
                     'deleted': 'deleted',
                 }))
             else:
                 text = str(rev["*"])
@@ -113,10 +113,11 @@
             for tag in revisionTags:
                 if tag in revisionElementsDict:
                     _revision.append(revisionElementsDict.pop(tag))
             for elem in revisionElementsDict.values():
                 _revision.append(elem)
             p.append(_revision)
     except KeyError as e:
-        print(e)
+        import traceback
+        traceback.print_exc()
         raise PageMissingError(page["title"], e)
     return etree.tostring(p, pretty_print=True, encoding="unicode")
```

### Comparing `wikiteam3-4.2.5/wikiteam3/dumpgenerator/dump/xmldump/xml_dump.py` & `wikiteam3-4.2.6/wikiteam3/dumpgenerator/dump/xmldump/xml_dump.py`

 * *Files identical despite different names*

### Comparing `wikiteam3-4.2.5/wikiteam3/dumpgenerator/dump/xmldump/xml_header.py` & `wikiteam3-4.2.6/wikiteam3/dumpgenerator/dump/xmldump/xml_header.py`

 * *Files identical despite different names*

### Comparing `wikiteam3-4.2.5/wikiteam3/dumpgenerator/dump/xmldump/xml_truncate.py` & `wikiteam3-4.2.6/wikiteam3/dumpgenerator/dump/xmldump/xml_truncate.py`

 * *Files identical despite different names*

### Comparing `wikiteam3-4.2.5/wikiteam3/uploader/compresser.py` & `wikiteam3-4.2.6/wikiteam3/uploader/compresser.py`

 * *Files identical despite different names*

### Comparing `wikiteam3-4.2.5/wikiteam3/uploader/socketLock.py` & `wikiteam3-4.2.6/wikiteam3/uploader/socketLock.py`

 * *Files identical despite different names*

### Comparing `wikiteam3-4.2.5/wikiteam3/uploader/uploader.py` & `wikiteam3-4.2.6/wikiteam3/uploader/uploader.py`

 * *Files identical despite different names*

### Comparing `wikiteam3-4.2.5/wikiteam3/utils/ia_checker.py` & `wikiteam3-4.2.6/wikiteam3/utils/ia_checker.py`

 * *Files identical despite different names*

### Comparing `wikiteam3-4.2.5/wikiteam3/utils/identifier.py` & `wikiteam3-4.2.6/wikiteam3/utils/identifier.py`

 * *Files identical despite different names*

### Comparing `wikiteam3-4.2.5/wikiteam3/utils/login/__init__.py` & `wikiteam3-4.2.6/wikiteam3/utils/login/__init__.py`

 * *Files identical despite different names*

### Comparing `wikiteam3-4.2.5/wikiteam3/utils/login/api.py` & `wikiteam3-4.2.6/wikiteam3/utils/login/api.py`

 * *Files identical despite different names*

### Comparing `wikiteam3-4.2.5/wikiteam3/utils/login/index.py` & `wikiteam3-4.2.6/wikiteam3/utils/login/index.py`

 * *Files identical despite different names*

### Comparing `wikiteam3-4.2.5/wikiteam3/utils/monkey_patch.py` & `wikiteam3-4.2.6/wikiteam3/utils/monkey_patch.py`

 * *Files identical despite different names*

### Comparing `wikiteam3-4.2.5/wikiteam3/utils/user_agent.py` & `wikiteam3-4.2.6/wikiteam3/utils/user_agent.py`

 * *Files identical despite different names*

### Comparing `wikiteam3-4.2.5/wikiteam3/utils/util.py` & `wikiteam3-4.2.6/wikiteam3/utils/util.py`

 * *Files 8% similar despite different names*

```diff
@@ -78,18 +78,14 @@
 
     return raw
 
 
 def clean_XML(xml: str = "") -> str:
     """Trim redundant info from the XML however it comes"""
     # do not touch XML codification, leave AS IS
-    # EDIT 2022: we are making this explicitly Unicode
-    # for Windows compatibility.
-    # If the encoding has to stay as is, we'll have
-    # to change all the file encodings, as well.
 
     if re.search(r"</siteinfo>\n", xml):
         xml = xml.split("</siteinfo>\n")[1]
     if re.search(r"</mediawiki>", xml):
         xml = xml.split("</mediawiki>")[0]
     return xml
```

### Comparing `wikiteam3-4.2.5/wikiteam3/utils/wiki_avoid.py` & `wikiteam3-4.2.6/wikiteam3/utils/wiki_avoid.py`

 * *Files identical despite different names*

### Comparing `wikiteam3-4.2.5/PKG-INFO` & `wikiteam3-4.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wikiteam3
-Version: 4.2.5
+Version: 4.2.6
 Summary: Tools for downloading and preserving MediaWikis. We archive MediaWikis, from Wikipedia to tiniest wikis.
 Home-page: https://github.com/saveweb/wikiteam3
 License: GPL-3.0-or-later
 Keywords: archiveteam,mediawiki,preservation,wiki,wikipedia
 Author: yzqzss
 Author-email: yzqzss@yandex.com
 Maintainer: yzqzss
@@ -82,21 +82,20 @@
 
 ```bash
 usage: wikiteam3dumpgenerator [-h] [-v] [--cookies cookies.txt] [--delay 1.5]
                               [--retries 5] [--path PATH] [--resume] [--force]
                               [--user USER] [--pass PASSWORD]
                               [--http-user HTTP_USER]
                               [--http-pass HTTP_PASSWORD] [--insecure]
-                              [--verbose] [--stdout-log-file STDOUT_LOG_PATH]
-                              [--api_chunksize 50] [--api API] [--index INDEX]
-                              [--index-check-threshold 0.80] [--xml]
-                              [--curonly] [--xmlapiexport] [--xmlrevisions]
-                              [--xmlrevisions_page] [--namespaces 1,2,3]
-                              [--exnamespaces 1,2,3] [--images]
-                              [--bypass-cdn-image-compression]
+                              [--verbose] [--api_chunksize 50] [--api API]
+                              [--index INDEX] [--index-check-threshold 0.80]
+                              [--xml] [--curonly] [--xmlapiexport]
+                              [--xmlrevisions] [--xmlrevisions_page]
+                              [--namespaces 1,2,3] [--exnamespaces 1,2,3]
+                              [--images] [--bypass-cdn-image-compression]
                               [--image-timestamp-interval 2019-01-02T01:36:06Z/2023-08-12T10:36:06Z]
                               [--ia-wbm-booster {0,1,2,3}]
                               [--assert-max-pages 123]
                               [--assert-max-edits 123]
                               [--assert-max-images 123]
                               [--assert-max-images-bytes 123]
                               [--get-wiki-engine] [--failfast] [--upload]
@@ -120,16 +119,14 @@
   --pass PASSWORD       Password if MediaWiki authentication is required.
   --http-user HTTP_USER
                         Username if HTTP authentication is required.
   --http-pass HTTP_PASSWORD
                         Password if HTTP authentication is required.
   --insecure            Disable SSL certificate verification
   --verbose
-  --stdout-log-file STDOUT_LOG_PATH
-                        Path to copy stdout to
   --api_chunksize 50    Chunk size for MediaWiki API (arvlimit, ailimit, etc.)
 
   wiki                  URL to wiki (e.g. http://wiki.domain.org), auto
                         detects API and index.php
   --api API             URL to API (e.g. http://wiki.domain.org/w/api.php)
   --index INDEX         URL to index.php (e.g.
                         http://wiki.domain.org/w/index.php), (not supported
@@ -161,15 +158,15 @@
 Image dump options:
   Options for image dump (--images)
 
   --bypass-cdn-image-compression
                         Bypass CDN image compression. (CloudFlare Polish,
                         etc.)
   --image-timestamp-interval 2019-01-02T01:36:06Z/2023-08-12T10:36:06Z
-                        [BETA] Only download images uploaded in the given time
+                        Only download images uploaded in the given time
                         interval. [format: ISO 8601 UTC interval] (only works
                         with api)
   --ia-wbm-booster {0,1,2,3}
                         Download images from Internet Archive Wayback Machine
                         if possible, reduce the bandwidth usage of the wiki.
                         [0: disabled (default), 1: use earliest snapshot, 2:
                         use latest snapshot, 3: the closest snapshot to the
```

