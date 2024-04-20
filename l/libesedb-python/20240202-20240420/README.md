# Comparing `tmp/libesedb-python-20240202.tar.gz` & `tmp/libesedb-python-20240420.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libesedb-python-20240202.tar", last modified: Fri Feb  2 04:07:52 2024, max compression
+gzip compressed data, was "libesedb-python-20240420.tar", last modified: Sat Apr 20 14:34:05 2024, max compression
```

## Comparing `libesedb-python-20240202.tar` & `libesedb-python-20240420.tar`

### file list

```diff
@@ -1,1112 +1,1112 @@
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-02 04:07:51.000000 libesedb-20240202/
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-02 04:07:50.000000 libesedb-20240202/libfdata/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-02-02 03:41:45.000000 libesedb-20240202/libfdata/libfdata_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37893 2024-02-02 03:41:45.000000 libesedb-20240202/libfdata/libfdata_area.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9700 2024-02-02 03:41:45.000000 libesedb-20240202/libfdata/libfdata_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1491 2024-02-02 03:41:45.000000 libesedb-20240202/libfdata/libfdata_cache.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30931 2024-02-02 03:41:45.000000 libesedb-20240202/libfdata/libfdata_range_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6826 2024-02-02 03:41:45.000000 libesedb-20240202/libfdata/libfdata_mapped_range.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-02-02 03:41:45.000000 libesedb-20240202/libfdata/libfdata_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6533 2024-02-02 03:41:45.000000 libesedb-20240202/libfdata/libfdata_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   107689 2024-02-02 03:41:45.000000 libesedb-20240202/libfdata/libfdata_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1548 2024-02-02 03:41:45.000000 libesedb-20240202/libfdata/libfdata_libcdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12090 2024-02-02 03:41:45.000000 libesedb-20240202/libfdata/libfdata_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4017 2024-02-02 03:41:45.000000 libesedb-20240202/libfdata/libfdata_list_element.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1291 2024-02-02 03:41:45.000000 libesedb-20240202/libfdata/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-02-02 03:41:45.000000 libesedb-20240202/libfdata/libfdata_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-02-02 03:41:45.000000 libesedb-20240202/libfdata/libfdata_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2754 2024-02-02 03:41:45.000000 libesedb-20240202/libfdata/libfdata_notify.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1658 2024-02-02 03:41:45.000000 libesedb-20240202/libfdata/libfdata_cache.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    66203 2024-02-02 03:41:45.000000 libesedb-20240202/libfdata/libfdata_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-02-02 03:41:45.000000 libesedb-20240202/libfdata/libfdata_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2092 2024-02-02 03:41:45.000000 libesedb-20240202/libfdata/libfdata_range.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7327 2024-02-02 03:41:45.000000 libesedb-20240202/libfdata/libfdata_area.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-02-02 03:41:45.000000 libesedb-20240202/libfdata/libfdata_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1230 2024-02-02 03:41:45.000000 libesedb-20240202/libfdata/libfdata_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7149 2024-02-02 03:41:45.000000 libesedb-20240202/libfdata/libfdata_range.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1995 2024-02-02 03:41:45.000000 libesedb-20240202/libfdata/libfdata_mapped_range.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1172 2024-02-02 03:41:45.000000 libesedb-20240202/libfdata/libfdata_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19329 2024-02-02 03:41:45.000000 libesedb-20240202/libfdata/libfdata_list_element.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21271 2024-02-02 03:41:45.000000 libesedb-20240202/libfdata/libfdata_segments_array.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2054 2024-02-02 03:41:45.000000 libesedb-20240202/libfdata/libfdata_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1593 2024-02-02 03:41:45.000000 libesedb-20240202/libfdata/libfdata_notify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6013 2024-02-02 03:41:45.000000 libesedb-20240202/libfdata/libfdata_range_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2804 2024-02-02 03:41:45.000000 libesedb-20240202/libfdata/libfdata_segments_array.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34168 2024-02-02 03:42:05.000000 libesedb-20240202/libfdata/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    49670 2024-02-02 03:41:45.000000 libesedb-20240202/libfdata/libfdata_vector.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-02-02 03:41:45.000000 libesedb-20240202/libfdata/libfdata_libfcache.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7810 2024-02-02 03:41:45.000000 libesedb-20240202/libfdata/libfdata_vector.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35149 2024-02-02 03:31:33.000000 libesedb-20240202/COPYING
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    15358 2024-02-02 03:42:05.000000 libesedb-20240202/install-sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-02 03:31:33.000000 libesedb-20240202/NEWS
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    23568 2024-02-02 03:42:06.000000 libesedb-20240202/depcomp
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-02 04:07:50.000000 libesedb-20240202/libfguid/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-02-02 03:41:48.000000 libesedb-20240202/libfguid/libfguid_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1192 2024-02-02 03:41:48.000000 libesedb-20240202/libfguid/libfguid_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5688 2024-02-02 03:41:48.000000 libesedb-20240202/libfguid/libfguid_identifier.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-02-02 03:41:48.000000 libesedb-20240202/libfguid/libfguid_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      681 2024-02-02 03:41:48.000000 libesedb-20240202/libfguid/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-02-02 03:41:48.000000 libesedb-20240202/libfguid/libfguid_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-02-02 03:41:48.000000 libesedb-20240202/libfguid/libfguid_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1515 2024-02-02 03:41:48.000000 libesedb-20240202/libfguid/libfguid_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    67571 2024-02-02 03:41:48.000000 libesedb-20240202/libfguid/libfguid_identifier.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1134 2024-02-02 03:41:48.000000 libesedb-20240202/libfguid/libfguid_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2341 2024-02-02 03:41:48.000000 libesedb-20240202/libfguid/libfguid_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30383 2024-02-02 03:42:06.000000 libesedb-20240202/libfguid/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-02-02 03:41:48.000000 libesedb-20240202/libfguid/libfguid_error.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-02 04:07:49.000000 libesedb-20240202/m4/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8809 2023-12-03 09:01:06.000000 libesedb-20240202/m4/libfwnt.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11498 2023-12-03 09:01:06.000000 libesedb-20240202/m4/libcfile.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18233 2023-12-03 09:01:06.000000 libesedb-20240202/m4/libfdatetime.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      756 2023-12-03 09:01:06.000000 libesedb-20240202/m4/tests.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9379 2023-12-03 09:01:06.000000 libesedb-20240202/m4/libcpath.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11944 2023-12-03 09:01:06.000000 libesedb-20240202/m4/lib-prefix.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3090 2023-12-03 09:01:06.000000 libesedb-20240202/m4/progtest.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31269 2023-12-03 09:01:06.000000 libesedb-20240202/m4/libuna.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14488 2023-12-03 09:01:06.000000 libesedb-20240202/m4/gettext.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5370 2023-12-03 09:01:06.000000 libesedb-20240202/m4/lib-ld.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8230 2023-12-03 09:01:06.000000 libesedb-20240202/m4/libclocale.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17147 2023-12-03 09:01:06.000000 libesedb-20240202/m4/libcdata.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7384 2023-12-03 09:01:06.000000 libesedb-20240202/m4/libcsplit.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14115 2023-12-03 09:01:06.000000 libesedb-20240202/m4/common.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11112 2023-12-03 09:01:06.000000 libesedb-20240202/m4/libcthreads.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4070 2023-12-03 09:01:06.000000 libesedb-20240202/m4/libmapidb.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      714 2024-02-02 03:42:00.000000 libesedb-20240202/m4/ltversion.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4395 2024-02-02 03:42:00.000000 libesedb-20240202/m4/ltsugar.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15545 2023-12-03 09:01:06.000000 libesedb-20240202/m4/libfdata.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22432 2023-12-03 09:01:06.000000 libesedb-20240202/m4/host-cpu-c-abi.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   307188 2024-02-02 03:42:00.000000 libesedb-20240202/m4/libtool.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18831 2023-12-03 09:01:06.000000 libesedb-20240202/m4/po.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6260 2023-12-03 09:01:06.000000 libesedb-20240202/m4/libcerror.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5638 2023-12-03 09:01:06.000000 libesedb-20240202/m4/libcnotify.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5640 2023-12-03 09:01:06.000000 libesedb-20240202/m4/libfguid.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11692 2023-12-03 09:01:06.000000 libesedb-20240202/m4/libbfio.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8941 2023-12-03 09:01:06.000000 libesedb-20240202/m4/libfmapi.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3229 2023-12-03 09:01:06.000000 libesedb-20240202/m4/intlmacosx.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6151 2024-02-02 03:42:00.000000 libesedb-20240202/m4/lt~obsolete.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34802 2023-12-03 09:01:06.000000 libesedb-20240202/m4/lib-link.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9731 2023-12-03 09:01:06.000000 libesedb-20240202/m4/iconv.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14525 2024-02-02 03:42:00.000000 libesedb-20240202/m4/ltoptions.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1234 2023-12-03 09:01:06.000000 libesedb-20240202/m4/nls.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6323 2023-12-03 09:01:06.000000 libesedb-20240202/m4/python.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19791 2023-12-03 09:01:06.000000 libesedb-20240202/m4/libfvalue.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2058 2023-12-03 09:01:06.000000 libesedb-20240202/m4/types.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7325 2023-12-03 09:01:06.000000 libesedb-20240202/m4/libfcache.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3852 2023-12-03 09:01:06.000000 libesedb-20240202/m4/pthread.m4
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-02 04:07:49.000000 libesedb-20240202/include/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      474 2024-02-02 03:31:33.000000 libesedb-20240202/include/Makefile.am
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-02 04:07:49.000000 libesedb-20240202/include/libesedb/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2981 2024-02-02 03:31:35.000000 libesedb-20240202/include/libesedb/definitions.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2979 2024-02-02 03:42:15.000000 libesedb-20240202/include/libesedb/definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5165 2024-02-02 03:31:35.000000 libesedb-20240202/include/libesedb/types.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5034 2024-02-02 03:42:15.000000 libesedb-20240202/include/libesedb/types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1551 2024-02-02 03:31:35.000000 libesedb-20240202/include/libesedb/features.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6758 2024-02-02 03:31:35.000000 libesedb-20240202/include/libesedb/error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2024-02-02 03:31:35.000000 libesedb-20240202/include/libesedb/extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1487 2024-02-02 03:42:15.000000 libesedb-20240202/include/libesedb/features.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5306 2024-02-02 03:31:35.000000 libesedb-20240202/include/libesedb/codepage.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39086 2024-02-02 03:42:15.000000 libesedb-20240202/include/libesedb.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28929 2024-02-02 03:42:05.000000 libesedb-20240202/include/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39086 2024-02-02 03:31:35.000000 libesedb-20240202/include/libesedb.h.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-02 04:07:49.000000 libesedb-20240202/common/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      957 2024-02-02 03:31:35.000000 libesedb-20240202/common/config_borlandc.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3878 2024-02-02 03:31:35.000000 libesedb-20240202/common/file_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3259 2024-02-02 03:31:35.000000 libesedb-20240202/common/memory.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10437 2024-02-02 03:31:35.000000 libesedb-20240202/common/byte_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1250 2024-02-02 03:31:35.000000 libesedb-20240202/common/common.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2382 2024-02-02 03:31:35.000000 libesedb-20240202/common/config_winapi.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4611 2024-02-02 03:31:35.000000 libesedb-20240202/common/system_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      366 2024-02-02 03:31:33.000000 libesedb-20240202/common/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7375 2024-02-02 03:31:35.000000 libesedb-20240202/common/types.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7374 2024-02-02 03:42:15.000000 libesedb-20240202/common/types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16997 2024-02-02 03:42:05.000000 libesedb-20240202/common/config.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18006 2024-02-02 03:42:15.000000 libesedb-20240202/common/config.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5064 2024-02-02 03:31:35.000000 libesedb-20240202/common/wide_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5419 2024-02-02 03:31:35.000000 libesedb-20240202/common/narrow_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1157 2024-02-02 03:31:35.000000 libesedb-20240202/common/config_msc.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25936 2024-02-02 03:42:05.000000 libesedb-20240202/common/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-02 04:07:50.000000 libesedb-20240202/libclocale/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1969 2024-02-02 03:41:39.000000 libesedb-20240202/libclocale/libclocale_wide_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1412 2024-02-02 03:41:39.000000 libesedb-20240202/libclocale/libclocale_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      779 2024-02-02 03:41:39.000000 libesedb-20240202/libclocale/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3412 2024-02-02 03:41:39.000000 libesedb-20240202/libclocale/libclocale_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2024-02-02 03:41:39.000000 libesedb-20240202/libclocale/libclocale_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1365 2024-02-02 03:41:39.000000 libesedb-20240202/libclocale/libclocale_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1717 2024-02-02 03:41:39.000000 libesedb-20240202/libclocale/libclocale_locale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3142 2024-02-02 03:41:39.000000 libesedb-20240202/libclocale/libclocale_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21033 2024-02-02 03:41:39.000000 libesedb-20240202/libclocale/libclocale_codepage.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10671 2024-02-02 03:41:39.000000 libesedb-20240202/libclocale/libclocale_locale.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30939 2024-02-02 03:42:05.000000 libesedb-20240202/libclocale/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1415 2024-02-02 03:41:39.000000 libesedb-20240202/libclocale/libclocale_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1696 2024-02-02 03:41:39.000000 libesedb-20240202/libclocale/libclocale_wide_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1961 2024-02-02 03:41:39.000000 libesedb-20240202/libclocale/libclocale_codepage.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-02 04:07:50.000000 libesedb-20240202/libfcache/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1551 2024-02-02 03:41:44.000000 libesedb-20240202/libfcache/libfcache_libcdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1619 2024-02-02 03:41:44.000000 libesedb-20240202/libfcache/libfcache_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12461 2024-02-02 03:41:44.000000 libesedb-20240202/libfcache/libfcache_cache_value.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-02-02 03:41:44.000000 libesedb-20240202/libfcache/libfcache_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      880 2024-02-02 03:41:44.000000 libesedb-20240202/libfcache/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2024-02-02 03:41:44.000000 libesedb-20240202/libfcache/libfcache_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-02-02 03:41:44.000000 libesedb-20240202/libfcache/libfcache_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1178 2024-02-02 03:41:44.000000 libesedb-20240202/libfcache/libfcache_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3806 2024-02-02 03:41:44.000000 libesedb-20240202/libfcache/libfcache_cache.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2924 2024-02-02 03:41:44.000000 libesedb-20240202/libfcache/libfcache_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-02-02 03:41:44.000000 libesedb-20240202/libfcache/libfcache_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2259 2024-02-02 03:41:44.000000 libesedb-20240202/libfcache/libfcache_date_time.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-02-02 03:41:44.000000 libesedb-20240202/libfcache/libfcache_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3161 2024-02-02 03:41:44.000000 libesedb-20240202/libfcache/libfcache_cache_value.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31412 2024-02-02 03:42:05.000000 libesedb-20240202/libfcache/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1250 2024-02-02 03:41:44.000000 libesedb-20240202/libfcache/libfcache_date_time.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1680 2024-02-02 03:41:44.000000 libesedb-20240202/libfcache/libfcache_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26186 2024-02-02 03:41:44.000000 libesedb-20240202/libfcache/libfcache_cache.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2446 2023-12-03 09:00:45.000000 libesedb-20240202/Makefile.am
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-02 04:07:50.000000 libesedb-20240202/libbfio/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2630 2024-02-02 03:41:33.000000 libesedb-20240202/libbfio/libbfio_file_range.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27543 2024-02-02 03:41:33.000000 libesedb-20240202/libbfio/libbfio_file_range_io_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2324 2024-02-02 03:41:33.000000 libesedb-20240202/libbfio/libbfio_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1362 2024-02-02 03:41:33.000000 libesedb-20240202/libbfio/libbfio_libcpath.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1772 2024-02-02 03:41:33.000000 libesedb-20240202/libbfio/libbfio_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-02-02 03:41:33.000000 libesedb-20240202/libbfio/libbfio_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2896 2024-02-02 03:41:33.000000 libesedb-20240202/libbfio/libbfio_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1733 2024-02-02 03:41:33.000000 libesedb-20240202/libbfio/libbfio_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4085 2024-02-02 03:41:33.000000 libesedb-20240202/libbfio/libbfio_file_io_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2077 2024-02-02 03:41:33.000000 libesedb-20240202/libbfio/libbfio_file_pool.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12186 2024-02-02 03:41:33.000000 libesedb-20240202/libbfio/libbfio_file_range.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1572 2024-02-02 03:41:33.000000 libesedb-20240202/libbfio/libbfio_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2024-02-02 03:41:33.000000 libesedb-20240202/libbfio/libbfio_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1545 2024-02-02 03:41:33.000000 libesedb-20240202/libbfio/libbfio_libcdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2234 2024-02-02 03:41:33.000000 libesedb-20240202/libbfio/libbfio_file.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-02-02 03:41:33.000000 libesedb-20240202/libbfio/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1420 2024-02-02 03:41:33.000000 libesedb-20240202/libbfio/libbfio_libcfile.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2708 2024-02-02 03:41:33.000000 libesedb-20240202/libbfio/libbfio_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2614 2024-02-02 03:41:33.000000 libesedb-20240202/libbfio/libbfio_codepage.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26845 2024-02-02 03:41:33.000000 libesedb-20240202/libbfio/libbfio_file_io_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1448 2024-02-02 03:41:33.000000 libesedb-20240202/libbfio/libbfio_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-02-02 03:41:33.000000 libesedb-20240202/libbfio/libbfio_memory_range.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10798 2024-02-02 03:41:33.000000 libesedb-20240202/libbfio/libbfio_file_pool.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4806 2024-02-02 03:41:33.000000 libesedb-20240202/libbfio/libbfio_file_range_io_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1918 2024-02-02 03:41:33.000000 libesedb-20240202/libbfio/libbfio_libcthreads.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2814 2024-02-02 03:41:33.000000 libesedb-20240202/libbfio/libbfio_system_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21082 2024-02-02 03:41:33.000000 libesedb-20240202/libbfio/libbfio_memory_range_io_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    64816 2024-02-02 03:41:33.000000 libesedb-20240202/libbfio/libbfio_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10899 2024-02-02 03:41:33.000000 libesedb-20240202/libbfio/libbfio_file.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8883 2024-02-02 03:41:33.000000 libesedb-20240202/libbfio/libbfio_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5821 2024-02-02 03:41:33.000000 libesedb-20240202/libbfio/libbfio_memory_range.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    81879 2024-02-02 03:41:33.000000 libesedb-20240202/libbfio/libbfio_pool.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2024-02-02 03:41:33.000000 libesedb-20240202/libbfio/libbfio_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34398 2024-02-02 03:42:05.000000 libesedb-20240202/libbfio/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25540 2024-02-02 03:41:33.000000 libesedb-20240202/libbfio/libbfio_system_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3835 2024-02-02 03:41:33.000000 libesedb-20240202/libbfio/libbfio_memory_range_io_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1376 2024-02-02 03:41:33.000000 libesedb-20240202/libbfio/libbfio_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6841 2024-02-02 03:41:33.000000 libesedb-20240202/libbfio/libbfio_pool.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       67 2023-12-03 09:00:45.000000 libesedb-20240202/ABOUT-NLS
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    49939 2024-02-02 03:42:05.000000 libesedb-20240202/config.guess
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-02 04:07:49.000000 libesedb-20240202/dpkg/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       18 2024-02-02 03:31:33.000000 libesedb-20240202/dpkg/libesedb-python3.install
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1026 2024-02-02 03:31:36.000000 libesedb-20240202/dpkg/copyright
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       22 2024-02-02 03:31:33.000000 libesedb-20240202/dpkg/libesedb.install
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-02 04:07:49.000000 libesedb-20240202/dpkg/source/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       12 2024-02-02 03:31:33.000000 libesedb-20240202/dpkg/source/format
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2206 2024-02-02 03:31:33.000000 libesedb-20240202/dpkg/control
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      769 2024-02-02 03:31:33.000000 libesedb-20240202/dpkg/rules
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      121 2024-02-02 03:31:33.000000 libesedb-20240202/dpkg/changelog.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      140 2024-02-02 03:42:15.000000 libesedb-20240202/dpkg/changelog
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        3 2024-02-02 03:31:33.000000 libesedb-20240202/dpkg/compat
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       96 2024-02-02 03:31:33.000000 libesedb-20240202/dpkg/libesedb-dev.install
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       27 2024-02-02 03:31:33.000000 libesedb-20240202/dpkg/libesedb-tools.install
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      486 2024-02-02 03:42:15.000000 libesedb-20240202/setup.cfg
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7652 2024-02-02 03:31:33.000000 libesedb-20240202/COPYING.LESSER
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-02 04:07:51.000000 libesedb-20240202/esedbtools/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5875 2024-02-02 03:32:44.000000 libesedb-20240202/esedbtools/esedbinfo.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1545 2024-02-02 03:31:36.000000 libesedb-20240202/esedbtools/esedbtools_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1467 2024-02-02 03:31:36.000000 libesedb-20240202/esedbtools/esedbtools_libcfile.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12269 2024-02-02 03:31:36.000000 libesedb-20240202/esedbtools/webcache.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1504 2024-02-02 03:31:36.000000 libesedb-20240202/esedbtools/esedbtools_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    78508 2024-02-02 03:31:36.000000 libesedb-20240202/esedbtools/windows_search.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1748 2024-02-02 03:31:36.000000 libesedb-20240202/esedbtools/esedbtools_libfwnt.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2724 2024-02-02 03:32:44.000000 libesedb-20240202/esedbtools/info_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1501 2024-02-02 03:31:36.000000 libesedb-20240202/esedbtools/esedbtools_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1443 2024-02-02 03:31:36.000000 libesedb-20240202/esedbtools/esedbtools_libfguid.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1454 2024-02-02 03:31:36.000000 libesedb-20240202/esedbtools/esedbtools_output.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6574 2024-02-02 03:31:36.000000 libesedb-20240202/esedbtools/srumdb.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1742 2024-02-02 03:31:36.000000 libesedb-20240202/esedbtools/esedbtools_libfmapi.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1494 2024-02-02 03:31:36.000000 libesedb-20240202/esedbtools/webcache.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4380 2024-02-02 03:31:36.000000 libesedb-20240202/esedbtools/esedbtools_output.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1213 2024-02-02 03:31:36.000000 libesedb-20240202/esedbtools/esedbtools_i18n.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1951 2024-02-02 03:31:36.000000 libesedb-20240202/esedbtools/windows_security.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6044 2024-02-02 03:31:36.000000 libesedb-20240202/esedbtools/database_types.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17428 2024-02-02 03:31:36.000000 libesedb-20240202/esedbtools/export.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2822 2023-12-03 09:01:07.000000 libesedb-20240202/esedbtools/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7769 2024-02-02 03:31:36.000000 libesedb-20240202/esedbtools/windows_search_compression.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5751 2024-02-02 03:31:36.000000 libesedb-20240202/esedbtools/esedbtools_signal.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1813 2024-02-02 03:31:36.000000 libesedb-20240202/esedbtools/esedbtools_getopt.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30817 2024-02-02 03:32:44.000000 libesedb-20240202/esedbtools/info_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    99282 2024-02-02 03:31:36.000000 libesedb-20240202/esedbtools/export_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1781 2024-02-02 03:31:36.000000 libesedb-20240202/esedbtools/esedbtools_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1554 2024-02-02 03:31:36.000000 libesedb-20240202/esedbtools/esedbtools_libcdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1771 2024-02-02 03:31:36.000000 libesedb-20240202/esedbtools/esedbtools_libfdatetime.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2959 2024-02-02 03:32:44.000000 libesedb-20240202/esedbtools/esedbtools_system_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1748 2024-02-02 03:31:36.000000 libesedb-20240202/esedbtools/esedbtools_libbfio.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5934 2024-02-02 03:31:36.000000 libesedb-20240202/esedbtools/log_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1896 2024-02-02 03:31:36.000000 libesedb-20240202/esedbtools/export.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1761 2024-02-02 03:31:36.000000 libesedb-20240202/esedbtools/esedbtools_signal.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12000 2024-02-02 03:31:36.000000 libesedb-20240202/esedbtools/esedbexport.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1483 2024-02-02 03:31:36.000000 libesedb-20240202/esedbtools/esedbtools_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2985 2024-02-02 03:31:36.000000 libesedb-20240202/esedbtools/windows_search.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6042 2024-02-02 03:31:36.000000 libesedb-20240202/esedbtools/export_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1762 2024-02-02 03:31:36.000000 libesedb-20240202/esedbtools/esedbtools_libfvalue.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      981 2024-02-02 03:31:36.000000 libesedb-20240202/esedbtools/esedbtools_libesedb.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1335 2024-02-02 03:31:36.000000 libesedb-20240202/esedbtools/srumdb.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1409 2024-02-02 03:31:36.000000 libesedb-20240202/esedbtools/esedbtools_libcpath.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    36780 2024-02-02 03:42:05.000000 libesedb-20240202/esedbtools/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1674 2024-02-02 03:31:36.000000 libesedb-20240202/esedbtools/log_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3617 2024-02-02 03:31:36.000000 libesedb-20240202/esedbtools/exchange.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1323 2024-02-02 03:32:44.000000 libesedb-20240202/esedbtools/esedbtools_system_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    85170 2024-02-02 03:31:36.000000 libesedb-20240202/esedbtools/exchange.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1597 2024-02-02 03:31:36.000000 libesedb-20240202/esedbtools/windows_search_compression.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23591 2024-02-02 03:31:36.000000 libesedb-20240202/esedbtools/windows_security.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1866 2024-02-02 03:31:36.000000 libesedb-20240202/esedbtools/database_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4535 2024-02-02 03:31:36.000000 libesedb-20240202/esedbtools/esedbtools_getopt.c
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)  2071504 2024-02-02 03:42:04.000000 libesedb-20240202/configure
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     7400 2024-02-02 03:42:05.000000 libesedb-20240202/compile
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     6878 2024-02-02 03:42:05.000000 libesedb-20240202/missing
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-02 04:07:51.000000 libesedb-20240202/libesedb/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1111 2024-02-02 03:42:15.000000 libesedb-20240202/libesedb/libesedb.rc
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7885 2024-02-02 03:31:35.000000 libesedb-20240202/libesedb/libesedb_definitions.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9034 2024-02-02 03:31:35.000000 libesedb-20240202/libesedb/libesedb_data_segment.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7344 2024-02-02 03:31:35.000000 libesedb-20240202/libesedb/esedb_file_header.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1842 2024-02-02 03:31:35.000000 libesedb-20240202/libesedb/libesedb_root_page_header.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-02-02 03:31:35.000000 libesedb-20240202/libesedb/libesedb_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1548 2024-02-02 03:31:35.000000 libesedb-20240202/libesedb/libesedb_libcdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3011 2024-02-02 03:31:35.000000 libesedb-20240202/libesedb/libesedb_column_type.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1553 2024-02-02 03:31:35.000000 libesedb-20240202/libesedb/libesedb_lcid.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-02-02 03:31:35.000000 libesedb-20240202/libesedb/libesedb_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19331 2024-02-02 03:31:35.000000 libesedb-20240202/libesedb/libesedb_file_header.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1709 2024-02-02 03:31:35.000000 libesedb-20240202/libesedb/libesedb_space_tree_value.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2840 2024-02-02 03:31:35.000000 libesedb-20240202/libesedb/libesedb_io_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4546 2024-02-02 03:31:35.000000 libesedb-20240202/libesedb/libesedb_leaf_page_descriptor.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1715 2024-02-02 03:31:35.000000 libesedb-20240202/libesedb/libesedb_i18n.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    41623 2024-02-02 03:31:35.000000 libesedb-20240202/libesedb/libesedb_multi_value.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1524 2024-02-02 03:31:35.000000 libesedb-20240202/libesedb/libesedb_block_descriptor.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2754 2024-02-02 03:31:35.000000 libesedb-20240202/libesedb/libesedb_notify.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2347 2024-02-02 03:31:35.000000 libesedb-20240202/libesedb/libesedb_block_tree.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3124 2024-02-02 03:32:44.000000 libesedb-20240202/libesedb/libesedb_codepage.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5067 2024-02-02 03:31:35.000000 libesedb-20240202/libesedb/libesedb_table.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7883 2024-02-02 03:42:15.000000 libesedb-20240202/libesedb/libesedb_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11397 2024-02-02 03:31:35.000000 libesedb-20240202/libesedb/libesedb_block_tree.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1985 2024-02-02 03:31:35.000000 libesedb-20240202/libesedb/libesedb_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3623 2024-02-02 03:31:35.000000 libesedb-20240202/libesedb/libesedb_catalog.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3434 2024-02-02 03:31:35.000000 libesedb-20240202/libesedb/libesedb_codepage.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4574 2024-02-02 03:31:35.000000 libesedb-20240202/libesedb/libesedb_file.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    38481 2024-02-02 03:31:35.000000 libesedb-20240202/libesedb/libesedb_page.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17716 2024-02-02 03:31:35.000000 libesedb-20240202/libesedb/libesedb_table_definition.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5705 2024-02-02 03:31:35.000000 libesedb-20240202/libesedb/libesedb_page_tree.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15964 2024-02-02 03:31:35.000000 libesedb-20240202/libesedb/libesedb_page_tree_key.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    78990 2024-02-02 03:31:35.000000 libesedb-20240202/libesedb/libesedb_page_tree.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3121 2024-02-02 03:31:35.000000 libesedb-20240202/libesedb/libesedb_block_descriptor.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15045 2024-02-02 03:31:35.000000 libesedb-20240202/libesedb/libesedb_block_tree_node.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9367 2024-02-02 03:31:35.000000 libesedb-20240202/libesedb/libesedb_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16782 2024-02-02 03:31:35.000000 libesedb-20240202/libesedb/libesedb_debug.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2713 2024-02-02 03:31:35.000000 libesedb-20240202/libesedb/libesedb_column.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    95847 2024-02-02 03:31:35.000000 libesedb-20240202/libesedb/libesedb_record.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1919 2024-02-02 03:31:35.000000 libesedb-20240202/libesedb/libesedb_leaf_page_descriptor.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1703 2024-02-02 03:31:35.000000 libesedb-20240202/libesedb/libesedb_libbfio.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3662 2023-12-03 09:01:09.000000 libesedb-20240202/libesedb/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-02-02 03:31:35.000000 libesedb-20240202/libesedb/libesedb_libfcache.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1593 2024-02-02 03:31:35.000000 libesedb-20240202/libesedb/libesedb_notify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5276 2024-02-02 03:31:35.000000 libesedb-20240202/libesedb/libesedb_catalog_definition.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3226 2024-02-02 03:31:35.000000 libesedb-20240202/libesedb/esedb_page.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-02-02 03:31:35.000000 libesedb-20240202/libesedb/libesedb_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1703 2024-02-02 03:31:35.000000 libesedb-20240202/libesedb/libesedb_libfwnt.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1354 2024-02-02 03:31:35.000000 libesedb-20240202/libesedb/libesedb_i18n.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5737 2024-02-02 03:31:35.000000 libesedb-20240202/libesedb/libesedb_value_data_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2061 2024-02-02 03:31:35.000000 libesedb-20240202/libesedb/libesedb_page_tree_key.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2977 2024-02-02 03:31:35.000000 libesedb-20240202/libesedb/libesedb_page_value.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15369 2024-02-02 03:31:35.000000 libesedb-20240202/libesedb/libesedb_checksum.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18457 2024-02-02 03:31:35.000000 libesedb-20240202/libesedb/libesedb_index.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5942 2024-02-02 03:31:35.000000 libesedb-20240202/libesedb/libesedb_multi_value.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-02-02 03:31:35.000000 libesedb-20240202/libesedb/libesedb_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11330 2024-02-02 03:31:35.000000 libesedb-20240202/libesedb/libesedb_column.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-02-02 03:31:35.000000 libesedb-20240202/libesedb/libesedb_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1113 2024-02-02 03:31:35.000000 libesedb-20240202/libesedb/libesedb.rc.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7230 2024-02-02 03:31:35.000000 libesedb-20240202/libesedb/libesedb_io_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1545 2024-02-02 03:31:35.000000 libesedb-20240202/libesedb/libesedb_libfdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1856 2024-02-02 03:31:35.000000 libesedb-20240202/libesedb/libesedb.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    49390 2024-02-02 03:31:35.000000 libesedb-20240202/libesedb/libesedb_file.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14047 2024-02-02 03:31:35.000000 libesedb-20240202/libesedb/libesedb_page_header.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4754 2024-02-02 03:31:35.000000 libesedb-20240202/libesedb/libesedb_space_tree_value.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3115 2024-02-02 03:31:35.000000 libesedb-20240202/libesedb/libesedb_compression.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7281 2024-02-02 03:31:35.000000 libesedb-20240202/libesedb/libesedb_root_page_header.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1736 2024-02-02 03:31:35.000000 libesedb-20240202/libesedb/libesedb_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4225 2024-02-02 03:31:35.000000 libesedb-20240202/libesedb/libesedb_index.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8883 2024-02-02 03:31:35.000000 libesedb-20240202/libesedb/libesedb_record.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3847 2024-02-02 03:31:35.000000 libesedb-20240202/libesedb/libesedb_table_definition.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4118 2024-02-02 03:31:35.000000 libesedb-20240202/libesedb/libesedb_long_value.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2263 2024-02-02 03:31:35.000000 libesedb-20240202/libesedb/libesedb_data_segment.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32872 2024-02-02 03:31:35.000000 libesedb-20240202/libesedb/libesedb_catalog.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11826 2024-02-02 03:31:35.000000 libesedb-20240202/libesedb/libesedb_record_value.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    38738 2024-02-02 03:31:35.000000 libesedb-20240202/libesedb/libesedb_table.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-02-02 03:31:35.000000 libesedb-20240202/libesedb/libesedb_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1784 2024-02-02 03:31:35.000000 libesedb-20240202/libesedb/libesedb_record_value.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2277 2024-02-02 03:31:35.000000 libesedb-20240202/libesedb/libesedb_debug.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2836 2024-02-02 03:31:35.000000 libesedb-20240202/libesedb/libesedb_page_header.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2949 2024-02-02 03:31:35.000000 libesedb-20240202/libesedb/libesedb_block_tree_node.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3339 2024-02-02 03:31:35.000000 libesedb-20240202/libesedb/libesedb_data_definition.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1791 2024-02-02 03:31:35.000000 libesedb-20240202/libesedb/libesedb_libfvalue.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    55707 2024-02-02 03:31:35.000000 libesedb-20240202/libesedb/libesedb_data_definition.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2200 2024-02-02 03:31:35.000000 libesedb-20240202/libesedb/libesedb_space_tree.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18749 2024-02-02 03:31:35.000000 libesedb-20240202/libesedb/libesedb_lcid.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20066 2024-02-02 03:31:35.000000 libesedb-20240202/libesedb/libesedb_space_tree.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2024-02-02 03:31:35.000000 libesedb-20240202/libesedb/libesedb_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6795 2024-02-02 03:31:35.000000 libesedb-20240202/libesedb/libesedb_page_tree_value.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    43667 2024-02-02 03:42:05.000000 libesedb-20240202/libesedb/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2141 2024-02-02 03:31:35.000000 libesedb-20240202/libesedb/libesedb_database.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30559 2024-02-02 03:31:35.000000 libesedb-20240202/libesedb/libesedb_compression.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2195 2024-02-02 03:31:35.000000 libesedb-20240202/libesedb/libesedb_file_header.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1914 2024-02-02 03:31:35.000000 libesedb-20240202/libesedb/libesedb_page_tree_value.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-02-02 03:31:35.000000 libesedb-20240202/libesedb/libesedb_value_data_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3862 2024-02-02 03:31:35.000000 libesedb-20240202/libesedb/libesedb_page.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    50190 2024-02-02 03:31:35.000000 libesedb-20240202/libesedb/libesedb_catalog_definition.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33342 2024-02-02 03:31:35.000000 libesedb-20240202/libesedb/libesedb_long_value.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5517 2024-02-02 03:31:35.000000 libesedb-20240202/libesedb/esedb_page_values.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1527 2024-02-02 03:31:35.000000 libesedb-20240202/libesedb/libesedb_checksum.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1556 2024-02-02 03:31:35.000000 libesedb-20240202/libesedb/libesedb_column_type.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1612 2024-02-02 03:31:35.000000 libesedb-20240202/libesedb/libesedb_page_value.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13891 2024-02-02 03:31:35.000000 libesedb-20240202/libesedb/libesedb_database.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2053 2024-02-02 03:31:35.000000 libesedb-20240202/libesedb/libesedb_types.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-02 04:07:51.000000 libesedb-20240202/msvscpp/
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-02 04:07:51.000000 libesedb-20240202/msvscpp/esedb_test_page_tree_value/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5983 2024-02-02 03:32:22.000000 libesedb-20240202/msvscpp/esedb_test_page_tree_value/esedb_test_page_tree_value.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-02 04:07:51.000000 libesedb-20240202/msvscpp/libfdata/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6858 2024-02-02 03:32:02.000000 libesedb-20240202/msvscpp/libfdata/libfdata.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-02 04:07:51.000000 libesedb-20240202/msvscpp/esedb_test_long_value/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5968 2024-02-02 03:32:22.000000 libesedb-20240202/msvscpp/esedb_test_long_value/esedb_test_long_value.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-02 04:07:51.000000 libesedb-20240202/msvscpp/esedb_test_space_tree/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5968 2024-02-02 03:32:22.000000 libesedb-20240202/msvscpp/esedb_test_space_tree/esedb_test_space_tree.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-02 04:07:51.000000 libesedb-20240202/msvscpp/esedb_test_file/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6613 2024-02-02 03:32:22.000000 libesedb-20240202/msvscpp/esedb_test_file/esedb_test_file.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-02 04:07:51.000000 libesedb-20240202/msvscpp/esedb_test_space_tree_value/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5986 2024-02-02 03:32:22.000000 libesedb-20240202/msvscpp/esedb_test_space_tree_value/esedb_test_space_tree_value.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-02 04:07:51.000000 libesedb-20240202/msvscpp/esedb_test_block_tree_node/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5983 2024-02-02 03:32:22.000000 libesedb-20240202/msvscpp/esedb_test_block_tree_node/esedb_test_block_tree_node.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-02 04:07:51.000000 libesedb-20240202/msvscpp/esedb_test_checksum/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5962 2024-02-02 03:32:22.000000 libesedb-20240202/msvscpp/esedb_test_checksum/esedb_test_checksum.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-02 04:07:51.000000 libesedb-20240202/msvscpp/esedb_test_block_descriptor/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5986 2024-02-02 03:32:22.000000 libesedb-20240202/msvscpp/esedb_test_block_descriptor/esedb_test_block_descriptor.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-02 04:07:51.000000 libesedb-20240202/msvscpp/esedb_test_database/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5962 2024-02-02 03:32:22.000000 libesedb-20240202/msvscpp/esedb_test_database/esedb_test_database.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-02 04:07:51.000000 libesedb-20240202/msvscpp/esedbexport/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9040 2024-02-02 03:32:02.000000 libesedb-20240202/msvscpp/esedbexport/esedbexport.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-02 04:07:51.000000 libesedb-20240202/msvscpp/esedb_test_table/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5953 2024-02-02 03:32:22.000000 libesedb-20240202/msvscpp/esedb_test_table/esedb_test_table.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-02 04:07:51.000000 libesedb-20240202/msvscpp/esedbinfo/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7122 2024-02-02 03:32:02.000000 libesedb-20240202/msvscpp/esedbinfo/esedbinfo.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-02 04:07:51.000000 libesedb-20240202/msvscpp/esedb_test_page/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6200 2024-02-02 03:32:22.000000 libesedb-20240202/msvscpp/esedb_test_page/esedb_test_page.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-02 04:07:51.000000 libesedb-20240202/msvscpp/esedb_test_column_type/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5971 2024-02-02 03:32:22.000000 libesedb-20240202/msvscpp/esedb_test_column_type/esedb_test_column_type.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-02 04:07:51.000000 libesedb-20240202/msvscpp/libfguid/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4631 2024-02-02 03:32:02.000000 libesedb-20240202/msvscpp/libfguid/libfguid.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-02 04:07:51.000000 libesedb-20240202/msvscpp/esedb_test_catalog_definition/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5992 2024-02-02 03:32:22.000000 libesedb-20240202/msvscpp/esedb_test_catalog_definition/esedb_test_catalog_definition.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-02 04:07:51.000000 libesedb-20240202/msvscpp/esedb_test_tools_windows_search_compression/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6141 2024-02-02 03:32:22.000000 libesedb-20240202/msvscpp/esedb_test_tools_windows_search_compression/esedb_test_tools_windows_search_compression.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-02 04:07:51.000000 libesedb-20240202/msvscpp/libclocale/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4778 2024-02-02 03:32:02.000000 libesedb-20240202/msvscpp/libclocale/libclocale.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-02 04:07:51.000000 libesedb-20240202/msvscpp/esedb_test_data_definition/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5983 2024-02-02 03:32:22.000000 libesedb-20240202/msvscpp/esedb_test_data_definition/esedb_test_data_definition.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-02 04:07:51.000000 libesedb-20240202/msvscpp/esedb_test_support/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6622 2024-02-02 03:32:22.000000 libesedb-20240202/msvscpp/esedb_test_support/esedb_test_support.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-02 04:07:51.000000 libesedb-20240202/msvscpp/esedb_test_index/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5953 2024-02-02 03:32:22.000000 libesedb-20240202/msvscpp/esedb_test_index/esedb_test_index.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-02 04:07:51.000000 libesedb-20240202/msvscpp/libfcache/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5237 2024-02-02 03:32:02.000000 libesedb-20240202/msvscpp/libfcache/libfcache.vcproj
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2937 2024-02-02 03:32:22.000000 libesedb-20240202/msvscpp/Makefile.am
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-02 04:07:51.000000 libesedb-20240202/msvscpp/libbfio/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7306 2024-02-02 03:32:02.000000 libesedb-20240202/msvscpp/libbfio/libbfio.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-02 04:07:51.000000 libesedb-20240202/msvscpp/esedb_test_column/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5956 2024-02-02 03:32:22.000000 libesedb-20240202/msvscpp/esedb_test_column/esedb_test_column.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-02 04:07:51.000000 libesedb-20240202/msvscpp/libesedb/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13652 2024-02-02 03:32:02.000000 libesedb-20240202/msvscpp/libesedb/libesedb.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-02 04:07:51.000000 libesedb-20240202/msvscpp/esedb_test_leaf_page_descriptor/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6081 2024-02-02 03:32:22.000000 libesedb-20240202/msvscpp/esedb_test_leaf_page_descriptor/esedb_test_leaf_page_descriptor.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-02 04:07:51.000000 libesedb-20240202/msvscpp/esedb_test_block_tree/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5968 2024-02-02 03:32:22.000000 libesedb-20240202/msvscpp/esedb_test_block_tree/esedb_test_block_tree.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-02 04:07:51.000000 libesedb-20240202/msvscpp/esedb_test_io_handle/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5965 2024-02-02 03:32:22.000000 libesedb-20240202/msvscpp/esedb_test_io_handle/esedb_test_io_handle.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-02 04:07:51.000000 libesedb-20240202/msvscpp/libcfile/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5597 2024-02-02 03:32:02.000000 libesedb-20240202/msvscpp/libcfile/libcfile.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-02 04:07:51.000000 libesedb-20240202/msvscpp/libmapidb/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4987 2024-02-02 03:32:02.000000 libesedb-20240202/msvscpp/libmapidb/libmapidb.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-02 04:07:51.000000 libesedb-20240202/msvscpp/esedb_test_compression/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5971 2024-02-02 03:32:22.000000 libesedb-20240202/msvscpp/esedb_test_compression/esedb_test_compression.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-02 04:07:51.000000 libesedb-20240202/msvscpp/libcdata/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6172 2024-02-02 03:32:02.000000 libesedb-20240202/msvscpp/libcdata/libcdata.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-02 04:07:51.000000 libesedb-20240202/msvscpp/esedb_test_page_tree_key/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6060 2024-02-02 03:32:22.000000 libesedb-20240202/msvscpp/esedb_test_page_tree_key/esedb_test_page_tree_key.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-02 04:07:51.000000 libesedb-20240202/msvscpp/libfmapi/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7276 2024-02-02 03:32:02.000000 libesedb-20240202/msvscpp/libfmapi/libfmapi.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-02 04:07:51.000000 libesedb-20240202/msvscpp/esedb_test_file_header/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6221 2024-02-02 03:32:22.000000 libesedb-20240202/msvscpp/esedb_test_file_header/esedb_test_file_header.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-02 04:07:51.000000 libesedb-20240202/msvscpp/esedb_test_tools_info_handle/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6066 2024-02-02 03:32:22.000000 libesedb-20240202/msvscpp/esedb_test_tools_info_handle/esedb_test_tools_info_handle.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-02 04:07:51.000000 libesedb-20240202/msvscpp/pyesedb/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8339 2024-02-02 03:32:22.000000 libesedb-20240202/msvscpp/pyesedb/pyesedb.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-02 04:07:51.000000 libesedb-20240202/msvscpp/esedb_test_page_value/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5968 2024-02-02 03:32:22.000000 libesedb-20240202/msvscpp/esedb_test_page_value/esedb_test_page_value.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-02 04:07:51.000000 libesedb-20240202/msvscpp/esedb_test_root_page_header/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5986 2024-02-02 03:32:22.000000 libesedb-20240202/msvscpp/esedb_test_root_page_header/esedb_test_root_page_header.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-02 04:07:51.000000 libesedb-20240202/msvscpp/libcthreads/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6177 2024-02-02 03:32:02.000000 libesedb-20240202/msvscpp/libcthreads/libcthreads.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-02 04:07:51.000000 libesedb-20240202/msvscpp/esedb_test_tools_output/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5901 2024-02-02 03:32:22.000000 libesedb-20240202/msvscpp/esedb_test_tools_output/esedb_test_tools_output.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-02 04:07:51.000000 libesedb-20240202/msvscpp/libcpath/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5183 2024-02-02 03:32:02.000000 libesedb-20240202/msvscpp/libcpath/libcpath.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-02 04:07:51.000000 libesedb-20240202/msvscpp/esedb_test_tools_signal/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5901 2024-02-02 03:32:22.000000 libesedb-20240202/msvscpp/esedb_test_tools_signal/esedb_test_tools_signal.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-02 04:07:51.000000 libesedb-20240202/msvscpp/libfwnt/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6895 2024-02-02 03:32:02.000000 libesedb-20240202/msvscpp/libfwnt/libfwnt.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-02 04:07:51.000000 libesedb-20240202/msvscpp/esedb_test_table_definition/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5986 2024-02-02 03:32:22.000000 libesedb-20240202/msvscpp/esedb_test_table_definition/esedb_test_table_definition.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-02 04:07:51.000000 libesedb-20240202/msvscpp/esedb_test_multi_value/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5971 2024-02-02 03:32:22.000000 libesedb-20240202/msvscpp/esedb_test_multi_value/esedb_test_multi_value.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-02 04:07:51.000000 libesedb-20240202/msvscpp/esedb_test_catalog/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6292 2024-02-02 03:32:22.000000 libesedb-20240202/msvscpp/esedb_test_catalog/esedb_test_catalog.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-02 04:07:51.000000 libesedb-20240202/msvscpp/libcsplit/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5225 2024-02-02 03:32:02.000000 libesedb-20240202/msvscpp/libcsplit/libcsplit.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-02 04:07:51.000000 libesedb-20240202/msvscpp/esedb_test_record/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5956 2024-02-02 03:32:22.000000 libesedb-20240202/msvscpp/esedb_test_record/esedb_test_record.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-02 04:07:51.000000 libesedb-20240202/msvscpp/libuna/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15387 2024-02-02 03:32:02.000000 libesedb-20240202/msvscpp/libuna/libuna.vcproj
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25841 2024-02-02 03:42:06.000000 libesedb-20240202/msvscpp/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-02 04:07:51.000000 libesedb-20240202/msvscpp/libfvalue/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8076 2024-02-02 03:32:02.000000 libesedb-20240202/msvscpp/libfvalue/libfvalue.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-02 04:07:51.000000 libesedb-20240202/msvscpp/esedb_test_page_tree/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5965 2024-02-02 03:32:22.000000 libesedb-20240202/msvscpp/esedb_test_page_tree/esedb_test_page_tree.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-02 04:07:51.000000 libesedb-20240202/msvscpp/esedb_test_error/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5707 2024-02-02 03:32:22.000000 libesedb-20240202/msvscpp/esedb_test_error/esedb_test_error.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-02 04:07:51.000000 libesedb-20240202/msvscpp/esedb_test_data_segment/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6391 2024-02-02 03:32:22.000000 libesedb-20240202/msvscpp/esedb_test_data_segment/esedb_test_data_segment.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-02 04:07:51.000000 libesedb-20240202/msvscpp/libcnotify/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4764 2024-02-02 03:32:02.000000 libesedb-20240202/msvscpp/libcnotify/libcnotify.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-02 04:07:51.000000 libesedb-20240202/msvscpp/libcerror/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4488 2024-02-02 03:32:02.000000 libesedb-20240202/msvscpp/libcerror/libcerror.vcproj
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    53317 2024-02-02 03:32:22.000000 libesedb-20240202/msvscpp/libesedb.sln
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-02 04:07:51.000000 libesedb-20240202/msvscpp/esedb_test_notify/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5794 2024-02-02 03:32:22.000000 libesedb-20240202/msvscpp/esedb_test_notify/esedb_test_notify.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-02 04:07:51.000000 libesedb-20240202/msvscpp/libfdatetime/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6069 2024-02-02 03:32:02.000000 libesedb-20240202/msvscpp/libfdatetime/libfdatetime.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-02 04:07:51.000000 libesedb-20240202/msvscpp/esedb_test_page_header/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5971 2024-02-02 03:32:22.000000 libesedb-20240202/msvscpp/esedb_test_page_header/esedb_test_page_header.vcproj
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       92 2024-02-02 03:31:34.000000 libesedb-20240202/AUTHORS
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-02 04:07:50.000000 libesedb-20240202/libcfile/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-02-02 03:41:37.000000 libesedb-20240202/libcfile/libcfile_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2389 2024-02-02 03:41:37.000000 libesedb-20240202/libcfile/libcfile_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-02-02 03:41:37.000000 libesedb-20240202/libcfile/libcfile_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1593 2024-02-02 03:41:37.000000 libesedb-20240202/libcfile/libcfile_notify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25753 2024-02-02 03:41:37.000000 libesedb-20240202/libcfile/libcfile_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1497 2024-02-02 03:41:37.000000 libesedb-20240202/libcfile/libcfile_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      942 2024-02-02 03:41:37.000000 libesedb-20240202/libcfile/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2754 2024-02-02 03:41:37.000000 libesedb-20240202/libcfile/libcfile_notify.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2826 2024-02-02 03:41:37.000000 libesedb-20240202/libcfile/libcfile_system_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6452 2024-02-02 03:41:37.000000 libesedb-20240202/libcfile/libcfile_file.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-02-02 03:41:37.000000 libesedb-20240202/libcfile/libcfile_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25560 2024-02-02 03:41:37.000000 libesedb-20240202/libcfile/libcfile_system_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-02-02 03:41:37.000000 libesedb-20240202/libcfile/libcfile_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-02-02 03:41:37.000000 libesedb-20240202/libcfile/libcfile_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   105597 2024-02-02 03:41:37.000000 libesedb-20240202/libcfile/libcfile_file.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2024-02-02 03:41:37.000000 libesedb-20240202/libcfile/libcfile_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3107 2024-02-02 03:41:37.000000 libesedb-20240202/libcfile/libcfile_winapi.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31703 2024-02-02 03:42:05.000000 libesedb-20240202/libcfile/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-02-02 03:41:37.000000 libesedb-20240202/libcfile/libcfile_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1736 2024-02-02 03:41:37.000000 libesedb-20240202/libcfile/libcfile_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18388 2024-02-02 03:41:37.000000 libesedb-20240202/libcfile/libcfile_winapi.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2879 2024-02-02 03:41:37.000000 libesedb-20240202/libcfile/libcfile_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      856 2024-02-02 03:32:22.000000 libesedb-20240202/README
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-02 04:07:51.000000 libesedb-20240202/libmapidb/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1390 2024-02-02 03:41:53.000000 libesedb-20240202/libmapidb/libmapidb_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1381 2024-02-02 03:41:53.000000 libesedb-20240202/libmapidb/libmapidb_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1537 2024-02-02 03:41:53.000000 libesedb-20240202/libmapidb/libmapidb_folder.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1820 2024-02-02 03:41:53.000000 libesedb-20240202/libmapidb/libmapidb_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      749 2024-02-02 03:41:53.000000 libesedb-20240202/libmapidb/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1733 2024-02-02 03:41:53.000000 libesedb-20240202/libmapidb/libmapidb_database.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1615 2024-02-02 03:41:53.000000 libesedb-20240202/libmapidb/libmapidb_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3222 2024-02-02 03:41:53.000000 libesedb-20240202/libmapidb/libmapidb_folder.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3314 2024-02-02 03:41:53.000000 libesedb-20240202/libmapidb/libmapidb_database.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1444 2024-02-02 03:41:53.000000 libesedb-20240202/libmapidb/libmapidb_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30890 2024-02-02 03:42:06.000000 libesedb-20240202/libmapidb/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1201 2024-02-02 03:41:53.000000 libesedb-20240202/libmapidb/libmapidb_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1393 2024-02-02 03:41:53.000000 libesedb-20240202/libmapidb/libmapidb_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1538 2024-02-02 03:41:53.000000 libesedb-20240202/libmapidb/libmapidb_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2926 2024-02-02 03:41:53.000000 libesedb-20240202/libmapidb/libmapidb_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1174 2024-02-02 03:41:53.000000 libesedb-20240202/libmapidb/libmapidb_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15766 2024-02-02 03:42:05.000000 libesedb-20240202/INSTALL
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-02 04:07:50.000000 libesedb-20240202/libcdata/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3871 2024-02-02 03:41:35.000000 libesedb-20240202/libcdata/libcdata_list_element.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5231 2024-02-02 03:41:35.000000 libesedb-20240202/libcdata/libcdata_array.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2115 2024-02-02 03:41:35.000000 libesedb-20240202/libcdata/libcdata_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-02-02 03:41:35.000000 libesedb-20240202/libcdata/libcdata_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-02-02 03:41:35.000000 libesedb-20240202/libcdata/libcdata_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3790 2024-02-02 03:41:35.000000 libesedb-20240202/libcdata/libcdata_btree.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22358 2024-02-02 03:41:35.000000 libesedb-20240202/libcdata/libcdata_btree.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1152 2024-02-02 03:41:35.000000 libesedb-20240202/libcdata/libcdata_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    69515 2024-02-02 03:41:35.000000 libesedb-20240202/libcdata/libcdata_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-02-02 03:41:35.000000 libesedb-20240202/libcdata/libcdata_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6448 2024-02-02 03:41:35.000000 libesedb-20240202/libcdata/libcdata_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1648 2024-02-02 03:41:35.000000 libesedb-20240202/libcdata/libcdata_btree_values_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1127 2024-02-02 03:41:35.000000 libesedb-20240202/libcdata/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2960 2024-02-02 03:41:35.000000 libesedb-20240202/libcdata/libcdata_btree_node.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2789 2024-02-02 03:41:35.000000 libesedb-20240202/libcdata/libcdata_range_list_value.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12295 2024-02-02 03:41:35.000000 libesedb-20240202/libcdata/libcdata_range_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   122285 2024-02-02 03:41:35.000000 libesedb-20240202/libcdata/libcdata_range_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    49968 2024-02-02 03:41:35.000000 libesedb-20240202/libcdata/libcdata_array.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23846 2024-02-02 03:41:35.000000 libesedb-20240202/libcdata/libcdata_list_element.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1925 2024-02-02 03:41:35.000000 libesedb-20240202/libcdata/libcdata_libcthreads.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8365 2024-02-02 03:41:35.000000 libesedb-20240202/libcdata/libcdata_tree_node.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-02-02 03:41:35.000000 libesedb-20240202/libcdata/libcdata_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1976 2024-02-02 03:41:35.000000 libesedb-20240202/libcdata/libcdata_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37549 2024-02-02 03:41:35.000000 libesedb-20240202/libcdata/libcdata_btree_node.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   100501 2024-02-02 03:41:35.000000 libesedb-20240202/libcdata/libcdata_tree_node.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1230 2024-02-02 03:41:35.000000 libesedb-20240202/libcdata/libcdata_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33387 2024-02-02 03:42:05.000000 libesedb-20240202/libcdata/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10647 2024-02-02 03:41:35.000000 libesedb-20240202/libcdata/libcdata_range_list_value.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5251 2024-02-02 03:41:35.000000 libesedb-20240202/libcdata/libcdata_btree_values_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-02-02 03:41:35.000000 libesedb-20240202/libcdata/libcdata_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       91 2024-02-02 03:31:33.000000 libesedb-20240202/pyproject.toml
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-02 04:07:51.000000 libesedb-20240202/libfmapi/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1508 2024-02-02 03:41:49.000000 libesedb-20240202/libfmapi/libfmapi_value_type.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   124848 2024-02-02 03:41:49.000000 libesedb-20240202/libfmapi/libfmapi_debug.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1913 2024-02-02 03:41:49.000000 libesedb-20240202/libfmapi/libfmapi_x400_object_identifier.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1398 2024-02-02 03:41:49.000000 libesedb-20240202/libfmapi/libfmapi_libfguid.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1377 2024-02-02 03:41:49.000000 libesedb-20240202/libfmapi/libfmapi_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2174 2024-02-02 03:41:49.000000 libesedb-20240202/libfmapi/libfmapi_entry_identifier.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1703 2024-02-02 03:41:49.000000 libesedb-20240202/libfmapi/libfmapi_libfwnt.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    40853 2024-02-02 03:41:49.000000 libesedb-20240202/libfmapi/libfmapi_one_off_entry_identifier.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5468 2024-02-02 03:41:49.000000 libesedb-20240202/libfmapi/libfmapi_one_off_entry_identifier.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1543 2024-02-02 03:41:49.000000 libesedb-20240202/libfmapi/libfmapi_codepage.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3422 2024-02-02 03:41:49.000000 libesedb-20240202/libfmapi/libfmapi_codepage.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1510 2024-02-02 03:41:49.000000 libesedb-20240202/libfmapi/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-02-02 03:41:49.000000 libesedb-20240202/libfmapi/libfmapi_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2927 2024-02-02 03:41:49.000000 libesedb-20240202/libfmapi/libfmapi_debug.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10342 2024-02-02 03:41:49.000000 libesedb-20240202/libfmapi/libfmapi_entry_identifier.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2951 2024-02-02 03:41:49.000000 libesedb-20240202/libfmapi/libfmapi_class_identifier.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3877 2024-02-02 03:41:49.000000 libesedb-20240202/libfmapi/libfmapi_value_type.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1736 2024-02-02 03:41:49.000000 libesedb-20240202/libfmapi/libfmapi_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2189 2024-02-02 03:41:49.000000 libesedb-20240202/libfmapi/libfmapi_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1152 2024-02-02 03:41:49.000000 libesedb-20240202/libfmapi/libfmapi_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-02-02 03:41:49.000000 libesedb-20240202/libfmapi/libfmapi_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5127 2024-02-02 03:41:49.000000 libesedb-20240202/libfmapi/libfmapi_class_identifier.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1670 2024-02-02 03:41:49.000000 libesedb-20240202/libfmapi/libfmapi_checksum.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4882 2024-02-02 03:41:49.000000 libesedb-20240202/libfmapi/libfmapi_checksum.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   158504 2024-02-02 03:41:49.000000 libesedb-20240202/libfmapi/libfmapi_property_type.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1726 2024-02-02 03:41:49.000000 libesedb-20240202/libfmapi/libfmapi_libfdatetime.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16455 2024-02-02 03:41:49.000000 libesedb-20240202/libfmapi/libfmapi_lzfu.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1677 2024-02-02 03:41:49.000000 libesedb-20240202/libfmapi/libfmapi_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3352 2024-02-02 03:41:49.000000 libesedb-20240202/libfmapi/libfmapi_property_type.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2015 2024-02-02 03:41:49.000000 libesedb-20240202/libfmapi/libfmapi_lzfu.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-02-02 03:41:49.000000 libesedb-20240202/libfmapi/libfmapi_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2780 2024-02-02 03:41:49.000000 libesedb-20240202/libfmapi/libfmapi_service_provider_identifier.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-02-02 03:41:49.000000 libesedb-20240202/libfmapi/libfmapi_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34723 2024-02-02 03:42:06.000000 libesedb-20240202/libfmapi/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1230 2024-02-02 03:41:49.000000 libesedb-20240202/libfmapi/libfmapi_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-02-02 03:41:49.000000 libesedb-20240202/libfmapi/libfmapi_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1523 2024-02-02 03:41:49.000000 libesedb-20240202/libfmapi/libfmapi_service_provider_identifier.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      487 2024-02-02 03:31:33.000000 libesedb-20240202/setup.cfg.in
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    35796 2024-02-02 03:42:05.000000 libesedb-20240202/config.sub
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2500 2024-02-02 03:42:15.000000 libesedb-20240202/libesedb.spec
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     9278 2024-02-02 03:31:33.000000 libesedb-20240202/setup.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1485 2024-02-02 03:31:33.000000 libesedb-20240202/acinclude.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      763 2024-02-02 03:31:33.000000 libesedb-20240202/libesedb.pc.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-02 04:07:51.000000 libesedb-20240202/pyesedb/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1525 2024-02-02 03:31:35.000000 libesedb-20240202/pyesedb/pyesedb_libbfio.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9143 2024-02-02 03:31:36.000000 libesedb-20240202/pyesedb/pyesedb_records.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-02-02 03:31:35.000000 libesedb-20240202/pyesedb/pyesedb_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2024-02-02 03:31:35.000000 libesedb-20240202/pyesedb/pyesedb_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2361 2024-02-02 03:31:36.000000 libesedb-20240202/pyesedb/pyesedb_tables.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2382 2024-02-02 03:31:36.000000 libesedb-20240202/pyesedb/pyesedb_records.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1540 2024-02-02 03:31:35.000000 libesedb-20240202/pyesedb/pyesedb_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19373 2024-02-02 03:32:44.000000 libesedb-20240202/pyesedb/pyesedb.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21412 2024-02-02 03:32:44.000000 libesedb-20240202/pyesedb/pyesedb_multi_value.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4118 2024-02-02 03:31:35.000000 libesedb-20240202/pyesedb/pyesedb_file_object_io_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14701 2024-02-02 03:32:44.000000 libesedb-20240202/pyesedb/pyesedb_index.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22344 2024-02-02 03:32:44.000000 libesedb-20240202/pyesedb/pyesedb_table.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2414 2024-02-02 03:31:35.000000 libesedb-20240202/pyesedb/pyesedb_index.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2661 2024-02-02 03:32:44.000000 libesedb-20240202/pyesedb/pyesedb_multi_value.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1648 2023-12-03 09:01:07.000000 libesedb-20240202/pyesedb/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1648 2024-02-02 03:31:35.000000 libesedb-20240202/pyesedb/pyesedb_column_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16609 2024-02-02 03:31:35.000000 libesedb-20240202/pyesedb/pyesedb_datetime.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5524 2024-02-02 03:31:35.000000 libesedb-20240202/pyesedb/pyesedb_file_types.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3527 2024-02-02 03:32:44.000000 libesedb-20240202/pyesedb/pyesedb_file.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2033 2024-02-02 03:31:36.000000 libesedb-20240202/pyesedb/pyesedb_python.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9143 2024-02-02 03:31:35.000000 libesedb-20240202/pyesedb/pyesedb_columns.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2055 2024-02-02 03:32:44.000000 libesedb-20240202/pyesedb/pyesedb_long_value.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9546 2024-02-02 03:31:35.000000 libesedb-20240202/pyesedb/pyesedb_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1544 2024-02-02 03:31:35.000000 libesedb-20240202/pyesedb/pyesedb_integer.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1860 2024-02-02 03:31:35.000000 libesedb-20240202/pyesedb/pyesedb.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8876 2024-02-02 03:31:35.000000 libesedb-20240202/pyesedb/pyesedb_integer.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      973 2024-02-02 03:31:35.000000 libesedb-20240202/pyesedb/pyesedb_libesedb.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9131 2024-02-02 03:31:35.000000 libesedb-20240202/pyesedb/pyesedb_indexes.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34152 2024-02-02 03:32:44.000000 libesedb-20240202/pyesedb/pyesedb_record.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9081 2024-02-02 03:31:36.000000 libesedb-20240202/pyesedb/pyesedb_tables.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33880 2024-02-02 03:31:35.000000 libesedb-20240202/pyesedb/pyesedb_file_object_io_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2024-02-02 03:31:36.000000 libesedb-20240202/pyesedb/pyesedb_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1826 2024-02-02 03:31:35.000000 libesedb-20240202/pyesedb/pyesedb_datetime.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6224 2024-02-02 03:31:36.000000 libesedb-20240202/pyesedb/pyesedb_value_flags.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3033 2024-02-02 03:32:44.000000 libesedb-20240202/pyesedb/pyesedb_table.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2058 2024-02-02 03:31:35.000000 libesedb-20240202/pyesedb/pyesedb_column.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2382 2024-02-02 03:31:35.000000 libesedb-20240202/pyesedb/pyesedb_indexes.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10759 2024-02-02 03:32:44.000000 libesedb-20240202/pyesedb/pyesedb_column.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10628 2024-02-02 03:32:44.000000 libesedb-20240202/pyesedb/pyesedb_long_value.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28235 2024-02-02 03:32:44.000000 libesedb-20240202/pyesedb/pyesedb_file.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2382 2024-02-02 03:31:35.000000 libesedb-20240202/pyesedb/pyesedb_columns.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    61481 2024-02-02 03:42:06.000000 libesedb-20240202/pyesedb/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1634 2024-02-02 03:31:36.000000 libesedb-20240202/pyesedb/pyesedb_value_flags.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1620 2024-02-02 03:31:35.000000 libesedb-20240202/pyesedb/pyesedb_file_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11099 2024-02-02 03:31:35.000000 libesedb-20240202/pyesedb/pyesedb_column_types.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3594 2024-02-02 03:32:44.000000 libesedb-20240202/pyesedb/pyesedb_record.h
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    18574 2023-12-03 09:00:45.000000 libesedb-20240202/config.rpath
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-02 04:07:50.000000 libesedb-20240202/libcthreads/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2356 2024-02-02 03:41:43.000000 libesedb-20240202/libcthreads/libcthreads_thread.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3195 2024-02-02 03:41:43.000000 libesedb-20240202/libcthreads/libcthreads_read_write_lock.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10198 2024-02-02 03:41:43.000000 libesedb-20240202/libcthreads/libcthreads_thread.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4175 2024-02-02 03:41:43.000000 libesedb-20240202/libcthreads/libcthreads_thread_pool.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1254 2024-02-02 03:41:43.000000 libesedb-20240202/libcthreads/libcthreads_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2208 2024-02-02 03:41:43.000000 libesedb-20240202/libcthreads/libcthreads_lock.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-02-02 03:41:43.000000 libesedb-20240202/libcthreads/libcthreads_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8753 2024-02-02 03:41:43.000000 libesedb-20240202/libcthreads/libcthreads_lock.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3040 2024-02-02 03:41:43.000000 libesedb-20240202/libcthreads/libcthreads_condition.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2870 2024-02-02 03:41:43.000000 libesedb-20240202/libcthreads/libcthreads_repeating_thread.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1171 2024-02-02 03:41:43.000000 libesedb-20240202/libcthreads/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1170 2024-02-02 03:41:43.000000 libesedb-20240202/libcthreads/libcthreads_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13601 2024-02-02 03:41:43.000000 libesedb-20240202/libcthreads/libcthreads_mutex.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26519 2024-02-02 03:41:43.000000 libesedb-20240202/libcthreads/libcthreads_queue.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2434 2024-02-02 03:41:43.000000 libesedb-20240202/libcthreads/libcthreads_mutex.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2510 2024-02-02 03:41:43.000000 libesedb-20240202/libcthreads/libcthreads_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2138 2024-02-02 03:41:43.000000 libesedb-20240202/libcthreads/libcthreads_thread_attributes.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18281 2024-02-02 03:41:43.000000 libesedb-20240202/libcthreads/libcthreads_condition.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2952 2024-02-02 03:41:43.000000 libesedb-20240202/libcthreads/libcthreads_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18426 2024-02-02 03:41:43.000000 libesedb-20240202/libcthreads/libcthreads_read_write_lock.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1447 2024-02-02 03:41:43.000000 libesedb-20240202/libcthreads/libcthreads_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2128 2024-02-02 03:41:43.000000 libesedb-20240202/libcthreads/libcthreads_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    43321 2024-02-02 03:41:43.000000 libesedb-20240202/libcthreads/libcthreads_thread_pool.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1864 2024-02-02 03:41:43.000000 libesedb-20240202/libcthreads/libcthreads_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4096 2024-02-02 03:41:43.000000 libesedb-20240202/libcthreads/libcthreads_thread_attributes.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1428 2024-02-02 03:41:43.000000 libesedb-20240202/libcthreads/libcthreads_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17481 2024-02-02 03:41:43.000000 libesedb-20240202/libcthreads/libcthreads_repeating_thread.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33793 2024-02-02 03:42:05.000000 libesedb-20240202/libcthreads/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3341 2024-02-02 03:41:43.000000 libesedb-20240202/libcthreads/libcthreads_queue.h
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4879 2024-02-02 03:42:06.000000 libesedb-20240202/test-driver
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-02 04:07:50.000000 libesedb-20240202/libcpath/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2336 2024-02-02 03:41:41.000000 libesedb-20240202/libcpath/libcpath_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-02-02 03:41:41.000000 libesedb-20240202/libcpath/libcpath_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1990 2024-02-02 03:41:41.000000 libesedb-20240202/libcpath/libcpath_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      842 2024-02-02 03:41:41.000000 libesedb-20240202/libcpath/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-02-02 03:41:41.000000 libesedb-20240202/libcpath/libcpath_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-02-02 03:41:41.000000 libesedb-20240202/libcpath/libcpath_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2826 2024-02-02 03:41:41.000000 libesedb-20240202/libcpath/libcpath_system_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1461 2024-02-02 03:41:41.000000 libesedb-20240202/libcpath/libcpath_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1536 2024-02-02 03:41:41.000000 libesedb-20240202/libcpath/libcpath_libcsplit.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25560 2024-02-02 03:41:41.000000 libesedb-20240202/libcpath/libcpath_system_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2024-02-02 03:41:41.000000 libesedb-20240202/libcpath/libcpath_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-02-02 03:41:41.000000 libesedb-20240202/libcpath/libcpath_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30981 2024-02-02 03:42:05.000000 libesedb-20240202/libcpath/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1736 2024-02-02 03:41:41.000000 libesedb-20240202/libcpath/libcpath_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-02-02 03:41:41.000000 libesedb-20240202/libcpath/libcpath_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   176165 2024-02-02 03:41:41.000000 libesedb-20240202/libcpath/libcpath_path.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7170 2024-02-02 03:41:41.000000 libesedb-20240202/libcpath/libcpath_path.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5278 2023-12-03 09:00:45.000000 libesedb-20240202/ChangeLog
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-02 04:07:51.000000 libesedb-20240202/manuals/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2863 2024-02-02 03:31:36.000000 libesedb-20240202/manuals/esedbinfo.1
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      158 2023-12-03 09:01:09.000000 libesedb-20240202/manuals/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17769 2024-02-02 03:31:36.000000 libesedb-20240202/manuals/libesedb.3
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27906 2024-02-02 03:42:06.000000 libesedb-20240202/manuals/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-02 04:07:51.000000 libesedb-20240202/tests/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2790 2024-02-02 03:32:22.000000 libesedb-20240202/tests/esedb_test_space_tree.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3092 2024-02-02 03:32:22.000000 libesedb-20240202/tests/esedb_test_index.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4169 2024-02-02 03:31:36.000000 libesedb-20240202/tests/esedb_test_tools_signal.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      981 2024-02-02 03:31:36.000000 libesedb-20240202/tests/esedb_test_libesedb.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17731 2024-02-02 03:32:22.000000 libesedb-20240202/tests/esedb_test_data_segment.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1444 2024-02-02 03:31:36.000000 libesedb-20240202/tests/esedb_test_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1742 2024-02-02 03:31:36.000000 libesedb-20240202/tests/esedb_test_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20720 2024-02-02 03:31:36.000000 libesedb-20240202/tests/esedb_test_tools_windows_search_compression.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13259 2024-02-02 03:31:36.000000 libesedb-20240202/tests/esedb_test_functions.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3605 2024-02-02 03:32:22.000000 libesedb-20240202/tests/esedb_test_table.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28708 2024-02-02 03:31:36.000000 libesedb-20240202/tests/esedb_test_compression.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29229 2024-02-02 03:31:36.000000 libesedb-20240202/tests/esedb_test_file.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    36143 2024-02-02 03:32:22.000000 libesedb-20240202/tests/esedb_test_catalog_definition.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3340 2024-02-02 03:32:44.000000 libesedb-20240202/tests/pyesedb_test_support.py
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4095 2024-02-02 03:32:44.000000 libesedb-20240202/tests/test_tools.sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1709 2024-02-02 03:31:36.000000 libesedb-20240202/tests/esedb_test_libbfio.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1462 2024-02-02 03:31:36.000000 libesedb-20240202/tests/esedb_test_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   106858 2024-02-02 03:31:36.000000 libesedb-20240202/tests/esedb_test_checksum.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8399 2024-02-02 03:32:22.000000 libesedb-20240202/tests/esedb_test_table_definition.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3139 2024-02-02 03:31:36.000000 libesedb-20240202/tests/esedb_test_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3980 2024-02-02 03:32:22.000000 libesedb-20240202/tests/esedb_test_multi_value.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5349 2024-02-02 03:31:36.000000 libesedb-20240202/tests/pyesedb_test_file.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9212 2024-02-02 03:31:36.000000 libesedb-20240202/tests/esedb_test_space_tree_value.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14751 2024-02-02 03:32:22.000000 libesedb-20240202/tests/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1702 2024-02-02 03:31:36.000000 libesedb-20240202/tests/esedb_test_memory.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1465 2024-02-02 03:31:36.000000 libesedb-20240202/tests/esedb_test_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4703 2024-02-02 03:32:22.000000 libesedb-20240202/tests/esedb_test_record.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14367 2024-02-02 03:31:36.000000 libesedb-20240202/tests/esedb_test_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4323 2024-02-02 03:31:36.000000 libesedb-20240202/tests/esedb_test_notify.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9728 2024-02-02 03:32:22.000000 libesedb-20240202/tests/esedb_test_leaf_page_descriptor.c
--rwxr--r--   0 lordyesta  (1000) lordyesta  (1000)     1653 2024-02-02 03:31:36.000000 libesedb-20240202/tests/test_manpage.sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5634 2024-02-02 03:31:36.000000 libesedb-20240202/tests/esedb_test_tools_info_handle.c
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4076 2024-02-02 03:31:36.000000 libesedb-20240202/tests/test_python_module.sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23738 2024-02-02 03:32:22.000000 libesedb-20240202/tests/esedb_test_catalog.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1554 2024-02-02 03:31:36.000000 libesedb-20240202/tests/esedb_test_libcdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4700 2024-02-02 03:31:36.000000 libesedb-20240202/tests/esedb_test_memory.c
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4789 2024-02-02 03:31:36.000000 libesedb-20240202/tests/test_esedbexport.sh
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     3320 2024-02-02 03:31:36.000000 libesedb-20240202/tests/test_esedbinfo.sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2447 2024-02-02 03:31:36.000000 libesedb-20240202/tests/esedb_test_tools_output.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3017 2024-02-02 03:32:22.000000 libesedb-20240202/tests/esedb_test_column_type.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6743 2024-02-02 03:32:22.000000 libesedb-20240202/tests/esedb_test_block_tree_node.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33607 2024-02-02 03:31:36.000000 libesedb-20240202/tests/test_runner.sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1545 2024-02-02 03:31:36.000000 libesedb-20240202/tests/esedb_test_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7826 2024-02-02 03:32:22.000000 libesedb-20240202/tests/esedb_test_database.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8181 2024-02-02 03:31:36.000000 libesedb-20240202/tests/esedb_test_io_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19281 2024-02-02 03:32:22.000000 libesedb-20240202/tests/esedb_test_file_header.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9255 2024-02-02 03:31:36.000000 libesedb-20240202/tests/esedb_test_page_tree_value.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4535 2024-02-02 03:31:36.000000 libesedb-20240202/tests/esedb_test_getopt.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1813 2024-02-02 03:31:36.000000 libesedb-20240202/tests/esedb_test_getopt.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1812 2024-02-02 03:31:36.000000 libesedb-20240202/tests/esedb_test_functions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14527 2024-02-02 03:32:22.000000 libesedb-20240202/tests/esedb_test_block_tree.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1447 2024-02-02 03:31:36.000000 libesedb-20240202/tests/esedb_test_libfcache.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1551 2024-02-02 03:31:36.000000 libesedb-20240202/tests/esedb_test_libfdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9553 2024-02-02 03:31:36.000000 libesedb-20240202/tests/esedb_test_data_definition.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    91150 2024-02-02 03:42:06.000000 libesedb-20240202/tests/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9288 2024-02-02 03:31:36.000000 libesedb-20240202/tests/esedb_test_root_page_header.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3378 2024-02-02 03:32:22.000000 libesedb-20240202/tests/esedb_test_long_value.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6011 2024-02-02 03:31:36.000000 libesedb-20240202/tests/esedb_test_page_value.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15037 2024-02-02 03:32:22.000000 libesedb-20240202/tests/esedb_test_page_tree_key.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6476 2024-02-02 03:32:22.000000 libesedb-20240202/tests/esedb_test_block_descriptor.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9078 2024-02-02 03:32:22.000000 libesedb-20240202/tests/esedb_test_page_tree.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    58326 2024-02-02 03:32:22.000000 libesedb-20240202/tests/esedb_test_page.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17919 2024-02-02 03:32:22.000000 libesedb-20240202/tests/esedb_test_page_header.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22535 2024-02-02 03:32:22.000000 libesedb-20240202/tests/esedb_test_column.c
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4429 2024-02-02 03:32:44.000000 libesedb-20240202/tests/test_library.sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8574 2024-02-02 03:31:36.000000 libesedb-20240202/tests/esedb_test_macros.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-02 04:07:51.000000 libesedb-20240202/ossfuzz/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2621 2024-02-02 03:31:35.000000 libesedb-20240202/ossfuzz/table_fuzzer.cc
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      972 2024-02-02 03:31:35.000000 libesedb-20240202/ossfuzz/ossfuzz_libesedb.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2422 2023-12-03 09:00:45.000000 libesedb-20240202/ossfuzz/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3118 2024-02-02 03:31:35.000000 libesedb-20240202/ossfuzz/column_fuzzer.cc
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1739 2024-02-02 03:31:35.000000 libesedb-20240202/ossfuzz/ossfuzz_libbfio.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3095 2024-02-02 03:31:35.000000 libesedb-20240202/ossfuzz/record_fuzzer.cc
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2214 2024-02-02 03:31:35.000000 libesedb-20240202/ossfuzz/file_fuzzer.cc
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    38705 2024-02-02 03:42:06.000000 libesedb-20240202/ossfuzz/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   332808 2024-02-02 03:42:00.000000 libesedb-20240202/ltmain.sh
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-02 04:07:50.000000 libesedb-20240202/libfwnt/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1627 2024-02-02 03:41:52.000000 libesedb-20240202/libfwnt/libfwnt_locale_identifier.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26551 2024-02-02 03:41:52.000000 libesedb-20240202/libfwnt/libfwnt_lzxpress.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1376 2024-02-02 03:41:52.000000 libesedb-20240202/libfwnt/libfwnt_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30230 2024-02-02 03:41:52.000000 libesedb-20240202/libfwnt/libfwnt_security_identifier.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2024-02-02 03:41:52.000000 libesedb-20240202/libfwnt/libfwnt_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7049 2024-02-02 03:41:52.000000 libesedb-20240202/libfwnt/libfwnt_bit_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1772 2024-02-02 03:41:52.000000 libesedb-20240202/libfwnt/libfwnt_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-02-02 03:41:52.000000 libesedb-20240202/libfwnt/libfwnt_lznt1.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2742 2024-02-02 03:41:52.000000 libesedb-20240202/libfwnt/libfwnt_notify.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1348 2024-02-02 03:41:52.000000 libesedb-20240202/libfwnt/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5264 2024-02-02 03:41:52.000000 libesedb-20240202/libfwnt/libfwnt_security_identifier.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1185 2024-02-02 03:41:52.000000 libesedb-20240202/libfwnt/libfwnt_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2072 2024-02-02 03:41:52.000000 libesedb-20240202/libfwnt/libfwnt_huffman_tree.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2896 2024-02-02 03:41:52.000000 libesedb-20240202/libfwnt/libfwnt_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2795 2024-02-02 03:41:52.000000 libesedb-20240202/libfwnt/libfwnt_access_control_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27064 2024-02-02 03:41:52.000000 libesedb-20240202/libfwnt/libfwnt_security_descriptor.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13639 2024-02-02 03:41:52.000000 libesedb-20240202/libfwnt/libfwnt_access_control_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3470 2024-02-02 03:41:52.000000 libesedb-20240202/libfwnt/libfwnt_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13113 2024-02-02 03:41:52.000000 libesedb-20240202/libfwnt/libfwnt_huffman_tree.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8377 2024-02-02 03:41:52.000000 libesedb-20240202/libfwnt/libfwnt_debug.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15166 2024-02-02 03:41:52.000000 libesedb-20240202/libfwnt/libfwnt_lznt1.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1578 2024-02-02 03:41:52.000000 libesedb-20240202/libfwnt/libfwnt_notify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18859 2024-02-02 03:41:52.000000 libesedb-20240202/libfwnt/libfwnt_locale_identifier.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1464 2024-02-02 03:41:52.000000 libesedb-20240202/libfwnt/libfwnt_debug.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1545 2024-02-02 03:41:52.000000 libesedb-20240202/libfwnt/libfwnt_libcdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2797 2024-02-02 03:41:52.000000 libesedb-20240202/libfwnt/libfwnt_lzx.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2024-02-02 03:41:52.000000 libesedb-20240202/libfwnt/libfwnt_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1453 2024-02-02 03:41:52.000000 libesedb-20240202/libfwnt/libfwnt_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19962 2024-02-02 03:41:52.000000 libesedb-20240202/libfwnt/libfwnt_access_control_entry.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2326 2024-02-02 03:41:52.000000 libesedb-20240202/libfwnt/libfwnt_lzxpress.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3336 2024-02-02 03:41:52.000000 libesedb-20240202/libfwnt/libfwnt_security_descriptor.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    36036 2024-02-02 03:41:52.000000 libesedb-20240202/libfwnt/libfwnt_lzx.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34608 2024-02-02 03:42:06.000000 libesedb-20240202/libfwnt/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2039 2024-02-02 03:41:52.000000 libesedb-20240202/libfwnt/libfwnt_bit_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1908 2024-02-02 03:41:52.000000 libesedb-20240202/libfwnt/libfwnt_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1129 2024-02-02 03:41:52.000000 libesedb-20240202/libfwnt/libfwnt_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3209 2024-02-02 03:41:52.000000 libesedb-20240202/libfwnt/libfwnt_access_control_entry.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-02 04:07:50.000000 libesedb-20240202/libcsplit/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6125 2024-02-02 03:41:42.000000 libesedb-20240202/libcsplit/libcsplit_narrow_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1360 2024-02-02 03:41:42.000000 libesedb-20240202/libcsplit/libcsplit_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1679 2024-02-02 03:41:42.000000 libesedb-20240202/libcsplit/libcsplit_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13944 2024-02-02 03:41:42.000000 libesedb-20240202/libcsplit/libcsplit_wide_split_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2024-02-02 03:41:42.000000 libesedb-20240202/libcsplit/libcsplit_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      884 2024-02-02 03:41:42.000000 libesedb-20240202/libcsplit/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-02-02 03:41:42.000000 libesedb-20240202/libcsplit/libcsplit_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6206 2024-02-02 03:41:42.000000 libesedb-20240202/libcsplit/libcsplit_wide_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-02-02 03:41:42.000000 libesedb-20240202/libcsplit/libcsplit_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2920 2024-02-02 03:41:42.000000 libesedb-20240202/libcsplit/libcsplit_wide_split_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2924 2024-02-02 03:41:42.000000 libesedb-20240202/libcsplit/libcsplit_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13912 2024-02-02 03:41:42.000000 libesedb-20240202/libcsplit/libcsplit_narrow_split_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-02-02 03:41:42.000000 libesedb-20240202/libcsplit/libcsplit_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-02-02 03:41:42.000000 libesedb-20240202/libcsplit/libcsplit_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1158 2024-02-02 03:41:42.000000 libesedb-20240202/libcsplit/libcsplit_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1471 2024-02-02 03:41:42.000000 libesedb-20240202/libcsplit/libcsplit_wide_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31761 2024-02-02 03:42:05.000000 libesedb-20240202/libcsplit/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2849 2024-02-02 03:41:42.000000 libesedb-20240202/libcsplit/libcsplit_narrow_split_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1386 2024-02-02 03:41:42.000000 libesedb-20240202/libcsplit/libcsplit_narrow_string.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-02 04:07:51.000000 libesedb-20240202/po/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      720 2023-12-03 09:01:06.000000 libesedb-20240202/po/remove-potcdate.sin
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       59 2023-12-03 09:01:06.000000 libesedb-20240202/po/POTFILES.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19571 2023-12-03 09:01:06.000000 libesedb-20240202/po/Makefile.in.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      153 2023-12-03 09:01:06.000000 libesedb-20240202/po/quot.sed
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1204 2023-12-03 09:01:06.000000 libesedb-20240202/po/en@quot.header
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1338 2023-12-03 09:01:06.000000 libesedb-20240202/po/en@boldquot.header
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      217 2023-12-03 09:01:06.000000 libesedb-20240202/po/boldquot.sed
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      906 2023-12-03 09:01:06.000000 libesedb-20240202/po/insert-header.sin
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       50 2023-12-03 09:01:06.000000 libesedb-20240202/po/ChangeLog
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1854 2024-02-02 03:42:15.000000 libesedb-20240202/po/Makevars
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1852 2023-12-03 09:01:06.000000 libesedb-20240202/po/Makevars.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2395 2023-12-03 09:01:06.000000 libesedb-20240202/po/Rules-quot
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-02 04:07:50.000000 libesedb-20240202/libuna/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8811 2024-02-02 03:41:56.000000 libesedb-20240202/libuna/libuna_codepage_windows_1251.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    98308 2024-02-02 03:41:56.000000 libesedb-20240202/libuna/libuna_utf16_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39461 2024-02-02 03:41:56.000000 libesedb-20240202/libuna/libuna_base16_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2993 2024-02-02 03:41:56.000000 libesedb-20240202/libuna/libuna_utf8_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1567 2024-02-02 03:41:56.000000 libesedb-20240202/libuna/libuna_codepage_iso_8859_2.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   286239 2024-02-02 03:41:56.000000 libesedb-20240202/libuna/libuna_codepage_windows_932.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-02-02 03:41:56.000000 libesedb-20240202/libuna/libuna_codepage_mac_dingbats.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   101450 2024-02-02 03:41:56.000000 libesedb-20240202/libuna/libuna_utf8_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    74767 2024-02-02 03:41:56.000000 libesedb-20240202/libuna/libuna_base64_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1749 2024-02-02 03:41:56.000000 libesedb-20240202/libuna/libuna_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1610 2024-02-02 03:41:56.000000 libesedb-20240202/libuna/libuna_codepage_mac_turkish.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   156918 2024-02-02 03:41:56.000000 libesedb-20240202/libuna/libuna_unicode_character.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10379 2024-02-02 03:41:56.000000 libesedb-20240202/libuna/libuna_codepage_mac_gaelic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-02-02 03:41:56.000000 libesedb-20240202/libuna/libuna_codepage_mac_arabic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9435 2024-02-02 03:41:56.000000 libesedb-20240202/libuna/libuna_codepage_mac_thai.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1618 2024-02-02 03:41:56.000000 libesedb-20240202/libuna/libuna_codepage_windows_874.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1346 2024-02-02 03:41:56.000000 libesedb-20240202/libuna/libuna_codepage_iso_8859_15.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9666 2024-02-02 03:41:56.000000 libesedb-20240202/libuna/libuna_utf8_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3296 2024-02-02 03:41:56.000000 libesedb-20240202/libuna/libuna_codepage_iso_8859_16.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9211 2024-02-02 03:41:56.000000 libesedb-20240202/libuna/libuna_codepage_windows_1255.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15691 2024-02-02 03:41:56.000000 libesedb-20240202/libuna/libuna_utf7_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2921 2024-02-02 03:41:56.000000 libesedb-20240202/libuna/libuna_byte_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9984 2024-02-02 03:41:56.000000 libesedb-20240202/libuna/libuna_codepage_koi8_u.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1392 2024-02-02 03:41:56.000000 libesedb-20240202/libuna/libuna_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2540 2024-02-02 03:41:56.000000 libesedb-20240202/libuna/libuna_codepage_iso_8859_6.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2823 2024-02-02 03:41:56.000000 libesedb-20240202/libuna/libuna_codepage_iso_8859_14.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3679 2024-02-02 03:41:56.000000 libesedb-20240202/libuna/libuna_base64_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2882 2024-02-02 03:41:56.000000 libesedb-20240202/libuna/libuna_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1658 2024-02-02 03:41:56.000000 libesedb-20240202/libuna/libuna_codepage_mac_centraleurroman.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9953 2024-02-02 03:41:56.000000 libesedb-20240202/libuna/libuna_codepage_mac_romanian.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1339 2024-02-02 03:41:56.000000 libesedb-20240202/libuna/libuna_codepage_iso_8859_6.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2053 2024-02-02 03:41:56.000000 libesedb-20240202/libuna/libuna_codepage_iso_8859_9.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1610 2024-02-02 03:41:56.000000 libesedb-20240202/libuna/libuna_codepage_mac_russian.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10134 2024-02-02 03:41:56.000000 libesedb-20240202/libuna/libuna_codepage_mac_dingbats.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2024-02-02 03:41:56.000000 libesedb-20240202/libuna/libuna_codepage_iso_8859_15.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   430461 2024-02-02 03:41:56.000000 libesedb-20240202/libuna/libuna_codepage_windows_936.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-02-02 03:41:56.000000 libesedb-20240202/libuna/libuna_codepage_mac_croatian.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1259 2024-02-02 03:41:56.000000 libesedb-20240202/libuna/libuna_scsu.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4197 2024-02-02 03:41:56.000000 libesedb-20240202/libuna/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20049 2024-02-02 03:41:56.000000 libesedb-20240202/libuna/libuna_utf32_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1830 2024-02-02 03:41:56.000000 libesedb-20240202/libuna/libuna_codepage_windows_936.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3225 2024-02-02 03:41:56.000000 libesedb-20240202/libuna/libuna_codepage_iso_8859_10.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9745 2024-02-02 03:41:56.000000 libesedb-20240202/libuna/libuna_codepage_mac_roman.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2808 2024-02-02 03:41:56.000000 libesedb-20240202/libuna/libuna_utf7_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1773 2024-02-02 03:41:56.000000 libesedb-20240202/libuna/libuna_codepage_iso_8859_3.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1787 2024-02-02 03:41:56.000000 libesedb-20240202/libuna/libuna_codepage_mac_thai.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-02-02 03:41:56.000000 libesedb-20240202/libuna/libuna_codepage_mac_farsi.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9088 2024-02-02 03:41:56.000000 libesedb-20240202/libuna/libuna_codepage_mac_ukrainian.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10880 2024-02-02 03:41:56.000000 libesedb-20240202/libuna/libuna_codepage_mac_inuit.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1830 2024-02-02 03:41:56.000000 libesedb-20240202/libuna/libuna_codepage_windows_932.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8050 2024-02-02 03:41:56.000000 libesedb-20240202/libuna/libuna_codepage_windows_874.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2738 2024-02-02 03:41:56.000000 libesedb-20240202/libuna/libuna_codepage_iso_8859_5.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-02-02 03:41:56.000000 libesedb-20240202/libuna/libuna_codepage_iso_8859_10.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16705 2024-02-02 03:41:56.000000 libesedb-20240202/libuna/libuna_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1929 2024-02-02 03:41:56.000000 libesedb-20240202/libuna/libuna_url_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1622 2024-02-02 03:41:56.000000 libesedb-20240202/libuna/libuna_codepage_mac_icelandic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1602 2024-02-02 03:41:56.000000 libesedb-20240202/libuna/libuna_codepage_koi8_u.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19850 2024-02-02 03:41:56.000000 libesedb-20240202/libuna/libuna_utf16_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8602 2024-02-02 03:41:56.000000 libesedb-20240202/libuna/libuna_codepage_windows_1253.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1449 2024-02-02 03:41:56.000000 libesedb-20240202/libuna/libuna_codepage_iso_8859_4.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9078 2024-02-02 03:41:56.000000 libesedb-20240202/libuna/libuna_codepage_mac_greek.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-02-02 03:41:56.000000 libesedb-20240202/libuna/libuna_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9394 2024-02-02 03:41:56.000000 libesedb-20240202/libuna/libuna_codepage_mac_centraleurroman.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8997 2024-02-02 03:41:56.000000 libesedb-20240202/libuna/libuna_codepage_windows_1254.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1455 2024-02-02 03:41:56.000000 libesedb-20240202/libuna/libuna_codepage_iso_8859_13.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1447 2024-02-02 03:41:56.000000 libesedb-20240202/libuna/libuna_codepage_iso_8859_7.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-02-02 03:41:56.000000 libesedb-20240202/libuna/libuna_codepage_windows_1255.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8000 2024-02-02 03:41:56.000000 libesedb-20240202/libuna/libuna_unicode_character.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1448 2024-02-02 03:41:56.000000 libesedb-20240202/libuna/libuna_codepage_iso_8859_8.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3664 2024-02-02 03:41:56.000000 libesedb-20240202/libuna/libuna_codepage_iso_8859_13.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-02-02 03:41:56.000000 libesedb-20240202/libuna/libuna_codepage_windows_949.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9125 2024-02-02 03:41:56.000000 libesedb-20240202/libuna/libuna_codepage_mac_cyrillic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9871 2024-02-02 03:41:56.000000 libesedb-20240202/libuna/libuna_codepage_mac_celtic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1234 2024-02-02 03:41:56.000000 libesedb-20240202/libuna/libuna_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3561 2024-02-02 03:41:56.000000 libesedb-20240202/libuna/libuna_codepage_iso_8859_4.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   484762 2024-02-02 03:41:56.000000 libesedb-20240202/libuna/libuna_codepage_windows_949.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3106 2024-02-02 03:41:56.000000 libesedb-20240202/libuna/libuna_utf16_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14020 2024-02-02 03:41:56.000000 libesedb-20240202/libuna/libuna_codepage_mac_symbol.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-02-02 03:41:56.000000 libesedb-20240202/libuna/libuna_codepage_mac_roman.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9076 2024-02-02 03:41:56.000000 libesedb-20240202/libuna/libuna_codepage_windows_1257.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1627 2024-02-02 03:41:56.000000 libesedb-20240202/libuna/libuna_codepage_windows_1254.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   360710 2024-02-02 03:41:56.000000 libesedb-20240202/libuna/libuna_codepage_windows_950.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1363 2024-02-02 03:41:56.000000 libesedb-20240202/libuna/libuna_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10005 2024-02-02 03:41:56.000000 libesedb-20240202/libuna/libuna_codepage_windows_1256.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1521 2024-02-02 03:41:56.000000 libesedb-20240202/libuna/libuna_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3704 2024-02-02 03:41:56.000000 libesedb-20240202/libuna/libuna_base32_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1625 2024-02-02 03:41:56.000000 libesedb-20240202/libuna/libuna_codepage_windows_1253.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1783 2024-02-02 03:41:56.000000 libesedb-20240202/libuna/libuna_codepage_iso_8859_16.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18019 2024-02-02 03:41:56.000000 libesedb-20240202/libuna/libuna_utf8_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1636 2024-02-02 03:41:56.000000 libesedb-20240202/libuna/libuna_codepage_windows_1250.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3610 2024-02-02 03:41:56.000000 libesedb-20240202/libuna/libuna_codepage_iso_8859_2.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1140 2024-02-02 03:41:56.000000 libesedb-20240202/libuna/libuna_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9542 2024-02-02 03:41:56.000000 libesedb-20240202/libuna/libuna_codepage_koi8_r.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1341 2024-02-02 03:41:56.000000 libesedb-20240202/libuna/libuna_codepage_iso_8859_5.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9656 2024-02-02 03:41:56.000000 libesedb-20240202/libuna/libuna_utf16_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    94606 2024-02-02 03:41:56.000000 libesedb-20240202/libuna/libuna_utf32_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9656 2024-02-02 03:41:56.000000 libesedb-20240202/libuna/libuna_codepage_mac_icelandic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-02-02 03:41:56.000000 libesedb-20240202/libuna/libuna_codepage_windows_1256.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9526 2024-02-02 03:41:56.000000 libesedb-20240202/libuna/libuna_utf32_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-02-02 03:41:56.000000 libesedb-20240202/libuna/libuna_codepage_mac_romanian.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2629 2024-02-02 03:41:56.000000 libesedb-20240202/libuna/libuna_codepage_iso_8859_8.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1600 2024-02-02 03:41:56.000000 libesedb-20240202/libuna/libuna_codepage_koi8_r.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-02-02 03:41:56.000000 libesedb-20240202/libuna/libuna_codepage_mac_cyrillic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10389 2024-02-02 03:41:56.000000 libesedb-20240202/libuna/libuna_codepage_mac_arabic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9776 2024-02-02 03:41:56.000000 libesedb-20240202/libuna/libuna_codepage_mac_croatian.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1340 2024-02-02 03:41:56.000000 libesedb-20240202/libuna/libuna_codepage_iso_8859_9.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-02-02 03:41:56.000000 libesedb-20240202/libuna/libuna_codepage_mac_greek.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1630 2024-02-02 03:41:56.000000 libesedb-20240202/libuna/libuna_codepage_windows_1258.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2873 2024-02-02 03:41:56.000000 libesedb-20240202/libuna/libuna_codepage_iso_8859_7.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    54505 2024-02-02 03:42:06.000000 libesedb-20240202/libuna/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3335 2024-02-02 03:41:56.000000 libesedb-20240202/libuna/libuna_codepage_iso_8859_3.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9776 2024-02-02 03:41:56.000000 libesedb-20240202/libuna/libuna_codepage_windows_1250.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3181 2024-02-02 03:41:56.000000 libesedb-20240202/libuna/libuna_scsu.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7189 2024-02-02 03:41:56.000000 libesedb-20240202/libuna/libuna_codepage_windows_1252.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9844 2024-02-02 03:41:56.000000 libesedb-20240202/libuna/libuna_codepage_mac_turkish.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1622 2024-02-02 03:41:56.000000 libesedb-20240202/libuna/libuna_codepage_mac_ukrainian.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8997 2024-02-02 03:41:56.000000 libesedb-20240202/libuna/libuna_codepage_mac_russian.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9116 2024-02-02 03:41:56.000000 libesedb-20240202/libuna/libuna_codepage_windows_1258.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-02-02 03:41:56.000000 libesedb-20240202/libuna/libuna_codepage_mac_celtic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15485 2024-02-02 03:41:56.000000 libesedb-20240202/libuna/libuna_byte_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-02-02 03:41:56.000000 libesedb-20240202/libuna/libuna_codepage_mac_gaelic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3106 2024-02-02 03:41:56.000000 libesedb-20240202/libuna/libuna_utf32_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1801 2024-02-02 03:41:56.000000 libesedb-20240202/libuna/libuna_codepage_mac_symbol.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-02-02 03:41:56.000000 libesedb-20240202/libuna/libuna_codepage_windows_1257.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-02-02 03:41:56.000000 libesedb-20240202/libuna/libuna_codepage_mac_inuit.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11002 2024-02-02 03:41:56.000000 libesedb-20240202/libuna/libuna_codepage_mac_farsi.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2024-02-02 03:41:56.000000 libesedb-20240202/libuna/libuna_codepage_windows_950.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15532 2024-02-02 03:41:56.000000 libesedb-20240202/libuna/libuna_url_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1628 2024-02-02 03:41:56.000000 libesedb-20240202/libuna/libuna_codepage_windows_1251.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1644 2024-02-02 03:41:56.000000 libesedb-20240202/libuna/libuna_codepage_windows_1252.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1563 2024-02-02 03:41:56.000000 libesedb-20240202/libuna/libuna_codepage_iso_8859_14.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2623 2024-02-02 03:41:56.000000 libesedb-20240202/libuna/libuna_base16_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    82226 2024-02-02 03:41:56.000000 libesedb-20240202/libuna/libuna_base32_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    42154 2024-02-02 03:42:05.000000 libesedb-20240202/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-02 04:07:50.000000 libesedb-20240202/libfvalue/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2913 2024-02-02 03:41:50.000000 libesedb-20240202/libfvalue/libfvalue_filetime.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6390 2024-02-02 03:41:50.000000 libesedb-20240202/libfvalue/libfvalue_utf16_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1707 2024-02-02 03:41:50.000000 libesedb-20240202/libfvalue/libfvalue_libfwnt.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   125143 2024-02-02 03:41:50.000000 libesedb-20240202/libfvalue/libfvalue_value.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20255 2024-02-02 03:41:50.000000 libesedb-20240202/libfvalue/libfvalue_value.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10693 2024-02-02 03:41:50.000000 libesedb-20240202/libfvalue/libfvalue_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3267 2024-02-02 03:41:50.000000 libesedb-20240202/libfvalue/libfvalue_codepage.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14234 2024-02-02 03:41:50.000000 libesedb-20240202/libfvalue/libfvalue_split_utf16_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2924 2024-02-02 03:41:50.000000 libesedb-20240202/libfvalue/libfvalue_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6349 2024-02-02 03:41:50.000000 libesedb-20240202/libfvalue/libfvalue_utf8_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-02-02 03:41:50.000000 libesedb-20240202/libfvalue/libfvalue_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3075 2024-02-02 03:41:50.000000 libesedb-20240202/libfvalue/libfvalue_split_utf16_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1629 2024-02-02 03:41:50.000000 libesedb-20240202/libfvalue/libfvalue_filetime.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1139 2024-02-02 03:41:50.000000 libesedb-20240202/libfvalue/libfvalue_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-02-02 03:41:50.000000 libesedb-20240202/libfvalue/libfvalue_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1706 2024-02-02 03:41:50.000000 libesedb-20240202/libfvalue/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2831 2024-02-02 03:41:50.000000 libesedb-20240202/libfvalue/libfvalue_value_type.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-02-02 03:41:50.000000 libesedb-20240202/libfvalue/libfvalue_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13854 2024-02-02 03:41:50.000000 libesedb-20240202/libfvalue/libfvalue_split_utf8_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5127 2024-02-02 03:41:50.000000 libesedb-20240202/libfvalue/libfvalue_data_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1379 2024-02-02 03:41:50.000000 libesedb-20240202/libfvalue/libfvalue_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    40414 2024-02-02 03:41:50.000000 libesedb-20240202/libfvalue/libfvalue_data_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    70736 2024-02-02 03:41:50.000000 libesedb-20240202/libfvalue/libfvalue_integer.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39827 2024-02-02 03:41:50.000000 libesedb-20240202/libfvalue/libfvalue_value_type.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7448 2024-02-02 03:41:50.000000 libesedb-20240202/libfvalue/libfvalue_integer.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3264 2024-02-02 03:41:50.000000 libesedb-20240202/libfvalue/libfvalue_binary_data.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1665 2024-02-02 03:41:50.000000 libesedb-20240202/libfvalue/libfvalue_value_entry.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1427 2024-02-02 03:41:50.000000 libesedb-20240202/libfvalue/libfvalue_utf16_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-02-02 03:41:50.000000 libesedb-20240202/libfvalue/libfvalue_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3515 2024-02-02 03:41:50.000000 libesedb-20240202/libfvalue/libfvalue_table.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1495 2024-02-02 03:41:50.000000 libesedb-20240202/libfvalue/libfvalue_libfguid.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3040 2024-02-02 03:41:50.000000 libesedb-20240202/libfvalue/libfvalue_split_utf8_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7626 2024-02-02 03:41:50.000000 libesedb-20240202/libfvalue/libfvalue_floating_point.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2024-02-02 03:41:50.000000 libesedb-20240202/libfvalue/libfvalue_libfdatetime.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4451 2024-02-02 03:41:50.000000 libesedb-20240202/libfvalue/libfvalue_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39905 2024-02-02 03:41:50.000000 libesedb-20240202/libfvalue/libfvalue_binary_data.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4662 2024-02-02 03:41:50.000000 libesedb-20240202/libfvalue/libfvalue_value_entry.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1551 2024-02-02 03:41:50.000000 libesedb-20240202/libfvalue/libfvalue_libcdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1199 2024-02-02 03:41:50.000000 libesedb-20240202/libfvalue/libfvalue_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32203 2024-02-02 03:41:50.000000 libesedb-20240202/libfvalue/libfvalue_table.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    36267 2024-02-02 03:42:06.000000 libesedb-20240202/libfvalue/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1417 2024-02-02 03:41:50.000000 libesedb-20240202/libfvalue/libfvalue_utf8_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    84529 2024-02-02 03:41:50.000000 libesedb-20240202/libfvalue/libfvalue_floating_point.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1964 2024-02-02 03:41:50.000000 libesedb-20240202/libfvalue/libfvalue_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    73330 2024-02-02 03:41:50.000000 libesedb-20240202/libfvalue/libfvalue_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1739 2024-02-02 03:41:50.000000 libesedb-20240202/libfvalue/libfvalue_libuna.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-02 04:07:50.000000 libesedb-20240202/libcnotify/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1548 2024-02-02 03:41:40.000000 libesedb-20240202/libcnotify/libcnotify_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1415 2024-02-02 03:41:40.000000 libesedb-20240202/libcnotify/libcnotify_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1164 2024-02-02 03:41:40.000000 libesedb-20240202/libcnotify/libcnotify_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1439 2024-02-02 03:41:40.000000 libesedb-20240202/libcnotify/libcnotify_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      728 2024-02-02 03:41:40.000000 libesedb-20240202/libcnotify/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2024-02-02 03:41:40.000000 libesedb-20240202/libcnotify/libcnotify_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1290 2024-02-02 03:41:40.000000 libesedb-20240202/libcnotify/libcnotify_verbose.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1722 2024-02-02 03:41:40.000000 libesedb-20240202/libcnotify/libcnotify_print.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4018 2024-02-02 03:41:40.000000 libesedb-20240202/libcnotify/libcnotify_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1266 2024-02-02 03:41:40.000000 libesedb-20240202/libcnotify/libcnotify_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1094 2024-02-02 03:41:40.000000 libesedb-20240202/libcnotify/libcnotify_verbose.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30815 2024-02-02 03:42:05.000000 libesedb-20240202/libcnotify/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1365 2024-02-02 03:41:40.000000 libesedb-20240202/libcnotify/libcnotify_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8166 2024-02-02 03:41:40.000000 libesedb-20240202/libcnotify/libcnotify_print.c
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-02 04:07:50.000000 libesedb-20240202/libcerror/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15420 2024-02-02 03:41:36.000000 libesedb-20240202/libcerror/libcerror_system.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19408 2024-02-02 03:41:36.000000 libesedb-20240202/libcerror/libcerror_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-02-02 03:41:36.000000 libesedb-20240202/libcerror/libcerror_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      640 2024-02-02 03:41:36.000000 libesedb-20240202/libcerror/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1522 2024-02-02 03:41:36.000000 libesedb-20240202/libcerror/libcerror_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2024-02-02 03:41:36.000000 libesedb-20240202/libcerror/libcerror_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2880 2024-02-02 03:41:36.000000 libesedb-20240202/libcerror/libcerror_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2026 2024-02-02 03:41:36.000000 libesedb-20240202/libcerror/libcerror_system.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7629 2024-02-02 03:41:36.000000 libesedb-20240202/libcerror/libcerror_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1158 2024-02-02 03:41:36.000000 libesedb-20240202/libcerror/libcerror_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-02-02 03:41:36.000000 libesedb-20240202/libcerror/libcerror_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30328 2024-02-02 03:42:05.000000 libesedb-20240202/libcerror/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3662 2024-02-02 03:31:33.000000 libesedb-20240202/libesedb.spec.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-02 04:07:50.000000 libesedb-20240202/libfdatetime/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5406 2024-02-02 03:41:47.000000 libesedb-20240202/libfdatetime/libfdatetime_floatingtime.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34352 2024-02-02 03:41:47.000000 libesedb-20240202/libfdatetime/libfdatetime_nsf_timedate.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1887 2024-02-02 03:41:47.000000 libesedb-20240202/libfdatetime/libfdatetime_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33399 2024-02-02 03:41:47.000000 libesedb-20240202/libfdatetime/libfdatetime_floatingtime.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1220 2024-02-02 03:41:47.000000 libesedb-20240202/libfdatetime/libfdatetime_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5010 2024-02-02 03:41:47.000000 libesedb-20240202/libfdatetime/libfdatetime_hfs_time.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4182 2024-02-02 03:41:47.000000 libesedb-20240202/libfdatetime/libfdatetime_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31774 2024-02-02 03:41:47.000000 libesedb-20240202/libfdatetime/libfdatetime_hfs_time.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1148 2024-02-02 03:41:47.000000 libesedb-20240202/libfdatetime/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35109 2024-02-02 03:41:47.000000 libesedb-20240202/libfdatetime/libfdatetime_filetime.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4993 2024-02-02 03:41:47.000000 libesedb-20240202/libfdatetime/libfdatetime_systemtime.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-02-02 03:41:47.000000 libesedb-20240202/libfdatetime/libfdatetime_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    50166 2024-02-02 03:41:47.000000 libesedb-20240202/libfdatetime/libfdatetime_posix_time.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1440 2024-02-02 03:41:47.000000 libesedb-20240202/libfdatetime/libfdatetime_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5342 2024-02-02 03:41:47.000000 libesedb-20240202/libfdatetime/libfdatetime_fat_date_time.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    41822 2024-02-02 03:41:47.000000 libesedb-20240202/libfdatetime/libfdatetime_systemtime.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5761 2024-02-02 03:41:47.000000 libesedb-20240202/libfdatetime/libfdatetime_nsf_timedate.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1450 2024-02-02 03:41:47.000000 libesedb-20240202/libfdatetime/libfdatetime_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1154 2024-02-02 03:41:47.000000 libesedb-20240202/libfdatetime/libfdatetime_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2966 2024-02-02 03:41:47.000000 libesedb-20240202/libfdatetime/libfdatetime_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5771 2024-02-02 03:41:47.000000 libesedb-20240202/libfdatetime/libfdatetime_posix_time.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3131 2024-02-02 03:41:47.000000 libesedb-20240202/libfdatetime/libfdatetime_date_time_values.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5340 2024-02-02 03:41:47.000000 libesedb-20240202/libfdatetime/libfdatetime_filetime.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    53085 2024-02-02 03:41:47.000000 libesedb-20240202/libfdatetime/libfdatetime_date_time_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2468 2024-02-02 03:41:47.000000 libesedb-20240202/libfdatetime/libfdatetime_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33554 2024-02-02 03:42:06.000000 libesedb-20240202/libfdatetime/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31754 2024-02-02 03:41:47.000000 libesedb-20240202/libfdatetime/libfdatetime_fat_date_time.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    56915 2024-02-02 03:42:02.000000 libesedb-20240202/aclocal.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8475 2024-02-02 03:31:33.000000 libesedb-20240202/configure.ac
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      418 2024-02-02 04:07:52.571676 libesedb-20240202/PKG-INFO
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-20 14:34:04.000000 libesedb-20240420/
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-20 14:34:02.000000 libesedb-20240420/libfdata/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-04-20 14:09:33.000000 libesedb-20240420/libfdata/libfdata_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37893 2024-04-20 14:09:33.000000 libesedb-20240420/libfdata/libfdata_area.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9700 2024-04-20 14:09:33.000000 libesedb-20240420/libfdata/libfdata_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1491 2024-04-20 14:09:33.000000 libesedb-20240420/libfdata/libfdata_cache.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30931 2024-04-20 14:09:33.000000 libesedb-20240420/libfdata/libfdata_range_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6826 2024-04-20 14:09:33.000000 libesedb-20240420/libfdata/libfdata_mapped_range.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-04-20 14:09:33.000000 libesedb-20240420/libfdata/libfdata_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6533 2024-04-20 14:09:33.000000 libesedb-20240420/libfdata/libfdata_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   107689 2024-04-20 14:09:33.000000 libesedb-20240420/libfdata/libfdata_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1548 2024-04-20 14:09:33.000000 libesedb-20240420/libfdata/libfdata_libcdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12090 2024-04-20 14:09:33.000000 libesedb-20240420/libfdata/libfdata_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4017 2024-04-20 14:09:33.000000 libesedb-20240420/libfdata/libfdata_list_element.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1287 2024-04-20 14:09:33.000000 libesedb-20240420/libfdata/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-04-20 14:09:33.000000 libesedb-20240420/libfdata/libfdata_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-04-20 14:09:33.000000 libesedb-20240420/libfdata/libfdata_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2754 2024-04-20 14:09:33.000000 libesedb-20240420/libfdata/libfdata_notify.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1658 2024-04-20 14:09:33.000000 libesedb-20240420/libfdata/libfdata_cache.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    66203 2024-04-20 14:09:33.000000 libesedb-20240420/libfdata/libfdata_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-04-20 14:09:33.000000 libesedb-20240420/libfdata/libfdata_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2092 2024-04-20 14:09:33.000000 libesedb-20240420/libfdata/libfdata_range.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7327 2024-04-20 14:09:33.000000 libesedb-20240420/libfdata/libfdata_area.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-04-20 14:09:33.000000 libesedb-20240420/libfdata/libfdata_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1230 2024-04-20 14:09:33.000000 libesedb-20240420/libfdata/libfdata_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7149 2024-04-20 14:09:33.000000 libesedb-20240420/libfdata/libfdata_range.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1995 2024-04-20 14:09:33.000000 libesedb-20240420/libfdata/libfdata_mapped_range.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1172 2024-04-20 14:09:33.000000 libesedb-20240420/libfdata/libfdata_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19329 2024-04-20 14:09:33.000000 libesedb-20240420/libfdata/libfdata_list_element.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21271 2024-04-20 14:09:33.000000 libesedb-20240420/libfdata/libfdata_segments_array.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2054 2024-04-20 14:09:33.000000 libesedb-20240420/libfdata/libfdata_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1593 2024-04-20 14:09:33.000000 libesedb-20240420/libfdata/libfdata_notify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6013 2024-04-20 14:09:33.000000 libesedb-20240420/libfdata/libfdata_range_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2804 2024-04-20 14:09:33.000000 libesedb-20240420/libfdata/libfdata_segments_array.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34732 2024-04-20 14:09:57.000000 libesedb-20240420/libfdata/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    49670 2024-04-20 14:09:33.000000 libesedb-20240420/libfdata/libfdata_vector.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-04-20 14:09:33.000000 libesedb-20240420/libfdata/libfdata_libfcache.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7810 2024-04-20 14:09:33.000000 libesedb-20240420/libfdata/libfdata_vector.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35149 2024-04-20 12:01:39.000000 libesedb-20240420/COPYING
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    15358 2024-04-20 14:09:57.000000 libesedb-20240420/install-sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-20 12:01:39.000000 libesedb-20240420/NEWS
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    23568 2024-04-20 14:09:58.000000 libesedb-20240420/depcomp
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-20 14:34:02.000000 libesedb-20240420/libfguid/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-04-20 14:09:36.000000 libesedb-20240420/libfguid/libfguid_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1192 2024-04-20 14:09:36.000000 libesedb-20240420/libfguid/libfguid_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5688 2024-04-20 14:09:36.000000 libesedb-20240420/libfguid/libfguid_identifier.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-04-20 14:09:36.000000 libesedb-20240420/libfguid/libfguid_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      677 2024-04-20 14:09:36.000000 libesedb-20240420/libfguid/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-04-20 14:09:36.000000 libesedb-20240420/libfguid/libfguid_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-04-20 14:09:36.000000 libesedb-20240420/libfguid/libfguid_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1515 2024-04-20 14:09:36.000000 libesedb-20240420/libfguid/libfguid_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    67571 2024-04-20 14:09:36.000000 libesedb-20240420/libfguid/libfguid_identifier.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1134 2024-04-20 14:09:36.000000 libesedb-20240420/libfguid/libfguid_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2341 2024-04-20 14:09:36.000000 libesedb-20240420/libfguid/libfguid_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30533 2024-04-20 14:09:57.000000 libesedb-20240420/libfguid/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-04-20 14:09:36.000000 libesedb-20240420/libfguid/libfguid_error.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-20 14:34:00.000000 libesedb-20240420/m4/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9040 2024-04-20 12:01:48.000000 libesedb-20240420/m4/libfwnt.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11734 2024-04-20 12:01:48.000000 libesedb-20240420/m4/libcfile.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18489 2024-04-20 12:01:48.000000 libesedb-20240420/m4/libfdatetime.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      756 2023-12-03 09:01:06.000000 libesedb-20240420/m4/tests.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9615 2024-04-20 12:01:48.000000 libesedb-20240420/m4/libcpath.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11944 2023-12-03 09:01:06.000000 libesedb-20240420/m4/lib-prefix.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3090 2023-12-03 09:01:06.000000 libesedb-20240420/m4/progtest.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31495 2024-04-20 12:01:48.000000 libesedb-20240420/m4/libuna.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14488 2023-12-03 09:01:06.000000 libesedb-20240420/m4/gettext.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5370 2023-12-03 09:01:06.000000 libesedb-20240420/m4/lib-ld.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8476 2024-04-20 12:01:48.000000 libesedb-20240420/m4/libclocale.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17383 2024-04-20 12:01:48.000000 libesedb-20240420/m4/libcdata.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7625 2024-04-20 12:01:48.000000 libesedb-20240420/m4/libcsplit.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14127 2024-04-20 12:01:48.000000 libesedb-20240420/m4/common.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11362 2024-04-20 12:01:48.000000 libesedb-20240420/m4/libcthreads.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4311 2024-04-20 12:01:48.000000 libesedb-20240420/m4/libmapidb.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      714 2024-04-20 14:09:50.000000 libesedb-20240420/m4/ltversion.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4395 2024-04-20 14:09:50.000000 libesedb-20240420/m4/ltsugar.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15781 2024-04-20 12:01:48.000000 libesedb-20240420/m4/libfdata.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22432 2023-12-03 09:01:06.000000 libesedb-20240420/m4/host-cpu-c-abi.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   307188 2024-04-20 14:09:49.000000 libesedb-20240420/m4/libtool.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18831 2023-12-03 09:01:06.000000 libesedb-20240420/m4/po.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6501 2024-04-20 12:01:48.000000 libesedb-20240420/m4/libcerror.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5886 2024-04-20 12:01:48.000000 libesedb-20240420/m4/libcnotify.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5876 2024-04-20 12:01:48.000000 libesedb-20240420/m4/libfguid.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11923 2024-04-20 12:01:48.000000 libesedb-20240420/m4/libbfio.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9177 2024-04-20 12:01:48.000000 libesedb-20240420/m4/libfmapi.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3229 2023-12-03 09:01:06.000000 libesedb-20240420/m4/intlmacosx.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6151 2024-04-20 14:09:50.000000 libesedb-20240420/m4/lt~obsolete.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34802 2023-12-03 09:01:06.000000 libesedb-20240420/m4/lib-link.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9731 2023-12-03 09:01:06.000000 libesedb-20240420/m4/iconv.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14525 2024-04-20 14:09:50.000000 libesedb-20240420/m4/ltoptions.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1234 2023-12-03 09:01:06.000000 libesedb-20240420/m4/nls.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6476 2024-04-20 12:01:48.000000 libesedb-20240420/m4/python.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20032 2024-04-20 12:01:48.000000 libesedb-20240420/m4/libfvalue.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2058 2023-12-03 09:01:06.000000 libesedb-20240420/m4/types.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7566 2024-04-20 12:01:48.000000 libesedb-20240420/m4/libfcache.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5093 2024-04-20 12:01:48.000000 libesedb-20240420/m4/pthread.m4
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-20 14:34:00.000000 libesedb-20240420/include/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      425 2024-04-20 12:11:46.000000 libesedb-20240420/include/Makefile.am
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-20 14:34:00.000000 libesedb-20240420/include/libesedb/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2981 2024-04-20 12:01:43.000000 libesedb-20240420/include/libesedb/definitions.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2979 2024-04-20 14:10:10.000000 libesedb-20240420/include/libesedb/definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5165 2024-04-20 12:01:43.000000 libesedb-20240420/include/libesedb/types.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5034 2024-04-20 14:10:10.000000 libesedb-20240420/include/libesedb/types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1551 2024-04-20 12:01:43.000000 libesedb-20240420/include/libesedb/features.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6758 2024-04-20 12:01:43.000000 libesedb-20240420/include/libesedb/error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2024-04-20 12:01:43.000000 libesedb-20240420/include/libesedb/extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1487 2024-04-20 14:10:10.000000 libesedb-20240420/include/libesedb/features.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5306 2024-04-20 12:01:43.000000 libesedb-20240420/include/libesedb/codepage.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39086 2024-04-20 14:10:10.000000 libesedb-20240420/include/libesedb.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28909 2024-04-20 14:09:57.000000 libesedb-20240420/include/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39086 2024-04-20 12:01:43.000000 libesedb-20240420/include/libesedb.h.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-20 14:34:00.000000 libesedb-20240420/common/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      957 2024-04-20 12:01:43.000000 libesedb-20240420/common/config_borlandc.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3878 2024-04-20 12:01:43.000000 libesedb-20240420/common/file_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3259 2024-04-20 12:01:43.000000 libesedb-20240420/common/memory.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10437 2024-04-20 12:01:43.000000 libesedb-20240420/common/byte_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1250 2024-04-20 12:01:43.000000 libesedb-20240420/common/common.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2382 2024-04-20 12:01:43.000000 libesedb-20240420/common/config_winapi.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4611 2024-04-20 12:01:43.000000 libesedb-20240420/common/system_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      343 2024-04-20 12:11:46.000000 libesedb-20240420/common/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7375 2024-04-20 12:01:43.000000 libesedb-20240420/common/types.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7374 2024-04-20 14:10:10.000000 libesedb-20240420/common/types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16997 2024-04-20 14:09:56.000000 libesedb-20240420/common/config.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18006 2024-04-20 14:10:10.000000 libesedb-20240420/common/config.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5064 2024-04-20 12:01:43.000000 libesedb-20240420/common/wide_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5419 2024-04-20 12:01:43.000000 libesedb-20240420/common/narrow_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1157 2024-04-20 12:01:43.000000 libesedb-20240420/common/config_msc.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25943 2024-04-20 14:09:57.000000 libesedb-20240420/common/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-20 14:34:01.000000 libesedb-20240420/libclocale/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1969 2024-04-20 14:09:26.000000 libesedb-20240420/libclocale/libclocale_wide_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1412 2024-04-20 14:09:26.000000 libesedb-20240420/libclocale/libclocale_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      775 2024-04-20 14:09:26.000000 libesedb-20240420/libclocale/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3412 2024-04-20 14:09:26.000000 libesedb-20240420/libclocale/libclocale_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2024-04-20 14:09:26.000000 libesedb-20240420/libclocale/libclocale_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1365 2024-04-20 14:09:26.000000 libesedb-20240420/libclocale/libclocale_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1717 2024-04-20 14:09:26.000000 libesedb-20240420/libclocale/libclocale_locale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3142 2024-04-20 14:09:26.000000 libesedb-20240420/libclocale/libclocale_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21033 2024-04-20 14:09:26.000000 libesedb-20240420/libclocale/libclocale_codepage.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10671 2024-04-20 14:09:26.000000 libesedb-20240420/libclocale/libclocale_locale.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31141 2024-04-20 14:09:57.000000 libesedb-20240420/libclocale/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1415 2024-04-20 14:09:26.000000 libesedb-20240420/libclocale/libclocale_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1696 2024-04-20 14:09:26.000000 libesedb-20240420/libclocale/libclocale_wide_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1961 2024-04-20 14:09:26.000000 libesedb-20240420/libclocale/libclocale_codepage.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-20 14:34:02.000000 libesedb-20240420/libfcache/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1551 2024-04-20 14:09:32.000000 libesedb-20240420/libfcache/libfcache_libcdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1619 2024-04-20 14:09:32.000000 libesedb-20240420/libfcache/libfcache_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12461 2024-04-20 14:09:32.000000 libesedb-20240420/libfcache/libfcache_cache_value.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-04-20 14:09:32.000000 libesedb-20240420/libfcache/libfcache_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      876 2024-04-20 14:09:32.000000 libesedb-20240420/libfcache/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2024-04-20 14:09:32.000000 libesedb-20240420/libfcache/libfcache_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-04-20 14:09:32.000000 libesedb-20240420/libfcache/libfcache_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1178 2024-04-20 14:09:32.000000 libesedb-20240420/libfcache/libfcache_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3806 2024-04-20 14:09:32.000000 libesedb-20240420/libfcache/libfcache_cache.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2924 2024-04-20 14:09:32.000000 libesedb-20240420/libfcache/libfcache_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-04-20 14:09:32.000000 libesedb-20240420/libfcache/libfcache_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2259 2024-04-20 14:09:32.000000 libesedb-20240420/libfcache/libfcache_date_time.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-04-20 14:09:32.000000 libesedb-20240420/libfcache/libfcache_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3161 2024-04-20 14:09:32.000000 libesedb-20240420/libfcache/libfcache_cache_value.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31650 2024-04-20 14:09:57.000000 libesedb-20240420/libfcache/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1250 2024-04-20 14:09:32.000000 libesedb-20240420/libfcache/libfcache_date_time.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1680 2024-04-20 14:09:32.000000 libesedb-20240420/libfcache/libfcache_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26186 2024-04-20 14:09:32.000000 libesedb-20240420/libfcache/libfcache_cache.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2254 2024-04-20 12:12:31.000000 libesedb-20240420/Makefile.am
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-20 14:34:02.000000 libesedb-20240420/libbfio/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2630 2024-04-20 14:09:21.000000 libesedb-20240420/libbfio/libbfio_file_range.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27543 2024-04-20 14:09:21.000000 libesedb-20240420/libbfio/libbfio_file_range_io_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2324 2024-04-20 14:09:21.000000 libesedb-20240420/libbfio/libbfio_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1362 2024-04-20 14:09:21.000000 libesedb-20240420/libbfio/libbfio_libcpath.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1772 2024-04-20 14:09:21.000000 libesedb-20240420/libbfio/libbfio_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-04-20 14:09:21.000000 libesedb-20240420/libbfio/libbfio_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2896 2024-04-20 14:09:21.000000 libesedb-20240420/libbfio/libbfio_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1733 2024-04-20 14:09:21.000000 libesedb-20240420/libbfio/libbfio_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4085 2024-04-20 14:09:21.000000 libesedb-20240420/libbfio/libbfio_file_io_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2077 2024-04-20 14:09:21.000000 libesedb-20240420/libbfio/libbfio_file_pool.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12186 2024-04-20 14:09:21.000000 libesedb-20240420/libbfio/libbfio_file_range.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1572 2024-04-20 14:09:21.000000 libesedb-20240420/libbfio/libbfio_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2024-04-20 14:09:21.000000 libesedb-20240420/libbfio/libbfio_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1545 2024-04-20 14:09:21.000000 libesedb-20240420/libbfio/libbfio_libcdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2234 2024-04-20 14:09:21.000000 libesedb-20240420/libbfio/libbfio_file.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1463 2024-04-20 14:09:21.000000 libesedb-20240420/libbfio/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1420 2024-04-20 14:09:21.000000 libesedb-20240420/libbfio/libbfio_libcfile.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2708 2024-04-20 14:09:21.000000 libesedb-20240420/libbfio/libbfio_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2614 2024-04-20 14:09:21.000000 libesedb-20240420/libbfio/libbfio_codepage.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26845 2024-04-20 14:09:21.000000 libesedb-20240420/libbfio/libbfio_file_io_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1448 2024-04-20 14:09:21.000000 libesedb-20240420/libbfio/libbfio_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-04-20 14:09:21.000000 libesedb-20240420/libbfio/libbfio_memory_range.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10798 2024-04-20 14:09:21.000000 libesedb-20240420/libbfio/libbfio_file_pool.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4806 2024-04-20 14:09:21.000000 libesedb-20240420/libbfio/libbfio_file_range_io_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1918 2024-04-20 14:09:21.000000 libesedb-20240420/libbfio/libbfio_libcthreads.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2814 2024-04-20 14:09:21.000000 libesedb-20240420/libbfio/libbfio_system_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21082 2024-04-20 14:09:21.000000 libesedb-20240420/libbfio/libbfio_memory_range_io_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    64816 2024-04-20 14:09:21.000000 libesedb-20240420/libbfio/libbfio_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10899 2024-04-20 14:09:21.000000 libesedb-20240420/libbfio/libbfio_file.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8883 2024-04-20 14:09:21.000000 libesedb-20240420/libbfio/libbfio_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5821 2024-04-20 14:09:21.000000 libesedb-20240420/libbfio/libbfio_memory_range.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    81879 2024-04-20 14:09:21.000000 libesedb-20240420/libbfio/libbfio_pool.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2024-04-20 14:09:21.000000 libesedb-20240420/libbfio/libbfio_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34993 2024-04-20 14:09:57.000000 libesedb-20240420/libbfio/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25540 2024-04-20 14:09:21.000000 libesedb-20240420/libbfio/libbfio_system_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3835 2024-04-20 14:09:21.000000 libesedb-20240420/libbfio/libbfio_memory_range_io_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1376 2024-04-20 14:09:21.000000 libesedb-20240420/libbfio/libbfio_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6841 2024-04-20 14:09:21.000000 libesedb-20240420/libbfio/libbfio_pool.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       67 2023-12-03 09:00:45.000000 libesedb-20240420/ABOUT-NLS
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    49939 2024-04-20 14:09:57.000000 libesedb-20240420/config.guess
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-20 14:34:00.000000 libesedb-20240420/dpkg/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       18 2024-04-20 12:01:39.000000 libesedb-20240420/dpkg/libesedb-python3.install
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1026 2024-04-20 12:01:48.000000 libesedb-20240420/dpkg/copyright
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       22 2024-04-20 12:01:39.000000 libesedb-20240420/dpkg/libesedb.install
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-20 14:34:00.000000 libesedb-20240420/dpkg/source/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       12 2024-04-20 12:01:39.000000 libesedb-20240420/dpkg/source/format
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2206 2024-04-20 12:01:39.000000 libesedb-20240420/dpkg/control
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      769 2024-04-20 12:01:39.000000 libesedb-20240420/dpkg/rules
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      121 2024-04-20 12:01:39.000000 libesedb-20240420/dpkg/changelog.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      140 2024-04-20 14:10:10.000000 libesedb-20240420/dpkg/changelog
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        3 2024-04-20 12:01:39.000000 libesedb-20240420/dpkg/compat
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       96 2024-04-20 12:01:39.000000 libesedb-20240420/dpkg/libesedb-dev.install
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       27 2024-04-20 12:01:39.000000 libesedb-20240420/dpkg/libesedb-tools.install
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      486 2024-04-20 14:10:10.000000 libesedb-20240420/setup.cfg
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7652 2024-04-20 12:01:39.000000 libesedb-20240420/COPYING.LESSER
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-20 14:34:03.000000 libesedb-20240420/esedbtools/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5875 2024-04-20 12:05:41.000000 libesedb-20240420/esedbtools/esedbinfo.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1545 2024-04-20 12:01:46.000000 libesedb-20240420/esedbtools/esedbtools_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1467 2024-04-20 12:01:46.000000 libesedb-20240420/esedbtools/esedbtools_libcfile.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12269 2024-04-20 12:01:46.000000 libesedb-20240420/esedbtools/webcache.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1504 2024-04-20 12:01:46.000000 libesedb-20240420/esedbtools/esedbtools_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    78508 2024-04-20 12:01:46.000000 libesedb-20240420/esedbtools/windows_search.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1748 2024-04-20 12:01:46.000000 libesedb-20240420/esedbtools/esedbtools_libfwnt.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2724 2024-04-20 12:05:41.000000 libesedb-20240420/esedbtools/info_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1501 2024-04-20 12:01:46.000000 libesedb-20240420/esedbtools/esedbtools_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1443 2024-04-20 12:01:46.000000 libesedb-20240420/esedbtools/esedbtools_libfguid.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1454 2024-04-20 12:01:46.000000 libesedb-20240420/esedbtools/esedbtools_output.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6574 2024-04-20 12:01:46.000000 libesedb-20240420/esedbtools/srumdb.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1742 2024-04-20 12:01:46.000000 libesedb-20240420/esedbtools/esedbtools_libfmapi.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1494 2024-04-20 12:01:46.000000 libesedb-20240420/esedbtools/webcache.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4380 2024-04-20 12:01:46.000000 libesedb-20240420/esedbtools/esedbtools_output.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1213 2024-04-20 12:01:46.000000 libesedb-20240420/esedbtools/esedbtools_i18n.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1951 2024-04-20 12:01:46.000000 libesedb-20240420/esedbtools/windows_security.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6044 2024-04-20 12:01:46.000000 libesedb-20240420/esedbtools/database_types.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17428 2024-04-20 12:01:46.000000 libesedb-20240420/esedbtools/export.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2818 2024-04-20 12:12:42.000000 libesedb-20240420/esedbtools/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7769 2024-04-20 12:01:46.000000 libesedb-20240420/esedbtools/windows_search_compression.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5751 2024-04-20 12:01:46.000000 libesedb-20240420/esedbtools/esedbtools_signal.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1813 2024-04-20 12:01:46.000000 libesedb-20240420/esedbtools/esedbtools_getopt.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30817 2024-04-20 12:05:41.000000 libesedb-20240420/esedbtools/info_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    99282 2024-04-20 12:01:46.000000 libesedb-20240420/esedbtools/export_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1781 2024-04-20 12:01:46.000000 libesedb-20240420/esedbtools/esedbtools_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1554 2024-04-20 12:01:46.000000 libesedb-20240420/esedbtools/esedbtools_libcdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1771 2024-04-20 12:01:46.000000 libesedb-20240420/esedbtools/esedbtools_libfdatetime.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2959 2024-04-20 12:05:41.000000 libesedb-20240420/esedbtools/esedbtools_system_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1748 2024-04-20 12:01:46.000000 libesedb-20240420/esedbtools/esedbtools_libbfio.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5934 2024-04-20 12:01:46.000000 libesedb-20240420/esedbtools/log_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1896 2024-04-20 12:01:46.000000 libesedb-20240420/esedbtools/export.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1761 2024-04-20 12:01:46.000000 libesedb-20240420/esedbtools/esedbtools_signal.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12000 2024-04-20 12:01:46.000000 libesedb-20240420/esedbtools/esedbexport.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1483 2024-04-20 12:01:46.000000 libesedb-20240420/esedbtools/esedbtools_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2985 2024-04-20 12:01:46.000000 libesedb-20240420/esedbtools/windows_search.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6042 2024-04-20 12:01:46.000000 libesedb-20240420/esedbtools/export_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1762 2024-04-20 12:01:46.000000 libesedb-20240420/esedbtools/esedbtools_libfvalue.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      981 2024-04-20 12:01:46.000000 libesedb-20240420/esedbtools/esedbtools_libesedb.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1335 2024-04-20 12:01:46.000000 libesedb-20240420/esedbtools/srumdb.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1409 2024-04-20 12:01:46.000000 libesedb-20240420/esedbtools/esedbtools_libcpath.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37441 2024-04-20 14:09:57.000000 libesedb-20240420/esedbtools/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1674 2024-04-20 12:01:46.000000 libesedb-20240420/esedbtools/log_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3617 2024-04-20 12:01:46.000000 libesedb-20240420/esedbtools/exchange.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1323 2024-04-20 12:05:41.000000 libesedb-20240420/esedbtools/esedbtools_system_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    85170 2024-04-20 12:01:46.000000 libesedb-20240420/esedbtools/exchange.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1597 2024-04-20 12:01:46.000000 libesedb-20240420/esedbtools/windows_search_compression.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23591 2024-04-20 12:01:46.000000 libesedb-20240420/esedbtools/windows_security.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1866 2024-04-20 12:01:46.000000 libesedb-20240420/esedbtools/database_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4535 2024-04-20 12:01:46.000000 libesedb-20240420/esedbtools/esedbtools_getopt.c
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)  2074432 2024-04-20 14:09:55.000000 libesedb-20240420/configure
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     7400 2024-04-20 14:09:57.000000 libesedb-20240420/compile
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     6878 2024-04-20 14:09:57.000000 libesedb-20240420/missing
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-20 14:34:02.000000 libesedb-20240420/libesedb/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1111 2024-04-20 14:10:10.000000 libesedb-20240420/libesedb/libesedb.rc
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7885 2024-04-20 12:01:44.000000 libesedb-20240420/libesedb/libesedb_definitions.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9034 2024-04-20 12:01:44.000000 libesedb-20240420/libesedb/libesedb_data_segment.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7344 2024-04-20 12:01:44.000000 libesedb-20240420/libesedb/esedb_file_header.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1842 2024-04-20 12:01:44.000000 libesedb-20240420/libesedb/libesedb_root_page_header.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-04-20 12:01:44.000000 libesedb-20240420/libesedb/libesedb_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1548 2024-04-20 12:01:44.000000 libesedb-20240420/libesedb/libesedb_libcdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3011 2024-04-20 12:01:44.000000 libesedb-20240420/libesedb/libesedb_column_type.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1553 2024-04-20 12:01:44.000000 libesedb-20240420/libesedb/libesedb_lcid.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-04-20 12:01:44.000000 libesedb-20240420/libesedb/libesedb_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19331 2024-04-20 12:01:44.000000 libesedb-20240420/libesedb/libesedb_file_header.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1709 2024-04-20 12:01:44.000000 libesedb-20240420/libesedb/libesedb_space_tree_value.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2840 2024-04-20 12:01:44.000000 libesedb-20240420/libesedb/libesedb_io_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4546 2024-04-20 12:01:44.000000 libesedb-20240420/libesedb/libesedb_leaf_page_descriptor.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1715 2024-04-20 12:01:44.000000 libesedb-20240420/libesedb/libesedb_i18n.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    41623 2024-04-20 12:01:44.000000 libesedb-20240420/libesedb/libesedb_multi_value.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1524 2024-04-20 12:01:44.000000 libesedb-20240420/libesedb/libesedb_block_descriptor.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2754 2024-04-20 12:01:44.000000 libesedb-20240420/libesedb/libesedb_notify.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2347 2024-04-20 12:01:44.000000 libesedb-20240420/libesedb/libesedb_block_tree.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3124 2024-04-20 12:05:52.000000 libesedb-20240420/libesedb/libesedb_codepage.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5067 2024-04-20 12:01:44.000000 libesedb-20240420/libesedb/libesedb_table.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7883 2024-04-20 14:10:10.000000 libesedb-20240420/libesedb/libesedb_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11397 2024-04-20 12:01:44.000000 libesedb-20240420/libesedb/libesedb_block_tree.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1985 2024-04-20 12:01:44.000000 libesedb-20240420/libesedb/libesedb_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3623 2024-04-20 12:01:44.000000 libesedb-20240420/libesedb/libesedb_catalog.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3434 2024-04-20 12:01:44.000000 libesedb-20240420/libesedb/libesedb_codepage.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4574 2024-04-20 12:01:44.000000 libesedb-20240420/libesedb/libesedb_file.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    38481 2024-04-20 12:01:44.000000 libesedb-20240420/libesedb/libesedb_page.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17716 2024-04-20 12:01:44.000000 libesedb-20240420/libesedb/libesedb_table_definition.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5705 2024-04-20 12:01:44.000000 libesedb-20240420/libesedb/libesedb_page_tree.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15964 2024-04-20 12:01:44.000000 libesedb-20240420/libesedb/libesedb_page_tree_key.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    78990 2024-04-20 12:01:44.000000 libesedb-20240420/libesedb/libesedb_page_tree.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3121 2024-04-20 12:01:44.000000 libesedb-20240420/libesedb/libesedb_block_descriptor.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15045 2024-04-20 12:01:44.000000 libesedb-20240420/libesedb/libesedb_block_tree_node.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9367 2024-04-20 12:01:44.000000 libesedb-20240420/libesedb/libesedb_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16782 2024-04-20 12:01:44.000000 libesedb-20240420/libesedb/libesedb_debug.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2713 2024-04-20 12:01:44.000000 libesedb-20240420/libesedb/libesedb_column.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    95847 2024-04-20 12:01:44.000000 libesedb-20240420/libesedb/libesedb_record.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1919 2024-04-20 12:01:44.000000 libesedb-20240420/libesedb/libesedb_leaf_page_descriptor.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1703 2024-04-20 12:01:44.000000 libesedb-20240420/libesedb/libesedb_libbfio.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3648 2024-04-20 12:12:56.000000 libesedb-20240420/libesedb/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-04-20 12:01:44.000000 libesedb-20240420/libesedb/libesedb_libfcache.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1593 2024-04-20 12:01:44.000000 libesedb-20240420/libesedb/libesedb_notify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5276 2024-04-20 12:01:44.000000 libesedb-20240420/libesedb/libesedb_catalog_definition.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3226 2024-04-20 12:01:44.000000 libesedb-20240420/libesedb/esedb_page.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-04-20 12:01:44.000000 libesedb-20240420/libesedb/libesedb_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1703 2024-04-20 12:01:44.000000 libesedb-20240420/libesedb/libesedb_libfwnt.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1354 2024-04-20 12:01:44.000000 libesedb-20240420/libesedb/libesedb_i18n.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5737 2024-04-20 12:01:44.000000 libesedb-20240420/libesedb/libesedb_value_data_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2061 2024-04-20 12:01:44.000000 libesedb-20240420/libesedb/libesedb_page_tree_key.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2977 2024-04-20 12:01:44.000000 libesedb-20240420/libesedb/libesedb_page_value.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15369 2024-04-20 12:01:44.000000 libesedb-20240420/libesedb/libesedb_checksum.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18457 2024-04-20 12:01:44.000000 libesedb-20240420/libesedb/libesedb_index.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5942 2024-04-20 12:01:44.000000 libesedb-20240420/libesedb/libesedb_multi_value.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-04-20 12:01:44.000000 libesedb-20240420/libesedb/libesedb_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11330 2024-04-20 12:01:44.000000 libesedb-20240420/libesedb/libesedb_column.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-04-20 12:01:44.000000 libesedb-20240420/libesedb/libesedb_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1113 2024-04-20 12:01:44.000000 libesedb-20240420/libesedb/libesedb.rc.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7230 2024-04-20 12:01:44.000000 libesedb-20240420/libesedb/libesedb_io_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1545 2024-04-20 12:01:44.000000 libesedb-20240420/libesedb/libesedb_libfdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1856 2024-04-20 12:01:44.000000 libesedb-20240420/libesedb/libesedb.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    49390 2024-04-20 12:01:44.000000 libesedb-20240420/libesedb/libesedb_file.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14047 2024-04-20 12:01:44.000000 libesedb-20240420/libesedb/libesedb_page_header.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4754 2024-04-20 12:01:44.000000 libesedb-20240420/libesedb/libesedb_space_tree_value.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3115 2024-04-20 12:01:44.000000 libesedb-20240420/libesedb/libesedb_compression.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7281 2024-04-20 12:01:44.000000 libesedb-20240420/libesedb/libesedb_root_page_header.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1736 2024-04-20 12:01:44.000000 libesedb-20240420/libesedb/libesedb_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4225 2024-04-20 12:01:44.000000 libesedb-20240420/libesedb/libesedb_index.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8883 2024-04-20 12:01:44.000000 libesedb-20240420/libesedb/libesedb_record.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3847 2024-04-20 12:01:44.000000 libesedb-20240420/libesedb/libesedb_table_definition.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4118 2024-04-20 12:01:44.000000 libesedb-20240420/libesedb/libesedb_long_value.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2263 2024-04-20 12:01:44.000000 libesedb-20240420/libesedb/libesedb_data_segment.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32872 2024-04-20 12:01:44.000000 libesedb-20240420/libesedb/libesedb_catalog.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11826 2024-04-20 12:01:44.000000 libesedb-20240420/libesedb/libesedb_record_value.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    38738 2024-04-20 12:01:44.000000 libesedb-20240420/libesedb/libesedb_table.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-04-20 12:01:44.000000 libesedb-20240420/libesedb/libesedb_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1784 2024-04-20 12:01:44.000000 libesedb-20240420/libesedb/libesedb_record_value.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2277 2024-04-20 12:01:44.000000 libesedb-20240420/libesedb/libesedb_debug.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2836 2024-04-20 12:01:44.000000 libesedb-20240420/libesedb/libesedb_page_header.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2949 2024-04-20 12:01:44.000000 libesedb-20240420/libesedb/libesedb_block_tree_node.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3339 2024-04-20 12:01:44.000000 libesedb-20240420/libesedb/libesedb_data_definition.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1791 2024-04-20 12:01:44.000000 libesedb-20240420/libesedb/libesedb_libfvalue.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    55707 2024-04-20 12:01:44.000000 libesedb-20240420/libesedb/libesedb_data_definition.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2200 2024-04-20 12:01:44.000000 libesedb-20240420/libesedb/libesedb_space_tree.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18749 2024-04-20 12:01:44.000000 libesedb-20240420/libesedb/libesedb_lcid.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20066 2024-04-20 12:01:44.000000 libesedb-20240420/libesedb/libesedb_space_tree.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2024-04-20 12:01:44.000000 libesedb-20240420/libesedb/libesedb_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6795 2024-04-20 12:01:44.000000 libesedb-20240420/libesedb/libesedb_page_tree_value.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    45482 2024-04-20 14:09:57.000000 libesedb-20240420/libesedb/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2141 2024-04-20 12:01:44.000000 libesedb-20240420/libesedb/libesedb_database.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30559 2024-04-20 12:01:44.000000 libesedb-20240420/libesedb/libesedb_compression.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2195 2024-04-20 12:01:44.000000 libesedb-20240420/libesedb/libesedb_file_header.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1914 2024-04-20 12:01:44.000000 libesedb-20240420/libesedb/libesedb_page_tree_value.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-04-20 12:01:44.000000 libesedb-20240420/libesedb/libesedb_value_data_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3862 2024-04-20 12:01:44.000000 libesedb-20240420/libesedb/libesedb_page.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    50190 2024-04-20 12:01:44.000000 libesedb-20240420/libesedb/libesedb_catalog_definition.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33342 2024-04-20 12:01:44.000000 libesedb-20240420/libesedb/libesedb_long_value.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5517 2024-04-20 12:01:44.000000 libesedb-20240420/libesedb/esedb_page_values.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1527 2024-04-20 12:01:44.000000 libesedb-20240420/libesedb/libesedb_checksum.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1556 2024-04-20 12:01:44.000000 libesedb-20240420/libesedb/libesedb_column_type.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1612 2024-04-20 12:01:44.000000 libesedb-20240420/libesedb/libesedb_page_value.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13891 2024-04-20 12:01:44.000000 libesedb-20240420/libesedb/libesedb_database.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2053 2024-04-20 12:01:44.000000 libesedb-20240420/libesedb/libesedb_types.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-20 14:34:04.000000 libesedb-20240420/msvscpp/
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-20 14:34:04.000000 libesedb-20240420/msvscpp/esedb_test_page_tree_value/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5983 2024-04-20 12:05:02.000000 libesedb-20240420/msvscpp/esedb_test_page_tree_value/esedb_test_page_tree_value.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-20 14:34:04.000000 libesedb-20240420/msvscpp/libfdata/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6858 2024-04-20 12:02:17.000000 libesedb-20240420/msvscpp/libfdata/libfdata.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-20 14:34:04.000000 libesedb-20240420/msvscpp/esedb_test_long_value/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5968 2024-04-20 12:05:02.000000 libesedb-20240420/msvscpp/esedb_test_long_value/esedb_test_long_value.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-20 14:34:04.000000 libesedb-20240420/msvscpp/esedb_test_space_tree/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5968 2024-04-20 12:05:02.000000 libesedb-20240420/msvscpp/esedb_test_space_tree/esedb_test_space_tree.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-20 14:34:04.000000 libesedb-20240420/msvscpp/esedb_test_file/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6613 2024-04-20 12:05:02.000000 libesedb-20240420/msvscpp/esedb_test_file/esedb_test_file.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-20 14:34:04.000000 libesedb-20240420/msvscpp/esedb_test_space_tree_value/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5986 2024-04-20 12:05:02.000000 libesedb-20240420/msvscpp/esedb_test_space_tree_value/esedb_test_space_tree_value.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-20 14:34:04.000000 libesedb-20240420/msvscpp/esedb_test_block_tree_node/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5983 2024-04-20 12:05:02.000000 libesedb-20240420/msvscpp/esedb_test_block_tree_node/esedb_test_block_tree_node.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-20 14:34:04.000000 libesedb-20240420/msvscpp/esedb_test_checksum/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5962 2024-04-20 12:05:02.000000 libesedb-20240420/msvscpp/esedb_test_checksum/esedb_test_checksum.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-20 14:34:04.000000 libesedb-20240420/msvscpp/esedb_test_block_descriptor/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5986 2024-04-20 12:05:02.000000 libesedb-20240420/msvscpp/esedb_test_block_descriptor/esedb_test_block_descriptor.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-20 14:34:04.000000 libesedb-20240420/msvscpp/esedb_test_database/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5962 2024-04-20 12:05:02.000000 libesedb-20240420/msvscpp/esedb_test_database/esedb_test_database.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-20 14:34:04.000000 libesedb-20240420/msvscpp/esedbexport/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9040 2024-04-20 12:02:17.000000 libesedb-20240420/msvscpp/esedbexport/esedbexport.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-20 14:34:04.000000 libesedb-20240420/msvscpp/esedb_test_table/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5953 2024-04-20 12:05:02.000000 libesedb-20240420/msvscpp/esedb_test_table/esedb_test_table.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-20 14:34:04.000000 libesedb-20240420/msvscpp/esedbinfo/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7122 2024-04-20 12:02:17.000000 libesedb-20240420/msvscpp/esedbinfo/esedbinfo.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-20 14:34:04.000000 libesedb-20240420/msvscpp/esedb_test_page/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6200 2024-04-20 12:05:02.000000 libesedb-20240420/msvscpp/esedb_test_page/esedb_test_page.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-20 14:34:04.000000 libesedb-20240420/msvscpp/esedb_test_column_type/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5971 2024-04-20 12:05:02.000000 libesedb-20240420/msvscpp/esedb_test_column_type/esedb_test_column_type.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-20 14:34:04.000000 libesedb-20240420/msvscpp/libfguid/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4631 2024-04-20 12:02:17.000000 libesedb-20240420/msvscpp/libfguid/libfguid.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-20 14:34:04.000000 libesedb-20240420/msvscpp/esedb_test_catalog_definition/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5992 2024-04-20 12:05:02.000000 libesedb-20240420/msvscpp/esedb_test_catalog_definition/esedb_test_catalog_definition.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-20 14:34:04.000000 libesedb-20240420/msvscpp/esedb_test_tools_windows_search_compression/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6141 2024-04-20 12:05:02.000000 libesedb-20240420/msvscpp/esedb_test_tools_windows_search_compression/esedb_test_tools_windows_search_compression.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-20 14:34:04.000000 libesedb-20240420/msvscpp/libclocale/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4778 2024-04-20 12:02:17.000000 libesedb-20240420/msvscpp/libclocale/libclocale.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-20 14:34:04.000000 libesedb-20240420/msvscpp/esedb_test_data_definition/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5983 2024-04-20 12:05:02.000000 libesedb-20240420/msvscpp/esedb_test_data_definition/esedb_test_data_definition.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-20 14:34:04.000000 libesedb-20240420/msvscpp/esedb_test_support/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6622 2024-04-20 12:05:02.000000 libesedb-20240420/msvscpp/esedb_test_support/esedb_test_support.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-20 14:34:04.000000 libesedb-20240420/msvscpp/esedb_test_index/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5953 2024-04-20 12:05:02.000000 libesedb-20240420/msvscpp/esedb_test_index/esedb_test_index.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-20 14:34:04.000000 libesedb-20240420/msvscpp/libfcache/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5237 2024-04-20 12:02:17.000000 libesedb-20240420/msvscpp/libfcache/libfcache.vcproj
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2908 2024-04-20 12:13:06.000000 libesedb-20240420/msvscpp/Makefile.am
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-20 14:34:04.000000 libesedb-20240420/msvscpp/libbfio/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7306 2024-04-20 12:02:17.000000 libesedb-20240420/msvscpp/libbfio/libbfio.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-20 14:34:04.000000 libesedb-20240420/msvscpp/esedb_test_column/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5956 2024-04-20 12:05:02.000000 libesedb-20240420/msvscpp/esedb_test_column/esedb_test_column.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-20 14:34:04.000000 libesedb-20240420/msvscpp/libesedb/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13652 2024-04-20 12:02:17.000000 libesedb-20240420/msvscpp/libesedb/libesedb.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-20 14:34:04.000000 libesedb-20240420/msvscpp/esedb_test_leaf_page_descriptor/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6081 2024-04-20 12:05:02.000000 libesedb-20240420/msvscpp/esedb_test_leaf_page_descriptor/esedb_test_leaf_page_descriptor.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-20 14:34:04.000000 libesedb-20240420/msvscpp/esedb_test_block_tree/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5968 2024-04-20 12:05:02.000000 libesedb-20240420/msvscpp/esedb_test_block_tree/esedb_test_block_tree.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-20 14:34:04.000000 libesedb-20240420/msvscpp/esedb_test_io_handle/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5965 2024-04-20 12:05:02.000000 libesedb-20240420/msvscpp/esedb_test_io_handle/esedb_test_io_handle.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-20 14:34:04.000000 libesedb-20240420/msvscpp/libcfile/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5597 2024-04-20 12:02:17.000000 libesedb-20240420/msvscpp/libcfile/libcfile.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-20 14:34:04.000000 libesedb-20240420/msvscpp/libmapidb/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4987 2024-04-20 12:02:17.000000 libesedb-20240420/msvscpp/libmapidb/libmapidb.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-20 14:34:04.000000 libesedb-20240420/msvscpp/esedb_test_compression/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5971 2024-04-20 12:05:02.000000 libesedb-20240420/msvscpp/esedb_test_compression/esedb_test_compression.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-20 14:34:04.000000 libesedb-20240420/msvscpp/libcdata/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6172 2024-04-20 12:02:17.000000 libesedb-20240420/msvscpp/libcdata/libcdata.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-20 14:34:04.000000 libesedb-20240420/msvscpp/esedb_test_page_tree_key/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6060 2024-04-20 12:05:02.000000 libesedb-20240420/msvscpp/esedb_test_page_tree_key/esedb_test_page_tree_key.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-20 14:34:04.000000 libesedb-20240420/msvscpp/libfmapi/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7276 2024-04-20 12:02:17.000000 libesedb-20240420/msvscpp/libfmapi/libfmapi.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-20 14:34:04.000000 libesedb-20240420/msvscpp/esedb_test_file_header/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6221 2024-04-20 12:05:02.000000 libesedb-20240420/msvscpp/esedb_test_file_header/esedb_test_file_header.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-20 14:34:04.000000 libesedb-20240420/msvscpp/esedb_test_tools_info_handle/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6066 2024-04-20 12:05:02.000000 libesedb-20240420/msvscpp/esedb_test_tools_info_handle/esedb_test_tools_info_handle.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-20 14:34:04.000000 libesedb-20240420/msvscpp/pyesedb/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8339 2024-04-20 12:05:02.000000 libesedb-20240420/msvscpp/pyesedb/pyesedb.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-20 14:34:04.000000 libesedb-20240420/msvscpp/esedb_test_page_value/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5968 2024-04-20 12:05:02.000000 libesedb-20240420/msvscpp/esedb_test_page_value/esedb_test_page_value.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-20 14:34:04.000000 libesedb-20240420/msvscpp/esedb_test_root_page_header/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5986 2024-04-20 12:05:02.000000 libesedb-20240420/msvscpp/esedb_test_root_page_header/esedb_test_root_page_header.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-20 14:34:04.000000 libesedb-20240420/msvscpp/libcthreads/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6177 2024-04-20 12:02:17.000000 libesedb-20240420/msvscpp/libcthreads/libcthreads.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-20 14:34:04.000000 libesedb-20240420/msvscpp/esedb_test_tools_output/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5901 2024-04-20 12:05:02.000000 libesedb-20240420/msvscpp/esedb_test_tools_output/esedb_test_tools_output.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-20 14:34:04.000000 libesedb-20240420/msvscpp/libcpath/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5183 2024-04-20 12:02:17.000000 libesedb-20240420/msvscpp/libcpath/libcpath.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-20 14:34:04.000000 libesedb-20240420/msvscpp/esedb_test_tools_signal/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5901 2024-04-20 12:05:02.000000 libesedb-20240420/msvscpp/esedb_test_tools_signal/esedb_test_tools_signal.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-20 14:34:04.000000 libesedb-20240420/msvscpp/libfwnt/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6895 2024-04-20 12:02:17.000000 libesedb-20240420/msvscpp/libfwnt/libfwnt.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-20 14:34:04.000000 libesedb-20240420/msvscpp/esedb_test_table_definition/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5986 2024-04-20 12:05:02.000000 libesedb-20240420/msvscpp/esedb_test_table_definition/esedb_test_table_definition.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-20 14:34:04.000000 libesedb-20240420/msvscpp/esedb_test_multi_value/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5971 2024-04-20 12:05:02.000000 libesedb-20240420/msvscpp/esedb_test_multi_value/esedb_test_multi_value.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-20 14:34:04.000000 libesedb-20240420/msvscpp/esedb_test_catalog/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6292 2024-04-20 12:05:02.000000 libesedb-20240420/msvscpp/esedb_test_catalog/esedb_test_catalog.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-20 14:34:04.000000 libesedb-20240420/msvscpp/libcsplit/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5225 2024-04-20 12:02:17.000000 libesedb-20240420/msvscpp/libcsplit/libcsplit.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-20 14:34:04.000000 libesedb-20240420/msvscpp/esedb_test_record/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5956 2024-04-20 12:05:02.000000 libesedb-20240420/msvscpp/esedb_test_record/esedb_test_record.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-20 14:34:04.000000 libesedb-20240420/msvscpp/libuna/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15387 2024-04-20 12:02:17.000000 libesedb-20240420/msvscpp/libuna/libuna.vcproj
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25841 2024-04-20 14:09:58.000000 libesedb-20240420/msvscpp/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-20 14:34:04.000000 libesedb-20240420/msvscpp/libfvalue/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8076 2024-04-20 12:02:17.000000 libesedb-20240420/msvscpp/libfvalue/libfvalue.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-20 14:34:04.000000 libesedb-20240420/msvscpp/esedb_test_page_tree/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5965 2024-04-20 12:05:02.000000 libesedb-20240420/msvscpp/esedb_test_page_tree/esedb_test_page_tree.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-20 14:34:04.000000 libesedb-20240420/msvscpp/esedb_test_error/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5707 2024-04-20 12:05:02.000000 libesedb-20240420/msvscpp/esedb_test_error/esedb_test_error.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-20 14:34:04.000000 libesedb-20240420/msvscpp/esedb_test_data_segment/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6391 2024-04-20 12:05:02.000000 libesedb-20240420/msvscpp/esedb_test_data_segment/esedb_test_data_segment.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-20 14:34:04.000000 libesedb-20240420/msvscpp/libcnotify/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4764 2024-04-20 12:02:17.000000 libesedb-20240420/msvscpp/libcnotify/libcnotify.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-20 14:34:04.000000 libesedb-20240420/msvscpp/libcerror/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4488 2024-04-20 12:02:17.000000 libesedb-20240420/msvscpp/libcerror/libcerror.vcproj
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    53317 2024-04-20 12:05:02.000000 libesedb-20240420/msvscpp/libesedb.sln
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-20 14:34:04.000000 libesedb-20240420/msvscpp/esedb_test_notify/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5794 2024-04-20 12:05:02.000000 libesedb-20240420/msvscpp/esedb_test_notify/esedb_test_notify.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-20 14:34:04.000000 libesedb-20240420/msvscpp/libfdatetime/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6069 2024-04-20 12:02:17.000000 libesedb-20240420/msvscpp/libfdatetime/libfdatetime.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-20 14:34:04.000000 libesedb-20240420/msvscpp/esedb_test_page_header/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5971 2024-04-20 12:05:02.000000 libesedb-20240420/msvscpp/esedb_test_page_header/esedb_test_page_header.vcproj
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       92 2024-04-20 12:01:42.000000 libesedb-20240420/AUTHORS
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-20 14:34:01.000000 libesedb-20240420/libcfile/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-04-20 14:09:25.000000 libesedb-20240420/libcfile/libcfile_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2389 2024-04-20 14:09:25.000000 libesedb-20240420/libcfile/libcfile_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-04-20 14:09:25.000000 libesedb-20240420/libcfile/libcfile_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1593 2024-04-20 14:09:25.000000 libesedb-20240420/libcfile/libcfile_notify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25753 2024-04-20 14:09:25.000000 libesedb-20240420/libcfile/libcfile_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1497 2024-04-20 14:09:25.000000 libesedb-20240420/libcfile/libcfile_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      938 2024-04-20 14:09:25.000000 libesedb-20240420/libcfile/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2754 2024-04-20 14:09:25.000000 libesedb-20240420/libcfile/libcfile_notify.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2826 2024-04-20 14:09:25.000000 libesedb-20240420/libcfile/libcfile_system_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6452 2024-04-20 14:09:25.000000 libesedb-20240420/libcfile/libcfile_file.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-04-20 14:09:25.000000 libesedb-20240420/libcfile/libcfile_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25560 2024-04-20 14:09:25.000000 libesedb-20240420/libcfile/libcfile_system_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-04-20 14:09:25.000000 libesedb-20240420/libcfile/libcfile_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-04-20 14:09:25.000000 libesedb-20240420/libcfile/libcfile_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   105597 2024-04-20 14:09:25.000000 libesedb-20240420/libcfile/libcfile_file.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2024-04-20 14:09:25.000000 libesedb-20240420/libcfile/libcfile_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3107 2024-04-20 14:09:25.000000 libesedb-20240420/libcfile/libcfile_winapi.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31974 2024-04-20 14:09:57.000000 libesedb-20240420/libcfile/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-04-20 14:09:25.000000 libesedb-20240420/libcfile/libcfile_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1736 2024-04-20 14:09:25.000000 libesedb-20240420/libcfile/libcfile_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18388 2024-04-20 14:09:25.000000 libesedb-20240420/libcfile/libcfile_winapi.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2879 2024-04-20 14:09:25.000000 libesedb-20240420/libcfile/libcfile_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      856 2024-04-20 12:05:41.000000 libesedb-20240420/README
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-20 14:34:03.000000 libesedb-20240420/libmapidb/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-04-20 14:09:42.000000 libesedb-20240420/libmapidb/libmapidb_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1379 2024-04-20 14:09:42.000000 libesedb-20240420/libmapidb/libmapidb_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1535 2024-04-20 14:09:42.000000 libesedb-20240420/libmapidb/libmapidb_folder.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-04-20 14:09:42.000000 libesedb-20240420/libmapidb/libmapidb_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      781 2024-04-20 14:09:42.000000 libesedb-20240420/libmapidb/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1731 2024-04-20 14:09:42.000000 libesedb-20240420/libmapidb/libmapidb_database.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1613 2024-04-20 14:09:42.000000 libesedb-20240420/libmapidb/libmapidb_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3220 2024-04-20 14:09:42.000000 libesedb-20240420/libmapidb/libmapidb_folder.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3312 2024-04-20 14:09:42.000000 libesedb-20240420/libmapidb/libmapidb_database.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-04-20 14:09:42.000000 libesedb-20240420/libmapidb/libmapidb_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31130 2024-04-20 14:09:58.000000 libesedb-20240420/libmapidb/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1199 2024-04-20 14:09:42.000000 libesedb-20240420/libmapidb/libmapidb_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-04-20 14:09:42.000000 libesedb-20240420/libmapidb/libmapidb_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1536 2024-04-20 14:09:42.000000 libesedb-20240420/libmapidb/libmapidb_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2924 2024-04-20 14:09:42.000000 libesedb-20240420/libmapidb/libmapidb_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1172 2024-04-20 14:09:42.000000 libesedb-20240420/libmapidb/libmapidb_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15766 2024-04-20 14:09:57.000000 libesedb-20240420/INSTALL
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-20 14:34:01.000000 libesedb-20240420/libcdata/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3871 2024-04-20 14:09:22.000000 libesedb-20240420/libcdata/libcdata_list_element.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5231 2024-04-20 14:09:22.000000 libesedb-20240420/libcdata/libcdata_array.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2115 2024-04-20 14:09:22.000000 libesedb-20240420/libcdata/libcdata_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-04-20 14:09:22.000000 libesedb-20240420/libcdata/libcdata_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-04-20 14:09:22.000000 libesedb-20240420/libcdata/libcdata_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3790 2024-04-20 14:09:22.000000 libesedb-20240420/libcdata/libcdata_btree.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22358 2024-04-20 14:09:22.000000 libesedb-20240420/libcdata/libcdata_btree.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1152 2024-04-20 14:09:22.000000 libesedb-20240420/libcdata/libcdata_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    69515 2024-04-20 14:09:22.000000 libesedb-20240420/libcdata/libcdata_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-04-20 14:09:22.000000 libesedb-20240420/libcdata/libcdata_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6448 2024-04-20 14:09:22.000000 libesedb-20240420/libcdata/libcdata_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1648 2024-04-20 14:09:22.000000 libesedb-20240420/libcdata/libcdata_btree_values_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1123 2024-04-20 14:09:22.000000 libesedb-20240420/libcdata/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2960 2024-04-20 14:09:22.000000 libesedb-20240420/libcdata/libcdata_btree_node.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2789 2024-04-20 14:09:22.000000 libesedb-20240420/libcdata/libcdata_range_list_value.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12295 2024-04-20 14:09:22.000000 libesedb-20240420/libcdata/libcdata_range_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   122285 2024-04-20 14:09:22.000000 libesedb-20240420/libcdata/libcdata_range_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    49968 2024-04-20 14:09:22.000000 libesedb-20240420/libcdata/libcdata_array.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23846 2024-04-20 14:09:22.000000 libesedb-20240420/libcdata/libcdata_list_element.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1925 2024-04-20 14:09:22.000000 libesedb-20240420/libcdata/libcdata_libcthreads.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8365 2024-04-20 14:09:22.000000 libesedb-20240420/libcdata/libcdata_tree_node.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-04-20 14:09:22.000000 libesedb-20240420/libcdata/libcdata_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1976 2024-04-20 14:09:22.000000 libesedb-20240420/libcdata/libcdata_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37549 2024-04-20 14:09:22.000000 libesedb-20240420/libcdata/libcdata_btree_node.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   100501 2024-04-20 14:09:22.000000 libesedb-20240420/libcdata/libcdata_tree_node.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1230 2024-04-20 14:09:22.000000 libesedb-20240420/libcdata/libcdata_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33887 2024-04-20 14:09:57.000000 libesedb-20240420/libcdata/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10647 2024-04-20 14:09:22.000000 libesedb-20240420/libcdata/libcdata_range_list_value.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5251 2024-04-20 14:09:22.000000 libesedb-20240420/libcdata/libcdata_btree_values_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-04-20 14:09:22.000000 libesedb-20240420/libcdata/libcdata_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       91 2024-04-20 12:01:39.000000 libesedb-20240420/pyproject.toml
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-20 14:34:03.000000 libesedb-20240420/libfmapi/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1508 2024-04-20 14:09:37.000000 libesedb-20240420/libfmapi/libfmapi_value_type.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   124848 2024-04-20 14:09:37.000000 libesedb-20240420/libfmapi/libfmapi_debug.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1913 2024-04-20 14:09:37.000000 libesedb-20240420/libfmapi/libfmapi_x400_object_identifier.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1398 2024-04-20 14:09:37.000000 libesedb-20240420/libfmapi/libfmapi_libfguid.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1377 2024-04-20 14:09:37.000000 libesedb-20240420/libfmapi/libfmapi_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2174 2024-04-20 14:09:37.000000 libesedb-20240420/libfmapi/libfmapi_entry_identifier.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1703 2024-04-20 14:09:37.000000 libesedb-20240420/libfmapi/libfmapi_libfwnt.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    40853 2024-04-20 14:09:37.000000 libesedb-20240420/libfmapi/libfmapi_one_off_entry_identifier.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5468 2024-04-20 14:09:37.000000 libesedb-20240420/libfmapi/libfmapi_one_off_entry_identifier.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1543 2024-04-20 14:09:37.000000 libesedb-20240420/libfmapi/libfmapi_codepage.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3422 2024-04-20 14:09:37.000000 libesedb-20240420/libfmapi/libfmapi_codepage.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1506 2024-04-20 14:09:37.000000 libesedb-20240420/libfmapi/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-04-20 14:09:37.000000 libesedb-20240420/libfmapi/libfmapi_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2927 2024-04-20 14:09:37.000000 libesedb-20240420/libfmapi/libfmapi_debug.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10342 2024-04-20 14:09:37.000000 libesedb-20240420/libfmapi/libfmapi_entry_identifier.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2951 2024-04-20 14:09:37.000000 libesedb-20240420/libfmapi/libfmapi_class_identifier.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3877 2024-04-20 14:09:37.000000 libesedb-20240420/libfmapi/libfmapi_value_type.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1736 2024-04-20 14:09:37.000000 libesedb-20240420/libfmapi/libfmapi_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2189 2024-04-20 14:09:37.000000 libesedb-20240420/libfmapi/libfmapi_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1152 2024-04-20 14:09:37.000000 libesedb-20240420/libfmapi/libfmapi_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-04-20 14:09:37.000000 libesedb-20240420/libfmapi/libfmapi_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5127 2024-04-20 14:09:37.000000 libesedb-20240420/libfmapi/libfmapi_class_identifier.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1670 2024-04-20 14:09:37.000000 libesedb-20240420/libfmapi/libfmapi_checksum.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4882 2024-04-20 14:09:37.000000 libesedb-20240420/libfmapi/libfmapi_checksum.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   158504 2024-04-20 14:09:37.000000 libesedb-20240420/libfmapi/libfmapi_property_type.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1726 2024-04-20 14:09:37.000000 libesedb-20240420/libfmapi/libfmapi_libfdatetime.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16455 2024-04-20 14:09:37.000000 libesedb-20240420/libfmapi/libfmapi_lzfu.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1677 2024-04-20 14:09:37.000000 libesedb-20240420/libfmapi/libfmapi_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3352 2024-04-20 14:09:37.000000 libesedb-20240420/libfmapi/libfmapi_property_type.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2015 2024-04-20 14:09:37.000000 libesedb-20240420/libfmapi/libfmapi_lzfu.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-04-20 14:09:37.000000 libesedb-20240420/libfmapi/libfmapi_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2780 2024-04-20 14:09:37.000000 libesedb-20240420/libfmapi/libfmapi_service_provider_identifier.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-04-20 14:09:37.000000 libesedb-20240420/libfmapi/libfmapi_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35300 2024-04-20 14:09:57.000000 libesedb-20240420/libfmapi/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1230 2024-04-20 14:09:37.000000 libesedb-20240420/libfmapi/libfmapi_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-04-20 14:09:37.000000 libesedb-20240420/libfmapi/libfmapi_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1523 2024-04-20 14:09:37.000000 libesedb-20240420/libfmapi/libfmapi_service_provider_identifier.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      487 2024-04-20 12:01:39.000000 libesedb-20240420/setup.cfg.in
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    35796 2024-04-20 14:09:57.000000 libesedb-20240420/config.sub
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2500 2024-04-20 14:10:10.000000 libesedb-20240420/libesedb.spec
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     9278 2024-04-20 12:01:39.000000 libesedb-20240420/setup.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1485 2024-04-20 12:01:39.000000 libesedb-20240420/acinclude.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      763 2024-04-20 12:01:39.000000 libesedb-20240420/libesedb.pc.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-20 14:34:03.000000 libesedb-20240420/pyesedb/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1525 2024-04-20 12:01:45.000000 libesedb-20240420/pyesedb/pyesedb_libbfio.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9143 2024-04-20 12:01:45.000000 libesedb-20240420/pyesedb/pyesedb_records.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-04-20 12:01:45.000000 libesedb-20240420/pyesedb/pyesedb_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2024-04-20 12:01:45.000000 libesedb-20240420/pyesedb/pyesedb_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2361 2024-04-20 12:01:45.000000 libesedb-20240420/pyesedb/pyesedb_tables.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2382 2024-04-20 12:01:45.000000 libesedb-20240420/pyesedb/pyesedb_records.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1540 2024-04-20 12:01:45.000000 libesedb-20240420/pyesedb/pyesedb_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19373 2024-04-20 12:05:41.000000 libesedb-20240420/pyesedb/pyesedb.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21412 2024-04-20 12:05:41.000000 libesedb-20240420/pyesedb/pyesedb_multi_value.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4118 2024-04-20 12:01:45.000000 libesedb-20240420/pyesedb/pyesedb_file_object_io_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14701 2024-04-20 12:05:41.000000 libesedb-20240420/pyesedb/pyesedb_index.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22344 2024-04-20 12:05:41.000000 libesedb-20240420/pyesedb/pyesedb_table.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2414 2024-04-20 12:01:45.000000 libesedb-20240420/pyesedb/pyesedb_index.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2661 2024-04-20 12:05:41.000000 libesedb-20240420/pyesedb/pyesedb_multi_value.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1644 2024-04-20 12:13:48.000000 libesedb-20240420/pyesedb/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1648 2024-04-20 12:01:45.000000 libesedb-20240420/pyesedb/pyesedb_column_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16609 2024-04-20 12:01:45.000000 libesedb-20240420/pyesedb/pyesedb_datetime.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5524 2024-04-20 12:01:45.000000 libesedb-20240420/pyesedb/pyesedb_file_types.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3527 2024-04-20 12:05:41.000000 libesedb-20240420/pyesedb/pyesedb_file.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2033 2024-04-20 12:01:45.000000 libesedb-20240420/pyesedb/pyesedb_python.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9143 2024-04-20 12:01:45.000000 libesedb-20240420/pyesedb/pyesedb_columns.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2055 2024-04-20 12:05:41.000000 libesedb-20240420/pyesedb/pyesedb_long_value.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9546 2024-04-20 12:01:45.000000 libesedb-20240420/pyesedb/pyesedb_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1544 2024-04-20 12:01:45.000000 libesedb-20240420/pyesedb/pyesedb_integer.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1860 2024-04-20 12:01:45.000000 libesedb-20240420/pyesedb/pyesedb.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8876 2024-04-20 12:01:45.000000 libesedb-20240420/pyesedb/pyesedb_integer.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      973 2024-04-20 12:01:45.000000 libesedb-20240420/pyesedb/pyesedb_libesedb.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9131 2024-04-20 12:01:45.000000 libesedb-20240420/pyesedb/pyesedb_indexes.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34152 2024-04-20 12:05:41.000000 libesedb-20240420/pyesedb/pyesedb_record.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9081 2024-04-20 12:01:45.000000 libesedb-20240420/pyesedb/pyesedb_tables.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33880 2024-04-20 12:01:45.000000 libesedb-20240420/pyesedb/pyesedb_file_object_io_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2024-04-20 12:01:45.000000 libesedb-20240420/pyesedb/pyesedb_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1826 2024-04-20 12:01:45.000000 libesedb-20240420/pyesedb/pyesedb_datetime.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6224 2024-04-20 12:01:45.000000 libesedb-20240420/pyesedb/pyesedb_value_flags.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3033 2024-04-20 12:05:41.000000 libesedb-20240420/pyesedb/pyesedb_table.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2058 2024-04-20 12:01:45.000000 libesedb-20240420/pyesedb/pyesedb_column.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2382 2024-04-20 12:01:45.000000 libesedb-20240420/pyesedb/pyesedb_indexes.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10759 2024-04-20 12:05:41.000000 libesedb-20240420/pyesedb/pyesedb_column.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10628 2024-04-20 12:05:41.000000 libesedb-20240420/pyesedb/pyesedb_long_value.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28235 2024-04-20 12:05:41.000000 libesedb-20240420/pyesedb/pyesedb_file.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2382 2024-04-20 12:01:45.000000 libesedb-20240420/pyesedb/pyesedb_columns.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    62490 2024-04-20 14:09:58.000000 libesedb-20240420/pyesedb/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1634 2024-04-20 12:01:45.000000 libesedb-20240420/pyesedb/pyesedb_value_flags.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1620 2024-04-20 12:01:45.000000 libesedb-20240420/pyesedb/pyesedb_file_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11099 2024-04-20 12:01:45.000000 libesedb-20240420/pyesedb/pyesedb_column_types.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3594 2024-04-20 12:05:41.000000 libesedb-20240420/pyesedb/pyesedb_record.h
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    18574 2023-12-03 09:00:45.000000 libesedb-20240420/config.rpath
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-20 14:34:01.000000 libesedb-20240420/libcthreads/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2356 2024-04-20 14:09:31.000000 libesedb-20240420/libcthreads/libcthreads_thread.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3195 2024-04-20 14:09:31.000000 libesedb-20240420/libcthreads/libcthreads_read_write_lock.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10198 2024-04-20 14:09:31.000000 libesedb-20240420/libcthreads/libcthreads_thread.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4175 2024-04-20 14:09:31.000000 libesedb-20240420/libcthreads/libcthreads_thread_pool.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1254 2024-04-20 14:09:31.000000 libesedb-20240420/libcthreads/libcthreads_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2208 2024-04-20 14:09:31.000000 libesedb-20240420/libcthreads/libcthreads_lock.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-04-20 14:09:31.000000 libesedb-20240420/libcthreads/libcthreads_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8753 2024-04-20 14:09:31.000000 libesedb-20240420/libcthreads/libcthreads_lock.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3040 2024-04-20 14:09:31.000000 libesedb-20240420/libcthreads/libcthreads_condition.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2870 2024-04-20 14:09:31.000000 libesedb-20240420/libcthreads/libcthreads_repeating_thread.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1167 2024-04-20 14:09:31.000000 libesedb-20240420/libcthreads/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1170 2024-04-20 14:09:31.000000 libesedb-20240420/libcthreads/libcthreads_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13601 2024-04-20 14:09:31.000000 libesedb-20240420/libcthreads/libcthreads_mutex.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26519 2024-04-20 14:09:31.000000 libesedb-20240420/libcthreads/libcthreads_queue.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2434 2024-04-20 14:09:31.000000 libesedb-20240420/libcthreads/libcthreads_mutex.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2510 2024-04-20 14:09:31.000000 libesedb-20240420/libcthreads/libcthreads_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2138 2024-04-20 14:09:31.000000 libesedb-20240420/libcthreads/libcthreads_thread_attributes.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18281 2024-04-20 14:09:31.000000 libesedb-20240420/libcthreads/libcthreads_condition.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2952 2024-04-20 14:09:31.000000 libesedb-20240420/libcthreads/libcthreads_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18426 2024-04-20 14:09:31.000000 libesedb-20240420/libcthreads/libcthreads_read_write_lock.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1447 2024-04-20 14:09:31.000000 libesedb-20240420/libcthreads/libcthreads_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2128 2024-04-20 14:09:31.000000 libesedb-20240420/libcthreads/libcthreads_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    43321 2024-04-20 14:09:31.000000 libesedb-20240420/libcthreads/libcthreads_thread_pool.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1864 2024-04-20 14:09:31.000000 libesedb-20240420/libcthreads/libcthreads_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4096 2024-04-20 14:09:31.000000 libesedb-20240420/libcthreads/libcthreads_thread_attributes.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1428 2024-04-20 14:09:31.000000 libesedb-20240420/libcthreads/libcthreads_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17481 2024-04-20 14:09:31.000000 libesedb-20240420/libcthreads/libcthreads_repeating_thread.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34326 2024-04-20 14:09:57.000000 libesedb-20240420/libcthreads/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3341 2024-04-20 14:09:31.000000 libesedb-20240420/libcthreads/libcthreads_queue.h
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4879 2024-04-20 14:09:58.000000 libesedb-20240420/test-driver
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-20 14:34:01.000000 libesedb-20240420/libcpath/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2336 2024-04-20 14:09:28.000000 libesedb-20240420/libcpath/libcpath_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-04-20 14:09:28.000000 libesedb-20240420/libcpath/libcpath_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1990 2024-04-20 14:09:28.000000 libesedb-20240420/libcpath/libcpath_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      838 2024-04-20 14:09:28.000000 libesedb-20240420/libcpath/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-04-20 14:09:28.000000 libesedb-20240420/libcpath/libcpath_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-04-20 14:09:28.000000 libesedb-20240420/libcpath/libcpath_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2826 2024-04-20 14:09:28.000000 libesedb-20240420/libcpath/libcpath_system_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1461 2024-04-20 14:09:28.000000 libesedb-20240420/libcpath/libcpath_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1536 2024-04-20 14:09:28.000000 libesedb-20240420/libcpath/libcpath_libcsplit.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25560 2024-04-20 14:09:28.000000 libesedb-20240420/libcpath/libcpath_system_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2024-04-20 14:09:28.000000 libesedb-20240420/libcpath/libcpath_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-04-20 14:09:28.000000 libesedb-20240420/libcpath/libcpath_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31172 2024-04-20 14:09:57.000000 libesedb-20240420/libcpath/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1736 2024-04-20 14:09:28.000000 libesedb-20240420/libcpath/libcpath_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-04-20 14:09:28.000000 libesedb-20240420/libcpath/libcpath_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   176165 2024-04-20 14:09:28.000000 libesedb-20240420/libcpath/libcpath_path.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7170 2024-04-20 14:09:28.000000 libesedb-20240420/libcpath/libcpath_path.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5278 2023-12-03 09:00:45.000000 libesedb-20240420/ChangeLog
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-20 14:34:03.000000 libesedb-20240420/manuals/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2863 2024-04-20 12:01:48.000000 libesedb-20240420/manuals/esedbinfo.1
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      129 2024-04-20 12:13:58.000000 libesedb-20240420/manuals/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17769 2024-04-20 12:01:48.000000 libesedb-20240420/manuals/libesedb.3
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27906 2024-04-20 14:09:58.000000 libesedb-20240420/manuals/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-20 14:34:04.000000 libesedb-20240420/tests/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2790 2024-04-20 12:05:02.000000 libesedb-20240420/tests/esedb_test_space_tree.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3092 2024-04-20 12:05:02.000000 libesedb-20240420/tests/esedb_test_index.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4169 2024-04-20 12:01:48.000000 libesedb-20240420/tests/esedb_test_tools_signal.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      981 2024-04-20 12:01:48.000000 libesedb-20240420/tests/esedb_test_libesedb.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17731 2024-04-20 12:05:02.000000 libesedb-20240420/tests/esedb_test_data_segment.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1444 2024-04-20 12:01:48.000000 libesedb-20240420/tests/esedb_test_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1742 2024-04-20 12:01:48.000000 libesedb-20240420/tests/esedb_test_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20720 2024-04-20 12:01:48.000000 libesedb-20240420/tests/esedb_test_tools_windows_search_compression.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13259 2024-04-20 12:01:48.000000 libesedb-20240420/tests/esedb_test_functions.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3605 2024-04-20 12:05:02.000000 libesedb-20240420/tests/esedb_test_table.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28708 2024-04-20 12:01:47.000000 libesedb-20240420/tests/esedb_test_compression.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29229 2024-04-20 12:01:48.000000 libesedb-20240420/tests/esedb_test_file.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    36143 2024-04-20 12:05:02.000000 libesedb-20240420/tests/esedb_test_catalog_definition.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3340 2024-04-20 12:05:02.000000 libesedb-20240420/tests/pyesedb_test_support.py
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4064 2024-04-20 12:09:46.000000 libesedb-20240420/tests/test_tools.sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1709 2024-04-20 12:01:48.000000 libesedb-20240420/tests/esedb_test_libbfio.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1462 2024-04-20 12:01:48.000000 libesedb-20240420/tests/esedb_test_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   106858 2024-04-20 12:01:47.000000 libesedb-20240420/tests/esedb_test_checksum.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8399 2024-04-20 12:05:02.000000 libesedb-20240420/tests/esedb_test_table_definition.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3139 2024-04-20 12:01:47.000000 libesedb-20240420/tests/esedb_test_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3980 2024-04-20 12:05:02.000000 libesedb-20240420/tests/esedb_test_multi_value.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5349 2024-04-20 12:01:47.000000 libesedb-20240420/tests/pyesedb_test_file.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9212 2024-04-20 12:01:48.000000 libesedb-20240420/tests/esedb_test_space_tree_value.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14768 2024-04-20 13:57:09.000000 libesedb-20240420/tests/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1702 2024-04-20 12:01:48.000000 libesedb-20240420/tests/esedb_test_memory.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1465 2024-04-20 12:01:48.000000 libesedb-20240420/tests/esedb_test_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4703 2024-04-20 12:05:02.000000 libesedb-20240420/tests/esedb_test_record.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14367 2024-04-20 12:01:48.000000 libesedb-20240420/tests/esedb_test_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4323 2024-04-20 12:01:48.000000 libesedb-20240420/tests/esedb_test_notify.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9728 2024-04-20 12:05:02.000000 libesedb-20240420/tests/esedb_test_leaf_page_descriptor.c
+-rwxr--r--   0 lordyesta  (1000) lordyesta  (1000)     1622 2024-04-20 12:01:47.000000 libesedb-20240420/tests/test_manpage.sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5634 2024-04-20 12:01:48.000000 libesedb-20240420/tests/esedb_test_tools_info_handle.c
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4405 2024-04-20 12:01:47.000000 libesedb-20240420/tests/test_python_module.sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23738 2024-04-20 12:05:02.000000 libesedb-20240420/tests/esedb_test_catalog.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1554 2024-04-20 12:01:48.000000 libesedb-20240420/tests/esedb_test_libcdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4700 2024-04-20 12:01:48.000000 libesedb-20240420/tests/esedb_test_memory.c
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4758 2024-04-20 12:10:13.000000 libesedb-20240420/tests/test_esedbexport.sh
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     3289 2024-04-20 12:01:47.000000 libesedb-20240420/tests/test_esedbinfo.sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2447 2024-04-20 12:01:48.000000 libesedb-20240420/tests/esedb_test_tools_output.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3017 2024-04-20 12:05:02.000000 libesedb-20240420/tests/esedb_test_column_type.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6743 2024-04-20 12:05:02.000000 libesedb-20240420/tests/esedb_test_block_tree_node.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33607 2024-04-20 12:01:47.000000 libesedb-20240420/tests/test_runner.sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1545 2024-04-20 12:01:48.000000 libesedb-20240420/tests/esedb_test_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7826 2024-04-20 12:05:02.000000 libesedb-20240420/tests/esedb_test_database.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8181 2024-04-20 12:01:48.000000 libesedb-20240420/tests/esedb_test_io_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19281 2024-04-20 12:05:02.000000 libesedb-20240420/tests/esedb_test_file_header.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9255 2024-04-20 12:01:48.000000 libesedb-20240420/tests/esedb_test_page_tree_value.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4535 2024-04-20 12:01:48.000000 libesedb-20240420/tests/esedb_test_getopt.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1813 2024-04-20 12:01:48.000000 libesedb-20240420/tests/esedb_test_getopt.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1812 2024-04-20 12:01:48.000000 libesedb-20240420/tests/esedb_test_functions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14527 2024-04-20 12:05:02.000000 libesedb-20240420/tests/esedb_test_block_tree.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1447 2024-04-20 12:01:48.000000 libesedb-20240420/tests/esedb_test_libfcache.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1551 2024-04-20 12:01:48.000000 libesedb-20240420/tests/esedb_test_libfdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9553 2024-04-20 12:01:47.000000 libesedb-20240420/tests/esedb_test_data_definition.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    93297 2024-04-20 14:09:58.000000 libesedb-20240420/tests/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9288 2024-04-20 12:01:48.000000 libesedb-20240420/tests/esedb_test_root_page_header.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3378 2024-04-20 12:05:02.000000 libesedb-20240420/tests/esedb_test_long_value.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6011 2024-04-20 12:01:48.000000 libesedb-20240420/tests/esedb_test_page_value.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15037 2024-04-20 12:05:02.000000 libesedb-20240420/tests/esedb_test_page_tree_key.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6476 2024-04-20 12:05:02.000000 libesedb-20240420/tests/esedb_test_block_descriptor.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9078 2024-04-20 12:05:02.000000 libesedb-20240420/tests/esedb_test_page_tree.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    58326 2024-04-20 12:05:02.000000 libesedb-20240420/tests/esedb_test_page.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17919 2024-04-20 12:05:02.000000 libesedb-20240420/tests/esedb_test_page_header.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22535 2024-04-20 12:05:02.000000 libesedb-20240420/tests/esedb_test_column.c
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4398 2024-04-20 12:09:08.000000 libesedb-20240420/tests/test_library.sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8574 2024-04-20 12:01:48.000000 libesedb-20240420/tests/esedb_test_macros.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-20 14:34:04.000000 libesedb-20240420/ossfuzz/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2621 2024-04-20 12:01:44.000000 libesedb-20240420/ossfuzz/table_fuzzer.cc
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      972 2024-04-20 12:01:44.000000 libesedb-20240420/ossfuzz/ossfuzz_libesedb.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2418 2024-04-20 12:14:21.000000 libesedb-20240420/ossfuzz/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3118 2024-04-20 12:01:44.000000 libesedb-20240420/ossfuzz/column_fuzzer.cc
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1739 2024-04-20 12:01:44.000000 libesedb-20240420/ossfuzz/ossfuzz_libbfio.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3095 2024-04-20 12:01:44.000000 libesedb-20240420/ossfuzz/record_fuzzer.cc
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2214 2024-04-20 12:01:44.000000 libesedb-20240420/ossfuzz/file_fuzzer.cc
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    38876 2024-04-20 14:09:58.000000 libesedb-20240420/ossfuzz/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   332808 2024-04-20 14:09:49.000000 libesedb-20240420/ltmain.sh
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-20 14:34:02.000000 libesedb-20240420/libfwnt/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1627 2024-04-20 14:09:41.000000 libesedb-20240420/libfwnt/libfwnt_locale_identifier.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26551 2024-04-20 14:09:41.000000 libesedb-20240420/libfwnt/libfwnt_lzxpress.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1376 2024-04-20 14:09:41.000000 libesedb-20240420/libfwnt/libfwnt_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30230 2024-04-20 14:09:41.000000 libesedb-20240420/libfwnt/libfwnt_security_identifier.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2024-04-20 14:09:41.000000 libesedb-20240420/libfwnt/libfwnt_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7049 2024-04-20 14:09:41.000000 libesedb-20240420/libfwnt/libfwnt_bit_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1772 2024-04-20 14:09:41.000000 libesedb-20240420/libfwnt/libfwnt_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-04-20 14:09:41.000000 libesedb-20240420/libfwnt/libfwnt_lznt1.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2742 2024-04-20 14:09:41.000000 libesedb-20240420/libfwnt/libfwnt_notify.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1344 2024-04-20 14:09:41.000000 libesedb-20240420/libfwnt/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5264 2024-04-20 14:09:41.000000 libesedb-20240420/libfwnt/libfwnt_security_identifier.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1185 2024-04-20 14:09:41.000000 libesedb-20240420/libfwnt/libfwnt_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2072 2024-04-20 14:09:41.000000 libesedb-20240420/libfwnt/libfwnt_huffman_tree.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2896 2024-04-20 14:09:41.000000 libesedb-20240420/libfwnt/libfwnt_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2795 2024-04-20 14:09:41.000000 libesedb-20240420/libfwnt/libfwnt_access_control_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27064 2024-04-20 14:09:41.000000 libesedb-20240420/libfwnt/libfwnt_security_descriptor.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13639 2024-04-20 14:09:41.000000 libesedb-20240420/libfwnt/libfwnt_access_control_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3470 2024-04-20 14:09:41.000000 libesedb-20240420/libfwnt/libfwnt_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13113 2024-04-20 14:09:41.000000 libesedb-20240420/libfwnt/libfwnt_huffman_tree.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8377 2024-04-20 14:09:41.000000 libesedb-20240420/libfwnt/libfwnt_debug.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15166 2024-04-20 14:09:41.000000 libesedb-20240420/libfwnt/libfwnt_lznt1.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1578 2024-04-20 14:09:41.000000 libesedb-20240420/libfwnt/libfwnt_notify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18859 2024-04-20 14:09:41.000000 libesedb-20240420/libfwnt/libfwnt_locale_identifier.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1464 2024-04-20 14:09:41.000000 libesedb-20240420/libfwnt/libfwnt_debug.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1545 2024-04-20 14:09:41.000000 libesedb-20240420/libfwnt/libfwnt_libcdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2797 2024-04-20 14:09:41.000000 libesedb-20240420/libfwnt/libfwnt_lzx.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2024-04-20 14:09:41.000000 libesedb-20240420/libfwnt/libfwnt_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1453 2024-04-20 14:09:41.000000 libesedb-20240420/libfwnt/libfwnt_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19962 2024-04-20 14:09:41.000000 libesedb-20240420/libfwnt/libfwnt_access_control_entry.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2326 2024-04-20 14:09:41.000000 libesedb-20240420/libfwnt/libfwnt_lzxpress.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3336 2024-04-20 14:09:41.000000 libesedb-20240420/libfwnt/libfwnt_security_descriptor.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    36036 2024-04-20 14:09:41.000000 libesedb-20240420/libfwnt/libfwnt_lzx.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35251 2024-04-20 14:09:58.000000 libesedb-20240420/libfwnt/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2039 2024-04-20 14:09:41.000000 libesedb-20240420/libfwnt/libfwnt_bit_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1908 2024-04-20 14:09:41.000000 libesedb-20240420/libfwnt/libfwnt_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1129 2024-04-20 14:09:41.000000 libesedb-20240420/libfwnt/libfwnt_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3209 2024-04-20 14:09:41.000000 libesedb-20240420/libfwnt/libfwnt_access_control_entry.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-20 14:34:01.000000 libesedb-20240420/libcsplit/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6125 2024-04-20 14:09:30.000000 libesedb-20240420/libcsplit/libcsplit_narrow_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1360 2024-04-20 14:09:30.000000 libesedb-20240420/libcsplit/libcsplit_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1679 2024-04-20 14:09:30.000000 libesedb-20240420/libcsplit/libcsplit_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13944 2024-04-20 14:09:30.000000 libesedb-20240420/libcsplit/libcsplit_wide_split_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2024-04-20 14:09:30.000000 libesedb-20240420/libcsplit/libcsplit_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      880 2024-04-20 14:09:30.000000 libesedb-20240420/libcsplit/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-04-20 14:09:30.000000 libesedb-20240420/libcsplit/libcsplit_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6206 2024-04-20 14:09:30.000000 libesedb-20240420/libcsplit/libcsplit_wide_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-04-20 14:09:30.000000 libesedb-20240420/libcsplit/libcsplit_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2920 2024-04-20 14:09:30.000000 libesedb-20240420/libcsplit/libcsplit_wide_split_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2924 2024-04-20 14:09:30.000000 libesedb-20240420/libcsplit/libcsplit_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13912 2024-04-20 14:09:30.000000 libesedb-20240420/libcsplit/libcsplit_narrow_split_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-04-20 14:09:30.000000 libesedb-20240420/libcsplit/libcsplit_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-04-20 14:09:30.000000 libesedb-20240420/libcsplit/libcsplit_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1158 2024-04-20 14:09:30.000000 libesedb-20240420/libcsplit/libcsplit_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1471 2024-04-20 14:09:30.000000 libesedb-20240420/libcsplit/libcsplit_wide_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32069 2024-04-20 14:09:57.000000 libesedb-20240420/libcsplit/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2849 2024-04-20 14:09:30.000000 libesedb-20240420/libcsplit/libcsplit_narrow_split_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1386 2024-04-20 14:09:30.000000 libesedb-20240420/libcsplit/libcsplit_narrow_string.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-20 14:34:03.000000 libesedb-20240420/po/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      720 2023-12-03 09:01:06.000000 libesedb-20240420/po/remove-potcdate.sin
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       59 2023-12-03 09:01:06.000000 libesedb-20240420/po/POTFILES.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19571 2023-12-03 09:01:06.000000 libesedb-20240420/po/Makefile.in.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      153 2023-12-03 09:01:06.000000 libesedb-20240420/po/quot.sed
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1204 2023-12-03 09:01:06.000000 libesedb-20240420/po/en@quot.header
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1338 2023-12-03 09:01:06.000000 libesedb-20240420/po/en@boldquot.header
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      217 2023-12-03 09:01:06.000000 libesedb-20240420/po/boldquot.sed
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      906 2023-12-03 09:01:06.000000 libesedb-20240420/po/insert-header.sin
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       50 2023-12-03 09:01:06.000000 libesedb-20240420/po/ChangeLog
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1854 2024-04-20 14:10:10.000000 libesedb-20240420/po/Makevars
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1852 2023-12-03 09:01:06.000000 libesedb-20240420/po/Makevars.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2395 2023-12-03 09:01:06.000000 libesedb-20240420/po/Rules-quot
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-20 14:34:01.000000 libesedb-20240420/libuna/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8811 2024-04-20 14:09:45.000000 libesedb-20240420/libuna/libuna_codepage_windows_1251.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    98308 2024-04-20 14:09:45.000000 libesedb-20240420/libuna/libuna_utf16_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39461 2024-04-20 14:09:45.000000 libesedb-20240420/libuna/libuna_base16_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2993 2024-04-20 14:09:45.000000 libesedb-20240420/libuna/libuna_utf8_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1567 2024-04-20 14:09:45.000000 libesedb-20240420/libuna/libuna_codepage_iso_8859_2.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   286239 2024-04-20 14:09:45.000000 libesedb-20240420/libuna/libuna_codepage_windows_932.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-04-20 14:09:45.000000 libesedb-20240420/libuna/libuna_codepage_mac_dingbats.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   101450 2024-04-20 14:09:45.000000 libesedb-20240420/libuna/libuna_utf8_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    74767 2024-04-20 14:09:45.000000 libesedb-20240420/libuna/libuna_base64_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1749 2024-04-20 14:09:45.000000 libesedb-20240420/libuna/libuna_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1610 2024-04-20 14:09:45.000000 libesedb-20240420/libuna/libuna_codepage_mac_turkish.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   156918 2024-04-20 14:09:45.000000 libesedb-20240420/libuna/libuna_unicode_character.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10379 2024-04-20 14:09:45.000000 libesedb-20240420/libuna/libuna_codepage_mac_gaelic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-04-20 14:09:45.000000 libesedb-20240420/libuna/libuna_codepage_mac_arabic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9435 2024-04-20 14:09:45.000000 libesedb-20240420/libuna/libuna_codepage_mac_thai.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1618 2024-04-20 14:09:45.000000 libesedb-20240420/libuna/libuna_codepage_windows_874.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1346 2024-04-20 14:09:45.000000 libesedb-20240420/libuna/libuna_codepage_iso_8859_15.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9666 2024-04-20 14:09:45.000000 libesedb-20240420/libuna/libuna_utf8_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3296 2024-04-20 14:09:45.000000 libesedb-20240420/libuna/libuna_codepage_iso_8859_16.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9211 2024-04-20 14:09:45.000000 libesedb-20240420/libuna/libuna_codepage_windows_1255.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15691 2024-04-20 14:09:45.000000 libesedb-20240420/libuna/libuna_utf7_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2921 2024-04-20 14:09:45.000000 libesedb-20240420/libuna/libuna_byte_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9984 2024-04-20 14:09:45.000000 libesedb-20240420/libuna/libuna_codepage_koi8_u.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1392 2024-04-20 14:09:45.000000 libesedb-20240420/libuna/libuna_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2540 2024-04-20 14:09:45.000000 libesedb-20240420/libuna/libuna_codepage_iso_8859_6.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2823 2024-04-20 14:09:45.000000 libesedb-20240420/libuna/libuna_codepage_iso_8859_14.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3679 2024-04-20 14:09:45.000000 libesedb-20240420/libuna/libuna_base64_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2882 2024-04-20 14:09:45.000000 libesedb-20240420/libuna/libuna_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1658 2024-04-20 14:09:45.000000 libesedb-20240420/libuna/libuna_codepage_mac_centraleurroman.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9953 2024-04-20 14:09:45.000000 libesedb-20240420/libuna/libuna_codepage_mac_romanian.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1339 2024-04-20 14:09:45.000000 libesedb-20240420/libuna/libuna_codepage_iso_8859_6.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2053 2024-04-20 14:09:45.000000 libesedb-20240420/libuna/libuna_codepage_iso_8859_9.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1610 2024-04-20 14:09:45.000000 libesedb-20240420/libuna/libuna_codepage_mac_russian.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10134 2024-04-20 14:09:45.000000 libesedb-20240420/libuna/libuna_codepage_mac_dingbats.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2024-04-20 14:09:45.000000 libesedb-20240420/libuna/libuna_codepage_iso_8859_15.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   430461 2024-04-20 14:09:45.000000 libesedb-20240420/libuna/libuna_codepage_windows_936.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-04-20 14:09:45.000000 libesedb-20240420/libuna/libuna_codepage_mac_croatian.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1259 2024-04-20 14:09:45.000000 libesedb-20240420/libuna/libuna_scsu.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4193 2024-04-20 14:09:45.000000 libesedb-20240420/libuna/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20049 2024-04-20 14:09:45.000000 libesedb-20240420/libuna/libuna_utf32_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1830 2024-04-20 14:09:45.000000 libesedb-20240420/libuna/libuna_codepage_windows_936.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3225 2024-04-20 14:09:45.000000 libesedb-20240420/libuna/libuna_codepage_iso_8859_10.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9745 2024-04-20 14:09:45.000000 libesedb-20240420/libuna/libuna_codepage_mac_roman.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2808 2024-04-20 14:09:45.000000 libesedb-20240420/libuna/libuna_utf7_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1773 2024-04-20 14:09:45.000000 libesedb-20240420/libuna/libuna_codepage_iso_8859_3.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1787 2024-04-20 14:09:45.000000 libesedb-20240420/libuna/libuna_codepage_mac_thai.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-04-20 14:09:45.000000 libesedb-20240420/libuna/libuna_codepage_mac_farsi.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9088 2024-04-20 14:09:45.000000 libesedb-20240420/libuna/libuna_codepage_mac_ukrainian.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10880 2024-04-20 14:09:45.000000 libesedb-20240420/libuna/libuna_codepage_mac_inuit.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1830 2024-04-20 14:09:45.000000 libesedb-20240420/libuna/libuna_codepage_windows_932.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8050 2024-04-20 14:09:45.000000 libesedb-20240420/libuna/libuna_codepage_windows_874.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2738 2024-04-20 14:09:45.000000 libesedb-20240420/libuna/libuna_codepage_iso_8859_5.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-04-20 14:09:45.000000 libesedb-20240420/libuna/libuna_codepage_iso_8859_10.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16705 2024-04-20 14:09:45.000000 libesedb-20240420/libuna/libuna_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1929 2024-04-20 14:09:45.000000 libesedb-20240420/libuna/libuna_url_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1622 2024-04-20 14:09:45.000000 libesedb-20240420/libuna/libuna_codepage_mac_icelandic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1602 2024-04-20 14:09:45.000000 libesedb-20240420/libuna/libuna_codepage_koi8_u.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19850 2024-04-20 14:09:45.000000 libesedb-20240420/libuna/libuna_utf16_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8602 2024-04-20 14:09:45.000000 libesedb-20240420/libuna/libuna_codepage_windows_1253.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1449 2024-04-20 14:09:45.000000 libesedb-20240420/libuna/libuna_codepage_iso_8859_4.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9078 2024-04-20 14:09:45.000000 libesedb-20240420/libuna/libuna_codepage_mac_greek.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-04-20 14:09:45.000000 libesedb-20240420/libuna/libuna_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9394 2024-04-20 14:09:45.000000 libesedb-20240420/libuna/libuna_codepage_mac_centraleurroman.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8997 2024-04-20 14:09:45.000000 libesedb-20240420/libuna/libuna_codepage_windows_1254.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1455 2024-04-20 14:09:45.000000 libesedb-20240420/libuna/libuna_codepage_iso_8859_13.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1447 2024-04-20 14:09:45.000000 libesedb-20240420/libuna/libuna_codepage_iso_8859_7.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-04-20 14:09:45.000000 libesedb-20240420/libuna/libuna_codepage_windows_1255.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8000 2024-04-20 14:09:45.000000 libesedb-20240420/libuna/libuna_unicode_character.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1448 2024-04-20 14:09:45.000000 libesedb-20240420/libuna/libuna_codepage_iso_8859_8.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3664 2024-04-20 14:09:45.000000 libesedb-20240420/libuna/libuna_codepage_iso_8859_13.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-04-20 14:09:45.000000 libesedb-20240420/libuna/libuna_codepage_windows_949.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9125 2024-04-20 14:09:45.000000 libesedb-20240420/libuna/libuna_codepage_mac_cyrillic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9871 2024-04-20 14:09:45.000000 libesedb-20240420/libuna/libuna_codepage_mac_celtic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1234 2024-04-20 14:09:45.000000 libesedb-20240420/libuna/libuna_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3561 2024-04-20 14:09:45.000000 libesedb-20240420/libuna/libuna_codepage_iso_8859_4.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   484762 2024-04-20 14:09:45.000000 libesedb-20240420/libuna/libuna_codepage_windows_949.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3106 2024-04-20 14:09:45.000000 libesedb-20240420/libuna/libuna_utf16_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14020 2024-04-20 14:09:45.000000 libesedb-20240420/libuna/libuna_codepage_mac_symbol.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-04-20 14:09:45.000000 libesedb-20240420/libuna/libuna_codepage_mac_roman.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9076 2024-04-20 14:09:45.000000 libesedb-20240420/libuna/libuna_codepage_windows_1257.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1627 2024-04-20 14:09:45.000000 libesedb-20240420/libuna/libuna_codepage_windows_1254.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   360710 2024-04-20 14:09:45.000000 libesedb-20240420/libuna/libuna_codepage_windows_950.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1363 2024-04-20 14:09:45.000000 libesedb-20240420/libuna/libuna_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10005 2024-04-20 14:09:45.000000 libesedb-20240420/libuna/libuna_codepage_windows_1256.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1521 2024-04-20 14:09:45.000000 libesedb-20240420/libuna/libuna_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3704 2024-04-20 14:09:45.000000 libesedb-20240420/libuna/libuna_base32_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1625 2024-04-20 14:09:45.000000 libesedb-20240420/libuna/libuna_codepage_windows_1253.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1783 2024-04-20 14:09:45.000000 libesedb-20240420/libuna/libuna_codepage_iso_8859_16.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18019 2024-04-20 14:09:45.000000 libesedb-20240420/libuna/libuna_utf8_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1636 2024-04-20 14:09:45.000000 libesedb-20240420/libuna/libuna_codepage_windows_1250.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3610 2024-04-20 14:09:45.000000 libesedb-20240420/libuna/libuna_codepage_iso_8859_2.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1140 2024-04-20 14:09:45.000000 libesedb-20240420/libuna/libuna_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9542 2024-04-20 14:09:45.000000 libesedb-20240420/libuna/libuna_codepage_koi8_r.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1341 2024-04-20 14:09:45.000000 libesedb-20240420/libuna/libuna_codepage_iso_8859_5.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9656 2024-04-20 14:09:45.000000 libesedb-20240420/libuna/libuna_utf16_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    94606 2024-04-20 14:09:45.000000 libesedb-20240420/libuna/libuna_utf32_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9656 2024-04-20 14:09:45.000000 libesedb-20240420/libuna/libuna_codepage_mac_icelandic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-04-20 14:09:45.000000 libesedb-20240420/libuna/libuna_codepage_windows_1256.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9526 2024-04-20 14:09:45.000000 libesedb-20240420/libuna/libuna_utf32_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-04-20 14:09:45.000000 libesedb-20240420/libuna/libuna_codepage_mac_romanian.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2629 2024-04-20 14:09:45.000000 libesedb-20240420/libuna/libuna_codepage_iso_8859_8.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1600 2024-04-20 14:09:45.000000 libesedb-20240420/libuna/libuna_codepage_koi8_r.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-04-20 14:09:45.000000 libesedb-20240420/libuna/libuna_codepage_mac_cyrillic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10389 2024-04-20 14:09:45.000000 libesedb-20240420/libuna/libuna_codepage_mac_arabic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9776 2024-04-20 14:09:45.000000 libesedb-20240420/libuna/libuna_codepage_mac_croatian.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1340 2024-04-20 14:09:45.000000 libesedb-20240420/libuna/libuna_codepage_iso_8859_9.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-04-20 14:09:45.000000 libesedb-20240420/libuna/libuna_codepage_mac_greek.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1630 2024-04-20 14:09:45.000000 libesedb-20240420/libuna/libuna_codepage_windows_1258.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2873 2024-04-20 14:09:45.000000 libesedb-20240420/libuna/libuna_codepage_iso_8859_7.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    57653 2024-04-20 14:09:58.000000 libesedb-20240420/libuna/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3335 2024-04-20 14:09:45.000000 libesedb-20240420/libuna/libuna_codepage_iso_8859_3.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9776 2024-04-20 14:09:45.000000 libesedb-20240420/libuna/libuna_codepage_windows_1250.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3181 2024-04-20 14:09:45.000000 libesedb-20240420/libuna/libuna_scsu.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7189 2024-04-20 14:09:45.000000 libesedb-20240420/libuna/libuna_codepage_windows_1252.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9844 2024-04-20 14:09:45.000000 libesedb-20240420/libuna/libuna_codepage_mac_turkish.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1622 2024-04-20 14:09:45.000000 libesedb-20240420/libuna/libuna_codepage_mac_ukrainian.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8997 2024-04-20 14:09:45.000000 libesedb-20240420/libuna/libuna_codepage_mac_russian.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9116 2024-04-20 14:09:45.000000 libesedb-20240420/libuna/libuna_codepage_windows_1258.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-04-20 14:09:45.000000 libesedb-20240420/libuna/libuna_codepage_mac_celtic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15485 2024-04-20 14:09:45.000000 libesedb-20240420/libuna/libuna_byte_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-04-20 14:09:45.000000 libesedb-20240420/libuna/libuna_codepage_mac_gaelic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3106 2024-04-20 14:09:45.000000 libesedb-20240420/libuna/libuna_utf32_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1801 2024-04-20 14:09:45.000000 libesedb-20240420/libuna/libuna_codepage_mac_symbol.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-04-20 14:09:45.000000 libesedb-20240420/libuna/libuna_codepage_windows_1257.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-04-20 14:09:45.000000 libesedb-20240420/libuna/libuna_codepage_mac_inuit.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11002 2024-04-20 14:09:45.000000 libesedb-20240420/libuna/libuna_codepage_mac_farsi.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2024-04-20 14:09:45.000000 libesedb-20240420/libuna/libuna_codepage_windows_950.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15532 2024-04-20 14:09:45.000000 libesedb-20240420/libuna/libuna_url_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1628 2024-04-20 14:09:45.000000 libesedb-20240420/libuna/libuna_codepage_windows_1251.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1644 2024-04-20 14:09:45.000000 libesedb-20240420/libuna/libuna_codepage_windows_1252.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1563 2024-04-20 14:09:45.000000 libesedb-20240420/libuna/libuna_codepage_iso_8859_14.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2623 2024-04-20 14:09:45.000000 libesedb-20240420/libuna/libuna_base16_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    82226 2024-04-20 14:09:45.000000 libesedb-20240420/libuna/libuna_base32_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    42036 2024-04-20 14:09:57.000000 libesedb-20240420/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-20 14:34:02.000000 libesedb-20240420/libfvalue/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2913 2024-04-20 14:09:39.000000 libesedb-20240420/libfvalue/libfvalue_filetime.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6390 2024-04-20 14:09:39.000000 libesedb-20240420/libfvalue/libfvalue_utf16_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1707 2024-04-20 14:09:39.000000 libesedb-20240420/libfvalue/libfvalue_libfwnt.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   125143 2024-04-20 14:09:39.000000 libesedb-20240420/libfvalue/libfvalue_value.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20255 2024-04-20 14:09:39.000000 libesedb-20240420/libfvalue/libfvalue_value.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10693 2024-04-20 14:09:39.000000 libesedb-20240420/libfvalue/libfvalue_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3267 2024-04-20 14:09:39.000000 libesedb-20240420/libfvalue/libfvalue_codepage.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14234 2024-04-20 14:09:39.000000 libesedb-20240420/libfvalue/libfvalue_split_utf16_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2924 2024-04-20 14:09:39.000000 libesedb-20240420/libfvalue/libfvalue_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6349 2024-04-20 14:09:39.000000 libesedb-20240420/libfvalue/libfvalue_utf8_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-04-20 14:09:39.000000 libesedb-20240420/libfvalue/libfvalue_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3075 2024-04-20 14:09:39.000000 libesedb-20240420/libfvalue/libfvalue_split_utf16_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1629 2024-04-20 14:09:39.000000 libesedb-20240420/libfvalue/libfvalue_filetime.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1139 2024-04-20 14:09:39.000000 libesedb-20240420/libfvalue/libfvalue_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-04-20 14:09:39.000000 libesedb-20240420/libfvalue/libfvalue_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1702 2024-04-20 14:09:39.000000 libesedb-20240420/libfvalue/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2831 2024-04-20 14:09:39.000000 libesedb-20240420/libfvalue/libfvalue_value_type.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-04-20 14:09:39.000000 libesedb-20240420/libfvalue/libfvalue_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13854 2024-04-20 14:09:39.000000 libesedb-20240420/libfvalue/libfvalue_split_utf8_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5127 2024-04-20 14:09:39.000000 libesedb-20240420/libfvalue/libfvalue_data_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1379 2024-04-20 14:09:39.000000 libesedb-20240420/libfvalue/libfvalue_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    40414 2024-04-20 14:09:39.000000 libesedb-20240420/libfvalue/libfvalue_data_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    70736 2024-04-20 14:09:39.000000 libesedb-20240420/libfvalue/libfvalue_integer.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39827 2024-04-20 14:09:39.000000 libesedb-20240420/libfvalue/libfvalue_value_type.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7448 2024-04-20 14:09:39.000000 libesedb-20240420/libfvalue/libfvalue_integer.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3264 2024-04-20 14:09:39.000000 libesedb-20240420/libfvalue/libfvalue_binary_data.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1665 2024-04-20 14:09:39.000000 libesedb-20240420/libfvalue/libfvalue_value_entry.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1427 2024-04-20 14:09:39.000000 libesedb-20240420/libfvalue/libfvalue_utf16_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-04-20 14:09:39.000000 libesedb-20240420/libfvalue/libfvalue_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3515 2024-04-20 14:09:39.000000 libesedb-20240420/libfvalue/libfvalue_table.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1495 2024-04-20 14:09:39.000000 libesedb-20240420/libfvalue/libfvalue_libfguid.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3040 2024-04-20 14:09:39.000000 libesedb-20240420/libfvalue/libfvalue_split_utf8_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7626 2024-04-20 14:09:39.000000 libesedb-20240420/libfvalue/libfvalue_floating_point.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2024-04-20 14:09:39.000000 libesedb-20240420/libfvalue/libfvalue_libfdatetime.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4451 2024-04-20 14:09:39.000000 libesedb-20240420/libfvalue/libfvalue_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39905 2024-04-20 14:09:39.000000 libesedb-20240420/libfvalue/libfvalue_binary_data.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4662 2024-04-20 14:09:39.000000 libesedb-20240420/libfvalue/libfvalue_value_entry.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1551 2024-04-20 14:09:39.000000 libesedb-20240420/libfvalue/libfvalue_libcdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1199 2024-04-20 14:09:39.000000 libesedb-20240420/libfvalue/libfvalue_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32203 2024-04-20 14:09:39.000000 libesedb-20240420/libfvalue/libfvalue_table.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37011 2024-04-20 14:09:58.000000 libesedb-20240420/libfvalue/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1417 2024-04-20 14:09:39.000000 libesedb-20240420/libfvalue/libfvalue_utf8_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    84529 2024-04-20 14:09:39.000000 libesedb-20240420/libfvalue/libfvalue_floating_point.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1964 2024-04-20 14:09:39.000000 libesedb-20240420/libfvalue/libfvalue_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    73330 2024-04-20 14:09:39.000000 libesedb-20240420/libfvalue/libfvalue_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1739 2024-04-20 14:09:39.000000 libesedb-20240420/libfvalue/libfvalue_libuna.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-20 14:34:01.000000 libesedb-20240420/libcnotify/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1548 2024-04-20 14:09:27.000000 libesedb-20240420/libcnotify/libcnotify_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1415 2024-04-20 14:09:27.000000 libesedb-20240420/libcnotify/libcnotify_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1164 2024-04-20 14:09:27.000000 libesedb-20240420/libcnotify/libcnotify_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1439 2024-04-20 14:09:27.000000 libesedb-20240420/libcnotify/libcnotify_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      724 2024-04-20 14:09:27.000000 libesedb-20240420/libcnotify/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2024-04-20 14:09:27.000000 libesedb-20240420/libcnotify/libcnotify_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1290 2024-04-20 14:09:27.000000 libesedb-20240420/libcnotify/libcnotify_verbose.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1722 2024-04-20 14:09:27.000000 libesedb-20240420/libcnotify/libcnotify_print.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4018 2024-04-20 14:09:27.000000 libesedb-20240420/libcnotify/libcnotify_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1266 2024-04-20 14:09:27.000000 libesedb-20240420/libcnotify/libcnotify_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1094 2024-04-20 14:09:27.000000 libesedb-20240420/libcnotify/libcnotify_verbose.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31010 2024-04-20 14:09:57.000000 libesedb-20240420/libcnotify/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1365 2024-04-20 14:09:27.000000 libesedb-20240420/libcnotify/libcnotify_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8166 2024-04-20 14:09:27.000000 libesedb-20240420/libcnotify/libcnotify_print.c
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-20 14:34:01.000000 libesedb-20240420/libcerror/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15420 2024-04-20 14:09:23.000000 libesedb-20240420/libcerror/libcerror_system.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19408 2024-04-20 14:09:23.000000 libesedb-20240420/libcerror/libcerror_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-04-20 14:09:23.000000 libesedb-20240420/libcerror/libcerror_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      636 2024-04-20 14:09:23.000000 libesedb-20240420/libcerror/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1522 2024-04-20 14:09:23.000000 libesedb-20240420/libcerror/libcerror_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2024-04-20 14:09:23.000000 libesedb-20240420/libcerror/libcerror_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2880 2024-04-20 14:09:23.000000 libesedb-20240420/libcerror/libcerror_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2026 2024-04-20 14:09:23.000000 libesedb-20240420/libcerror/libcerror_system.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7629 2024-04-20 14:09:23.000000 libesedb-20240420/libcerror/libcerror_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1158 2024-04-20 14:09:23.000000 libesedb-20240420/libcerror/libcerror_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-04-20 14:09:23.000000 libesedb-20240420/libcerror/libcerror_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30477 2024-04-20 14:09:57.000000 libesedb-20240420/libcerror/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3662 2024-04-20 12:01:39.000000 libesedb-20240420/libesedb.spec.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-20 14:34:02.000000 libesedb-20240420/libfdatetime/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5406 2024-04-20 14:09:35.000000 libesedb-20240420/libfdatetime/libfdatetime_floatingtime.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34352 2024-04-20 14:09:35.000000 libesedb-20240420/libfdatetime/libfdatetime_nsf_timedate.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1887 2024-04-20 14:09:35.000000 libesedb-20240420/libfdatetime/libfdatetime_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33399 2024-04-20 14:09:35.000000 libesedb-20240420/libfdatetime/libfdatetime_floatingtime.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1220 2024-04-20 14:09:35.000000 libesedb-20240420/libfdatetime/libfdatetime_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5010 2024-04-20 14:09:35.000000 libesedb-20240420/libfdatetime/libfdatetime_hfs_time.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4182 2024-04-20 14:09:35.000000 libesedb-20240420/libfdatetime/libfdatetime_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31774 2024-04-20 14:09:35.000000 libesedb-20240420/libfdatetime/libfdatetime_hfs_time.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1144 2024-04-20 14:09:35.000000 libesedb-20240420/libfdatetime/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35109 2024-04-20 14:09:35.000000 libesedb-20240420/libfdatetime/libfdatetime_filetime.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4993 2024-04-20 14:09:35.000000 libesedb-20240420/libfdatetime/libfdatetime_systemtime.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-04-20 14:09:35.000000 libesedb-20240420/libfdatetime/libfdatetime_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    50166 2024-04-20 14:09:35.000000 libesedb-20240420/libfdatetime/libfdatetime_posix_time.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1440 2024-04-20 14:09:35.000000 libesedb-20240420/libfdatetime/libfdatetime_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5342 2024-04-20 14:09:35.000000 libesedb-20240420/libfdatetime/libfdatetime_fat_date_time.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    41822 2024-04-20 14:09:35.000000 libesedb-20240420/libfdatetime/libfdatetime_systemtime.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5761 2024-04-20 14:09:35.000000 libesedb-20240420/libfdatetime/libfdatetime_nsf_timedate.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1450 2024-04-20 14:09:35.000000 libesedb-20240420/libfdatetime/libfdatetime_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1154 2024-04-20 14:09:35.000000 libesedb-20240420/libfdatetime/libfdatetime_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2966 2024-04-20 14:09:35.000000 libesedb-20240420/libfdatetime/libfdatetime_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5771 2024-04-20 14:09:35.000000 libesedb-20240420/libfdatetime/libfdatetime_posix_time.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3131 2024-04-20 14:09:35.000000 libesedb-20240420/libfdatetime/libfdatetime_date_time_values.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5340 2024-04-20 14:09:35.000000 libesedb-20240420/libfdatetime/libfdatetime_filetime.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    53085 2024-04-20 14:09:35.000000 libesedb-20240420/libfdatetime/libfdatetime_date_time_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2468 2024-04-20 14:09:35.000000 libesedb-20240420/libfdatetime/libfdatetime_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34061 2024-04-20 14:09:57.000000 libesedb-20240420/libfdatetime/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31754 2024-04-20 14:09:35.000000 libesedb-20240420/libfdatetime/libfdatetime_fat_date_time.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    56915 2024-04-20 14:09:53.000000 libesedb-20240420/aclocal.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8475 2024-04-20 12:01:39.000000 libesedb-20240420/configure.ac
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      418 2024-04-20 14:34:05.071900 libesedb-20240420/PKG-INFO
```

### Comparing `libesedb-20240202/libfdata/libfdata_error.h` & `libesedb-20240420/libfdata/libfdata_error.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfdata/libfdata_area.c` & `libesedb-20240420/libfdata/libfdata_area.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfdata/libfdata_stream.h` & `libesedb-20240420/libfdata/libfdata_stream.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfdata/libfdata_cache.h` & `libesedb-20240420/libfdata/libfdata_cache.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfdata/libfdata_range_list.c` & `libesedb-20240420/libfdata/libfdata_range_list.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfdata/libfdata_mapped_range.c` & `libesedb-20240420/libfdata/libfdata_mapped_range.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfdata/libfdata_libcerror.h` & `libesedb-20240420/libfdata/libfdata_libcerror.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfdata/libfdata_definitions.h` & `libesedb-20240420/libfdata/libfdata_definitions.h`

 * *Files 0% similar despite different names*

```diff
@@ -29,19 +29,19 @@
 #if !defined( HAVE_LOCAL_LIBFDATA )
 #include <libfdata/definitions.h>
 
 /* The definitions in <libfdata/definitions.h> are copied here
  * for local use of libfdata
  */
 #else
-#define LIBFDATA_VERSION						20240114
+#define LIBFDATA_VERSION						20240415
 
 /* The libfdata version string
  */
-#define LIBFDATA_VERSION_STRING						"20240114"
+#define LIBFDATA_VERSION_STRING						"20240415"
 
 /* The library flag definitions
  */
 enum LIBFDATA_FLAGS
 {
 	/* The data is not managed by the library
 	 */
```

### Comparing `libesedb-20240202/libfdata/libfdata_list.c` & `libesedb-20240420/libfdata/libfdata_list.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfdata/libfdata_libcdata.h` & `libesedb-20240420/libfdata/libfdata_libcdata.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfdata/libfdata_list.h` & `libesedb-20240420/libfdata/libfdata_list.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfdata/libfdata_list_element.h` & `libesedb-20240420/libfdata/libfdata_list_element.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfdata/Makefile.am` & `libesedb-20240420/libfdata/Makefile.am`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBFDATA
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCTHREADS_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBFCACHE_CPPFLAGS@ \
 	@PTHREAD_CPPFLAGS@ 
 
@@ -31,19 +31,17 @@
 	libfdata_stream.c libfdata_stream.h \
 	libfdata_support.c libfdata_support.h \
 	libfdata_types.h \
 	libfdata_unused.h \
 	libfdata_vector.c libfdata_vector.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libfdata ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfdata_la_SOURCES)
```

### Comparing `libesedb-20240202/libfdata/libfdata_libcnotify.h` & `libesedb-20240420/libfdata/libfdata_libcnotify.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfdata/libfdata_extern.h` & `libesedb-20240420/libfdata/libfdata_extern.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfdata/libfdata_notify.c` & `libesedb-20240420/libfdata/libfdata_notify.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfdata/libfdata_cache.c` & `libesedb-20240420/libfdata/libfdata_cache.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfdata/libfdata_stream.c` & `libesedb-20240420/libfdata/libfdata_stream.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfdata/libfdata_unused.h` & `libesedb-20240420/libfdata/libfdata_unused.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfdata/libfdata_range.h` & `libesedb-20240420/libfdata/libfdata_range.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfdata/libfdata_area.h` & `libesedb-20240420/libfdata/libfdata_area.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfdata/libfdata_error.c` & `libesedb-20240420/libfdata/libfdata_error.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfdata/libfdata_support.h` & `libesedb-20240420/libfdata/libfdata_support.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfdata/libfdata_range.c` & `libesedb-20240420/libfdata/libfdata_range.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfdata/libfdata_mapped_range.h` & `libesedb-20240420/libfdata/libfdata_mapped_range.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfdata/libfdata_support.c` & `libesedb-20240420/libfdata/libfdata_support.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfdata/libfdata_list_element.c` & `libesedb-20240420/libfdata/libfdata_list_element.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfdata/libfdata_segments_array.c` & `libesedb-20240420/libfdata/libfdata_segments_array.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfdata/libfdata_types.h` & `libesedb-20240420/libfdata/libfdata_types.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfdata/libfdata_notify.h` & `libesedb-20240420/libfdata/libfdata_notify.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfdata/libfdata_range_list.h` & `libesedb-20240420/libfdata/libfdata_range_list.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfdata/libfdata_segments_array.h` & `libesedb-20240420/libfdata/libfdata_segments_array.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfdata/Makefile.in` & `libesedb-20240420/libfdata/Makefile.in`

 * *Files 3% similar despite different names*

```diff
@@ -564,16 +564,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBFDATA_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBFDATA_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBFDATA_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBFDATA_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBFDATA_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBFDATA_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFDATA_TRUE@	@LIBCTHREADS_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFDATA_TRUE@	@LIBCDATA_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFDATA_TRUE@	@LIBCNOTIFY_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFDATA_TRUE@	@LIBFCACHE_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFDATA_TRUE@	@PTHREAD_CPPFLAGS@ 
 
@@ -597,15 +597,16 @@
 @HAVE_LOCAL_LIBFDATA_TRUE@	libfdata_segments_array.c libfdata_segments_array.h \
 @HAVE_LOCAL_LIBFDATA_TRUE@	libfdata_stream.c libfdata_stream.h \
 @HAVE_LOCAL_LIBFDATA_TRUE@	libfdata_support.c libfdata_support.h \
 @HAVE_LOCAL_LIBFDATA_TRUE@	libfdata_types.h \
 @HAVE_LOCAL_LIBFDATA_TRUE@	libfdata_unused.h \
 @HAVE_LOCAL_LIBFDATA_TRUE@	libfdata_vector.c libfdata_vector.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -817,24 +818,39 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libfdata_area.Plo
+	-rm -f ./$(DEPDIR)/libfdata_cache.Plo
+	-rm -f ./$(DEPDIR)/libfdata_error.Plo
+	-rm -f ./$(DEPDIR)/libfdata_list.Plo
+	-rm -f ./$(DEPDIR)/libfdata_list_element.Plo
+	-rm -f ./$(DEPDIR)/libfdata_mapped_range.Plo
+	-rm -f ./$(DEPDIR)/libfdata_notify.Plo
+	-rm -f ./$(DEPDIR)/libfdata_range.Plo
+	-rm -f ./$(DEPDIR)/libfdata_range_list.Plo
+	-rm -f ./$(DEPDIR)/libfdata_segments_array.Plo
+	-rm -f ./$(DEPDIR)/libfdata_stream.Plo
+	-rm -f ./$(DEPDIR)/libfdata_support.Plo
+	-rm -f ./$(DEPDIR)/libfdata_vector.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -930,17 +946,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libfdata ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfdata_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libesedb-20240202/libfdata/libfdata_vector.c` & `libesedb-20240420/libfdata/libfdata_vector.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfdata/libfdata_libfcache.h` & `libesedb-20240420/libfdata/libfdata_libfcache.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfdata/libfdata_vector.h` & `libesedb-20240420/libfdata/libfdata_vector.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/COPYING` & `libesedb-20240420/COPYING`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/install-sh` & `libesedb-20240420/install-sh`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/depcomp` & `libesedb-20240420/depcomp`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfguid/libfguid_error.c` & `libesedb-20240420/libfguid/libfguid_error.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfguid/libfguid_support.h` & `libesedb-20240420/libfguid/libfguid_support.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfguid/libfguid_identifier.h` & `libesedb-20240420/libfguid/libfguid_identifier.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfguid/libfguid_libcerror.h` & `libesedb-20240420/libfguid/libfguid_libcerror.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfguid/Makefile.am` & `libesedb-20240420/libfguid/Makefile.am`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBFGUID
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libfguid.la
 
 libfguid_la_SOURCES = \
 	libfguid_definitions.h \
 	libfguid_extern.h \
@@ -13,19 +13,17 @@
 	libfguid_libcerror.h \
 	libfguid_identifier.c libfguid_identifier.h \
 	libfguid_support.c libfguid_support.h \
 	libfguid_types.h \
 	libfguid_unused.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libfguid ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfguid_la_SOURCES)
```

### Comparing `libesedb-20240202/libfguid/libfguid_unused.h` & `libesedb-20240420/libfguid/libfguid_unused.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfguid/libfguid_extern.h` & `libesedb-20240420/libfguid/libfguid_extern.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfguid/libfguid_types.h` & `libesedb-20240420/libfguid/libfguid_types.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfguid/libfguid_identifier.c` & `libesedb-20240420/libfguid/libfguid_identifier.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfguid/libfguid_support.c` & `libesedb-20240420/libfguid/libfguid_support.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfguid/libfguid_definitions.h` & `libesedb-20240420/libfguid/libfguid_definitions.h`

 * *Files 6% similar despite different names*

```diff
@@ -32,19 +32,19 @@
 
 /* The definitions in <libfguid/definitions.h> are copied here
  * for local use of libfguid
  */
 #else
 #include <byte_stream.h>
 
-#define LIBFGUID_VERSION					20240116
+#define LIBFGUID_VERSION					20240415
 
 /* The version string
  */
-#define LIBFGUID_VERSION_STRING					"20240116"
+#define LIBFGUID_VERSION_STRING					"20240415"
 
 /* The byte order definitions
  */
 #define LIBFGUID_ENDIAN_BIG					_BYTE_STREAM_ENDIAN_BIG
 #define LIBFGUID_ENDIAN_LITTLE					_BYTE_STREAM_ENDIAN_LITTLE
 
 /* The GUID identifier version definitions
```

### Comparing `libesedb-20240202/libfguid/Makefile.in` & `libesedb-20240420/libfguid/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -540,30 +540,31 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBFGUID_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBFGUID_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBFGUID_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBFGUID_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBFGUID_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBFGUID_TRUE@	@LIBCERROR_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBFGUID_TRUE@noinst_LTLIBRARIES = libfguid.la
 @HAVE_LOCAL_LIBFGUID_TRUE@libfguid_la_SOURCES = \
 @HAVE_LOCAL_LIBFGUID_TRUE@	libfguid_definitions.h \
 @HAVE_LOCAL_LIBFGUID_TRUE@	libfguid_extern.h \
 @HAVE_LOCAL_LIBFGUID_TRUE@	libfguid_error.c libfguid_error.h \
 @HAVE_LOCAL_LIBFGUID_TRUE@	libfguid_libcerror.h \
 @HAVE_LOCAL_LIBFGUID_TRUE@	libfguid_identifier.c libfguid_identifier.h \
 @HAVE_LOCAL_LIBFGUID_TRUE@	libfguid_support.c libfguid_support.h \
 @HAVE_LOCAL_LIBFGUID_TRUE@	libfguid_types.h \
 @HAVE_LOCAL_LIBFGUID_TRUE@	libfguid_unused.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -765,24 +766,29 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libfguid_error.Plo
+	-rm -f ./$(DEPDIR)/libfguid_identifier.Plo
+	-rm -f ./$(DEPDIR)/libfguid_support.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -868,17 +874,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libfguid ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfguid_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libesedb-20240202/libfguid/libfguid_error.h` & `libesedb-20240420/libfguid/libfguid_error.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/m4/libfwnt.m4` & `libesedb-20240420/m4/libfwnt.m4`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libfwnt required headers and functions
 dnl
-dnl Version: 20191217
+dnl Version: 20240413
 
 dnl Function to detect if libfwnt is available
 dnl ac_libfwnt_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBFWNT_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libfwnt" = xno],
     [ac_cv_libfwnt=no],
     [ac_cv_libfwnt=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libfwnt which returns "yes" and --with-libfwnt= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libfwnt" != x && test "x$ac_cv_with_libfwnt" != xauto-detect],
+      [test "x$ac_cv_with_libfwnt" != x && test "x$ac_cv_with_libfwnt" != xauto-detect && test "x$ac_cv_with_libfwnt" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libfwnt"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libfwnt}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libfwnt}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libfwnt],
           [1])
@@ -214,16 +216,17 @@
           fwnt,
           libfwnt_lzxpress_huffman_decompress,
           [ac_cv_libfwnt_dummy=yes],
           [ac_cv_libfwnt=no])
 
         ac_cv_libfwnt_LIBADD="-lfwnt"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libfwnt" != x && test "x$ac_cv_with_libfwnt" != xauto-detect && test "x$ac_cv_libfwnt" != xyes],
+      [test "x$ac_cv_libfwnt" != xyes && test "x$ac_cv_with_libfwnt" != x && test "x$ac_cv_with_libfwnt" != xauto-detect && test "x$ac_cv_with_libfwnt" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libfwnt in directory: $ac_cv_with_libfwnt],
         [1])
       ])
     ])
 
   AS_IF(
@@ -245,15 +248,15 @@
     ])
   ])
 
 dnl Function to detect if libfwnt dependencies are available
 AC_DEFUN([AX_LIBFWNT_CHECK_LOCAL],
   [dnl No additional checks.
 
-  ac_cv_libfwnt_CPPFLAGS="-I../libfwnt";
+  ac_cv_libfwnt_CPPFLAGS="-I../libfwnt -I\$(top_srcdir)/libfwnt";
   ac_cv_libfwnt_LIBADD="../libfwnt/libfwnt.la";
 
   ac_cv_libfwnt=local
   ])
 
 dnl Function to detect how to enable libfwnt
 AC_DEFUN([AX_LIBFWNT_CHECK_ENABLE],
```

### Comparing `libesedb-20240202/m4/libcfile.m4` & `libesedb-20240420/m4/libcfile.m4`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libcfile required headers and functions
 dnl
-dnl Version: 20190308
+dnl Version: 20240413
 
 dnl Function to detect if libcfile is available
 dnl ac_libcfile_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBCFILE_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcfile" = xno],
     [ac_cv_libcfile=no],
     [ac_cv_libcfile=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libcfile which returns "yes" and --with-libcfile= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libcfile" != x && test "x$ac_cv_with_libcfile" != xauto-detect],
+      [test "x$ac_cv_with_libcfile" != x && test "x$ac_cv_with_libcfile" != xauto-detect && test "x$ac_cv_with_libcfile" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libcfile"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libcfile}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcfile}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libcfile],
           [1])
@@ -199,16 +201,17 @@
             libcfile_file_remove_wide,
             [ac_cv_libcfile_dummy=yes],
             [ac_cv_libcfile=no])
           ])
 
         ac_cv_libcfile_LIBADD="-lcfile"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libcfile" != x && test "x$ac_cv_with_libcfile" != xauto-detect && test "x$ac_cv_libcfile" != xyes],
+      [test "x$ac_cv_libcfile" != xyes && test "x$ac_cv_with_libcfile" != x && test "x$ac_cv_with_libcfile" != xauto-detect && test "x$ac_cv_with_libcfile" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libcfile in directory: $ac_cv_with_libcfile],
         [1])
       ])
     ])
 
   AS_IF(
@@ -354,15 +357,15 @@
   AS_IF(
     [test "x$ac_cv_func_unlink" != xyes],
     [AC_MSG_FAILURE(
       [Missing function: unlink],
       [1])
     ])
 
-  ac_cv_libcfile_CPPFLAGS="-I../libcfile";
+  ac_cv_libcfile_CPPFLAGS="-I../libcfile -I\$(top_srcdir)/libcfile";
   ac_cv_libcfile_LIBADD="../libcfile/libcfile.la";
 
   ac_cv_libcfile=local
   ])
 
 dnl Function to detect how to enable libcfile
 AC_DEFUN([AX_LIBCFILE_CHECK_ENABLE],
```

### Comparing `libesedb-20240202/m4/libfdatetime.m4` & `libesedb-20240420/m4/libfdatetime.m4`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libfdatetime required headers and functions
 dnl
-dnl Version: 20190308
+dnl Version: 20240413
 
 dnl Function to detect if libfdatetime is available
 dnl ac_libfdatetime_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBFDATETIME_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libfdatetime" = xno],
     [ac_cv_libfdatetime=no],
     [ac_cv_libfdatetime=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libfdatetime which returns "yes" and --with-libfdatetime= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libfdatetime" != x && test "x$ac_cv_with_libfdatetime" != xauto-detect],
+      [test "x$ac_cv_with_libfdatetime" != x && test "x$ac_cv_with_libfdatetime" != xauto-detect && test "x$ac_cv_with_libfdatetime" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libfdatetime"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libfdatetime}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libfdatetime}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libfdatetime],
           [1])
@@ -455,16 +457,17 @@
           fdatetime,
           libfdatetime_systemetime_copy_to_utf32_string_with_index,
           [ac_cv_libfdatetime_dummy=yes],
           [ac_cv_libfdatetime=no])
 
         ac_cv_libfdatetime_LIBADD="-lfdatetime"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libfdatetime" != x && test "x$ac_cv_with_libfdatetime" != xauto-detect && test "x$ac_cv_libfdatetime" != xyes],
+      [test "x$ac_cv_libfdatetime" != xyes && test "x$ac_cv_with_libfdatetime" != x && test "x$ac_cv_with_libfdatetime" != xauto-detect && test "x$ac_cv_with_libfdatetime" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libfdatetime in directory: $ac_cv_with_libfdatetime],
         [1])
       ])
     ])
 
   AS_IF(
@@ -486,15 +489,15 @@
     ])
   ])
 
 dnl Function to detect if libfdatetime dependencies are available
 AC_DEFUN([AX_LIBFDATETIME_CHECK_LOCAL],
   [dnl No additional checks.
 
-  ac_cv_libfdatetime_CPPFLAGS="-I../libfdatetime";
+  ac_cv_libfdatetime_CPPFLAGS="-I../libfdatetime -I\$(top_srcdir)/libfdatetime";
   ac_cv_libfdatetime_LIBADD="../libfdatetime/libfdatetime.la";
 
   ac_cv_libfdatetime=local
   ])
 
 dnl Function to detect how to enable libfdatetime
 AC_DEFUN([AX_LIBFDATETIME_CHECK_ENABLE],
```

### Comparing `libesedb-20240202/m4/tests.m4` & `libesedb-20240420/m4/tests.m4`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/m4/libcpath.m4` & `libesedb-20240420/m4/libcpath.m4`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libcpath required headers and functions
 dnl
-dnl Version: 20190308
+dnl Version: 20240413
 
 dnl Function to detect if libcpath is available
 dnl ac_libcpath_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBCPATH_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcpath" = xno],
     [ac_cv_libcpath=no],
     [ac_cv_libcpath=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libcpath which returns "yes" and --with-libcpath= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libcpath" != x && test "x$ac_cv_with_libcpath" != xauto-detect],
+      [test "x$ac_cv_with_libcpath" != x && test "x$ac_cv_with_libcpath" != xauto-detect && test "x$ac_cv_with_libcpath" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libcpath"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libcpath}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcpath}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libcpath],
           [1])
@@ -148,16 +150,17 @@
             libcpath_path_make_directory_wide,
             [ac_cv_libcpath_dummy=yes],
             [ac_cv_libcpath=no])
           ])
 
         ac_cv_libcpath_LIBADD="-lcpath"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libcpath" != x && test "x$ac_cv_with_libcpath" != xauto-detect && test "x$ac_cv_libcpath" != xyes],
+      [test "x$ac_cv_libcpath" != xyes && test "x$ac_cv_with_libcpath" != x && test "x$ac_cv_with_libcpath" != xauto-detect && test "x$ac_cv_with_libcpath" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libcpath in directory: $ac_cv_with_libcpath],
         [1])
       ])
     ])
 
   AS_IF(
@@ -269,15 +272,15 @@
     [AC_MSG_FAILURE(
       [Missing functions: getcwd],
       [1])
     ])
 
   AX_LIBCPATH_CHECK_FUNC_MKDIR
 
-  ac_cv_libcpath_CPPFLAGS="-I../libcpath";
+  ac_cv_libcpath_CPPFLAGS="-I../libcpath -I\$(top_srcdir)/libcpath";
   ac_cv_libcpath_LIBADD="../libcpath/libcpath.la";
 
   ac_cv_libcpath=local
   ])
 
 dnl Function to detect how to enable libcpath
 AC_DEFUN([AX_LIBCPATH_CHECK_ENABLE],
```

### Comparing `libesedb-20240202/m4/lib-prefix.m4` & `libesedb-20240420/m4/lib-prefix.m4`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/m4/progtest.m4` & `libesedb-20240420/m4/progtest.m4`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/m4/libuna.m4` & `libesedb-20240420/m4/libuna.m4`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 dnl Checks for libuna or required headers and functions
 dnl
-dnl Version: 20230702
+dnl Version: 20240413
 
 dnl Function to detect if a specific libuna definition is available.
 AC_DEFUN([AX_LIBUNA_CHECK_DEFINITION],
   [AC_CACHE_CHECK(
     [if `$1' is defined],
     [$2],
     [AC_LANG_PUSH(C)
@@ -23,16 +23,18 @@
 dnl ac_libuna_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBUNA_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libuna" = xno],
     [ac_cv_libuna=no],
     [ac_cv_libuna=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libuna which returns "yes" and --with-libuna= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libuna" != x && test "x$ac_cv_with_libuna" != xauto-detect],
+      [test "x$ac_cv_with_libuna" != x && test "x$ac_cv_with_libuna" != xauto-detect && test "x$ac_cv_with_libuna" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libuna"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libuna}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libuna}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libuna],
           [1])
@@ -938,16 +940,17 @@
           [ac_cv_libuna_defines_compare_greater])
         AS_IF(
           [test "x$ac_cv_libuna_defines_utf16_stream_allow_unpaired_surrogate" != xyes],
           [ac_cv_libuna=no])
 
         ac_cv_libuna_LIBADD="-luna"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libuna" != x && test "x$ac_cv_with_libuna" != xauto-detect && test "x$ac_cv_libuna" != xyes],
+      [test "x$ac_cv_libuna" != xyes && test "x$ac_cv_with_libuna" != x && test "x$ac_cv_with_libuna" != xauto-detect && test "x$ac_cv_with_libuna" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libuna in directory: $ac_cv_with_libuna],
         [1])
       ])
     ])
 
   AS_IF(
@@ -969,15 +972,15 @@
     ])
   ])
 
 dnl Function to detect if libuna dependencies are available
 AC_DEFUN([AX_LIBUNA_CHECK_LOCAL],
   [dnl No additional checks.
 
-  ac_cv_libuna_CPPFLAGS="-I../libuna";
+  ac_cv_libuna_CPPFLAGS="-I../libuna -I\$(top_srcdir)/libuna";
   ac_cv_libuna_LIBADD="../libuna/libuna.la";
 
   ac_cv_libuna=local
   ])
 
 dnl Function to detect how to enable libuna
 AC_DEFUN([AX_LIBUNA_CHECK_ENABLE],
```

### Comparing `libesedb-20240202/m4/gettext.m4` & `libesedb-20240420/m4/gettext.m4`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/m4/lib-ld.m4` & `libesedb-20240420/m4/lib-ld.m4`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/m4/libclocale.m4` & `libesedb-20240420/m4/libclocale.m4`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libclocale required headers and functions
 dnl
-dnl Version: 20190308
+dnl Version: 20240413
 
 dnl Function to detect if libclocale is available
 dnl ac_libclocale_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBCLOCALE_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libclocale" = xno],
     [ac_cv_libclocale=no],
     [ac_cv_libclocale=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libclocale which returns "yes" and --with-libclocale= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libclocale" != x && test "x$ac_cv_with_libclocale" != xauto-detect],
+      [test "x$ac_cv_with_libclocale" != x && test "x$ac_cv_with_libclocale" != xauto-detect && test "x$ac_cv_with_libclocale" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libclocale"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libclocale}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libclocale}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libclocale],
           [1])
@@ -122,16 +124,17 @@
           clocale,
           libclocale_initialize,
           [ac_cv_libclocale_dummy=yes],
           [ac_cv_libclocale=no])
 
         ac_cv_libclocale_LIBADD="-lclocale"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libclocale" != x && test "x$ac_cv_with_libclocale" != xauto-detect && test "x$ac_cv_libclocale" != xyes],
+      [test "x$ac_cv_libclocale" != xyes && test "x$ac_cv_with_libclocale" != x && test "x$ac_cv_with_libclocale" != xauto-detect && test "x$ac_cv_with_libclocale" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libclocale in directory: $ac_cv_with_libclocale],
         [1])
       ])
     ])
 
   AS_IF(
@@ -216,15 +219,15 @@
     [AC_MSG_FAILURE(
       [Missing function: setlocale],
       [1])
     ])
 
   AX_LIBCLOCALE_CHECK_FUNC_LANGINFO_CODESET
 
-  ac_cv_libclocale_CPPFLAGS="-I../libclocale";
+  ac_cv_libclocale_CPPFLAGS="-I../libclocale -I\$(top_srcdir)/libclocale";
   ac_cv_libclocale_LIBADD="../libclocale/libclocale.la";
 
   ac_cv_libclocale=local
   ])
 
 dnl Function to detect how to enable libclocale
 AC_DEFUN([AX_LIBCLOCALE_CHECK_ENABLE],
```

### Comparing `libesedb-20240202/m4/libcdata.m4` & `libesedb-20240420/m4/libcdata.m4`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libcdata required headers and functions
 dnl
-dnl Version: 20230108
+dnl Version: 20240413
 
 dnl Function to detect if libcdata is available
 dnl ac_libcdata_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBCDATA_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcdata" = xno],
     [ac_cv_libcdata=no],
     [ac_cv_libcdata=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libcdata which returns "yes" and --with-libcdata= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libcdata" != x && test "x$ac_cv_with_libcdata" != xauto-detect],
+      [test "x$ac_cv_with_libcdata" != x && test "x$ac_cv_with_libcdata" != xauto-detect && test "x$ac_cv_with_libcdata" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libcdata"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libcdata}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcdata}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libcdata],
           [1])
@@ -493,16 +495,17 @@
           cdata,
           libcdata_tree_node_get_leaf_node_list,
           [ac_cv_libcdata_dummy=yes],
           [ac_cv_libcdata=no])
 
         ac_cv_libcdata_LIBADD="-lcdata"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libcdata" != x && test "x$ac_cv_with_libcdata" != xauto-detect && test "x$ac_cv_libcdata" != xyes],
+      [test "x$ac_cv_libcdata" != xyes && test "x$ac_cv_with_libcdata" != x && test "x$ac_cv_with_libcdata" != xauto-detect && test "x$ac_cv_with_libcdata" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libcdata in directory: $ac_cv_with_libcdata],
         [1])
       ])
     ])
 
   AS_IF(
@@ -524,15 +527,15 @@
     ])
   ])
 
 dnl Function to detect if libcdata dependencies are available
 AC_DEFUN([AX_LIBCDATA_CHECK_LOCAL],
   [dnl No additional checks.
 
-  ac_cv_libcdata_CPPFLAGS="-I../libcdata";
+  ac_cv_libcdata_CPPFLAGS="-I../libcdata -I\$(top_srcdir)/libcdata";
   ac_cv_libcdata_LIBADD="../libcdata/libcdata.la";
 
   ac_cv_libcdata=local
   ])
 
 dnl Function to detect how to enable libcdata
 AC_DEFUN([AX_LIBCDATA_CHECK_ENABLE],
```

### Comparing `libesedb-20240202/m4/libcsplit.m4` & `libesedb-20240420/m4/libcsplit.m4`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libcsplit required headers and functions
 dnl
-dnl Version: 20190308
+dnl Version: 20240413
 
 dnl Function to detect if libcsplit is available
 dnl ac_libcsplit_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBCSPLIT_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcsplit" = xno],
     [ac_cv_libcsplit=no],
     [ac_cv_libcsplit=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libcsplit which returns "yes" and --with-libcsplit= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libcsplit" != x && test "x$ac_cv_with_libcsplit" != xauto-detect],
+      [test "x$ac_cv_with_libcsplit" != x && test "x$ac_cv_with_libcsplit" != xauto-detect && test "x$ac_cv_with_libcsplit" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libcsplit"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libcsplit}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcsplit}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libcsplit],
           [1])
@@ -143,16 +145,17 @@
             libcsplit_wide_split_string_set_segment_by_index,
             [ac_cv_libcsplit_dummy=yes],
             [ac_cv_libcsplit=no])
           ])
 
         ac_cv_libcsplit_LIBADD="-lcsplit"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libcsplit" != x && test "x$ac_cv_with_libcsplit" != xauto-detect && test "x$ac_cv_libcsplit" != xyes],
+      [test "x$ac_cv_libcsplit" != xyes && test "x$ac_cv_with_libcsplit" != x && test "x$ac_cv_with_libcsplit" != xauto-detect && test "x$ac_cv_with_libcsplit" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libcsplit in directory: $ac_cv_with_libcsplit],
         [1])
       ])
     ])
 
   AS_IF(
@@ -174,15 +177,15 @@
     ])
   ])
 
 dnl Function to detect if libcsplit dependencies are available
 AC_DEFUN([AX_LIBCSPLIT_CHECK_LOCAL],
   [dnl No additional checks.
 
-  ac_cv_libcsplit_CPPFLAGS="-I../libcsplit";
+  ac_cv_libcsplit_CPPFLAGS="-I../libcsplit -I\$(top_srcdir)/libcsplit";
   ac_cv_libcsplit_LIBADD="../libcsplit/libcsplit.la";
 
   ac_cv_libcsplit=local
   ])
 
 dnl Function to detect how to enable libcsplit
 AC_DEFUN([AX_LIBCSPLIT_CHECK_ENABLE],
```

### Comparing `libesedb-20240202/m4/common.m4` & `libesedb-20240420/m4/common.m4`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 dnl Checks for common headers and functions
 dnl
-dnl Version: 20181117
+dnl Version: 20240308
 
 dnl Function to test if a certain feature was disabled
 AC_DEFUN([AX_COMMON_ARG_DISABLE],
 [
   AC_ARG_ENABLE(
     [$1],
     [AS_HELP_STRING(
@@ -22,15 +22,15 @@
 dnl Function to test if a certain feature was enabled
 AC_DEFUN([AX_COMMON_ARG_ENABLE],
 [
   AC_ARG_ENABLE(
     [$1],
     [AS_HELP_STRING(
       [--enable-$1],
-      [$3 [default=$4]])],
+      [$3 @<:@default=$4@:>@])],
     [ac_cv_enable_$2=$enableval],
     [ac_cv_enable_$2=$4])dnl
 
     AC_CACHE_CHECK(
       [whether to enable $3],
       [ac_cv_enable_$2],
       [ac_cv_enable_$2=$4])dnl
@@ -39,15 +39,15 @@
 dnl Function to test if the location of a certain feature was provided
 AC_DEFUN([AX_COMMON_ARG_WITH],
 [
   AC_ARG_WITH(
     [$1],
     [AS_HELP_STRING(
       [--with-$1[[=$5]]],
-      [$3 [default=$4]])],
+      [$3 @<:@default=$4@:>@])],
     [ac_cv_with_$2=$withval],
     [ac_cv_with_$2=$4])dnl
 
     AC_CACHE_CHECK(
       [whether to use $3],
       [ac_cv_with_$2],
       [ac_cv_with_$2=$4])dnl
```

### Comparing `libesedb-20240202/m4/libcthreads.m4` & `libesedb-20240420/m4/libcthreads.m4`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libcthreads required headers and functions
 dnl
-dnl Version: 20190308
+dnl Version: 20240413
 
 dnl Function to detect if libcthreads is available
 dnl ac_libcthreads_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBCTHREADS_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcthreads" = xno],
     [ac_cv_libcthreads=no],
     [ac_cv_libcthreads=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libcthreads which returns "yes" and --with-libcthreads= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libcthreads" != x && test "x$ac_cv_with_libcthreads" != xauto-detect],
+      [test "x$ac_cv_with_libcthreads" != x && test "x$ac_cv_with_libcthreads" != xauto-detect && test "x$ac_cv_with_libcthreads" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libcthreads"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libcthreads}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcthreads}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libcthreads],
           [1])
@@ -244,15 +246,15 @@
           [ac_cv_libcthreads_dummy=yes],
           [ac_cv_libcthreads=no])
 
         ac_cv_libcthreads_LIBADD="-lcthreads"])
       ])
 
     AS_IF(
-      [test "x$ac_cv_with_libcthreads" != x && test "x$ac_cv_with_libcthreads" != xauto-detect && test "x$ac_cv_libcthreads" != xyes],
+      [test "x$ac_cv_libcthreads" != xyes && test "x$ac_cv_with_libcthreads" != x && test "x$ac_cv_with_libcthreads" != xauto-detect && test "x$ac_cv_with_libcthreads" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libcthreads in directory: $ac_cv_with_libcthreads],
         [1])
       ])
     ])
 
   AS_IF(
@@ -286,15 +288,15 @@
     [dnl Check for enabling pthread support
     AX_PTHREAD_CHECK_ENABLE
       ac_cv_libcthreads_multi_threading=$ac_cv_pthread],
     [ac_cv_libcthreads_multi_threading="winapi"])
 
   AS_IF(
     [test "x$ac_cv_libcthreads_multi_threading" != xno],
-    [ac_cv_libcthreads_CPPFLAGS="-I../libcthreads";
+    [ac_cv_libcthreads_CPPFLAGS="-I../libcthreads -I\$(top_srcdir)/libcthreads";
     ac_cv_libcthreads_LIBADD="../libcthreads/libcthreads.la";
 
     ac_cv_libcthreads=local],
     [ac_cv_libcthreads=no])
   ])
 
 dnl Function to detect how to enable libcthreads
```

### Comparing `libesedb-20240202/m4/libmapidb.m4` & `libesedb-20240420/m4/libmapidb.m4`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libmapidb required headers and functions
 dnl
-dnl Version: 20200715
+dnl Version: 20240413
 
 dnl Function to detect if libmapidb is available
 dnl ac_libmapidb_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBMAPIDB_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libmapidb" = xno],
     [ac_cv_libmapidb=no],
     [ac_cv_libmapidb=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libmapidb which returns "yes" and --with-libmapidb= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libmapidb" != x && test "x$ac_cv_with_libmapidb" != xauto-detect],
+      [test "x$ac_cv_with_libmapidb" != x && test "x$ac_cv_with_libmapidb" != xauto-detect && test "x$ac_cv_with_libmapidb" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libmapidb"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libmapidb}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libmapidb}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libmapidb],
           [1])
@@ -53,16 +55,17 @@
           [ac_cv_libmapidb_dummy=yes],
           [ac_cv_libmapidb=no])
 
         dnl TODO add functions
 
         ac_cv_libmapidb_LIBADD="-lmapidb"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libmapidb" != x && test "x$ac_cv_with_libmapidb" != xauto-detect && test "x$ac_cv_libmapidb" != xyes],
+      [test "x$ac_cv_libmapidb" != xyes && test "x$ac_cv_with_libmapidb" != x && test "x$ac_cv_with_libmapidb" != xauto-detect && test "x$ac_cv_with_libmapidb" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libmapidb in directory: $ac_cv_with_libmapidb],
         [1])
       ])
     ])
 
   AS_IF(
@@ -82,15 +85,15 @@
       [HAVE_LIBMAPIDB],
       [0])
     ])
   ])
 
 dnl Function to detect if libmapidb dependencies are available
 AC_DEFUN([AX_LIBMAPIDB_CHECK_LOCAL],
-  [ac_cv_libmapidb_CPPFLAGS="-I../libmapidb";
+  [ac_cv_libmapidb_CPPFLAGS="-I../libmapidb -I\$(top_srcdir)/libmapidb";
   ac_cv_libmapidb_LIBADD="../libmapidb/libmapidb.la";
 
   ac_cv_libmapidb=local
   ])
 
 dnl Function to detect how to enable libmapidb
 AC_DEFUN([AX_LIBMAPIDB_CHECK_ENABLE],
```

### Comparing `libesedb-20240202/m4/ltversion.m4` & `libesedb-20240420/m4/ltversion.m4`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/m4/ltsugar.m4` & `libesedb-20240420/m4/ltsugar.m4`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/m4/libfdata.m4` & `libesedb-20240420/m4/libfdata.m4`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Functions for libfdata
 dnl
-dnl Version: 20230318
+dnl Version: 20240413
 
 dnl Function to detect if libfdata is available
 dnl ac_libfdata_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBFDATA_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libfdata" = xno],
     [ac_cv_libfdata=no],
     [ac_cv_libfdata=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libfdata which returns "yes" and --with-libfdata= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libfdata" != x && test "x$ac_cv_with_libfdata" != xauto-detect],
+      [test "x$ac_cv_with_libfdata" != x && test "x$ac_cv_with_libfdata" != xauto-detect && test "x$ac_cv_with_libfdata" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libfdata"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libfdata}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libfdata}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libfdata],
           [1])
@@ -450,16 +452,17 @@
         dnl TODO: add functions
 
         dnl Vector list functions
         dnl TODO: add functions
 
         ac_cv_libfdata_LIBADD="-lfdata"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libfdata" != x && test "x$ac_cv_with_libfdata" != xauto-detect && test "x$ac_cv_libfdata" != xyes],
+      [test "x$ac_cv_libfdata" != xyes && test "x$ac_cv_with_libfdata" != x && test "x$ac_cv_with_libfdata" != xauto-detect && test "x$ac_cv_with_libfdata" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libfdata in directory: $ac_cv_with_libfdata],
         [1])
       ])
     ])
 
   AS_IF(
@@ -481,15 +484,15 @@
     ])
   ])
 
 dnl Function to detect if libfdata dependencies are available
 AC_DEFUN([AX_LIBFDATA_CHECK_LOCAL],
   [dnl No additional checks.
 
-  ac_cv_libfdata_CPPFLAGS="-I../libfdata";
+  ac_cv_libfdata_CPPFLAGS="-I../libfdata -I\$(top_srcdir)/libfdata";
   ac_cv_libfdata_LIBADD="../libfdata/libfdata.la";
 
   ac_cv_libfdata=local
   ])
 
 dnl Function to detect how to enable libfdata
 AC_DEFUN([AX_LIBFDATA_CHECK_ENABLE],
```

### Comparing `libesedb-20240202/m4/host-cpu-c-abi.m4` & `libesedb-20240420/m4/host-cpu-c-abi.m4`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/m4/libtool.m4` & `libesedb-20240420/m4/libtool.m4`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/m4/po.m4` & `libesedb-20240420/m4/po.m4`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/m4/libcerror.m4` & `libesedb-20240420/m4/libcerror.m4`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libcerror required headers and functions
 dnl
-dnl Version: 20190308
+dnl Version: 20240413
 
 dnl Function to detect if libcerror is available
 dnl ac_libcerror_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBCERROR_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcerror" = xno],
     [ac_cv_libcerror=no],
     [ac_cv_libcerror=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libcerror which returns "yes" and --with-libcerror= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libcerror" != x && test "x$ac_cv_with_libcerror" != xauto-detect],
+      [test "x$ac_cv_with_libcerror" != x && test "x$ac_cv_with_libcerror" != xauto-detect && test "x$ac_cv_with_libcerror" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libcerror"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libcerror}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcerror}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libcerror],
           [1])
@@ -95,16 +97,17 @@
           cerror,
           libcerror_system_set_error,
           [ac_cv_libcerror_dummy=yes],
           [ac_cv_libcerror=no])
 
         ac_cv_libcerror_LIBADD="-lcerror"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libcerror" != x && test "x$ac_cv_with_libcerror" != xauto-detect && test "x$ac_cv_libcerror" != xyes],
+      [test "x$ac_cv_libcerror" != xyes && test "x$ac_cv_with_libcerror" != x && test "x$ac_cv_with_libcerror" != xauto-detect && test "x$ac_cv_with_libcerror" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libcerror in directory: $ac_cv_with_libcerror],
         [1])
       ])
     ])
 
   AS_IF(
@@ -162,15 +165,15 @@
       [test "x$ac_cv_func_strerror" != xyes],
       [AC_MSG_FAILURE(
         [Missing functions: strerror_r and strerror],
         [1])
       ])
     ])
 
-  ac_cv_libcerror_CPPFLAGS="-I../libcerror";
+  ac_cv_libcerror_CPPFLAGS="-I../libcerror -I\$(top_srcdir)/libcerror";
   ac_cv_libcerror_LIBADD="../libcerror/libcerror.la";
 
   ac_cv_libcerror=local
   ])
 
 dnl Function to detect how to enable libcerror
 AC_DEFUN([AX_LIBCERROR_CHECK_ENABLE],
```

### Comparing `libesedb-20240202/m4/libcnotify.m4` & `libesedb-20240420/m4/libcnotify.m4`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libcnotify required headers and functions
 dnl
-dnl Version: 20190308
+dnl Version: 20240413
 
 dnl Function to detect if libcnotify is available
 dnl ac_libcnotify_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBCNOTIFY_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcnotify" = xno],
     [ac_cv_libcnotify=no],
     [ac_cv_libcnotify=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libcnotify which returns "yes" and --with-libcnotify= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libcnotify" != x && test "x$ac_cv_with_libcnotify" != xauto-detect],
+      [test "x$ac_cv_with_libcnotify" != x && test "x$ac_cv_with_libcnotify" != xauto-detect && test "x$ac_cv_with_libcnotify" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libcnotify"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libcnotify}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcnotify}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libcnotify],
           [1])
@@ -92,16 +94,17 @@
           cnotify,
           libcnotify_verbose_set,
           [ac_cv_libcnotify_dummy=yes],
           [ac_cv_libcnotify=no])
 
         ac_cv_libcnotify_LIBADD="-lcnotify"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libcnotify" != x && test "x$ac_cv_with_libcnotify" != xauto-detect && test "x$ac_cv_libcnotify" != xyes],
+      [test "x$ac_with_libcnotify" != xyes && test "x$ac_cv_with_libcnotify" != x && test "x$ac_cv_with_libcnotify" != xauto-detect && test "x$ac_cv_with_libcnotify" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libcnotify in directory: $ac_cv_with_libcnotify],
         [1])
       ])
     ])
 
   AS_IF(
@@ -134,15 +137,15 @@
       [Missing headers: stdarg.h and varargs.h],
       [1])
     ])
 
   dnl Headers included in libcnotify/libcnotify_stream.c
   AC_CHECK_HEADERS([errno.h])
 
-  ac_cv_libcnotify_CPPFLAGS="-I../libcnotify";
+  ac_cv_libcnotify_CPPFLAGS="-I../libcnotify -I\$(top_srcdir)/libcnotify";
   ac_cv_libcnotify_LIBADD="../libcnotify/libcnotify.la";
 
   ac_cv_libcnotify=local
   ])
 
 dnl Function to detect how to enable libcnotify
 AC_DEFUN([AX_LIBCNOTIFY_CHECK_ENABLE],
```

### Comparing `libesedb-20240202/m4/libfguid.m4` & `libesedb-20240420/m4/libfguid.m4`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libfguid required headers and functions
 dnl
-dnl Version: 20190308
+dnl Version: 20240413
 
 dnl Function to detect if libfguid is available
 dnl ac_libfguid_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBFGUID_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libfguid" = xno],
     [ac_cv_libfguid=no],
     [ac_cv_libfguid=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libfguid which returns "yes" and --with-libfguid= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libfguid" != x && test "x$ac_cv_with_libfguid" != xauto-detect],
+      [test "x$ac_cv_with_libfguid" != x && test "x$ac_cv_with_libfguid" != xauto-detect && test "x$ac_cv_with_libfguid" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libfguid"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libfguid}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libfguid}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libfguid],
           [1])
@@ -103,16 +105,17 @@
           fguid,
           libfguid_identifier_copy_to_utf32_string_with_index,
           [ac_cv_libfguid_dummy=yes],
           [ac_cv_libfguid=no])
 
         ac_cv_libfguid_LIBADD="-lfguid"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libfguid" != x && test "x$ac_cv_with_libfguid" != xauto-detect && test "x$ac_cv_libfguid" != xyes],
+      [test "x$ac_cv_libfguid" != xyes && test "x$ac_cv_with_libfguid" != x && test "x$ac_cv_with_libfguid" != xauto-detect && test "x$ac_cv_with_libfguid" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libfguid in directory: $ac_cv_with_libfguid],
         [1])
       ])
     ])
 
   AS_IF(
@@ -134,15 +137,15 @@
     ])
   ])
 
 dnl Function to detect if libfguid dependencies are available
 AC_DEFUN([AX_LIBFGUID_CHECK_LOCAL],
   [dnl No additional checks.
 
-  ac_cv_libfguid_CPPFLAGS="-I../libfguid";
+  ac_cv_libfguid_CPPFLAGS="-I../libfguid -I\$(top_srcdir)/libfguid";
   ac_cv_libfguid_LIBADD="../libfguid/libfguid.la";
 
   ac_cv_libfguid=local
   ])
 
 
 dnl Function to detect how to enable libfguid
```

### Comparing `libesedb-20240202/m4/libbfio.m4` & `libesedb-20240420/m4/libbfio.m4`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libbfio required headers and functions
 dnl
-dnl Version: 20201125
+dnl Version: 20240413
 
 dnl Function to detect if libbfio is available
 dnl ac_libbfio_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBBFIO_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libbfio" = xno],
     [ac_cv_libbfio=no],
     [ac_cv_libbfio=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libbfio which returns "yes" and --with-libbfio= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libbfio" != x && test "x$ac_cv_with_libbfio" != xauto-detect],
+      [test "x$ac_cv_with_libbfio" != x && test "x$ac_cv_with_libbfio" != xauto-detect && test "x$ac_cv_with_libbfio" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libbfio"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libbfio}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libbfio}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libbfio],
           [1])
@@ -316,16 +318,17 @@
             libbfio_file_pool_open_wide,
             [ac_cv_libbfio_dummy=yes],
             [ac_cv_libbfio=no])
           ])
 
         ac_cv_libbfio_LIBADD="-lbfio"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libbfio" != x && test "x$ac_cv_with_libbfio" != xauto-detect && test "x$ac_cv_libbfio" != xyes],
+      [test "x$ac_cv_libbfio" != xyes && test "x$ac_cv_with_libbfio" != x && test "x$ac_cv_with_libbfio" != xauto-detect && test "x$ac_cv_with_libbfio" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libbfio in directory: $ac_cv_with_libbfio],
         [1])
       ])
     ])
 
   AS_IF(
@@ -347,15 +350,15 @@
     ])
   ])
 
 dnl Function to detect if libbfio dependencies are available
 AC_DEFUN([AX_LIBBFIO_CHECK_LOCAL],
   [dnl No additional checks.
 
-  ac_cv_libbfio_CPPFLAGS="-I../libbfio";
+  ac_cv_libbfio_CPPFLAGS="-I../libbfio -I\$(top_srcdir)/libbfio";
   ac_cv_libbfio_LIBADD="../libbfio/libbfio.la";
 
   ac_cv_libbfio=local
   ])
 
 dnl Function to detect how to enable libbfio
 AC_DEFUN([AX_LIBBFIO_CHECK_ENABLE],
```

### Comparing `libesedb-20240202/m4/libfmapi.m4` & `libesedb-20240420/m4/libfmapi.m4`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libfmapi required headers and functions
 dnl
-dnl Version: 20230404
+dnl Version: 20240413
 
 dnl Function to detect if libfmapi is available
 dnl ac_libfmapi_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBFMAPI_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libfmapi" = xno],
     [ac_cv_libfmapi=no],
     [ac_cv_libfmapi=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libfmapi which returns "yes" and --with-libfmapi= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libfmapi" != x && test "x$ac_cv_with_libfmapi" != xauto-detect],
+      [test "x$ac_cv_with_libfmapi" != x && test "x$ac_cv_with_libfmapi" != xauto-detect && test "x$ac_cv_with_libfmapi" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libfmapi"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libfmapi}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libfmapi}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libfmapi],
           [1])
@@ -179,16 +181,17 @@
           fmapi,
           libfmapi_lzfu_decompress,
           [ac_cv_libfmapi_dummy=yes],
           [ac_cv_libfmapi=no])
 
         ac_cv_libfmapi_LIBADD="-lfmapi"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libfmapi" != x && test "x$ac_cv_with_libfmapi" != xauto-detect && test "x$ac_cv_libfmapi" != xyes],
+      [test "x$ac_cv_libfmapi" != xyes && test "x$ac_cv_with_libfmapi" != x && test "x$ac_cv_with_libfmapi" != xauto-detect && test "x$ac_cv_with_libfmapi" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libfmapi in directory: $ac_cv_with_libfmapi],
         [1])
       ])
     ])
 
   dnl Check for debug functions
@@ -236,15 +239,15 @@
     ])
   ])
 
 dnl Function to detect if libfmapi dependencies are available
 AC_DEFUN([AX_LIBFMAPI_CHECK_LOCAL],
   [dnl No additional checks.
 
-  ac_cv_libfmapi_CPPFLAGS="-I../libfmapi";
+  ac_cv_libfmapi_CPPFLAGS="-I../libfmapi -I\$(top_srcdir)/libfmapi";
   ac_cv_libfmapi_LIBADD="../libfmapi/libfmapi.la";
 
   ac_cv_libfmapi=local
   ])
 
 dnl Function to detect how to enable libfmapi
 AC_DEFUN([AX_LIBFMAPI_CHECK_ENABLE],
```

### Comparing `libesedb-20240202/m4/intlmacosx.m4` & `libesedb-20240420/m4/intlmacosx.m4`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/m4/lt~obsolete.m4` & `libesedb-20240420/m4/lt~obsolete.m4`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/m4/lib-link.m4` & `libesedb-20240420/m4/lib-link.m4`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/m4/iconv.m4` & `libesedb-20240420/m4/iconv.m4`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/m4/ltoptions.m4` & `libesedb-20240420/m4/ltoptions.m4`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/m4/nls.m4` & `libesedb-20240420/m4/nls.m4`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/m4/python.m4` & `libesedb-20240420/m4/python.m4`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 dnl Functions for Python bindings
 dnl
-dnl Version: 20231119
+dnl Version: 20240418
 
 dnl Function to check if the python binary is available
 dnl "python${PYTHON_VERSION} python python# python#.#"
 AC_DEFUN([AX_PROG_PYTHON],
   [AS_IF(
     [test "x${PYTHON_VERSION}" != x],
     [ax_python_progs="python${PYTHON_VERSION}"],
@@ -72,18 +72,20 @@
     PYTHON_LDFLAGS=`${PYTHON_CONFIG} --ldflags 2>/dev/null`;
 
     AC_MSG_CHECKING(
       [for Python libraries])
     AC_MSG_RESULT(
       [$PYTHON_LDFLAGS])
 
-    dnl For CygWin add the -no-undefined linker flag
+    dnl For CygWin and MinGW add the -no-undefined linker flag
     AS_CASE(
-      [$host_os],
-      [cygwin*],[PYTHON_LDFLAGS="${PYTHON_LDFLAGS} -no-undefined"],
+      [$build],
+      [*-*-cygwin*],[PYTHON_LDFLAGS="${PYTHON_LDFLAGS} -no-undefined"],
+      [*-*-mingw*],[PYTHON_LDFLAGS="${PYTHON_LDFLAGS} -no-undefined"],
+      [*-*-msys*],[PYTHON_LDFLAGS="${PYTHON_LDFLAGS} -no-undefined"],
       [*],[])
 
     dnl Check for the existence of Python.h
     BACKUP_CPPFLAGS="${CPPFLAGS}"
     CPPFLAGS="${CPPFLAGS} ${PYTHON_INCLUDES}"
 
     AC_CHECK_HEADERS(
```

### Comparing `libesedb-20240202/m4/libfvalue.m4` & `libesedb-20240420/m4/libfvalue.m4`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libfvalue required headers and functions
 dnl
-dnl Version: 20200711
+dnl Version: 20240413
 
 dnl Function to detect if libfvalue is available
 dnl ac_libfvalue_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBFVALUE_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libfvalue" = xno],
     [ac_cv_libfvalue=no],
     [ac_cv_libfvalue=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libfvalue which returns "yes" and --with-libfvalue= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libfvalue" != x && test "x$ac_cv_with_libfvalue" != xauto-detect],
+      [test "x$ac_cv_with_libfvalue" != x && test "x$ac_cv_with_libfvalue" != xauto-detect && test "x$ac_cv_with_libfvalue" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libfvalue"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libfvalue}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libfvalue}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libfvalue],
           [1])
@@ -585,16 +587,17 @@
           fvalue,
           libfvalue_value_type_set_data_strings_array,
           [ac_cv_libfvalue_dummy=yes],
           [ac_cv_libfvalue=no])
 
         ac_cv_libfvalue_LIBADD="-lfvalue"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libfvalue" != x && test "x$ac_cv_with_libfvalue" != xauto-detect && test "x$ac_cv_libfvalue" != xyes],
+      [test "x$ac_cv_libfvalue" != xyes && test "x$ac_cv_with_libfvalue" != x && test "x$ac_cv_with_libfvalue" != xauto-detect && test "x$ac_cv_with_libfvalue" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libfvalue in directory: $ac_cv_with_libfvalue],
         [1])
       ])
     ])
 
   AS_IF(
@@ -616,15 +619,15 @@
     ])
   ])
 
 dnl Function to detect if libfvalue dependencies are available
 AC_DEFUN([AX_LIBFVALUE_CHECK_LOCAL],
   [dnl No additional checks.
 
-  ac_cv_libfvalue_CPPFLAGS="-I../libfvalue";
+  ac_cv_libfvalue_CPPFLAGS="-I../libfvalue -I\$(top_srcdir)/libfvalue";
   ac_cv_libfvalue_LIBADD="../libfvalue/libfvalue.la";
 
   ac_cv_libfvalue=local
   ])
 
 dnl Function to detect how to enable libfvalue
 AC_DEFUN([AX_LIBFVALUE_CHECK_ENABLE],
```

### Comparing `libesedb-20240202/m4/types.m4` & `libesedb-20240420/m4/types.m4`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/m4/libfcache.m4` & `libesedb-20240420/m4/libfcache.m4`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libfcache required headers and functions
 dnl
-dnl Version: 20230115
+dnl Version: 20240413
 
 dnl Function to detect if libfcache is available
 dnl ac_libfcache_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBFCACHE_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libfcache" = xno],
     [ac_cv_libfcache=no],
     [ac_cv_libfcache=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libfcache which returns "yes" and --with-libfcache= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libfcache" != x && test "x$ac_cv_with_libfcache" != xauto-detect],
+      [test "x$ac_cv_with_libfcache" != x && test "x$ac_cv_with_libfcache" != xauto-detect && test "x$ac_cv_with_libfcache" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libfcache"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libfcache}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libfcache}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libfcache],
           [1])
@@ -147,16 +149,17 @@
           fcache,
           libfcache_date_time_get_timestamp,
           [ac_cv_libfcache_dummy=yes],
           [ac_cv_libfcache=no])
 
         ac_cv_libfcache_LIBADD="-lfcache"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libfcache" != x && test "x$ac_cv_with_libfcache" != xauto-detect && test "x$ac_cv_libfcache" != xyes],
+      [test "x$ac_cv_libfcache" != xyes && test "x$ac_cv_with_libfcache" != x && test "x$ac_cv_with_libfcache" != xauto-detect && test "x$ac_cv_with_libfcache" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libfcache in directory: $ac_cv_with_libfcache],
         [1])
       ])
     ])
 
   AS_IF(
@@ -192,15 +195,15 @@
   AS_IF(
     [test "x$ac_cv_func_time" != xyes],
     [AC_MSG_FAILURE(
       [Missing function: time],
       [1])
     ])
 
-  ac_cv_libfcache_CPPFLAGS="-I../libfcache";
+  ac_cv_libfcache_CPPFLAGS="-I../libfcache -I\$(top_srcdir)/libfcache";
   ac_cv_libfcache_LIBADD="../libfcache/libfcache.la";
 
   ac_cv_libfcache=local
   ])
 
 dnl Function to detect how to enable libfcache
 AC_DEFUN([AX_LIBFCACHE_CHECK_ENABLE],
```

### Comparing `libesedb-20240202/m4/pthread.m4` & `libesedb-20240420/m4/pthread.m4`

 * *Files 18% similar despite different names*

```diff
@@ -1,183 +1,196 @@
 dnl Functions for pthread
 dnl
-dnl Version: 20130509
+dnl Version: 20240308
 
 dnl Function to detect if pthread is available
 AC_DEFUN([AX_PTHREAD_CHECK_LIB],
- [dnl Check if parameters were provided
- AS_IF(
-  [test "x$ac_cv_with_pthread" != x && test "x$ac_cv_with_pthread" != xno && test "x$ac_cv_with_pthread" != xauto-detect],
   [AS_IF(
-   [test -d "$ac_cv_with_pthread"],
-   [CFLAGS="$CFLAGS -I${ac_cv_with_pthread}/include"
-   LDFLAGS="$LDFLAGS -L${ac_cv_with_pthread}/lib"],
-   [AC_MSG_WARN([no such directory: $ac_cv_with_pthread])
-   ])
-  ])
-
- AS_IF(
-  [test "x$ac_cv_with_pthread" = xno],
-  [ac_cv_pthread=no],
-  [dnl Check for headers
-  AC_CHECK_HEADERS([pthread.h])
+    [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_pthread" = xno],
+    [ac_cv_pthread=no],
+    [ac_cv_pthread=check
+    dnl Check if parameters were provided
+    dnl For both --with-pthread which returns "yes" and --with-pthread= which returns ""
+    dnl treat them as auto-detection.
+    AS_IF(
+      [test "x$ac_cv_with_pthread" != x && test "x$ac_cv_with_pthread" != xauto-detect && test "x$ac_cv_with_pthread" != xyes],
+      [AS_IF(
+        [test -d "$ac_cv_with_pthread"],
+        [CFLAGS="$CFLAGS -I${ac_cv_with_pthread}/include"
+        LDFLAGS="$LDFLAGS -L${ac_cv_with_pthread}/lib"],
+        [AC_MSG_WARN([no such directory: $ac_cv_with_pthread])
+        ])
+      ])
+    ])
+
+    AS_IF(
+      [test "x$ac_cv_pthread" = xcheck],
+      [dnl Check for headers
+      AC_CHECK_HEADERS([pthread.h])
+
+      AS_IF(
+        [test "x$ac_cv_header_pthread_h" = xno],
+        [ac_cv_pthread=no],
+        [dnl Check for the individual functions
+        ac_cv_pthread=pthread
+
+        dnl Thread functions
+        AC_CHECK_LIB(
+          pthread,
+          pthread_create,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_exit,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_join,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+
+        dnl Condition functions
+        AC_CHECK_LIB(
+          pthread,
+          pthread_cond_init,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_cond_destroy,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_cond_broadcast,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_cond_signal,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_cond_wait,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+
+        dnl Mutex functions
+        AC_CHECK_LIB(
+          pthread,
+          pthread_mutex_init,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_mutex_destroy,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_mutex_lock,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_mutex_trylock,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_mutex_unlock,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+
+        dnl Read/Write lock functions
+        AC_CHECK_LIB(
+          pthread,
+          pthread_rwlock_init,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_rwlock_destroy,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_rwlock_rdlock,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_rwlock_wrlock,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_rwlock_unlock,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+
+        ac_cv_pthread_LIBADD="-lpthread";
+      ])
+
+    AS_IF(
+      [test "x$ac_cv_with_pthread" != x && test "x$ac_cv_with_pthread" != xauto-detect && test "x$ac_cv_with_pthread" != xyes],
+      [AC_MSG_FAILURE(
+        [unable to find supported pthread in directory: $ac_cv_with_pthread],
+        [1])
+      ])
+    ])
 
   AS_IF(
-   [test "x$ac_cv_header_pthread_h" = xno],
-   [ac_cv_pthread=no],
-   [dnl Check for the individual functions
-   ac_cv_pthread=pthread
-
-   dnl Thread functions
-   AC_CHECK_LIB(
-    pthread,
-    pthread_create,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_exit,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_join,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-
-   dnl Condition functions
-   AC_CHECK_LIB(
-    pthread,
-    pthread_cond_init,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_cond_destroy,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_cond_broadcast,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_cond_signal,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_cond_wait,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-
-   dnl Mutex functions
-   AC_CHECK_LIB(
-    pthread,
-    pthread_mutex_init,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_mutex_destroy,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_mutex_lock,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_mutex_trylock,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_mutex_unlock,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-
-   dnl Read/Write lock functions
-   AC_CHECK_LIB(
-    pthread,
-    pthread_rwlock_init,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_rwlock_destroy,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_rwlock_rdlock,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_rwlock_wrlock,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_rwlock_unlock,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-
-   ac_cv_pthread_LIBADD="-lpthread";
-   ])
-  ])
+    [test "x$ac_cv_pthread" = xpthread],
+    [AC_DEFINE(
+      [HAVE_PTHREAD],
+      [1],
+      [Define to 1 if you have the 'pthread' library (-lpthread).])
+    ])
 
- AS_IF(
-  [test "x$ac_cv_pthread" = xpthread],
-  [AC_DEFINE(
-   [HAVE_PTHREAD],
-   [1],
-   [Define to 1 if you have the 'pthread' library (-lpthread).])
-  ])
-
- AS_IF(
-  [test "x$ac_cv_pthread" != xno],
-  [AC_SUBST(
-   [HAVE_PTHREAD],
-   [1]) ],
-  [AC_SUBST(
-   [HAVE_PTHREAD],
-   [0])
+  AS_IF(
+    [test "x$ac_cv_pthread" != xno],
+    [AC_SUBST(
+      [HAVE_PTHREAD],
+      [1]) ],
+    [AC_SUBST(
+      [HAVE_PTHREAD],
+      [0])
+    ])
   ])
- ])
 
 dnl Function to detect how to enable pthread
 AC_DEFUN([AX_PTHREAD_CHECK_ENABLE],
- [AX_COMMON_ARG_WITH(
-  [pthread],
-  [pthread],
-  [search for pthread in includedir and libdir or in the specified DIR, or no if not to use pthread],
-  [auto-detect],
-  [DIR])
-
- dnl Check for a shared library version
- AX_PTHREAD_CHECK_LIB
-
- AS_IF(
-  [test "x$ac_cv_pthread_CPPFLAGS" != "x"],
-  [AC_SUBST(
-   [PTHREAD_CPPFLAGS],
-   [$ac_cv_pthread_CPPFLAGS])
-  ])
- AS_IF(
-  [test "x$ac_cv_pthread_LIBADD" != "x"],
-  [AC_SUBST(
-   [PTHREAD_LIBADD],
-   [$ac_cv_pthread_LIBADD])
-  ])
+  [AX_COMMON_ARG_WITH(
+    [pthread],
+    [pthread],
+    [search for pthread in includedir and libdir or in the specified DIR, or no if not to use pthread],
+    [auto-detect],
+    [DIR])
 
- AS_IF(
-  [test "x$ac_cv_pthread" = xpthread],
-  [AC_SUBST(
-   [ax_pthread_pc_libs_private],
-   [-lpthread])
+  dnl Check for a shared library version
+  AX_PTHREAD_CHECK_LIB
+
+  AS_IF(
+    [test "x$ac_cv_pthread_CPPFLAGS" != "x"],
+    [AC_SUBST(
+      [PTHREAD_CPPFLAGS],
+      [$ac_cv_pthread_CPPFLAGS])
+    ])
+  AS_IF(
+    [test "x$ac_cv_pthread_LIBADD" != "x"],
+    [AC_SUBST(
+      [PTHREAD_LIBADD],
+      [$ac_cv_pthread_LIBADD])
+    ])
+
+  AS_IF(
+    [test "x$ac_cv_pthread" = xpthread],
+    [AC_SUBST(
+      [ax_pthread_pc_libs_private],
+      [-lpthread])
+    ])
   ])
- ])
```

### Comparing `libesedb-20240202/include/libesedb/definitions.h.in` & `libesedb-20240420/include/libesedb/definitions.h.in`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/include/libesedb/definitions.h` & `libesedb-20240420/include/libesedb/definitions.h`

 * *Files 0% similar despite different names*

```diff
@@ -20,19 +20,19 @@
  */
 
 #if !defined( _LIBESEDB_DEFINITIONS_H )
 #define _LIBESEDB_DEFINITIONS_H
 
 #include <libesedb/types.h>
 
-#define LIBESEDB_VERSION				20240202
+#define LIBESEDB_VERSION				20240420
 
 /* The version string
  */
-#define LIBESEDB_VERSION_STRING				"20240202"
+#define LIBESEDB_VERSION_STRING				"20240420"
 
 /* The access flags definitions
  * bit 1        set to 1 for read access
  * bit 2        set to 1 for write access
  * bit 3-8      not used
  */
 enum LIBESEDB_ACCESS_FLAGS
```

### Comparing `libesedb-20240202/include/libesedb/types.h.in` & `libesedb-20240420/include/libesedb/types.h.in`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/include/libesedb/types.h` & `libesedb-20240420/include/libesedb/types.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/include/libesedb/features.h.in` & `libesedb-20240420/include/libesedb/features.h.in`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/include/libesedb/error.h` & `libesedb-20240420/include/libesedb/error.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/include/libesedb/extern.h` & `libesedb-20240420/include/libesedb/extern.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/include/libesedb/features.h` & `libesedb-20240420/include/libesedb/features.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/include/libesedb/codepage.h` & `libesedb-20240420/include/libesedb/codepage.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/include/libesedb.h` & `libesedb-20240420/include/libesedb.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/include/Makefile.in` & `libesedb-20240420/include/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -546,15 +546,20 @@
 
 EXTRA_DIST = \
 	libesedb.h.in \
 	libesedb/definitions.h.in \
 	libesedb/features.h.in \
 	libesedb/types.h.in
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	libesedb.h \
+	libesedb/definitions.h \
+	libesedb/features.h \
+	libesedb/types.h \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
 	@for dep in $?; do \
@@ -751,23 +756,25 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool mostlyclean-am
 
+distclean: distclean-am
+	-rm -f Makefile
 distclean-am: clean-am distclean-generic distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
 html: html-am
@@ -849,17 +856,10 @@
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am uninstall-includeHEADERS \
 	uninstall-pkgincludeHEADERS
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f libesedb.h
-	-rm -f libesedb/definitions.h
-	-rm -f libesedb/features.h
-	-rm -f libesedb/types.h
-	-rm -f Makefile
-
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libesedb-20240202/include/libesedb.h.in` & `libesedb-20240420/include/libesedb.h.in`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/common/config_borlandc.h` & `libesedb-20240420/common/config_borlandc.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/common/file_stream.h` & `libesedb-20240420/common/file_stream.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/common/memory.h` & `libesedb-20240420/common/memory.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/common/byte_stream.h` & `libesedb-20240420/common/byte_stream.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/common/common.h` & `libesedb-20240420/common/common.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/common/config_winapi.h` & `libesedb-20240420/common/config_winapi.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/common/system_string.h` & `libesedb-20240420/common/system_string.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/common/types.h.in` & `libesedb-20240420/common/types.h.in`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/common/types.h` & `libesedb-20240420/common/types.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/common/config.h.in` & `libesedb-20240420/common/config.h.in`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/common/config.h` & `libesedb-20240420/common/config.h`

 * *Files 1% similar despite different names*

```diff
@@ -559,24 +559,24 @@
 /* Define to the address where bug reports for this package should be sent. */
 #define PACKAGE_BUGREPORT "joachim.metz@gmail.com"
 
 /* Define to the full name of this package. */
 #define PACKAGE_NAME "libesedb"
 
 /* Define to the full name and version of this package. */
-#define PACKAGE_STRING "libesedb 20240202"
+#define PACKAGE_STRING "libesedb 20240420"
 
 /* Define to the one symbol short name of this package. */
 #define PACKAGE_TARNAME "libesedb"
 
 /* Define to the home page for this package. */
 #define PACKAGE_URL ""
 
 /* Define to the version of this package. */
-#define PACKAGE_VERSION "20240202"
+#define PACKAGE_VERSION "20240420"
 
 /* The size of `int', as computed by sizeof. */
 #define SIZEOF_INT 4
 
 /* The size of `long', as computed by sizeof. */
 #define SIZEOF_LONG 8
 
@@ -597,15 +597,15 @@
 /* Define to 1 if strerror_r returns char *. */
 /* #undef STRERROR_R_CHAR_P */
 
 /* Define to 1 if your <sys/time.h> declares `struct tm'. */
 /* #undef TM_IN_SYS_TIME */
 
 /* Version number of package */
-#define VERSION "20240202"
+#define VERSION "20240420"
 
 /* Number of bits in a file offset, on hosts where this is settable. */
 /* #undef _FILE_OFFSET_BITS */
 
 /* Define for large files, on AIX-style hosts. */
 /* #undef _LARGE_FILES */
```

### Comparing `libesedb-20240202/common/wide_string.h` & `libesedb-20240420/common/wide_string.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/common/narrow_string.h` & `libesedb-20240420/common/narrow_string.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/common/config_msc.h` & `libesedb-20240420/common/config_msc.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/common/Makefile.in` & `libesedb-20240420/common/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -499,15 +499,17 @@
 sharedstatedir = @sharedstatedir@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
-AM_CPPFLAGS = -I$(top_srcdir)/include
+AM_CPPFLAGS = \
+	-I../include -I$(top_srcdir)/include
+
 EXTRA_DIST = \
 	byte_stream.h \
 	common.h \
 	config.h \
 	config_borlandc.h \
 	config_msc.h \
 	config_winapi.h \
@@ -515,15 +517,18 @@
 	memory.h \
 	narrow_string.h \
 	system_string.h \
 	types.h \
 	types.h.in \
 	wide_string.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	config.h \
+	types.h \
+	Makefile \
 	Makefile.in
 
 all: config.h
 	$(MAKE) $(AM_MAKEFLAGS) all-am
 
 .SUFFIXES:
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -691,23 +696,25 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool mostlyclean-am
 
+distclean: distclean-am
+	-rm -f Makefile
 distclean-am: clean-am distclean-generic distclean-hdr distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
 html: html-am
@@ -787,15 +794,10 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f config.h
-	-rm -f types.h
-	-rm -f Makefile
-
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libesedb-20240202/libclocale/libclocale_wide_string.c` & `libesedb-20240420/libclocale/libclocale_wide_string.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libclocale/libclocale_support.h` & `libesedb-20240420/libclocale/libclocale_support.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libclocale/Makefile.am` & `libesedb-20240420/libclocale/Makefile.am`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 if HAVE_LOCAL_LIBCLOCALE
 AM_CPPFLAGS = \
 	-DLOCALEDIR=\"$(datadir)/locale\" \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libclocale.la
 
 libclocale_la_SOURCES = \
 	libclocale_codepage.c libclocale_codepage.h \
 	libclocale_definitions.h \
@@ -14,19 +14,17 @@
 	libclocale_libcerror.h \
 	libclocale_locale.c libclocale_locale.h \
 	libclocale_support.c libclocale_support.h \
 	libclocale_unused.h \
 	libclocale_wide_string.c libclocale_wide_string.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libclocale ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libclocale_la_SOURCES)
```

### Comparing `libesedb-20240202/libclocale/libclocale_definitions.h` & `libesedb-20240420/libclocale/libclocale_definitions.h`

 * *Files 2% similar despite different names*

```diff
@@ -30,19 +30,19 @@
 #include <libclocale/definitions.h>
 
 /* The definitions in <libclocale/definitions.h> are copied here
  * for local use of libclocale
  */
 #else
 
-#define LIBCLOCALE_VERSION					20240107
+#define LIBCLOCALE_VERSION					20240414
 
 /* The libclocale version string
  */
-#define LIBCLOCALE_VERSION_STRING				"20240107"
+#define LIBCLOCALE_VERSION_STRING				"20240414"
 
 /* The codepage feature flag definitions
  */
 enum LIBCLOCALE_CODEPAGES_FEATURE_FLAGS
 {
 	LIBCLOCALE_CODEPAGE_FEATURE_FLAG_HAVE_ISO_8859		= 0x00000001UL,
 	LIBCLOCALE_CODEPAGE_FEATURE_FLAG_HAVE_KOI8		= 0x00000002UL,
```

### Comparing `libesedb-20240202/libclocale/libclocale_unused.h` & `libesedb-20240420/libclocale/libclocale_unused.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libclocale/libclocale_libcerror.h` & `libesedb-20240420/libclocale/libclocale_libcerror.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libclocale/libclocale_locale.h` & `libesedb-20240420/libclocale/libclocale_locale.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libclocale/libclocale_support.c` & `libesedb-20240420/libclocale/libclocale_support.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libclocale/libclocale_codepage.c` & `libesedb-20240420/libclocale/libclocale_codepage.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libclocale/libclocale_locale.c` & `libesedb-20240420/libclocale/libclocale_locale.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libclocale/Makefile.in` & `libesedb-20240420/libclocale/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -545,30 +545,31 @@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBCLOCALE_TRUE@AM_CPPFLAGS = \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	-DLOCALEDIR=\"$(datadir)/locale\" \
-@HAVE_LOCAL_LIBCLOCALE_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBCLOCALE_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBCLOCALE_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBCLOCALE_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	@LIBCERROR_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBCLOCALE_TRUE@noinst_LTLIBRARIES = libclocale.la
 @HAVE_LOCAL_LIBCLOCALE_TRUE@libclocale_la_SOURCES = \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	libclocale_codepage.c libclocale_codepage.h \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	libclocale_definitions.h \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	libclocale_extern.h \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	libclocale_libcerror.h \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	libclocale_locale.c libclocale_locale.h \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	libclocale_support.c libclocale_support.h \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	libclocale_unused.h \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	libclocale_wide_string.c libclocale_wide_string.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -771,24 +772,30 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libclocale_codepage.Plo
+	-rm -f ./$(DEPDIR)/libclocale_locale.Plo
+	-rm -f ./$(DEPDIR)/libclocale_support.Plo
+	-rm -f ./$(DEPDIR)/libclocale_wide_string.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -875,17 +882,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libclocale ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libclocale_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libesedb-20240202/libclocale/libclocale_extern.h` & `libesedb-20240420/libclocale/libclocale_extern.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libclocale/libclocale_wide_string.h` & `libesedb-20240420/libclocale/libclocale_wide_string.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libclocale/libclocale_codepage.h` & `libesedb-20240420/libclocale/libclocale_codepage.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfcache/libfcache_libcdata.h` & `libesedb-20240420/libfcache/libfcache_libcdata.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfcache/libfcache_types.h` & `libesedb-20240420/libfcache/libfcache_types.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfcache/libfcache_cache_value.c` & `libesedb-20240420/libfcache/libfcache_cache_value.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfcache/libfcache_unused.h` & `libesedb-20240420/libfcache/libfcache_unused.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfcache/Makefile.am` & `libesedb-20240420/libfcache/Makefile.am`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBFCACHE
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCTHREADS_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@PTHREAD_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libfcache.la
 
@@ -19,19 +19,17 @@
 	libfcache_libcdata.h \
 	libfcache_libcerror.h \
 	libfcache_support.c libfcache_support.h \
 	libfcache_types.h \
 	libfcache_unused.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libfcache ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfcache_la_SOURCES)
```

### Comparing `libesedb-20240202/libfcache/libfcache_support.h` & `libesedb-20240420/libfcache/libfcache_support.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfcache/libfcache_error.h` & `libesedb-20240420/libfcache/libfcache_error.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfcache/libfcache_support.c` & `libesedb-20240420/libfcache/libfcache_support.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfcache/libfcache_cache.h` & `libesedb-20240420/libfcache/libfcache_cache.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfcache/libfcache_error.c` & `libesedb-20240420/libfcache/libfcache_error.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfcache/libfcache_libcerror.h` & `libesedb-20240420/libfcache/libfcache_libcerror.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfcache/libfcache_date_time.c` & `libesedb-20240420/libfcache/libfcache_date_time.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfcache/libfcache_extern.h` & `libesedb-20240420/libfcache/libfcache_extern.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfcache/libfcache_cache_value.h` & `libesedb-20240420/libfcache/libfcache_cache_value.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfcache/Makefile.in` & `libesedb-20240420/libfcache/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -547,16 +547,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBFCACHE_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBFCACHE_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBFCACHE_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBFCACHE_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBFCACHE_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBFCACHE_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFCACHE_TRUE@	@LIBCTHREADS_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFCACHE_TRUE@	@LIBCDATA_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFCACHE_TRUE@	@PTHREAD_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBFCACHE_TRUE@noinst_LTLIBRARIES = libfcache.la
 @HAVE_LOCAL_LIBFCACHE_TRUE@libfcache_la_SOURCES = \
@@ -568,15 +568,16 @@
 @HAVE_LOCAL_LIBFCACHE_TRUE@	libfcache_extern.h \
 @HAVE_LOCAL_LIBFCACHE_TRUE@	libfcache_libcdata.h \
 @HAVE_LOCAL_LIBFCACHE_TRUE@	libfcache_libcerror.h \
 @HAVE_LOCAL_LIBFCACHE_TRUE@	libfcache_support.c libfcache_support.h \
 @HAVE_LOCAL_LIBFCACHE_TRUE@	libfcache_types.h \
 @HAVE_LOCAL_LIBFCACHE_TRUE@	libfcache_unused.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -780,24 +781,31 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libfcache_cache.Plo
+	-rm -f ./$(DEPDIR)/libfcache_cache_value.Plo
+	-rm -f ./$(DEPDIR)/libfcache_date_time.Plo
+	-rm -f ./$(DEPDIR)/libfcache_error.Plo
+	-rm -f ./$(DEPDIR)/libfcache_support.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -885,17 +893,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libfcache ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfcache_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libesedb-20240202/libfcache/libfcache_date_time.h` & `libesedb-20240420/libfcache/libfcache_date_time.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfcache/libfcache_definitions.h` & `libesedb-20240420/libfcache/libfcache_definitions.h`

 * *Files 6% similar despite different names*

```diff
@@ -29,19 +29,19 @@
 #if !defined( HAVE_LOCAL_LIBFCACHE )
 #include <libfcache/definitions.h>
 
 /* The definitions in <libfcache/definitions.h> are copied here
  * for local use of libfcache
  */
 #else
-#define LIBFCACHE_VERSION					20240112
+#define LIBFCACHE_VERSION					20240414
 
 /* The libfcache version string
  */
-#define LIBFCACHE_VERSION_STRING				"20240112"
+#define LIBFCACHE_VERSION_STRING				"20240414"
 
 /* The cache value flags definitions
  */
 enum LIBFCACHE_CACHE_VALUE_FLAGS
 {
 	/* The cache value is not managed by the library
 	 */
```

### Comparing `libesedb-20240202/libfcache/libfcache_cache.c` & `libesedb-20240420/libfcache/libfcache_cache.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/Makefile.am` & `libesedb-20240420/Makefile.am`

 * *Files 4% similar despite different names*

```diff
@@ -63,16 +63,23 @@
 EXTRA_DIST = \
 	$(DPKG_FILES) \
 	$(GETTEXT_FILES) \
 	$(PKGCONFIG_FILES) \
 	$(SETUP_PY_FILES) \
 	$(SPEC_FILES)
 
-MAINTAINERCLEANFILES = \
-	Makefile.in
+DISTCLEANFILES = \
+	config.status \
+	config.cache \
+	config.log \
+	libesedb.pc \
+	libesedb.spec \
+	Makefile \
+	Makefile.in \
+	po/Makevars
 
 pkgconfigdir = $(libdir)/pkgconfig
 
 pkgconfig_DATA = \
 	libesedb.pc
 
 libtool:
@@ -98,19 +105,7 @@
 	(cd $(srcdir)/libfdatetime && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libfguid && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libfvalue && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libfwnt && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libesedb && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/po && $(MAKE) $(AM_MAKEFLAGS))
 
-distclean: clean
-	-rm -f Makefile
-	-rm -f config.status
-	-rm -f config.cache
-	-rm -f config.log
-	-rm -f libesedb.pc
-	-rm -f libesedb.spec
-	@for dir in ${subdirs}; do \
-		(cd $$dir && $(MAKE) distclean) \
-		|| case "$(MFLAGS)" in *k*) fail=yes;; *) exit 1;; esac; \
-	done && test -z "$$fail"
-
```

### Comparing `libesedb-20240202/libbfio/libbfio_file_range.h` & `libesedb-20240420/libbfio/libbfio_file_range.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * File range functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libesedb-20240202/libbfio/libbfio_file_range_io_handle.c` & `libesedb-20240420/libbfio/libbfio_file_range_io_handle.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * File range IO handle functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libesedb-20240202/libbfio/libbfio_support.c` & `libesedb-20240420/libbfio/libbfio_support.c`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Support functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libesedb-20240202/libbfio/libbfio_libcpath.h` & `libesedb-20240420/libbfio/libbfio_libcpath.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal libcpath header
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libesedb-20240202/libbfio/libbfio_error.h` & `libesedb-20240420/libbfio/libbfio_error.h`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Error functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libesedb-20240202/libbfio/libbfio_libclocale.h` & `libesedb-20240420/libbfio/libbfio_libclocale.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libclocale header wrapper
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libesedb-20240202/libbfio/libbfio_error.c` & `libesedb-20240420/libbfio/libbfio_error.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Error functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libesedb-20240202/libbfio/libbfio_libuna.h` & `libesedb-20240420/libbfio/libbfio_libuna.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libuna header wrapper
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libesedb-20240202/libbfio/libbfio_file_io_handle.h` & `libesedb-20240420/libbfio/libbfio_file_io_handle.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * File IO handle functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libesedb-20240202/libbfio/libbfio_file_pool.h` & `libesedb-20240420/libbfio/libbfio_file_pool.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * File pool functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libesedb-20240202/libbfio/libbfio_file_range.c` & `libesedb-20240420/libbfio/libbfio_file_range.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * File range functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libesedb-20240202/libbfio/libbfio_types.h` & `libesedb-20240420/libbfio/libbfio_types.h`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal type definitions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libesedb-20240202/libbfio/libbfio_unused.h` & `libesedb-20240420/libbfio/libbfio_unused.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Definitions to silence compiler warnings about unused function attributes/parameters.
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libesedb-20240202/libbfio/libbfio_libcdata.h` & `libesedb-20240420/libbfio/libbfio_libcdata.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libcdata header wrapper
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libesedb-20240202/libbfio/libbfio_file.h` & `libesedb-20240420/libbfio/libbfio_file.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * File functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libesedb-20240202/libbfio/Makefile.am` & `libesedb-20240420/libbfio/Makefile.am`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBBFIO
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCTHREADS_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCSPLIT_CPPFLAGS@ \
 	@LIBCFILE_CPPFLAGS@ \
@@ -38,17 +38,17 @@
 	libbfio_pool.c libbfio_pool.h \
 	libbfio_support.c libbfio_support.h \
 	libbfio_system_string.c libbfio_system_string.h \
 	libbfio_types.h \
 	libbfio_unused.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	/bin/rm -f Makefile
+sources-local: $(BUILT_SOURCES)
 
-splint:
+splint-local:
 	@echo "Running splint on libbfio ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libbfio_la_SOURCES)
```

### Comparing `libesedb-20240202/libbfio/libbfio_libcfile.h` & `libesedb-20240420/libbfio/libbfio_libcfile.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal libcfile header
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libesedb-20240202/libbfio/libbfio_definitions.h` & `libesedb-20240420/libbfio/libbfio_definitions.h`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal definitions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -29,19 +29,19 @@
 #if !defined( HAVE_LOCAL_LIBBFIO )
 #include <libbfio/definitions.h>
 
 /* The definitions in <libbfio/definitions.h> are copied here
  * for local use of libbfio
  */
 #else
-#define LIBBFIO_VERSION					20221025
+#define LIBBFIO_VERSION					20240414
 
 /* The libbfio version string
  */
-#define LIBBFIO_VERSION_STRING				"20221025"
+#define LIBBFIO_VERSION_STRING				"20240414"
 
 /* The library flags definitions
  */
 enum LIBBFIO_FLAGS
 {
 	/* The IO handle is not managed by the library
 	 */
```

### Comparing `libesedb-20240202/libbfio/libbfio_codepage.h` & `libesedb-20240420/libbfio/libbfio_codepage.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Codepage functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libesedb-20240202/libbfio/libbfio_file_io_handle.c` & `libesedb-20240420/libbfio/libbfio_file_io_handle.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * File IO handle functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libesedb-20240202/libbfio/libbfio_support.h` & `libesedb-20240420/libbfio/libbfio_support.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Support functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libesedb-20240202/libbfio/libbfio_memory_range.h` & `libesedb-20240420/libbfio/libbfio_memory_range.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Memory range functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libesedb-20240202/libbfio/libbfio_file_pool.c` & `libesedb-20240420/libbfio/libbfio_file_pool.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * File pool functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libesedb-20240202/libbfio/libbfio_file_range_io_handle.h` & `libesedb-20240420/libbfio/libbfio_file_range_io_handle.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * File range IO handle functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libesedb-20240202/libbfio/libbfio_libcthreads.h` & `libesedb-20240420/libbfio/libbfio_libcthreads.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libcthreads header wrapper
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libesedb-20240202/libbfio/libbfio_system_string.h` & `libesedb-20240420/libbfio/libbfio_system_string.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * System string functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libesedb-20240202/libbfio/libbfio_memory_range_io_handle.c` & `libesedb-20240420/libbfio/libbfio_memory_range_io_handle.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Memory range IO handle functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libesedb-20240202/libbfio/libbfio_handle.c` & `libesedb-20240420/libbfio/libbfio_handle.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The handle functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libesedb-20240202/libbfio/libbfio_file.c` & `libesedb-20240420/libbfio/libbfio_file.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * File functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libesedb-20240202/libbfio/libbfio_handle.h` & `libesedb-20240420/libbfio/libbfio_handle.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The handle functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libesedb-20240202/libbfio/libbfio_memory_range.c` & `libesedb-20240420/libbfio/libbfio_memory_range.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Memory range functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libesedb-20240202/libbfio/libbfio_pool.c` & `libesedb-20240420/libbfio/libbfio_pool.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal pool functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libesedb-20240202/libbfio/libbfio_libcerror.h` & `libesedb-20240420/libbfio/libbfio_libcerror.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libcerror header wrapper
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libesedb-20240202/libbfio/Makefile.in` & `libesedb-20240420/libbfio/Makefile.in`

 * *Files 3% similar despite different names*

```diff
@@ -565,16 +565,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBBFIO_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBBFIO_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBBFIO_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBBFIO_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBBFIO_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBBFIO_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_LOCAL_LIBBFIO_TRUE@	@LIBCTHREADS_CPPFLAGS@ \
 @HAVE_LOCAL_LIBBFIO_TRUE@	@LIBCLOCALE_CPPFLAGS@ \
 @HAVE_LOCAL_LIBBFIO_TRUE@	@LIBCNOTIFY_CPPFLAGS@ \
 @HAVE_LOCAL_LIBBFIO_TRUE@	@LIBCDATA_CPPFLAGS@ \
 @HAVE_LOCAL_LIBBFIO_TRUE@	@LIBCSPLIT_CPPFLAGS@ \
 @HAVE_LOCAL_LIBBFIO_TRUE@	@LIBCFILE_CPPFLAGS@ \
@@ -605,15 +605,16 @@
 @HAVE_LOCAL_LIBBFIO_TRUE@	libbfio_memory_range_io_handle.c libbfio_memory_range_io_handle.h \
 @HAVE_LOCAL_LIBBFIO_TRUE@	libbfio_pool.c libbfio_pool.h \
 @HAVE_LOCAL_LIBBFIO_TRUE@	libbfio_support.c libbfio_support.h \
 @HAVE_LOCAL_LIBBFIO_TRUE@	libbfio_system_string.c libbfio_system_string.h \
 @HAVE_LOCAL_LIBBFIO_TRUE@	libbfio_types.h \
 @HAVE_LOCAL_LIBBFIO_TRUE@	libbfio_unused.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -824,24 +825,38 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libbfio_error.Plo
+	-rm -f ./$(DEPDIR)/libbfio_file.Plo
+	-rm -f ./$(DEPDIR)/libbfio_file_io_handle.Plo
+	-rm -f ./$(DEPDIR)/libbfio_file_pool.Plo
+	-rm -f ./$(DEPDIR)/libbfio_file_range.Plo
+	-rm -f ./$(DEPDIR)/libbfio_file_range_io_handle.Plo
+	-rm -f ./$(DEPDIR)/libbfio_handle.Plo
+	-rm -f ./$(DEPDIR)/libbfio_memory_range.Plo
+	-rm -f ./$(DEPDIR)/libbfio_memory_range_io_handle.Plo
+	-rm -f ./$(DEPDIR)/libbfio_pool.Plo
+	-rm -f ./$(DEPDIR)/libbfio_support.Plo
+	-rm -f ./$(DEPDIR)/libbfio_system_string.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -910,14 +925,16 @@
 
 ps-am:
 
 sources: sources-am
 
 sources-am: sources-local
 
+splint: splint-am
+
 splint-am: splint-local
 
 uninstall-am:
 
 .MAKE: install-am install-strip
 
 .PHONY: CTAGS GTAGS TAGS all all-am am--depfiles check check-am clean \
@@ -928,23 +945,22 @@
 	install-data install-data-am install-dvi install-dvi-am \
 	install-exec install-exec-am install-html install-html-am \
 	install-info install-info-am install-man install-pdf \
 	install-pdf-am install-ps install-ps-am install-strip \
 	installcheck installcheck-am installdirs maintainer-clean \
 	maintainer-clean-generic mostlyclean mostlyclean-compile \
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
-	sources-am sources-local splint splint-am splint-local tags \
-	tags-am uninstall uninstall-am
+	sources-am sources-local splint-am splint-local tags tags-am \
+	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	/bin/rm -f Makefile
+sources-local: $(BUILT_SOURCES)
 
-splint:
+splint-local:
 	@echo "Running splint on libbfio ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libbfio_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libesedb-20240202/libbfio/libbfio_system_string.c` & `libesedb-20240420/libbfio/libbfio_system_string.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * System string functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libesedb-20240202/libbfio/libbfio_memory_range_io_handle.h` & `libesedb-20240420/libbfio/libbfio_memory_range_io_handle.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Memory range IO handle functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libesedb-20240202/libbfio/libbfio_extern.h` & `libesedb-20240420/libbfio/libbfio_extern.h`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal extern definition
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libesedb-20240202/libbfio/libbfio_pool.h` & `libesedb-20240420/libbfio/libbfio_pool.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal pool functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libesedb-20240202/config.guess` & `libesedb-20240420/config.guess`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/dpkg/copyright` & `libesedb-20240420/dpkg/copyright`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/dpkg/control` & `libesedb-20240420/dpkg/control`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/dpkg/rules` & `libesedb-20240420/dpkg/rules`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/COPYING.LESSER` & `libesedb-20240420/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/esedbtools/esedbinfo.c` & `libesedb-20240420/esedbtools/esedbinfo.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/esedbtools/esedbtools_unused.h` & `libesedb-20240420/esedbtools/esedbtools_unused.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/esedbtools/esedbtools_libcfile.h` & `libesedb-20240420/esedbtools/esedbtools_libcfile.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/esedbtools/webcache.c` & `libesedb-20240420/esedbtools/webcache.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/esedbtools/esedbtools_libclocale.h` & `libesedb-20240420/esedbtools/esedbtools_libclocale.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/esedbtools/windows_search.c` & `libesedb-20240420/esedbtools/windows_search.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/esedbtools/esedbtools_libfwnt.h` & `libesedb-20240420/esedbtools/esedbtools_libfwnt.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/esedbtools/info_handle.h` & `libesedb-20240420/esedbtools/info_handle.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/esedbtools/esedbtools_libcnotify.h` & `libesedb-20240420/esedbtools/esedbtools_libcnotify.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/esedbtools/esedbtools_libfguid.h` & `libesedb-20240420/esedbtools/esedbtools_libfguid.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/esedbtools/esedbtools_output.h` & `libesedb-20240420/esedbtools/esedbtools_output.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/esedbtools/srumdb.c` & `libesedb-20240420/esedbtools/srumdb.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/esedbtools/esedbtools_libfmapi.h` & `libesedb-20240420/esedbtools/esedbtools_libfmapi.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/esedbtools/webcache.h` & `libesedb-20240420/esedbtools/webcache.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/esedbtools/esedbtools_output.c` & `libesedb-20240420/esedbtools/esedbtools_output.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/esedbtools/esedbtools_i18n.h` & `libesedb-20240420/esedbtools/esedbtools_i18n.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/esedbtools/windows_security.h` & `libesedb-20240420/esedbtools/windows_security.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/esedbtools/database_types.c` & `libesedb-20240420/esedbtools/database_types.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/esedbtools/export.c` & `libesedb-20240420/esedbtools/export.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/esedbtools/Makefile.am` & `libesedb-20240420/esedbtools/Makefile.am`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBCSPLIT_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ \
 	@LIBCFILE_CPPFLAGS@ \
@@ -96,19 +96,17 @@
 esedbinfo_LDADD = \
 	@LIBCNOTIFY_LIBADD@ \
 	@LIBCLOCALE_LIBADD@ \
 	../libesedb/libesedb.la \
 	@LIBCERROR_LIBADD@ \
 	@LIBINTL@
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 splint-local:
 	@echo "Running splint on esedbexport ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(esedbexport_SOURCES)
 	@echo "Running splint on esedbinfo ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(esedbinfo_SOURCES)
```

### Comparing `libesedb-20240202/esedbtools/windows_search_compression.c` & `libesedb-20240420/esedbtools/windows_search_compression.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/esedbtools/esedbtools_signal.c` & `libesedb-20240420/esedbtools/esedbtools_signal.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/esedbtools/esedbtools_getopt.h` & `libesedb-20240420/esedbtools/esedbtools_getopt.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/esedbtools/info_handle.c` & `libesedb-20240420/esedbtools/info_handle.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/esedbtools/export_handle.c` & `libesedb-20240420/esedbtools/export_handle.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/esedbtools/esedbtools_libuna.h` & `libesedb-20240420/esedbtools/esedbtools_libuna.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/esedbtools/esedbtools_libcdata.h` & `libesedb-20240420/esedbtools/esedbtools_libcdata.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/esedbtools/esedbtools_libfdatetime.h` & `libesedb-20240420/esedbtools/esedbtools_libfdatetime.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/esedbtools/esedbtools_system_string.c` & `libesedb-20240420/esedbtools/esedbtools_system_string.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/esedbtools/esedbtools_libbfio.h` & `libesedb-20240420/esedbtools/esedbtools_libbfio.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/esedbtools/log_handle.c` & `libesedb-20240420/esedbtools/log_handle.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/esedbtools/export.h` & `libesedb-20240420/esedbtools/export.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/esedbtools/esedbtools_signal.h` & `libesedb-20240420/esedbtools/esedbtools_signal.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/esedbtools/esedbexport.c` & `libesedb-20240420/esedbtools/esedbexport.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/esedbtools/esedbtools_libcerror.h` & `libesedb-20240420/esedbtools/esedbtools_libcerror.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/esedbtools/windows_search.h` & `libesedb-20240420/esedbtools/windows_search.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/esedbtools/export_handle.h` & `libesedb-20240420/esedbtools/export_handle.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/esedbtools/esedbtools_libfvalue.h` & `libesedb-20240420/esedbtools/esedbtools_libfvalue.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/esedbtools/esedbtools_libesedb.h` & `libesedb-20240420/esedbtools/esedbtools_libesedb.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/esedbtools/srumdb.h` & `libesedb-20240420/esedbtools/srumdb.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/esedbtools/esedbtools_libcpath.h` & `libesedb-20240420/esedbtools/esedbtools_libcpath.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/esedbtools/Makefile.in` & `libesedb-20240420/esedbtools/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -555,16 +555,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBCSPLIT_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ \
 	@LIBCFILE_CPPFLAGS@ \
@@ -651,15 +651,16 @@
 esedbinfo_LDADD = \
 	@LIBCNOTIFY_LIBADD@ \
 	@LIBCLOCALE_LIBADD@ \
 	../libesedb/libesedb.la \
 	@LIBCERROR_LIBADD@ \
 	@LIBINTL@
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -921,23 +922,42 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-binPROGRAMS clean-generic clean-libtool mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/database_types.Po
+	-rm -f ./$(DEPDIR)/esedbexport.Po
+	-rm -f ./$(DEPDIR)/esedbinfo.Po
+	-rm -f ./$(DEPDIR)/esedbtools_getopt.Po
+	-rm -f ./$(DEPDIR)/esedbtools_output.Po
+	-rm -f ./$(DEPDIR)/esedbtools_signal.Po
+	-rm -f ./$(DEPDIR)/esedbtools_system_string.Po
+	-rm -f ./$(DEPDIR)/exchange.Po
+	-rm -f ./$(DEPDIR)/export.Po
+	-rm -f ./$(DEPDIR)/export_handle.Po
+	-rm -f ./$(DEPDIR)/info_handle.Po
+	-rm -f ./$(DEPDIR)/log_handle.Po
+	-rm -f ./$(DEPDIR)/srumdb.Po
+	-rm -f ./$(DEPDIR)/webcache.Po
+	-rm -f ./$(DEPDIR)/windows_search.Po
+	-rm -f ./$(DEPDIR)/windows_search_compression.Po
+	-rm -f ./$(DEPDIR)/windows_security.Po
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -1037,17 +1057,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am uninstall-binPROGRAMS
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 splint-local:
 	@echo "Running splint on esedbexport ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(esedbexport_SOURCES)
 	@echo "Running splint on esedbinfo ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(esedbinfo_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libesedb-20240202/esedbtools/log_handle.h` & `libesedb-20240420/esedbtools/log_handle.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/esedbtools/exchange.h` & `libesedb-20240420/esedbtools/exchange.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/esedbtools/esedbtools_system_string.h` & `libesedb-20240420/esedbtools/esedbtools_system_string.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/esedbtools/exchange.c` & `libesedb-20240420/esedbtools/exchange.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/esedbtools/windows_search_compression.h` & `libesedb-20240420/esedbtools/windows_search_compression.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/esedbtools/windows_security.c` & `libesedb-20240420/esedbtools/windows_security.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/esedbtools/database_types.h` & `libesedb-20240420/esedbtools/database_types.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/esedbtools/esedbtools_getopt.c` & `libesedb-20240420/esedbtools/esedbtools_getopt.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/configure` & `libesedb-20240420/configure`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #! /bin/sh
 # Guess values for system-dependent variables and create Makefiles.
-# Generated by GNU Autoconf 2.71 for libesedb 20240202.
+# Generated by GNU Autoconf 2.71 for libesedb 20240420.
 #
 # Report bugs to <joachim.metz@gmail.com>.
 #
 #
 # Copyright (C) 1992-1996, 1998-2017, 2020-2021 Free Software Foundation,
 # Inc.
 #
@@ -617,16 +617,16 @@
 subdirs=
 MFLAGS=
 MAKEFLAGS=
 
 # Identity of this package.
 PACKAGE_NAME='libesedb'
 PACKAGE_TARNAME='libesedb'
-PACKAGE_VERSION='20240202'
-PACKAGE_STRING='libesedb 20240202'
+PACKAGE_VERSION='20240420'
+PACKAGE_STRING='libesedb 20240420'
 PACKAGE_BUGREPORT='joachim.metz@gmail.com'
 PACKAGE_URL=''
 
 ac_unique_file="include/libesedb.h.in"
 # Factoring default headers for most tests.
 ac_includes_default="\
 #include <stddef.h>
@@ -1696,15 +1696,15 @@
 #
 # Report the --help message.
 #
 if test "$ac_init_help" = "long"; then
   # Omit some internal or obsolete options to make the list less imposing.
   # This message is too long to be a string in the A/UX 3.1 sh.
   cat <<_ACEOF
-\`configure' configures libesedb 20240202 to adapt to many kinds of systems.
+\`configure' configures libesedb 20240420 to adapt to many kinds of systems.
 
 Usage: $0 [OPTION]... [VAR=VALUE]...
 
 To assign environment variables (e.g., CC, CFLAGS...), specify them as
 VAR=VALUE.  See below for descriptions of some of the useful variables.
 
 Defaults for the options are specified in brackets.
@@ -1767,15 +1767,15 @@
   --build=BUILD     configure for building on BUILD [guessed]
   --host=HOST       cross-compile to build programs to run on HOST [BUILD]
 _ACEOF
 fi
 
 if test -n "$ac_init_help"; then
   case $ac_init_help in
-     short | recursive ) echo "Configuration of libesedb 20240202:";;
+     short | recursive ) echo "Configuration of libesedb 20240420:";;
    esac
   cat <<\_ACEOF
 
 Optional Features:
   --disable-option-checking  ignore unrecognized --enable/--with options
   --disable-FEATURE       do not include FEATURE (same as --enable-FEATURE=no)
   --enable-FEATURE[=ARG]  include FEATURE [ARG=yes]
@@ -2040,15 +2040,15 @@
     cd "$ac_pwd" || { ac_status=$?; break; }
   done
 fi
 
 test -n "$ac_init_help" && exit $ac_status
 if $ac_init_version; then
   cat <<\_ACEOF
-libesedb configure 20240202
+libesedb configure 20240420
 generated by GNU Autoconf 2.71
 
 Copyright (C) 2021 Free Software Foundation, Inc.
 This configure script is free software; the Free Software Foundation
 gives unlimited permission to copy, distribute and modify it.
 _ACEOF
   exit
@@ -2761,15 +2761,15 @@
     ac_configure_args_raw=`      printf "%s\n" "$ac_configure_args_raw" | sed "$ac_safe_unquote"`;;
 esac
 
 cat >config.log <<_ACEOF
 This file contains any messages produced by compilers while
 running configure, to aid debugging if configure makes a mistake.
 
-It was created by libesedb $as_me 20240202, which was
+It was created by libesedb $as_me 20240420, which was
 generated by GNU Autoconf 2.71.  Invocation command line was
 
   $ $0$ac_configure_args_raw
 
 _ACEOF
 exec 5>>config.log
 {
@@ -4250,15 +4250,15 @@
     CYGPATH_W=echo
   fi
 fi
 
 
 # Define the identity of the package.
  PACKAGE='libesedb'
- VERSION='20240202'
+ VERSION='20240420'
 
 
 printf "%s\n" "#define PACKAGE \"$PACKAGE\"" >>confdefs.h
 
 
 printf "%s\n" "#define VERSION \"$VERSION\"" >>confdefs.h
 
@@ -23845,15 +23845,15 @@
 printf "%s\n" "$ac_cv_with_libcerror" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcerror" = xno
 then :
   ac_cv_libcerror=no
 else $as_nop
   ac_cv_libcerror=check
-        if test "x$ac_cv_with_libcerror" != x && test "x$ac_cv_with_libcerror" != xauto-detect
+                if test "x$ac_cv_with_libcerror" != x && test "x$ac_cv_with_libcerror" != xauto-detect && test "x$ac_cv_with_libcerror" != xyes
 then :
   if test -d "$ac_cv_with_libcerror"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libcerror}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcerror}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -24344,15 +24344,16 @@
 fi
 
 
         ac_cv_libcerror_LIBADD="-lcerror"
 fi
 
 fi
-    if test "x$ac_cv_with_libcerror" != x && test "x$ac_cv_with_libcerror" != xauto-detect && test "x$ac_cv_libcerror" != xyes
+
+    if test "x$ac_cv_libcerror" != xyes && test "x$ac_cv_with_libcerror" != x && test "x$ac_cv_with_libcerror" != xauto-detect && test "x$ac_cv_with_libcerror" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libcerror in directory: $ac_cv_with_libcerror
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -24494,15 +24495,15 @@
 as_fn_error 1 "Missing functions: strerror_r and strerror
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
 
 fi
 
-  ac_cv_libcerror_CPPFLAGS="-I../libcerror";
+  ac_cv_libcerror_CPPFLAGS="-I../libcerror -I\$(top_srcdir)/libcerror";
   ac_cv_libcerror_LIBADD="../libcerror/libcerror.la";
 
   ac_cv_libcerror=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCERROR 1" >>confdefs.h
@@ -24596,15 +24597,15 @@
     ac_cv_libcthreads_multi_threading="no"
 else $as_nop
       if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcthreads" = xno
 then :
   ac_cv_libcthreads=no
 else $as_nop
   ac_cv_libcthreads=check
-        if test "x$ac_cv_with_libcthreads" != x && test "x$ac_cv_with_libcthreads" != xauto-detect
+                if test "x$ac_cv_with_libcthreads" != x && test "x$ac_cv_with_libcthreads" != xauto-detect && test "x$ac_cv_with_libcthreads" != xyes
 then :
   if test -d "$ac_cv_with_libcthreads"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libcthreads}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcthreads}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -26236,15 +26237,15 @@
 
 
         ac_cv_libcthreads_LIBADD="-lcthreads"
 fi
 
 fi
 
-    if test "x$ac_cv_with_libcthreads" != x && test "x$ac_cv_with_libcthreads" != xauto-detect && test "x$ac_cv_libcthreads" != xyes
+    if test "x$ac_cv_libcthreads" != xyes && test "x$ac_cv_with_libcthreads" != x && test "x$ac_cv_with_libcthreads" != xauto-detect && test "x$ac_cv_with_libcthreads" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libcthreads in directory: $ac_cv_with_libcthreads
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -26298,47 +26299,52 @@
   printf %s "(cached) " >&6
 else $as_nop
   ac_cv_with_pthread=auto-detect
 fi
 { printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_with_pthread" >&5
 printf "%s\n" "$ac_cv_with_pthread" >&6; }
 
-   if test "x$ac_cv_with_pthread" != x && test "x$ac_cv_with_pthread" != xno && test "x$ac_cv_with_pthread" != xauto-detect
+    if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_pthread" = xno
+then :
+  ac_cv_pthread=no
+else $as_nop
+  ac_cv_pthread=check
+                if test "x$ac_cv_with_pthread" != x && test "x$ac_cv_with_pthread" != xauto-detect && test "x$ac_cv_with_pthread" != xyes
 then :
   if test -d "$ac_cv_with_pthread"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_pthread}/include"
-   LDFLAGS="$LDFLAGS -L${ac_cv_with_pthread}/lib"
+        LDFLAGS="$LDFLAGS -L${ac_cv_with_pthread}/lib"
 else $as_nop
   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: WARNING: no such directory: $ac_cv_with_pthread" >&5
 printf "%s\n" "$as_me: WARNING: no such directory: $ac_cv_with_pthread" >&2;}
 
 fi
 
 fi
 
- if test "x$ac_cv_with_pthread" = xno
+fi
+
+    if test "x$ac_cv_pthread" = xcheck
 then :
-  ac_cv_pthread=no
-else $as_nop
-    ac_fn_c_check_header_compile "$LINENO" "pthread.h" "ac_cv_header_pthread_h" "$ac_includes_default"
+        ac_fn_c_check_header_compile "$LINENO" "pthread.h" "ac_cv_header_pthread_h" "$ac_includes_default"
 if test "x$ac_cv_header_pthread_h" = xyes
 then :
   printf "%s\n" "#define HAVE_PTHREAD_H 1" >>confdefs.h
 
 fi
 
 
-  if test "x$ac_cv_header_pthread_h" = xno
+      if test "x$ac_cv_header_pthread_h" = xno
 then :
   ac_cv_pthread=no
 else $as_nop
-     ac_cv_pthread=pthread
+          ac_cv_pthread=pthread
 
-      { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_create in -lpthread" >&5
+                { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_create in -lpthread" >&5
 printf %s "checking for pthread_create in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_create+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26372,15 +26378,15 @@
 if test "x$ac_cv_lib_pthread_pthread_create" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_exit in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_exit in -lpthread" >&5
 printf %s "checking for pthread_exit in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_exit+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26414,15 +26420,15 @@
 if test "x$ac_cv_lib_pthread_pthread_exit" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_join in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_join in -lpthread" >&5
 printf %s "checking for pthread_join in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_join+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26457,15 +26463,15 @@
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
 
-      { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_init in -lpthread" >&5
+                { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_init in -lpthread" >&5
 printf %s "checking for pthread_cond_init in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_cond_init+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26499,15 +26505,15 @@
 if test "x$ac_cv_lib_pthread_pthread_cond_init" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_destroy in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_destroy in -lpthread" >&5
 printf %s "checking for pthread_cond_destroy in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_cond_destroy+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26541,15 +26547,15 @@
 if test "x$ac_cv_lib_pthread_pthread_cond_destroy" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_broadcast in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_broadcast in -lpthread" >&5
 printf %s "checking for pthread_cond_broadcast in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_cond_broadcast+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26583,15 +26589,15 @@
 if test "x$ac_cv_lib_pthread_pthread_cond_broadcast" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_signal in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_signal in -lpthread" >&5
 printf %s "checking for pthread_cond_signal in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_cond_signal+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26625,15 +26631,15 @@
 if test "x$ac_cv_lib_pthread_pthread_cond_signal" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_wait in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_wait in -lpthread" >&5
 printf %s "checking for pthread_cond_wait in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_cond_wait+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26668,15 +26674,15 @@
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
 
-      { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_init in -lpthread" >&5
+                { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_init in -lpthread" >&5
 printf %s "checking for pthread_mutex_init in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_mutex_init+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26710,15 +26716,15 @@
 if test "x$ac_cv_lib_pthread_pthread_mutex_init" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_destroy in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_destroy in -lpthread" >&5
 printf %s "checking for pthread_mutex_destroy in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_mutex_destroy+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26752,15 +26758,15 @@
 if test "x$ac_cv_lib_pthread_pthread_mutex_destroy" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_lock in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_lock in -lpthread" >&5
 printf %s "checking for pthread_mutex_lock in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_mutex_lock+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26794,15 +26800,15 @@
 if test "x$ac_cv_lib_pthread_pthread_mutex_lock" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_trylock in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_trylock in -lpthread" >&5
 printf %s "checking for pthread_mutex_trylock in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_mutex_trylock+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26836,15 +26842,15 @@
 if test "x$ac_cv_lib_pthread_pthread_mutex_trylock" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_unlock in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_unlock in -lpthread" >&5
 printf %s "checking for pthread_mutex_unlock in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_mutex_unlock+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26879,15 +26885,15 @@
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
 
-      { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_init in -lpthread" >&5
+                { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_init in -lpthread" >&5
 printf %s "checking for pthread_rwlock_init in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_rwlock_init+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26921,15 +26927,15 @@
 if test "x$ac_cv_lib_pthread_pthread_rwlock_init" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_destroy in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_destroy in -lpthread" >&5
 printf %s "checking for pthread_rwlock_destroy in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_rwlock_destroy+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26963,15 +26969,15 @@
 if test "x$ac_cv_lib_pthread_pthread_rwlock_destroy" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_rdlock in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_rdlock in -lpthread" >&5
 printf %s "checking for pthread_rwlock_rdlock in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_rwlock_rdlock+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -27005,15 +27011,15 @@
 if test "x$ac_cv_lib_pthread_pthread_rwlock_rdlock" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_wrlock in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_wrlock in -lpthread" >&5
 printf %s "checking for pthread_rwlock_wrlock in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_rwlock_wrlock+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -27047,15 +27053,15 @@
 if test "x$ac_cv_lib_pthread_pthread_rwlock_wrlock" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_unlock in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_unlock in -lpthread" >&5
 printf %s "checking for pthread_rwlock_unlock in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_rwlock_unlock+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -27090,67 +27096,76 @@
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
 
-   ac_cv_pthread_LIBADD="-lpthread";
+        ac_cv_pthread_LIBADD="-lpthread";
 
 fi
 
+    if test "x$ac_cv_with_pthread" != x && test "x$ac_cv_with_pthread" != xauto-detect && test "x$ac_cv_with_pthread" != xyes
+then :
+  { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
+printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
+as_fn_error 1 "unable to find supported pthread in directory: $ac_cv_with_pthread
+See \`config.log' for more details" "$LINENO" 5; }
+
 fi
 
- if test "x$ac_cv_pthread" = xpthread
+fi
+
+  if test "x$ac_cv_pthread" = xpthread
 then :
 
 printf "%s\n" "#define HAVE_PTHREAD 1" >>confdefs.h
 
 
 fi
 
- if test "x$ac_cv_pthread" != xno
+  if test "x$ac_cv_pthread" != xno
 then :
   HAVE_PTHREAD=1
 
 else $as_nop
   HAVE_PTHREAD=0
 
 
 fi
 
 
- if test "x$ac_cv_pthread_CPPFLAGS" != "x"
+  if test "x$ac_cv_pthread_CPPFLAGS" != "x"
 then :
   PTHREAD_CPPFLAGS=$ac_cv_pthread_CPPFLAGS
 
 
 fi
- if test "x$ac_cv_pthread_LIBADD" != "x"
+  if test "x$ac_cv_pthread_LIBADD" != "x"
 then :
   PTHREAD_LIBADD=$ac_cv_pthread_LIBADD
 
 
 fi
 
- if test "x$ac_cv_pthread" = xpthread
+  if test "x$ac_cv_pthread" = xpthread
 then :
   ax_pthread_pc_libs_private=-lpthread
 
 
 fi
 
       ac_cv_libcthreads_multi_threading=$ac_cv_pthread
 else $as_nop
   ac_cv_libcthreads_multi_threading="winapi"
 fi
 
   if test "x$ac_cv_libcthreads_multi_threading" != xno
 then :
-  ac_cv_libcthreads_CPPFLAGS="-I../libcthreads";
+  ac_cv_libcthreads_CPPFLAGS="-I../libcthreads -I\$(top_srcdir)/libcthreads";
     ac_cv_libcthreads_LIBADD="../libcthreads/libcthreads.la";
 
     ac_cv_libcthreads=local
 else $as_nop
   ac_cv_libcthreads=no
 fi
 
@@ -27238,15 +27253,15 @@
 printf "%s\n" "$ac_cv_with_libcdata" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcdata" = xno
 then :
   ac_cv_libcdata=no
 else $as_nop
   ac_cv_libcdata=check
-        if test "x$ac_cv_with_libcdata" != x && test "x$ac_cv_with_libcdata" != xauto-detect
+                if test "x$ac_cv_with_libcdata" != x && test "x$ac_cv_with_libcdata" != xauto-detect && test "x$ac_cv_with_libcdata" != xyes
 then :
   if test -d "$ac_cv_with_libcdata"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libcdata}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcdata}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -31017,15 +31032,16 @@
 fi
 
 
         ac_cv_libcdata_LIBADD="-lcdata"
 fi
 
 fi
-    if test "x$ac_cv_with_libcdata" != x && test "x$ac_cv_with_libcdata" != xauto-detect && test "x$ac_cv_libcdata" != xyes
+
+    if test "x$ac_cv_libcdata" != xyes && test "x$ac_cv_with_libcdata" != x && test "x$ac_cv_with_libcdata" != xauto-detect && test "x$ac_cv_with_libcdata" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libcdata in directory: $ac_cv_with_libcdata
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -31050,15 +31066,15 @@
 
 fi
 
 
     if test "x$ac_cv_libcdata" != xyes
 then :
 
-  ac_cv_libcdata_CPPFLAGS="-I../libcdata";
+  ac_cv_libcdata_CPPFLAGS="-I../libcdata -I\$(top_srcdir)/libcdata";
   ac_cv_libcdata_LIBADD="../libcdata/libcdata.la";
 
   ac_cv_libcdata=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCDATA 1" >>confdefs.h
@@ -31128,15 +31144,15 @@
 printf "%s\n" "$ac_cv_with_libclocale" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libclocale" = xno
 then :
   ac_cv_libclocale=no
 else $as_nop
   ac_cv_libclocale=check
-        if test "x$ac_cv_with_libclocale" != x && test "x$ac_cv_with_libclocale" != xauto-detect
+                if test "x$ac_cv_with_libclocale" != x && test "x$ac_cv_with_libclocale" != xauto-detect && test "x$ac_cv_with_libclocale" != xyes
 then :
   if test -d "$ac_cv_with_libclocale"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libclocale}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libclocale}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -31683,15 +31699,16 @@
 fi
 
 
         ac_cv_libclocale_LIBADD="-lclocale"
 fi
 
 fi
-    if test "x$ac_cv_with_libclocale" != x && test "x$ac_cv_with_libclocale" != xauto-detect && test "x$ac_cv_libclocale" != xyes
+
+    if test "x$ac_cv_libclocale" != xyes && test "x$ac_cv_with_libclocale" != x && test "x$ac_cv_with_libclocale" != xauto-detect && test "x$ac_cv_with_libclocale" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libclocale in directory: $ac_cv_with_libclocale
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -31847,15 +31864,15 @@
 
 printf "%s\n" "#define HAVE_LANGINFO_CODESET 1" >>confdefs.h
 
 
 fi
 
 
-  ac_cv_libclocale_CPPFLAGS="-I../libclocale";
+  ac_cv_libclocale_CPPFLAGS="-I../libclocale -I\$(top_srcdir)/libclocale";
   ac_cv_libclocale_LIBADD="../libclocale/libclocale.la";
 
   ac_cv_libclocale=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCLOCALE 1" >>confdefs.h
@@ -31925,15 +31942,15 @@
 printf "%s\n" "$ac_cv_with_libcnotify" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcnotify" = xno
 then :
   ac_cv_libcnotify=no
 else $as_nop
   ac_cv_libcnotify=check
-        if test "x$ac_cv_with_libcnotify" != x && test "x$ac_cv_with_libcnotify" != xauto-detect
+                if test "x$ac_cv_with_libcnotify" != x && test "x$ac_cv_with_libcnotify" != xauto-detect && test "x$ac_cv_with_libcnotify" != xyes
 then :
   if test -d "$ac_cv_with_libcnotify"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libcnotify}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcnotify}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -32383,15 +32400,16 @@
 fi
 
 
         ac_cv_libcnotify_LIBADD="-lcnotify"
 fi
 
 fi
-    if test "x$ac_cv_with_libcnotify" != x && test "x$ac_cv_with_libcnotify" != xauto-detect && test "x$ac_cv_libcnotify" != xyes
+
+    if test "x$ac_with_libcnotify" != xyes && test "x$ac_cv_with_libcnotify" != x && test "x$ac_cv_with_libcnotify" != xauto-detect && test "x$ac_cv_with_libcnotify" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libcnotify in directory: $ac_cv_with_libcnotify
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -32446,15 +32464,15 @@
 if test "x$ac_cv_header_errno_h" = xyes
 then :
   printf "%s\n" "#define HAVE_ERRNO_H 1" >>confdefs.h
 
 fi
 
 
-  ac_cv_libcnotify_CPPFLAGS="-I../libcnotify";
+  ac_cv_libcnotify_CPPFLAGS="-I../libcnotify -I\$(top_srcdir)/libcnotify";
   ac_cv_libcnotify_LIBADD="../libcnotify/libcnotify.la";
 
   ac_cv_libcnotify=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCNOTIFY 1" >>confdefs.h
@@ -32524,15 +32542,15 @@
 printf "%s\n" "$ac_cv_with_libcsplit" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcsplit" = xno
 then :
   ac_cv_libcsplit=no
 else $as_nop
   ac_cv_libcsplit=check
-        if test "x$ac_cv_with_libcsplit" != x && test "x$ac_cv_with_libcsplit" != xauto-detect
+                if test "x$ac_cv_with_libcsplit" != x && test "x$ac_cv_with_libcsplit" != xauto-detect && test "x$ac_cv_with_libcsplit" != xyes
 then :
   if test -d "$ac_cv_with_libcsplit"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libcsplit}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcsplit}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -33247,15 +33265,16 @@
 
 fi
 
         ac_cv_libcsplit_LIBADD="-lcsplit"
 fi
 
 fi
-    if test "x$ac_cv_with_libcsplit" != x && test "x$ac_cv_with_libcsplit" != xauto-detect && test "x$ac_cv_libcsplit" != xyes
+
+    if test "x$ac_cv_libcsplit" != xyes && test "x$ac_cv_with_libcsplit" != x && test "x$ac_cv_with_libcsplit" != xauto-detect && test "x$ac_cv_with_libcsplit" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libcsplit in directory: $ac_cv_with_libcsplit
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -33280,15 +33299,15 @@
 
 fi
 
 
     if test "x$ac_cv_libcsplit" != xyes
 then :
 
-  ac_cv_libcsplit_CPPFLAGS="-I../libcsplit";
+  ac_cv_libcsplit_CPPFLAGS="-I../libcsplit -I\$(top_srcdir)/libcsplit";
   ac_cv_libcsplit_LIBADD="../libcsplit/libcsplit.la";
 
   ac_cv_libcsplit=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCSPLIT 1" >>confdefs.h
@@ -33358,15 +33377,15 @@
 printf "%s\n" "$ac_cv_with_libuna" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libuna" = xno
 then :
   ac_cv_libuna=no
 else $as_nop
   ac_cv_libuna=check
-        if test "x$ac_cv_with_libuna" != x && test "x$ac_cv_with_libuna" != xauto-detect
+                if test "x$ac_cv_with_libuna" != x && test "x$ac_cv_with_libuna" != xauto-detect && test "x$ac_cv_with_libuna" != xyes
 then :
   if test -d "$ac_cv_with_libuna"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libuna}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libuna}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -40568,15 +40587,16 @@
   ac_cv_libuna=no
 fi
 
         ac_cv_libuna_LIBADD="-luna"
 fi
 
 fi
-    if test "x$ac_cv_with_libuna" != x && test "x$ac_cv_with_libuna" != xauto-detect && test "x$ac_cv_libuna" != xyes
+
+    if test "x$ac_cv_libuna" != xyes && test "x$ac_cv_with_libuna" != x && test "x$ac_cv_with_libuna" != xauto-detect && test "x$ac_cv_with_libuna" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libuna in directory: $ac_cv_with_libuna
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -40601,15 +40621,15 @@
 
 fi
 
 
     if test "x$ac_cv_libuna" != xyes
 then :
 
-  ac_cv_libuna_CPPFLAGS="-I../libuna";
+  ac_cv_libuna_CPPFLAGS="-I../libuna -I\$(top_srcdir)/libuna";
   ac_cv_libuna_LIBADD="../libuna/libuna.la";
 
   ac_cv_libuna=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBUNA 1" >>confdefs.h
@@ -40679,15 +40699,15 @@
 printf "%s\n" "$ac_cv_with_libcfile" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcfile" = xno
 then :
   ac_cv_libcfile=no
 else $as_nop
   ac_cv_libcfile=check
-        if test "x$ac_cv_with_libcfile" != x && test "x$ac_cv_with_libcfile" != xauto-detect
+                if test "x$ac_cv_with_libcfile" != x && test "x$ac_cv_with_libcfile" != xauto-detect && test "x$ac_cv_with_libcfile" != xyes
 then :
   if test -d "$ac_cv_with_libcfile"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libcfile}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcfile}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -41868,15 +41888,16 @@
 
 fi
 
         ac_cv_libcfile_LIBADD="-lcfile"
 fi
 
 fi
-    if test "x$ac_cv_with_libcfile" != x && test "x$ac_cv_with_libcfile" != xauto-detect && test "x$ac_cv_libcfile" != xyes
+
+    if test "x$ac_cv_libcfile" != xyes && test "x$ac_cv_with_libcfile" != x && test "x$ac_cv_with_libcfile" != xauto-detect && test "x$ac_cv_with_libcfile" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libcfile in directory: $ac_cv_with_libcfile
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -42190,15 +42211,15 @@
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "Missing function: unlink
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
 
-  ac_cv_libcfile_CPPFLAGS="-I../libcfile";
+  ac_cv_libcfile_CPPFLAGS="-I../libcfile -I\$(top_srcdir)/libcfile";
   ac_cv_libcfile_LIBADD="../libcfile/libcfile.la";
 
   ac_cv_libcfile=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCFILE 1" >>confdefs.h
@@ -42268,15 +42289,15 @@
 printf "%s\n" "$ac_cv_with_libcpath" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcpath" = xno
 then :
   ac_cv_libcpath=no
 else $as_nop
   ac_cv_libcpath=check
-        if test "x$ac_cv_with_libcpath" != x && test "x$ac_cv_with_libcpath" != xauto-detect
+                if test "x$ac_cv_with_libcpath" != x && test "x$ac_cv_with_libcpath" != xauto-detect && test "x$ac_cv_with_libcpath" != xyes
 then :
   if test -d "$ac_cv_with_libcpath"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libcpath}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcpath}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -43073,15 +43094,16 @@
 
 fi
 
         ac_cv_libcpath_LIBADD="-lcpath"
 fi
 
 fi
-    if test "x$ac_cv_with_libcpath" != x && test "x$ac_cv_with_libcpath" != xauto-detect && test "x$ac_cv_libcpath" != xyes
+
+    if test "x$ac_cv_libcpath" != xyes && test "x$ac_cv_with_libcpath" != x && test "x$ac_cv_with_libcpath" != xauto-detect && test "x$ac_cv_with_libcpath" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libcpath in directory: $ac_cv_with_libcpath
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -43271,15 +43293,15 @@
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "Missing function: mkdir
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
 
 
-  ac_cv_libcpath_CPPFLAGS="-I../libcpath";
+  ac_cv_libcpath_CPPFLAGS="-I../libcpath -I\$(top_srcdir)/libcpath";
   ac_cv_libcpath_LIBADD="../libcpath/libcpath.la";
 
   ac_cv_libcpath=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCPATH 1" >>confdefs.h
@@ -43349,15 +43371,15 @@
 printf "%s\n" "$ac_cv_with_libbfio" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libbfio" = xno
 then :
   ac_cv_libbfio=no
 else $as_nop
   ac_cv_libbfio=check
-        if test "x$ac_cv_with_libbfio" != x && test "x$ac_cv_with_libbfio" != xauto-detect
+                if test "x$ac_cv_with_libbfio" != x && test "x$ac_cv_with_libbfio" != xauto-detect && test "x$ac_cv_with_libbfio" != xyes
 then :
   if test -d "$ac_cv_with_libbfio"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libbfio}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libbfio}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -45467,15 +45489,16 @@
 
 fi
 
         ac_cv_libbfio_LIBADD="-lbfio"
 fi
 
 fi
-    if test "x$ac_cv_with_libbfio" != x && test "x$ac_cv_with_libbfio" != xauto-detect && test "x$ac_cv_libbfio" != xyes
+
+    if test "x$ac_cv_libbfio" != xyes && test "x$ac_cv_with_libbfio" != x && test "x$ac_cv_with_libbfio" != xauto-detect && test "x$ac_cv_with_libbfio" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libbfio in directory: $ac_cv_with_libbfio
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -45500,15 +45523,15 @@
 
 fi
 
 
     if test "x$ac_cv_libbfio" != xyes
 then :
 
-  ac_cv_libbfio_CPPFLAGS="-I../libbfio";
+  ac_cv_libbfio_CPPFLAGS="-I../libbfio -I\$(top_srcdir)/libbfio";
   ac_cv_libbfio_LIBADD="../libbfio/libbfio.la";
 
   ac_cv_libbfio=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBBFIO 1" >>confdefs.h
@@ -45578,15 +45601,15 @@
 printf "%s\n" "$ac_cv_with_libfcache" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libfcache" = xno
 then :
   ac_cv_libfcache=no
 else $as_nop
   ac_cv_libfcache=check
-        if test "x$ac_cv_with_libfcache" != x && test "x$ac_cv_with_libfcache" != xauto-detect
+                if test "x$ac_cv_with_libfcache" != x && test "x$ac_cv_with_libfcache" != xauto-detect && test "x$ac_cv_with_libfcache" != xyes
 then :
   if test -d "$ac_cv_with_libfcache"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libfcache}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libfcache}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -46498,15 +46521,16 @@
 fi
 
 
         ac_cv_libfcache_LIBADD="-lfcache"
 fi
 
 fi
-    if test "x$ac_cv_with_libfcache" != x && test "x$ac_cv_with_libfcache" != xauto-detect && test "x$ac_cv_libfcache" != xyes
+
+    if test "x$ac_cv_libfcache" != xyes && test "x$ac_cv_with_libfcache" != x && test "x$ac_cv_with_libfcache" != xauto-detect && test "x$ac_cv_with_libfcache" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libfcache in directory: $ac_cv_with_libfcache
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -46599,15 +46623,15 @@
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "Missing function: time
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
 
-  ac_cv_libfcache_CPPFLAGS="-I../libfcache";
+  ac_cv_libfcache_CPPFLAGS="-I../libfcache -I\$(top_srcdir)/libfcache";
   ac_cv_libfcache_LIBADD="../libfcache/libfcache.la";
 
   ac_cv_libfcache=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBFCACHE 1" >>confdefs.h
@@ -46677,15 +46701,15 @@
 printf "%s\n" "$ac_cv_with_libfdata" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libfdata" = xno
 then :
   ac_cv_libfdata=no
 else $as_nop
   ac_cv_libfdata=check
-        if test "x$ac_cv_with_libfdata" != x && test "x$ac_cv_with_libfdata" != xauto-detect
+                if test "x$ac_cv_with_libfdata" != x && test "x$ac_cv_with_libfdata" != xauto-detect && test "x$ac_cv_with_libfdata" != xyes
 then :
   if test -d "$ac_cv_with_libfdata"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libfdata}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libfdata}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -49965,15 +49989,16 @@
 
 
 
         ac_cv_libfdata_LIBADD="-lfdata"
 fi
 
 fi
-    if test "x$ac_cv_with_libfdata" != x && test "x$ac_cv_with_libfdata" != xauto-detect && test "x$ac_cv_libfdata" != xyes
+
+    if test "x$ac_cv_libfdata" != xyes && test "x$ac_cv_with_libfdata" != x && test "x$ac_cv_with_libfdata" != xauto-detect && test "x$ac_cv_with_libfdata" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libfdata in directory: $ac_cv_with_libfdata
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -49998,15 +50023,15 @@
 
 fi
 
 
     if test "x$ac_cv_libfdata" != xyes
 then :
 
-  ac_cv_libfdata_CPPFLAGS="-I../libfdata";
+  ac_cv_libfdata_CPPFLAGS="-I../libfdata -I\$(top_srcdir)/libfdata";
   ac_cv_libfdata_LIBADD="../libfdata/libfdata.la";
 
   ac_cv_libfdata=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBFDATA 1" >>confdefs.h
@@ -50076,15 +50101,15 @@
 printf "%s\n" "$ac_cv_with_libfdatetime" >&6; }
 
   if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libfdatetime" = xno
 then :
   ac_cv_libfdatetime=no
 else $as_nop
   ac_cv_libfdatetime=check
-        if test "x$ac_cv_with_libfdatetime" != x && test "x$ac_cv_with_libfdatetime" != xauto-detect
+                if test "x$ac_cv_with_libfdatetime" != x && test "x$ac_cv_with_libfdatetime" != xauto-detect && test "x$ac_cv_with_libfdatetime" != xyes
 then :
   if test -d "$ac_cv_with_libfdatetime"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libfdatetime}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libfdatetime}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -53520,15 +53545,16 @@
 fi
 
 
         ac_cv_libfdatetime_LIBADD="-lfdatetime"
 fi
 
 fi
-    if test "x$ac_cv_with_libfdatetime" != x && test "x$ac_cv_with_libfdatetime" != xauto-detect && test "x$ac_cv_libfdatetime" != xyes
+
+    if test "x$ac_cv_libfdatetime" != xyes && test "x$ac_cv_with_libfdatetime" != x && test "x$ac_cv_with_libfdatetime" != xauto-detect && test "x$ac_cv_with_libfdatetime" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libfdatetime in directory: $ac_cv_with_libfdatetime
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -53553,15 +53579,15 @@
 
 fi
 
 
     if test "x$ac_cv_libfdatetime" != xyes
 then :
 
-  ac_cv_libfdatetime_CPPFLAGS="-I../libfdatetime";
+  ac_cv_libfdatetime_CPPFLAGS="-I../libfdatetime -I\$(top_srcdir)/libfdatetime";
   ac_cv_libfdatetime_LIBADD="../libfdatetime/libfdatetime.la";
 
   ac_cv_libfdatetime=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBFDATETIME 1" >>confdefs.h
@@ -53631,15 +53657,15 @@
 printf "%s\n" "$ac_cv_with_libfguid" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libfguid" = xno
 then :
   ac_cv_libfguid=no
 else $as_nop
   ac_cv_libfguid=check
-        if test "x$ac_cv_with_libfguid" != x && test "x$ac_cv_with_libfguid" != xauto-detect
+                if test "x$ac_cv_with_libfguid" != x && test "x$ac_cv_with_libfguid" != xauto-detect && test "x$ac_cv_with_libfguid" != xyes
 then :
   if test -d "$ac_cv_with_libfguid"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libfguid}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libfguid}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -54213,15 +54239,16 @@
 fi
 
 
         ac_cv_libfguid_LIBADD="-lfguid"
 fi
 
 fi
-    if test "x$ac_cv_with_libfguid" != x && test "x$ac_cv_with_libfguid" != xauto-detect && test "x$ac_cv_libfguid" != xyes
+
+    if test "x$ac_cv_libfguid" != xyes && test "x$ac_cv_with_libfguid" != x && test "x$ac_cv_with_libfguid" != xauto-detect && test "x$ac_cv_with_libfguid" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libfguid in directory: $ac_cv_with_libfguid
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -54246,15 +54273,15 @@
 
 fi
 
 
     if test "x$ac_cv_libfguid" != xyes
 then :
 
-  ac_cv_libfguid_CPPFLAGS="-I../libfguid";
+  ac_cv_libfguid_CPPFLAGS="-I../libfguid -I\$(top_srcdir)/libfguid";
   ac_cv_libfguid_LIBADD="../libfguid/libfguid.la";
 
   ac_cv_libfguid=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBFGUID 1" >>confdefs.h
@@ -54324,15 +54351,15 @@
 printf "%s\n" "$ac_cv_with_libfvalue" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libfvalue" = xno
 then :
   ac_cv_libfvalue=no
 else $as_nop
   ac_cv_libfvalue=check
-        if test "x$ac_cv_with_libfvalue" != x && test "x$ac_cv_with_libfvalue" != xauto-detect
+                if test "x$ac_cv_with_libfvalue" != x && test "x$ac_cv_with_libfvalue" != xauto-detect && test "x$ac_cv_with_libfvalue" != xyes
 then :
   if test -d "$ac_cv_with_libfvalue"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libfvalue}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libfvalue}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -58638,15 +58665,16 @@
 fi
 
 
         ac_cv_libfvalue_LIBADD="-lfvalue"
 fi
 
 fi
-    if test "x$ac_cv_with_libfvalue" != x && test "x$ac_cv_with_libfvalue" != xauto-detect && test "x$ac_cv_libfvalue" != xyes
+
+    if test "x$ac_cv_libfvalue" != xyes && test "x$ac_cv_with_libfvalue" != x && test "x$ac_cv_with_libfvalue" != xauto-detect && test "x$ac_cv_with_libfvalue" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libfvalue in directory: $ac_cv_with_libfvalue
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -58671,15 +58699,15 @@
 
 fi
 
 
     if test "x$ac_cv_libfvalue" != xyes
 then :
 
-  ac_cv_libfvalue_CPPFLAGS="-I../libfvalue";
+  ac_cv_libfvalue_CPPFLAGS="-I../libfvalue -I\$(top_srcdir)/libfvalue";
   ac_cv_libfvalue_LIBADD="../libfvalue/libfvalue.la";
 
   ac_cv_libfvalue=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBFVALUE 1" >>confdefs.h
@@ -58749,15 +58777,15 @@
 printf "%s\n" "$ac_cv_with_libfwnt" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libfwnt" = xno
 then :
   ac_cv_libfwnt=no
 else $as_nop
   ac_cv_libfwnt=check
-        if test "x$ac_cv_with_libfwnt" != x && test "x$ac_cv_with_libfwnt" != xauto-detect
+                if test "x$ac_cv_with_libfwnt" != x && test "x$ac_cv_with_libfwnt" != xauto-detect && test "x$ac_cv_with_libfwnt" != xyes
 then :
   if test -d "$ac_cv_with_libfwnt"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libfwnt}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libfwnt}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -60139,15 +60167,16 @@
 fi
 
 
         ac_cv_libfwnt_LIBADD="-lfwnt"
 fi
 
 fi
-    if test "x$ac_cv_with_libfwnt" != x && test "x$ac_cv_with_libfwnt" != xauto-detect && test "x$ac_cv_libfwnt" != xyes
+
+    if test "x$ac_cv_libfwnt" != xyes && test "x$ac_cv_with_libfwnt" != x && test "x$ac_cv_with_libfwnt" != xauto-detect && test "x$ac_cv_with_libfwnt" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libfwnt in directory: $ac_cv_with_libfwnt
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -60172,15 +60201,15 @@
 
 fi
 
 
     if test "x$ac_cv_libfwnt" != xyes
 then :
 
-  ac_cv_libfwnt_CPPFLAGS="-I../libfwnt";
+  ac_cv_libfwnt_CPPFLAGS="-I../libfwnt -I\$(top_srcdir)/libfwnt";
   ac_cv_libfwnt_LIBADD="../libfwnt/libfwnt.la";
 
   ac_cv_libfwnt=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBFWNT 1" >>confdefs.h
@@ -60491,16 +60520,20 @@
         PYTHON_LDFLAGS=`${PYTHON_CONFIG} --ldflags 2>/dev/null`;
 
     { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for Python libraries" >&5
 printf %s "checking for Python libraries... " >&6; }
     { printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $PYTHON_LDFLAGS" >&5
 printf "%s\n" "$PYTHON_LDFLAGS" >&6; }
 
-        case $host_os in #(
-  cygwin*) :
+        case $build in #(
+  *-*-cygwin*) :
+    PYTHON_LDFLAGS="${PYTHON_LDFLAGS} -no-undefined" ;; #(
+  *-*-mingw*) :
+    PYTHON_LDFLAGS="${PYTHON_LDFLAGS} -no-undefined" ;; #(
+  *-*-msys*) :
     PYTHON_LDFLAGS="${PYTHON_LDFLAGS} -no-undefined" ;; #(
   *) :
      ;; #(
   *) :
      ;;
 esac
 
@@ -60663,15 +60696,15 @@
 printf "%s\n" "$ac_cv_with_libfmapi" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libfmapi" = xno
 then :
   ac_cv_libfmapi=no
 else $as_nop
   ac_cv_libfmapi=check
-        if test "x$ac_cv_with_libfmapi" != x && test "x$ac_cv_with_libfmapi" != xauto-detect
+                if test "x$ac_cv_with_libfmapi" != x && test "x$ac_cv_with_libfmapi" != xauto-detect && test "x$ac_cv_with_libfmapi" != xyes
 then :
   if test -d "$ac_cv_with_libfmapi"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libfmapi}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libfmapi}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -61836,15 +61869,16 @@
 fi
 
 
         ac_cv_libfmapi_LIBADD="-lfmapi"
 fi
 
 fi
-    if test "x$ac_cv_with_libfmapi" != x && test "x$ac_cv_with_libfmapi" != xauto-detect && test "x$ac_cv_libfmapi" != xyes
+
+    if test "x$ac_cv_libfmapi" != xyes && test "x$ac_cv_with_libfmapi" != x && test "x$ac_cv_with_libfmapi" != xauto-detect && test "x$ac_cv_with_libfmapi" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libfmapi in directory: $ac_cv_with_libfmapi
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -62043,15 +62077,15 @@
 
 fi
 
 
     if test "x$ac_cv_libfmapi" != xyes
 then :
 
-  ac_cv_libfmapi_CPPFLAGS="-I../libfmapi";
+  ac_cv_libfmapi_CPPFLAGS="-I../libfmapi -I\$(top_srcdir)/libfmapi";
   ac_cv_libfmapi_LIBADD="../libfmapi/libfmapi.la";
 
   ac_cv_libfmapi=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBFMAPI 1" >>confdefs.h
@@ -62121,15 +62155,15 @@
 printf "%s\n" "$ac_cv_with_libmapidb" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libmapidb" = xno
 then :
   ac_cv_libmapidb=no
 else $as_nop
   ac_cv_libmapidb=check
-        if test "x$ac_cv_with_libmapidb" != x && test "x$ac_cv_with_libmapidb" != xauto-detect
+                if test "x$ac_cv_with_libmapidb" != x && test "x$ac_cv_with_libmapidb" != xauto-detect && test "x$ac_cv_with_libmapidb" != xyes
 then :
   if test -d "$ac_cv_with_libmapidb"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libmapidb}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libmapidb}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -62283,15 +62317,16 @@
 
 
 
         ac_cv_libmapidb_LIBADD="-lmapidb"
 fi
 
 fi
-    if test "x$ac_cv_with_libmapidb" != x && test "x$ac_cv_with_libmapidb" != xauto-detect && test "x$ac_cv_libmapidb" != xyes
+
+    if test "x$ac_cv_libmapidb" != xyes && test "x$ac_cv_with_libmapidb" != x && test "x$ac_cv_with_libmapidb" != xauto-detect && test "x$ac_cv_with_libmapidb" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libmapidb in directory: $ac_cv_with_libmapidb
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -62315,15 +62350,15 @@
 
 
 fi
 
 
     if test "x$ac_cv_libmapidb" != xyes
 then :
-  ac_cv_libmapidb_CPPFLAGS="-I../libmapidb";
+  ac_cv_libmapidb_CPPFLAGS="-I../libmapidb -I\$(top_srcdir)/libmapidb";
   ac_cv_libmapidb_LIBADD="../libmapidb/libmapidb.la";
 
   ac_cv_libmapidb=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBMAPIDB 1" >>confdefs.h
@@ -63295,15 +63330,15 @@
 test $as_write_fail = 0 && chmod +x $CONFIG_STATUS || ac_write_fail=1
 
 cat >>$CONFIG_STATUS <<\_ACEOF || ac_write_fail=1
 # Save the log message, to keep $0 and so on meaningful, and to
 # report actual input values of CONFIG_FILES etc. instead of their
 # values after options handling.
 ac_log="
-This file was extended by libesedb $as_me 20240202, which was
+This file was extended by libesedb $as_me 20240420, which was
 generated by GNU Autoconf 2.71.  Invocation command line was
 
   CONFIG_FILES    = $CONFIG_FILES
   CONFIG_HEADERS  = $CONFIG_HEADERS
   CONFIG_LINKS    = $CONFIG_LINKS
   CONFIG_COMMANDS = $CONFIG_COMMANDS
   $ $0 $@
@@ -63363,15 +63398,15 @@
 
 _ACEOF
 ac_cs_config=`printf "%s\n" "$ac_configure_args" | sed "$ac_safe_unquote"`
 ac_cs_config_escaped=`printf "%s\n" "$ac_cs_config" | sed "s/^ //; s/'/'\\\\\\\\''/g"`
 cat >>$CONFIG_STATUS <<_ACEOF || ac_write_fail=1
 ac_cs_config='$ac_cs_config_escaped'
 ac_cs_version="\\
-libesedb config.status 20240202
+libesedb config.status 20240420
 configured by $0, generated by GNU Autoconf 2.71,
   with options \\"\$ac_cs_config\\"
 
 Copyright (C) 2021 Free Software Foundation, Inc.
 This config.status script is free software; the Free Software Foundation
 gives unlimited permission to copy, distribute and modify it."
```

### Comparing `libesedb-20240202/compile` & `libesedb-20240420/compile`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/missing` & `libesedb-20240420/missing`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libesedb/libesedb.rc` & `libesedb-20240420/libesedb/libesedb.rc`

 * *Files 2% similar despite different names*

```diff
@@ -18,20 +18,20 @@
   FILESUBTYPE				0x0L
 BEGIN
   BLOCK "StringFileInfo"
   BEGIN
     BLOCK "040904E4"
     BEGIN
       VALUE "FileDescription",		"Library to access the Extensible Storage Engine (ESE) Database File (EDB) format\0"
-      VALUE "FileVersion",		"20240202" "\0"
+      VALUE "FileVersion",		"20240420" "\0"
       VALUE "InternalName",		"libesedb.dll\0"
       VALUE "LegalCopyright",		"(C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>\0"
       VALUE "OriginalFilename",		"libesedb.dll\0"
       VALUE "ProductName",		"libesedb\0"
-      VALUE "ProductVersion",		"20240202" "\0"
+      VALUE "ProductVersion",		"20240420" "\0"
       VALUE "Comments",			"For more information visit https://github.com/libyal/libesedb/\0"
     END
   END
   BLOCK "VarFileInfo"
   BEGIN
     VALUE "Translation", 0x0409, 1200
   END
```

### Comparing `libesedb-20240202/libesedb/libesedb_definitions.h.in` & `libesedb-20240420/libesedb/libesedb_definitions.h.in`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libesedb/libesedb_data_segment.c` & `libesedb-20240420/libesedb/libesedb_data_segment.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libesedb/esedb_file_header.h` & `libesedb-20240420/libesedb/esedb_file_header.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libesedb/libesedb_root_page_header.h` & `libesedb-20240420/libesedb/libesedb_root_page_header.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libesedb/libesedb_error.h` & `libesedb-20240420/libesedb/libesedb_error.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libesedb/libesedb_libcdata.h` & `libesedb-20240420/libesedb/libesedb_libcdata.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libesedb/libesedb_column_type.c` & `libesedb-20240420/libesedb/libesedb_column_type.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libesedb/libesedb_lcid.h` & `libesedb-20240420/libesedb/libesedb_lcid.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libesedb/libesedb_libcerror.h` & `libesedb-20240420/libesedb/libesedb_libcerror.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libesedb/libesedb_file_header.c` & `libesedb-20240420/libesedb/libesedb_file_header.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libesedb/libesedb_space_tree_value.h` & `libesedb-20240420/libesedb/libesedb_space_tree_value.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libesedb/libesedb_io_handle.h` & `libesedb-20240420/libesedb/libesedb_io_handle.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libesedb/libesedb_leaf_page_descriptor.c` & `libesedb-20240420/libesedb/libesedb_leaf_page_descriptor.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libesedb/libesedb_i18n.c` & `libesedb-20240420/libesedb/libesedb_i18n.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libesedb/libesedb_multi_value.c` & `libesedb-20240420/libesedb/libesedb_multi_value.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libesedb/libesedb_block_descriptor.h` & `libesedb-20240420/libesedb/libesedb_block_descriptor.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libesedb/libesedb_notify.c` & `libesedb-20240420/libesedb/libesedb_notify.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libesedb/libesedb_block_tree.h` & `libesedb-20240420/libesedb/libesedb_block_tree.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libesedb/libesedb_codepage.h` & `libesedb-20240420/libesedb/libesedb_codepage.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libesedb/libesedb_table.h` & `libesedb-20240420/libesedb/libesedb_table.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libesedb/libesedb_definitions.h` & `libesedb-20240420/libesedb/libesedb_definitions.h`

 * *Files 0% similar despite different names*

```diff
@@ -36,19 +36,19 @@
 #if !defined( HAVE_LOCAL_LIBESEDB )
 #include <libesedb/definitions.h>
 
 /* The definitions in <libesedb/definitions.h> are copied here
  * for local use of libesedb
  */
 #else
-#define LIBESEDB_VERSION						20240202
+#define LIBESEDB_VERSION						20240420
 
 /* The version string
  */
-#define LIBESEDB_VERSION_STRING						"20240202"
+#define LIBESEDB_VERSION_STRING						"20240420"
 
 /* The access flags definitions
  * bit 1        set to 1 for read access
  * bit 2        set to 1 for write access
  * bit 3-8      not used
  */
 enum LIBESEDB_ACCESS_FLAGS
```

### Comparing `libesedb-20240202/libesedb/libesedb_block_tree.c` & `libesedb-20240420/libesedb/libesedb_block_tree.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libesedb/libesedb_support.h` & `libesedb-20240420/libesedb/libesedb_support.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libesedb/libesedb_catalog.h` & `libesedb-20240420/libesedb/libesedb_catalog.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libesedb/libesedb_codepage.c` & `libesedb-20240420/libesedb/libesedb_codepage.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libesedb/libesedb_file.h` & `libesedb-20240420/libesedb/libesedb_file.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libesedb/libesedb_page.c` & `libesedb-20240420/libesedb/libesedb_page.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libesedb/libesedb_table_definition.c` & `libesedb-20240420/libesedb/libesedb_table_definition.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libesedb/libesedb_page_tree.h` & `libesedb-20240420/libesedb/libesedb_page_tree.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libesedb/libesedb_page_tree_key.c` & `libesedb-20240420/libesedb/libesedb_page_tree_key.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libesedb/libesedb_page_tree.c` & `libesedb-20240420/libesedb/libesedb_page_tree.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libesedb/libesedb_block_descriptor.c` & `libesedb-20240420/libesedb/libesedb_block_descriptor.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libesedb/libesedb_block_tree_node.c` & `libesedb-20240420/libesedb/libesedb_block_tree_node.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libesedb/libesedb_support.c` & `libesedb-20240420/libesedb/libesedb_support.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libesedb/libesedb_debug.c` & `libesedb-20240420/libesedb/libesedb_debug.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libesedb/libesedb_column.h` & `libesedb-20240420/libesedb/libesedb_column.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libesedb/libesedb_record.c` & `libesedb-20240420/libesedb/libesedb_record.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libesedb/libesedb_leaf_page_descriptor.h` & `libesedb-20240420/libesedb/libesedb_leaf_page_descriptor.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libesedb/libesedb_libbfio.h` & `libesedb-20240420/libesedb/libesedb_libbfio.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libesedb/Makefile.am` & `libesedb-20240420/libesedb/Makefile.am`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 AM_CPPFLAGS = \
 	-DLOCALEDIR=\"$(datadir)/locale\" \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBCSPLIT_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ \
 	@LIBCFILE_CPPFLAGS@ \
@@ -103,21 +103,19 @@
 libesedb_la_LDFLAGS = -no-undefined -version-info 1:0:0
 
 EXTRA_DIST = \
 	libesedb_definitions.h.in \
 	libesedb.rc \
 	libesedb.rc.in
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	libesedb_definitions.h \
+	libesedb.rc \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f libesedb_definitions.h
-	-rm -f libesedb.rc
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libesedb ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libesedb_la_SOURCES)
```

### Comparing `libesedb-20240202/libesedb/libesedb_libfcache.h` & `libesedb-20240420/libesedb/libesedb_libfcache.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libesedb/libesedb_notify.h` & `libesedb-20240420/libesedb/libesedb_notify.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libesedb/libesedb_catalog_definition.h` & `libesedb-20240420/libesedb/libesedb_catalog_definition.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libesedb/esedb_page.h` & `libesedb-20240420/libesedb/esedb_page.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libesedb/libesedb_extern.h` & `libesedb-20240420/libesedb/libesedb_extern.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libesedb/libesedb_libfwnt.h` & `libesedb-20240420/libesedb/libesedb_libfwnt.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libesedb/libesedb_i18n.h` & `libesedb-20240420/libesedb/libesedb_i18n.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libesedb/libesedb_value_data_handle.c` & `libesedb-20240420/libesedb/libesedb_value_data_handle.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libesedb/libesedb_page_tree_key.h` & `libesedb-20240420/libesedb/libesedb_page_tree_key.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libesedb/libesedb_page_value.c` & `libesedb-20240420/libesedb/libesedb_page_value.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libesedb/libesedb_checksum.c` & `libesedb-20240420/libesedb/libesedb_checksum.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libesedb/libesedb_index.c` & `libesedb-20240420/libesedb/libesedb_index.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libesedb/libesedb_multi_value.h` & `libesedb-20240420/libesedb/libesedb_multi_value.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libesedb/libesedb_libcnotify.h` & `libesedb-20240420/libesedb/libesedb_libcnotify.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libesedb/libesedb_column.c` & `libesedb-20240420/libesedb/libesedb_column.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libesedb/libesedb_unused.h` & `libesedb-20240420/libesedb/libesedb_unused.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libesedb/libesedb.rc.in` & `libesedb-20240420/libesedb/libesedb.rc.in`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libesedb/libesedb_io_handle.c` & `libesedb-20240420/libesedb/libesedb_io_handle.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libesedb/libesedb_libfdata.h` & `libesedb-20240420/libesedb/libesedb_libfdata.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libesedb/libesedb.c` & `libesedb-20240420/libesedb/libesedb.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libesedb/libesedb_file.c` & `libesedb-20240420/libesedb/libesedb_file.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libesedb/libesedb_page_header.c` & `libesedb-20240420/libesedb/libesedb_page_header.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libesedb/libesedb_space_tree_value.c` & `libesedb-20240420/libesedb/libesedb_space_tree_value.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libesedb/libesedb_compression.h` & `libesedb-20240420/libesedb/libesedb_compression.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libesedb/libesedb_root_page_header.c` & `libesedb-20240420/libesedb/libesedb_root_page_header.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libesedb/libesedb_libuna.h` & `libesedb-20240420/libesedb/libesedb_libuna.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libesedb/libesedb_index.h` & `libesedb-20240420/libesedb/libesedb_index.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libesedb/libesedb_record.h` & `libesedb-20240420/libesedb/libesedb_record.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libesedb/libesedb_table_definition.h` & `libesedb-20240420/libesedb/libesedb_table_definition.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libesedb/libesedb_long_value.h` & `libesedb-20240420/libesedb/libesedb_long_value.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libesedb/libesedb_data_segment.h` & `libesedb-20240420/libesedb/libesedb_data_segment.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libesedb/libesedb_catalog.c` & `libesedb-20240420/libesedb/libesedb_catalog.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libesedb/libesedb_record_value.c` & `libesedb-20240420/libesedb/libesedb_record_value.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libesedb/libesedb_table.c` & `libesedb-20240420/libesedb/libesedb_table.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libesedb/libesedb_error.c` & `libesedb-20240420/libesedb/libesedb_error.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libesedb/libesedb_record_value.h` & `libesedb-20240420/libesedb/libesedb_record_value.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libesedb/libesedb_debug.h` & `libesedb-20240420/libesedb/libesedb_debug.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libesedb/libesedb_page_header.h` & `libesedb-20240420/libesedb/libesedb_page_header.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libesedb/libesedb_block_tree_node.h` & `libesedb-20240420/libesedb/libesedb_block_tree_node.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libesedb/libesedb_data_definition.h` & `libesedb-20240420/libesedb/libesedb_data_definition.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libesedb/libesedb_libfvalue.h` & `libesedb-20240420/libesedb/libesedb_libfvalue.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libesedb/libesedb_data_definition.c` & `libesedb-20240420/libesedb/libesedb_data_definition.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libesedb/libesedb_space_tree.h` & `libesedb-20240420/libesedb/libesedb_space_tree.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libesedb/libesedb_lcid.c` & `libesedb-20240420/libesedb/libesedb_lcid.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libesedb/libesedb_space_tree.c` & `libesedb-20240420/libesedb/libesedb_space_tree.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libesedb/libesedb_libclocale.h` & `libesedb-20240420/libesedb/libesedb_libclocale.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libesedb/libesedb_page_tree_value.c` & `libesedb-20240420/libesedb/libesedb_page_tree_value.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libesedb/Makefile.in` & `libesedb-20240420/libesedb/Makefile.in`

 * *Files 6% similar despite different names*

```diff
@@ -617,16 +617,16 @@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 AM_CPPFLAGS = \
 	-DLOCALEDIR=\"$(datadir)/locale\" \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBCSPLIT_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ \
 	@LIBCFILE_CPPFLAGS@ \
@@ -722,15 +722,18 @@
 
 libesedb_la_LDFLAGS = -no-undefined -version-info 1:0:0
 EXTRA_DIST = \
 	libesedb_definitions.h.in \
 	libesedb.rc \
 	libesedb.rc.in
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	libesedb_definitions.h \
+	libesedb.rc \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -1001,24 +1004,67 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libLTLIBRARIES clean-libtool \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libesedb.Plo
+	-rm -f ./$(DEPDIR)/libesedb_block_descriptor.Plo
+	-rm -f ./$(DEPDIR)/libesedb_block_tree.Plo
+	-rm -f ./$(DEPDIR)/libesedb_block_tree_node.Plo
+	-rm -f ./$(DEPDIR)/libesedb_catalog.Plo
+	-rm -f ./$(DEPDIR)/libesedb_catalog_definition.Plo
+	-rm -f ./$(DEPDIR)/libesedb_checksum.Plo
+	-rm -f ./$(DEPDIR)/libesedb_codepage.Plo
+	-rm -f ./$(DEPDIR)/libesedb_column.Plo
+	-rm -f ./$(DEPDIR)/libesedb_column_type.Plo
+	-rm -f ./$(DEPDIR)/libesedb_compression.Plo
+	-rm -f ./$(DEPDIR)/libesedb_data_definition.Plo
+	-rm -f ./$(DEPDIR)/libesedb_data_segment.Plo
+	-rm -f ./$(DEPDIR)/libesedb_database.Plo
+	-rm -f ./$(DEPDIR)/libesedb_debug.Plo
+	-rm -f ./$(DEPDIR)/libesedb_error.Plo
+	-rm -f ./$(DEPDIR)/libesedb_file.Plo
+	-rm -f ./$(DEPDIR)/libesedb_file_header.Plo
+	-rm -f ./$(DEPDIR)/libesedb_i18n.Plo
+	-rm -f ./$(DEPDIR)/libesedb_index.Plo
+	-rm -f ./$(DEPDIR)/libesedb_io_handle.Plo
+	-rm -f ./$(DEPDIR)/libesedb_lcid.Plo
+	-rm -f ./$(DEPDIR)/libesedb_leaf_page_descriptor.Plo
+	-rm -f ./$(DEPDIR)/libesedb_long_value.Plo
+	-rm -f ./$(DEPDIR)/libesedb_multi_value.Plo
+	-rm -f ./$(DEPDIR)/libesedb_notify.Plo
+	-rm -f ./$(DEPDIR)/libesedb_page.Plo
+	-rm -f ./$(DEPDIR)/libesedb_page_header.Plo
+	-rm -f ./$(DEPDIR)/libesedb_page_tree.Plo
+	-rm -f ./$(DEPDIR)/libesedb_page_tree_key.Plo
+	-rm -f ./$(DEPDIR)/libesedb_page_tree_value.Plo
+	-rm -f ./$(DEPDIR)/libesedb_page_value.Plo
+	-rm -f ./$(DEPDIR)/libesedb_record.Plo
+	-rm -f ./$(DEPDIR)/libesedb_record_value.Plo
+	-rm -f ./$(DEPDIR)/libesedb_root_page_header.Plo
+	-rm -f ./$(DEPDIR)/libesedb_space_tree.Plo
+	-rm -f ./$(DEPDIR)/libesedb_space_tree_value.Plo
+	-rm -f ./$(DEPDIR)/libesedb_support.Plo
+	-rm -f ./$(DEPDIR)/libesedb_table.Plo
+	-rm -f ./$(DEPDIR)/libesedb_table_definition.Plo
+	-rm -f ./$(DEPDIR)/libesedb_value_data_handle.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -1142,19 +1188,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am uninstall-libLTLIBRARIES
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f libesedb_definitions.h
-	-rm -f libesedb.rc
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libesedb ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libesedb_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libesedb-20240202/libesedb/libesedb_database.h` & `libesedb-20240420/libesedb/libesedb_database.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libesedb/libesedb_compression.c` & `libesedb-20240420/libesedb/libesedb_compression.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libesedb/libesedb_file_header.h` & `libesedb-20240420/libesedb/libesedb_file_header.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libesedb/libesedb_page_tree_value.h` & `libesedb-20240420/libesedb/libesedb_page_tree_value.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libesedb/libesedb_value_data_handle.h` & `libesedb-20240420/libesedb/libesedb_value_data_handle.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libesedb/libesedb_page.h` & `libesedb-20240420/libesedb/libesedb_page.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libesedb/libesedb_catalog_definition.c` & `libesedb-20240420/libesedb/libesedb_catalog_definition.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libesedb/libesedb_long_value.c` & `libesedb-20240420/libesedb/libesedb_long_value.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libesedb/esedb_page_values.h` & `libesedb-20240420/libesedb/esedb_page_values.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libesedb/libesedb_checksum.h` & `libesedb-20240420/libesedb/libesedb_checksum.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libesedb/libesedb_column_type.h` & `libesedb-20240420/libesedb/libesedb_column_type.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libesedb/libesedb_page_value.h` & `libesedb-20240420/libesedb/libesedb_page_value.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libesedb/libesedb_database.c` & `libesedb-20240420/libesedb/libesedb_database.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libesedb/libesedb_types.h` & `libesedb-20240420/libesedb/libesedb_types.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/msvscpp/esedb_test_page_tree_value/esedb_test_page_tree_value.vcproj` & `libesedb-20240420/msvscpp/esedb_test_page_tree_value/esedb_test_page_tree_value.vcproj`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/msvscpp/libfdata/libfdata.vcproj` & `libesedb-20240420/msvscpp/libfdata/libfdata.vcproj`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/msvscpp/esedb_test_long_value/esedb_test_long_value.vcproj` & `libesedb-20240420/msvscpp/esedb_test_long_value/esedb_test_long_value.vcproj`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/msvscpp/esedb_test_space_tree/esedb_test_space_tree.vcproj` & `libesedb-20240420/msvscpp/esedb_test_space_tree/esedb_test_space_tree.vcproj`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/msvscpp/esedb_test_file/esedb_test_file.vcproj` & `libesedb-20240420/msvscpp/esedb_test_file/esedb_test_file.vcproj`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/msvscpp/esedb_test_space_tree_value/esedb_test_space_tree_value.vcproj` & `libesedb-20240420/msvscpp/esedb_test_space_tree_value/esedb_test_space_tree_value.vcproj`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/msvscpp/esedb_test_block_tree_node/esedb_test_block_tree_node.vcproj` & `libesedb-20240420/msvscpp/esedb_test_block_tree_node/esedb_test_block_tree_node.vcproj`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/msvscpp/esedb_test_checksum/esedb_test_checksum.vcproj` & `libesedb-20240420/msvscpp/esedb_test_checksum/esedb_test_checksum.vcproj`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/msvscpp/esedb_test_block_descriptor/esedb_test_block_descriptor.vcproj` & `libesedb-20240420/msvscpp/esedb_test_block_descriptor/esedb_test_block_descriptor.vcproj`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/msvscpp/esedb_test_database/esedb_test_database.vcproj` & `libesedb-20240420/msvscpp/esedb_test_database/esedb_test_database.vcproj`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/msvscpp/esedbexport/esedbexport.vcproj` & `libesedb-20240420/msvscpp/esedbexport/esedbexport.vcproj`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/msvscpp/esedb_test_table/esedb_test_table.vcproj` & `libesedb-20240420/msvscpp/esedb_test_table/esedb_test_table.vcproj`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/msvscpp/esedbinfo/esedbinfo.vcproj` & `libesedb-20240420/msvscpp/esedbinfo/esedbinfo.vcproj`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/msvscpp/esedb_test_page/esedb_test_page.vcproj` & `libesedb-20240420/msvscpp/esedb_test_page/esedb_test_page.vcproj`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/msvscpp/esedb_test_column_type/esedb_test_column_type.vcproj` & `libesedb-20240420/msvscpp/esedb_test_column_type/esedb_test_column_type.vcproj`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/msvscpp/libfguid/libfguid.vcproj` & `libesedb-20240420/msvscpp/libfguid/libfguid.vcproj`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/msvscpp/esedb_test_catalog_definition/esedb_test_catalog_definition.vcproj` & `libesedb-20240420/msvscpp/esedb_test_catalog_definition/esedb_test_catalog_definition.vcproj`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/msvscpp/esedb_test_tools_windows_search_compression/esedb_test_tools_windows_search_compression.vcproj` & `libesedb-20240420/msvscpp/esedb_test_tools_windows_search_compression/esedb_test_tools_windows_search_compression.vcproj`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/msvscpp/libclocale/libclocale.vcproj` & `libesedb-20240420/msvscpp/libclocale/libclocale.vcproj`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/msvscpp/esedb_test_data_definition/esedb_test_data_definition.vcproj` & `libesedb-20240420/msvscpp/esedb_test_data_definition/esedb_test_data_definition.vcproj`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/msvscpp/esedb_test_support/esedb_test_support.vcproj` & `libesedb-20240420/msvscpp/esedb_test_support/esedb_test_support.vcproj`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/msvscpp/esedb_test_index/esedb_test_index.vcproj` & `libesedb-20240420/msvscpp/esedb_test_index/esedb_test_index.vcproj`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/msvscpp/libfcache/libfcache.vcproj` & `libesedb-20240420/msvscpp/libfcache/libfcache.vcproj`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/msvscpp/Makefile.am` & `libesedb-20240420/msvscpp/Makefile.am`

 * *Files 2% similar despite different names*

```diff
@@ -60,13 +60,11 @@
 	libuna/libuna.vcproj \
 	pyesedb/pyesedb.vcproj \
 	libesedb.sln
 
 EXTRA_DIST = \
 	$(MSVSCPP_FILES)
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
```

### Comparing `libesedb-20240202/msvscpp/libbfio/libbfio.vcproj` & `libesedb-20240420/msvscpp/libbfio/libbfio.vcproj`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/msvscpp/esedb_test_column/esedb_test_column.vcproj` & `libesedb-20240420/msvscpp/esedb_test_column/esedb_test_column.vcproj`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/msvscpp/libesedb/libesedb.vcproj` & `libesedb-20240420/msvscpp/libesedb/libesedb.vcproj`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/msvscpp/esedb_test_leaf_page_descriptor/esedb_test_leaf_page_descriptor.vcproj` & `libesedb-20240420/msvscpp/esedb_test_leaf_page_descriptor/esedb_test_leaf_page_descriptor.vcproj`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/msvscpp/esedb_test_block_tree/esedb_test_block_tree.vcproj` & `libesedb-20240420/msvscpp/esedb_test_block_tree/esedb_test_block_tree.vcproj`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/msvscpp/esedb_test_io_handle/esedb_test_io_handle.vcproj` & `libesedb-20240420/msvscpp/esedb_test_io_handle/esedb_test_io_handle.vcproj`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/msvscpp/libcfile/libcfile.vcproj` & `libesedb-20240420/msvscpp/libcfile/libcfile.vcproj`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/msvscpp/libmapidb/libmapidb.vcproj` & `libesedb-20240420/msvscpp/libmapidb/libmapidb.vcproj`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/msvscpp/esedb_test_compression/esedb_test_compression.vcproj` & `libesedb-20240420/msvscpp/esedb_test_compression/esedb_test_compression.vcproj`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/msvscpp/libcdata/libcdata.vcproj` & `libesedb-20240420/msvscpp/libcdata/libcdata.vcproj`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/msvscpp/esedb_test_page_tree_key/esedb_test_page_tree_key.vcproj` & `libesedb-20240420/msvscpp/esedb_test_page_tree_key/esedb_test_page_tree_key.vcproj`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/msvscpp/libfmapi/libfmapi.vcproj` & `libesedb-20240420/msvscpp/libfmapi/libfmapi.vcproj`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/msvscpp/esedb_test_file_header/esedb_test_file_header.vcproj` & `libesedb-20240420/msvscpp/esedb_test_file_header/esedb_test_file_header.vcproj`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/msvscpp/esedb_test_tools_info_handle/esedb_test_tools_info_handle.vcproj` & `libesedb-20240420/msvscpp/esedb_test_tools_info_handle/esedb_test_tools_info_handle.vcproj`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/msvscpp/pyesedb/pyesedb.vcproj` & `libesedb-20240420/msvscpp/pyesedb/pyesedb.vcproj`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/msvscpp/esedb_test_page_value/esedb_test_page_value.vcproj` & `libesedb-20240420/msvscpp/esedb_test_page_value/esedb_test_page_value.vcproj`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/msvscpp/esedb_test_root_page_header/esedb_test_root_page_header.vcproj` & `libesedb-20240420/msvscpp/esedb_test_root_page_header/esedb_test_root_page_header.vcproj`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/msvscpp/libcthreads/libcthreads.vcproj` & `libesedb-20240420/msvscpp/libcthreads/libcthreads.vcproj`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/msvscpp/esedb_test_tools_output/esedb_test_tools_output.vcproj` & `libesedb-20240420/msvscpp/esedb_test_tools_output/esedb_test_tools_output.vcproj`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/msvscpp/libcpath/libcpath.vcproj` & `libesedb-20240420/msvscpp/libcpath/libcpath.vcproj`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/msvscpp/esedb_test_tools_signal/esedb_test_tools_signal.vcproj` & `libesedb-20240420/msvscpp/esedb_test_tools_signal/esedb_test_tools_signal.vcproj`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/msvscpp/libfwnt/libfwnt.vcproj` & `libesedb-20240420/msvscpp/libfwnt/libfwnt.vcproj`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/msvscpp/esedb_test_table_definition/esedb_test_table_definition.vcproj` & `libesedb-20240420/msvscpp/esedb_test_table_definition/esedb_test_table_definition.vcproj`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/msvscpp/esedb_test_multi_value/esedb_test_multi_value.vcproj` & `libesedb-20240420/msvscpp/esedb_test_multi_value/esedb_test_multi_value.vcproj`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/msvscpp/esedb_test_catalog/esedb_test_catalog.vcproj` & `libesedb-20240420/msvscpp/esedb_test_catalog/esedb_test_catalog.vcproj`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/msvscpp/libcsplit/libcsplit.vcproj` & `libesedb-20240420/msvscpp/libcsplit/libcsplit.vcproj`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/msvscpp/esedb_test_record/esedb_test_record.vcproj` & `libesedb-20240420/msvscpp/esedb_test_record/esedb_test_record.vcproj`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/msvscpp/libuna/libuna.vcproj` & `libesedb-20240420/msvscpp/libuna/libuna.vcproj`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/msvscpp/Makefile.in` & `libesedb-20240420/msvscpp/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -547,15 +547,16 @@
 	libuna/libuna.vcproj \
 	pyesedb/pyesedb.vcproj \
 	libesedb.sln
 
 EXTRA_DIST = \
 	$(MSVSCPP_FILES)
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
 	@for dep in $?; do \
@@ -659,23 +660,25 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool mostlyclean-am
 
+distclean: distclean-am
+	-rm -f Makefile
 distclean-am: clean-am distclean-generic
 
 dvi: dvi-am
 
 dvi-am:
 
 html: html-am
@@ -754,13 +757,10 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libesedb-20240202/msvscpp/libfvalue/libfvalue.vcproj` & `libesedb-20240420/msvscpp/libfvalue/libfvalue.vcproj`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/msvscpp/esedb_test_page_tree/esedb_test_page_tree.vcproj` & `libesedb-20240420/msvscpp/esedb_test_page_tree/esedb_test_page_tree.vcproj`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/msvscpp/esedb_test_error/esedb_test_error.vcproj` & `libesedb-20240420/msvscpp/esedb_test_error/esedb_test_error.vcproj`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/msvscpp/esedb_test_data_segment/esedb_test_data_segment.vcproj` & `libesedb-20240420/msvscpp/esedb_test_data_segment/esedb_test_data_segment.vcproj`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/msvscpp/libcnotify/libcnotify.vcproj` & `libesedb-20240420/msvscpp/libcnotify/libcnotify.vcproj`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/msvscpp/libcerror/libcerror.vcproj` & `libesedb-20240420/msvscpp/libcerror/libcerror.vcproj`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/msvscpp/libesedb.sln` & `libesedb-20240420/msvscpp/libesedb.sln`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/msvscpp/esedb_test_notify/esedb_test_notify.vcproj` & `libesedb-20240420/msvscpp/esedb_test_notify/esedb_test_notify.vcproj`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/msvscpp/libfdatetime/libfdatetime.vcproj` & `libesedb-20240420/msvscpp/libfdatetime/libfdatetime.vcproj`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/msvscpp/esedb_test_page_header/esedb_test_page_header.vcproj` & `libesedb-20240420/msvscpp/esedb_test_page_header/esedb_test_page_header.vcproj`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libcfile/libcfile_extern.h` & `libesedb-20240420/libcfile/libcfile_extern.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libcfile/libcfile_support.h` & `libesedb-20240420/libcfile/libcfile_support.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libcfile/libcfile_unused.h` & `libesedb-20240420/libcfile/libcfile_unused.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libcfile/libcfile_notify.h` & `libesedb-20240420/libcfile/libcfile_notify.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libcfile/libcfile_support.c` & `libesedb-20240420/libcfile/libcfile_support.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libcfile/libcfile_types.h` & `libesedb-20240420/libcfile/libcfile_types.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libcfile/Makefile.am` & `libesedb-20240420/libcfile/Makefile.am`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBCFILE
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libcfile.la
 
@@ -22,19 +22,17 @@
 	libcfile_support.c libcfile_support.h \
 	libcfile_system_string.c libcfile_system_string.h \
 	libcfile_types.h \
 	libcfile_unused.h \
 	libcfile_winapi.c libcfile_winapi.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcfile ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcfile_la_SOURCES)
```

### Comparing `libesedb-20240202/libcfile/libcfile_notify.c` & `libesedb-20240420/libcfile/libcfile_notify.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libcfile/libcfile_system_string.h` & `libesedb-20240420/libcfile/libcfile_system_string.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libcfile/libcfile_file.h` & `libesedb-20240420/libcfile/libcfile_file.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libcfile/libcfile_libcnotify.h` & `libesedb-20240420/libcfile/libcfile_libcnotify.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libcfile/libcfile_system_string.c` & `libesedb-20240420/libcfile/libcfile_system_string.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libcfile/libcfile_error.h` & `libesedb-20240420/libcfile/libcfile_error.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libcfile/libcfile_libcerror.h` & `libesedb-20240420/libcfile/libcfile_libcerror.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libcfile/libcfile_file.c` & `libesedb-20240420/libcfile/libcfile_file.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libcfile/libcfile_libclocale.h` & `libesedb-20240420/libcfile/libcfile_libclocale.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libcfile/libcfile_winapi.h` & `libesedb-20240420/libcfile/libcfile_winapi.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libcfile/Makefile.in` & `libesedb-20240420/libcfile/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -547,16 +547,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBCFILE_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBCFILE_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBCFILE_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBCFILE_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBCFILE_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBCFILE_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_LOCAL_LIBCFILE_TRUE@	@LIBCLOCALE_CPPFLAGS@ \
 @HAVE_LOCAL_LIBCFILE_TRUE@	@LIBCNOTIFY_CPPFLAGS@ \
 @HAVE_LOCAL_LIBCFILE_TRUE@	@LIBUNA_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBCFILE_TRUE@noinst_LTLIBRARIES = libcfile.la
 @HAVE_LOCAL_LIBCFILE_TRUE@libcfile_la_SOURCES = \
@@ -571,15 +571,16 @@
 @HAVE_LOCAL_LIBCFILE_TRUE@	libcfile_notify.c libcfile_notify.h \
 @HAVE_LOCAL_LIBCFILE_TRUE@	libcfile_support.c libcfile_support.h \
 @HAVE_LOCAL_LIBCFILE_TRUE@	libcfile_system_string.c libcfile_system_string.h \
 @HAVE_LOCAL_LIBCFILE_TRUE@	libcfile_types.h \
 @HAVE_LOCAL_LIBCFILE_TRUE@	libcfile_unused.h \
 @HAVE_LOCAL_LIBCFILE_TRUE@	libcfile_winapi.c libcfile_winapi.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -784,24 +785,32 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libcfile_error.Plo
+	-rm -f ./$(DEPDIR)/libcfile_file.Plo
+	-rm -f ./$(DEPDIR)/libcfile_notify.Plo
+	-rm -f ./$(DEPDIR)/libcfile_support.Plo
+	-rm -f ./$(DEPDIR)/libcfile_system_string.Plo
+	-rm -f ./$(DEPDIR)/libcfile_winapi.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -890,17 +899,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcfile ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcfile_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libesedb-20240202/libcfile/libcfile_error.c` & `libesedb-20240420/libcfile/libcfile_error.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libcfile/libcfile_libuna.h` & `libesedb-20240420/libcfile/libcfile_libuna.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libcfile/libcfile_winapi.c` & `libesedb-20240420/libcfile/libcfile_winapi.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libcfile/libcfile_definitions.h` & `libesedb-20240420/libcfile/libcfile_definitions.h`

 * *Files 2% similar despite different names*

```diff
@@ -31,19 +31,19 @@
 #include <libcfile/definitions.h>
 
 /* The definitions in <libcfile/definitions.h> are copied here
  * for local use of libcfile
  */
 #else
 
-#define LIBCFILE_VERSION				20240106
+#define LIBCFILE_VERSION				20240414
 
 /* The libcfile version string
  */
-#define LIBCFILE_VERSION_STRING				"20240106"
+#define LIBCFILE_VERSION_STRING				"20240414"
 
 /* The file access flags
  * bit 1	set to 1 for read access
  * bit 2	set to 1 for write access
  * bit 3	set to 1 to truncate an existing file on write
  * bit 4-8	not used
  */
```

### Comparing `libesedb-20240202/README` & `libesedb-20240420/README`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libmapidb/libmapidb_unused.h` & `libesedb-20240420/libmapidb/libmapidb_unused.h`

 * *Files 24% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 /*
- * The internal unused definition
+ * Definitions to silence compiler warnings about unused function attributes/parameters.
  *
- * Copyright (C) 2011-2017, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
- * This software is free software: you can redistribute it and/or modify
+ * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
  *
- * This software is distributed in the hope that it will be useful,
+ * This program is distributed in the hope that it will be useful,
  * but WITHOUT ANY WARRANTY; without even the implied warranty of
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License
- * along with this software.  If not, see <http://www.gnu.org/licenses/>.
+ * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
-#if !defined( _LIBMAPIDB_INTERNAL_UNUSED_H )
-#define _LIBMAPIDB_INTERNAL_UNUSED_H
+#if !defined( _LIBMAPIDB_UNUSED_H )
+#define _LIBMAPIDB_UNUSED_H
 
 #include <common.h>
 
 #if !defined( LIBMAPIDB_ATTRIBUTE_UNUSED )
 #if defined( __GNUC__ ) && __GNUC__ >= 3
 #define LIBMAPIDB_ATTRIBUTE_UNUSED	__attribute__ ((__unused__))
 #else
@@ -36,9 +36,9 @@
 #define LIBMAPIDB_UNREFERENCED_PARAMETER( parameter ) \
 	UNREFERENCED_PARAMETER( parameter );
 #else
 #define LIBMAPIDB_UNREFERENCED_PARAMETER( parameter ) \
 	/* parameter */
 #endif
 
-#endif /* !defined( _LIBMAPIDB_INTERNAL_UNUSED_H ) */
+#endif /* !defined( _LIBMAPIDB_UNUSED_H ) */
```

### Comparing `libesedb-20240202/libmapidb/libmapidb_libcnotify.h` & `libesedb-20240420/libmapidb/libmapidb_libcnotify.h`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 /*
  * The internal libcnotify header
  *
- * Copyright (C) 2011-2017, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
- * This software is free software: you can redistribute it and/or modify
+ * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
  *
- * This software is distributed in the hope that it will be useful,
+ * This program is distributed in the hope that it will be useful,
  * but WITHOUT ANY WARRANTY; without even the implied warranty of
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License
- * along with this software.  If not, see <http://www.gnu.org/licenses/>.
+ * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
 #if !defined( _LIBMAPIDB_LIBCNOTIFY_H )
 #define _LIBMAPIDB_LIBCNOTIFY_H
 
 #include <common.h>
```

### Comparing `libesedb-20240202/libmapidb/libmapidb_folder.h` & `libesedb-20240420/libmapidb/libmapidb_folder.h`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 /*
  * Folder functions
  *
- * Copyright (C) 2011-2017, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
- * This software is free software: you can redistribute it and/or modify
+ * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
  *
- * This software is distributed in the hope that it will be useful,
+ * This program is distributed in the hope that it will be useful,
  * but WITHOUT ANY WARRANTY; without even the implied warranty of
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License
- * along with this software.  If not, see <http://www.gnu.org/licenses/>.
+ * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
 #if !defined( _LIBMAPIDB_INTERNAL_FOLDER_H )
 #define _LIBMAPIDB_INTERNAL_FOLDER_H
 
 #include <common.h>
 #include <types.h>
```

### Comparing `libesedb-20240202/libmapidb/libmapidb_error.h` & `libesedb-20240420/libmapidb/libmapidb_error.h`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 /*
  * Error functions
  *
- * Copyright (C) 2011-2017, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
- * This software is free software: you can redistribute it and/or modify
+ * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
  *
- * This software is distributed in the hope that it will be useful,
+ * This program is distributed in the hope that it will be useful,
  * but WITHOUT ANY WARRANTY; without even the implied warranty of
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License
- * along with this software.  If not, see <http://www.gnu.org/licenses/>.
+ * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
 #if !defined( _LIBMAPIDB_INTERNAL_ERROR_H )
 #define _LIBMAPIDB_INTERNAL_ERROR_H
 
 #include <common.h>
 #include <file_stream.h>
```

### Comparing `libesedb-20240202/libmapidb/Makefile.am` & `libesedb-20240420/libmapidb/Makefile.am`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 if HAVE_LOCAL_LIBMAPIDB
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
-	@LIBCNOTIFY_CPPFLAGS@
+	@LIBCNOTIFY_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libmapidb.la
 
 libmapidb_la_SOURCES = \
 	libmapidb_database.c libmapidb_database.h \
 	libmapidb_definitions.h \
 	libmapidb_error.c libmapidb_error.h \
@@ -16,17 +16,17 @@
 	libmapidb_libcerror.h \
 	libmapidb_libcnotify.h \
 	libmapidb_support.c libmapidb_support.h \
 	libmapidb_types.h \
 	libmapidb_unused.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	/bin/rm -f Makefile
+sources-local: $(BUILT_SOURCES)
 
-splint:
+splint-local:
 	@echo "Running splint on libmapidb ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libmapidb_la_SOURCES)
```

### Comparing `libesedb-20240202/libmapidb/libmapidb_database.h` & `libesedb-20240420/libmapidb/libmapidb_database.h`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 /*
  * Database functions
  *
- * Copyright (C) 2011-2017, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
- * This software is free software: you can redistribute it and/or modify
+ * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
  *
- * This software is distributed in the hope that it will be useful,
+ * This program is distributed in the hope that it will be useful,
  * but WITHOUT ANY WARRANTY; without even the implied warranty of
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License
- * along with this software.  If not, see <http://www.gnu.org/licenses/>.
+ * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
 #if !defined( _LIBMAPIDB_INTERNAL_DATABASE_H )
 #define _LIBMAPIDB_INTERNAL_DATABASE_H
 
 #include <common.h>
 #include <types.h>
```

### Comparing `libesedb-20240202/libmapidb/libmapidb_types.h` & `libesedb-20240420/libmapidb/libmapidb_types.h`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 /*
  * The internal type definitions
  *
- * Copyright (C) 2011-2017, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
- * This software is free software: you can redistribute it and/or modify
+ * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
  *
- * This software is distributed in the hope that it will be useful,
+ * This program is distributed in the hope that it will be useful,
  * but WITHOUT ANY WARRANTY; without even the implied warranty of
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License
- * along with this software.  If not, see <http://www.gnu.org/licenses/>.
+ * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
 #if !defined( _LIBMAPIDB_INTERNAL_TYPES_H )
 #define _LIBMAPIDB_INTERNAL_TYPES_H
 
 #include <common.h>
 #include <types.h>
```

### Comparing `libesedb-20240202/libmapidb/libmapidb_folder.c` & `libesedb-20240420/libmapidb/libmapidb_folder.c`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 /*
  * Folder functions
  *
- * Copyright (C) 2011-2017, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
- * This software is free software: you can redistribute it and/or modify
+ * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
  *
- * This software is distributed in the hope that it will be useful,
+ * This program is distributed in the hope that it will be useful,
  * but WITHOUT ANY WARRANTY; without even the implied warranty of
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License
- * along with this software.  If not, see <http://www.gnu.org/licenses/>.
+ * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
 #include <common.h>
 #include <byte_stream.h>
 #include <memory.h>
 #include <types.h>
```

### Comparing `libesedb-20240202/libmapidb/libmapidb_database.c` & `libesedb-20240420/libmapidb/libmapidb_database.c`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 /*
  * Database functions
  *
- * Copyright (C) 2011-2017, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
- * This software is free software: you can redistribute it and/or modify
+ * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
  *
- * This software is distributed in the hope that it will be useful,
+ * This program is distributed in the hope that it will be useful,
  * but WITHOUT ANY WARRANTY; without even the implied warranty of
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License
- * along with this software.  If not, see <http://www.gnu.org/licenses/>.
+ * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
 #include <common.h>
 #include <byte_stream.h>
 #include <memory.h>
 #include <types.h>
```

### Comparing `libesedb-20240202/libmapidb/libmapidb_libcerror.h` & `libesedb-20240420/libcthreads/libcthreads_libcerror.h`

 * *Files 7% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 /*
- * The internal libcerror header
+ * The libcerror header wrapper
  *
- * Copyright (C) 2011-2017, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2012-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
- * This software is free software: you can redistribute it and/or modify
+ * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
  *
- * This software is distributed in the hope that it will be useful,
+ * This program is distributed in the hope that it will be useful,
  * but WITHOUT ANY WARRANTY; without even the implied warranty of
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License
- * along with this software.  If not, see <http://www.gnu.org/licenses/>.
+ * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
-#if !defined( _LIBMAPIDB_LIBCERROR_H )
-#define _LIBMAPIDB_LIBCERROR_H
+#if !defined( _LIBCTHREADS_LIBCERROR_H )
+#define _LIBCTHREADS_LIBCERROR_H
 
 #include <common.h>
 
 /* Define HAVE_LOCAL_LIBCERROR for local use of libcerror
  */
 #if defined( HAVE_LOCAL_LIBCERROR )
 
@@ -42,9 +42,9 @@
 #define LIBCERROR_DLL_IMPORT
 #endif
 
 #include <libcerror.h>
 
 #endif /* defined( HAVE_LOCAL_LIBCERROR ) */
 
-#endif /* !defined( _LIBMAPIDB_LIBCERROR_H ) */
+#endif /* !defined( _LIBCTHREADS_LIBCERROR_H ) */
```

### Comparing `libesedb-20240202/libmapidb/Makefile.in` & `libesedb-20240420/libmapidb/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -544,33 +544,34 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBMAPIDB_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBMAPIDB_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBMAPIDB_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBMAPIDB_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBMAPIDB_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBMAPIDB_TRUE@	@LIBCERROR_CPPFLAGS@ \
-@HAVE_LOCAL_LIBMAPIDB_TRUE@	@LIBCNOTIFY_CPPFLAGS@
+@HAVE_LOCAL_LIBMAPIDB_TRUE@	@LIBCNOTIFY_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBMAPIDB_TRUE@noinst_LTLIBRARIES = libmapidb.la
 @HAVE_LOCAL_LIBMAPIDB_TRUE@libmapidb_la_SOURCES = \
 @HAVE_LOCAL_LIBMAPIDB_TRUE@	libmapidb_database.c libmapidb_database.h \
 @HAVE_LOCAL_LIBMAPIDB_TRUE@	libmapidb_definitions.h \
 @HAVE_LOCAL_LIBMAPIDB_TRUE@	libmapidb_error.c libmapidb_error.h \
 @HAVE_LOCAL_LIBMAPIDB_TRUE@	libmapidb_extern.h \
 @HAVE_LOCAL_LIBMAPIDB_TRUE@	libmapidb_folder.c libmapidb_folder.h \
 @HAVE_LOCAL_LIBMAPIDB_TRUE@	libmapidb_libcerror.h \
 @HAVE_LOCAL_LIBMAPIDB_TRUE@	libmapidb_libcnotify.h \
 @HAVE_LOCAL_LIBMAPIDB_TRUE@	libmapidb_support.c libmapidb_support.h \
 @HAVE_LOCAL_LIBMAPIDB_TRUE@	libmapidb_types.h \
 @HAVE_LOCAL_LIBMAPIDB_TRUE@	libmapidb_unused.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -773,24 +774,30 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libmapidb_database.Plo
+	-rm -f ./$(DEPDIR)/libmapidb_error.Plo
+	-rm -f ./$(DEPDIR)/libmapidb_folder.Plo
+	-rm -f ./$(DEPDIR)/libmapidb_support.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -851,14 +858,16 @@
 
 ps-am:
 
 sources: sources-am
 
 sources-am: sources-local
 
+splint: splint-am
+
 splint-am: splint-local
 
 uninstall-am:
 
 .MAKE: install-am install-strip
 
 .PHONY: CTAGS GTAGS TAGS all all-am am--depfiles check check-am clean \
@@ -869,23 +878,22 @@
 	install-data install-data-am install-dvi install-dvi-am \
 	install-exec install-exec-am install-html install-html-am \
 	install-info install-info-am install-man install-pdf \
 	install-pdf-am install-ps install-ps-am install-strip \
 	installcheck installcheck-am installdirs maintainer-clean \
 	maintainer-clean-generic mostlyclean mostlyclean-compile \
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
-	sources-am sources-local splint splint-am splint-local tags \
-	tags-am uninstall uninstall-am
+	sources-am sources-local splint-am splint-local tags tags-am \
+	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	/bin/rm -f Makefile
+sources-local: $(BUILT_SOURCES)
 
-splint:
+splint-local:
 	@echo "Running splint on libmapidb ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libmapidb_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libesedb-20240202/libmapidb/libmapidb_support.h` & `libesedb-20240420/libmapidb/libmapidb_support.h`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 /*
  * Support functions
  *
- * Copyright (C) 2011-2017, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
- * This software is free software: you can redistribute it and/or modify
+ * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
  *
- * This software is distributed in the hope that it will be useful,
+ * This program is distributed in the hope that it will be useful,
  * but WITHOUT ANY WARRANTY; without even the implied warranty of
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License
- * along with this software.  If not, see <http://www.gnu.org/licenses/>.
+ * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
 #if !defined( _LIBMAPIDB_SUPPORT_H )
 #define _LIBMAPIDB_SUPPORT_H
 
 #include <common.h>
 #include <types.h>
```

### Comparing `libesedb-20240202/libmapidb/libmapidb_extern.h` & `libesedb-20240420/libcpath/libcpath_extern.h`

 * *Files 16% similar despite different names*

```diff
@@ -1,46 +1,46 @@
 /*
  * The internal extern definition
  *
- * Copyright (C) 2011-2017, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
- * This software is free software: you can redistribute it and/or modify
+ * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
  *
- * This software is distributed in the hope that it will be useful,
+ * This program is distributed in the hope that it will be useful,
  * but WITHOUT ANY WARRANTY; without even the implied warranty of
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License
- * along with this software.  If not, see <http://www.gnu.org/licenses/>.
+ * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
-#if !defined( _LIBMAPIDB_INTERNAL_EXTERN_H )
-#define _LIBMAPIDB_INTERNAL_EXTERN_H
+#if !defined( _LIBCPATH_INTERNAL_EXTERN_H )
+#define _LIBCPATH_INTERNAL_EXTERN_H
 
 #include <common.h>
 
-/* Define HAVE_LOCAL_LIBMAPIDB for local use of libmapidb
+/* Define HAVE_LOCAL_LIBCPATH for local use of libcpath
  */
-#if !defined( HAVE_LOCAL_LIBMAPIDB )
+#if !defined( HAVE_LOCAL_LIBCPATH )
 
-/* If libtool DLL support is enabled set LIBMAPIDB_DLL_EXPORT
- * before including libmapidb/extern.h
- */
-#if defined( _WIN32 ) && defined( DLL_EXPORT )
-#define LIBMAPIDB_DLL_EXPORT
-#endif
+#include <libcpath/extern.h>
 
-#include <libmapidb/extern.h>
+#if defined( __CYGWIN__ ) || defined( __MINGW32__ )
+#define LIBCPATH_EXTERN_VARIABLE	extern
+#else
+#define LIBCPATH_EXTERN_VARIABLE	LIBCPATH_EXTERN
+#endif
 
 #else
-#define LIBMAPIDB_EXTERN	/* extern */
+#define LIBCPATH_EXTERN		/* extern */
+#define LIBCPATH_EXTERN_VARIABLE	extern
 
-#endif /* !defined( HAVE_LOCAL_LIBMAPIDB ) */
+#endif /* !defined( HAVE_LOCAL_LIBCPATH ) */
 
-#endif /* !defined( _LIBMAPIDB_INTERNAL_EXTERN_H ) */
+#endif /* !defined( _LIBCPATH_INTERNAL_EXTERN_H ) */
```

### Comparing `libesedb-20240202/libmapidb/libmapidb_definitions.h` & `libesedb-20240420/libmapidb/libmapidb_definitions.h`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 /*
  * The internal definitions
  *
- * Copyright (C) 2011-2017, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
- * This software is free software: you can redistribute it and/or modify
+ * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
  *
- * This software is distributed in the hope that it will be useful,
+ * This program is distributed in the hope that it will be useful,
  * but WITHOUT ANY WARRANTY; without even the implied warranty of
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License
- * along with this software.  If not, see <http://www.gnu.org/licenses/>.
+ * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
 #if !defined( LIBMAPIDB_INTERNAL_DEFINITIONS_H )
 #define LIBMAPIDB_INTERNAL_DEFINITIONS_H
 
 #include <common.h>
 #include <types.h>
@@ -32,19 +32,19 @@
 
 /* The definitions in <libmapidb/definitions.h> are copied here
  * for local use of libmapidb
  */
 #else
 #include <byte_stream.h>
 
-#define LIBMAPIDB_VERSION				20170304
+#define LIBMAPIDB_VERSION				20240420
 
 /* The libmapidb version string
  */
-#define LIBMAPIDB_VERSION_STRING			"20170304"
+#define LIBMAPIDB_VERSION_STRING			"20240420"
 
 /* The endian definitions
  */
 #define LIBMAPIDB_ENDIAN_BIG				_BYTE_STREAM_ENDIAN_BIG
 #define LIBMAPIDB_ENDIAN_LITTLE				_BYTE_STREAM_ENDIAN_LITTLE
 
 #endif /* !defined( HAVE_LOCAL_LIBMAPIDB ) */
```

### Comparing `libesedb-20240202/libmapidb/libmapidb_error.c` & `libesedb-20240420/libfmapi/libfmapi_error.c`

 * *Files 8% similar despite different names*

```diff
@@ -1,51 +1,51 @@
 /*
  * Error functions
  *
- * Copyright (C) 2011-2017, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
- * This software is free software: you can redistribute it and/or modify
+ * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
  *
- * This software is distributed in the hope that it will be useful,
+ * This program is distributed in the hope that it will be useful,
  * but WITHOUT ANY WARRANTY; without even the implied warranty of
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License
- * along with this software.  If not, see <http://www.gnu.org/licenses/>.
+ * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
 #include <common.h>
 #include <file_stream.h>
 #include <types.h>
 
-#include "libmapidb_error.h"
-#include "libmapidb_libcerror.h"
+#include "libfmapi_error.h"
+#include "libfmapi_libcerror.h"
 
-#if !defined( HAVE_LOCAL_LIBMAPIDB )
+#if !defined( HAVE_LOCAL_LIBFMAPI )
 
 /* Free an error and its elements
  */
-void libmapidb_error_free(
-      libmapidb_error_t **error )
+void libfmapi_error_free(
+      libfmapi_error_t **error )
 {
 	libcerror_error_free(
 	 (libcerror_error_t **) error );
 }
 
 /* Prints a descriptive string of the error to the stream
  * Returns the number of printed characters if successful or -1 on error
  */
-int libmapidb_error_fprint(
-     libmapidb_error_t *error,
+int libfmapi_error_fprint(
+     libfmapi_error_t *error,
      FILE *stream )
 {
 	int print_count = 0;
 
 	print_count = libcerror_error_fprint(
 	               (libcerror_error_t *) error,
 	               stream );
@@ -53,16 +53,16 @@
 	return( print_count );
 }
 
 /* Prints a descriptive string of the error to the string
  * The end-of-string character is not included in the return value
  * Returns the number of printed characters if successful or -1 on error
  */
-int libmapidb_error_sprint(
-     libmapidb_error_t *error,
+int libfmapi_error_sprint(
+     libfmapi_error_t *error,
      char *string,
      size_t size )
 {
 	int print_count = 0;
 
 	print_count = libcerror_error_sprint(
 	               (libcerror_error_t *) error,
@@ -71,16 +71,16 @@
 
 	return( print_count );
 }
 
 /* Prints a backtrace of the error to the stream
  * Returns the number of printed characters if successful or -1 on error
  */
-int libmapidb_error_backtrace_fprint(
-     libmapidb_error_t *error,
+int libfmapi_error_backtrace_fprint(
+     libfmapi_error_t *error,
       FILE *stream )
 {
 	int print_count = 0;
 
 	print_count = libcerror_error_backtrace_fprint(
 	               (libcerror_error_t *) error,
 	               stream );
@@ -88,24 +88,24 @@
 	return( print_count );
 }
 
 /* Prints a backtrace of the error to the string
  * The end-of-string character is not included in the return value
  * Returns the number of printed characters if successful or -1 on error
  */
-int libmapidb_error_backtrace_sprint(
-     libmapidb_error_t *error,
+int libfmapi_error_backtrace_sprint(
+     libfmapi_error_t *error,
      char *string,
      size_t size )
 {
 	int print_count = 0;
 
 	print_count = libcerror_error_backtrace_sprint(
 	               (libcerror_error_t *) error,
 	               string,
 	               size );
 
 	return( print_count );
 }
 
-#endif /* !defined( HAVE_LOCAL_LIBMAPIDB ) */
+#endif /* !defined( HAVE_LOCAL_LIBFMAPI ) */
```

### Comparing `libesedb-20240202/libmapidb/libmapidb_support.c` & `libesedb-20240420/libuna/libuna_support.c`

 * *Files 14% similar despite different names*

```diff
@@ -1,42 +1,39 @@
 /*
  * Support functions
  *
- * Copyright (C) 2011-2017, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
- * This software is free software: you can redistribute it and/or modify
+ * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
  *
- * This software is distributed in the hope that it will be useful,
+ * This program is distributed in the hope that it will be useful,
  * but WITHOUT ANY WARRANTY; without even the implied warranty of
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License
- * along with this software.  If not, see <http://www.gnu.org/licenses/>.
+ * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
 #include <common.h>
 #include <types.h>
 
-#include <stdio.h>
+#include "libuna_definitions.h"
+#include "libuna_support.h"
 
-#include "libmapidb_definitions.h"
-#include "libmapidb_libcerror.h"
-#include "libmapidb_support.h"
-
-#if !defined( HAVE_LOCAL_LIBMAPIDB )
+#if !defined( HAVE_LOCAL_LIBUNA )
 
 /* Returns the library version as a string
  */
-const char *libmapidb_get_version(
+const char *libuna_get_version(
              void )
 {
-	return( (const char *) LIBMAPIDB_VERSION_STRING );
+	return( (const char *) LIBUNA_VERSION_STRING );
 }
 
-#endif
+#endif /* !defined( HAVE_LOCAL_LIBUNA ) */
```

### Comparing `libesedb-20240202/INSTALL` & `libesedb-20240420/INSTALL`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libcdata/libcdata_list_element.h` & `libesedb-20240420/libcdata/libcdata_list_element.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libcdata/libcdata_array.h` & `libesedb-20240420/libcdata/libcdata_array.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libcdata/libcdata_definitions.h` & `libesedb-20240420/libcdata/libcdata_definitions.h`

 * *Files 2% similar despite different names*

```diff
@@ -31,19 +31,19 @@
 #include <libcdata/definitions.h>
 
 /* The definitions in <libcdata/definitions.h> are copied here
  * for local use of libcdata
  */
 #else
 
-#define LIBCDATA_VERSION				20240103
+#define LIBCDATA_VERSION				20240414
 
 /* The libcdata version string
  */
-#define LIBCDATA_VERSION_STRING				"20240103"
+#define LIBCDATA_VERSION_STRING				"20240414"
 
 /* The comparison function definitions
  */
 enum LIBCDATA_COMPARE_DEFINITIONS
 {
 	/* The first value is less than the second value
 	 */
```

### Comparing `libesedb-20240202/libcdata/libcdata_libcerror.h` & `libesedb-20240420/libcdata/libcdata_libcerror.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libcdata/libcdata_unused.h` & `libesedb-20240420/libcdata/libcdata_unused.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libcdata/libcdata_btree.h` & `libesedb-20240420/libcdata/libcdata_btree.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libcdata/libcdata_btree.c` & `libesedb-20240420/libcdata/libcdata_btree.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libcdata/libcdata_support.c` & `libesedb-20240420/libcdata/libcdata_support.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libcdata/libcdata_list.c` & `libesedb-20240420/libcdata/libcdata_list.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libcdata/libcdata_extern.h` & `libesedb-20240420/libcdata/libcdata_extern.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libcdata/libcdata_list.h` & `libesedb-20240420/libcdata/libcdata_list.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libcdata/libcdata_btree_values_list.h` & `libesedb-20240420/libcdata/libcdata_btree_values_list.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libcdata/Makefile.am` & `libesedb-20240420/libcdata/Makefile.am`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBCDATA
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCTHREADS_CPPFLAGS@ \
 	@PTHREAD_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libcdata.la
 
 libcdata_la_SOURCES = \
@@ -24,19 +24,17 @@
 	libcdata_range_list_value.c libcdata_range_list_value.h \
 	libcdata_support.c libcdata_support.h \
 	libcdata_tree_node.c libcdata_tree_node.h \
 	libcdata_types.h \
 	libcdata_unused.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcdata ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcdata_la_SOURCES)
```

### Comparing `libesedb-20240202/libcdata/libcdata_btree_node.h` & `libesedb-20240420/libcdata/libcdata_btree_node.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libcdata/libcdata_range_list_value.h` & `libesedb-20240420/libcdata/libcdata_range_list_value.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libcdata/libcdata_range_list.h` & `libesedb-20240420/libcdata/libcdata_range_list.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libcdata/libcdata_range_list.c` & `libesedb-20240420/libcdata/libcdata_range_list.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libcdata/libcdata_array.c` & `libesedb-20240420/libcdata/libcdata_array.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libcdata/libcdata_list_element.c` & `libesedb-20240420/libcdata/libcdata_list_element.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libcdata/libcdata_libcthreads.h` & `libesedb-20240420/libcdata/libcdata_libcthreads.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libcdata/libcdata_tree_node.h` & `libesedb-20240420/libcdata/libcdata_tree_node.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libcdata/libcdata_error.h` & `libesedb-20240420/libcdata/libcdata_error.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libcdata/libcdata_types.h` & `libesedb-20240420/libcdata/libcdata_types.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libcdata/libcdata_btree_node.c` & `libesedb-20240420/libcdata/libcdata_btree_node.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libcdata/libcdata_tree_node.c` & `libesedb-20240420/libcdata/libcdata_tree_node.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libcdata/libcdata_support.h` & `libesedb-20240420/libcdata/libcdata_support.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libcdata/Makefile.in` & `libesedb-20240420/libcdata/Makefile.in`

 * *Files 3% similar despite different names*

```diff
@@ -561,16 +561,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBCDATA_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBCDATA_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBCDATA_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBCDATA_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBCDATA_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBCDATA_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_LOCAL_LIBCDATA_TRUE@	@LIBCTHREADS_CPPFLAGS@ \
 @HAVE_LOCAL_LIBCDATA_TRUE@	@PTHREAD_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBCDATA_TRUE@noinst_LTLIBRARIES = libcdata.la
 @HAVE_LOCAL_LIBCDATA_TRUE@libcdata_la_SOURCES = \
 @HAVE_LOCAL_LIBCDATA_TRUE@	libcdata_array.c libcdata_array.h \
@@ -587,15 +587,16 @@
 @HAVE_LOCAL_LIBCDATA_TRUE@	libcdata_range_list.c libcdata_range_list.h \
 @HAVE_LOCAL_LIBCDATA_TRUE@	libcdata_range_list_value.c libcdata_range_list_value.h \
 @HAVE_LOCAL_LIBCDATA_TRUE@	libcdata_support.c libcdata_support.h \
 @HAVE_LOCAL_LIBCDATA_TRUE@	libcdata_tree_node.c libcdata_tree_node.h \
 @HAVE_LOCAL_LIBCDATA_TRUE@	libcdata_types.h \
 @HAVE_LOCAL_LIBCDATA_TRUE@	libcdata_unused.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -805,24 +806,37 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libcdata_array.Plo
+	-rm -f ./$(DEPDIR)/libcdata_btree.Plo
+	-rm -f ./$(DEPDIR)/libcdata_btree_node.Plo
+	-rm -f ./$(DEPDIR)/libcdata_btree_values_list.Plo
+	-rm -f ./$(DEPDIR)/libcdata_error.Plo
+	-rm -f ./$(DEPDIR)/libcdata_list.Plo
+	-rm -f ./$(DEPDIR)/libcdata_list_element.Plo
+	-rm -f ./$(DEPDIR)/libcdata_range_list.Plo
+	-rm -f ./$(DEPDIR)/libcdata_range_list_value.Plo
+	-rm -f ./$(DEPDIR)/libcdata_support.Plo
+	-rm -f ./$(DEPDIR)/libcdata_tree_node.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -916,17 +930,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcdata ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcdata_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libesedb-20240202/libcdata/libcdata_range_list_value.c` & `libesedb-20240420/libcdata/libcdata_range_list_value.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libcdata/libcdata_btree_values_list.c` & `libesedb-20240420/libcdata/libcdata_btree_values_list.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libcdata/libcdata_error.c` & `libesedb-20240420/libcdata/libcdata_error.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfmapi/libfmapi_value_type.h` & `libesedb-20240420/libfmapi/libfmapi_value_type.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfmapi/libfmapi_debug.c` & `libesedb-20240420/libfmapi/libfmapi_debug.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfmapi/libfmapi_x400_object_identifier.h` & `libesedb-20240420/libfmapi/libfmapi_x400_object_identifier.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfmapi/libfmapi_libfguid.h` & `libesedb-20240420/libfmapi/libfmapi_libfguid.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfmapi/libfmapi_libcnotify.h` & `libesedb-20240420/libfmapi/libfmapi_libcnotify.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfmapi/libfmapi_entry_identifier.h` & `libesedb-20240420/libfmapi/libfmapi_entry_identifier.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfmapi/libfmapi_libfwnt.h` & `libesedb-20240420/libfmapi/libfmapi_libfwnt.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfmapi/libfmapi_one_off_entry_identifier.c` & `libesedb-20240420/libfmapi/libfmapi_one_off_entry_identifier.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfmapi/libfmapi_one_off_entry_identifier.h` & `libesedb-20240420/libfmapi/libfmapi_one_off_entry_identifier.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfmapi/libfmapi_codepage.h` & `libesedb-20240420/libfmapi/libfmapi_codepage.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfmapi/libfmapi_codepage.c` & `libesedb-20240420/libfmapi/libfmapi_codepage.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfmapi/Makefile.am` & `libesedb-20240420/libfmapi/Makefile.am`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBFMAPI
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCTHREADS_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ \
 	@LIBFDATETIME_CPPFLAGS@ \
 	@LIBFGUID_CPPFLAGS@ \
@@ -36,19 +36,17 @@
 	libfmapi_support.c libfmapi_support.h \
 	libfmapi_types.h \
 	libfmapi_unused.h \
 	libfmapi_value_type.c libfmapi_value_type.h \
 	libfmapi_x400_object_identifier.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libfmapi ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfmapi_la_SOURCES)
```

### Comparing `libesedb-20240202/libfmapi/libfmapi_error.h` & `libesedb-20240420/libfmapi/libfmapi_error.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfmapi/libfmapi_debug.h` & `libesedb-20240420/libfmapi/libfmapi_debug.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfmapi/libfmapi_entry_identifier.c` & `libesedb-20240420/libfmapi/libfmapi_entry_identifier.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfmapi/libfmapi_class_identifier.h` & `libesedb-20240420/libfmapi/libfmapi_class_identifier.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfmapi/libfmapi_value_type.c` & `libesedb-20240420/libfmapi/libfmapi_value_type.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfmapi/libfmapi_libuna.h` & `libesedb-20240420/libfmapi/libfmapi_libuna.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfmapi/libfmapi_definitions.h` & `libesedb-20240420/libfmapi/libfmapi_definitions.h`

 * *Files 2% similar despite different names*

```diff
@@ -32,19 +32,19 @@
 
 /* The definitions in <libfmapi/definitions.h> are copied here
  * for local use of libfmapi
  */
 #else
 #include <byte_stream.h>
 
-#define LIBFMAPI_VERSION					20240117
+#define LIBFMAPI_VERSION					20240415
 
 /* The libfmapi version string
  */
-#define LIBFMAPI_VERSION_STRING					"20240117"
+#define LIBFMAPI_VERSION_STRING					"20240415"
 
 /* The endian definitions
  */
 #define LIBFMAPI_ENDIAN_BIG					_BYTE_STREAM_ENDIAN_BIG
 #define LIBFMAPI_ENDIAN_LITTLE					_BYTE_STREAM_ENDIAN_LITTLE
 
 enum LIBFMAPI_ENTRY_IDENTIFIER_FLAGS
```

### Comparing `libesedb-20240202/libfmapi/libfmapi_support.c` & `libesedb-20240420/libfmapi/libfmapi_support.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfmapi/libfmapi_unused.h` & `libesedb-20240420/libfmapi/libfmapi_unused.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfmapi/libfmapi_class_identifier.c` & `libesedb-20240420/libfmapi/libfmapi_class_identifier.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfmapi/libfmapi_checksum.h` & `libesedb-20240420/libfmapi/libfmapi_checksum.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfmapi/libfmapi_checksum.c` & `libesedb-20240420/libfmapi/libfmapi_checksum.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfmapi/libfmapi_property_type.c` & `libesedb-20240420/libfmapi/libfmapi_property_type.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfmapi/libfmapi_libfdatetime.h` & `libesedb-20240420/libfmapi/libfmapi_libfdatetime.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfmapi/libfmapi_lzfu.c` & `libesedb-20240420/libfmapi/libfmapi_lzfu.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfmapi/libfmapi_types.h` & `libesedb-20240420/libfmapi/libfmapi_types.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfmapi/libfmapi_property_type.h` & `libesedb-20240420/libfmapi/libfmapi_property_type.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfmapi/libfmapi_lzfu.h` & `libesedb-20240420/libfmapi/libfmapi_lzfu.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfmapi/libfmapi_libcerror.h` & `libesedb-20240420/libfmapi/libfmapi_libcerror.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfmapi/libfmapi_service_provider_identifier.c` & `libesedb-20240420/libfmapi/libfmapi_service_provider_identifier.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfmapi/libfmapi_error.c` & `libesedb-20240420/libcsplit/libcsplit_error.c`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Error functions
  *
- * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -19,33 +19,33 @@
  * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
 #include <common.h>
 #include <file_stream.h>
 #include <types.h>
 
-#include "libfmapi_error.h"
-#include "libfmapi_libcerror.h"
+#include "libcsplit_error.h"
+#include "libcsplit_libcerror.h"
 
-#if !defined( HAVE_LOCAL_LIBFMAPI )
+#if !defined( HAVE_LOCAL_LIBCSPLIT )
 
 /* Free an error and its elements
  */
-void libfmapi_error_free(
-      libfmapi_error_t **error )
+void libcsplit_error_free(
+      libcsplit_error_t **error )
 {
 	libcerror_error_free(
 	 (libcerror_error_t **) error );
 }
 
 /* Prints a descriptive string of the error to the stream
  * Returns the number of printed characters if successful or -1 on error
  */
-int libfmapi_error_fprint(
-     libfmapi_error_t *error,
+int libcsplit_error_fprint(
+     libcsplit_error_t *error,
      FILE *stream )
 {
 	int print_count = 0;
 
 	print_count = libcerror_error_fprint(
 	               (libcerror_error_t *) error,
 	               stream );
@@ -53,16 +53,16 @@
 	return( print_count );
 }
 
 /* Prints a descriptive string of the error to the string
  * The end-of-string character is not included in the return value
  * Returns the number of printed characters if successful or -1 on error
  */
-int libfmapi_error_sprint(
-     libfmapi_error_t *error,
+int libcsplit_error_sprint(
+     libcsplit_error_t *error,
      char *string,
      size_t size )
 {
 	int print_count = 0;
 
 	print_count = libcerror_error_sprint(
 	               (libcerror_error_t *) error,
@@ -71,16 +71,16 @@
 
 	return( print_count );
 }
 
 /* Prints a backtrace of the error to the stream
  * Returns the number of printed characters if successful or -1 on error
  */
-int libfmapi_error_backtrace_fprint(
-     libfmapi_error_t *error,
+int libcsplit_error_backtrace_fprint(
+     libcsplit_error_t *error,
       FILE *stream )
 {
 	int print_count = 0;
 
 	print_count = libcerror_error_backtrace_fprint(
 	               (libcerror_error_t *) error,
 	               stream );
@@ -88,24 +88,24 @@
 	return( print_count );
 }
 
 /* Prints a backtrace of the error to the string
  * The end-of-string character is not included in the return value
  * Returns the number of printed characters if successful or -1 on error
  */
-int libfmapi_error_backtrace_sprint(
-     libfmapi_error_t *error,
+int libcsplit_error_backtrace_sprint(
+     libcsplit_error_t *error,
      char *string,
      size_t size )
 {
 	int print_count = 0;
 
 	print_count = libcerror_error_backtrace_sprint(
 	               (libcerror_error_t *) error,
 	               string,
 	               size );
 
 	return( print_count );
 }
 
-#endif /* !defined( HAVE_LOCAL_LIBFMAPI ) */
+#endif /* !defined( HAVE_LOCAL_LIBCSPLIT ) */
```

### Comparing `libesedb-20240202/libfmapi/Makefile.in` & `libesedb-20240420/libfmapi/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -569,16 +569,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBFMAPI_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBFMAPI_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBFMAPI_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBFMAPI_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBFMAPI_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBFMAPI_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFMAPI_TRUE@	@LIBCDATA_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFMAPI_TRUE@	@LIBCTHREADS_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFMAPI_TRUE@	@LIBCNOTIFY_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFMAPI_TRUE@	@LIBUNA_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFMAPI_TRUE@	@LIBFDATETIME_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFMAPI_TRUE@	@LIBFGUID_CPPFLAGS@ \
@@ -607,15 +607,16 @@
 @HAVE_LOCAL_LIBFMAPI_TRUE@	libfmapi_service_provider_identifier.c libfmapi_service_provider_identifier.h \
 @HAVE_LOCAL_LIBFMAPI_TRUE@	libfmapi_support.c libfmapi_support.h \
 @HAVE_LOCAL_LIBFMAPI_TRUE@	libfmapi_types.h \
 @HAVE_LOCAL_LIBFMAPI_TRUE@	libfmapi_unused.h \
 @HAVE_LOCAL_LIBFMAPI_TRUE@	libfmapi_value_type.c libfmapi_value_type.h \
 @HAVE_LOCAL_LIBFMAPI_TRUE@	libfmapi_x400_object_identifier.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -826,24 +827,38 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libfmapi_checksum.Plo
+	-rm -f ./$(DEPDIR)/libfmapi_class_identifier.Plo
+	-rm -f ./$(DEPDIR)/libfmapi_codepage.Plo
+	-rm -f ./$(DEPDIR)/libfmapi_debug.Plo
+	-rm -f ./$(DEPDIR)/libfmapi_entry_identifier.Plo
+	-rm -f ./$(DEPDIR)/libfmapi_error.Plo
+	-rm -f ./$(DEPDIR)/libfmapi_lzfu.Plo
+	-rm -f ./$(DEPDIR)/libfmapi_one_off_entry_identifier.Plo
+	-rm -f ./$(DEPDIR)/libfmapi_property_type.Plo
+	-rm -f ./$(DEPDIR)/libfmapi_service_provider_identifier.Plo
+	-rm -f ./$(DEPDIR)/libfmapi_support.Plo
+	-rm -f ./$(DEPDIR)/libfmapi_value_type.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -938,17 +953,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libfmapi ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfmapi_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libesedb-20240202/libfmapi/libfmapi_support.h` & `libesedb-20240420/libfmapi/libfmapi_support.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfmapi/libfmapi_extern.h` & `libesedb-20240420/libfmapi/libfmapi_extern.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfmapi/libfmapi_service_provider_identifier.h` & `libesedb-20240420/libfmapi/libfmapi_service_provider_identifier.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/config.sub` & `libesedb-20240420/config.sub`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libesedb.spec` & `libesedb-20240420/libesedb.spec`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 Name: libesedb
-Version: 20240202
+Version: 20240420
 Release: 1
 Summary: Library to access the Extensible Storage Engine (ESE) Database File (EDB) format
 Group: System Environment/Libraries
 License: LGPL-3.0-or-later
 Source: %{name}-%{version}.tar.gz
 URL: https://github.com/libyal/libesedb
                 
@@ -91,10 +91,10 @@
 %files -n libesedb-tools
 %license COPYING COPYING.LESSER
 %doc AUTHORS README
 %{_bindir}/*
 %{_mandir}/man1/*
 
 %changelog
-* Fri Feb  2 2024 Joachim Metz <joachim.metz@gmail.com> 20240202-1
+* Sat Apr 20 2024 Joachim Metz <joachim.metz@gmail.com> 20240420-1
 - Auto-generated
```

### Comparing `libesedb-20240202/setup.py` & `libesedb-20240420/setup.py`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/acinclude.m4` & `libesedb-20240420/acinclude.m4`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libesedb.pc.in` & `libesedb-20240420/libesedb.pc.in`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/pyesedb/pyesedb_libbfio.h` & `libesedb-20240420/pyesedb/pyesedb_libbfio.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/pyesedb/pyesedb_records.c` & `libesedb-20240420/pyesedb/pyesedb_records.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/pyesedb/pyesedb_libclocale.h` & `libesedb-20240420/pyesedb/pyesedb_libclocale.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/pyesedb/pyesedb_libcerror.h` & `libesedb-20240420/pyesedb/pyesedb_libcerror.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/pyesedb/pyesedb_tables.h` & `libesedb-20240420/pyesedb/pyesedb_tables.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/pyesedb/pyesedb_records.h` & `libesedb-20240420/pyesedb/pyesedb_records.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/pyesedb/pyesedb_error.h` & `libesedb-20240420/pyesedb/pyesedb_error.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/pyesedb/pyesedb.c` & `libesedb-20240420/pyesedb/pyesedb.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/pyesedb/pyesedb_multi_value.c` & `libesedb-20240420/pyesedb/pyesedb_multi_value.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/pyesedb/pyesedb_file_object_io_handle.h` & `libesedb-20240420/pyesedb/pyesedb_file_object_io_handle.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/pyesedb/pyesedb_index.c` & `libesedb-20240420/pyesedb/pyesedb_index.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/pyesedb/pyesedb_table.c` & `libesedb-20240420/pyesedb/pyesedb_table.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/pyesedb/pyesedb_index.h` & `libesedb-20240420/pyesedb/pyesedb_index.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/pyesedb/pyesedb_multi_value.h` & `libesedb-20240420/pyesedb/pyesedb_multi_value.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/pyesedb/Makefile.am` & `libesedb-20240420/pyesedb/Makefile.am`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_PYTHON
 AM_CFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCSPLIT_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ \
 	@LIBCFILE_CPPFLAGS@ \
 	@LIBCPATH_CPPFLAGS@ \
@@ -53,13 +53,11 @@
 	@LIBBFIO_LIBADD@
 
 pyesedb_la_CPPFLAGS = $(PYTHON_CPPFLAGS)
 pyesedb_la_LDFLAGS  = -module -avoid-version $(PYTHON_LDFLAGS)
 
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
```

### Comparing `libesedb-20240202/pyesedb/pyesedb_column_types.h` & `libesedb-20240420/pyesedb/pyesedb_column_types.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/pyesedb/pyesedb_datetime.c` & `libesedb-20240420/pyesedb/pyesedb_datetime.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/pyesedb/pyesedb_file_types.c` & `libesedb-20240420/pyesedb/pyesedb_file_types.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/pyesedb/pyesedb_file.h` & `libesedb-20240420/pyesedb/pyesedb_file.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/pyesedb/pyesedb_python.h` & `libesedb-20240420/pyesedb/pyesedb_python.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/pyesedb/pyesedb_columns.c` & `libesedb-20240420/pyesedb/pyesedb_columns.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/pyesedb/pyesedb_long_value.h` & `libesedb-20240420/pyesedb/pyesedb_long_value.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/pyesedb/pyesedb_error.c` & `libesedb-20240420/pyesedb/pyesedb_error.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/pyesedb/pyesedb_integer.h` & `libesedb-20240420/pyesedb/pyesedb_integer.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/pyesedb/pyesedb.h` & `libesedb-20240420/pyesedb/pyesedb.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/pyesedb/pyesedb_integer.c` & `libesedb-20240420/pyesedb/pyesedb_integer.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/pyesedb/pyesedb_libesedb.h` & `libesedb-20240420/pyesedb/pyesedb_libesedb.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/pyesedb/pyesedb_indexes.c` & `libesedb-20240420/pyesedb/pyesedb_indexes.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/pyesedb/pyesedb_record.c` & `libesedb-20240420/pyesedb/pyesedb_record.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/pyesedb/pyesedb_tables.c` & `libesedb-20240420/pyesedb/pyesedb_tables.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/pyesedb/pyesedb_file_object_io_handle.c` & `libesedb-20240420/pyesedb/pyesedb_file_object_io_handle.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/pyesedb/pyesedb_unused.h` & `libesedb-20240420/pyesedb/pyesedb_unused.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/pyesedb/pyesedb_datetime.h` & `libesedb-20240420/pyesedb/pyesedb_datetime.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/pyesedb/pyesedb_value_flags.c` & `libesedb-20240420/pyesedb/pyesedb_value_flags.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/pyesedb/pyesedb_table.h` & `libesedb-20240420/pyesedb/pyesedb_table.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/pyesedb/pyesedb_column.h` & `libesedb-20240420/pyesedb/pyesedb_column.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/pyesedb/pyesedb_indexes.h` & `libesedb-20240420/pyesedb/pyesedb_indexes.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/pyesedb/pyesedb_column.c` & `libesedb-20240420/pyesedb/pyesedb_column.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/pyesedb/pyesedb_long_value.c` & `libesedb-20240420/pyesedb/pyesedb_long_value.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/pyesedb/pyesedb_file.c` & `libesedb-20240420/pyesedb/pyesedb_file.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/pyesedb/pyesedb_columns.h` & `libesedb-20240420/pyesedb/pyesedb_columns.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/pyesedb/Makefile.in` & `libesedb-20240420/pyesedb/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -614,16 +614,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_PYTHON_TRUE@AM_CFLAGS = \
-@HAVE_PYTHON_TRUE@	-I$(top_srcdir)/include \
-@HAVE_PYTHON_TRUE@	-I$(top_srcdir)/common \
+@HAVE_PYTHON_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_PYTHON_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_PYTHON_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_PYTHON_TRUE@	@LIBCDATA_CPPFLAGS@ \
 @HAVE_PYTHON_TRUE@	@LIBCLOCALE_CPPFLAGS@ \
 @HAVE_PYTHON_TRUE@	@LIBCSPLIT_CPPFLAGS@ \
 @HAVE_PYTHON_TRUE@	@LIBUNA_CPPFLAGS@ \
 @HAVE_PYTHON_TRUE@	@LIBCFILE_CPPFLAGS@ \
 @HAVE_PYTHON_TRUE@	@LIBCPATH_CPPFLAGS@ \
@@ -667,15 +667,16 @@
 @HAVE_PYTHON_TRUE@	@LIBUNA_LIBADD@ \
 @HAVE_PYTHON_TRUE@	@LIBCFILE_LIBADD@ \
 @HAVE_PYTHON_TRUE@	@LIBCPATH_LIBADD@ \
 @HAVE_PYTHON_TRUE@	@LIBBFIO_LIBADD@
 
 @HAVE_PYTHON_TRUE@pyesedb_la_CPPFLAGS = $(PYTHON_CPPFLAGS)
 @HAVE_PYTHON_TRUE@pyesedb_la_LDFLAGS = -module -avoid-version $(PYTHON_LDFLAGS)
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -1053,24 +1054,45 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-pyexecLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/pyesedb_la-pyesedb.Plo
+	-rm -f ./$(DEPDIR)/pyesedb_la-pyesedb_column.Plo
+	-rm -f ./$(DEPDIR)/pyesedb_la-pyesedb_column_types.Plo
+	-rm -f ./$(DEPDIR)/pyesedb_la-pyesedb_columns.Plo
+	-rm -f ./$(DEPDIR)/pyesedb_la-pyesedb_datetime.Plo
+	-rm -f ./$(DEPDIR)/pyesedb_la-pyesedb_error.Plo
+	-rm -f ./$(DEPDIR)/pyesedb_la-pyesedb_file.Plo
+	-rm -f ./$(DEPDIR)/pyesedb_la-pyesedb_file_object_io_handle.Plo
+	-rm -f ./$(DEPDIR)/pyesedb_la-pyesedb_file_types.Plo
+	-rm -f ./$(DEPDIR)/pyesedb_la-pyesedb_index.Plo
+	-rm -f ./$(DEPDIR)/pyesedb_la-pyesedb_indexes.Plo
+	-rm -f ./$(DEPDIR)/pyesedb_la-pyesedb_integer.Plo
+	-rm -f ./$(DEPDIR)/pyesedb_la-pyesedb_long_value.Plo
+	-rm -f ./$(DEPDIR)/pyesedb_la-pyesedb_multi_value.Plo
+	-rm -f ./$(DEPDIR)/pyesedb_la-pyesedb_record.Plo
+	-rm -f ./$(DEPDIR)/pyesedb_la-pyesedb_records.Plo
+	-rm -f ./$(DEPDIR)/pyesedb_la-pyesedb_table.Plo
+	-rm -f ./$(DEPDIR)/pyesedb_la-pyesedb_tables.Plo
+	-rm -f ./$(DEPDIR)/pyesedb_la-pyesedb_value_flags.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -1173,13 +1195,10 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am uninstall-pyexecLTLIBRARIES
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libesedb-20240202/pyesedb/pyesedb_value_flags.h` & `libesedb-20240420/pyesedb/pyesedb_value_flags.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/pyesedb/pyesedb_file_types.h` & `libesedb-20240420/pyesedb/pyesedb_file_types.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/pyesedb/pyesedb_column_types.c` & `libesedb-20240420/pyesedb/pyesedb_column_types.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/pyesedb/pyesedb_record.h` & `libesedb-20240420/pyesedb/pyesedb_record.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/config.rpath` & `libesedb-20240420/config.rpath`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libcthreads/libcthreads_thread.h` & `libesedb-20240420/libcthreads/libcthreads_thread.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libcthreads/libcthreads_read_write_lock.h` & `libesedb-20240420/libcthreads/libcthreads_read_write_lock.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libcthreads/libcthreads_thread.c` & `libesedb-20240420/libcthreads/libcthreads_thread.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libcthreads/libcthreads_thread_pool.h` & `libesedb-20240420/libcthreads/libcthreads_thread_pool.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libcthreads/libcthreads_support.h` & `libesedb-20240420/libcthreads/libcthreads_support.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libcthreads/libcthreads_lock.h` & `libesedb-20240420/libcthreads/libcthreads_lock.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libcthreads/libcthreads_unused.h` & `libesedb-20240420/libcthreads/libcthreads_unused.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libcthreads/libcthreads_lock.c` & `libesedb-20240420/libcthreads/libcthreads_lock.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libcthreads/libcthreads_condition.h` & `libesedb-20240420/libcthreads/libcthreads_condition.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libcthreads/libcthreads_repeating_thread.h` & `libesedb-20240420/libcthreads/libcthreads_repeating_thread.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libcthreads/Makefile.am` & `libesedb-20240420/libcthreads/Makefile.am`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBCTHREADS
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@PTHREAD_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libcthreads.la
 
 libcthreads_la_SOURCES = \
 	libcthreads_condition.c libcthreads_condition.h \
@@ -22,19 +22,17 @@
 	libcthreads_thread.c libcthreads_thread.h \
 	libcthreads_thread_attributes.c libcthreads_thread_attributes.h \
 	libcthreads_thread_pool.c libcthreads_thread_pool.h \
 	libcthreads_types.h \
 	libcthreads_unused.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcthreads ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcthreads_la_SOURCES)
```

### Comparing `libesedb-20240202/libcthreads/libcthreads_support.c` & `libesedb-20240420/libcthreads/libcthreads_support.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libcthreads/libcthreads_mutex.c` & `libesedb-20240420/libcthreads/libcthreads_mutex.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libcthreads/libcthreads_queue.c` & `libesedb-20240420/libcthreads/libcthreads_queue.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libcthreads/libcthreads_mutex.h` & `libesedb-20240420/libcthreads/libcthreads_mutex.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libcthreads/libcthreads_types.h` & `libesedb-20240420/libcthreads/libcthreads_types.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libcthreads/libcthreads_thread_attributes.h` & `libesedb-20240420/libcthreads/libcthreads_thread_attributes.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libcthreads/libcthreads_condition.c` & `libesedb-20240420/libcthreads/libcthreads_condition.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libcthreads/libcthreads_error.c` & `libesedb-20240420/libcthreads/libcthreads_error.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libcthreads/libcthreads_read_write_lock.c` & `libesedb-20240420/libcthreads/libcthreads_read_write_lock.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libcthreads/libcthreads_libcerror.h` & `libesedb-20240420/libcpath/libcpath_libcerror.h`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libcerror header wrapper
  *
- * Copyright (C) 2012-2024, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -15,16 +15,16 @@
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License
  * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
-#if !defined( _LIBCTHREADS_LIBCERROR_H )
-#define _LIBCTHREADS_LIBCERROR_H
+#if !defined( _LIBCPATH_LIBCERROR_H )
+#define _LIBCPATH_LIBCERROR_H
 
 #include <common.h>
 
 /* Define HAVE_LOCAL_LIBCERROR for local use of libcerror
  */
 #if defined( HAVE_LOCAL_LIBCERROR )
 
@@ -42,9 +42,9 @@
 #define LIBCERROR_DLL_IMPORT
 #endif
 
 #include <libcerror.h>
 
 #endif /* defined( HAVE_LOCAL_LIBCERROR ) */
 
-#endif /* !defined( _LIBCTHREADS_LIBCERROR_H ) */
+#endif /* !defined( _LIBCPATH_LIBCERROR_H ) */
```

### Comparing `libesedb-20240202/libcthreads/libcthreads_definitions.h` & `libesedb-20240420/libcthreads/libcthreads_definitions.h`

 * *Files 2% similar despite different names*

```diff
@@ -31,19 +31,19 @@
 #include <libcthreads/definitions.h>
 
 /* The definitions in <libcthreads/definitions.h> are copied here
  * for local use of libcthreads
  */
 #else
 
-#define LIBCTHREADS_VERSION				20240102
+#define LIBCTHREADS_VERSION				20240413
 
 /* The libcthreads version string
  */
-#define LIBCTHREADS_VERSION_STRING			"20240102"
+#define LIBCTHREADS_VERSION_STRING			"20240413"
 
 /* The comparison function definitions
  */
 enum LIBCTHREADS_COMPARE_DEFINITIONS
 {
 	/* The first value is less than the second value
 	 */
```

### Comparing `libesedb-20240202/libcthreads/libcthreads_thread_pool.c` & `libesedb-20240420/libcthreads/libcthreads_thread_pool.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libcthreads/libcthreads_error.h` & `libesedb-20240420/libcthreads/libcthreads_error.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libcthreads/libcthreads_thread_attributes.c` & `libesedb-20240420/libcthreads/libcthreads_thread_attributes.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libcthreads/libcthreads_extern.h` & `libesedb-20240420/libcthreads/libcthreads_extern.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libcthreads/libcthreads_repeating_thread.c` & `libesedb-20240420/libcthreads/libcthreads_repeating_thread.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libcthreads/Makefile.in` & `libesedb-20240420/libcthreads/Makefile.in`

 * *Files 3% similar despite different names*

```diff
@@ -565,16 +565,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBCTHREADS_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBCTHREADS_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBCTHREADS_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBCTHREADS_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBCTHREADS_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	@PTHREAD_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBCTHREADS_TRUE@noinst_LTLIBRARIES = libcthreads.la
 @HAVE_LOCAL_LIBCTHREADS_TRUE@libcthreads_la_SOURCES = \
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	libcthreads_condition.c libcthreads_condition.h \
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	libcthreads_definitions.h \
@@ -589,15 +589,16 @@
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	libcthreads_support.c libcthreads_support.h \
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	libcthreads_thread.c libcthreads_thread.h \
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	libcthreads_thread_attributes.c libcthreads_thread_attributes.h \
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	libcthreads_thread_pool.c libcthreads_thread_pool.h \
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	libcthreads_types.h \
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	libcthreads_unused.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -807,24 +808,37 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libcthreads_condition.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_error.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_lock.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_mutex.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_queue.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_read_write_lock.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_repeating_thread.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_support.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_thread.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_thread_attributes.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_thread_pool.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -918,17 +932,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcthreads ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcthreads_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libesedb-20240202/libcthreads/libcthreads_queue.h` & `libesedb-20240420/libcthreads/libcthreads_queue.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/test-driver` & `libesedb-20240420/test-driver`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libcpath/libcpath_support.c` & `libesedb-20240420/libcpath/libcpath_support.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libcpath/libcpath_libcerror.h` & `libesedb-20240420/libcsplit/libcsplit_libcerror.h`

 * *Files 3% similar despite different names*

```diff
@@ -15,16 +15,16 @@
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License
  * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
-#if !defined( _LIBCPATH_LIBCERROR_H )
-#define _LIBCPATH_LIBCERROR_H
+#if !defined( _LIBCSPLIT_LIBCERROR_H )
+#define _LIBCSPLIT_LIBCERROR_H
 
 #include <common.h>
 
 /* Define HAVE_LOCAL_LIBCERROR for local use of libcerror
  */
 #if defined( HAVE_LOCAL_LIBCERROR )
 
@@ -42,9 +42,9 @@
 #define LIBCERROR_DLL_IMPORT
 #endif
 
 #include <libcerror.h>
 
 #endif /* defined( HAVE_LOCAL_LIBCERROR ) */
 
-#endif /* !defined( _LIBCPATH_LIBCERROR_H ) */
+#endif /* !defined( _LIBCSPLIT_LIBCERROR_H ) */
```

### Comparing `libesedb-20240202/libcpath/libcpath_definitions.h` & `libesedb-20240420/libcpath/libcpath_definitions.h`

 * *Files 4% similar despite different names*

```diff
@@ -31,19 +31,19 @@
 #include <libcpath/definitions.h>
 
 /* The definitions in <libcpath/definitions.h> are copied here
  * for local use of libcpath
  */
 #else
 
-#define LIBCPATH_VERSION			20240109
+#define LIBCPATH_VERSION			20240414
 
 /* The libcpath version string
  */
-#define LIBCPATH_VERSION_STRING			"20240109"
+#define LIBCPATH_VERSION_STRING			"20240414"
 
 #if defined( WINAPI )
 #define LIBCPATH_SEPARATOR			'\\'
 
 #else
 #define LIBCPATH_SEPARATOR			'/'
```

### Comparing `libesedb-20240202/libcpath/Makefile.am` & `libesedb-20240420/libcpath/Makefile.am`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBCPATH
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCSPLIT_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libcpath.la
 
@@ -19,19 +19,17 @@
 	libcpath_libcsplit.h \
 	libcpath_libuna.h \
 	libcpath_support.c libcpath_support.h \
 	libcpath_system_string.c libcpath_system_string.h \
 	libcpath_unused.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcpath ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcpath_la_SOURCES)
```

### Comparing `libesedb-20240202/libcpath/libcpath_error.c` & `libesedb-20240420/libcpath/libcpath_error.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libcpath/libcpath_extern.h` & `libesedb-20240420/libuna/libuna_extern.h`

 * *Files 12% similar despite different names*

```diff
@@ -15,32 +15,32 @@
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License
  * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
-#if !defined( _LIBCPATH_INTERNAL_EXTERN_H )
-#define _LIBCPATH_INTERNAL_EXTERN_H
+#if !defined( _LIBUNA_INTERNAL_EXTERN_H )
+#define _LIBUNA_INTERNAL_EXTERN_H
 
 #include <common.h>
 
-/* Define HAVE_LOCAL_LIBCPATH for local use of libcpath
+/* Define HAVE_LOCAL_LIBUNA for local use of libuna
  */
-#if !defined( HAVE_LOCAL_LIBCPATH )
+#if !defined( HAVE_LOCAL_LIBUNA )
 
-#include <libcpath/extern.h>
+#include <libuna/extern.h>
 
 #if defined( __CYGWIN__ ) || defined( __MINGW32__ )
-#define LIBCPATH_EXTERN_VARIABLE	extern
+#define LIBUNA_EXTERN_VARIABLE	extern
 #else
-#define LIBCPATH_EXTERN_VARIABLE	LIBCPATH_EXTERN
+#define LIBUNA_EXTERN_VARIABLE	LIBUNA_EXTERN
 #endif
 
 #else
-#define LIBCPATH_EXTERN		/* extern */
-#define LIBCPATH_EXTERN_VARIABLE	extern
+#define LIBUNA_EXTERN		/* extern */
+#define LIBUNA_EXTERN_VARIABLE	extern
 
-#endif /* !defined( HAVE_LOCAL_LIBCPATH ) */
+#endif /* !defined( HAVE_LOCAL_LIBUNA ) */
 
-#endif /* !defined( _LIBCPATH_INTERNAL_EXTERN_H ) */
+#endif /* !defined( _LIBUNA_INTERNAL_EXTERN_H ) */
```

### Comparing `libesedb-20240202/libcpath/libcpath_system_string.h` & `libesedb-20240420/libcpath/libcpath_system_string.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libcpath/libcpath_support.h` & `libesedb-20240420/libcpath/libcpath_support.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libcpath/libcpath_libcsplit.h` & `libesedb-20240420/libcpath/libcpath_libcsplit.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libcpath/libcpath_system_string.c` & `libesedb-20240420/libcpath/libcpath_system_string.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libcpath/libcpath_libclocale.h` & `libesedb-20240420/libcpath/libcpath_libclocale.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libcpath/libcpath_error.h` & `libesedb-20240420/libcpath/libcpath_error.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libcpath/Makefile.in` & `libesedb-20240420/libcpath/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -541,16 +541,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBCPATH_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBCPATH_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBCPATH_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBCPATH_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBCPATH_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBCPATH_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_LOCAL_LIBCPATH_TRUE@	@LIBCLOCALE_CPPFLAGS@ \
 @HAVE_LOCAL_LIBCPATH_TRUE@	@LIBCSPLIT_CPPFLAGS@ \
 @HAVE_LOCAL_LIBCPATH_TRUE@	@LIBUNA_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBCPATH_TRUE@noinst_LTLIBRARIES = libcpath.la
 @HAVE_LOCAL_LIBCPATH_TRUE@libcpath_la_SOURCES = \
@@ -562,15 +562,16 @@
 @HAVE_LOCAL_LIBCPATH_TRUE@	libcpath_libclocale.h \
 @HAVE_LOCAL_LIBCPATH_TRUE@	libcpath_libcsplit.h \
 @HAVE_LOCAL_LIBCPATH_TRUE@	libcpath_libuna.h \
 @HAVE_LOCAL_LIBCPATH_TRUE@	libcpath_support.c libcpath_support.h \
 @HAVE_LOCAL_LIBCPATH_TRUE@	libcpath_system_string.c libcpath_system_string.h \
 @HAVE_LOCAL_LIBCPATH_TRUE@	libcpath_unused.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -773,24 +774,30 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libcpath_error.Plo
+	-rm -f ./$(DEPDIR)/libcpath_path.Plo
+	-rm -f ./$(DEPDIR)/libcpath_support.Plo
+	-rm -f ./$(DEPDIR)/libcpath_system_string.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -877,17 +884,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcpath ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcpath_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libesedb-20240202/libcpath/libcpath_libuna.h` & `libesedb-20240420/libcpath/libcpath_libuna.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libcpath/libcpath_unused.h` & `libesedb-20240420/libcpath/libcpath_unused.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libcpath/libcpath_path.c` & `libesedb-20240420/libcpath/libcpath_path.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libcpath/libcpath_path.h` & `libesedb-20240420/libcpath/libcpath_path.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/ChangeLog` & `libesedb-20240420/ChangeLog`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/manuals/esedbinfo.1` & `libesedb-20240420/manuals/esedbinfo.1`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/manuals/libesedb.3` & `libesedb-20240420/manuals/libesedb.3`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/manuals/Makefile.in` & `libesedb-20240420/manuals/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -521,15 +521,16 @@
 	esedbinfo.1 \
 	libesedb.3
 
 EXTRA_DIST = \
 	esedbinfo.1 \
 	libesedb.3
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
 	@for dep in $?; do \
@@ -722,23 +723,25 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool mostlyclean-am
 
+distclean: distclean-am
+	-rm -f Makefile
 distclean-am: clean-am distclean-generic
 
 dvi: dvi-am
 
 dvi-am:
 
 html: html-am
@@ -820,13 +823,10 @@
 	mostlyclean-libtool pdf pdf-am ps ps-am sources-am \
 	sources-local splint-am splint-local tags-am uninstall \
 	uninstall-am uninstall-man uninstall-man1 uninstall-man3
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libesedb-20240202/tests/esedb_test_space_tree.c` & `libesedb-20240420/tests/esedb_test_space_tree.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/tests/esedb_test_index.c` & `libesedb-20240420/tests/esedb_test_index.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/tests/esedb_test_tools_signal.c` & `libesedb-20240420/tests/esedb_test_tools_signal.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/tests/esedb_test_libesedb.h` & `libesedb-20240420/tests/esedb_test_libesedb.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/tests/esedb_test_data_segment.c` & `libesedb-20240420/tests/esedb_test_data_segment.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/tests/esedb_test_libcerror.h` & `libesedb-20240420/tests/esedb_test_libcerror.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/tests/esedb_test_libuna.h` & `libesedb-20240420/tests/esedb_test_libuna.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/tests/esedb_test_tools_windows_search_compression.c` & `libesedb-20240420/tests/esedb_test_tools_windows_search_compression.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/tests/esedb_test_functions.c` & `libesedb-20240420/tests/esedb_test_functions.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/tests/esedb_test_table.c` & `libesedb-20240420/tests/esedb_test_table.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/tests/esedb_test_compression.c` & `libesedb-20240420/tests/esedb_test_compression.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/tests/esedb_test_file.c` & `libesedb-20240420/tests/esedb_test_file.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/tests/esedb_test_catalog_definition.c` & `libesedb-20240420/tests/esedb_test_catalog_definition.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/tests/pyesedb_test_support.py` & `libesedb-20240420/tests/pyesedb_test_support.py`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/tests/test_tools.sh` & `libesedb-20240420/tests/test_tools.sh`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env bash
 # Tests tools functions and types.
 #
-# Version: 20231007
+# Version: 20240413
 
 EXIT_SUCCESS=0;
 EXIT_FAILURE=1;
 EXIT_IGNORE=77;
 
 TOOLS_TESTS="info_handle output signal windows_search_compression";
 TOOLS_TESTS_WITH_INPUT="";
@@ -137,20 +137,17 @@
 }
 
 if test -n "${SKIP_TOOLS_TESTS}";
 then
 	exit ${EXIT_IGNORE};
 fi
 
-TEST_RUNNER="tests/test_runner.sh";
+TEST_DIRECTORY=`dirname $0`;
 
-if ! test -f "${TEST_RUNNER}";
-then
-	TEST_RUNNER="./test_runner.sh";
-fi
+TEST_RUNNER="${TEST_DIRECTORY}/test_runner.sh";
 
 if ! test -f "${TEST_RUNNER}";
 then
 	echo "Missing test runner: ${TEST_RUNNER}";
 
 	exit ${EXIT_FAILURE};
 fi
```

### Comparing `libesedb-20240202/tests/esedb_test_libbfio.h` & `libesedb-20240420/tests/esedb_test_libbfio.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/tests/esedb_test_libcnotify.h` & `libesedb-20240420/tests/esedb_test_libcnotify.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/tests/esedb_test_checksum.c` & `libesedb-20240420/tests/esedb_test_checksum.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/tests/esedb_test_table_definition.c` & `libesedb-20240420/tests/esedb_test_table_definition.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/tests/esedb_test_error.c` & `libesedb-20240420/tests/esedb_test_error.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/tests/esedb_test_multi_value.c` & `libesedb-20240420/tests/esedb_test_multi_value.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/tests/pyesedb_test_file.py` & `libesedb-20240420/tests/pyesedb_test_file.py`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/tests/esedb_test_space_tree_value.c` & `libesedb-20240420/tests/esedb_test_space_tree_value.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/tests/Makefile.am` & `libesedb-20240420/tests/Makefile.am`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 AUTOMAKE_OPTIONS = subdir-objects
 
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBCSPLIT_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ \
 	@LIBCFILE_CPPFLAGS@ \
@@ -613,13 +613,12 @@
 	esedb_test_tools_windows_search_compression.c \
 	esedb_test_unused.h
 
 esedb_test_tools_windows_search_compression_LDADD = \
 	@LIBCNOTIFY_LIBADD@ \
 	@LIBCERROR_LIBADD@
 
-MAINTAINERCLEANFILES = \
-	Makefile.in
-
-distclean: clean
-	-rm -f Makefile
+DISTCLEANFILES = \
+	Makefile \
+	Makefile.in \
+	notify_stream.log
```

### Comparing `libesedb-20240202/tests/esedb_test_memory.h` & `libesedb-20240420/tests/esedb_test_memory.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/tests/esedb_test_libclocale.h` & `libesedb-20240420/tests/esedb_test_libclocale.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/tests/esedb_test_record.c` & `libesedb-20240420/tests/esedb_test_record.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/tests/esedb_test_support.c` & `libesedb-20240420/tests/esedb_test_support.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/tests/esedb_test_notify.c` & `libesedb-20240420/tests/esedb_test_notify.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/tests/esedb_test_leaf_page_descriptor.c` & `libesedb-20240420/tests/esedb_test_leaf_page_descriptor.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/tests/esedb_test_tools_info_handle.c` & `libesedb-20240420/tests/esedb_test_tools_info_handle.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/tests/test_python_module.sh` & `libesedb-20240420/tests/test_python_module.sh`

 * *Files 8% similar despite different names*

```diff
@@ -1,43 +1,46 @@
 #!/usr/bin/env bash
 # Tests Python module functions and types.
 #
-# Version: 20240120
+# Version: 20240417
 
 EXIT_SUCCESS=0;
 EXIT_FAILURE=1;
 EXIT_NO_TESTS_RAN=5;
 EXIT_IGNORE=77;
 
 TEST_FUNCTIONS="support";
 TEST_FUNCTIONS_WITH_INPUT="file";
 OPTION_SETS=();
 
 TEST_TOOL_DIRECTORY=".";
 INPUT_GLOB="*";
 
+LIBRARY_NAME="libesedb";
+PYTHON_MODULE="pyesedb";
+
 test_python_function()
 {
 	local TEST_FUNCTION=$1;
 
 	local TEST_DESCRIPTION="Testing Python-bindings functions: ${TEST_FUNCTION}";
-	local TEST_SCRIPT="${TEST_TOOL_DIRECTORY}/pyesedb_test_${TEST_FUNCTION}.py";
+	local TEST_SCRIPT="${TEST_TOOL_DIRECTORY}/${PYTHON_MODULE}_test_${TEST_FUNCTION}.py";
 
 	run_test_with_arguments "${TEST_DESCRIPTION}" "${TEST_SCRIPT}";
 	local RESULT=$?;
 
 	return ${RESULT};
 }
 
 test_python_function_with_input()
 {
 	local TEST_FUNCTION=$1;
 
 	local TEST_DESCRIPTION="Testing Python-bindings functions: ${TEST_FUNCTION}";
-	local TEST_SCRIPT="${TEST_TOOL_DIRECTORY}/pyesedb_test_${TEST_FUNCTION}.py";
+	local TEST_SCRIPT="${TEST_TOOL_DIRECTORY}/${PYTHON_MODULE}_test_${TEST_FUNCTION}.py";
 
 	if ! test -d "input";
 	then
 		echo "Test input directory not found.";
 
 		return ${EXIT_IGNORE};
 	fi
@@ -46,15 +49,15 @@
 	if test ${RESULT} -eq ${EXIT_SUCCESS};
 	then
 		echo "No files or directories found in the test input directory";
 
 		return ${EXIT_IGNORE};
 	fi
 
-	local TEST_PROFILE_DIRECTORY=$(get_test_profile_directory "input" "pyesedb");
+	local TEST_PROFILE_DIRECTORY=$(get_test_profile_directory "input" "${PYTHON_MODULE}");
 
 	local IGNORE_LIST=$(read_ignore_list "${TEST_PROFILE_DIRECTORY}");
 
 	RESULT=${EXIT_SUCCESS};
 
 	for TEST_SET_INPUT_DIRECTORY in input/*;
 	do
@@ -121,30 +124,35 @@
 }
 
 if test -n "${SKIP_PYTHON_TESTS}";
 then
 	exit ${EXIT_IGNORE};
 fi
 
-TEST_RUNNER="tests/test_runner.sh";
+TEST_DIRECTORY=`dirname $0`;
 
-if ! test -f "${TEST_RUNNER}";
-then
-	TEST_RUNNER="./test_runner.sh";
-fi
+TEST_RUNNER="${TEST_DIRECTORY}/test_runner.sh";
 
 if ! test -f "${TEST_RUNNER}";
 then
 	echo "Missing test runner: ${TEST_RUNNER}";
 
 	exit ${EXIT_FAILURE};
 fi
 
 source ${TEST_RUNNER};
 
+PLATFORM=`uname -s | sed 's/-.*$//'`;
+
+if test "${PLATFORM}" = "MINGW64_NT" || test "${PLATFORM}" = "MSYS_NT";
+then
+	cp ../${LIBRARY_NAME}/.libs/*.dll ../${PYTHON_MODULE}/.libs/;
+	cp ../${PYTHON_MODULE}/.libs/${PYTHON_MODULE}.dll ../${PYTHON_MODULE}/.libs/${PYTHON_MODULE}.pyd;
+fi
+
 RESULT=${EXIT_IGNORE};
 
 for TEST_FUNCTION in ${TEST_FUNCTIONS};
 do
 	test_python_function "${TEST_FUNCTION}";
 	RESULT=$?;
```

### Comparing `libesedb-20240202/tests/esedb_test_catalog.c` & `libesedb-20240420/tests/esedb_test_catalog.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/tests/esedb_test_libcdata.h` & `libesedb-20240420/tests/esedb_test_libcdata.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/tests/esedb_test_memory.c` & `libesedb-20240420/tests/esedb_test_memory.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/tests/test_esedbexport.sh` & `libesedb-20240420/tests/test_esedbexport.sh`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env bash
 # Export tool testing script
 #
-# Version: 20231005
+# Version: 20240413
 
 EXIT_SUCCESS=0;
 EXIT_FAILURE=1;
 EXIT_IGNORE=77;
 
 PROFILES=("esedbexport");
 OPTIONS_PER_PROFILE=("");
@@ -71,20 +71,17 @@
 if ! test -x "${TEST_EXECUTABLE}";
 then
 	echo "Missing test executable: ${TEST_EXECUTABLE}";
 
 	exit ${EXIT_FAILURE};
 fi
 
-TEST_RUNNER="tests/test_runner.sh";
+TEST_DIRECTORY=`dirname $0`;
 
-if ! test -f "${TEST_RUNNER}";
-then
-	TEST_RUNNER="./test_runner.sh";
-fi
+TEST_RUNNER="${TEST_DIRECTORY}/test_runner.sh";
 
 if ! test -f "${TEST_RUNNER}";
 then
 	echo "Missing test runner: ${TEST_RUNNER}";
 
 	exit ${EXIT_FAILURE};
 fi
```

### Comparing `libesedb-20240202/tests/test_esedbinfo.sh` & `libesedb-20240420/tests/test_esedbinfo.sh`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env bash
 # Info tool testing script
 #
-# Version: 20231005
+# Version: 20240413
 
 EXIT_SUCCESS=0;
 EXIT_FAILURE=1;
 EXIT_IGNORE=77;
 
 PROFILES=("esedbinfo");
 OPTIONS_PER_PROFILE=("");
@@ -28,20 +28,17 @@
 if ! test -x "${TEST_EXECUTABLE}";
 then
 	echo "Missing test executable: ${TEST_EXECUTABLE}";
 
 	exit ${EXIT_FAILURE};
 fi
 
-TEST_RUNNER="tests/test_runner.sh";
+TEST_DIRECTORY=`dirname $0`;
 
-if ! test -f "${TEST_RUNNER}";
-then
-	TEST_RUNNER="./test_runner.sh";
-fi
+TEST_RUNNER="${TEST_DIRECTORY}/test_runner.sh";
 
 if ! test -f "${TEST_RUNNER}";
 then
 	echo "Missing test runner: ${TEST_RUNNER}";
 
 	exit ${EXIT_FAILURE};
 fi
```

### Comparing `libesedb-20240202/tests/esedb_test_tools_output.c` & `libesedb-20240420/tests/esedb_test_tools_output.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/tests/esedb_test_column_type.c` & `libesedb-20240420/tests/esedb_test_column_type.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/tests/esedb_test_block_tree_node.c` & `libesedb-20240420/tests/esedb_test_block_tree_node.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/tests/test_runner.sh` & `libesedb-20240420/tests/test_runner.sh`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/tests/esedb_test_unused.h` & `libesedb-20240420/tests/esedb_test_unused.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/tests/esedb_test_database.c` & `libesedb-20240420/tests/esedb_test_database.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/tests/esedb_test_io_handle.c` & `libesedb-20240420/tests/esedb_test_io_handle.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/tests/esedb_test_file_header.c` & `libesedb-20240420/tests/esedb_test_file_header.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/tests/esedb_test_page_tree_value.c` & `libesedb-20240420/tests/esedb_test_page_tree_value.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/tests/esedb_test_getopt.c` & `libesedb-20240420/tests/esedb_test_getopt.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/tests/esedb_test_getopt.h` & `libesedb-20240420/tests/esedb_test_getopt.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/tests/esedb_test_functions.h` & `libesedb-20240420/tests/esedb_test_functions.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/tests/esedb_test_block_tree.c` & `libesedb-20240420/tests/esedb_test_block_tree.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/tests/esedb_test_libfcache.h` & `libesedb-20240420/tests/esedb_test_libfcache.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/tests/esedb_test_libfdata.h` & `libesedb-20240420/tests/esedb_test_libfdata.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/tests/esedb_test_data_definition.c` & `libesedb-20240420/tests/esedb_test_data_definition.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/tests/Makefile.in` & `libesedb-20240420/tests/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -1043,16 +1043,16 @@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 AUTOMAKE_OPTIONS = subdir-objects
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBCSPLIT_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ \
 	@LIBCFILE_CPPFLAGS@ \
@@ -1617,16 +1617,18 @@
 	esedb_test_tools_windows_search_compression.c \
 	esedb_test_unused.h
 
 esedb_test_tools_windows_search_compression_LDADD = \
 	@LIBCNOTIFY_LIBADD@ \
 	@LIBCERROR_LIBADD@
 
-MAINTAINERCLEANFILES = \
-	Makefile.in
+DISTCLEANFILES = \
+	Makefile \
+	Makefile.in \
+	notify_stream.log
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .log .o .obj .test .test$(EXEEXT) .trs
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
 	@for dep in $?; do \
@@ -2235,24 +2237,71 @@
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
 	-rm -f ../esedbtools/$(DEPDIR)/$(am__dirstamp)
 	-rm -f ../esedbtools/$(am__dirstamp)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-checkPROGRAMS clean-generic clean-libtool \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ../esedbtools/$(DEPDIR)/esedbtools_output.Po
+	-rm -f ../esedbtools/$(DEPDIR)/esedbtools_signal.Po
+	-rm -f ../esedbtools/$(DEPDIR)/info_handle.Po
+	-rm -f ../esedbtools/$(DEPDIR)/windows_search_compression.Po
+	-rm -f ./$(DEPDIR)/esedb_test_block_descriptor.Po
+	-rm -f ./$(DEPDIR)/esedb_test_block_tree.Po
+	-rm -f ./$(DEPDIR)/esedb_test_block_tree_node.Po
+	-rm -f ./$(DEPDIR)/esedb_test_catalog.Po
+	-rm -f ./$(DEPDIR)/esedb_test_catalog_definition.Po
+	-rm -f ./$(DEPDIR)/esedb_test_checksum.Po
+	-rm -f ./$(DEPDIR)/esedb_test_column.Po
+	-rm -f ./$(DEPDIR)/esedb_test_column_type.Po
+	-rm -f ./$(DEPDIR)/esedb_test_compression.Po
+	-rm -f ./$(DEPDIR)/esedb_test_data_definition.Po
+	-rm -f ./$(DEPDIR)/esedb_test_data_segment.Po
+	-rm -f ./$(DEPDIR)/esedb_test_database.Po
+	-rm -f ./$(DEPDIR)/esedb_test_error.Po
+	-rm -f ./$(DEPDIR)/esedb_test_file.Po
+	-rm -f ./$(DEPDIR)/esedb_test_file_header.Po
+	-rm -f ./$(DEPDIR)/esedb_test_functions.Po
+	-rm -f ./$(DEPDIR)/esedb_test_getopt.Po
+	-rm -f ./$(DEPDIR)/esedb_test_index.Po
+	-rm -f ./$(DEPDIR)/esedb_test_io_handle.Po
+	-rm -f ./$(DEPDIR)/esedb_test_leaf_page_descriptor.Po
+	-rm -f ./$(DEPDIR)/esedb_test_long_value.Po
+	-rm -f ./$(DEPDIR)/esedb_test_memory.Po
+	-rm -f ./$(DEPDIR)/esedb_test_multi_value.Po
+	-rm -f ./$(DEPDIR)/esedb_test_notify.Po
+	-rm -f ./$(DEPDIR)/esedb_test_page.Po
+	-rm -f ./$(DEPDIR)/esedb_test_page_header.Po
+	-rm -f ./$(DEPDIR)/esedb_test_page_tree.Po
+	-rm -f ./$(DEPDIR)/esedb_test_page_tree_key.Po
+	-rm -f ./$(DEPDIR)/esedb_test_page_tree_value.Po
+	-rm -f ./$(DEPDIR)/esedb_test_page_value.Po
+	-rm -f ./$(DEPDIR)/esedb_test_record.Po
+	-rm -f ./$(DEPDIR)/esedb_test_root_page_header.Po
+	-rm -f ./$(DEPDIR)/esedb_test_space_tree.Po
+	-rm -f ./$(DEPDIR)/esedb_test_space_tree_value.Po
+	-rm -f ./$(DEPDIR)/esedb_test_support.Po
+	-rm -f ./$(DEPDIR)/esedb_test_table.Po
+	-rm -f ./$(DEPDIR)/esedb_test_table_definition.Po
+	-rm -f ./$(DEPDIR)/esedb_test_tools_info_handle.Po
+	-rm -f ./$(DEPDIR)/esedb_test_tools_output.Po
+	-rm -f ./$(DEPDIR)/esedb_test_tools_signal.Po
+	-rm -f ./$(DEPDIR)/esedb_test_tools_windows_search_compression.Po
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -2380,13 +2429,10 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	recheck sources-am sources-local splint-am splint-local tags \
 	tags-am uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libesedb-20240202/tests/esedb_test_root_page_header.c` & `libesedb-20240420/tests/esedb_test_root_page_header.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/tests/esedb_test_long_value.c` & `libesedb-20240420/tests/esedb_test_long_value.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/tests/esedb_test_page_value.c` & `libesedb-20240420/tests/esedb_test_page_value.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/tests/esedb_test_page_tree_key.c` & `libesedb-20240420/tests/esedb_test_page_tree_key.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/tests/esedb_test_block_descriptor.c` & `libesedb-20240420/tests/esedb_test_block_descriptor.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/tests/esedb_test_page_tree.c` & `libesedb-20240420/tests/esedb_test_page_tree.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/tests/esedb_test_page.c` & `libesedb-20240420/tests/esedb_test_page.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/tests/esedb_test_page_header.c` & `libesedb-20240420/tests/esedb_test_page_header.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/tests/esedb_test_column.c` & `libesedb-20240420/tests/esedb_test_column.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/tests/test_library.sh` & `libesedb-20240420/tests/test_library.sh`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env bash
 # Tests library functions and types.
 #
-# Version: 20231007
+# Version: 20240413
 
 EXIT_SUCCESS=0;
 EXIT_FAILURE=1;
 EXIT_IGNORE=77;
 
 LIBRARY_TESTS="block_descriptor block_tree block_tree_node catalog catalog_definition checksum column column_type compression data_definition data_segment database error file_header index io_handle leaf_page_descriptor long_value multi_value notify page page_header page_tree page_tree_key page_tree_value page_value record table root_page_header space_tree space_tree_value table_definition";
 LIBRARY_TESTS_WITH_INPUT="file support";
@@ -137,20 +137,17 @@
 }
 
 if test -n "${SKIP_LIBRARY_TESTS}";
 then
 	exit ${EXIT_IGNORE};
 fi
 
-TEST_RUNNER="tests/test_runner.sh";
+TEST_DIRECTORY=`dirname $0`;
 
-if ! test -f "${TEST_RUNNER}";
-then
-	TEST_RUNNER="./test_runner.sh";
-fi
+TEST_RUNNER="${TEST_DIRECTORY}/test_runner.sh";
 
 if ! test -f "${TEST_RUNNER}";
 then
 	echo "Missing test runner: ${TEST_RUNNER}";
 
 	exit ${EXIT_FAILURE};
 fi
```

### Comparing `libesedb-20240202/tests/esedb_test_macros.h` & `libesedb-20240420/tests/esedb_test_macros.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/ossfuzz/table_fuzzer.cc` & `libesedb-20240420/ossfuzz/table_fuzzer.cc`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/ossfuzz/ossfuzz_libesedb.h` & `libesedb-20240420/ossfuzz/ossfuzz_libesedb.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/ossfuzz/Makefile.am` & `libesedb-20240420/ossfuzz/Makefile.am`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LIB_FUZZING_ENGINE
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ \
 	@LIBCFILE_CPPFLAGS@ \
 	@LIBCPATH_CPPFLAGS@ \
@@ -86,20 +86,18 @@
 	../libesedb/libesedb.la \
 	@LIBCNOTIFY_LIBADD@ \
 	@LIBCLOCALE_LIBADD@ \
 	@LIBCERROR_LIBADD@ \
 	@LIBINTL@
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 splint-local:
 	@echo "Running splint on column_fuzzer ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(column_fuzzer_SOURCES)
 	@echo "Running splint on file_fuzzer ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(file_fuzzer_SOURCES)
 	@echo "Running splint on record_fuzzer ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(record_fuzzer_SOURCES)
```

### Comparing `libesedb-20240202/ossfuzz/column_fuzzer.cc` & `libesedb-20240420/ossfuzz/column_fuzzer.cc`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/ossfuzz/ossfuzz_libbfio.h` & `libesedb-20240420/ossfuzz/ossfuzz_libbfio.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/ossfuzz/record_fuzzer.cc` & `libesedb-20240420/ossfuzz/record_fuzzer.cc`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/ossfuzz/file_fuzzer.cc` & `libesedb-20240420/ossfuzz/file_fuzzer.cc`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/ossfuzz/Makefile.in` & `libesedb-20240420/ossfuzz/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -584,16 +584,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LIB_FUZZING_ENGINE_TRUE@AM_CPPFLAGS = \
-@HAVE_LIB_FUZZING_ENGINE_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LIB_FUZZING_ENGINE_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LIB_FUZZING_ENGINE_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LIB_FUZZING_ENGINE_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBCDATA_CPPFLAGS@ \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBCLOCALE_CPPFLAGS@ \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBCNOTIFY_CPPFLAGS@ \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBUNA_CPPFLAGS@ \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBCFILE_CPPFLAGS@ \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBCPATH_CPPFLAGS@ \
@@ -667,15 +667,16 @@
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBCDATA_LIBADD@ \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	../libesedb/libesedb.la \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBCNOTIFY_LIBADD@ \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBCLOCALE_LIBADD@ \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBCERROR_LIBADD@ \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBINTL@
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .cc .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -932,23 +933,29 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-binPROGRAMS clean-generic clean-libtool mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/column_fuzzer.Po
+	-rm -f ./$(DEPDIR)/file_fuzzer.Po
+	-rm -f ./$(DEPDIR)/record_fuzzer.Po
+	-rm -f ./$(DEPDIR)/table_fuzzer.Po
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -1035,17 +1042,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am uninstall-binPROGRAMS
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 splint-local:
 	@echo "Running splint on column_fuzzer ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(column_fuzzer_SOURCES)
 	@echo "Running splint on file_fuzzer ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(file_fuzzer_SOURCES)
 	@echo "Running splint on record_fuzzer ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(record_fuzzer_SOURCES)
```

### Comparing `libesedb-20240202/ltmain.sh` & `libesedb-20240420/ltmain.sh`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfwnt/libfwnt_locale_identifier.h` & `libesedb-20240420/libfwnt/libfwnt_locale_identifier.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfwnt/libfwnt_lzxpress.c` & `libesedb-20240420/libfwnt/libfwnt_lzxpress.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfwnt/libfwnt_extern.h` & `libesedb-20240420/libfwnt/libfwnt_extern.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfwnt/libfwnt_security_identifier.c` & `libesedb-20240420/libfwnt/libfwnt_security_identifier.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfwnt/libfwnt_libcerror.h` & `libesedb-20240420/libfwnt/libfwnt_libcerror.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfwnt/libfwnt_bit_stream.c` & `libesedb-20240420/libfwnt/libfwnt_bit_stream.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfwnt/libfwnt_error.h` & `libesedb-20240420/libfwnt/libfwnt_error.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfwnt/libfwnt_lznt1.h` & `libesedb-20240420/libfwnt/libfwnt_lznt1.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfwnt/libfwnt_notify.c` & `libesedb-20240420/libfwnt/libfwnt_notify.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfwnt/Makefile.am` & `libesedb-20240420/libfwnt/Makefile.am`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBFWNT
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCTHREADS_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@PTHREAD_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libfwnt.la
@@ -30,19 +30,17 @@
 	libfwnt_security_descriptor.c libfwnt_security_descriptor.h \
 	libfwnt_security_identifier.c libfwnt_security_identifier.h \
 	libfwnt_support.c libfwnt_support.h \
 	libfwnt_types.h \
 	libfwnt_unused.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libfwnt ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfwnt_la_SOURCES)
```

### Comparing `libesedb-20240202/libfwnt/libfwnt_security_identifier.h` & `libesedb-20240420/libfwnt/libfwnt_security_identifier.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfwnt/libfwnt_support.h` & `libesedb-20240420/libfwnt/libfwnt_support.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfwnt/libfwnt_huffman_tree.h` & `libesedb-20240420/libfwnt/libfwnt_huffman_tree.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfwnt/libfwnt_error.c` & `libesedb-20240420/libfwnt/libfwnt_error.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfwnt/libfwnt_access_control_list.h` & `libesedb-20240420/libfwnt/libfwnt_access_control_list.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfwnt/libfwnt_security_descriptor.c` & `libesedb-20240420/libfwnt/libfwnt_security_descriptor.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfwnt/libfwnt_access_control_list.c` & `libesedb-20240420/libfwnt/libfwnt_access_control_list.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfwnt/libfwnt_definitions.h` & `libesedb-20240420/libfwnt/libfwnt_definitions.h`

 * *Files 1% similar despite different names*

```diff
@@ -32,19 +32,19 @@
 
 /* The definitions in <libfwnt/definitions.h> are copied here
  * for local use of libfwnt
  */
 #else
 #include <byte_stream.h>
 
-#define LIBFWNT_VERSION					20240126
+#define LIBFWNT_VERSION					20240415
 
 /* The version string
  */
-#define LIBFWNT_VERSION_STRING				"20240126"
+#define LIBFWNT_VERSION_STRING				"20240415"
 
 
 /* The endian definitions
  */
 #define LIBFWNT_ENDIAN_BIG				_BYTE_STREAM_ENDIAN_BIG
 #define LIBFWNT_ENDIAN_LITTLE				_BYTE_STREAM_ENDIAN_LITTLE
```

### Comparing `libesedb-20240202/libfwnt/libfwnt_huffman_tree.c` & `libesedb-20240420/libfwnt/libfwnt_huffman_tree.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfwnt/libfwnt_debug.c` & `libesedb-20240420/libfwnt/libfwnt_debug.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfwnt/libfwnt_lznt1.c` & `libesedb-20240420/libfwnt/libfwnt_lznt1.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfwnt/libfwnt_notify.h` & `libesedb-20240420/libfwnt/libfwnt_notify.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfwnt/libfwnt_locale_identifier.c` & `libesedb-20240420/libfwnt/libfwnt_locale_identifier.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfwnt/libfwnt_debug.h` & `libesedb-20240420/libfwnt/libfwnt_debug.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfwnt/libfwnt_libcdata.h` & `libesedb-20240420/libfwnt/libfwnt_libcdata.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfwnt/libfwnt_lzx.h` & `libesedb-20240420/libfwnt/libfwnt_lzx.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfwnt/libfwnt_unused.h` & `libesedb-20240420/libfwnt/libfwnt_unused.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfwnt/libfwnt_libcnotify.h` & `libesedb-20240420/libfwnt/libfwnt_libcnotify.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfwnt/libfwnt_access_control_entry.c` & `libesedb-20240420/libfwnt/libfwnt_access_control_entry.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfwnt/libfwnt_lzxpress.h` & `libesedb-20240420/libfwnt/libfwnt_lzxpress.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfwnt/libfwnt_security_descriptor.h` & `libesedb-20240420/libfwnt/libfwnt_security_descriptor.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfwnt/libfwnt_lzx.c` & `libesedb-20240420/libfwnt/libfwnt_lzx.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfwnt/Makefile.in` & `libesedb-20240420/libfwnt/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -567,16 +567,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBFWNT_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBFWNT_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBFWNT_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBFWNT_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBFWNT_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBFWNT_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFWNT_TRUE@	@LIBCTHREADS_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFWNT_TRUE@	@LIBCDATA_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFWNT_TRUE@	@LIBCNOTIFY_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFWNT_TRUE@	@PTHREAD_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBFWNT_TRUE@noinst_LTLIBRARIES = libfwnt.la
@@ -599,15 +599,16 @@
 @HAVE_LOCAL_LIBFWNT_TRUE@	libfwnt_notify.c libfwnt_notify.h \
 @HAVE_LOCAL_LIBFWNT_TRUE@	libfwnt_security_descriptor.c libfwnt_security_descriptor.h \
 @HAVE_LOCAL_LIBFWNT_TRUE@	libfwnt_security_identifier.c libfwnt_security_identifier.h \
 @HAVE_LOCAL_LIBFWNT_TRUE@	libfwnt_support.c libfwnt_support.h \
 @HAVE_LOCAL_LIBFWNT_TRUE@	libfwnt_types.h \
 @HAVE_LOCAL_LIBFWNT_TRUE@	libfwnt_unused.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -820,24 +821,40 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libfwnt_access_control_entry.Plo
+	-rm -f ./$(DEPDIR)/libfwnt_access_control_list.Plo
+	-rm -f ./$(DEPDIR)/libfwnt_bit_stream.Plo
+	-rm -f ./$(DEPDIR)/libfwnt_debug.Plo
+	-rm -f ./$(DEPDIR)/libfwnt_error.Plo
+	-rm -f ./$(DEPDIR)/libfwnt_huffman_tree.Plo
+	-rm -f ./$(DEPDIR)/libfwnt_locale_identifier.Plo
+	-rm -f ./$(DEPDIR)/libfwnt_lznt1.Plo
+	-rm -f ./$(DEPDIR)/libfwnt_lzx.Plo
+	-rm -f ./$(DEPDIR)/libfwnt_lzxpress.Plo
+	-rm -f ./$(DEPDIR)/libfwnt_notify.Plo
+	-rm -f ./$(DEPDIR)/libfwnt_security_descriptor.Plo
+	-rm -f ./$(DEPDIR)/libfwnt_security_identifier.Plo
+	-rm -f ./$(DEPDIR)/libfwnt_support.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -934,17 +951,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libfwnt ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfwnt_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libesedb-20240202/libfwnt/libfwnt_bit_stream.h` & `libesedb-20240420/libfwnt/libfwnt_bit_stream.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfwnt/libfwnt_types.h` & `libesedb-20240420/libfwnt/libfwnt_types.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfwnt/libfwnt_support.c` & `libesedb-20240420/libfwnt/libfwnt_support.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfwnt/libfwnt_access_control_entry.h` & `libesedb-20240420/libfwnt/libfwnt_access_control_entry.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libcsplit/libcsplit_narrow_string.c` & `libesedb-20240420/libcsplit/libcsplit_narrow_string.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libcsplit/libcsplit_definitions.h` & `libesedb-20240420/libcsplit/libcsplit_definitions.h`

 * *Files 5% similar despite different names*

```diff
@@ -31,17 +31,17 @@
 #include <libcsplit/definitions.h>
 
 /* The definitions in <libcsplit/definitions.h> are copied here
  * for local use of libcsplit
  */
 #else
 
-#define LIBCSPLIT_VERSION			20240110
+#define LIBCSPLIT_VERSION			20240414
 
 /* The libcsplit version string
  */
-#define LIBCSPLIT_VERSION_STRING		"20240110"
+#define LIBCSPLIT_VERSION_STRING		"20240414"
 
 #endif /* !defined( HAVE_LOCAL_LIBCSPLIT ) */
 
 #endif
```

### Comparing `libesedb-20240202/libcsplit/libcsplit_types.h` & `libesedb-20240420/libcsplit/libcsplit_types.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libcsplit/libcsplit_wide_split_string.c` & `libesedb-20240420/libcsplit/libcsplit_wide_split_string.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libcsplit/libcsplit_support.h` & `libesedb-20240420/libcsplit/libcsplit_support.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libcsplit/Makefile.am` & `libesedb-20240420/libcsplit/Makefile.am`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBCSPLIT
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libcsplit.la
 
 libcsplit_la_SOURCES = \
 	libcsplit_definitions.h \
 	libcsplit_error.c libcsplit_error.h \
@@ -16,19 +16,17 @@
 	libcsplit_support.c libcsplit_support.h \
 	libcsplit_types.h \
 	libcsplit_unused.h \
 	libcsplit_wide_split_string.c libcsplit_wide_split_string.h \
 	libcsplit_wide_string.c libcsplit_wide_string.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcsplit ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcsplit_la_SOURCES)
```

### Comparing `libesedb-20240202/libcsplit/libcsplit_libcerror.h` & `libesedb-20240420/libuna/libuna_libcerror.h`

 * *Files 4% similar despite different names*

```diff
@@ -15,16 +15,16 @@
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License
  * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
-#if !defined( _LIBCSPLIT_LIBCERROR_H )
-#define _LIBCSPLIT_LIBCERROR_H
+#if !defined( _LIBUNA_LIBCERROR_H )
+#define _LIBUNA_LIBCERROR_H
 
 #include <common.h>
 
 /* Define HAVE_LOCAL_LIBCERROR for local use of libcerror
  */
 #if defined( HAVE_LOCAL_LIBCERROR )
 
@@ -42,9 +42,9 @@
 #define LIBCERROR_DLL_IMPORT
 #endif
 
 #include <libcerror.h>
 
 #endif /* defined( HAVE_LOCAL_LIBCERROR ) */
 
-#endif /* !defined( _LIBCSPLIT_LIBCERROR_H ) */
+#endif /* !defined( _LIBUNA_LIBCERROR_H ) */
```

### Comparing `libesedb-20240202/libcsplit/libcsplit_wide_string.c` & `libesedb-20240420/libcsplit/libcsplit_wide_string.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libcsplit/libcsplit_unused.h` & `libesedb-20240420/libcsplit/libcsplit_unused.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libcsplit/libcsplit_wide_split_string.h` & `libesedb-20240420/libcsplit/libcsplit_wide_split_string.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libcsplit/libcsplit_error.c` & `libesedb-20240420/libuna/libuna_error.c`

 * *Files 10% similar despite different names*

```diff
@@ -19,33 +19,33 @@
  * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
 #include <common.h>
 #include <file_stream.h>
 #include <types.h>
 
-#include "libcsplit_error.h"
-#include "libcsplit_libcerror.h"
+#include "libuna_error.h"
+#include "libuna_libcerror.h"
 
-#if !defined( HAVE_LOCAL_LIBCSPLIT )
+#if !defined( HAVE_LOCAL_LIBUNA )
 
 /* Free an error and its elements
  */
-void libcsplit_error_free(
-      libcsplit_error_t **error )
+void libuna_error_free(
+      libuna_error_t **error )
 {
 	libcerror_error_free(
 	 (libcerror_error_t **) error );
 }
 
 /* Prints a descriptive string of the error to the stream
  * Returns the number of printed characters if successful or -1 on error
  */
-int libcsplit_error_fprint(
-     libcsplit_error_t *error,
+int libuna_error_fprint(
+     libuna_error_t *error,
      FILE *stream )
 {
 	int print_count = 0;
 
 	print_count = libcerror_error_fprint(
 	               (libcerror_error_t *) error,
 	               stream );
@@ -53,16 +53,16 @@
 	return( print_count );
 }
 
 /* Prints a descriptive string of the error to the string
  * The end-of-string character is not included in the return value
  * Returns the number of printed characters if successful or -1 on error
  */
-int libcsplit_error_sprint(
-     libcsplit_error_t *error,
+int libuna_error_sprint(
+     libuna_error_t *error,
      char *string,
      size_t size )
 {
 	int print_count = 0;
 
 	print_count = libcerror_error_sprint(
 	               (libcerror_error_t *) error,
@@ -71,16 +71,16 @@
 
 	return( print_count );
 }
 
 /* Prints a backtrace of the error to the stream
  * Returns the number of printed characters if successful or -1 on error
  */
-int libcsplit_error_backtrace_fprint(
-     libcsplit_error_t *error,
+int libuna_error_backtrace_fprint(
+     libuna_error_t *error,
       FILE *stream )
 {
 	int print_count = 0;
 
 	print_count = libcerror_error_backtrace_fprint(
 	               (libcerror_error_t *) error,
 	               stream );
@@ -88,24 +88,24 @@
 	return( print_count );
 }
 
 /* Prints a backtrace of the error to the string
  * The end-of-string character is not included in the return value
  * Returns the number of printed characters if successful or -1 on error
  */
-int libcsplit_error_backtrace_sprint(
-     libcsplit_error_t *error,
+int libuna_error_backtrace_sprint(
+     libuna_error_t *error,
      char *string,
      size_t size )
 {
 	int print_count = 0;
 
 	print_count = libcerror_error_backtrace_sprint(
 	               (libcerror_error_t *) error,
 	               string,
 	               size );
 
 	return( print_count );
 }
 
-#endif /* !defined( HAVE_LOCAL_LIBCSPLIT ) */
+#endif /* !defined( HAVE_LOCAL_LIBUNA ) */
```

### Comparing `libesedb-20240202/libcsplit/libcsplit_narrow_split_string.c` & `libesedb-20240420/libcsplit/libcsplit_narrow_split_string.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libcsplit/libcsplit_extern.h` & `libesedb-20240420/libcsplit/libcsplit_extern.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libcsplit/libcsplit_error.h` & `libesedb-20240420/libcsplit/libcsplit_error.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libcsplit/libcsplit_support.c` & `libesedb-20240420/libcsplit/libcsplit_support.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libcsplit/libcsplit_wide_string.h` & `libesedb-20240420/libcsplit/libcsplit_wide_string.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libcsplit/Makefile.in` & `libesedb-20240420/libcsplit/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -551,16 +551,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBCSPLIT_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBCSPLIT_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBCSPLIT_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBCSPLIT_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBCSPLIT_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBCSPLIT_TRUE@	@LIBCERROR_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBCSPLIT_TRUE@noinst_LTLIBRARIES = libcsplit.la
 @HAVE_LOCAL_LIBCSPLIT_TRUE@libcsplit_la_SOURCES = \
 @HAVE_LOCAL_LIBCSPLIT_TRUE@	libcsplit_definitions.h \
 @HAVE_LOCAL_LIBCSPLIT_TRUE@	libcsplit_error.c libcsplit_error.h \
 @HAVE_LOCAL_LIBCSPLIT_TRUE@	libcsplit_extern.h \
@@ -569,15 +569,16 @@
 @HAVE_LOCAL_LIBCSPLIT_TRUE@	libcsplit_libcerror.h \
 @HAVE_LOCAL_LIBCSPLIT_TRUE@	libcsplit_support.c libcsplit_support.h \
 @HAVE_LOCAL_LIBCSPLIT_TRUE@	libcsplit_types.h \
 @HAVE_LOCAL_LIBCSPLIT_TRUE@	libcsplit_unused.h \
 @HAVE_LOCAL_LIBCSPLIT_TRUE@	libcsplit_wide_split_string.c libcsplit_wide_split_string.h \
 @HAVE_LOCAL_LIBCSPLIT_TRUE@	libcsplit_wide_string.c libcsplit_wide_string.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -782,24 +783,32 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libcsplit_error.Plo
+	-rm -f ./$(DEPDIR)/libcsplit_narrow_split_string.Plo
+	-rm -f ./$(DEPDIR)/libcsplit_narrow_string.Plo
+	-rm -f ./$(DEPDIR)/libcsplit_support.Plo
+	-rm -f ./$(DEPDIR)/libcsplit_wide_split_string.Plo
+	-rm -f ./$(DEPDIR)/libcsplit_wide_string.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -888,17 +897,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcsplit ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcsplit_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libesedb-20240202/libcsplit/libcsplit_narrow_split_string.h` & `libesedb-20240420/libcsplit/libcsplit_narrow_split_string.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libcsplit/libcsplit_narrow_string.h` & `libesedb-20240420/libcsplit/libcsplit_narrow_string.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/po/remove-potcdate.sin` & `libesedb-20240420/po/remove-potcdate.sin`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/po/Makefile.in.in` & `libesedb-20240420/po/Makefile.in.in`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/po/en@quot.header` & `libesedb-20240420/po/en@quot.header`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/po/en@boldquot.header` & `libesedb-20240420/po/en@boldquot.header`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/po/insert-header.sin` & `libesedb-20240420/po/insert-header.sin`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/po/Makevars` & `libesedb-20240420/po/Makevars`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/po/Makevars.in` & `libesedb-20240420/po/Makevars.in`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/po/Rules-quot` & `libesedb-20240420/po/Rules-quot`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libuna/libuna_codepage_windows_1251.c` & `libesedb-20240420/libuna/libuna_codepage_windows_1251.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libuna/libuna_utf16_string.c` & `libesedb-20240420/libuna/libuna_utf16_string.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libuna/libuna_base16_stream.c` & `libesedb-20240420/libuna/libuna_base16_stream.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libuna/libuna_utf8_stream.h` & `libesedb-20240420/libuna/libuna_utf8_stream.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libuna/libuna_codepage_iso_8859_2.h` & `libesedb-20240420/libuna/libuna_codepage_iso_8859_2.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libuna/libuna_codepage_windows_932.c` & `libesedb-20240420/libuna/libuna_codepage_windows_932.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libuna/libuna_codepage_mac_dingbats.h` & `libesedb-20240420/libuna/libuna_codepage_mac_dingbats.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libuna/libuna_utf8_string.c` & `libesedb-20240420/libuna/libuna_utf8_string.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libuna/libuna_base64_stream.c` & `libesedb-20240420/libuna/libuna_base64_stream.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libuna/libuna_error.h` & `libesedb-20240420/libuna/libuna_error.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libuna/libuna_codepage_mac_turkish.h` & `libesedb-20240420/libuna/libuna_codepage_mac_turkish.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libuna/libuna_unicode_character.c` & `libesedb-20240420/libuna/libuna_unicode_character.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libuna/libuna_codepage_mac_gaelic.c` & `libesedb-20240420/libuna/libuna_codepage_mac_gaelic.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libuna/libuna_codepage_mac_arabic.h` & `libesedb-20240420/libuna/libuna_codepage_mac_arabic.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libuna/libuna_codepage_mac_thai.c` & `libesedb-20240420/libuna/libuna_codepage_mac_thai.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libuna/libuna_codepage_windows_874.h` & `libesedb-20240420/libuna/libuna_codepage_windows_874.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libuna/libuna_codepage_iso_8859_15.h` & `libesedb-20240420/libuna/libuna_codepage_iso_8859_15.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libuna/libuna_utf8_string.h` & `libesedb-20240420/libuna/libuna_utf8_string.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libuna/libuna_codepage_iso_8859_16.c` & `libesedb-20240420/libuna/libuna_codepage_iso_8859_16.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libuna/libuna_codepage_windows_1255.c` & `libesedb-20240420/libuna/libuna_codepage_windows_1255.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libuna/libuna_utf7_stream.c` & `libesedb-20240420/libuna/libuna_utf7_stream.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libuna/libuna_byte_stream.h` & `libesedb-20240420/libuna/libuna_byte_stream.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libuna/libuna_codepage_koi8_u.c` & `libesedb-20240420/libuna/libuna_codepage_koi8_u.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libuna/libuna_unused.h` & `libesedb-20240420/libuna/libuna_unused.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libuna/libuna_codepage_iso_8859_6.c` & `libesedb-20240420/libuna/libuna_codepage_iso_8859_6.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libuna/libuna_codepage_iso_8859_14.c` & `libesedb-20240420/libuna/libuna_codepage_iso_8859_14.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libuna/libuna_base64_stream.h` & `libesedb-20240420/libuna/libuna_base64_stream.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libuna/libuna_error.c` & `libesedb-20240420/libfvalue/libfvalue_error.c`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Error functions
  *
- * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -19,33 +19,33 @@
  * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
 #include <common.h>
 #include <file_stream.h>
 #include <types.h>
 
-#include "libuna_error.h"
-#include "libuna_libcerror.h"
+#include "libfvalue_error.h"
+#include "libfvalue_libcerror.h"
 
-#if !defined( HAVE_LOCAL_LIBUNA )
+#if !defined( HAVE_LOCAL_LIBFVALUE )
 
 /* Free an error and its elements
  */
-void libuna_error_free(
-      libuna_error_t **error )
+void libfvalue_error_free(
+      libfvalue_error_t **error )
 {
 	libcerror_error_free(
 	 (libcerror_error_t **) error );
 }
 
 /* Prints a descriptive string of the error to the stream
  * Returns the number of printed characters if successful or -1 on error
  */
-int libuna_error_fprint(
-     libuna_error_t *error,
+int libfvalue_error_fprint(
+     libfvalue_error_t *error,
      FILE *stream )
 {
 	int print_count = 0;
 
 	print_count = libcerror_error_fprint(
 	               (libcerror_error_t *) error,
 	               stream );
@@ -53,16 +53,16 @@
 	return( print_count );
 }
 
 /* Prints a descriptive string of the error to the string
  * The end-of-string character is not included in the return value
  * Returns the number of printed characters if successful or -1 on error
  */
-int libuna_error_sprint(
-     libuna_error_t *error,
+int libfvalue_error_sprint(
+     libfvalue_error_t *error,
      char *string,
      size_t size )
 {
 	int print_count = 0;
 
 	print_count = libcerror_error_sprint(
 	               (libcerror_error_t *) error,
@@ -71,16 +71,16 @@
 
 	return( print_count );
 }
 
 /* Prints a backtrace of the error to the stream
  * Returns the number of printed characters if successful or -1 on error
  */
-int libuna_error_backtrace_fprint(
-     libuna_error_t *error,
+int libfvalue_error_backtrace_fprint(
+     libfvalue_error_t *error,
       FILE *stream )
 {
 	int print_count = 0;
 
 	print_count = libcerror_error_backtrace_fprint(
 	               (libcerror_error_t *) error,
 	               stream );
@@ -88,24 +88,24 @@
 	return( print_count );
 }
 
 /* Prints a backtrace of the error to the string
  * The end-of-string character is not included in the return value
  * Returns the number of printed characters if successful or -1 on error
  */
-int libuna_error_backtrace_sprint(
-     libuna_error_t *error,
+int libfvalue_error_backtrace_sprint(
+     libfvalue_error_t *error,
      char *string,
      size_t size )
 {
 	int print_count = 0;
 
 	print_count = libcerror_error_backtrace_sprint(
 	               (libcerror_error_t *) error,
 	               string,
 	               size );
 
 	return( print_count );
 }
 
-#endif /* !defined( HAVE_LOCAL_LIBUNA ) */
+#endif /* !defined( HAVE_LOCAL_LIBFVALUE ) */
```

### Comparing `libesedb-20240202/libuna/libuna_codepage_mac_centraleurroman.h` & `libesedb-20240420/libuna/libuna_codepage_mac_centraleurroman.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libuna/libuna_codepage_mac_romanian.c` & `libesedb-20240420/libuna/libuna_codepage_mac_romanian.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libuna/libuna_codepage_iso_8859_6.h` & `libesedb-20240420/libuna/libuna_codepage_iso_8859_6.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libuna/libuna_codepage_iso_8859_9.c` & `libesedb-20240420/libuna/libuna_codepage_iso_8859_9.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libuna/libuna_codepage_mac_russian.h` & `libesedb-20240420/libuna/libuna_codepage_mac_russian.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libuna/libuna_codepage_mac_dingbats.c` & `libesedb-20240420/libuna/libuna_codepage_mac_dingbats.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libuna/libuna_codepage_iso_8859_15.c` & `libesedb-20240420/libuna/libuna_codepage_iso_8859_15.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libuna/libuna_codepage_windows_936.c` & `libesedb-20240420/libuna/libuna_codepage_windows_936.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libuna/libuna_codepage_mac_croatian.h` & `libesedb-20240420/libuna/libuna_codepage_mac_croatian.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libuna/libuna_scsu.h` & `libesedb-20240420/libuna/libuna_scsu.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libuna/Makefile.am` & `libesedb-20240420/libuna/Makefile.am`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBUNA
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libuna.la
 
 libuna_la_SOURCES = \
 	libuna_base16_stream.c libuna_base16_stream.h \
 	libuna_base32_stream.c libuna_base32_stream.h \
@@ -73,19 +73,17 @@
 	libuna_utf32_stream.c libuna_utf32_stream.h \
 	libuna_utf32_string.c libuna_utf32_string.h \
 	libuna_utf7_stream.c libuna_utf7_stream.h \
 	libuna_utf8_stream.c libuna_utf8_stream.h \
 	libuna_utf8_string.c libuna_utf8_string.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libuna ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libuna_la_SOURCES)
```

### Comparing `libesedb-20240202/libuna/libuna_utf32_stream.c` & `libesedb-20240420/libuna/libuna_utf32_stream.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libuna/libuna_codepage_windows_936.h` & `libesedb-20240420/libuna/libuna_codepage_windows_936.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libuna/libuna_codepage_iso_8859_10.c` & `libesedb-20240420/libuna/libuna_codepage_iso_8859_10.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libuna/libuna_codepage_mac_roman.c` & `libesedb-20240420/libuna/libuna_codepage_mac_roman.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libuna/libuna_utf7_stream.h` & `libesedb-20240420/libuna/libuna_utf7_stream.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libuna/libuna_codepage_iso_8859_3.h` & `libesedb-20240420/libuna/libuna_codepage_iso_8859_3.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libuna/libuna_codepage_mac_thai.h` & `libesedb-20240420/libuna/libuna_codepage_mac_thai.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libuna/libuna_codepage_mac_farsi.h` & `libesedb-20240420/libuna/libuna_codepage_mac_farsi.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libuna/libuna_codepage_mac_ukrainian.c` & `libesedb-20240420/libuna/libuna_codepage_mac_ukrainian.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libuna/libuna_codepage_mac_inuit.c` & `libesedb-20240420/libuna/libuna_codepage_mac_inuit.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libuna/libuna_codepage_windows_932.h` & `libesedb-20240420/libuna/libuna_codepage_windows_932.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libuna/libuna_codepage_windows_874.c` & `libesedb-20240420/libuna/libuna_codepage_windows_874.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libuna/libuna_codepage_iso_8859_5.c` & `libesedb-20240420/libuna/libuna_codepage_iso_8859_5.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libuna/libuna_codepage_iso_8859_10.h` & `libesedb-20240420/libuna/libuna_codepage_iso_8859_10.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libuna/libuna_definitions.h` & `libesedb-20240420/libuna/libuna_definitions.h`

 * *Files 0% similar despite different names*

```diff
@@ -31,19 +31,19 @@
 
 /* The definitions in <libuna/definitions.h> are copied here
  * for local use of libuna
  */
 #else
 #include <byte_stream.h>
 
-#define LIBUNA_VERSION						20240130
+#define LIBUNA_VERSION						20240414
 
 /* The libuna version string
  */
-#define LIBUNA_VERSION_STRING					"20240130"
+#define LIBUNA_VERSION_STRING					"20240414"
 
 /* The endian definitions
  */
 #define	LIBUNA_ENDIAN_BIG					_BYTE_STREAM_ENDIAN_BIG
 #define	LIBUNA_ENDIAN_LITTLE					_BYTE_STREAM_ENDIAN_LITTLE
 
 /* The codepage definitions
```

### Comparing `libesedb-20240202/libuna/libuna_url_stream.h` & `libesedb-20240420/libuna/libuna_url_stream.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libuna/libuna_codepage_mac_icelandic.h` & `libesedb-20240420/libuna/libuna_codepage_mac_icelandic.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libuna/libuna_codepage_koi8_u.h` & `libesedb-20240420/libuna/libuna_codepage_koi8_u.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libuna/libuna_utf16_stream.c` & `libesedb-20240420/libuna/libuna_utf16_stream.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libuna/libuna_codepage_windows_1253.c` & `libesedb-20240420/libuna/libuna_codepage_windows_1253.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libuna/libuna_codepage_iso_8859_4.h` & `libesedb-20240420/libuna/libuna_codepage_iso_8859_4.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libuna/libuna_codepage_mac_greek.c` & `libesedb-20240420/libuna/libuna_codepage_mac_greek.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libuna/libuna_libcerror.h` & `libesedb-20240420/libfvalue/libfvalue_libcerror.h`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libcerror header wrapper
  *
- * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -15,16 +15,16 @@
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License
  * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
-#if !defined( _LIBUNA_LIBCERROR_H )
-#define _LIBUNA_LIBCERROR_H
+#if !defined( _LIBFVALUE_LIBCERROR_H )
+#define _LIBFVALUE_LIBCERROR_H
 
 #include <common.h>
 
 /* Define HAVE_LOCAL_LIBCERROR for local use of libcerror
  */
 #if defined( HAVE_LOCAL_LIBCERROR )
 
@@ -42,9 +42,9 @@
 #define LIBCERROR_DLL_IMPORT
 #endif
 
 #include <libcerror.h>
 
 #endif /* defined( HAVE_LOCAL_LIBCERROR ) */
 
-#endif /* !defined( _LIBUNA_LIBCERROR_H ) */
+#endif /* !defined( _LIBFVALUE_LIBCERROR_H ) */
```

### Comparing `libesedb-20240202/libuna/libuna_codepage_mac_centraleurroman.c` & `libesedb-20240420/libuna/libuna_codepage_mac_centraleurroman.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libuna/libuna_codepage_windows_1254.c` & `libesedb-20240420/libuna/libuna_codepage_windows_1254.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libuna/libuna_codepage_iso_8859_13.h` & `libesedb-20240420/libuna/libuna_codepage_iso_8859_13.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libuna/libuna_codepage_iso_8859_7.h` & `libesedb-20240420/libuna/libuna_codepage_iso_8859_7.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libuna/libuna_codepage_windows_1255.h` & `libesedb-20240420/libuna/libuna_codepage_windows_1255.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libuna/libuna_unicode_character.h` & `libesedb-20240420/libuna/libuna_unicode_character.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libuna/libuna_codepage_iso_8859_8.h` & `libesedb-20240420/libuna/libuna_codepage_iso_8859_8.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libuna/libuna_codepage_iso_8859_13.c` & `libesedb-20240420/libuna/libuna_codepage_iso_8859_13.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libuna/libuna_codepage_windows_949.h` & `libesedb-20240420/libuna/libuna_codepage_windows_949.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libuna/libuna_codepage_mac_cyrillic.c` & `libesedb-20240420/libuna/libuna_codepage_mac_cyrillic.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libuna/libuna_codepage_mac_celtic.c` & `libesedb-20240420/libuna/libuna_codepage_mac_celtic.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libuna/libuna_support.h` & `libesedb-20240420/libuna/libuna_support.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libuna/libuna_codepage_iso_8859_4.c` & `libesedb-20240420/libuna/libuna_codepage_iso_8859_4.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libuna/libuna_codepage_windows_949.c` & `libesedb-20240420/libuna/libuna_codepage_windows_949.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libuna/libuna_utf16_stream.h` & `libesedb-20240420/libuna/libuna_utf16_stream.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libuna/libuna_codepage_mac_symbol.c` & `libesedb-20240420/libuna/libuna_codepage_mac_symbol.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libuna/libuna_codepage_mac_roman.h` & `libesedb-20240420/libuna/libuna_codepage_mac_roman.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libuna/libuna_codepage_windows_1257.c` & `libesedb-20240420/libuna/libuna_codepage_windows_1257.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libuna/libuna_codepage_windows_1254.h` & `libesedb-20240420/libuna/libuna_codepage_windows_1254.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libuna/libuna_codepage_windows_950.c` & `libesedb-20240420/libuna/libuna_codepage_windows_950.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libuna/libuna_extern.h` & `libesedb-20240420/libcnotify/libcnotify_extern.h`

 * *Files 20% similar despite different names*

```diff
@@ -15,32 +15,32 @@
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License
  * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
-#if !defined( _LIBUNA_INTERNAL_EXTERN_H )
-#define _LIBUNA_INTERNAL_EXTERN_H
+#if !defined( _LIBCNOTIFY_INTERNAL_EXTERN_H )
+#define _LIBCNOTIFY_INTERNAL_EXTERN_H
 
 #include <common.h>
 
-/* Define HAVE_LOCAL_LIBUNA for local use of libuna
+/* Define HAVE_LOCAL_LIBCNOTIFY for local use of libcnotify
  */
-#if !defined( HAVE_LOCAL_LIBUNA )
+#if !defined( HAVE_LOCAL_LIBCNOTIFY )
 
-#include <libuna/extern.h>
+#include <libcnotify/extern.h>
 
 #if defined( __CYGWIN__ ) || defined( __MINGW32__ )
-#define LIBUNA_EXTERN_VARIABLE	extern
+#define LIBCNOTIFY_EXTERN_VARIABLE	extern
 #else
-#define LIBUNA_EXTERN_VARIABLE	LIBUNA_EXTERN
+#define LIBCNOTIFY_EXTERN_VARIABLE	LIBCNOTIFY_EXTERN
 #endif
 
 #else
-#define LIBUNA_EXTERN		/* extern */
-#define LIBUNA_EXTERN_VARIABLE	extern
+#define LIBCNOTIFY_EXTERN		/* extern */
+#define LIBCNOTIFY_EXTERN_VARIABLE	extern
 
-#endif /* !defined( HAVE_LOCAL_LIBUNA ) */
+#endif /* !defined( HAVE_LOCAL_LIBCNOTIFY ) */
 
-#endif /* !defined( _LIBUNA_INTERNAL_EXTERN_H ) */
+#endif /* !defined( _LIBCNOTIFY_INTERNAL_EXTERN_H ) */
```

### Comparing `libesedb-20240202/libuna/libuna_codepage_windows_1256.c` & `libesedb-20240420/libuna/libuna_codepage_windows_1256.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libuna/libuna_types.h` & `libesedb-20240420/libuna/libuna_types.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libuna/libuna_base32_stream.h` & `libesedb-20240420/libuna/libuna_base32_stream.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libuna/libuna_codepage_windows_1253.h` & `libesedb-20240420/libuna/libuna_codepage_windows_1253.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libuna/libuna_codepage_iso_8859_16.h` & `libesedb-20240420/libuna/libuna_codepage_iso_8859_16.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libuna/libuna_utf8_stream.c` & `libesedb-20240420/libuna/libuna_utf8_stream.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libuna/libuna_codepage_windows_1250.h` & `libesedb-20240420/libuna/libuna_codepage_windows_1250.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libuna/libuna_codepage_iso_8859_2.c` & `libesedb-20240420/libuna/libuna_codepage_iso_8859_2.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libuna/libuna_support.c` & `libesedb-20240420/libcerror/libcerror_support.c`

 * *Files 12% similar despite different names*

```diff
@@ -18,22 +18,22 @@
  * You should have received a copy of the GNU Lesser General Public License
  * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
 #include <common.h>
 #include <types.h>
 
-#include "libuna_definitions.h"
-#include "libuna_support.h"
+#include "libcerror_definitions.h"
+#include "libcerror_support.h"
 
-#if !defined( HAVE_LOCAL_LIBUNA )
+#if !defined( HAVE_LOCAL_LIBCERROR )
 
 /* Returns the library version as a string
  */
-const char *libuna_get_version(
+const char *libcerror_get_version(
              void )
 {
-	return( (const char *) LIBUNA_VERSION_STRING );
+	return( (const char *) LIBCERROR_VERSION_STRING );
 }
 
-#endif /* !defined( HAVE_LOCAL_LIBUNA ) */
+#endif /* !defined( HAVE_LOCAL_LIBCERROR ) */
```

### Comparing `libesedb-20240202/libuna/libuna_codepage_koi8_r.c` & `libesedb-20240420/libuna/libuna_codepage_koi8_r.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libuna/libuna_codepage_iso_8859_5.h` & `libesedb-20240420/libuna/libuna_codepage_iso_8859_5.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libuna/libuna_utf16_string.h` & `libesedb-20240420/libuna/libuna_utf16_string.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libuna/libuna_utf32_string.c` & `libesedb-20240420/libuna/libuna_utf32_string.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libuna/libuna_codepage_mac_icelandic.c` & `libesedb-20240420/libuna/libuna_codepage_mac_icelandic.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libuna/libuna_codepage_windows_1256.h` & `libesedb-20240420/libuna/libuna_codepage_windows_1256.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libuna/libuna_utf32_string.h` & `libesedb-20240420/libuna/libuna_utf32_string.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libuna/libuna_codepage_mac_romanian.h` & `libesedb-20240420/libuna/libuna_codepage_mac_romanian.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libuna/libuna_codepage_iso_8859_8.c` & `libesedb-20240420/libuna/libuna_codepage_iso_8859_8.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libuna/libuna_codepage_koi8_r.h` & `libesedb-20240420/libuna/libuna_codepage_koi8_r.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libuna/libuna_codepage_mac_cyrillic.h` & `libesedb-20240420/libuna/libuna_codepage_mac_cyrillic.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libuna/libuna_codepage_mac_arabic.c` & `libesedb-20240420/libuna/libuna_codepage_mac_arabic.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libuna/libuna_codepage_mac_croatian.c` & `libesedb-20240420/libuna/libuna_codepage_mac_croatian.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libuna/libuna_codepage_iso_8859_9.h` & `libesedb-20240420/libuna/libuna_codepage_iso_8859_9.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libuna/libuna_codepage_mac_greek.h` & `libesedb-20240420/libuna/libuna_codepage_mac_greek.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libuna/libuna_codepage_windows_1258.h` & `libesedb-20240420/libuna/libuna_codepage_windows_1258.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libuna/libuna_codepage_iso_8859_7.c` & `libesedb-20240420/libuna/libuna_codepage_iso_8859_7.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libuna/Makefile.in` & `libesedb-20240420/libuna/Makefile.in`

 * *Files 10% similar despite different names*

```diff
@@ -719,16 +719,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBUNA_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBUNA_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBUNA_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBUNA_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBUNA_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBUNA_TRUE@	@LIBCERROR_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBUNA_TRUE@noinst_LTLIBRARIES = libuna.la
 @HAVE_LOCAL_LIBUNA_TRUE@libuna_la_SOURCES = \
 @HAVE_LOCAL_LIBUNA_TRUE@	libuna_base16_stream.c libuna_base16_stream.h \
 @HAVE_LOCAL_LIBUNA_TRUE@	libuna_base32_stream.c libuna_base32_stream.h \
 @HAVE_LOCAL_LIBUNA_TRUE@	libuna_base64_stream.c libuna_base64_stream.h \
@@ -794,15 +794,16 @@
 @HAVE_LOCAL_LIBUNA_TRUE@	libuna_utf16_string.c libuna_utf16_string.h \
 @HAVE_LOCAL_LIBUNA_TRUE@	libuna_utf32_stream.c libuna_utf32_stream.h \
 @HAVE_LOCAL_LIBUNA_TRUE@	libuna_utf32_string.c libuna_utf32_string.h \
 @HAVE_LOCAL_LIBUNA_TRUE@	libuna_utf7_stream.c libuna_utf7_stream.h \
 @HAVE_LOCAL_LIBUNA_TRUE@	libuna_utf8_stream.c libuna_utf8_stream.h \
 @HAVE_LOCAL_LIBUNA_TRUE@	libuna_utf8_string.c libuna_utf8_string.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -1064,24 +1065,89 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libuna_base16_stream.Plo
+	-rm -f ./$(DEPDIR)/libuna_base32_stream.Plo
+	-rm -f ./$(DEPDIR)/libuna_base64_stream.Plo
+	-rm -f ./$(DEPDIR)/libuna_byte_stream.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_10.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_13.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_14.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_15.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_16.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_2.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_3.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_4.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_5.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_6.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_7.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_8.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_9.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_koi8_r.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_koi8_u.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_arabic.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_celtic.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_centraleurroman.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_croatian.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_cyrillic.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_dingbats.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_farsi.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_gaelic.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_greek.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_icelandic.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_inuit.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_roman.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_romanian.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_russian.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_symbol.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_thai.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_turkish.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_ukrainian.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_1250.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_1251.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_1252.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_1253.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_1254.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_1255.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_1256.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_1257.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_1258.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_874.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_932.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_936.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_949.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_950.Plo
+	-rm -f ./$(DEPDIR)/libuna_error.Plo
+	-rm -f ./$(DEPDIR)/libuna_scsu.Plo
+	-rm -f ./$(DEPDIR)/libuna_support.Plo
+	-rm -f ./$(DEPDIR)/libuna_unicode_character.Plo
+	-rm -f ./$(DEPDIR)/libuna_url_stream.Plo
+	-rm -f ./$(DEPDIR)/libuna_utf16_stream.Plo
+	-rm -f ./$(DEPDIR)/libuna_utf16_string.Plo
+	-rm -f ./$(DEPDIR)/libuna_utf32_stream.Plo
+	-rm -f ./$(DEPDIR)/libuna_utf32_string.Plo
+	-rm -f ./$(DEPDIR)/libuna_utf7_stream.Plo
+	-rm -f ./$(DEPDIR)/libuna_utf8_stream.Plo
+	-rm -f ./$(DEPDIR)/libuna_utf8_string.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -1227,17 +1293,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libuna ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libuna_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libesedb-20240202/libuna/libuna_codepage_iso_8859_3.c` & `libesedb-20240420/libuna/libuna_codepage_iso_8859_3.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libuna/libuna_codepage_windows_1250.c` & `libesedb-20240420/libuna/libuna_codepage_windows_1250.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libuna/libuna_scsu.c` & `libesedb-20240420/libuna/libuna_scsu.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libuna/libuna_codepage_windows_1252.c` & `libesedb-20240420/libuna/libuna_codepage_windows_1252.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libuna/libuna_codepage_mac_turkish.c` & `libesedb-20240420/libuna/libuna_codepage_mac_turkish.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libuna/libuna_codepage_mac_ukrainian.h` & `libesedb-20240420/libuna/libuna_codepage_mac_ukrainian.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libuna/libuna_codepage_mac_russian.c` & `libesedb-20240420/libuna/libuna_codepage_mac_russian.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libuna/libuna_codepage_windows_1258.c` & `libesedb-20240420/libuna/libuna_codepage_windows_1258.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libuna/libuna_codepage_mac_celtic.h` & `libesedb-20240420/libuna/libuna_codepage_mac_celtic.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libuna/libuna_byte_stream.c` & `libesedb-20240420/libuna/libuna_byte_stream.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libuna/libuna_codepage_mac_gaelic.h` & `libesedb-20240420/libuna/libuna_codepage_mac_gaelic.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libuna/libuna_utf32_stream.h` & `libesedb-20240420/libuna/libuna_utf32_stream.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libuna/libuna_codepage_mac_symbol.h` & `libesedb-20240420/libuna/libuna_codepage_mac_symbol.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libuna/libuna_codepage_windows_1257.h` & `libesedb-20240420/libuna/libuna_codepage_windows_1257.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libuna/libuna_codepage_mac_inuit.h` & `libesedb-20240420/libuna/libuna_codepage_mac_inuit.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libuna/libuna_codepage_mac_farsi.c` & `libesedb-20240420/libuna/libuna_codepage_mac_farsi.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libuna/libuna_codepage_windows_950.h` & `libesedb-20240420/libuna/libuna_codepage_windows_950.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libuna/libuna_url_stream.c` & `libesedb-20240420/libuna/libuna_url_stream.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libuna/libuna_codepage_windows_1251.h` & `libesedb-20240420/libuna/libuna_codepage_windows_1251.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libuna/libuna_codepage_windows_1252.h` & `libesedb-20240420/libuna/libuna_codepage_windows_1252.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libuna/libuna_codepage_iso_8859_14.h` & `libesedb-20240420/libuna/libuna_codepage_iso_8859_14.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libuna/libuna_base16_stream.h` & `libesedb-20240420/libuna/libuna_base16_stream.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libuna/libuna_base32_stream.c` & `libesedb-20240420/libuna/libuna_base32_stream.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/Makefile.in` & `libesedb-20240420/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -668,16 +668,23 @@
 EXTRA_DIST = \
 	$(DPKG_FILES) \
 	$(GETTEXT_FILES) \
 	$(PKGCONFIG_FILES) \
 	$(SETUP_PY_FILES) \
 	$(SPEC_FILES)
 
-MAINTAINERCLEANFILES = \
-	Makefile.in
+DISTCLEANFILES = \
+	config.status \
+	config.cache \
+	config.log \
+	libesedb.pc \
+	libesedb.spec \
+	Makefile \
+	Makefile.in \
+	po/Makevars
 
 pkgconfigdir = $(libdir)/pkgconfig
 pkgconfig_DATA = \
 	libesedb.pc
 
 all: all-recursive
 
@@ -1094,23 +1101,26 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-recursive
 
 clean-am: clean-generic clean-libtool mostlyclean-am
 
+distclean: distclean-recursive
+	-rm -f $(am__CONFIG_DISTCLEAN_FILES)
+	-rm -f Makefile
 distclean-am: clean-am distclean-generic distclean-libtool \
 	distclean-tags
 
 dvi: dvi-recursive
 
 dvi-am:
 
@@ -1224,22 +1234,10 @@
 	(cd $(srcdir)/libfdatetime && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libfguid && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libfvalue && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libfwnt && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libesedb && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/po && $(MAKE) $(AM_MAKEFLAGS))
 
-distclean: clean
-	-rm -f Makefile
-	-rm -f config.status
-	-rm -f config.cache
-	-rm -f config.log
-	-rm -f libesedb.pc
-	-rm -f libesedb.spec
-	@for dir in ${subdirs}; do \
-		(cd $$dir && $(MAKE) distclean) \
-		|| case "$(MFLAGS)" in *k*) fail=yes;; *) exit 1;; esac; \
-	done && test -z "$$fail"
-
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libesedb-20240202/libfvalue/libfvalue_filetime.c` & `libesedb-20240420/libfvalue/libfvalue_filetime.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfvalue/libfvalue_utf16_string.c` & `libesedb-20240420/libfvalue/libfvalue_utf16_string.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfvalue/libfvalue_libfwnt.h` & `libesedb-20240420/libfvalue/libfvalue_libfwnt.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfvalue/libfvalue_value.c` & `libesedb-20240420/libfvalue/libfvalue_value.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfvalue/libfvalue_value.h` & `libesedb-20240420/libfvalue/libfvalue_value.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfvalue/libfvalue_definitions.h` & `libesedb-20240420/libfvalue/libfvalue_definitions.h`

 * *Files 0% similar despite different names*

```diff
@@ -32,19 +32,19 @@
 
 /* The definitions in <libfvalue/definitions.h> are copied here
  * for local use of libfvalue
  */
 #else
 #include <byte_stream.h>
 
-#define LIBFVALUE_VERSION						20240124
+#define LIBFVALUE_VERSION						20240415
 
 /* The libfvalue version string
  */
-#define LIBFVALUE_VERSION_STRING					"20240124"
+#define LIBFVALUE_VERSION_STRING					"20240415"
 
 /* The endian definitions
  */
 #define LIBFVALUE_ENDIAN_BIG						_BYTE_STREAM_ENDIAN_BIG
 #define LIBFVALUE_ENDIAN_LITTLE						_BYTE_STREAM_ENDIAN_LITTLE
 #define LIBFVALUE_ENDIAN_NATIVE						(uint8_t) 'n'
```

### Comparing `libesedb-20240202/libfvalue/libfvalue_codepage.h` & `libesedb-20240420/libfvalue/libfvalue_codepage.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfvalue/libfvalue_split_utf16_string.c` & `libesedb-20240420/libfvalue/libfvalue_split_utf16_string.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfvalue/libfvalue_error.c` & `libesedb-20240420/libfdatetime/libfdatetime_error.c`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Error functions
  *
- * Copyright (C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -19,33 +19,33 @@
  * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
 #include <common.h>
 #include <file_stream.h>
 #include <types.h>
 
-#include "libfvalue_error.h"
-#include "libfvalue_libcerror.h"
+#include "libfdatetime_error.h"
+#include "libfdatetime_libcerror.h"
 
-#if !defined( HAVE_LOCAL_LIBFVALUE )
+#if !defined( HAVE_LOCAL_LIBFDATETIME )
 
 /* Free an error and its elements
  */
-void libfvalue_error_free(
-      libfvalue_error_t **error )
+void libfdatetime_error_free(
+      libfdatetime_error_t **error )
 {
 	libcerror_error_free(
 	 (libcerror_error_t **) error );
 }
 
 /* Prints a descriptive string of the error to the stream
  * Returns the number of printed characters if successful or -1 on error
  */
-int libfvalue_error_fprint(
-     libfvalue_error_t *error,
+int libfdatetime_error_fprint(
+     libfdatetime_error_t *error,
      FILE *stream )
 {
 	int print_count = 0;
 
 	print_count = libcerror_error_fprint(
 	               (libcerror_error_t *) error,
 	               stream );
@@ -53,16 +53,16 @@
 	return( print_count );
 }
 
 /* Prints a descriptive string of the error to the string
  * The end-of-string character is not included in the return value
  * Returns the number of printed characters if successful or -1 on error
  */
-int libfvalue_error_sprint(
-     libfvalue_error_t *error,
+int libfdatetime_error_sprint(
+     libfdatetime_error_t *error,
      char *string,
      size_t size )
 {
 	int print_count = 0;
 
 	print_count = libcerror_error_sprint(
 	               (libcerror_error_t *) error,
@@ -71,16 +71,16 @@
 
 	return( print_count );
 }
 
 /* Prints a backtrace of the error to the stream
  * Returns the number of printed characters if successful or -1 on error
  */
-int libfvalue_error_backtrace_fprint(
-     libfvalue_error_t *error,
+int libfdatetime_error_backtrace_fprint(
+     libfdatetime_error_t *error,
       FILE *stream )
 {
 	int print_count = 0;
 
 	print_count = libcerror_error_backtrace_fprint(
 	               (libcerror_error_t *) error,
 	               stream );
@@ -88,24 +88,24 @@
 	return( print_count );
 }
 
 /* Prints a backtrace of the error to the string
  * The end-of-string character is not included in the return value
  * Returns the number of printed characters if successful or -1 on error
  */
-int libfvalue_error_backtrace_sprint(
-     libfvalue_error_t *error,
+int libfdatetime_error_backtrace_sprint(
+     libfdatetime_error_t *error,
      char *string,
      size_t size )
 {
 	int print_count = 0;
 
 	print_count = libcerror_error_backtrace_sprint(
 	               (libcerror_error_t *) error,
 	               string,
 	               size );
 
 	return( print_count );
 }
 
-#endif /* !defined( HAVE_LOCAL_LIBFVALUE ) */
+#endif /* !defined( HAVE_LOCAL_LIBFDATETIME ) */
```

### Comparing `libesedb-20240202/libfvalue/libfvalue_utf8_string.c` & `libesedb-20240420/libfvalue/libfvalue_utf8_string.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfvalue/libfvalue_unused.h` & `libesedb-20240420/libfvalue/libfvalue_unused.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfvalue/libfvalue_split_utf16_string.h` & `libesedb-20240420/libfvalue/libfvalue_split_utf16_string.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfvalue/libfvalue_filetime.h` & `libesedb-20240420/libfvalue/libfvalue_filetime.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfvalue/libfvalue_support.c` & `libesedb-20240420/libfvalue/libfvalue_support.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfvalue/libfvalue_extern.h` & `libesedb-20240420/libfvalue/libfvalue_extern.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfvalue/Makefile.am` & `libesedb-20240420/libfvalue/Makefile.am`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBFVALUE
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCTHREADS_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ \
 	@LIBFDATETIME_CPPFLAGS@ \
 	@LIBFGUID_CPPFLAGS@ \
@@ -41,19 +41,17 @@
 	libfvalue_value_type.c libfvalue_value_type.h \
 	libfvalue_support.c libfvalue_support.h \
 	libfvalue_unused.h \
 	libfvalue_utf8_string.c libfvalue_utf8_string.h \
 	libfvalue_utf16_string.c libfvalue_utf16_string.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libfvalue ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfvalue_la_SOURCES)
```

### Comparing `libesedb-20240202/libfvalue/libfvalue_value_type.h` & `libesedb-20240420/libfvalue/libfvalue_value_type.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfvalue/libfvalue_libcerror.h` & `libesedb-20240420/libmapidb/libmapidb_libcerror.h`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libcerror header wrapper
  *
- * Copyright (C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -15,16 +15,16 @@
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License
  * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
-#if !defined( _LIBFVALUE_LIBCERROR_H )
-#define _LIBFVALUE_LIBCERROR_H
+#if !defined( _LIBMAPIDB_LIBCERROR_H )
+#define _LIBMAPIDB_LIBCERROR_H
 
 #include <common.h>
 
 /* Define HAVE_LOCAL_LIBCERROR for local use of libcerror
  */
 #if defined( HAVE_LOCAL_LIBCERROR )
 
@@ -42,9 +42,9 @@
 #define LIBCERROR_DLL_IMPORT
 #endif
 
 #include <libcerror.h>
 
 #endif /* defined( HAVE_LOCAL_LIBCERROR ) */
 
-#endif /* !defined( _LIBFVALUE_LIBCERROR_H ) */
+#endif /* !defined( _LIBMAPIDB_LIBCERROR_H ) */
```

### Comparing `libesedb-20240202/libfvalue/libfvalue_split_utf8_string.c` & `libesedb-20240420/libfvalue/libfvalue_split_utf8_string.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfvalue/libfvalue_data_handle.h` & `libesedb-20240420/libfvalue/libfvalue_data_handle.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfvalue/libfvalue_libcnotify.h` & `libesedb-20240420/libfvalue/libfvalue_libcnotify.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfvalue/libfvalue_data_handle.c` & `libesedb-20240420/libfvalue/libfvalue_data_handle.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfvalue/libfvalue_integer.c` & `libesedb-20240420/libfvalue/libfvalue_integer.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfvalue/libfvalue_value_type.c` & `libesedb-20240420/libfvalue/libfvalue_value_type.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfvalue/libfvalue_integer.h` & `libesedb-20240420/libfvalue/libfvalue_integer.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfvalue/libfvalue_binary_data.h` & `libesedb-20240420/libfvalue/libfvalue_binary_data.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfvalue/libfvalue_value_entry.h` & `libesedb-20240420/libfvalue/libfvalue_value_entry.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfvalue/libfvalue_utf16_string.h` & `libesedb-20240420/libfvalue/libfvalue_utf16_string.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfvalue/libfvalue_error.h` & `libesedb-20240420/libfvalue/libfvalue_error.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfvalue/libfvalue_table.h` & `libesedb-20240420/libfvalue/libfvalue_table.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfvalue/libfvalue_libfguid.h` & `libesedb-20240420/libfvalue/libfvalue_libfguid.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfvalue/libfvalue_split_utf8_string.h` & `libesedb-20240420/libfvalue/libfvalue_split_utf8_string.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfvalue/libfvalue_floating_point.h` & `libesedb-20240420/libfvalue/libfvalue_floating_point.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfvalue/libfvalue_libfdatetime.h` & `libesedb-20240420/libfvalue/libfvalue_libfdatetime.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfvalue/libfvalue_string.h` & `libesedb-20240420/libfvalue/libfvalue_string.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfvalue/libfvalue_binary_data.c` & `libesedb-20240420/libfvalue/libfvalue_binary_data.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfvalue/libfvalue_value_entry.c` & `libesedb-20240420/libfvalue/libfvalue_value_entry.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfvalue/libfvalue_libcdata.h` & `libesedb-20240420/libfvalue/libfvalue_libcdata.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfvalue/libfvalue_support.h` & `libesedb-20240420/libfvalue/libfvalue_support.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfvalue/libfvalue_table.c` & `libesedb-20240420/libfvalue/libfvalue_table.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfvalue/Makefile.in` & `libesedb-20240420/libfvalue/Makefile.in`

 * *Files 7% similar despite different names*

```diff
@@ -582,16 +582,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBFVALUE_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBFVALUE_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBFVALUE_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBFVALUE_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBFVALUE_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBFVALUE_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFVALUE_TRUE@	@LIBCTHREADS_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFVALUE_TRUE@	@LIBCDATA_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFVALUE_TRUE@	@LIBCNOTIFY_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFVALUE_TRUE@	@LIBUNA_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFVALUE_TRUE@	@LIBFDATETIME_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFVALUE_TRUE@	@LIBFGUID_CPPFLAGS@ \
@@ -625,15 +625,16 @@
 @HAVE_LOCAL_LIBFVALUE_TRUE@	libfvalue_value_entry.c libfvalue_value_entry.h \
 @HAVE_LOCAL_LIBFVALUE_TRUE@	libfvalue_value_type.c libfvalue_value_type.h \
 @HAVE_LOCAL_LIBFVALUE_TRUE@	libfvalue_support.c libfvalue_support.h \
 @HAVE_LOCAL_LIBFVALUE_TRUE@	libfvalue_unused.h \
 @HAVE_LOCAL_LIBFVALUE_TRUE@	libfvalue_utf8_string.c libfvalue_utf8_string.h \
 @HAVE_LOCAL_LIBFVALUE_TRUE@	libfvalue_utf16_string.c libfvalue_utf16_string.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -848,24 +849,42 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libfvalue_binary_data.Plo
+	-rm -f ./$(DEPDIR)/libfvalue_data_handle.Plo
+	-rm -f ./$(DEPDIR)/libfvalue_error.Plo
+	-rm -f ./$(DEPDIR)/libfvalue_filetime.Plo
+	-rm -f ./$(DEPDIR)/libfvalue_floating_point.Plo
+	-rm -f ./$(DEPDIR)/libfvalue_integer.Plo
+	-rm -f ./$(DEPDIR)/libfvalue_split_utf16_string.Plo
+	-rm -f ./$(DEPDIR)/libfvalue_split_utf8_string.Plo
+	-rm -f ./$(DEPDIR)/libfvalue_string.Plo
+	-rm -f ./$(DEPDIR)/libfvalue_support.Plo
+	-rm -f ./$(DEPDIR)/libfvalue_table.Plo
+	-rm -f ./$(DEPDIR)/libfvalue_utf16_string.Plo
+	-rm -f ./$(DEPDIR)/libfvalue_utf8_string.Plo
+	-rm -f ./$(DEPDIR)/libfvalue_value.Plo
+	-rm -f ./$(DEPDIR)/libfvalue_value_entry.Plo
+	-rm -f ./$(DEPDIR)/libfvalue_value_type.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -964,17 +983,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libfvalue ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfvalue_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libesedb-20240202/libfvalue/libfvalue_utf8_string.h` & `libesedb-20240420/libfvalue/libfvalue_utf8_string.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfvalue/libfvalue_floating_point.c` & `libesedb-20240420/libfvalue/libfvalue_floating_point.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfvalue/libfvalue_types.h` & `libesedb-20240420/libfvalue/libfvalue_types.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfvalue/libfvalue_string.c` & `libesedb-20240420/libfvalue/libfvalue_string.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfvalue/libfvalue_libuna.h` & `libesedb-20240420/libfvalue/libfvalue_libuna.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libcnotify/libcnotify_definitions.h` & `libesedb-20240420/libcnotify/libcnotify_definitions.h`

 * *Files 5% similar despite different names*

```diff
@@ -31,19 +31,19 @@
 #include <libcnotify/definitions.h>
 
 /* The definitions in <libcnotify/definitions.h> are copied here
  * for local use of libcnotify
  */
 #else
 
-#define LIBCNOTIFY_VERSION				20240108
+#define LIBCNOTIFY_VERSION				20240414
 
 /* The libcnotify version string
  */
-#define LIBCNOTIFY_VERSION_STRING			"20240108"
+#define LIBCNOTIFY_VERSION_STRING			"20240414"
 
 /* The print data flags
  */
 enum LIBCNOTIFY_NOTIFY_PRINT_DATA_FLAGS
 {
 	LIBCNOTIFY_PRINT_DATA_FLAG_GROUP_DATA		= 0x01,
 };
```

### Comparing `libesedb-20240202/libcnotify/libcnotify_extern.h` & `libesedb-20240420/libfdatetime/libfdatetime_extern.h`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal extern definition
  *
- * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -15,32 +15,32 @@
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License
  * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
-#if !defined( _LIBCNOTIFY_INTERNAL_EXTERN_H )
-#define _LIBCNOTIFY_INTERNAL_EXTERN_H
+#if !defined( _LIBFDATETIME_INTERNAL_EXTERN_H )
+#define _LIBFDATETIME_INTERNAL_EXTERN_H
 
 #include <common.h>
 
-/* Define HAVE_LOCAL_LIBCNOTIFY for local use of libcnotify
+/* Define HAVE_LOCAL_LIBFDATETIME for local use of libfdatetime
  */
-#if !defined( HAVE_LOCAL_LIBCNOTIFY )
+#if !defined( HAVE_LOCAL_LIBFDATETIME )
 
-#include <libcnotify/extern.h>
+#include <libfdatetime/extern.h>
 
 #if defined( __CYGWIN__ ) || defined( __MINGW32__ )
-#define LIBCNOTIFY_EXTERN_VARIABLE	extern
+#define LIBFDATETIME_EXTERN_VARIABLE	extern
 #else
-#define LIBCNOTIFY_EXTERN_VARIABLE	LIBCNOTIFY_EXTERN
+#define LIBFDATETIME_EXTERN_VARIABLE	LIBFDATETIME_EXTERN
 #endif
 
 #else
-#define LIBCNOTIFY_EXTERN		/* extern */
-#define LIBCNOTIFY_EXTERN_VARIABLE	extern
+#define LIBFDATETIME_EXTERN		/* extern */
+#define LIBFDATETIME_EXTERN_VARIABLE	extern
 
-#endif /* !defined( HAVE_LOCAL_LIBCNOTIFY ) */
+#endif /* !defined( HAVE_LOCAL_LIBFDATETIME ) */
 
-#endif /* !defined( _LIBCNOTIFY_INTERNAL_EXTERN_H ) */
+#endif /* !defined( _LIBFDATETIME_INTERNAL_EXTERN_H ) */
```

### Comparing `libesedb-20240202/libcnotify/libcnotify_support.c` & `libesedb-20240420/libcnotify/libcnotify_support.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libcnotify/libcnotify_stream.h` & `libesedb-20240420/libcnotify/libcnotify_stream.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libcnotify/Makefile.am` & `libesedb-20240420/libcnotify/Makefile.am`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBCNOTIFY
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libcnotify.la
 
 libcnotify_la_SOURCES = \
 	libcnotify_definitions.h \
 	libcnotify_extern.h \
@@ -13,19 +13,17 @@
 	libcnotify_print.c libcnotify_print.h \
 	libcnotify_stream.c libcnotify_stream.h \
 	libcnotify_support.c libcnotify_support.h \
 	libcnotify_unused.h \
 	libcnotify_verbose.c libcnotify_verbose.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcnotify ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcnotify_la_SOURCES)
```

### Comparing `libesedb-20240202/libcnotify/libcnotify_unused.h` & `libesedb-20240420/libcnotify/libcnotify_unused.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libcnotify/libcnotify_verbose.h` & `libesedb-20240420/libcnotify/libcnotify_verbose.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libcnotify/libcnotify_print.h` & `libesedb-20240420/libcnotify/libcnotify_print.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libcnotify/libcnotify_stream.c` & `libesedb-20240420/libcnotify/libcnotify_stream.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libcnotify/libcnotify_support.h` & `libesedb-20240420/libcnotify/libcnotify_support.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libcnotify/libcnotify_verbose.c` & `libesedb-20240420/libcnotify/libcnotify_verbose.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libcnotify/Makefile.in` & `libesedb-20240420/libcnotify/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -543,30 +543,31 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBCNOTIFY_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBCNOTIFY_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBCNOTIFY_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBCNOTIFY_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@	@LIBCERROR_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@noinst_LTLIBRARIES = libcnotify.la
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@libcnotify_la_SOURCES = \
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@	libcnotify_definitions.h \
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@	libcnotify_extern.h \
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@	libcnotify_libcerror.h \
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@	libcnotify_print.c libcnotify_print.h \
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@	libcnotify_stream.c libcnotify_stream.h \
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@	libcnotify_support.c libcnotify_support.h \
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@	libcnotify_unused.h \
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@	libcnotify_verbose.c libcnotify_verbose.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -769,24 +770,30 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libcnotify_print.Plo
+	-rm -f ./$(DEPDIR)/libcnotify_stream.Plo
+	-rm -f ./$(DEPDIR)/libcnotify_support.Plo
+	-rm -f ./$(DEPDIR)/libcnotify_verbose.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -873,17 +880,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcnotify ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcnotify_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libesedb-20240202/libcnotify/libcnotify_libcerror.h` & `libesedb-20240420/libcnotify/libcnotify_libcerror.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libcnotify/libcnotify_print.c` & `libesedb-20240420/libcnotify/libcnotify_print.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libcerror/libcerror_system.c` & `libesedb-20240420/libcerror/libcerror_system.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libcerror/libcerror_error.c` & `libesedb-20240420/libcerror/libcerror_error.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libcerror/libcerror_extern.h` & `libesedb-20240420/libcerror/libcerror_extern.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libcerror/Makefile.am` & `libesedb-20240420/libcerror/Makefile.am`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 if HAVE_LOCAL_LIBCERROR
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common 
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common 
 
 noinst_LTLIBRARIES = libcerror.la
 
 libcerror_la_SOURCES = \
 	libcerror_definitions.h \
 	libcerror_extern.h \
 	libcerror_error.c libcerror_error.h \
 	libcerror_support.c libcerror_support.h \
 	libcerror_system.c libcerror_system.h \
 	libcerror_types.h \
 	libcerror_unused.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcerror ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcerror_la_SOURCES)
```

### Comparing `libesedb-20240202/libcerror/libcerror_types.h` & `libesedb-20240420/libcerror/libcerror_types.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libcerror/libcerror_support.h` & `libesedb-20240420/libcerror/libcerror_support.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libcerror/libcerror_error.h` & `libesedb-20240420/libcerror/libcerror_error.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libcerror/libcerror_system.h` & `libesedb-20240420/libcerror/libcerror_system.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libcerror/libcerror_definitions.h` & `libesedb-20240420/libcerror/libcerror_definitions.h`

 * *Files 1% similar despite different names*

```diff
@@ -31,19 +31,19 @@
 #include <libcerror/definitions.h>
 
 /* The definitions in <libcerror/definitions.h> are copied here
  * for local use of libcerror
  */
 #else
 
-#define LIBCERROR_VERSION				20240101
+#define LIBCERROR_VERSION				20240413
 
 /* The libcerror version string
  */
-#define LIBCERROR_VERSION_STRING			"20240101"
+#define LIBCERROR_VERSION_STRING			"20240413"
 
 /* The error domains
  */
 enum LIBCERROR_ERROR_DOMAINS
 {
 	LIBCERROR_ERROR_DOMAIN_ARGUMENTS		= (int) 'a',
 	LIBCERROR_ERROR_DOMAIN_CONVERSION		= (int) 'c',
```

### Comparing `libesedb-20240202/libcerror/libcerror_support.c` & `libesedb-20240420/libfdatetime/libfdatetime_support.c`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Support functions
  *
- * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -18,22 +18,24 @@
  * You should have received a copy of the GNU Lesser General Public License
  * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
 #include <common.h>
 #include <types.h>
 
-#include "libcerror_definitions.h"
-#include "libcerror_support.h"
+#include <stdio.h>
 
-#if !defined( HAVE_LOCAL_LIBCERROR )
+#include "libfdatetime_definitions.h"
+#include "libfdatetime_support.h"
+
+#if !defined( HAVE_LOCAL_LIBFDATETIME )
 
 /* Returns the library version as a string
  */
-const char *libcerror_get_version(
+const char *libfdatetime_get_version(
              void )
 {
-	return( (const char *) LIBCERROR_VERSION_STRING );
+	return( (const char *) LIBFDATETIME_VERSION_STRING );
 }
 
-#endif /* !defined( HAVE_LOCAL_LIBCERROR ) */
+#endif
```

### Comparing `libesedb-20240202/libcerror/libcerror_unused.h` & `libesedb-20240420/libcerror/libcerror_unused.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libcerror/Makefile.in` & `libesedb-20240420/libcerror/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -540,28 +540,29 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBCERROR_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBCERROR_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBCERROR_TRUE@	-I$(top_srcdir)/common 
+@HAVE_LOCAL_LIBCERROR_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBCERROR_TRUE@	-I../common -I$(top_srcdir)/common 
 
 @HAVE_LOCAL_LIBCERROR_TRUE@noinst_LTLIBRARIES = libcerror.la
 @HAVE_LOCAL_LIBCERROR_TRUE@libcerror_la_SOURCES = \
 @HAVE_LOCAL_LIBCERROR_TRUE@	libcerror_definitions.h \
 @HAVE_LOCAL_LIBCERROR_TRUE@	libcerror_extern.h \
 @HAVE_LOCAL_LIBCERROR_TRUE@	libcerror_error.c libcerror_error.h \
 @HAVE_LOCAL_LIBCERROR_TRUE@	libcerror_support.c libcerror_support.h \
 @HAVE_LOCAL_LIBCERROR_TRUE@	libcerror_system.c libcerror_system.h \
 @HAVE_LOCAL_LIBCERROR_TRUE@	libcerror_types.h \
 @HAVE_LOCAL_LIBCERROR_TRUE@	libcerror_unused.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -763,24 +764,29 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libcerror_error.Plo
+	-rm -f ./$(DEPDIR)/libcerror_support.Plo
+	-rm -f ./$(DEPDIR)/libcerror_system.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -866,17 +872,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcerror ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcerror_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libesedb-20240202/libesedb.spec.in` & `libesedb-20240420/libesedb.spec.in`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfdatetime/libfdatetime_floatingtime.h` & `libesedb-20240420/libfdatetime/libfdatetime_floatingtime.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfdatetime/libfdatetime_nsf_timedate.c` & `libesedb-20240420/libfdatetime/libfdatetime_nsf_timedate.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfdatetime/libfdatetime_error.h` & `libesedb-20240420/libfdatetime/libfdatetime_error.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfdatetime/libfdatetime_floatingtime.c` & `libesedb-20240420/libfdatetime/libfdatetime_floatingtime.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfdatetime/libfdatetime_support.h` & `libesedb-20240420/libfdatetime/libfdatetime_support.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfdatetime/libfdatetime_hfs_time.h` & `libesedb-20240420/libfdatetime/libfdatetime_hfs_time.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfdatetime/libfdatetime_definitions.h` & `libesedb-20240420/libfdatetime/libfdatetime_definitions.h`

 * *Files 0% similar despite different names*

```diff
@@ -32,19 +32,19 @@
 
 /* The definitions in <libfdatetime/definitions.h> are copied here
  * for local use of libfdatetime
  */
 #else
 #include <byte_stream.h>
 
-#define LIBFDATETIME_VERSION					20240115
+#define LIBFDATETIME_VERSION					20240415
 
 /* The version string
  */
-#define LIBFDATETIME_VERSION_STRING				"20240115"
+#define LIBFDATETIME_VERSION_STRING				"20240415"
 
 /* The byte order definitions
  */
 #define LIBFDATETIME_ENDIAN_BIG					_BYTE_STREAM_ENDIAN_BIG
 #define LIBFDATETIME_ENDIAN_LITTLE				_BYTE_STREAM_ENDIAN_LITTLE
 
 /* The string format definition flags
```

### Comparing `libesedb-20240202/libfdatetime/libfdatetime_hfs_time.c` & `libesedb-20240420/libfdatetime/libfdatetime_hfs_time.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfdatetime/Makefile.am` & `libesedb-20240420/libfdatetime/Makefile.am`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBFDATETIME
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libfdatetime.la
 
 libfdatetime_la_SOURCES = \
 	libfdatetime_date_time_values.c libfdatetime_date_time_values.h \
 	libfdatetime_definitions.h \
@@ -20,19 +20,17 @@
 	libfdatetime_posix_time.c libfdatetime_posix_time.h \
 	libfdatetime_support.c libfdatetime_support.h \
 	libfdatetime_systemtime.c libfdatetime_systemtime.h \
 	libfdatetime_types.h \
 	libfdatetime_unused.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libfdatetime ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfdatetime_la_SOURCES)
```

### Comparing `libesedb-20240202/libfdatetime/libfdatetime_filetime.c` & `libesedb-20240420/libfdatetime/libfdatetime_filetime.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfdatetime/libfdatetime_systemtime.h` & `libesedb-20240420/libfdatetime/libfdatetime_systemtime.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfdatetime/libfdatetime_posix_time.c` & `libesedb-20240420/libfdatetime/libfdatetime_posix_time.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfdatetime/libfdatetime_unused.h` & `libesedb-20240420/libfdatetime/libfdatetime_unused.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfdatetime/libfdatetime_fat_date_time.h` & `libesedb-20240420/libfdatetime/libfdatetime_fat_date_time.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfdatetime/libfdatetime_systemtime.c` & `libesedb-20240420/libfdatetime/libfdatetime_systemtime.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfdatetime/libfdatetime_nsf_timedate.h` & `libesedb-20240420/libfdatetime/libfdatetime_nsf_timedate.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfdatetime/libfdatetime_libcerror.h` & `libesedb-20240420/libfdatetime/libfdatetime_libcerror.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfdatetime/libfdatetime_support.c` & `libesedb-20240420/libmapidb/libmapidb_support.c`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Support functions
  *
- * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -20,22 +20,23 @@
  */
 
 #include <common.h>
 #include <types.h>
 
 #include <stdio.h>
 
-#include "libfdatetime_definitions.h"
-#include "libfdatetime_support.h"
+#include "libmapidb_definitions.h"
+#include "libmapidb_libcerror.h"
+#include "libmapidb_support.h"
 
-#if !defined( HAVE_LOCAL_LIBFDATETIME )
+#if !defined( HAVE_LOCAL_LIBMAPIDB )
 
 /* Returns the library version as a string
  */
-const char *libfdatetime_get_version(
+const char *libmapidb_get_version(
              void )
 {
-	return( (const char *) LIBFDATETIME_VERSION_STRING );
+	return( (const char *) LIBMAPIDB_VERSION_STRING );
 }
 
 #endif
```

### Comparing `libesedb-20240202/libfdatetime/libfdatetime_error.c` & `libesedb-20240420/libmapidb/libmapidb_error.c`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Error functions
  *
- * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -19,33 +19,33 @@
  * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
 #include <common.h>
 #include <file_stream.h>
 #include <types.h>
 
-#include "libfdatetime_error.h"
-#include "libfdatetime_libcerror.h"
+#include "libmapidb_error.h"
+#include "libmapidb_libcerror.h"
 
-#if !defined( HAVE_LOCAL_LIBFDATETIME )
+#if !defined( HAVE_LOCAL_LIBMAPIDB )
 
 /* Free an error and its elements
  */
-void libfdatetime_error_free(
-      libfdatetime_error_t **error )
+void libmapidb_error_free(
+      libmapidb_error_t **error )
 {
 	libcerror_error_free(
 	 (libcerror_error_t **) error );
 }
 
 /* Prints a descriptive string of the error to the stream
  * Returns the number of printed characters if successful or -1 on error
  */
-int libfdatetime_error_fprint(
-     libfdatetime_error_t *error,
+int libmapidb_error_fprint(
+     libmapidb_error_t *error,
      FILE *stream )
 {
 	int print_count = 0;
 
 	print_count = libcerror_error_fprint(
 	               (libcerror_error_t *) error,
 	               stream );
@@ -53,16 +53,16 @@
 	return( print_count );
 }
 
 /* Prints a descriptive string of the error to the string
  * The end-of-string character is not included in the return value
  * Returns the number of printed characters if successful or -1 on error
  */
-int libfdatetime_error_sprint(
-     libfdatetime_error_t *error,
+int libmapidb_error_sprint(
+     libmapidb_error_t *error,
      char *string,
      size_t size )
 {
 	int print_count = 0;
 
 	print_count = libcerror_error_sprint(
 	               (libcerror_error_t *) error,
@@ -71,16 +71,16 @@
 
 	return( print_count );
 }
 
 /* Prints a backtrace of the error to the stream
  * Returns the number of printed characters if successful or -1 on error
  */
-int libfdatetime_error_backtrace_fprint(
-     libfdatetime_error_t *error,
+int libmapidb_error_backtrace_fprint(
+     libmapidb_error_t *error,
       FILE *stream )
 {
 	int print_count = 0;
 
 	print_count = libcerror_error_backtrace_fprint(
 	               (libcerror_error_t *) error,
 	               stream );
@@ -88,24 +88,24 @@
 	return( print_count );
 }
 
 /* Prints a backtrace of the error to the string
  * The end-of-string character is not included in the return value
  * Returns the number of printed characters if successful or -1 on error
  */
-int libfdatetime_error_backtrace_sprint(
-     libfdatetime_error_t *error,
+int libmapidb_error_backtrace_sprint(
+     libmapidb_error_t *error,
      char *string,
      size_t size )
 {
 	int print_count = 0;
 
 	print_count = libcerror_error_backtrace_sprint(
 	               (libcerror_error_t *) error,
 	               string,
 	               size );
 
 	return( print_count );
 }
 
-#endif /* !defined( HAVE_LOCAL_LIBFDATETIME ) */
+#endif /* !defined( HAVE_LOCAL_LIBMAPIDB ) */
```

### Comparing `libesedb-20240202/libfdatetime/libfdatetime_posix_time.h` & `libesedb-20240420/libfdatetime/libfdatetime_posix_time.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfdatetime/libfdatetime_date_time_values.h` & `libesedb-20240420/libfdatetime/libfdatetime_date_time_values.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfdatetime/libfdatetime_filetime.h` & `libesedb-20240420/libfdatetime/libfdatetime_filetime.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfdatetime/libfdatetime_date_time_values.c` & `libesedb-20240420/libfdatetime/libfdatetime_date_time_values.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfdatetime/libfdatetime_types.h` & `libesedb-20240420/libfdatetime/libfdatetime_types.h`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/libfdatetime/Makefile.in` & `libesedb-20240420/libfdatetime/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -562,16 +562,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBFDATETIME_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBFDATETIME_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBFDATETIME_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBFDATETIME_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBFDATETIME_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBFDATETIME_TRUE@	@LIBCERROR_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBFDATETIME_TRUE@noinst_LTLIBRARIES = libfdatetime.la
 @HAVE_LOCAL_LIBFDATETIME_TRUE@libfdatetime_la_SOURCES = \
 @HAVE_LOCAL_LIBFDATETIME_TRUE@	libfdatetime_date_time_values.c libfdatetime_date_time_values.h \
 @HAVE_LOCAL_LIBFDATETIME_TRUE@	libfdatetime_definitions.h \
 @HAVE_LOCAL_LIBFDATETIME_TRUE@	libfdatetime_extern.h \
@@ -584,15 +584,16 @@
 @HAVE_LOCAL_LIBFDATETIME_TRUE@	libfdatetime_nsf_timedate.c libfdatetime_nsf_timedate.h \
 @HAVE_LOCAL_LIBFDATETIME_TRUE@	libfdatetime_posix_time.c libfdatetime_posix_time.h \
 @HAVE_LOCAL_LIBFDATETIME_TRUE@	libfdatetime_support.c libfdatetime_support.h \
 @HAVE_LOCAL_LIBFDATETIME_TRUE@	libfdatetime_systemtime.c libfdatetime_systemtime.h \
 @HAVE_LOCAL_LIBFDATETIME_TRUE@	libfdatetime_types.h \
 @HAVE_LOCAL_LIBFDATETIME_TRUE@	libfdatetime_unused.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -801,24 +802,36 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libfdatetime_date_time_values.Plo
+	-rm -f ./$(DEPDIR)/libfdatetime_error.Plo
+	-rm -f ./$(DEPDIR)/libfdatetime_fat_date_time.Plo
+	-rm -f ./$(DEPDIR)/libfdatetime_filetime.Plo
+	-rm -f ./$(DEPDIR)/libfdatetime_floatingtime.Plo
+	-rm -f ./$(DEPDIR)/libfdatetime_hfs_time.Plo
+	-rm -f ./$(DEPDIR)/libfdatetime_nsf_timedate.Plo
+	-rm -f ./$(DEPDIR)/libfdatetime_posix_time.Plo
+	-rm -f ./$(DEPDIR)/libfdatetime_support.Plo
+	-rm -f ./$(DEPDIR)/libfdatetime_systemtime.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -911,17 +924,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libfdatetime ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfdatetime_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libesedb-20240202/libfdatetime/libfdatetime_fat_date_time.c` & `libesedb-20240420/libfdatetime/libfdatetime_fat_date_time.c`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/aclocal.m4` & `libesedb-20240420/aclocal.m4`

 * *Files identical despite different names*

### Comparing `libesedb-20240202/configure.ac` & `libesedb-20240420/configure.ac`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 AC_PREREQ([2.71])
 
 AC_INIT(
  [libesedb],
- [20240202],
+ [20240420],
  [joachim.metz@gmail.com])
 
 AC_CONFIG_SRCDIR(
  [include/libesedb.h.in])
 
 AM_INIT_AUTOMAKE([gnu 1.6 tar-ustar])
 AM_EXTRA_RECURSIVE_TARGETS([sources splint])
```

