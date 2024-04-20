# Comparing `tmp/libexe-python-20240205.tar.gz` & `tmp/libexe-python-20240420.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libexe-python-20240205.tar", last modified: Mon Feb  5 05:07:27 2024, max compression
+gzip compressed data, was "libexe-python-20240420.tar", last modified: Sat Apr 20 19:41:16 2024, max compression
```

## Comparing `libexe-python-20240205.tar` & `libexe-python-20240420.tar`

### file list

```diff
@@ -1,788 +1,788 @@
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-05 05:07:27.000000 libexe-20240205/
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-05 05:07:26.000000 libexe-20240205/libfdata/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-02-05 04:54:54.000000 libexe-20240205/libfdata/libfdata_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37893 2024-02-05 04:54:54.000000 libexe-20240205/libfdata/libfdata_area.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9700 2024-02-05 04:54:54.000000 libexe-20240205/libfdata/libfdata_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1491 2024-02-05 04:54:54.000000 libexe-20240205/libfdata/libfdata_cache.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30931 2024-02-05 04:54:54.000000 libexe-20240205/libfdata/libfdata_range_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6826 2024-02-05 04:54:54.000000 libexe-20240205/libfdata/libfdata_mapped_range.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-02-05 04:54:54.000000 libexe-20240205/libfdata/libfdata_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6533 2024-02-05 04:54:54.000000 libexe-20240205/libfdata/libfdata_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   107689 2024-02-05 04:54:54.000000 libexe-20240205/libfdata/libfdata_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1548 2024-02-05 04:54:54.000000 libexe-20240205/libfdata/libfdata_libcdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12090 2024-02-05 04:54:54.000000 libexe-20240205/libfdata/libfdata_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4017 2024-02-05 04:54:54.000000 libexe-20240205/libfdata/libfdata_list_element.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1291 2024-02-05 04:54:54.000000 libexe-20240205/libfdata/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-02-05 04:54:54.000000 libexe-20240205/libfdata/libfdata_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-02-05 04:54:54.000000 libexe-20240205/libfdata/libfdata_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2754 2024-02-05 04:54:54.000000 libexe-20240205/libfdata/libfdata_notify.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1658 2024-02-05 04:54:54.000000 libexe-20240205/libfdata/libfdata_cache.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    66203 2024-02-05 04:54:54.000000 libexe-20240205/libfdata/libfdata_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-02-05 04:54:54.000000 libexe-20240205/libfdata/libfdata_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2092 2024-02-05 04:54:54.000000 libexe-20240205/libfdata/libfdata_range.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7327 2024-02-05 04:54:54.000000 libexe-20240205/libfdata/libfdata_area.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-02-05 04:54:54.000000 libexe-20240205/libfdata/libfdata_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1230 2024-02-05 04:54:54.000000 libexe-20240205/libfdata/libfdata_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7149 2024-02-05 04:54:54.000000 libexe-20240205/libfdata/libfdata_range.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1995 2024-02-05 04:54:54.000000 libexe-20240205/libfdata/libfdata_mapped_range.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1172 2024-02-05 04:54:54.000000 libexe-20240205/libfdata/libfdata_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19329 2024-02-05 04:54:54.000000 libexe-20240205/libfdata/libfdata_list_element.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21271 2024-02-05 04:54:54.000000 libexe-20240205/libfdata/libfdata_segments_array.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2054 2024-02-05 04:54:54.000000 libexe-20240205/libfdata/libfdata_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1593 2024-02-05 04:54:54.000000 libexe-20240205/libfdata/libfdata_notify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6013 2024-02-05 04:54:54.000000 libexe-20240205/libfdata/libfdata_range_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2804 2024-02-05 04:54:54.000000 libexe-20240205/libfdata/libfdata_segments_array.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31889 2024-02-05 04:55:06.000000 libexe-20240205/libfdata/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    49670 2024-02-05 04:54:54.000000 libexe-20240205/libfdata/libfdata_vector.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-02-05 04:54:54.000000 libexe-20240205/libfdata/libfdata_libfcache.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7810 2024-02-05 04:54:54.000000 libexe-20240205/libfdata/libfdata_vector.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-05 05:07:26.000000 libexe-20240205/libexe/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5298 2024-02-05 04:46:59.000000 libexe-20240205/libexe/libexe_definitions.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2730 2024-02-05 04:46:59.000000 libexe-20240205/libexe/libexe_notify.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5145 2024-02-05 04:46:59.000000 libexe-20240205/libexe/libexe_debug_data.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10344 2024-02-05 04:46:59.000000 libexe-20240205/libexe/libexe_mz_header.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1070 2024-02-05 04:46:59.000000 libexe-20240205/libexe/libexe.rc.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14025 2024-02-05 04:46:59.000000 libexe-20240205/libexe/libexe_section_io_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1791 2024-02-05 04:46:59.000000 libexe-20240205/libexe/libexe_mz_header.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6441 2024-02-05 04:46:59.000000 libexe-20240205/libexe/libexe_ne_header.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1068 2024-02-05 04:55:15.000000 libexe-20240205/libexe/libexe.rc
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1938 2024-02-05 04:46:59.000000 libexe-20240205/libexe/libexe_coff_header.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2589 2024-02-05 04:46:59.000000 libexe-20240205/libexe/exe_mz_header.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3010 2024-02-05 04:46:59.000000 libexe-20240205/libexe/libexe_section_io_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3906 2024-02-05 04:46:59.000000 libexe-20240205/libexe/libexe_io_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1730 2024-02-05 04:46:59.000000 libexe-20240205/libexe/libexe_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1748 2024-02-05 04:46:59.000000 libexe-20240205/libexe/libexe_ne_header.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4152 2024-02-05 04:46:59.000000 libexe-20240205/libexe/libexe_section.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29646 2024-02-05 04:46:59.000000 libexe-20240205/libexe/libexe_io_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1650 2024-02-05 04:46:59.000000 libexe-20240205/libexe/libexe_import_table.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12313 2024-02-05 04:46:59.000000 libexe-20240205/libexe/libexe_debug.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2428 2023-12-03 09:03:41.000000 libexe-20240205/libexe/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5296 2024-02-05 04:55:15.000000 libexe-20240205/libexe/libexe_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4026 2024-02-05 04:46:59.000000 libexe-20240205/libexe/libexe_file.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1392 2024-02-05 04:46:59.000000 libexe-20240205/libexe/libexe_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7527 2024-02-05 04:46:59.000000 libexe-20240205/libexe/libexe_section_descriptor.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1749 2024-02-05 04:46:59.000000 libexe-20240205/libexe/libexe_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2172 2024-02-05 04:46:59.000000 libexe-20240205/libexe/libexe_coff_optional_header.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2882 2024-02-05 04:46:59.000000 libexe-20240205/libexe/libexe_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1211 2024-02-05 04:46:59.000000 libexe-20240205/libexe/exe_pe_header.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1453 2024-02-05 04:46:59.000000 libexe-20240205/libexe/libexe_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1563 2024-02-05 04:46:59.000000 libexe-20240205/libexe/libexe_notify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9263 2024-02-05 04:46:59.000000 libexe-20240205/libexe/libexe_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1450 2024-02-05 04:46:59.000000 libexe-20240205/libexe/libexe_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10091 2024-02-05 04:46:59.000000 libexe-20240205/libexe/exe_file_header.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5312 2024-02-05 04:46:59.000000 libexe-20240205/libexe/libexe_import_table.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1320 2024-02-05 04:46:59.000000 libexe-20240205/libexe/exe_ne_header.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39233 2024-02-05 04:46:59.000000 libexe-20240205/libexe/libexe_file.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8466 2024-02-05 04:46:59.000000 libexe-20240205/libexe/libexe_coff_header.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1720 2024-02-05 04:46:59.000000 libexe-20240205/libexe/libexe_libfdatetime.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2267 2024-02-05 04:46:59.000000 libexe-20240205/libexe/libexe_section_descriptor.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1697 2024-02-05 04:46:59.000000 libexe-20240205/libexe/libexe_libbfio.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1260 2024-02-05 04:46:59.000000 libexe-20240205/libexe/exe_le_header.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1539 2024-02-05 04:46:59.000000 libexe-20240205/libexe/libexe_libfdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1807 2024-02-05 04:46:59.000000 libexe-20240205/libexe/libexe.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1560 2024-02-05 04:46:59.000000 libexe-20240205/libexe/libexe_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1542 2024-02-05 04:46:59.000000 libexe-20240205/libexe/libexe_libcdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-02-05 04:46:59.000000 libexe-20240205/libexe/libexe_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1832 2024-02-05 04:46:59.000000 libexe-20240205/libexe/libexe_debug.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1649 2024-02-05 04:46:59.000000 libexe-20240205/libexe/libexe_export_table.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2571 2024-02-05 04:46:59.000000 libexe-20240205/libexe/libexe_codepage.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35054 2024-02-05 04:55:06.000000 libexe-20240205/libexe/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5306 2024-02-05 04:46:59.000000 libexe-20240205/libexe/libexe_export_table.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1363 2024-02-05 04:46:59.000000 libexe-20240205/libexe/libexe_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1362 2024-02-05 04:46:59.000000 libexe-20240205/libexe/libexe_data_directory_descriptor.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6441 2024-02-05 04:46:59.000000 libexe-20240205/libexe/libexe_le_header.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2085 2024-02-05 04:46:59.000000 libexe-20240205/libexe/exe_section_table.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    24494 2024-02-05 04:46:59.000000 libexe-20240205/libexe/libexe_section.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37745 2024-02-05 04:46:59.000000 libexe-20240205/libexe/libexe_coff_optional_header.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1986 2024-02-05 04:46:59.000000 libexe-20240205/libexe/libexe_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2024-02-05 04:46:59.000000 libexe-20240205/libexe/libexe_libfcache.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1618 2024-02-05 04:46:59.000000 libexe-20240205/libexe/libexe_debug_data.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1748 2024-02-05 04:46:59.000000 libexe-20240205/libexe/libexe_le_header.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      667 2024-02-05 04:46:57.000000 libexe-20240205/libexe.pc.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35149 2024-02-05 04:46:57.000000 libexe-20240205/COPYING
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    15358 2024-02-05 04:55:06.000000 libexe-20240205/install-sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-05 04:46:57.000000 libexe-20240205/NEWS
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    23568 2024-02-05 04:55:06.000000 libexe-20240205/depcomp
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-05 05:07:25.000000 libexe-20240205/m4/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11498 2023-12-03 09:03:43.000000 libexe-20240205/m4/libcfile.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18233 2023-12-03 09:03:43.000000 libexe-20240205/m4/libfdatetime.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      756 2023-12-03 09:03:43.000000 libexe-20240205/m4/tests.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9379 2023-12-03 09:03:43.000000 libexe-20240205/m4/libcpath.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11944 2023-12-03 09:03:43.000000 libexe-20240205/m4/lib-prefix.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3090 2023-12-03 09:03:43.000000 libexe-20240205/m4/progtest.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31269 2023-12-03 09:03:43.000000 libexe-20240205/m4/libuna.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14488 2023-12-03 09:03:43.000000 libexe-20240205/m4/gettext.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5370 2023-12-03 09:03:43.000000 libexe-20240205/m4/lib-ld.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8230 2023-12-03 09:03:43.000000 libexe-20240205/m4/libclocale.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17147 2023-12-03 09:03:43.000000 libexe-20240205/m4/libcdata.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7384 2023-12-03 09:03:43.000000 libexe-20240205/m4/libcsplit.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14115 2023-12-03 09:03:43.000000 libexe-20240205/m4/common.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11112 2023-12-03 09:03:43.000000 libexe-20240205/m4/libcthreads.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      714 2024-02-05 04:55:02.000000 libexe-20240205/m4/ltversion.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4395 2024-02-05 04:55:02.000000 libexe-20240205/m4/ltsugar.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15545 2023-12-03 09:03:43.000000 libexe-20240205/m4/libfdata.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22432 2023-12-03 09:03:43.000000 libexe-20240205/m4/host-cpu-c-abi.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   307188 2024-02-05 04:55:02.000000 libexe-20240205/m4/libtool.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18831 2023-12-03 09:03:43.000000 libexe-20240205/m4/po.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6260 2023-12-03 09:03:43.000000 libexe-20240205/m4/libcerror.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5638 2023-12-03 09:03:43.000000 libexe-20240205/m4/libcnotify.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11692 2023-12-03 09:03:43.000000 libexe-20240205/m4/libbfio.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3229 2023-12-03 09:03:43.000000 libexe-20240205/m4/intlmacosx.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6151 2024-02-05 04:55:02.000000 libexe-20240205/m4/lt~obsolete.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34802 2023-12-03 09:03:43.000000 libexe-20240205/m4/lib-link.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9731 2023-12-03 09:03:43.000000 libexe-20240205/m4/iconv.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14525 2024-02-05 04:55:02.000000 libexe-20240205/m4/ltoptions.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1234 2023-12-03 09:03:43.000000 libexe-20240205/m4/nls.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6323 2023-12-03 09:03:43.000000 libexe-20240205/m4/python.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2058 2023-12-03 09:03:43.000000 libexe-20240205/m4/types.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7325 2023-12-03 09:03:43.000000 libexe-20240205/m4/libfcache.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3852 2023-12-03 09:03:43.000000 libexe-20240205/m4/pthread.m4
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-05 05:07:25.000000 libexe-20240205/include/
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-05 05:07:25.000000 libexe-20240205/include/libexe/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3783 2024-02-05 04:46:58.000000 libexe-20240205/include/libexe/definitions.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3781 2024-02-05 04:55:15.000000 libexe-20240205/include/libexe/definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4959 2024-02-05 04:46:58.000000 libexe-20240205/include/libexe/types.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4828 2024-02-05 04:55:15.000000 libexe-20240205/include/libexe/types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1527 2024-02-05 04:46:58.000000 libexe-20240205/include/libexe/features.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6622 2024-02-05 04:46:58.000000 libexe-20240205/include/libexe/error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2024-02-05 04:46:58.000000 libexe-20240205/include/libexe/extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1463 2024-02-05 04:55:15.000000 libexe-20240205/include/libexe/features.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5078 2024-02-05 04:46:58.000000 libexe-20240205/include/libexe/codepage.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      444 2024-02-05 04:46:57.000000 libexe-20240205/include/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13070 2024-02-05 04:55:15.000000 libexe-20240205/include/libexe.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26612 2024-02-05 04:55:06.000000 libexe-20240205/include/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13070 2024-02-05 04:46:58.000000 libexe-20240205/include/libexe.h.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-05 05:07:26.000000 libexe-20240205/common/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      957 2024-02-05 04:46:58.000000 libexe-20240205/common/config_borlandc.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3878 2024-02-05 04:46:58.000000 libexe-20240205/common/file_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3259 2024-02-05 04:46:58.000000 libexe-20240205/common/memory.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10437 2024-02-05 04:46:58.000000 libexe-20240205/common/byte_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1250 2024-02-05 04:46:58.000000 libexe-20240205/common/common.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2382 2024-02-05 04:46:58.000000 libexe-20240205/common/config_winapi.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4611 2024-02-05 04:46:58.000000 libexe-20240205/common/system_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      366 2024-02-05 04:46:57.000000 libexe-20240205/common/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7375 2024-02-05 04:46:58.000000 libexe-20240205/common/types.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7372 2024-02-05 04:55:15.000000 libexe-20240205/common/types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15715 2024-02-05 04:55:05.000000 libexe-20240205/common/config.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16641 2024-02-05 04:55:15.000000 libexe-20240205/common/config.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5064 2024-02-05 04:46:58.000000 libexe-20240205/common/wide_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5419 2024-02-05 04:46:58.000000 libexe-20240205/common/narrow_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1157 2024-02-05 04:46:58.000000 libexe-20240205/common/config_msc.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23657 2024-02-05 04:55:06.000000 libexe-20240205/common/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-05 05:07:26.000000 libexe-20240205/exetools/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1737 2024-02-05 04:46:59.000000 libexe-20240205/exetools/exetools_signal.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1433 2024-02-05 04:46:59.000000 libexe-20240205/exetools/exetools_output.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2172 2024-02-05 04:48:15.000000 libexe-20240205/exetools/info_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1207 2024-02-05 04:46:59.000000 libexe-20240205/exetools/exetools_i18n.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1775 2024-02-05 04:46:59.000000 libexe-20240205/exetools/exetools_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      965 2024-02-05 04:46:59.000000 libexe-20240205/exetools/exetools_libexe.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1742 2024-02-05 04:46:59.000000 libexe-20240205/exetools/exetools_libbfio.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1765 2024-02-05 04:46:59.000000 libexe-20240205/exetools/exetools_libfdatetime.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3784 2024-02-05 04:46:59.000000 libexe-20240205/exetools/exetools_output.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1185 2023-12-03 09:03:42.000000 libexe-20240205/exetools/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1498 2024-02-05 04:46:59.000000 libexe-20240205/exetools/exetools_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11760 2024-02-05 04:48:15.000000 libexe-20240205/exetools/info_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1477 2024-02-05 04:46:59.000000 libexe-20240205/exetools/exetools_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4527 2024-02-05 04:46:59.000000 libexe-20240205/exetools/exetools_getopt.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1495 2024-02-05 04:46:59.000000 libexe-20240205/exetools/exetools_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1803 2024-02-05 04:46:59.000000 libexe-20240205/exetools/exetools_getopt.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5701 2024-02-05 04:46:59.000000 libexe-20240205/exetools/exetools_signal.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1527 2024-02-05 04:46:59.000000 libexe-20240205/exetools/exetools_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30021 2024-02-05 04:55:06.000000 libexe-20240205/exetools/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6835 2024-02-05 04:48:15.000000 libexe-20240205/exetools/exeinfo.c
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-05 05:07:26.000000 libexe-20240205/libclocale/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1969 2024-02-05 04:54:47.000000 libexe-20240205/libclocale/libclocale_wide_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1412 2024-02-05 04:54:47.000000 libexe-20240205/libclocale/libclocale_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      779 2024-02-05 04:54:47.000000 libexe-20240205/libclocale/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3412 2024-02-05 04:54:47.000000 libexe-20240205/libclocale/libclocale_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2024-02-05 04:54:47.000000 libexe-20240205/libclocale/libclocale_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1365 2024-02-05 04:54:47.000000 libexe-20240205/libclocale/libclocale_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1717 2024-02-05 04:54:47.000000 libexe-20240205/libclocale/libclocale_locale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3142 2024-02-05 04:54:47.000000 libexe-20240205/libclocale/libclocale_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21033 2024-02-05 04:54:47.000000 libexe-20240205/libclocale/libclocale_codepage.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10671 2024-02-05 04:54:47.000000 libexe-20240205/libclocale/libclocale_locale.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28660 2024-02-05 04:55:06.000000 libexe-20240205/libclocale/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1415 2024-02-05 04:54:47.000000 libexe-20240205/libclocale/libclocale_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1696 2024-02-05 04:54:47.000000 libexe-20240205/libclocale/libclocale_wide_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1961 2024-02-05 04:54:47.000000 libexe-20240205/libclocale/libclocale_codepage.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-05 05:07:26.000000 libexe-20240205/libfcache/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1551 2024-02-05 04:54:53.000000 libexe-20240205/libfcache/libfcache_libcdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1619 2024-02-05 04:54:53.000000 libexe-20240205/libfcache/libfcache_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12461 2024-02-05 04:54:53.000000 libexe-20240205/libfcache/libfcache_cache_value.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-02-05 04:54:53.000000 libexe-20240205/libfcache/libfcache_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      880 2024-02-05 04:54:53.000000 libexe-20240205/libfcache/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2024-02-05 04:54:53.000000 libexe-20240205/libfcache/libfcache_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-02-05 04:54:53.000000 libexe-20240205/libfcache/libfcache_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1178 2024-02-05 04:54:53.000000 libexe-20240205/libfcache/libfcache_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3806 2024-02-05 04:54:53.000000 libexe-20240205/libfcache/libfcache_cache.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2924 2024-02-05 04:54:53.000000 libexe-20240205/libfcache/libfcache_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-02-05 04:54:53.000000 libexe-20240205/libfcache/libfcache_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2259 2024-02-05 04:54:53.000000 libexe-20240205/libfcache/libfcache_date_time.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-02-05 04:54:53.000000 libexe-20240205/libfcache/libfcache_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3161 2024-02-05 04:54:53.000000 libexe-20240205/libfcache/libfcache_cache_value.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29133 2024-02-05 04:55:06.000000 libexe-20240205/libfcache/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1250 2024-02-05 04:54:53.000000 libexe-20240205/libfcache/libfcache_date_time.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1680 2024-02-05 04:54:53.000000 libexe-20240205/libfcache/libfcache_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26186 2024-02-05 04:54:53.000000 libexe-20240205/libfcache/libfcache_cache.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2200 2023-12-03 09:03:28.000000 libexe-20240205/Makefile.am
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-05 05:07:26.000000 libexe-20240205/libbfio/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2630 2024-02-05 04:54:40.000000 libexe-20240205/libbfio/libbfio_file_range.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27543 2024-02-05 04:54:40.000000 libexe-20240205/libbfio/libbfio_file_range_io_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2324 2024-02-05 04:54:40.000000 libexe-20240205/libbfio/libbfio_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1362 2024-02-05 04:54:40.000000 libexe-20240205/libbfio/libbfio_libcpath.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1772 2024-02-05 04:54:40.000000 libexe-20240205/libbfio/libbfio_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-02-05 04:54:40.000000 libexe-20240205/libbfio/libbfio_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2896 2024-02-05 04:54:40.000000 libexe-20240205/libbfio/libbfio_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1733 2024-02-05 04:54:40.000000 libexe-20240205/libbfio/libbfio_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4085 2024-02-05 04:54:40.000000 libexe-20240205/libbfio/libbfio_file_io_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2077 2024-02-05 04:54:40.000000 libexe-20240205/libbfio/libbfio_file_pool.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12186 2024-02-05 04:54:40.000000 libexe-20240205/libbfio/libbfio_file_range.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1572 2024-02-05 04:54:40.000000 libexe-20240205/libbfio/libbfio_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2024-02-05 04:54:40.000000 libexe-20240205/libbfio/libbfio_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1545 2024-02-05 04:54:40.000000 libexe-20240205/libbfio/libbfio_libcdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2234 2024-02-05 04:54:40.000000 libexe-20240205/libbfio/libbfio_file.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-02-05 04:54:40.000000 libexe-20240205/libbfio/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1420 2024-02-05 04:54:40.000000 libexe-20240205/libbfio/libbfio_libcfile.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2708 2024-02-05 04:54:40.000000 libexe-20240205/libbfio/libbfio_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2614 2024-02-05 04:54:40.000000 libexe-20240205/libbfio/libbfio_codepage.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26845 2024-02-05 04:54:40.000000 libexe-20240205/libbfio/libbfio_file_io_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1448 2024-02-05 04:54:40.000000 libexe-20240205/libbfio/libbfio_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-02-05 04:54:40.000000 libexe-20240205/libbfio/libbfio_memory_range.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10798 2024-02-05 04:54:40.000000 libexe-20240205/libbfio/libbfio_file_pool.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4806 2024-02-05 04:54:40.000000 libexe-20240205/libbfio/libbfio_file_range_io_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1918 2024-02-05 04:54:40.000000 libexe-20240205/libbfio/libbfio_libcthreads.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2814 2024-02-05 04:54:40.000000 libexe-20240205/libbfio/libbfio_system_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21082 2024-02-05 04:54:40.000000 libexe-20240205/libbfio/libbfio_memory_range_io_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    64816 2024-02-05 04:54:40.000000 libexe-20240205/libbfio/libbfio_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10899 2024-02-05 04:54:40.000000 libexe-20240205/libbfio/libbfio_file.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8883 2024-02-05 04:54:40.000000 libexe-20240205/libbfio/libbfio_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5821 2024-02-05 04:54:40.000000 libexe-20240205/libbfio/libbfio_memory_range.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    81879 2024-02-05 04:54:40.000000 libexe-20240205/libbfio/libbfio_pool.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2024-02-05 04:54:40.000000 libexe-20240205/libbfio/libbfio_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32119 2024-02-05 04:55:06.000000 libexe-20240205/libbfio/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25540 2024-02-05 04:54:40.000000 libexe-20240205/libbfio/libbfio_system_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3835 2024-02-05 04:54:40.000000 libexe-20240205/libbfio/libbfio_memory_range_io_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1376 2024-02-05 04:54:40.000000 libexe-20240205/libbfio/libbfio_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6841 2024-02-05 04:54:40.000000 libexe-20240205/libbfio/libbfio_pool.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       67 2023-12-03 09:03:28.000000 libexe-20240205/ABOUT-NLS
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    49939 2024-02-05 04:55:06.000000 libexe-20240205/config.guess
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-05 05:07:25.000000 libexe-20240205/dpkg/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       27 2024-02-05 04:46:57.000000 libexe-20240205/dpkg/libexe-tools.install
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1022 2024-02-05 04:46:59.000000 libexe-20240205/dpkg/copyright
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-05 05:07:25.000000 libexe-20240205/dpkg/source/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       12 2024-02-05 04:46:57.000000 libexe-20240205/dpkg/source/format
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2006 2024-02-05 04:46:57.000000 libexe-20240205/dpkg/control
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      753 2024-02-05 04:46:57.000000 libexe-20240205/dpkg/rules
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       22 2024-02-05 04:46:57.000000 libexe-20240205/dpkg/libexe.install
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       96 2024-02-05 04:46:57.000000 libexe-20240205/dpkg/libexe-dev.install
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      119 2024-02-05 04:46:57.000000 libexe-20240205/dpkg/changelog.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      138 2024-02-05 04:55:15.000000 libexe-20240205/dpkg/changelog
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        3 2024-02-05 04:46:57.000000 libexe-20240205/dpkg/compat
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       18 2024-02-05 04:46:57.000000 libexe-20240205/dpkg/libexe-python3.install
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      480 2024-02-05 04:55:15.000000 libexe-20240205/setup.cfg
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7652 2024-02-05 04:46:57.000000 libexe-20240205/COPYING.LESSER
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)  1792166 2024-02-05 04:55:05.000000 libexe-20240205/configure
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     7400 2024-02-05 04:55:06.000000 libexe-20240205/compile
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     6878 2024-02-05 04:55:06.000000 libexe-20240205/missing
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-05 05:07:27.000000 libexe-20240205/msvscpp/
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-05 05:07:27.000000 libexe-20240205/msvscpp/libfdata/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6858 2024-02-05 04:47:20.000000 libexe-20240205/msvscpp/libfdata/libfdata.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-05 05:07:27.000000 libexe-20240205/msvscpp/libexe/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9678 2024-02-05 04:47:20.000000 libexe-20240205/msvscpp/libexe/libexe.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-05 05:07:27.000000 libexe-20240205/msvscpp/exe_test_error/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5491 2024-02-05 04:47:20.000000 libexe-20240205/msvscpp/exe_test_error/exe_test_error.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-05 05:07:27.000000 libexe-20240205/msvscpp/exeinfo/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6556 2024-02-05 04:47:20.000000 libexe-20240205/msvscpp/exeinfo/exeinfo.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-05 05:07:27.000000 libexe-20240205/msvscpp/exe_test_tools_info_handle/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5844 2024-02-05 04:47:20.000000 libexe-20240205/msvscpp/exe_test_tools_info_handle/exe_test_tools_info_handle.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-05 05:07:27.000000 libexe-20240205/msvscpp/exe_test_coff_optional_header/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5776 2024-02-05 04:47:52.000000 libexe-20240205/msvscpp/exe_test_coff_optional_header/exe_test_coff_optional_header.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-05 05:07:27.000000 libexe-20240205/msvscpp/libclocale/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4778 2024-02-05 04:47:20.000000 libexe-20240205/msvscpp/libclocale/libclocale.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-05 05:07:27.000000 libexe-20240205/msvscpp/exe_test_import_table/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5752 2024-02-05 04:47:20.000000 libexe-20240205/msvscpp/exe_test_import_table/exe_test_import_table.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-05 05:07:27.000000 libexe-20240205/msvscpp/libfcache/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5237 2024-02-05 04:47:20.000000 libexe-20240205/msvscpp/libfcache/libfcache.vcproj
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1659 2024-02-05 04:47:20.000000 libexe-20240205/msvscpp/Makefile.am
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-05 05:07:27.000000 libexe-20240205/msvscpp/libbfio/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7306 2024-02-05 04:47:20.000000 libexe-20240205/msvscpp/libbfio/libbfio.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-05 05:07:27.000000 libexe-20240205/msvscpp/exe_test_le_header/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5743 2024-02-05 04:47:52.000000 libexe-20240205/msvscpp/exe_test_le_header/exe_test_le_header.vcproj
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30356 2024-02-05 04:47:52.000000 libexe-20240205/msvscpp/libexe.sln
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-05 05:07:27.000000 libexe-20240205/msvscpp/exe_test_tools_signal/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5679 2024-02-05 04:47:20.000000 libexe-20240205/msvscpp/exe_test_tools_signal/exe_test_tools_signal.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-05 05:07:27.000000 libexe-20240205/msvscpp/exe_test_mz_header/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5743 2024-02-05 04:47:52.000000 libexe-20240205/msvscpp/exe_test_mz_header/exe_test_mz_header.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-05 05:07:27.000000 libexe-20240205/msvscpp/exe_test_support/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6384 2024-02-05 04:47:20.000000 libexe-20240205/msvscpp/exe_test_support/exe_test_support.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-05 05:07:27.000000 libexe-20240205/msvscpp/libcfile/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5597 2024-02-05 04:47:20.000000 libexe-20240205/msvscpp/libcfile/libcfile.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-05 05:07:27.000000 libexe-20240205/msvscpp/exe_test_debug_data/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5746 2024-02-05 04:47:20.000000 libexe-20240205/msvscpp/exe_test_debug_data/exe_test_debug_data.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-05 05:07:27.000000 libexe-20240205/msvscpp/exe_test_tools_output/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5679 2024-02-05 04:47:20.000000 libexe-20240205/msvscpp/exe_test_tools_output/exe_test_tools_output.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-05 05:07:27.000000 libexe-20240205/msvscpp/libcdata/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6172 2024-02-05 04:47:20.000000 libexe-20240205/msvscpp/libcdata/libcdata.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-05 05:07:27.000000 libexe-20240205/msvscpp/exe_test_io_handle/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5743 2024-02-05 04:47:20.000000 libexe-20240205/msvscpp/exe_test_io_handle/exe_test_io_handle.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-05 05:07:27.000000 libexe-20240205/msvscpp/exe_test_file/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6375 2024-02-05 04:47:20.000000 libexe-20240205/msvscpp/exe_test_file/exe_test_file.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-05 05:07:27.000000 libexe-20240205/msvscpp/exe_test_ne_header/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5743 2024-02-05 04:47:52.000000 libexe-20240205/msvscpp/exe_test_ne_header/exe_test_ne_header.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-05 05:07:27.000000 libexe-20240205/msvscpp/libcthreads/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6177 2024-02-05 04:47:20.000000 libexe-20240205/msvscpp/libcthreads/libcthreads.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-05 05:07:27.000000 libexe-20240205/msvscpp/exe_test_coff_header/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5749 2024-02-05 04:47:52.000000 libexe-20240205/msvscpp/exe_test_coff_header/exe_test_coff_header.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-05 05:07:27.000000 libexe-20240205/msvscpp/exe_test_data_directory_descriptor/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5791 2024-02-05 04:47:20.000000 libexe-20240205/msvscpp/exe_test_data_directory_descriptor/exe_test_data_directory_descriptor.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-05 05:07:27.000000 libexe-20240205/msvscpp/exe_test_notify/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5576 2024-02-05 04:47:20.000000 libexe-20240205/msvscpp/exe_test_notify/exe_test_notify.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-05 05:07:27.000000 libexe-20240205/msvscpp/libcpath/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5183 2024-02-05 04:47:20.000000 libexe-20240205/msvscpp/libcpath/libcpath.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-05 05:07:27.000000 libexe-20240205/msvscpp/exe_test_section_io_handle/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5767 2024-02-05 04:47:20.000000 libexe-20240205/msvscpp/exe_test_section_io_handle/exe_test_section_io_handle.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-05 05:07:27.000000 libexe-20240205/msvscpp/exe_test_section/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5737 2024-02-05 04:47:20.000000 libexe-20240205/msvscpp/exe_test_section/exe_test_section.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-05 05:07:27.000000 libexe-20240205/msvscpp/libcsplit/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5225 2024-02-05 04:47:20.000000 libexe-20240205/msvscpp/libcsplit/libcsplit.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-05 05:07:27.000000 libexe-20240205/msvscpp/libuna/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15387 2024-02-05 04:47:20.000000 libexe-20240205/msvscpp/libuna/libuna.vcproj
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22284 2024-02-05 04:55:06.000000 libexe-20240205/msvscpp/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-05 05:07:27.000000 libexe-20240205/msvscpp/pyexe/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6593 2024-02-05 04:47:52.000000 libexe-20240205/msvscpp/pyexe/pyexe.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-05 05:07:27.000000 libexe-20240205/msvscpp/libcnotify/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4764 2024-02-05 04:47:20.000000 libexe-20240205/msvscpp/libcnotify/libcnotify.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-05 05:07:27.000000 libexe-20240205/msvscpp/libcerror/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4488 2024-02-05 04:47:20.000000 libexe-20240205/msvscpp/libcerror/libcerror.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-05 05:07:27.000000 libexe-20240205/msvscpp/exe_test_section_descriptor/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5770 2024-02-05 04:47:20.000000 libexe-20240205/msvscpp/exe_test_section_descriptor/exe_test_section_descriptor.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-05 05:07:27.000000 libexe-20240205/msvscpp/libfdatetime/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6069 2024-02-05 04:47:20.000000 libexe-20240205/msvscpp/libfdatetime/libfdatetime.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-05 05:07:27.000000 libexe-20240205/msvscpp/exe_test_export_table/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5752 2024-02-05 04:47:20.000000 libexe-20240205/msvscpp/exe_test_export_table/exe_test_export_table.vcproj
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       90 2024-02-05 04:46:58.000000 libexe-20240205/AUTHORS
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-05 05:07:26.000000 libexe-20240205/libcfile/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-02-05 04:54:46.000000 libexe-20240205/libcfile/libcfile_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2389 2024-02-05 04:54:46.000000 libexe-20240205/libcfile/libcfile_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-02-05 04:54:46.000000 libexe-20240205/libcfile/libcfile_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1593 2024-02-05 04:54:46.000000 libexe-20240205/libcfile/libcfile_notify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25753 2024-02-05 04:54:46.000000 libexe-20240205/libcfile/libcfile_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1497 2024-02-05 04:54:46.000000 libexe-20240205/libcfile/libcfile_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      942 2024-02-05 04:54:46.000000 libexe-20240205/libcfile/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2754 2024-02-05 04:54:46.000000 libexe-20240205/libcfile/libcfile_notify.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2826 2024-02-05 04:54:46.000000 libexe-20240205/libcfile/libcfile_system_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6452 2024-02-05 04:54:46.000000 libexe-20240205/libcfile/libcfile_file.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-02-05 04:54:46.000000 libexe-20240205/libcfile/libcfile_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25560 2024-02-05 04:54:46.000000 libexe-20240205/libcfile/libcfile_system_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-02-05 04:54:46.000000 libexe-20240205/libcfile/libcfile_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-02-05 04:54:46.000000 libexe-20240205/libcfile/libcfile_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   105597 2024-02-05 04:54:46.000000 libexe-20240205/libcfile/libcfile_file.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2024-02-05 04:54:46.000000 libexe-20240205/libcfile/libcfile_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3107 2024-02-05 04:54:46.000000 libexe-20240205/libcfile/libcfile_winapi.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29424 2024-02-05 04:55:06.000000 libexe-20240205/libcfile/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-02-05 04:54:46.000000 libexe-20240205/libcfile/libcfile_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1736 2024-02-05 04:54:46.000000 libexe-20240205/libcfile/libcfile_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18388 2024-02-05 04:54:46.000000 libexe-20240205/libcfile/libcfile_winapi.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2879 2024-02-05 04:54:46.000000 libexe-20240205/libcfile/libcfile_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      574 2024-02-05 04:47:52.000000 libexe-20240205/README
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15766 2024-02-05 04:55:06.000000 libexe-20240205/INSTALL
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-05 05:07:26.000000 libexe-20240205/libcdata/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3871 2024-02-05 04:54:42.000000 libexe-20240205/libcdata/libcdata_list_element.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5231 2024-02-05 04:54:42.000000 libexe-20240205/libcdata/libcdata_array.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2115 2024-02-05 04:54:42.000000 libexe-20240205/libcdata/libcdata_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-02-05 04:54:42.000000 libexe-20240205/libcdata/libcdata_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-02-05 04:54:42.000000 libexe-20240205/libcdata/libcdata_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3790 2024-02-05 04:54:42.000000 libexe-20240205/libcdata/libcdata_btree.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22358 2024-02-05 04:54:42.000000 libexe-20240205/libcdata/libcdata_btree.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1152 2024-02-05 04:54:42.000000 libexe-20240205/libcdata/libcdata_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    69515 2024-02-05 04:54:42.000000 libexe-20240205/libcdata/libcdata_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-02-05 04:54:42.000000 libexe-20240205/libcdata/libcdata_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6448 2024-02-05 04:54:42.000000 libexe-20240205/libcdata/libcdata_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1648 2024-02-05 04:54:42.000000 libexe-20240205/libcdata/libcdata_btree_values_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1127 2024-02-05 04:54:42.000000 libexe-20240205/libcdata/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2960 2024-02-05 04:54:42.000000 libexe-20240205/libcdata/libcdata_btree_node.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2789 2024-02-05 04:54:42.000000 libexe-20240205/libcdata/libcdata_range_list_value.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12295 2024-02-05 04:54:42.000000 libexe-20240205/libcdata/libcdata_range_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   122285 2024-02-05 04:54:42.000000 libexe-20240205/libcdata/libcdata_range_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    49968 2024-02-05 04:54:42.000000 libexe-20240205/libcdata/libcdata_array.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23846 2024-02-05 04:54:42.000000 libexe-20240205/libcdata/libcdata_list_element.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1925 2024-02-05 04:54:42.000000 libexe-20240205/libcdata/libcdata_libcthreads.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8365 2024-02-05 04:54:42.000000 libexe-20240205/libcdata/libcdata_tree_node.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-02-05 04:54:42.000000 libexe-20240205/libcdata/libcdata_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1976 2024-02-05 04:54:42.000000 libexe-20240205/libcdata/libcdata_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37549 2024-02-05 04:54:42.000000 libexe-20240205/libcdata/libcdata_btree_node.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   100501 2024-02-05 04:54:42.000000 libexe-20240205/libcdata/libcdata_tree_node.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1230 2024-02-05 04:54:42.000000 libexe-20240205/libcdata/libcdata_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31108 2024-02-05 04:55:06.000000 libexe-20240205/libcdata/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10647 2024-02-05 04:54:42.000000 libexe-20240205/libcdata/libcdata_range_list_value.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5251 2024-02-05 04:54:42.000000 libexe-20240205/libcdata/libcdata_btree_values_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-02-05 04:54:42.000000 libexe-20240205/libcdata/libcdata_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       91 2024-02-05 04:46:57.000000 libexe-20240205/pyproject.toml
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      481 2024-02-05 04:46:57.000000 libexe-20240205/setup.cfg.in
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    35796 2024-02-05 04:55:06.000000 libexe-20240205/config.sub
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     9278 2024-02-05 04:46:57.000000 libexe-20240205/setup.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1196 2024-02-05 04:48:15.000000 libexe-20240205/acinclude.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2272 2024-02-05 04:55:15.000000 libexe-20240205/libexe.spec
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    18574 2023-12-03 09:03:28.000000 libexe-20240205/config.rpath
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-05 05:07:26.000000 libexe-20240205/libcthreads/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2356 2024-02-05 04:54:52.000000 libexe-20240205/libcthreads/libcthreads_thread.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3195 2024-02-05 04:54:52.000000 libexe-20240205/libcthreads/libcthreads_read_write_lock.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10198 2024-02-05 04:54:52.000000 libexe-20240205/libcthreads/libcthreads_thread.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4175 2024-02-05 04:54:52.000000 libexe-20240205/libcthreads/libcthreads_thread_pool.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1254 2024-02-05 04:54:52.000000 libexe-20240205/libcthreads/libcthreads_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2208 2024-02-05 04:54:52.000000 libexe-20240205/libcthreads/libcthreads_lock.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-02-05 04:54:52.000000 libexe-20240205/libcthreads/libcthreads_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8753 2024-02-05 04:54:52.000000 libexe-20240205/libcthreads/libcthreads_lock.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3040 2024-02-05 04:54:52.000000 libexe-20240205/libcthreads/libcthreads_condition.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2870 2024-02-05 04:54:52.000000 libexe-20240205/libcthreads/libcthreads_repeating_thread.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1171 2024-02-05 04:54:52.000000 libexe-20240205/libcthreads/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1170 2024-02-05 04:54:52.000000 libexe-20240205/libcthreads/libcthreads_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13601 2024-02-05 04:54:52.000000 libexe-20240205/libcthreads/libcthreads_mutex.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26519 2024-02-05 04:54:52.000000 libexe-20240205/libcthreads/libcthreads_queue.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2434 2024-02-05 04:54:52.000000 libexe-20240205/libcthreads/libcthreads_mutex.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2510 2024-02-05 04:54:52.000000 libexe-20240205/libcthreads/libcthreads_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2138 2024-02-05 04:54:52.000000 libexe-20240205/libcthreads/libcthreads_thread_attributes.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18281 2024-02-05 04:54:52.000000 libexe-20240205/libcthreads/libcthreads_condition.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2952 2024-02-05 04:54:52.000000 libexe-20240205/libcthreads/libcthreads_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18426 2024-02-05 04:54:52.000000 libexe-20240205/libcthreads/libcthreads_read_write_lock.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1447 2024-02-05 04:54:52.000000 libexe-20240205/libcthreads/libcthreads_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2128 2024-02-05 04:54:52.000000 libexe-20240205/libcthreads/libcthreads_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    43321 2024-02-05 04:54:52.000000 libexe-20240205/libcthreads/libcthreads_thread_pool.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1864 2024-02-05 04:54:52.000000 libexe-20240205/libcthreads/libcthreads_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4096 2024-02-05 04:54:52.000000 libexe-20240205/libcthreads/libcthreads_thread_attributes.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1428 2024-02-05 04:54:52.000000 libexe-20240205/libcthreads/libcthreads_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17481 2024-02-05 04:54:52.000000 libexe-20240205/libcthreads/libcthreads_repeating_thread.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31514 2024-02-05 04:55:06.000000 libexe-20240205/libcthreads/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3341 2024-02-05 04:54:52.000000 libexe-20240205/libcthreads/libcthreads_queue.h
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4879 2024-02-05 04:55:06.000000 libexe-20240205/test-driver
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-05 05:07:26.000000 libexe-20240205/libcpath/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2336 2024-02-05 04:54:49.000000 libexe-20240205/libcpath/libcpath_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-02-05 04:54:49.000000 libexe-20240205/libcpath/libcpath_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1990 2024-02-05 04:54:50.000000 libexe-20240205/libcpath/libcpath_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      842 2024-02-05 04:54:50.000000 libexe-20240205/libcpath/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-02-05 04:54:49.000000 libexe-20240205/libcpath/libcpath_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-02-05 04:54:49.000000 libexe-20240205/libcpath/libcpath_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2826 2024-02-05 04:54:49.000000 libexe-20240205/libcpath/libcpath_system_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1461 2024-02-05 04:54:49.000000 libexe-20240205/libcpath/libcpath_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1536 2024-02-05 04:54:49.000000 libexe-20240205/libcpath/libcpath_libcsplit.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25560 2024-02-05 04:54:49.000000 libexe-20240205/libcpath/libcpath_system_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2024-02-05 04:54:49.000000 libexe-20240205/libcpath/libcpath_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-02-05 04:54:49.000000 libexe-20240205/libcpath/libcpath_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28702 2024-02-05 04:55:06.000000 libexe-20240205/libcpath/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1736 2024-02-05 04:54:49.000000 libexe-20240205/libcpath/libcpath_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-02-05 04:54:49.000000 libexe-20240205/libcpath/libcpath_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   176165 2024-02-05 04:54:49.000000 libexe-20240205/libcpath/libcpath_path.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7170 2024-02-05 04:54:49.000000 libexe-20240205/libcpath/libcpath_path.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3094 2024-02-05 04:46:57.000000 libexe-20240205/libexe.spec.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      438 2023-12-03 09:03:28.000000 libexe-20240205/ChangeLog
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-05 05:07:27.000000 libexe-20240205/manuals/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2032 2024-02-05 04:46:59.000000 libexe-20240205/manuals/exeinfo.1
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      150 2023-12-03 09:03:42.000000 libexe-20240205/manuals/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6064 2024-02-05 04:46:59.000000 libexe-20240205/manuals/libexe.3
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25619 2024-02-05 04:55:06.000000 libexe-20240205/manuals/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-05 05:07:27.000000 libexe-20240205/tests/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1527 2024-02-05 04:46:59.000000 libexe-20240205/tests/exe_test_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1703 2024-02-05 04:46:59.000000 libexe-20240205/tests/exe_test_libbfio.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5939 2024-02-05 04:47:52.000000 libexe-20240205/tests/exe_test_mz_header.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4077 2024-02-05 04:46:59.000000 libexe-20240205/tests/exe_test_tools_signal.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5546 2024-02-05 04:46:59.000000 libexe-20240205/tests/exe_test_tools_info_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6627 2024-02-05 04:46:59.000000 libexe-20240205/tests/exe_test_coff_optional_header.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3012 2024-02-05 04:47:52.000000 libexe-20240205/tests/exe_test_section_io_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34387 2024-02-05 04:46:59.000000 libexe-20240205/tests/exe_test_file.c
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4062 2024-02-05 04:48:30.000000 libexe-20240205/tests/test_tools.sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8356 2024-02-05 04:46:59.000000 libexe-20240205/tests/exe_test_io_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5939 2024-02-05 04:47:52.000000 libexe-20240205/tests/exe_test_ne_header.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7650 2024-02-05 04:47:52.000000 libexe-20240205/tests/exe_test_export_table.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1736 2024-02-05 04:46:59.000000 libexe-20240205/tests/exe_test_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1680 2024-02-05 04:46:59.000000 libexe-20240205/tests/exe_test_memory.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      965 2024-02-05 04:46:59.000000 libexe-20240205/tests/exe_test_libexe.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7295 2024-02-05 04:47:52.000000 libexe-20240205/tests/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4229 2024-02-05 04:46:59.000000 libexe-20240205/tests/exe_test_notify.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6105 2024-02-05 04:46:59.000000 libexe-20240205/tests/exe_test_coff_header.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8609 2024-02-05 04:47:52.000000 libexe-20240205/tests/exe_test_section_descriptor.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7650 2024-02-05 04:47:52.000000 libexe-20240205/tests/exe_test_import_table.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3408 2024-02-05 04:48:15.000000 libexe-20240205/tests/pyexe_test_support.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1794 2024-02-05 04:46:59.000000 libexe-20240205/tests/exe_test_functions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3059 2024-02-05 04:46:59.000000 libexe-20240205/tests/exe_test_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-02-05 04:46:59.000000 libexe-20240205/tests/exe_test_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14071 2024-02-05 04:46:59.000000 libexe-20240205/tests/exe_test_support.c
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     1653 2024-02-05 04:46:59.000000 libexe-20240205/tests/test_manpage.sh
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4070 2024-02-05 04:46:59.000000 libexe-20240205/tests/test_python_module.sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6001 2024-02-05 04:46:59.000000 libexe-20240205/tests/exe_test_le_header.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7490 2024-02-05 04:47:52.000000 libexe-20240205/tests/exe_test_debug_data.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-02-05 04:46:59.000000 libexe-20240205/tests/exe_test_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33607 2024-02-05 04:46:59.000000 libexe-20240205/tests/test_runner.sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4527 2024-02-05 04:46:59.000000 libexe-20240205/tests/exe_test_getopt.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2024-02-05 04:46:59.000000 libexe-20240205/tests/exe_test_libclocale.h
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     3306 2024-02-05 04:46:59.000000 libexe-20240205/tests/test_exeinfo.sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13235 2024-02-05 04:46:59.000000 libexe-20240205/tests/exe_test_functions.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4606 2024-02-05 04:46:59.000000 libexe-20240205/tests/exe_test_memory.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2403 2024-02-05 04:46:59.000000 libexe-20240205/tests/exe_test_tools_output.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1573 2024-02-05 04:46:59.000000 libexe-20240205/tests/exe_test_data_directory_descriptor.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3704 2024-02-05 04:47:52.000000 libexe-20240205/tests/exe_test_section.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    65262 2024-02-05 04:55:06.000000 libexe-20240205/tests/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1803 2024-02-05 04:46:59.000000 libexe-20240205/tests/exe_test_getopt.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5731 2024-02-05 04:46:59.000000 libexe-20240205/tests/pyexe_test_file.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8504 2024-02-05 04:46:59.000000 libexe-20240205/tests/exe_test_macros.h
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4207 2024-02-05 04:48:30.000000 libexe-20240205/tests/test_library.sh
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-05 05:07:27.000000 libexe-20240205/ossfuzz/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      962 2024-02-05 04:46:59.000000 libexe-20240205/ossfuzz/ossfuzz_libexe.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      886 2023-12-03 09:03:29.000000 libexe-20240205/ossfuzz/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1739 2024-02-05 04:46:59.000000 libexe-20240205/ossfuzz/ossfuzz_libbfio.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2184 2024-02-05 04:46:59.000000 libexe-20240205/ossfuzz/file_fuzzer.cc
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30850 2024-02-05 04:55:06.000000 libexe-20240205/ossfuzz/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   332808 2024-02-05 04:55:02.000000 libexe-20240205/ltmain.sh
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-05 05:07:26.000000 libexe-20240205/libcsplit/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6125 2024-02-05 04:54:51.000000 libexe-20240205/libcsplit/libcsplit_narrow_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1360 2024-02-05 04:54:51.000000 libexe-20240205/libcsplit/libcsplit_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1679 2024-02-05 04:54:51.000000 libexe-20240205/libcsplit/libcsplit_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13944 2024-02-05 04:54:51.000000 libexe-20240205/libcsplit/libcsplit_wide_split_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2024-02-05 04:54:51.000000 libexe-20240205/libcsplit/libcsplit_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      884 2024-02-05 04:54:51.000000 libexe-20240205/libcsplit/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-02-05 04:54:51.000000 libexe-20240205/libcsplit/libcsplit_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6206 2024-02-05 04:54:51.000000 libexe-20240205/libcsplit/libcsplit_wide_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-02-05 04:54:51.000000 libexe-20240205/libcsplit/libcsplit_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2920 2024-02-05 04:54:51.000000 libexe-20240205/libcsplit/libcsplit_wide_split_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2924 2024-02-05 04:54:51.000000 libexe-20240205/libcsplit/libcsplit_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13912 2024-02-05 04:54:51.000000 libexe-20240205/libcsplit/libcsplit_narrow_split_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-02-05 04:54:51.000000 libexe-20240205/libcsplit/libcsplit_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-02-05 04:54:51.000000 libexe-20240205/libcsplit/libcsplit_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1158 2024-02-05 04:54:51.000000 libexe-20240205/libcsplit/libcsplit_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1471 2024-02-05 04:54:51.000000 libexe-20240205/libcsplit/libcsplit_wide_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29482 2024-02-05 04:55:06.000000 libexe-20240205/libcsplit/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2849 2024-02-05 04:54:51.000000 libexe-20240205/libcsplit/libcsplit_narrow_split_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1386 2024-02-05 04:54:51.000000 libexe-20240205/libcsplit/libcsplit_narrow_string.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-05 05:07:27.000000 libexe-20240205/po/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      720 2023-12-03 09:03:44.000000 libexe-20240205/po/remove-potcdate.sin
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       59 2023-12-03 09:03:44.000000 libexe-20240205/po/POTFILES.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19571 2023-12-03 09:03:44.000000 libexe-20240205/po/Makefile.in.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      153 2023-12-03 09:03:44.000000 libexe-20240205/po/quot.sed
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1204 2023-12-03 09:03:44.000000 libexe-20240205/po/en@quot.header
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1338 2023-12-03 09:03:44.000000 libexe-20240205/po/en@boldquot.header
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      217 2023-12-03 09:03:44.000000 libexe-20240205/po/boldquot.sed
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      906 2023-12-03 09:03:44.000000 libexe-20240205/po/insert-header.sin
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       50 2023-12-03 09:03:44.000000 libexe-20240205/po/ChangeLog
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1852 2024-02-05 04:55:15.000000 libexe-20240205/po/Makevars
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1852 2023-12-03 09:03:43.000000 libexe-20240205/po/Makevars.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2395 2023-12-03 09:03:44.000000 libexe-20240205/po/Rules-quot
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-05 05:07:26.000000 libexe-20240205/libuna/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8811 2024-02-05 04:54:58.000000 libexe-20240205/libuna/libuna_codepage_windows_1251.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    98308 2024-02-05 04:54:58.000000 libexe-20240205/libuna/libuna_utf16_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39461 2024-02-05 04:54:58.000000 libexe-20240205/libuna/libuna_base16_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2993 2024-02-05 04:54:58.000000 libexe-20240205/libuna/libuna_utf8_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1567 2024-02-05 04:54:58.000000 libexe-20240205/libuna/libuna_codepage_iso_8859_2.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   286239 2024-02-05 04:54:58.000000 libexe-20240205/libuna/libuna_codepage_windows_932.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-02-05 04:54:58.000000 libexe-20240205/libuna/libuna_codepage_mac_dingbats.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   101450 2024-02-05 04:54:58.000000 libexe-20240205/libuna/libuna_utf8_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    74767 2024-02-05 04:54:58.000000 libexe-20240205/libuna/libuna_base64_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1749 2024-02-05 04:54:58.000000 libexe-20240205/libuna/libuna_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1610 2024-02-05 04:54:58.000000 libexe-20240205/libuna/libuna_codepage_mac_turkish.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   156918 2024-02-05 04:54:58.000000 libexe-20240205/libuna/libuna_unicode_character.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10379 2024-02-05 04:54:58.000000 libexe-20240205/libuna/libuna_codepage_mac_gaelic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-02-05 04:54:58.000000 libexe-20240205/libuna/libuna_codepage_mac_arabic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9435 2024-02-05 04:54:58.000000 libexe-20240205/libuna/libuna_codepage_mac_thai.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1618 2024-02-05 04:54:58.000000 libexe-20240205/libuna/libuna_codepage_windows_874.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1346 2024-02-05 04:54:58.000000 libexe-20240205/libuna/libuna_codepage_iso_8859_15.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9666 2024-02-05 04:54:58.000000 libexe-20240205/libuna/libuna_utf8_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3296 2024-02-05 04:54:58.000000 libexe-20240205/libuna/libuna_codepage_iso_8859_16.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9211 2024-02-05 04:54:58.000000 libexe-20240205/libuna/libuna_codepage_windows_1255.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15691 2024-02-05 04:54:58.000000 libexe-20240205/libuna/libuna_utf7_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2921 2024-02-05 04:54:58.000000 libexe-20240205/libuna/libuna_byte_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9984 2024-02-05 04:54:58.000000 libexe-20240205/libuna/libuna_codepage_koi8_u.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1392 2024-02-05 04:54:58.000000 libexe-20240205/libuna/libuna_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2540 2024-02-05 04:54:58.000000 libexe-20240205/libuna/libuna_codepage_iso_8859_6.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2823 2024-02-05 04:54:58.000000 libexe-20240205/libuna/libuna_codepage_iso_8859_14.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3679 2024-02-05 04:54:58.000000 libexe-20240205/libuna/libuna_base64_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2882 2024-02-05 04:54:58.000000 libexe-20240205/libuna/libuna_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1658 2024-02-05 04:54:58.000000 libexe-20240205/libuna/libuna_codepage_mac_centraleurroman.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9953 2024-02-05 04:54:58.000000 libexe-20240205/libuna/libuna_codepage_mac_romanian.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1339 2024-02-05 04:54:58.000000 libexe-20240205/libuna/libuna_codepage_iso_8859_6.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2053 2024-02-05 04:54:58.000000 libexe-20240205/libuna/libuna_codepage_iso_8859_9.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1610 2024-02-05 04:54:58.000000 libexe-20240205/libuna/libuna_codepage_mac_russian.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10134 2024-02-05 04:54:58.000000 libexe-20240205/libuna/libuna_codepage_mac_dingbats.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2024-02-05 04:54:58.000000 libexe-20240205/libuna/libuna_codepage_iso_8859_15.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   430461 2024-02-05 04:54:58.000000 libexe-20240205/libuna/libuna_codepage_windows_936.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-02-05 04:54:58.000000 libexe-20240205/libuna/libuna_codepage_mac_croatian.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1259 2024-02-05 04:54:58.000000 libexe-20240205/libuna/libuna_scsu.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4197 2024-02-05 04:54:58.000000 libexe-20240205/libuna/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20049 2024-02-05 04:54:58.000000 libexe-20240205/libuna/libuna_utf32_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1830 2024-02-05 04:54:58.000000 libexe-20240205/libuna/libuna_codepage_windows_936.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3225 2024-02-05 04:54:58.000000 libexe-20240205/libuna/libuna_codepage_iso_8859_10.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9745 2024-02-05 04:54:58.000000 libexe-20240205/libuna/libuna_codepage_mac_roman.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2808 2024-02-05 04:54:58.000000 libexe-20240205/libuna/libuna_utf7_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1773 2024-02-05 04:54:58.000000 libexe-20240205/libuna/libuna_codepage_iso_8859_3.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1787 2024-02-05 04:54:58.000000 libexe-20240205/libuna/libuna_codepage_mac_thai.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-02-05 04:54:58.000000 libexe-20240205/libuna/libuna_codepage_mac_farsi.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9088 2024-02-05 04:54:58.000000 libexe-20240205/libuna/libuna_codepage_mac_ukrainian.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10880 2024-02-05 04:54:58.000000 libexe-20240205/libuna/libuna_codepage_mac_inuit.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1830 2024-02-05 04:54:58.000000 libexe-20240205/libuna/libuna_codepage_windows_932.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8050 2024-02-05 04:54:58.000000 libexe-20240205/libuna/libuna_codepage_windows_874.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2738 2024-02-05 04:54:58.000000 libexe-20240205/libuna/libuna_codepage_iso_8859_5.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-02-05 04:54:58.000000 libexe-20240205/libuna/libuna_codepage_iso_8859_10.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16705 2024-02-05 04:54:58.000000 libexe-20240205/libuna/libuna_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1929 2024-02-05 04:54:58.000000 libexe-20240205/libuna/libuna_url_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1622 2024-02-05 04:54:58.000000 libexe-20240205/libuna/libuna_codepage_mac_icelandic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1602 2024-02-05 04:54:58.000000 libexe-20240205/libuna/libuna_codepage_koi8_u.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19850 2024-02-05 04:54:58.000000 libexe-20240205/libuna/libuna_utf16_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8602 2024-02-05 04:54:58.000000 libexe-20240205/libuna/libuna_codepage_windows_1253.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1449 2024-02-05 04:54:58.000000 libexe-20240205/libuna/libuna_codepage_iso_8859_4.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9078 2024-02-05 04:54:58.000000 libexe-20240205/libuna/libuna_codepage_mac_greek.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-02-05 04:54:58.000000 libexe-20240205/libuna/libuna_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9394 2024-02-05 04:54:58.000000 libexe-20240205/libuna/libuna_codepage_mac_centraleurroman.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8997 2024-02-05 04:54:58.000000 libexe-20240205/libuna/libuna_codepage_windows_1254.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1455 2024-02-05 04:54:58.000000 libexe-20240205/libuna/libuna_codepage_iso_8859_13.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1447 2024-02-05 04:54:58.000000 libexe-20240205/libuna/libuna_codepage_iso_8859_7.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-02-05 04:54:58.000000 libexe-20240205/libuna/libuna_codepage_windows_1255.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8000 2024-02-05 04:54:58.000000 libexe-20240205/libuna/libuna_unicode_character.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1448 2024-02-05 04:54:58.000000 libexe-20240205/libuna/libuna_codepage_iso_8859_8.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3664 2024-02-05 04:54:58.000000 libexe-20240205/libuna/libuna_codepage_iso_8859_13.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-02-05 04:54:58.000000 libexe-20240205/libuna/libuna_codepage_windows_949.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9125 2024-02-05 04:54:58.000000 libexe-20240205/libuna/libuna_codepage_mac_cyrillic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9871 2024-02-05 04:54:58.000000 libexe-20240205/libuna/libuna_codepage_mac_celtic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1234 2024-02-05 04:54:58.000000 libexe-20240205/libuna/libuna_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3561 2024-02-05 04:54:58.000000 libexe-20240205/libuna/libuna_codepage_iso_8859_4.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   484762 2024-02-05 04:54:58.000000 libexe-20240205/libuna/libuna_codepage_windows_949.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3106 2024-02-05 04:54:58.000000 libexe-20240205/libuna/libuna_utf16_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14020 2024-02-05 04:54:58.000000 libexe-20240205/libuna/libuna_codepage_mac_symbol.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-02-05 04:54:58.000000 libexe-20240205/libuna/libuna_codepage_mac_roman.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9076 2024-02-05 04:54:58.000000 libexe-20240205/libuna/libuna_codepage_windows_1257.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1627 2024-02-05 04:54:58.000000 libexe-20240205/libuna/libuna_codepage_windows_1254.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   360710 2024-02-05 04:54:58.000000 libexe-20240205/libuna/libuna_codepage_windows_950.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1363 2024-02-05 04:54:58.000000 libexe-20240205/libuna/libuna_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10005 2024-02-05 04:54:58.000000 libexe-20240205/libuna/libuna_codepage_windows_1256.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1521 2024-02-05 04:54:58.000000 libexe-20240205/libuna/libuna_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3704 2024-02-05 04:54:58.000000 libexe-20240205/libuna/libuna_base32_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1625 2024-02-05 04:54:58.000000 libexe-20240205/libuna/libuna_codepage_windows_1253.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1783 2024-02-05 04:54:58.000000 libexe-20240205/libuna/libuna_codepage_iso_8859_16.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18019 2024-02-05 04:54:58.000000 libexe-20240205/libuna/libuna_utf8_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1636 2024-02-05 04:54:58.000000 libexe-20240205/libuna/libuna_codepage_windows_1250.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3610 2024-02-05 04:54:58.000000 libexe-20240205/libuna/libuna_codepage_iso_8859_2.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1140 2024-02-05 04:54:58.000000 libexe-20240205/libuna/libuna_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9542 2024-02-05 04:54:58.000000 libexe-20240205/libuna/libuna_codepage_koi8_r.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1341 2024-02-05 04:54:58.000000 libexe-20240205/libuna/libuna_codepage_iso_8859_5.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9656 2024-02-05 04:54:58.000000 libexe-20240205/libuna/libuna_utf16_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    94606 2024-02-05 04:54:58.000000 libexe-20240205/libuna/libuna_utf32_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9656 2024-02-05 04:54:58.000000 libexe-20240205/libuna/libuna_codepage_mac_icelandic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-02-05 04:54:58.000000 libexe-20240205/libuna/libuna_codepage_windows_1256.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9526 2024-02-05 04:54:58.000000 libexe-20240205/libuna/libuna_utf32_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-02-05 04:54:58.000000 libexe-20240205/libuna/libuna_codepage_mac_romanian.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2629 2024-02-05 04:54:58.000000 libexe-20240205/libuna/libuna_codepage_iso_8859_8.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1600 2024-02-05 04:54:58.000000 libexe-20240205/libuna/libuna_codepage_koi8_r.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-02-05 04:54:58.000000 libexe-20240205/libuna/libuna_codepage_mac_cyrillic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10389 2024-02-05 04:54:58.000000 libexe-20240205/libuna/libuna_codepage_mac_arabic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9776 2024-02-05 04:54:58.000000 libexe-20240205/libuna/libuna_codepage_mac_croatian.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1340 2024-02-05 04:54:58.000000 libexe-20240205/libuna/libuna_codepage_iso_8859_9.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-02-05 04:54:58.000000 libexe-20240205/libuna/libuna_codepage_mac_greek.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1630 2024-02-05 04:54:58.000000 libexe-20240205/libuna/libuna_codepage_windows_1258.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2873 2024-02-05 04:54:58.000000 libexe-20240205/libuna/libuna_codepage_iso_8859_7.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    52226 2024-02-05 04:55:06.000000 libexe-20240205/libuna/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3335 2024-02-05 04:54:58.000000 libexe-20240205/libuna/libuna_codepage_iso_8859_3.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9776 2024-02-05 04:54:58.000000 libexe-20240205/libuna/libuna_codepage_windows_1250.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3181 2024-02-05 04:54:58.000000 libexe-20240205/libuna/libuna_scsu.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7189 2024-02-05 04:54:58.000000 libexe-20240205/libuna/libuna_codepage_windows_1252.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9844 2024-02-05 04:54:58.000000 libexe-20240205/libuna/libuna_codepage_mac_turkish.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1622 2024-02-05 04:54:58.000000 libexe-20240205/libuna/libuna_codepage_mac_ukrainian.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8997 2024-02-05 04:54:58.000000 libexe-20240205/libuna/libuna_codepage_mac_russian.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9116 2024-02-05 04:54:58.000000 libexe-20240205/libuna/libuna_codepage_windows_1258.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-02-05 04:54:58.000000 libexe-20240205/libuna/libuna_codepage_mac_celtic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15485 2024-02-05 04:54:58.000000 libexe-20240205/libuna/libuna_byte_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-02-05 04:54:58.000000 libexe-20240205/libuna/libuna_codepage_mac_gaelic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3106 2024-02-05 04:54:58.000000 libexe-20240205/libuna/libuna_utf32_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1801 2024-02-05 04:54:58.000000 libexe-20240205/libuna/libuna_codepage_mac_symbol.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-02-05 04:54:58.000000 libexe-20240205/libuna/libuna_codepage_windows_1257.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-02-05 04:54:58.000000 libexe-20240205/libuna/libuna_codepage_mac_inuit.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11002 2024-02-05 04:54:58.000000 libexe-20240205/libuna/libuna_codepage_mac_farsi.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2024-02-05 04:54:58.000000 libexe-20240205/libuna/libuna_codepage_windows_950.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15532 2024-02-05 04:54:58.000000 libexe-20240205/libuna/libuna_url_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1628 2024-02-05 04:54:58.000000 libexe-20240205/libuna/libuna_codepage_windows_1251.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1644 2024-02-05 04:54:58.000000 libexe-20240205/libuna/libuna_codepage_windows_1252.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1563 2024-02-05 04:54:58.000000 libexe-20240205/libuna/libuna_codepage_iso_8859_14.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2623 2024-02-05 04:54:58.000000 libexe-20240205/libuna/libuna_base16_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    82226 2024-02-05 04:54:58.000000 libexe-20240205/libuna/libuna_base32_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39589 2024-02-05 04:55:06.000000 libexe-20240205/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-05 05:07:27.000000 libexe-20240205/pyexe/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3161 2024-02-05 04:48:15.000000 libexe-20240205/pyexe/pyexe_file.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2357 2024-02-05 04:46:59.000000 libexe-20240205/pyexe/pyexe_sections.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33702 2024-02-05 04:46:59.000000 libexe-20240205/pyexe/pyexe_file_object_io_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16577 2024-02-05 04:46:59.000000 libexe-20240205/pyexe/pyexe_datetime.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1429 2024-02-05 04:46:59.000000 libexe-20240205/pyexe/pyexe_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2751 2024-02-05 04:48:15.000000 libexe-20240205/pyexe/pyexe_section.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1136 2024-02-05 04:46:59.000000 libexe-20240205/pyexe/pyexe_codepage.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1519 2024-02-05 04:46:59.000000 libexe-20240205/pyexe/pyexe_libbfio.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1172 2023-12-03 09:03:43.000000 libexe-20240205/pyexe/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9506 2024-02-05 04:46:59.000000 libexe-20240205/pyexe/pyexe_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1384 2024-02-05 04:46:59.000000 libexe-20240205/pyexe/pyexe_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14606 2024-02-05 04:46:59.000000 libexe-20240205/pyexe/pyexe.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1526 2024-02-05 04:46:59.000000 libexe-20240205/pyexe/pyexe_integer.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      957 2024-02-05 04:46:59.000000 libexe-20240205/pyexe/pyexe_libexe.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2027 2024-02-05 04:46:59.000000 libexe-20240205/pyexe/pyexe_python.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1450 2024-02-05 04:46:59.000000 libexe-20240205/pyexe/pyexe_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1834 2024-02-05 04:46:59.000000 libexe-20240205/pyexe/pyexe.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8840 2024-02-05 04:46:59.000000 libexe-20240205/pyexe/pyexe_integer.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3218 2024-02-05 04:46:59.000000 libexe-20240205/pyexe/pyexe_codepage.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4042 2024-02-05 04:46:59.000000 libexe-20240205/pyexe/pyexe_file_object_io_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29879 2024-02-05 04:48:15.000000 libexe-20240205/pyexe/pyexe_file.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9121 2024-02-05 04:46:59.000000 libexe-20240205/pyexe/pyexe_sections.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1804 2024-02-05 04:46:59.000000 libexe-20240205/pyexe/pyexe_datetime.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21141 2024-02-05 04:48:15.000000 libexe-20240205/pyexe/pyexe_section.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    43260 2024-02-05 04:55:06.000000 libexe-20240205/pyexe/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1522 2024-02-05 04:46:59.000000 libexe-20240205/pyexe/pyexe_error.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-05 05:07:26.000000 libexe-20240205/libcnotify/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1548 2024-02-05 04:54:48.000000 libexe-20240205/libcnotify/libcnotify_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1415 2024-02-05 04:54:48.000000 libexe-20240205/libcnotify/libcnotify_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1164 2024-02-05 04:54:48.000000 libexe-20240205/libcnotify/libcnotify_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1439 2024-02-05 04:54:48.000000 libexe-20240205/libcnotify/libcnotify_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      728 2024-02-05 04:54:48.000000 libexe-20240205/libcnotify/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2024-02-05 04:54:48.000000 libexe-20240205/libcnotify/libcnotify_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1290 2024-02-05 04:54:48.000000 libexe-20240205/libcnotify/libcnotify_verbose.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1722 2024-02-05 04:54:48.000000 libexe-20240205/libcnotify/libcnotify_print.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4018 2024-02-05 04:54:48.000000 libexe-20240205/libcnotify/libcnotify_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1266 2024-02-05 04:54:48.000000 libexe-20240205/libcnotify/libcnotify_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1094 2024-02-05 04:54:48.000000 libexe-20240205/libcnotify/libcnotify_verbose.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28536 2024-02-05 04:55:06.000000 libexe-20240205/libcnotify/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1365 2024-02-05 04:54:48.000000 libexe-20240205/libcnotify/libcnotify_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8166 2024-02-05 04:54:48.000000 libexe-20240205/libcnotify/libcnotify_print.c
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-05 05:07:26.000000 libexe-20240205/libcerror/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15420 2024-02-05 04:54:43.000000 libexe-20240205/libcerror/libcerror_system.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19408 2024-02-05 04:54:43.000000 libexe-20240205/libcerror/libcerror_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-02-05 04:54:43.000000 libexe-20240205/libcerror/libcerror_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      640 2024-02-05 04:54:43.000000 libexe-20240205/libcerror/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1522 2024-02-05 04:54:43.000000 libexe-20240205/libcerror/libcerror_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2024-02-05 04:54:43.000000 libexe-20240205/libcerror/libcerror_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2880 2024-02-05 04:54:43.000000 libexe-20240205/libcerror/libcerror_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2026 2024-02-05 04:54:43.000000 libexe-20240205/libcerror/libcerror_system.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7629 2024-02-05 04:54:43.000000 libexe-20240205/libcerror/libcerror_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1158 2024-02-05 04:54:43.000000 libexe-20240205/libcerror/libcerror_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-02-05 04:54:43.000000 libexe-20240205/libcerror/libcerror_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28049 2024-02-05 04:55:06.000000 libexe-20240205/libcerror/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-05 05:07:26.000000 libexe-20240205/libfdatetime/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5406 2024-02-05 04:54:55.000000 libexe-20240205/libfdatetime/libfdatetime_floatingtime.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34352 2024-02-05 04:54:55.000000 libexe-20240205/libfdatetime/libfdatetime_nsf_timedate.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1887 2024-02-05 04:54:55.000000 libexe-20240205/libfdatetime/libfdatetime_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33399 2024-02-05 04:54:55.000000 libexe-20240205/libfdatetime/libfdatetime_floatingtime.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1220 2024-02-05 04:54:55.000000 libexe-20240205/libfdatetime/libfdatetime_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5010 2024-02-05 04:54:55.000000 libexe-20240205/libfdatetime/libfdatetime_hfs_time.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4182 2024-02-05 04:54:55.000000 libexe-20240205/libfdatetime/libfdatetime_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31774 2024-02-05 04:54:55.000000 libexe-20240205/libfdatetime/libfdatetime_hfs_time.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1148 2024-02-05 04:54:55.000000 libexe-20240205/libfdatetime/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35109 2024-02-05 04:54:55.000000 libexe-20240205/libfdatetime/libfdatetime_filetime.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4993 2024-02-05 04:54:55.000000 libexe-20240205/libfdatetime/libfdatetime_systemtime.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-02-05 04:54:55.000000 libexe-20240205/libfdatetime/libfdatetime_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    50166 2024-02-05 04:54:55.000000 libexe-20240205/libfdatetime/libfdatetime_posix_time.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1440 2024-02-05 04:54:55.000000 libexe-20240205/libfdatetime/libfdatetime_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5342 2024-02-05 04:54:55.000000 libexe-20240205/libfdatetime/libfdatetime_fat_date_time.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    41822 2024-02-05 04:54:55.000000 libexe-20240205/libfdatetime/libfdatetime_systemtime.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5761 2024-02-05 04:54:55.000000 libexe-20240205/libfdatetime/libfdatetime_nsf_timedate.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1450 2024-02-05 04:54:55.000000 libexe-20240205/libfdatetime/libfdatetime_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1154 2024-02-05 04:54:55.000000 libexe-20240205/libfdatetime/libfdatetime_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2966 2024-02-05 04:54:55.000000 libexe-20240205/libfdatetime/libfdatetime_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5771 2024-02-05 04:54:55.000000 libexe-20240205/libfdatetime/libfdatetime_posix_time.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3131 2024-02-05 04:54:55.000000 libexe-20240205/libfdatetime/libfdatetime_date_time_values.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5340 2024-02-05 04:54:55.000000 libexe-20240205/libfdatetime/libfdatetime_filetime.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    53085 2024-02-05 04:54:55.000000 libexe-20240205/libfdatetime/libfdatetime_date_time_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2468 2024-02-05 04:54:55.000000 libexe-20240205/libfdatetime/libfdatetime_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31275 2024-02-05 04:55:06.000000 libexe-20240205/libfdatetime/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31754 2024-02-05 04:54:55.000000 libexe-20240205/libfdatetime/libfdatetime_fat_date_time.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    56769 2024-02-05 04:55:04.000000 libexe-20240205/aclocal.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7147 2024-02-05 04:46:57.000000 libexe-20240205/configure.ac
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      412 2024-02-05 05:07:27.971650 libexe-20240205/PKG-INFO
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-20 19:41:16.000000 libexe-20240420/
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-20 19:41:14.000000 libexe-20240420/libfdata/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-04-20 18:01:27.000000 libexe-20240420/libfdata/libfdata_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37893 2024-04-20 18:01:27.000000 libexe-20240420/libfdata/libfdata_area.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9700 2024-04-20 18:01:27.000000 libexe-20240420/libfdata/libfdata_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1491 2024-04-20 18:01:27.000000 libexe-20240420/libfdata/libfdata_cache.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30931 2024-04-20 18:01:27.000000 libexe-20240420/libfdata/libfdata_range_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6826 2024-04-20 18:01:27.000000 libexe-20240420/libfdata/libfdata_mapped_range.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-04-20 18:01:27.000000 libexe-20240420/libfdata/libfdata_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6533 2024-04-20 18:01:27.000000 libexe-20240420/libfdata/libfdata_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   107689 2024-04-20 18:01:27.000000 libexe-20240420/libfdata/libfdata_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1548 2024-04-20 18:01:27.000000 libexe-20240420/libfdata/libfdata_libcdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12090 2024-04-20 18:01:27.000000 libexe-20240420/libfdata/libfdata_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4017 2024-04-20 18:01:27.000000 libexe-20240420/libfdata/libfdata_list_element.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1287 2024-04-20 18:01:27.000000 libexe-20240420/libfdata/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-04-20 18:01:27.000000 libexe-20240420/libfdata/libfdata_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-04-20 18:01:27.000000 libexe-20240420/libfdata/libfdata_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2754 2024-04-20 18:01:27.000000 libexe-20240420/libfdata/libfdata_notify.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1658 2024-04-20 18:01:27.000000 libexe-20240420/libfdata/libfdata_cache.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    66203 2024-04-20 18:01:27.000000 libexe-20240420/libfdata/libfdata_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-04-20 18:01:27.000000 libexe-20240420/libfdata/libfdata_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2092 2024-04-20 18:01:27.000000 libexe-20240420/libfdata/libfdata_range.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7327 2024-04-20 18:01:27.000000 libexe-20240420/libfdata/libfdata_area.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-04-20 18:01:27.000000 libexe-20240420/libfdata/libfdata_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1230 2024-04-20 18:01:27.000000 libexe-20240420/libfdata/libfdata_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7149 2024-04-20 18:01:27.000000 libexe-20240420/libfdata/libfdata_range.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1995 2024-04-20 18:01:27.000000 libexe-20240420/libfdata/libfdata_mapped_range.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1172 2024-04-20 18:01:27.000000 libexe-20240420/libfdata/libfdata_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19329 2024-04-20 18:01:27.000000 libexe-20240420/libfdata/libfdata_list_element.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21271 2024-04-20 18:01:27.000000 libexe-20240420/libfdata/libfdata_segments_array.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2054 2024-04-20 18:01:27.000000 libexe-20240420/libfdata/libfdata_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1593 2024-04-20 18:01:27.000000 libexe-20240420/libfdata/libfdata_notify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6013 2024-04-20 18:01:27.000000 libexe-20240420/libfdata/libfdata_range_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2804 2024-04-20 18:01:27.000000 libexe-20240420/libfdata/libfdata_segments_array.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32453 2024-04-20 18:01:54.000000 libexe-20240420/libfdata/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    49670 2024-04-20 18:01:27.000000 libexe-20240420/libfdata/libfdata_vector.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-04-20 18:01:27.000000 libexe-20240420/libfdata/libfdata_libfcache.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7810 2024-04-20 18:01:27.000000 libexe-20240420/libfdata/libfdata_vector.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-20 19:41:15.000000 libexe-20240420/libexe/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5298 2024-04-20 17:11:51.000000 libexe-20240420/libexe/libexe_definitions.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2730 2024-04-20 17:11:51.000000 libexe-20240420/libexe/libexe_notify.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5145 2024-04-20 17:11:51.000000 libexe-20240420/libexe/libexe_debug_data.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10344 2024-04-20 17:11:51.000000 libexe-20240420/libexe/libexe_mz_header.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1070 2024-04-20 17:11:51.000000 libexe-20240420/libexe/libexe.rc.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14025 2024-04-20 17:11:51.000000 libexe-20240420/libexe/libexe_section_io_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1791 2024-04-20 17:11:51.000000 libexe-20240420/libexe/libexe_mz_header.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6441 2024-04-20 17:11:51.000000 libexe-20240420/libexe/libexe_ne_header.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1068 2024-04-20 18:02:11.000000 libexe-20240420/libexe/libexe.rc
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1938 2024-04-20 17:11:51.000000 libexe-20240420/libexe/libexe_coff_header.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2589 2024-04-20 17:11:51.000000 libexe-20240420/libexe/exe_mz_header.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3010 2024-04-20 17:11:51.000000 libexe-20240420/libexe/libexe_section_io_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3906 2024-04-20 17:11:51.000000 libexe-20240420/libexe/libexe_io_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1730 2024-04-20 17:11:51.000000 libexe-20240420/libexe/libexe_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1748 2024-04-20 17:11:51.000000 libexe-20240420/libexe/libexe_ne_header.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4152 2024-04-20 17:11:51.000000 libexe-20240420/libexe/libexe_section.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29646 2024-04-20 17:11:51.000000 libexe-20240420/libexe/libexe_io_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1650 2024-04-20 17:11:51.000000 libexe-20240420/libexe/libexe_import_table.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12313 2024-04-20 17:11:51.000000 libexe-20240420/libexe/libexe_debug.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2414 2024-04-20 17:14:49.000000 libexe-20240420/libexe/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5296 2024-04-20 18:02:11.000000 libexe-20240420/libexe/libexe_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4026 2024-04-20 17:11:51.000000 libexe-20240420/libexe/libexe_file.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1392 2024-04-20 17:11:51.000000 libexe-20240420/libexe/libexe_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7527 2024-04-20 17:11:51.000000 libexe-20240420/libexe/libexe_section_descriptor.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1749 2024-04-20 17:11:51.000000 libexe-20240420/libexe/libexe_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2172 2024-04-20 17:11:51.000000 libexe-20240420/libexe/libexe_coff_optional_header.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2882 2024-04-20 17:11:51.000000 libexe-20240420/libexe/libexe_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1211 2024-04-20 17:11:51.000000 libexe-20240420/libexe/exe_pe_header.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1453 2024-04-20 17:11:51.000000 libexe-20240420/libexe/libexe_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1563 2024-04-20 17:11:51.000000 libexe-20240420/libexe/libexe_notify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9263 2024-04-20 17:11:51.000000 libexe-20240420/libexe/libexe_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1450 2024-04-20 17:11:51.000000 libexe-20240420/libexe/libexe_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10091 2024-04-20 17:11:51.000000 libexe-20240420/libexe/exe_file_header.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5312 2024-04-20 17:11:51.000000 libexe-20240420/libexe/libexe_import_table.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1320 2024-04-20 17:11:51.000000 libexe-20240420/libexe/exe_ne_header.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39233 2024-04-20 17:11:51.000000 libexe-20240420/libexe/libexe_file.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8466 2024-04-20 17:11:51.000000 libexe-20240420/libexe/libexe_coff_header.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1720 2024-04-20 17:11:51.000000 libexe-20240420/libexe/libexe_libfdatetime.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2267 2024-04-20 17:11:51.000000 libexe-20240420/libexe/libexe_section_descriptor.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1697 2024-04-20 17:11:51.000000 libexe-20240420/libexe/libexe_libbfio.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1260 2024-04-20 17:11:51.000000 libexe-20240420/libexe/exe_le_header.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1539 2024-04-20 17:11:51.000000 libexe-20240420/libexe/libexe_libfdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1807 2024-04-20 17:11:51.000000 libexe-20240420/libexe/libexe.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1560 2024-04-20 17:11:51.000000 libexe-20240420/libexe/libexe_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1542 2024-04-20 17:11:51.000000 libexe-20240420/libexe/libexe_libcdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-04-20 17:11:51.000000 libexe-20240420/libexe/libexe_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1832 2024-04-20 17:11:51.000000 libexe-20240420/libexe/libexe_debug.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1649 2024-04-20 17:11:51.000000 libexe-20240420/libexe/libexe_export_table.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2571 2024-04-20 17:11:51.000000 libexe-20240420/libexe/libexe_codepage.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35815 2024-04-20 18:01:54.000000 libexe-20240420/libexe/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5306 2024-04-20 17:11:51.000000 libexe-20240420/libexe/libexe_export_table.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1363 2024-04-20 17:11:51.000000 libexe-20240420/libexe/libexe_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1362 2024-04-20 17:11:51.000000 libexe-20240420/libexe/libexe_data_directory_descriptor.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6441 2024-04-20 17:11:51.000000 libexe-20240420/libexe/libexe_le_header.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2085 2024-04-20 17:11:51.000000 libexe-20240420/libexe/exe_section_table.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    24494 2024-04-20 17:11:51.000000 libexe-20240420/libexe/libexe_section.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37745 2024-04-20 17:11:51.000000 libexe-20240420/libexe/libexe_coff_optional_header.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1986 2024-04-20 17:11:51.000000 libexe-20240420/libexe/libexe_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2024-04-20 17:11:51.000000 libexe-20240420/libexe/libexe_libfcache.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1618 2024-04-20 17:11:51.000000 libexe-20240420/libexe/libexe_debug_data.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1748 2024-04-20 17:11:51.000000 libexe-20240420/libexe/libexe_le_header.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      667 2024-04-20 17:11:48.000000 libexe-20240420/libexe.pc.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35149 2024-04-20 17:11:48.000000 libexe-20240420/COPYING
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    15358 2024-04-20 18:01:54.000000 libexe-20240420/install-sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-20 17:11:48.000000 libexe-20240420/NEWS
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    23568 2024-04-20 18:01:54.000000 libexe-20240420/depcomp
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-20 19:41:12.000000 libexe-20240420/m4/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11734 2024-04-20 17:11:53.000000 libexe-20240420/m4/libcfile.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18489 2024-04-20 17:11:53.000000 libexe-20240420/m4/libfdatetime.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      756 2023-12-03 09:03:43.000000 libexe-20240420/m4/tests.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9615 2024-04-20 17:11:53.000000 libexe-20240420/m4/libcpath.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11944 2023-12-03 09:03:43.000000 libexe-20240420/m4/lib-prefix.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3090 2023-12-03 09:03:43.000000 libexe-20240420/m4/progtest.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31495 2024-04-20 17:11:53.000000 libexe-20240420/m4/libuna.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14488 2023-12-03 09:03:43.000000 libexe-20240420/m4/gettext.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5370 2023-12-03 09:03:43.000000 libexe-20240420/m4/lib-ld.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8476 2024-04-20 17:11:53.000000 libexe-20240420/m4/libclocale.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17383 2024-04-20 17:11:53.000000 libexe-20240420/m4/libcdata.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7625 2024-04-20 17:11:53.000000 libexe-20240420/m4/libcsplit.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14127 2024-04-20 17:11:53.000000 libexe-20240420/m4/common.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11362 2024-04-20 17:11:53.000000 libexe-20240420/m4/libcthreads.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      714 2024-04-20 18:01:49.000000 libexe-20240420/m4/ltversion.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4395 2024-04-20 18:01:49.000000 libexe-20240420/m4/ltsugar.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15781 2024-04-20 17:11:53.000000 libexe-20240420/m4/libfdata.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22432 2023-12-03 09:03:43.000000 libexe-20240420/m4/host-cpu-c-abi.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   307188 2024-04-20 18:01:48.000000 libexe-20240420/m4/libtool.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18831 2023-12-03 09:03:43.000000 libexe-20240420/m4/po.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6501 2024-04-20 17:11:53.000000 libexe-20240420/m4/libcerror.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5886 2024-04-20 17:11:53.000000 libexe-20240420/m4/libcnotify.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11923 2024-04-20 17:11:53.000000 libexe-20240420/m4/libbfio.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3229 2023-12-03 09:03:43.000000 libexe-20240420/m4/intlmacosx.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6151 2024-04-20 18:01:49.000000 libexe-20240420/m4/lt~obsolete.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34802 2023-12-03 09:03:43.000000 libexe-20240420/m4/lib-link.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9731 2023-12-03 09:03:43.000000 libexe-20240420/m4/iconv.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14525 2024-04-20 18:01:48.000000 libexe-20240420/m4/ltoptions.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1234 2023-12-03 09:03:43.000000 libexe-20240420/m4/nls.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6476 2024-04-20 17:11:53.000000 libexe-20240420/m4/python.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2058 2023-12-03 09:03:43.000000 libexe-20240420/m4/types.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7566 2024-04-20 17:11:53.000000 libexe-20240420/m4/libfcache.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5093 2024-04-20 17:11:53.000000 libexe-20240420/m4/pthread.m4
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-20 19:41:12.000000 libexe-20240420/include/
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-20 19:41:12.000000 libexe-20240420/include/libexe/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3783 2024-04-20 17:11:50.000000 libexe-20240420/include/libexe/definitions.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3781 2024-04-20 18:02:11.000000 libexe-20240420/include/libexe/definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4959 2024-04-20 17:11:50.000000 libexe-20240420/include/libexe/types.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4828 2024-04-20 18:02:11.000000 libexe-20240420/include/libexe/types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1527 2024-04-20 17:11:50.000000 libexe-20240420/include/libexe/features.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6622 2024-04-20 17:11:50.000000 libexe-20240420/include/libexe/error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2024-04-20 17:11:50.000000 libexe-20240420/include/libexe/extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1463 2024-04-20 18:02:11.000000 libexe-20240420/include/libexe/features.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5078 2024-04-20 17:11:50.000000 libexe-20240420/include/libexe/codepage.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      395 2024-04-20 17:14:32.000000 libexe-20240420/include/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13070 2024-04-20 18:02:11.000000 libexe-20240420/include/libexe.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26592 2024-04-20 18:01:54.000000 libexe-20240420/include/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13070 2024-04-20 17:11:50.000000 libexe-20240420/include/libexe.h.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-20 19:41:12.000000 libexe-20240420/common/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      957 2024-04-20 17:11:50.000000 libexe-20240420/common/config_borlandc.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3878 2024-04-20 17:11:50.000000 libexe-20240420/common/file_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3259 2024-04-20 17:11:50.000000 libexe-20240420/common/memory.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10437 2024-04-20 17:11:50.000000 libexe-20240420/common/byte_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1250 2024-04-20 17:11:50.000000 libexe-20240420/common/common.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2382 2024-04-20 17:11:50.000000 libexe-20240420/common/config_winapi.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4611 2024-04-20 17:11:50.000000 libexe-20240420/common/system_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      343 2024-04-20 17:14:32.000000 libexe-20240420/common/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7375 2024-04-20 17:11:50.000000 libexe-20240420/common/types.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7372 2024-04-20 18:02:11.000000 libexe-20240420/common/types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15715 2024-04-20 18:01:53.000000 libexe-20240420/common/config.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16641 2024-04-20 18:02:11.000000 libexe-20240420/common/config.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5064 2024-04-20 17:11:50.000000 libexe-20240420/common/wide_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5419 2024-04-20 17:11:50.000000 libexe-20240420/common/narrow_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1157 2024-04-20 17:11:50.000000 libexe-20240420/common/config_msc.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23664 2024-04-20 18:01:54.000000 libexe-20240420/common/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-20 19:41:15.000000 libexe-20240420/exetools/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1737 2024-04-20 17:11:52.000000 libexe-20240420/exetools/exetools_signal.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1433 2024-04-20 17:11:52.000000 libexe-20240420/exetools/exetools_output.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2172 2024-04-20 17:12:57.000000 libexe-20240420/exetools/info_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1207 2024-04-20 17:11:52.000000 libexe-20240420/exetools/exetools_i18n.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1775 2024-04-20 17:11:52.000000 libexe-20240420/exetools/exetools_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      965 2024-04-20 17:11:52.000000 libexe-20240420/exetools/exetools_libexe.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1742 2024-04-20 17:11:52.000000 libexe-20240420/exetools/exetools_libbfio.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1765 2024-04-20 17:11:52.000000 libexe-20240420/exetools/exetools_libfdatetime.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3784 2024-04-20 17:11:52.000000 libexe-20240420/exetools/exetools_output.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1181 2024-04-20 17:14:58.000000 libexe-20240420/exetools/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1498 2024-04-20 17:11:52.000000 libexe-20240420/exetools/exetools_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11760 2024-04-20 17:12:57.000000 libexe-20240420/exetools/info_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1477 2024-04-20 17:11:52.000000 libexe-20240420/exetools/exetools_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4527 2024-04-20 17:11:52.000000 libexe-20240420/exetools/exetools_getopt.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1495 2024-04-20 17:11:52.000000 libexe-20240420/exetools/exetools_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1803 2024-04-20 17:11:52.000000 libexe-20240420/exetools/exetools_getopt.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5701 2024-04-20 17:11:52.000000 libexe-20240420/exetools/exetools_signal.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1527 2024-04-20 17:11:52.000000 libexe-20240420/exetools/exetools_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30230 2024-04-20 18:01:54.000000 libexe-20240420/exetools/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6835 2024-04-20 17:12:57.000000 libexe-20240420/exetools/exeinfo.c
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-20 19:41:13.000000 libexe-20240420/libclocale/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1969 2024-04-20 18:01:07.000000 libexe-20240420/libclocale/libclocale_wide_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1412 2024-04-20 18:01:07.000000 libexe-20240420/libclocale/libclocale_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      775 2024-04-20 18:01:07.000000 libexe-20240420/libclocale/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3412 2024-04-20 18:01:07.000000 libexe-20240420/libclocale/libclocale_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2024-04-20 18:01:07.000000 libexe-20240420/libclocale/libclocale_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1365 2024-04-20 18:01:07.000000 libexe-20240420/libclocale/libclocale_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1717 2024-04-20 18:01:07.000000 libexe-20240420/libclocale/libclocale_locale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3142 2024-04-20 18:01:07.000000 libexe-20240420/libclocale/libclocale_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21033 2024-04-20 18:01:07.000000 libexe-20240420/libclocale/libclocale_codepage.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10671 2024-04-20 18:01:07.000000 libexe-20240420/libclocale/libclocale_locale.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28862 2024-04-20 18:01:54.000000 libexe-20240420/libclocale/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1415 2024-04-20 18:01:07.000000 libexe-20240420/libclocale/libclocale_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1696 2024-04-20 18:01:07.000000 libexe-20240420/libclocale/libclocale_wide_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1961 2024-04-20 18:01:07.000000 libexe-20240420/libclocale/libclocale_codepage.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-20 19:41:14.000000 libexe-20240420/libfcache/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1551 2024-04-20 18:01:25.000000 libexe-20240420/libfcache/libfcache_libcdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1619 2024-04-20 18:01:25.000000 libexe-20240420/libfcache/libfcache_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12461 2024-04-20 18:01:25.000000 libexe-20240420/libfcache/libfcache_cache_value.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-04-20 18:01:25.000000 libexe-20240420/libfcache/libfcache_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      876 2024-04-20 18:01:25.000000 libexe-20240420/libfcache/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2024-04-20 18:01:25.000000 libexe-20240420/libfcache/libfcache_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-04-20 18:01:25.000000 libexe-20240420/libfcache/libfcache_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1178 2024-04-20 18:01:25.000000 libexe-20240420/libfcache/libfcache_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3806 2024-04-20 18:01:25.000000 libexe-20240420/libfcache/libfcache_cache.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2924 2024-04-20 18:01:25.000000 libexe-20240420/libfcache/libfcache_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-04-20 18:01:25.000000 libexe-20240420/libfcache/libfcache_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2259 2024-04-20 18:01:25.000000 libexe-20240420/libfcache/libfcache_date_time.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-04-20 18:01:25.000000 libexe-20240420/libfcache/libfcache_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3161 2024-04-20 18:01:25.000000 libexe-20240420/libfcache/libfcache_cache_value.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29371 2024-04-20 18:01:54.000000 libexe-20240420/libfcache/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1250 2024-04-20 18:01:25.000000 libexe-20240420/libfcache/libfcache_date_time.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1680 2024-04-20 18:01:25.000000 libexe-20240420/libfcache/libfcache_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26186 2024-04-20 18:01:25.000000 libexe-20240420/libfcache/libfcache_cache.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2008 2024-04-20 17:16:52.000000 libexe-20240420/Makefile.am
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-20 19:41:14.000000 libexe-20240420/libbfio/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2630 2024-04-20 18:00:58.000000 libexe-20240420/libbfio/libbfio_file_range.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27543 2024-04-20 18:00:58.000000 libexe-20240420/libbfio/libbfio_file_range_io_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2324 2024-04-20 18:00:58.000000 libexe-20240420/libbfio/libbfio_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1362 2024-04-20 18:00:58.000000 libexe-20240420/libbfio/libbfio_libcpath.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1772 2024-04-20 18:00:58.000000 libexe-20240420/libbfio/libbfio_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-04-20 18:00:58.000000 libexe-20240420/libbfio/libbfio_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2896 2024-04-20 18:00:58.000000 libexe-20240420/libbfio/libbfio_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1733 2024-04-20 18:00:58.000000 libexe-20240420/libbfio/libbfio_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4085 2024-04-20 18:00:58.000000 libexe-20240420/libbfio/libbfio_file_io_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2077 2024-04-20 18:00:58.000000 libexe-20240420/libbfio/libbfio_file_pool.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12186 2024-04-20 18:00:58.000000 libexe-20240420/libbfio/libbfio_file_range.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1572 2024-04-20 18:00:58.000000 libexe-20240420/libbfio/libbfio_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2024-04-20 18:00:58.000000 libexe-20240420/libbfio/libbfio_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1545 2024-04-20 18:00:58.000000 libexe-20240420/libbfio/libbfio_libcdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2234 2024-04-20 18:00:58.000000 libexe-20240420/libbfio/libbfio_file.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1463 2024-04-20 18:00:58.000000 libexe-20240420/libbfio/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1420 2024-04-20 18:00:58.000000 libexe-20240420/libbfio/libbfio_libcfile.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2708 2024-04-20 18:00:58.000000 libexe-20240420/libbfio/libbfio_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2614 2024-04-20 18:00:58.000000 libexe-20240420/libbfio/libbfio_codepage.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26845 2024-04-20 18:00:58.000000 libexe-20240420/libbfio/libbfio_file_io_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1448 2024-04-20 18:00:58.000000 libexe-20240420/libbfio/libbfio_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-04-20 18:00:58.000000 libexe-20240420/libbfio/libbfio_memory_range.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10798 2024-04-20 18:00:58.000000 libexe-20240420/libbfio/libbfio_file_pool.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4806 2024-04-20 18:00:58.000000 libexe-20240420/libbfio/libbfio_file_range_io_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1918 2024-04-20 18:00:58.000000 libexe-20240420/libbfio/libbfio_libcthreads.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2814 2024-04-20 18:00:58.000000 libexe-20240420/libbfio/libbfio_system_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21082 2024-04-20 18:00:58.000000 libexe-20240420/libbfio/libbfio_memory_range_io_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    64816 2024-04-20 18:00:58.000000 libexe-20240420/libbfio/libbfio_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10899 2024-04-20 18:00:58.000000 libexe-20240420/libbfio/libbfio_file.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8883 2024-04-20 18:00:58.000000 libexe-20240420/libbfio/libbfio_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5821 2024-04-20 18:00:58.000000 libexe-20240420/libbfio/libbfio_memory_range.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    81879 2024-04-20 18:00:58.000000 libexe-20240420/libbfio/libbfio_pool.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2024-04-20 18:00:58.000000 libexe-20240420/libbfio/libbfio_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32714 2024-04-20 18:01:54.000000 libexe-20240420/libbfio/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25540 2024-04-20 18:00:58.000000 libexe-20240420/libbfio/libbfio_system_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3835 2024-04-20 18:00:58.000000 libexe-20240420/libbfio/libbfio_memory_range_io_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1376 2024-04-20 18:00:58.000000 libexe-20240420/libbfio/libbfio_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6841 2024-04-20 18:00:58.000000 libexe-20240420/libbfio/libbfio_pool.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       67 2023-12-03 09:03:28.000000 libexe-20240420/ABOUT-NLS
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    49939 2024-04-20 18:01:54.000000 libexe-20240420/config.guess
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-20 19:41:12.000000 libexe-20240420/dpkg/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       27 2024-04-20 17:11:48.000000 libexe-20240420/dpkg/libexe-tools.install
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1022 2024-04-20 17:11:53.000000 libexe-20240420/dpkg/copyright
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-20 19:41:12.000000 libexe-20240420/dpkg/source/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       12 2024-04-20 17:11:48.000000 libexe-20240420/dpkg/source/format
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2006 2024-04-20 17:11:48.000000 libexe-20240420/dpkg/control
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      753 2024-04-20 17:11:48.000000 libexe-20240420/dpkg/rules
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       22 2024-04-20 17:11:48.000000 libexe-20240420/dpkg/libexe.install
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       96 2024-04-20 17:11:48.000000 libexe-20240420/dpkg/libexe-dev.install
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      119 2024-04-20 17:11:48.000000 libexe-20240420/dpkg/changelog.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      138 2024-04-20 18:02:11.000000 libexe-20240420/dpkg/changelog
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        3 2024-04-20 17:11:48.000000 libexe-20240420/dpkg/compat
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       18 2024-04-20 17:11:48.000000 libexe-20240420/dpkg/libexe-python3.install
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      480 2024-04-20 18:02:11.000000 libexe-20240420/setup.cfg
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7652 2024-04-20 17:11:48.000000 libexe-20240420/COPYING.LESSER
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)  1794516 2024-04-20 18:01:52.000000 libexe-20240420/configure
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     7400 2024-04-20 18:01:54.000000 libexe-20240420/compile
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     6878 2024-04-20 18:01:54.000000 libexe-20240420/missing
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-20 19:41:16.000000 libexe-20240420/msvscpp/
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-20 19:41:16.000000 libexe-20240420/msvscpp/libfdata/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6858 2024-04-20 17:12:13.000000 libexe-20240420/msvscpp/libfdata/libfdata.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-20 19:41:16.000000 libexe-20240420/msvscpp/libexe/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9678 2024-04-20 17:12:13.000000 libexe-20240420/msvscpp/libexe/libexe.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-20 19:41:16.000000 libexe-20240420/msvscpp/exe_test_error/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5491 2024-04-20 17:12:13.000000 libexe-20240420/msvscpp/exe_test_error/exe_test_error.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-20 19:41:16.000000 libexe-20240420/msvscpp/exeinfo/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6556 2024-04-20 17:12:13.000000 libexe-20240420/msvscpp/exeinfo/exeinfo.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-20 19:41:16.000000 libexe-20240420/msvscpp/exe_test_tools_info_handle/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5844 2024-04-20 17:12:13.000000 libexe-20240420/msvscpp/exe_test_tools_info_handle/exe_test_tools_info_handle.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-20 19:41:16.000000 libexe-20240420/msvscpp/exe_test_coff_optional_header/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5776 2024-04-20 17:12:39.000000 libexe-20240420/msvscpp/exe_test_coff_optional_header/exe_test_coff_optional_header.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-20 19:41:16.000000 libexe-20240420/msvscpp/libclocale/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4778 2024-04-20 17:12:13.000000 libexe-20240420/msvscpp/libclocale/libclocale.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-20 19:41:16.000000 libexe-20240420/msvscpp/exe_test_import_table/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5752 2024-04-20 17:12:13.000000 libexe-20240420/msvscpp/exe_test_import_table/exe_test_import_table.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-20 19:41:16.000000 libexe-20240420/msvscpp/libfcache/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5237 2024-04-20 17:12:13.000000 libexe-20240420/msvscpp/libfcache/libfcache.vcproj
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1630 2024-04-20 17:15:06.000000 libexe-20240420/msvscpp/Makefile.am
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-20 19:41:16.000000 libexe-20240420/msvscpp/libbfio/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7306 2024-04-20 17:12:13.000000 libexe-20240420/msvscpp/libbfio/libbfio.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-20 19:41:16.000000 libexe-20240420/msvscpp/exe_test_le_header/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5743 2024-04-20 17:12:39.000000 libexe-20240420/msvscpp/exe_test_le_header/exe_test_le_header.vcproj
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30356 2024-04-20 17:12:39.000000 libexe-20240420/msvscpp/libexe.sln
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-20 19:41:16.000000 libexe-20240420/msvscpp/exe_test_tools_signal/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5679 2024-04-20 17:12:13.000000 libexe-20240420/msvscpp/exe_test_tools_signal/exe_test_tools_signal.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-20 19:41:16.000000 libexe-20240420/msvscpp/exe_test_mz_header/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5743 2024-04-20 17:12:39.000000 libexe-20240420/msvscpp/exe_test_mz_header/exe_test_mz_header.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-20 19:41:16.000000 libexe-20240420/msvscpp/exe_test_support/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6384 2024-04-20 17:12:13.000000 libexe-20240420/msvscpp/exe_test_support/exe_test_support.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-20 19:41:16.000000 libexe-20240420/msvscpp/libcfile/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5597 2024-04-20 17:12:13.000000 libexe-20240420/msvscpp/libcfile/libcfile.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-20 19:41:16.000000 libexe-20240420/msvscpp/exe_test_debug_data/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5746 2024-04-20 17:12:13.000000 libexe-20240420/msvscpp/exe_test_debug_data/exe_test_debug_data.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-20 19:41:16.000000 libexe-20240420/msvscpp/exe_test_tools_output/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5679 2024-04-20 17:12:13.000000 libexe-20240420/msvscpp/exe_test_tools_output/exe_test_tools_output.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-20 19:41:16.000000 libexe-20240420/msvscpp/libcdata/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6172 2024-04-20 17:12:13.000000 libexe-20240420/msvscpp/libcdata/libcdata.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-20 19:41:16.000000 libexe-20240420/msvscpp/exe_test_io_handle/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5743 2024-04-20 17:12:13.000000 libexe-20240420/msvscpp/exe_test_io_handle/exe_test_io_handle.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-20 19:41:16.000000 libexe-20240420/msvscpp/exe_test_file/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6375 2024-04-20 17:12:13.000000 libexe-20240420/msvscpp/exe_test_file/exe_test_file.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-20 19:41:16.000000 libexe-20240420/msvscpp/exe_test_ne_header/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5743 2024-04-20 17:12:39.000000 libexe-20240420/msvscpp/exe_test_ne_header/exe_test_ne_header.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-20 19:41:16.000000 libexe-20240420/msvscpp/libcthreads/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6177 2024-04-20 17:12:13.000000 libexe-20240420/msvscpp/libcthreads/libcthreads.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-20 19:41:16.000000 libexe-20240420/msvscpp/exe_test_coff_header/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5749 2024-04-20 17:12:39.000000 libexe-20240420/msvscpp/exe_test_coff_header/exe_test_coff_header.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-20 19:41:16.000000 libexe-20240420/msvscpp/exe_test_data_directory_descriptor/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5791 2024-04-20 17:12:13.000000 libexe-20240420/msvscpp/exe_test_data_directory_descriptor/exe_test_data_directory_descriptor.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-20 19:41:16.000000 libexe-20240420/msvscpp/exe_test_notify/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5576 2024-04-20 17:12:13.000000 libexe-20240420/msvscpp/exe_test_notify/exe_test_notify.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-20 19:41:16.000000 libexe-20240420/msvscpp/libcpath/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5183 2024-04-20 17:12:13.000000 libexe-20240420/msvscpp/libcpath/libcpath.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-20 19:41:16.000000 libexe-20240420/msvscpp/exe_test_section_io_handle/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5767 2024-04-20 17:12:13.000000 libexe-20240420/msvscpp/exe_test_section_io_handle/exe_test_section_io_handle.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-20 19:41:16.000000 libexe-20240420/msvscpp/exe_test_section/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5737 2024-04-20 17:12:13.000000 libexe-20240420/msvscpp/exe_test_section/exe_test_section.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-20 19:41:16.000000 libexe-20240420/msvscpp/libcsplit/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5225 2024-04-20 17:12:13.000000 libexe-20240420/msvscpp/libcsplit/libcsplit.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-20 19:41:16.000000 libexe-20240420/msvscpp/libuna/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15387 2024-04-20 17:12:13.000000 libexe-20240420/msvscpp/libuna/libuna.vcproj
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22284 2024-04-20 18:01:54.000000 libexe-20240420/msvscpp/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-20 19:41:16.000000 libexe-20240420/msvscpp/pyexe/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6593 2024-04-20 17:12:39.000000 libexe-20240420/msvscpp/pyexe/pyexe.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-20 19:41:16.000000 libexe-20240420/msvscpp/libcnotify/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4764 2024-04-20 17:12:13.000000 libexe-20240420/msvscpp/libcnotify/libcnotify.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-20 19:41:16.000000 libexe-20240420/msvscpp/libcerror/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4488 2024-04-20 17:12:13.000000 libexe-20240420/msvscpp/libcerror/libcerror.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-20 19:41:16.000000 libexe-20240420/msvscpp/exe_test_section_descriptor/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5770 2024-04-20 17:12:13.000000 libexe-20240420/msvscpp/exe_test_section_descriptor/exe_test_section_descriptor.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-20 19:41:16.000000 libexe-20240420/msvscpp/libfdatetime/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6069 2024-04-20 17:12:13.000000 libexe-20240420/msvscpp/libfdatetime/libfdatetime.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-20 19:41:16.000000 libexe-20240420/msvscpp/exe_test_export_table/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5752 2024-04-20 17:12:13.000000 libexe-20240420/msvscpp/exe_test_export_table/exe_test_export_table.vcproj
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       90 2024-04-20 17:11:50.000000 libexe-20240420/AUTHORS
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-20 19:41:14.000000 libexe-20240420/libcfile/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-04-20 18:01:05.000000 libexe-20240420/libcfile/libcfile_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2389 2024-04-20 18:01:05.000000 libexe-20240420/libcfile/libcfile_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-04-20 18:01:05.000000 libexe-20240420/libcfile/libcfile_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1593 2024-04-20 18:01:05.000000 libexe-20240420/libcfile/libcfile_notify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25753 2024-04-20 18:01:05.000000 libexe-20240420/libcfile/libcfile_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1497 2024-04-20 18:01:05.000000 libexe-20240420/libcfile/libcfile_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      938 2024-04-20 18:01:06.000000 libexe-20240420/libcfile/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2754 2024-04-20 18:01:05.000000 libexe-20240420/libcfile/libcfile_notify.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2826 2024-04-20 18:01:05.000000 libexe-20240420/libcfile/libcfile_system_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6452 2024-04-20 18:01:05.000000 libexe-20240420/libcfile/libcfile_file.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-04-20 18:01:05.000000 libexe-20240420/libcfile/libcfile_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25560 2024-04-20 18:01:05.000000 libexe-20240420/libcfile/libcfile_system_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-04-20 18:01:05.000000 libexe-20240420/libcfile/libcfile_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-04-20 18:01:05.000000 libexe-20240420/libcfile/libcfile_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   105597 2024-04-20 18:01:05.000000 libexe-20240420/libcfile/libcfile_file.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2024-04-20 18:01:05.000000 libexe-20240420/libcfile/libcfile_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3107 2024-04-20 18:01:05.000000 libexe-20240420/libcfile/libcfile_winapi.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29695 2024-04-20 18:01:54.000000 libexe-20240420/libcfile/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-04-20 18:01:05.000000 libexe-20240420/libcfile/libcfile_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1736 2024-04-20 18:01:05.000000 libexe-20240420/libcfile/libcfile_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18388 2024-04-20 18:01:05.000000 libexe-20240420/libcfile/libcfile_winapi.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2879 2024-04-20 18:01:06.000000 libexe-20240420/libcfile/libcfile_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      574 2024-04-20 17:12:57.000000 libexe-20240420/README
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15766 2024-04-20 18:01:54.000000 libexe-20240420/INSTALL
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-20 19:41:13.000000 libexe-20240420/libcdata/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3871 2024-04-20 18:01:01.000000 libexe-20240420/libcdata/libcdata_list_element.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5231 2024-04-20 18:01:01.000000 libexe-20240420/libcdata/libcdata_array.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2115 2024-04-20 18:01:01.000000 libexe-20240420/libcdata/libcdata_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-04-20 18:01:01.000000 libexe-20240420/libcdata/libcdata_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-04-20 18:01:01.000000 libexe-20240420/libcdata/libcdata_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3790 2024-04-20 18:01:01.000000 libexe-20240420/libcdata/libcdata_btree.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22358 2024-04-20 18:01:01.000000 libexe-20240420/libcdata/libcdata_btree.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1152 2024-04-20 18:01:01.000000 libexe-20240420/libcdata/libcdata_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    69515 2024-04-20 18:01:01.000000 libexe-20240420/libcdata/libcdata_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-04-20 18:01:01.000000 libexe-20240420/libcdata/libcdata_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6448 2024-04-20 18:01:01.000000 libexe-20240420/libcdata/libcdata_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1648 2024-04-20 18:01:01.000000 libexe-20240420/libcdata/libcdata_btree_values_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1123 2024-04-20 18:01:01.000000 libexe-20240420/libcdata/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2960 2024-04-20 18:01:01.000000 libexe-20240420/libcdata/libcdata_btree_node.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2789 2024-04-20 18:01:01.000000 libexe-20240420/libcdata/libcdata_range_list_value.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12295 2024-04-20 18:01:01.000000 libexe-20240420/libcdata/libcdata_range_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   122285 2024-04-20 18:01:01.000000 libexe-20240420/libcdata/libcdata_range_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    49968 2024-04-20 18:01:01.000000 libexe-20240420/libcdata/libcdata_array.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23846 2024-04-20 18:01:01.000000 libexe-20240420/libcdata/libcdata_list_element.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1925 2024-04-20 18:01:01.000000 libexe-20240420/libcdata/libcdata_libcthreads.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8365 2024-04-20 18:01:01.000000 libexe-20240420/libcdata/libcdata_tree_node.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-04-20 18:01:01.000000 libexe-20240420/libcdata/libcdata_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1976 2024-04-20 18:01:01.000000 libexe-20240420/libcdata/libcdata_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37549 2024-04-20 18:01:01.000000 libexe-20240420/libcdata/libcdata_btree_node.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   100501 2024-04-20 18:01:01.000000 libexe-20240420/libcdata/libcdata_tree_node.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1230 2024-04-20 18:01:01.000000 libexe-20240420/libcdata/libcdata_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31608 2024-04-20 18:01:54.000000 libexe-20240420/libcdata/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10647 2024-04-20 18:01:01.000000 libexe-20240420/libcdata/libcdata_range_list_value.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5251 2024-04-20 18:01:01.000000 libexe-20240420/libcdata/libcdata_btree_values_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-04-20 18:01:01.000000 libexe-20240420/libcdata/libcdata_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       91 2024-04-20 17:11:48.000000 libexe-20240420/pyproject.toml
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      481 2024-04-20 17:11:48.000000 libexe-20240420/setup.cfg.in
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    35796 2024-04-20 18:01:54.000000 libexe-20240420/config.sub
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     9278 2024-04-20 17:11:48.000000 libexe-20240420/setup.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1196 2024-04-20 17:12:57.000000 libexe-20240420/acinclude.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2272 2024-04-20 18:02:11.000000 libexe-20240420/libexe.spec
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    18574 2023-12-03 09:03:28.000000 libexe-20240420/config.rpath
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-20 19:41:12.000000 libexe-20240420/libcthreads/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2356 2024-04-20 18:01:23.000000 libexe-20240420/libcthreads/libcthreads_thread.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3195 2024-04-20 18:01:23.000000 libexe-20240420/libcthreads/libcthreads_read_write_lock.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10198 2024-04-20 18:01:23.000000 libexe-20240420/libcthreads/libcthreads_thread.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4175 2024-04-20 18:01:23.000000 libexe-20240420/libcthreads/libcthreads_thread_pool.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1254 2024-04-20 18:01:23.000000 libexe-20240420/libcthreads/libcthreads_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2208 2024-04-20 18:01:23.000000 libexe-20240420/libcthreads/libcthreads_lock.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-04-20 18:01:23.000000 libexe-20240420/libcthreads/libcthreads_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8753 2024-04-20 18:01:23.000000 libexe-20240420/libcthreads/libcthreads_lock.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3040 2024-04-20 18:01:23.000000 libexe-20240420/libcthreads/libcthreads_condition.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2870 2024-04-20 18:01:23.000000 libexe-20240420/libcthreads/libcthreads_repeating_thread.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1167 2024-04-20 18:01:23.000000 libexe-20240420/libcthreads/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1170 2024-04-20 18:01:23.000000 libexe-20240420/libcthreads/libcthreads_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13601 2024-04-20 18:01:23.000000 libexe-20240420/libcthreads/libcthreads_mutex.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26519 2024-04-20 18:01:23.000000 libexe-20240420/libcthreads/libcthreads_queue.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2434 2024-04-20 18:01:23.000000 libexe-20240420/libcthreads/libcthreads_mutex.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2510 2024-04-20 18:01:23.000000 libexe-20240420/libcthreads/libcthreads_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2138 2024-04-20 18:01:23.000000 libexe-20240420/libcthreads/libcthreads_thread_attributes.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18281 2024-04-20 18:01:23.000000 libexe-20240420/libcthreads/libcthreads_condition.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2952 2024-04-20 18:01:23.000000 libexe-20240420/libcthreads/libcthreads_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18426 2024-04-20 18:01:23.000000 libexe-20240420/libcthreads/libcthreads_read_write_lock.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1447 2024-04-20 18:01:23.000000 libexe-20240420/libcthreads/libcthreads_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2128 2024-04-20 18:01:23.000000 libexe-20240420/libcthreads/libcthreads_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    43321 2024-04-20 18:01:23.000000 libexe-20240420/libcthreads/libcthreads_thread_pool.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1864 2024-04-20 18:01:23.000000 libexe-20240420/libcthreads/libcthreads_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4096 2024-04-20 18:01:23.000000 libexe-20240420/libcthreads/libcthreads_thread_attributes.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1428 2024-04-20 18:01:23.000000 libexe-20240420/libcthreads/libcthreads_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17481 2024-04-20 18:01:23.000000 libexe-20240420/libcthreads/libcthreads_repeating_thread.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32047 2024-04-20 18:01:54.000000 libexe-20240420/libcthreads/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3341 2024-04-20 18:01:23.000000 libexe-20240420/libcthreads/libcthreads_queue.h
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4879 2024-04-20 18:01:54.000000 libexe-20240420/test-driver
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-20 19:41:14.000000 libexe-20240420/libcpath/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2336 2024-04-20 18:01:14.000000 libexe-20240420/libcpath/libcpath_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-04-20 18:01:14.000000 libexe-20240420/libcpath/libcpath_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1990 2024-04-20 18:01:14.000000 libexe-20240420/libcpath/libcpath_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      838 2024-04-20 18:01:14.000000 libexe-20240420/libcpath/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-04-20 18:01:14.000000 libexe-20240420/libcpath/libcpath_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-04-20 18:01:14.000000 libexe-20240420/libcpath/libcpath_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2826 2024-04-20 18:01:14.000000 libexe-20240420/libcpath/libcpath_system_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1461 2024-04-20 18:01:14.000000 libexe-20240420/libcpath/libcpath_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1536 2024-04-20 18:01:14.000000 libexe-20240420/libcpath/libcpath_libcsplit.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25560 2024-04-20 18:01:14.000000 libexe-20240420/libcpath/libcpath_system_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2024-04-20 18:01:14.000000 libexe-20240420/libcpath/libcpath_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-04-20 18:01:14.000000 libexe-20240420/libcpath/libcpath_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28893 2024-04-20 18:01:54.000000 libexe-20240420/libcpath/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1736 2024-04-20 18:01:14.000000 libexe-20240420/libcpath/libcpath_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-04-20 18:01:14.000000 libexe-20240420/libcpath/libcpath_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   176165 2024-04-20 18:01:14.000000 libexe-20240420/libcpath/libcpath_path.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7170 2024-04-20 18:01:14.000000 libexe-20240420/libcpath/libcpath_path.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3094 2024-04-20 17:11:48.000000 libexe-20240420/libexe.spec.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      438 2023-12-03 09:03:28.000000 libexe-20240420/ChangeLog
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-20 19:41:15.000000 libexe-20240420/manuals/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2032 2024-04-20 17:11:53.000000 libexe-20240420/manuals/exeinfo.1
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      121 2024-04-20 17:16:03.000000 libexe-20240420/manuals/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6064 2024-04-20 17:11:53.000000 libexe-20240420/manuals/libexe.3
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25619 2024-04-20 18:01:54.000000 libexe-20240420/manuals/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-20 19:41:15.000000 libexe-20240420/tests/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1527 2024-04-20 17:11:53.000000 libexe-20240420/tests/exe_test_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1703 2024-04-20 17:11:53.000000 libexe-20240420/tests/exe_test_libbfio.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5939 2024-04-20 17:12:39.000000 libexe-20240420/tests/exe_test_mz_header.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4077 2024-04-20 17:11:53.000000 libexe-20240420/tests/exe_test_tools_signal.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5546 2024-04-20 17:11:53.000000 libexe-20240420/tests/exe_test_tools_info_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6627 2024-04-20 17:11:53.000000 libexe-20240420/tests/exe_test_coff_optional_header.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3012 2024-04-20 17:12:39.000000 libexe-20240420/tests/exe_test_section_io_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34387 2024-04-20 17:11:53.000000 libexe-20240420/tests/exe_test_file.c
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4031 2024-04-20 17:18:06.000000 libexe-20240420/tests/test_tools.sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8356 2024-04-20 17:11:53.000000 libexe-20240420/tests/exe_test_io_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5939 2024-04-20 17:12:39.000000 libexe-20240420/tests/exe_test_ne_header.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7650 2024-04-20 17:12:39.000000 libexe-20240420/tests/exe_test_export_table.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1736 2024-04-20 17:11:53.000000 libexe-20240420/tests/exe_test_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1680 2024-04-20 17:11:53.000000 libexe-20240420/tests/exe_test_memory.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      965 2024-04-20 17:11:53.000000 libexe-20240420/tests/exe_test_libexe.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7312 2024-04-20 17:15:48.000000 libexe-20240420/tests/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4229 2024-04-20 17:11:53.000000 libexe-20240420/tests/exe_test_notify.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6105 2024-04-20 17:11:53.000000 libexe-20240420/tests/exe_test_coff_header.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8609 2024-04-20 17:12:39.000000 libexe-20240420/tests/exe_test_section_descriptor.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7650 2024-04-20 17:12:39.000000 libexe-20240420/tests/exe_test_import_table.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3408 2024-04-20 17:13:11.000000 libexe-20240420/tests/pyexe_test_support.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1794 2024-04-20 17:11:53.000000 libexe-20240420/tests/exe_test_functions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3059 2024-04-20 17:11:53.000000 libexe-20240420/tests/exe_test_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-04-20 17:11:53.000000 libexe-20240420/tests/exe_test_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14071 2024-04-20 17:11:53.000000 libexe-20240420/tests/exe_test_support.c
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     1622 2024-04-20 17:11:53.000000 libexe-20240420/tests/test_manpage.sh
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4401 2024-04-20 17:11:53.000000 libexe-20240420/tests/test_python_module.sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6001 2024-04-20 17:11:53.000000 libexe-20240420/tests/exe_test_le_header.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7490 2024-04-20 17:12:39.000000 libexe-20240420/tests/exe_test_debug_data.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-04-20 17:11:53.000000 libexe-20240420/tests/exe_test_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33607 2024-04-20 17:11:53.000000 libexe-20240420/tests/test_runner.sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4527 2024-04-20 17:11:53.000000 libexe-20240420/tests/exe_test_getopt.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2024-04-20 17:11:53.000000 libexe-20240420/tests/exe_test_libclocale.h
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     3275 2024-04-20 17:11:53.000000 libexe-20240420/tests/test_exeinfo.sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13235 2024-04-20 17:11:53.000000 libexe-20240420/tests/exe_test_functions.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4606 2024-04-20 17:11:53.000000 libexe-20240420/tests/exe_test_memory.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2403 2024-04-20 17:11:53.000000 libexe-20240420/tests/exe_test_tools_output.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1573 2024-04-20 17:11:53.000000 libexe-20240420/tests/exe_test_data_directory_descriptor.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3704 2024-04-20 17:12:39.000000 libexe-20240420/tests/exe_test_section.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    66463 2024-04-20 18:01:54.000000 libexe-20240420/tests/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1803 2024-04-20 17:11:53.000000 libexe-20240420/tests/exe_test_getopt.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5731 2024-04-20 17:11:53.000000 libexe-20240420/tests/pyexe_test_file.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8504 2024-04-20 17:11:53.000000 libexe-20240420/tests/exe_test_macros.h
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4176 2024-04-20 17:14:14.000000 libexe-20240420/tests/test_library.sh
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-20 19:41:15.000000 libexe-20240420/ossfuzz/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      962 2024-04-20 17:11:51.000000 libexe-20240420/ossfuzz/ossfuzz_libexe.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      882 2024-04-20 17:15:21.000000 libexe-20240420/ossfuzz/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1739 2024-04-20 17:11:51.000000 libexe-20240420/ossfuzz/ossfuzz_libbfio.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2184 2024-04-20 17:11:51.000000 libexe-20240420/ossfuzz/file_fuzzer.cc
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30911 2024-04-20 18:01:54.000000 libexe-20240420/ossfuzz/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   332808 2024-04-20 18:01:48.000000 libexe-20240420/ltmain.sh
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-20 19:41:13.000000 libexe-20240420/libcsplit/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6125 2024-04-20 18:01:16.000000 libexe-20240420/libcsplit/libcsplit_narrow_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1360 2024-04-20 18:01:16.000000 libexe-20240420/libcsplit/libcsplit_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1679 2024-04-20 18:01:16.000000 libexe-20240420/libcsplit/libcsplit_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13944 2024-04-20 18:01:16.000000 libexe-20240420/libcsplit/libcsplit_wide_split_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2024-04-20 18:01:16.000000 libexe-20240420/libcsplit/libcsplit_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      880 2024-04-20 18:01:16.000000 libexe-20240420/libcsplit/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-04-20 18:01:16.000000 libexe-20240420/libcsplit/libcsplit_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6206 2024-04-20 18:01:16.000000 libexe-20240420/libcsplit/libcsplit_wide_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-04-20 18:01:16.000000 libexe-20240420/libcsplit/libcsplit_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2920 2024-04-20 18:01:16.000000 libexe-20240420/libcsplit/libcsplit_wide_split_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2924 2024-04-20 18:01:16.000000 libexe-20240420/libcsplit/libcsplit_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13912 2024-04-20 18:01:16.000000 libexe-20240420/libcsplit/libcsplit_narrow_split_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-04-20 18:01:16.000000 libexe-20240420/libcsplit/libcsplit_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-04-20 18:01:16.000000 libexe-20240420/libcsplit/libcsplit_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1158 2024-04-20 18:01:16.000000 libexe-20240420/libcsplit/libcsplit_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1471 2024-04-20 18:01:16.000000 libexe-20240420/libcsplit/libcsplit_wide_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29790 2024-04-20 18:01:54.000000 libexe-20240420/libcsplit/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2849 2024-04-20 18:01:16.000000 libexe-20240420/libcsplit/libcsplit_narrow_split_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1386 2024-04-20 18:01:16.000000 libexe-20240420/libcsplit/libcsplit_narrow_string.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-20 19:41:15.000000 libexe-20240420/po/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      720 2023-12-03 09:03:44.000000 libexe-20240420/po/remove-potcdate.sin
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       59 2023-12-03 09:03:44.000000 libexe-20240420/po/POTFILES.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19571 2023-12-03 09:03:44.000000 libexe-20240420/po/Makefile.in.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      153 2023-12-03 09:03:44.000000 libexe-20240420/po/quot.sed
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1204 2023-12-03 09:03:44.000000 libexe-20240420/po/en@quot.header
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1338 2023-12-03 09:03:44.000000 libexe-20240420/po/en@boldquot.header
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      217 2023-12-03 09:03:44.000000 libexe-20240420/po/boldquot.sed
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      906 2023-12-03 09:03:44.000000 libexe-20240420/po/insert-header.sin
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       50 2023-12-03 09:03:44.000000 libexe-20240420/po/ChangeLog
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1852 2024-04-20 18:02:11.000000 libexe-20240420/po/Makevars
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1852 2023-12-03 09:03:43.000000 libexe-20240420/po/Makevars.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2395 2023-12-03 09:03:44.000000 libexe-20240420/po/Rules-quot
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-20 19:41:13.000000 libexe-20240420/libuna/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8811 2024-04-20 18:01:44.000000 libexe-20240420/libuna/libuna_codepage_windows_1251.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    98308 2024-04-20 18:01:44.000000 libexe-20240420/libuna/libuna_utf16_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39461 2024-04-20 18:01:44.000000 libexe-20240420/libuna/libuna_base16_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2993 2024-04-20 18:01:44.000000 libexe-20240420/libuna/libuna_utf8_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1567 2024-04-20 18:01:44.000000 libexe-20240420/libuna/libuna_codepage_iso_8859_2.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   286239 2024-04-20 18:01:44.000000 libexe-20240420/libuna/libuna_codepage_windows_932.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-04-20 18:01:44.000000 libexe-20240420/libuna/libuna_codepage_mac_dingbats.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   101450 2024-04-20 18:01:44.000000 libexe-20240420/libuna/libuna_utf8_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    74767 2024-04-20 18:01:44.000000 libexe-20240420/libuna/libuna_base64_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1749 2024-04-20 18:01:44.000000 libexe-20240420/libuna/libuna_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1610 2024-04-20 18:01:44.000000 libexe-20240420/libuna/libuna_codepage_mac_turkish.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   156918 2024-04-20 18:01:44.000000 libexe-20240420/libuna/libuna_unicode_character.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10379 2024-04-20 18:01:44.000000 libexe-20240420/libuna/libuna_codepage_mac_gaelic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-04-20 18:01:44.000000 libexe-20240420/libuna/libuna_codepage_mac_arabic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9435 2024-04-20 18:01:44.000000 libexe-20240420/libuna/libuna_codepage_mac_thai.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1618 2024-04-20 18:01:44.000000 libexe-20240420/libuna/libuna_codepage_windows_874.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1346 2024-04-20 18:01:44.000000 libexe-20240420/libuna/libuna_codepage_iso_8859_15.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9666 2024-04-20 18:01:44.000000 libexe-20240420/libuna/libuna_utf8_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3296 2024-04-20 18:01:44.000000 libexe-20240420/libuna/libuna_codepage_iso_8859_16.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9211 2024-04-20 18:01:44.000000 libexe-20240420/libuna/libuna_codepage_windows_1255.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15691 2024-04-20 18:01:44.000000 libexe-20240420/libuna/libuna_utf7_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2921 2024-04-20 18:01:44.000000 libexe-20240420/libuna/libuna_byte_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9984 2024-04-20 18:01:44.000000 libexe-20240420/libuna/libuna_codepage_koi8_u.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1392 2024-04-20 18:01:44.000000 libexe-20240420/libuna/libuna_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2540 2024-04-20 18:01:44.000000 libexe-20240420/libuna/libuna_codepage_iso_8859_6.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2823 2024-04-20 18:01:44.000000 libexe-20240420/libuna/libuna_codepage_iso_8859_14.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3679 2024-04-20 18:01:44.000000 libexe-20240420/libuna/libuna_base64_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2882 2024-04-20 18:01:44.000000 libexe-20240420/libuna/libuna_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1658 2024-04-20 18:01:44.000000 libexe-20240420/libuna/libuna_codepage_mac_centraleurroman.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9953 2024-04-20 18:01:44.000000 libexe-20240420/libuna/libuna_codepage_mac_romanian.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1339 2024-04-20 18:01:44.000000 libexe-20240420/libuna/libuna_codepage_iso_8859_6.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2053 2024-04-20 18:01:44.000000 libexe-20240420/libuna/libuna_codepage_iso_8859_9.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1610 2024-04-20 18:01:44.000000 libexe-20240420/libuna/libuna_codepage_mac_russian.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10134 2024-04-20 18:01:44.000000 libexe-20240420/libuna/libuna_codepage_mac_dingbats.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2024-04-20 18:01:44.000000 libexe-20240420/libuna/libuna_codepage_iso_8859_15.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   430461 2024-04-20 18:01:44.000000 libexe-20240420/libuna/libuna_codepage_windows_936.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-04-20 18:01:44.000000 libexe-20240420/libuna/libuna_codepage_mac_croatian.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1259 2024-04-20 18:01:44.000000 libexe-20240420/libuna/libuna_scsu.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4193 2024-04-20 18:01:44.000000 libexe-20240420/libuna/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20049 2024-04-20 18:01:44.000000 libexe-20240420/libuna/libuna_utf32_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1830 2024-04-20 18:01:44.000000 libexe-20240420/libuna/libuna_codepage_windows_936.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3225 2024-04-20 18:01:44.000000 libexe-20240420/libuna/libuna_codepage_iso_8859_10.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9745 2024-04-20 18:01:44.000000 libexe-20240420/libuna/libuna_codepage_mac_roman.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2808 2024-04-20 18:01:44.000000 libexe-20240420/libuna/libuna_utf7_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1773 2024-04-20 18:01:44.000000 libexe-20240420/libuna/libuna_codepage_iso_8859_3.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1787 2024-04-20 18:01:44.000000 libexe-20240420/libuna/libuna_codepage_mac_thai.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-04-20 18:01:44.000000 libexe-20240420/libuna/libuna_codepage_mac_farsi.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9088 2024-04-20 18:01:44.000000 libexe-20240420/libuna/libuna_codepage_mac_ukrainian.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10880 2024-04-20 18:01:44.000000 libexe-20240420/libuna/libuna_codepage_mac_inuit.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1830 2024-04-20 18:01:44.000000 libexe-20240420/libuna/libuna_codepage_windows_932.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8050 2024-04-20 18:01:44.000000 libexe-20240420/libuna/libuna_codepage_windows_874.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2738 2024-04-20 18:01:44.000000 libexe-20240420/libuna/libuna_codepage_iso_8859_5.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-04-20 18:01:44.000000 libexe-20240420/libuna/libuna_codepage_iso_8859_10.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16705 2024-04-20 18:01:44.000000 libexe-20240420/libuna/libuna_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1929 2024-04-20 18:01:44.000000 libexe-20240420/libuna/libuna_url_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1622 2024-04-20 18:01:44.000000 libexe-20240420/libuna/libuna_codepage_mac_icelandic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1602 2024-04-20 18:01:44.000000 libexe-20240420/libuna/libuna_codepage_koi8_u.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19850 2024-04-20 18:01:44.000000 libexe-20240420/libuna/libuna_utf16_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8602 2024-04-20 18:01:44.000000 libexe-20240420/libuna/libuna_codepage_windows_1253.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1449 2024-04-20 18:01:44.000000 libexe-20240420/libuna/libuna_codepage_iso_8859_4.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9078 2024-04-20 18:01:44.000000 libexe-20240420/libuna/libuna_codepage_mac_greek.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-04-20 18:01:44.000000 libexe-20240420/libuna/libuna_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9394 2024-04-20 18:01:44.000000 libexe-20240420/libuna/libuna_codepage_mac_centraleurroman.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8997 2024-04-20 18:01:44.000000 libexe-20240420/libuna/libuna_codepage_windows_1254.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1455 2024-04-20 18:01:44.000000 libexe-20240420/libuna/libuna_codepage_iso_8859_13.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1447 2024-04-20 18:01:44.000000 libexe-20240420/libuna/libuna_codepage_iso_8859_7.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-04-20 18:01:44.000000 libexe-20240420/libuna/libuna_codepage_windows_1255.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8000 2024-04-20 18:01:44.000000 libexe-20240420/libuna/libuna_unicode_character.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1448 2024-04-20 18:01:44.000000 libexe-20240420/libuna/libuna_codepage_iso_8859_8.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3664 2024-04-20 18:01:44.000000 libexe-20240420/libuna/libuna_codepage_iso_8859_13.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-04-20 18:01:44.000000 libexe-20240420/libuna/libuna_codepage_windows_949.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9125 2024-04-20 18:01:44.000000 libexe-20240420/libuna/libuna_codepage_mac_cyrillic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9871 2024-04-20 18:01:44.000000 libexe-20240420/libuna/libuna_codepage_mac_celtic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1234 2024-04-20 18:01:44.000000 libexe-20240420/libuna/libuna_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3561 2024-04-20 18:01:44.000000 libexe-20240420/libuna/libuna_codepage_iso_8859_4.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   484762 2024-04-20 18:01:44.000000 libexe-20240420/libuna/libuna_codepage_windows_949.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3106 2024-04-20 18:01:44.000000 libexe-20240420/libuna/libuna_utf16_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14020 2024-04-20 18:01:44.000000 libexe-20240420/libuna/libuna_codepage_mac_symbol.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-04-20 18:01:44.000000 libexe-20240420/libuna/libuna_codepage_mac_roman.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9076 2024-04-20 18:01:44.000000 libexe-20240420/libuna/libuna_codepage_windows_1257.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1627 2024-04-20 18:01:44.000000 libexe-20240420/libuna/libuna_codepage_windows_1254.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   360710 2024-04-20 18:01:44.000000 libexe-20240420/libuna/libuna_codepage_windows_950.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1363 2024-04-20 18:01:44.000000 libexe-20240420/libuna/libuna_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10005 2024-04-20 18:01:44.000000 libexe-20240420/libuna/libuna_codepage_windows_1256.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1521 2024-04-20 18:01:44.000000 libexe-20240420/libuna/libuna_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3704 2024-04-20 18:01:44.000000 libexe-20240420/libuna/libuna_base32_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1625 2024-04-20 18:01:44.000000 libexe-20240420/libuna/libuna_codepage_windows_1253.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1783 2024-04-20 18:01:44.000000 libexe-20240420/libuna/libuna_codepage_iso_8859_16.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18019 2024-04-20 18:01:44.000000 libexe-20240420/libuna/libuna_utf8_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1636 2024-04-20 18:01:44.000000 libexe-20240420/libuna/libuna_codepage_windows_1250.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3610 2024-04-20 18:01:44.000000 libexe-20240420/libuna/libuna_codepage_iso_8859_2.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1140 2024-04-20 18:01:44.000000 libexe-20240420/libuna/libuna_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9542 2024-04-20 18:01:44.000000 libexe-20240420/libuna/libuna_codepage_koi8_r.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1341 2024-04-20 18:01:44.000000 libexe-20240420/libuna/libuna_codepage_iso_8859_5.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9656 2024-04-20 18:01:44.000000 libexe-20240420/libuna/libuna_utf16_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    94606 2024-04-20 18:01:44.000000 libexe-20240420/libuna/libuna_utf32_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9656 2024-04-20 18:01:44.000000 libexe-20240420/libuna/libuna_codepage_mac_icelandic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-04-20 18:01:44.000000 libexe-20240420/libuna/libuna_codepage_windows_1256.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9526 2024-04-20 18:01:44.000000 libexe-20240420/libuna/libuna_utf32_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-04-20 18:01:44.000000 libexe-20240420/libuna/libuna_codepage_mac_romanian.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2629 2024-04-20 18:01:44.000000 libexe-20240420/libuna/libuna_codepage_iso_8859_8.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1600 2024-04-20 18:01:44.000000 libexe-20240420/libuna/libuna_codepage_koi8_r.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-04-20 18:01:44.000000 libexe-20240420/libuna/libuna_codepage_mac_cyrillic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10389 2024-04-20 18:01:44.000000 libexe-20240420/libuna/libuna_codepage_mac_arabic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9776 2024-04-20 18:01:44.000000 libexe-20240420/libuna/libuna_codepage_mac_croatian.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1340 2024-04-20 18:01:44.000000 libexe-20240420/libuna/libuna_codepage_iso_8859_9.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-04-20 18:01:44.000000 libexe-20240420/libuna/libuna_codepage_mac_greek.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1630 2024-04-20 18:01:44.000000 libexe-20240420/libuna/libuna_codepage_windows_1258.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2873 2024-04-20 18:01:44.000000 libexe-20240420/libuna/libuna_codepage_iso_8859_7.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    55374 2024-04-20 18:01:54.000000 libexe-20240420/libuna/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3335 2024-04-20 18:01:44.000000 libexe-20240420/libuna/libuna_codepage_iso_8859_3.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9776 2024-04-20 18:01:44.000000 libexe-20240420/libuna/libuna_codepage_windows_1250.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3181 2024-04-20 18:01:44.000000 libexe-20240420/libuna/libuna_scsu.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7189 2024-04-20 18:01:44.000000 libexe-20240420/libuna/libuna_codepage_windows_1252.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9844 2024-04-20 18:01:44.000000 libexe-20240420/libuna/libuna_codepage_mac_turkish.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1622 2024-04-20 18:01:44.000000 libexe-20240420/libuna/libuna_codepage_mac_ukrainian.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8997 2024-04-20 18:01:44.000000 libexe-20240420/libuna/libuna_codepage_mac_russian.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9116 2024-04-20 18:01:44.000000 libexe-20240420/libuna/libuna_codepage_windows_1258.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-04-20 18:01:44.000000 libexe-20240420/libuna/libuna_codepage_mac_celtic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15485 2024-04-20 18:01:44.000000 libexe-20240420/libuna/libuna_byte_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-04-20 18:01:44.000000 libexe-20240420/libuna/libuna_codepage_mac_gaelic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3106 2024-04-20 18:01:44.000000 libexe-20240420/libuna/libuna_utf32_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1801 2024-04-20 18:01:44.000000 libexe-20240420/libuna/libuna_codepage_mac_symbol.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-04-20 18:01:44.000000 libexe-20240420/libuna/libuna_codepage_windows_1257.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-04-20 18:01:44.000000 libexe-20240420/libuna/libuna_codepage_mac_inuit.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11002 2024-04-20 18:01:44.000000 libexe-20240420/libuna/libuna_codepage_mac_farsi.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2024-04-20 18:01:44.000000 libexe-20240420/libuna/libuna_codepage_windows_950.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15532 2024-04-20 18:01:44.000000 libexe-20240420/libuna/libuna_url_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1628 2024-04-20 18:01:44.000000 libexe-20240420/libuna/libuna_codepage_windows_1251.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1644 2024-04-20 18:01:44.000000 libexe-20240420/libuna/libuna_codepage_windows_1252.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1563 2024-04-20 18:01:44.000000 libexe-20240420/libuna/libuna_codepage_iso_8859_14.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2623 2024-04-20 18:01:44.000000 libexe-20240420/libuna/libuna_base16_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    82226 2024-04-20 18:01:44.000000 libexe-20240420/libuna/libuna_base32_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39471 2024-04-20 18:01:54.000000 libexe-20240420/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-20 19:41:15.000000 libexe-20240420/pyexe/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3161 2024-04-20 17:13:11.000000 libexe-20240420/pyexe/pyexe_file.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2357 2024-04-20 17:11:52.000000 libexe-20240420/pyexe/pyexe_sections.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33702 2024-04-20 17:11:52.000000 libexe-20240420/pyexe/pyexe_file_object_io_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16577 2024-04-20 17:11:52.000000 libexe-20240420/pyexe/pyexe_datetime.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1429 2024-04-20 17:11:52.000000 libexe-20240420/pyexe/pyexe_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2751 2024-04-20 17:13:11.000000 libexe-20240420/pyexe/pyexe_section.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1136 2024-04-20 17:11:52.000000 libexe-20240420/pyexe/pyexe_codepage.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1519 2024-04-20 17:11:52.000000 libexe-20240420/pyexe/pyexe_libbfio.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1168 2024-04-20 17:15:13.000000 libexe-20240420/pyexe/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9506 2024-04-20 17:11:52.000000 libexe-20240420/pyexe/pyexe_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1384 2024-04-20 17:11:52.000000 libexe-20240420/pyexe/pyexe_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14606 2024-04-20 17:11:52.000000 libexe-20240420/pyexe/pyexe.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1526 2024-04-20 17:11:52.000000 libexe-20240420/pyexe/pyexe_integer.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      957 2024-04-20 17:11:52.000000 libexe-20240420/pyexe/pyexe_libexe.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2027 2024-04-20 17:11:52.000000 libexe-20240420/pyexe/pyexe_python.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1450 2024-04-20 17:11:52.000000 libexe-20240420/pyexe/pyexe_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1834 2024-04-20 17:11:52.000000 libexe-20240420/pyexe/pyexe.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8840 2024-04-20 17:11:52.000000 libexe-20240420/pyexe/pyexe_integer.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3218 2024-04-20 17:11:52.000000 libexe-20240420/pyexe/pyexe_codepage.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4042 2024-04-20 17:11:52.000000 libexe-20240420/pyexe/pyexe_file_object_io_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29879 2024-04-20 17:13:11.000000 libexe-20240420/pyexe/pyexe_file.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9121 2024-04-20 17:11:52.000000 libexe-20240420/pyexe/pyexe_sections.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1804 2024-04-20 17:11:52.000000 libexe-20240420/pyexe/pyexe_datetime.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21141 2024-04-20 17:13:11.000000 libexe-20240420/pyexe/pyexe_section.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    43713 2024-04-20 18:01:54.000000 libexe-20240420/pyexe/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1522 2024-04-20 17:11:52.000000 libexe-20240420/pyexe/pyexe_error.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-20 19:41:13.000000 libexe-20240420/libcnotify/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1548 2024-04-20 18:01:08.000000 libexe-20240420/libcnotify/libcnotify_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1415 2024-04-20 18:01:08.000000 libexe-20240420/libcnotify/libcnotify_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1164 2024-04-20 18:01:08.000000 libexe-20240420/libcnotify/libcnotify_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1439 2024-04-20 18:01:08.000000 libexe-20240420/libcnotify/libcnotify_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      724 2024-04-20 18:01:08.000000 libexe-20240420/libcnotify/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2024-04-20 18:01:08.000000 libexe-20240420/libcnotify/libcnotify_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1290 2024-04-20 18:01:08.000000 libexe-20240420/libcnotify/libcnotify_verbose.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1722 2024-04-20 18:01:08.000000 libexe-20240420/libcnotify/libcnotify_print.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4018 2024-04-20 18:01:08.000000 libexe-20240420/libcnotify/libcnotify_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1266 2024-04-20 18:01:08.000000 libexe-20240420/libcnotify/libcnotify_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1094 2024-04-20 18:01:08.000000 libexe-20240420/libcnotify/libcnotify_verbose.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28731 2024-04-20 18:01:54.000000 libexe-20240420/libcnotify/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1365 2024-04-20 18:01:08.000000 libexe-20240420/libcnotify/libcnotify_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8166 2024-04-20 18:01:08.000000 libexe-20240420/libcnotify/libcnotify_print.c
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-20 19:41:12.000000 libexe-20240420/libcerror/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15420 2024-04-20 18:01:03.000000 libexe-20240420/libcerror/libcerror_system.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19408 2024-04-20 18:01:03.000000 libexe-20240420/libcerror/libcerror_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-04-20 18:01:03.000000 libexe-20240420/libcerror/libcerror_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      636 2024-04-20 18:01:03.000000 libexe-20240420/libcerror/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1522 2024-04-20 18:01:03.000000 libexe-20240420/libcerror/libcerror_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2024-04-20 18:01:03.000000 libexe-20240420/libcerror/libcerror_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2880 2024-04-20 18:01:03.000000 libexe-20240420/libcerror/libcerror_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2026 2024-04-20 18:01:03.000000 libexe-20240420/libcerror/libcerror_system.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7629 2024-04-20 18:01:03.000000 libexe-20240420/libcerror/libcerror_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1158 2024-04-20 18:01:03.000000 libexe-20240420/libcerror/libcerror_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-04-20 18:01:03.000000 libexe-20240420/libcerror/libcerror_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28198 2024-04-20 18:01:54.000000 libexe-20240420/libcerror/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-20 19:41:14.000000 libexe-20240420/libfdatetime/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5406 2024-04-20 18:01:30.000000 libexe-20240420/libfdatetime/libfdatetime_floatingtime.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34352 2024-04-20 18:01:30.000000 libexe-20240420/libfdatetime/libfdatetime_nsf_timedate.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1887 2024-04-20 18:01:30.000000 libexe-20240420/libfdatetime/libfdatetime_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33399 2024-04-20 18:01:30.000000 libexe-20240420/libfdatetime/libfdatetime_floatingtime.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1220 2024-04-20 18:01:30.000000 libexe-20240420/libfdatetime/libfdatetime_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5010 2024-04-20 18:01:30.000000 libexe-20240420/libfdatetime/libfdatetime_hfs_time.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4182 2024-04-20 18:01:30.000000 libexe-20240420/libfdatetime/libfdatetime_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31774 2024-04-20 18:01:30.000000 libexe-20240420/libfdatetime/libfdatetime_hfs_time.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1144 2024-04-20 18:01:30.000000 libexe-20240420/libfdatetime/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35109 2024-04-20 18:01:30.000000 libexe-20240420/libfdatetime/libfdatetime_filetime.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4993 2024-04-20 18:01:30.000000 libexe-20240420/libfdatetime/libfdatetime_systemtime.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-04-20 18:01:30.000000 libexe-20240420/libfdatetime/libfdatetime_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    50166 2024-04-20 18:01:30.000000 libexe-20240420/libfdatetime/libfdatetime_posix_time.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1440 2024-04-20 18:01:30.000000 libexe-20240420/libfdatetime/libfdatetime_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5342 2024-04-20 18:01:30.000000 libexe-20240420/libfdatetime/libfdatetime_fat_date_time.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    41822 2024-04-20 18:01:30.000000 libexe-20240420/libfdatetime/libfdatetime_systemtime.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5761 2024-04-20 18:01:30.000000 libexe-20240420/libfdatetime/libfdatetime_nsf_timedate.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1450 2024-04-20 18:01:30.000000 libexe-20240420/libfdatetime/libfdatetime_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1154 2024-04-20 18:01:30.000000 libexe-20240420/libfdatetime/libfdatetime_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2966 2024-04-20 18:01:30.000000 libexe-20240420/libfdatetime/libfdatetime_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5771 2024-04-20 18:01:30.000000 libexe-20240420/libfdatetime/libfdatetime_posix_time.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3131 2024-04-20 18:01:30.000000 libexe-20240420/libfdatetime/libfdatetime_date_time_values.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5340 2024-04-20 18:01:30.000000 libexe-20240420/libfdatetime/libfdatetime_filetime.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    53085 2024-04-20 18:01:30.000000 libexe-20240420/libfdatetime/libfdatetime_date_time_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2468 2024-04-20 18:01:30.000000 libexe-20240420/libfdatetime/libfdatetime_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31782 2024-04-20 18:01:54.000000 libexe-20240420/libfdatetime/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31754 2024-04-20 18:01:30.000000 libexe-20240420/libfdatetime/libfdatetime_fat_date_time.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    56769 2024-04-20 18:01:51.000000 libexe-20240420/aclocal.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7147 2024-04-20 17:11:48.000000 libexe-20240420/configure.ac
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      412 2024-04-20 19:41:16.882891 libexe-20240420/PKG-INFO
```

### Comparing `libexe-20240205/libfdata/libfdata_error.h` & `libexe-20240420/libfdata/libfdata_error.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libfdata/libfdata_area.c` & `libexe-20240420/libfdata/libfdata_area.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libfdata/libfdata_stream.h` & `libexe-20240420/libfdata/libfdata_stream.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libfdata/libfdata_cache.h` & `libexe-20240420/libfdata/libfdata_cache.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libfdata/libfdata_range_list.c` & `libexe-20240420/libfdata/libfdata_range_list.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libfdata/libfdata_mapped_range.c` & `libexe-20240420/libfdata/libfdata_mapped_range.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libfdata/libfdata_libcerror.h` & `libexe-20240420/libfdata/libfdata_libcerror.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libfdata/libfdata_definitions.h` & `libexe-20240420/libfdata/libfdata_definitions.h`

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

### Comparing `libexe-20240205/libfdata/libfdata_list.c` & `libexe-20240420/libfdata/libfdata_list.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libfdata/libfdata_libcdata.h` & `libexe-20240420/libfdata/libfdata_libcdata.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libfdata/libfdata_list.h` & `libexe-20240420/libfdata/libfdata_list.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libfdata/libfdata_list_element.h` & `libexe-20240420/libfdata/libfdata_list_element.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libfdata/Makefile.am` & `libexe-20240420/libfdata/Makefile.am`

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

### Comparing `libexe-20240205/libfdata/libfdata_libcnotify.h` & `libexe-20240420/libfdata/libfdata_libcnotify.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libfdata/libfdata_extern.h` & `libexe-20240420/libfdata/libfdata_extern.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libfdata/libfdata_notify.c` & `libexe-20240420/libfdata/libfdata_notify.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libfdata/libfdata_cache.c` & `libexe-20240420/libfdata/libfdata_cache.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libfdata/libfdata_stream.c` & `libexe-20240420/libfdata/libfdata_stream.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libfdata/libfdata_unused.h` & `libexe-20240420/libfdata/libfdata_unused.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libfdata/libfdata_range.h` & `libexe-20240420/libfdata/libfdata_range.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libfdata/libfdata_area.h` & `libexe-20240420/libfdata/libfdata_area.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libfdata/libfdata_error.c` & `libexe-20240420/libfdata/libfdata_error.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libfdata/libfdata_support.h` & `libexe-20240420/libfdata/libfdata_support.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libfdata/libfdata_range.c` & `libexe-20240420/libfdata/libfdata_range.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libfdata/libfdata_mapped_range.h` & `libexe-20240420/libfdata/libfdata_mapped_range.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libfdata/libfdata_support.c` & `libexe-20240420/libfdata/libfdata_support.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libfdata/libfdata_list_element.c` & `libexe-20240420/libfdata/libfdata_list_element.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libfdata/libfdata_segments_array.c` & `libexe-20240420/libfdata/libfdata_segments_array.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libfdata/libfdata_types.h` & `libexe-20240420/libfdata/libfdata_types.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libfdata/libfdata_notify.h` & `libexe-20240420/libfdata/libfdata_notify.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libfdata/libfdata_range_list.h` & `libexe-20240420/libfdata/libfdata_range_list.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libfdata/libfdata_segments_array.h` & `libexe-20240420/libfdata/libfdata_segments_array.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libfdata/Makefile.in` & `libexe-20240420/libfdata/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -515,16 +515,16 @@
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
 
@@ -548,15 +548,16 @@
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
@@ -768,24 +769,39 @@
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
 
@@ -881,17 +897,14 @@
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

### Comparing `libexe-20240205/libfdata/libfdata_vector.c` & `libexe-20240420/libfdata/libfdata_vector.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libfdata/libfdata_libfcache.h` & `libexe-20240420/libfdata/libfdata_libfcache.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libfdata/libfdata_vector.h` & `libexe-20240420/libfdata/libfdata_vector.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libexe/libexe_definitions.h.in` & `libexe-20240420/libexe/libexe_definitions.h.in`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libexe/libexe_notify.c` & `libexe-20240420/libexe/libexe_notify.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libexe/libexe_debug_data.c` & `libexe-20240420/libexe/libexe_debug_data.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libexe/libexe_mz_header.c` & `libexe-20240420/libexe/libexe_mz_header.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libexe/libexe.rc.in` & `libexe-20240420/libexe/libexe.rc.in`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libexe/libexe_section_io_handle.c` & `libexe-20240420/libexe/libexe_section_io_handle.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libexe/libexe_mz_header.h` & `libexe-20240420/libexe/libexe_mz_header.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libexe/libexe_ne_header.c` & `libexe-20240420/libexe/libexe_ne_header.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libexe/libexe.rc` & `libexe-20240420/libexe/libexe.rc`

 * *Files 10% similar despite different names*

```diff
@@ -18,20 +18,20 @@
   FILESUBTYPE				0x0L
 BEGIN
   BLOCK "StringFileInfo"
   BEGIN
     BLOCK "040904E4"
     BEGIN
       VALUE "FileDescription",		"Library to access the executable (EXE) format\0"
-      VALUE "FileVersion",		"20240205" "\0"
+      VALUE "FileVersion",		"20240420" "\0"
       VALUE "InternalName",		"libexe.dll\0"
       VALUE "LegalCopyright",		"(C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>\0"
       VALUE "OriginalFilename",		"libexe.dll\0"
       VALUE "ProductName",		"libexe\0"
-      VALUE "ProductVersion",		"20240205" "\0"
+      VALUE "ProductVersion",		"20240420" "\0"
       VALUE "Comments",			"For more information visit https://github.com/libyal/libexe/\0"
     END
   END
   BLOCK "VarFileInfo"
   BEGIN
     VALUE "Translation", 0x0409, 1200
   END
```

### Comparing `libexe-20240205/libexe/libexe_coff_header.h` & `libexe-20240420/libexe/libexe_coff_header.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libexe/exe_mz_header.h` & `libexe-20240420/libexe/exe_mz_header.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libexe/libexe_section_io_handle.h` & `libexe-20240420/libexe/libexe_section_io_handle.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libexe/libexe_io_handle.h` & `libexe-20240420/libexe/libexe_io_handle.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libexe/libexe_libuna.h` & `libexe-20240420/libexe/libexe_libuna.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libexe/libexe_ne_header.h` & `libexe-20240420/libexe/libexe_ne_header.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libexe/libexe_section.h` & `libexe-20240420/libexe/libexe_section.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libexe/libexe_io_handle.c` & `libexe-20240420/libexe/libexe_io_handle.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libexe/libexe_import_table.h` & `libexe-20240420/libexe/libexe_import_table.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libexe/libexe_debug.c` & `libexe-20240420/libexe/libexe_debug.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libexe/Makefile.am` & `libexe-20240420/libexe/Makefile.am`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCTHREADS_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBCSPLIT_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ \
@@ -79,21 +79,19 @@
 libexe_la_LDFLAGS = -no-undefined -version-info 1:0:0
 
 EXTRA_DIST = \
 	libexe_definitions.h.in \
 	libexe.rc \
 	libexe.rc.in
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	libexe_definitions.h \
+	libexe.rc \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f libexe_definitions.h
-	-rm -f libexe.rc
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libexe ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libexe_la_SOURCES)
```

### Comparing `libexe-20240205/libexe/libexe_definitions.h` & `libexe-20240420/libexe/libexe_definitions.h`

 * *Files 1% similar despite different names*

```diff
@@ -33,19 +33,19 @@
 #if !defined( HAVE_LOCAL_LIBEXE )
 #include <libexe/definitions.h>
 
 /* The definitions in <libexe/definitions.h> are copied here
  * for local use of libexe
  */
 #else
-#define LIBEXE_VERSION						20240205
+#define LIBEXE_VERSION						20240420
 
 /* The version string
  */
-#define LIBEXE_VERSION_STRING					"20240205"
+#define LIBEXE_VERSION_STRING					"20240420"
 
 /* The access flags definitions
  * bit 1        set to 1 for read access
  * bit 2        set to 1 for write access
  * bit 3-8      not used
  */
 enum LIBEXE_ACCESS_FLAGS
```

### Comparing `libexe-20240205/libexe/libexe_file.h` & `libexe-20240420/libexe/libexe_file.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libexe/libexe_unused.h` & `libexe-20240420/libexe/libexe_unused.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libexe/libexe_section_descriptor.c` & `libexe-20240420/libexe/libexe_section_descriptor.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libexe/libexe_error.h` & `libexe-20240420/libexe/libexe_error.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libexe/libexe_coff_optional_header.h` & `libexe-20240420/libexe/libexe_coff_optional_header.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libexe/libexe_error.c` & `libexe-20240420/libexe/libexe_error.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libexe/exe_pe_header.h` & `libexe-20240420/libexe/exe_pe_header.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libexe/libexe_libclocale.h` & `libexe-20240420/libexe/libexe_libclocale.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libexe/libexe_notify.h` & `libexe-20240420/libexe/libexe_notify.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libexe/libexe_support.c` & `libexe-20240420/libexe/libexe_support.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libexe/libexe_libcnotify.h` & `libexe-20240420/libexe/libexe_libcnotify.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libexe/exe_file_header.h` & `libexe-20240420/libexe/exe_file_header.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libexe/libexe_import_table.c` & `libexe-20240420/libexe/libexe_import_table.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libexe/exe_ne_header.h` & `libexe-20240420/libexe/exe_ne_header.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libexe/libexe_file.c` & `libexe-20240420/libexe/libexe_file.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libexe/libexe_coff_header.c` & `libexe-20240420/libexe/libexe_coff_header.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libexe/libexe_libfdatetime.h` & `libexe-20240420/libexe/libexe_libfdatetime.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libexe/libexe_section_descriptor.h` & `libexe-20240420/libexe/libexe_section_descriptor.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libexe/libexe_libbfio.h` & `libexe-20240420/libexe/libexe_libbfio.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libexe/exe_le_header.h` & `libexe-20240420/libexe/exe_le_header.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libexe/libexe_libfdata.h` & `libexe-20240420/libexe/libexe_libfdata.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libexe/libexe.c` & `libexe-20240420/libexe/libexe.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libexe/libexe_types.h` & `libexe-20240420/libexe/libexe_types.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libexe/libexe_libcdata.h` & `libexe-20240420/libexe/libexe_libcdata.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libexe/libexe_libcerror.h` & `libexe-20240420/libexe/libexe_libcerror.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libexe/libexe_debug.h` & `libexe-20240420/libexe/libexe_debug.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libexe/libexe_export_table.h` & `libexe-20240420/libexe/libexe_export_table.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libexe/libexe_codepage.h` & `libexe-20240420/libexe/libexe_codepage.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libexe/Makefile.in` & `libexe-20240420/libexe/Makefile.in`

 * *Files 5% similar despite different names*

```diff
@@ -535,16 +535,16 @@
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
 	@LIBCTHREADS_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBCSPLIT_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ \
@@ -617,15 +617,18 @@
 
 libexe_la_LDFLAGS = -no-undefined -version-info 1:0:0
 EXTRA_DIST = \
 	libexe_definitions.h.in \
 	libexe.rc \
 	libexe.rc.in
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	libexe_definitions.h \
+	libexe.rc \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -873,24 +876,44 @@
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
+		-rm -f ./$(DEPDIR)/libexe.Plo
+	-rm -f ./$(DEPDIR)/libexe_coff_header.Plo
+	-rm -f ./$(DEPDIR)/libexe_coff_optional_header.Plo
+	-rm -f ./$(DEPDIR)/libexe_debug.Plo
+	-rm -f ./$(DEPDIR)/libexe_debug_data.Plo
+	-rm -f ./$(DEPDIR)/libexe_error.Plo
+	-rm -f ./$(DEPDIR)/libexe_export_table.Plo
+	-rm -f ./$(DEPDIR)/libexe_file.Plo
+	-rm -f ./$(DEPDIR)/libexe_import_table.Plo
+	-rm -f ./$(DEPDIR)/libexe_io_handle.Plo
+	-rm -f ./$(DEPDIR)/libexe_le_header.Plo
+	-rm -f ./$(DEPDIR)/libexe_mz_header.Plo
+	-rm -f ./$(DEPDIR)/libexe_ne_header.Plo
+	-rm -f ./$(DEPDIR)/libexe_notify.Plo
+	-rm -f ./$(DEPDIR)/libexe_section.Plo
+	-rm -f ./$(DEPDIR)/libexe_section_descriptor.Plo
+	-rm -f ./$(DEPDIR)/libexe_section_io_handle.Plo
+	-rm -f ./$(DEPDIR)/libexe_support.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -991,19 +1014,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am uninstall-libLTLIBRARIES
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f libexe_definitions.h
-	-rm -f libexe.rc
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libexe ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libexe_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libexe-20240205/libexe/libexe_export_table.c` & `libexe-20240420/libexe/libexe_export_table.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libexe/libexe_extern.h` & `libexe-20240420/libexe/libexe_extern.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libexe/libexe_data_directory_descriptor.h` & `libexe-20240420/libexe/libexe_data_directory_descriptor.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libexe/libexe_le_header.c` & `libexe-20240420/libexe/libexe_le_header.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libexe/exe_section_table.h` & `libexe-20240420/libexe/exe_section_table.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libexe/libexe_section.c` & `libexe-20240420/libexe/libexe_section.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libexe/libexe_coff_optional_header.c` & `libexe-20240420/libexe/libexe_coff_optional_header.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libexe/libexe_support.h` & `libexe-20240420/libexe/libexe_support.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libexe/libexe_libfcache.h` & `libexe-20240420/libexe/libexe_libfcache.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libexe/libexe_debug_data.h` & `libexe-20240420/libexe/libexe_debug_data.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libexe/libexe_le_header.h` & `libexe-20240420/libexe/libexe_le_header.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libexe.pc.in` & `libexe-20240420/libexe.pc.in`

 * *Files identical despite different names*

### Comparing `libexe-20240205/COPYING` & `libexe-20240420/COPYING`

 * *Files identical despite different names*

### Comparing `libexe-20240205/install-sh` & `libexe-20240420/install-sh`

 * *Files identical despite different names*

### Comparing `libexe-20240205/depcomp` & `libexe-20240420/depcomp`

 * *Files identical despite different names*

### Comparing `libexe-20240205/m4/libcfile.m4` & `libexe-20240420/m4/libcfile.m4`

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

### Comparing `libexe-20240205/m4/libfdatetime.m4` & `libexe-20240420/m4/libfdatetime.m4`

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

### Comparing `libexe-20240205/m4/tests.m4` & `libexe-20240420/m4/tests.m4`

 * *Files identical despite different names*

### Comparing `libexe-20240205/m4/libcpath.m4` & `libexe-20240420/m4/libcpath.m4`

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

### Comparing `libexe-20240205/m4/lib-prefix.m4` & `libexe-20240420/m4/lib-prefix.m4`

 * *Files identical despite different names*

### Comparing `libexe-20240205/m4/progtest.m4` & `libexe-20240420/m4/progtest.m4`

 * *Files identical despite different names*

### Comparing `libexe-20240205/m4/libuna.m4` & `libexe-20240420/m4/libuna.m4`

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

### Comparing `libexe-20240205/m4/gettext.m4` & `libexe-20240420/m4/gettext.m4`

 * *Files identical despite different names*

### Comparing `libexe-20240205/m4/lib-ld.m4` & `libexe-20240420/m4/lib-ld.m4`

 * *Files identical despite different names*

### Comparing `libexe-20240205/m4/libclocale.m4` & `libexe-20240420/m4/libclocale.m4`

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

### Comparing `libexe-20240205/m4/libcdata.m4` & `libexe-20240420/m4/libcdata.m4`

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

### Comparing `libexe-20240205/m4/libcsplit.m4` & `libexe-20240420/m4/libcsplit.m4`

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

### Comparing `libexe-20240205/m4/common.m4` & `libexe-20240420/m4/common.m4`

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

### Comparing `libexe-20240205/m4/libcthreads.m4` & `libexe-20240420/m4/libcthreads.m4`

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

### Comparing `libexe-20240205/m4/ltversion.m4` & `libexe-20240420/m4/ltversion.m4`

 * *Files identical despite different names*

### Comparing `libexe-20240205/m4/ltsugar.m4` & `libexe-20240420/m4/ltsugar.m4`

 * *Files identical despite different names*

### Comparing `libexe-20240205/m4/libfdata.m4` & `libexe-20240420/m4/libfdata.m4`

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

### Comparing `libexe-20240205/m4/host-cpu-c-abi.m4` & `libexe-20240420/m4/host-cpu-c-abi.m4`

 * *Files identical despite different names*

### Comparing `libexe-20240205/m4/libtool.m4` & `libexe-20240420/m4/libtool.m4`

 * *Files identical despite different names*

### Comparing `libexe-20240205/m4/po.m4` & `libexe-20240420/m4/po.m4`

 * *Files identical despite different names*

### Comparing `libexe-20240205/m4/libcerror.m4` & `libexe-20240420/m4/libcerror.m4`

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

### Comparing `libexe-20240205/m4/libcnotify.m4` & `libexe-20240420/m4/libcnotify.m4`

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

### Comparing `libexe-20240205/m4/libbfio.m4` & `libexe-20240420/m4/libbfio.m4`

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

### Comparing `libexe-20240205/m4/intlmacosx.m4` & `libexe-20240420/m4/intlmacosx.m4`

 * *Files identical despite different names*

### Comparing `libexe-20240205/m4/lt~obsolete.m4` & `libexe-20240420/m4/lt~obsolete.m4`

 * *Files identical despite different names*

### Comparing `libexe-20240205/m4/lib-link.m4` & `libexe-20240420/m4/lib-link.m4`

 * *Files identical despite different names*

### Comparing `libexe-20240205/m4/iconv.m4` & `libexe-20240420/m4/iconv.m4`

 * *Files identical despite different names*

### Comparing `libexe-20240205/m4/ltoptions.m4` & `libexe-20240420/m4/ltoptions.m4`

 * *Files identical despite different names*

### Comparing `libexe-20240205/m4/nls.m4` & `libexe-20240420/m4/nls.m4`

 * *Files identical despite different names*

### Comparing `libexe-20240205/m4/python.m4` & `libexe-20240420/m4/python.m4`

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

### Comparing `libexe-20240205/m4/types.m4` & `libexe-20240420/m4/types.m4`

 * *Files identical despite different names*

### Comparing `libexe-20240205/m4/libfcache.m4` & `libexe-20240420/m4/libfcache.m4`

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

### Comparing `libexe-20240205/m4/pthread.m4` & `libexe-20240420/m4/pthread.m4`

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

### Comparing `libexe-20240205/include/libexe/definitions.h.in` & `libexe-20240420/include/libexe/definitions.h.in`

 * *Files identical despite different names*

### Comparing `libexe-20240205/include/libexe/definitions.h` & `libexe-20240420/include/libexe/definitions.h`

 * *Files 2% similar despite different names*

```diff
@@ -20,19 +20,19 @@
  */
 
 #if !defined( _LIBEXE_DEFINITIONS_H )
 #define _LIBEXE_DEFINITIONS_H
 
 #include <libexe/types.h>
 
-#define LIBEXE_VERSION						20240205
+#define LIBEXE_VERSION						20240420
 
 /* The version string
  */
-#define LIBEXE_VERSION_STRING					"20240205"
+#define LIBEXE_VERSION_STRING					"20240420"
 
 /* The access flags definitions
  * bit 1        set to 1 for read access
  * bit 2        set to 1 for write access
  * bit 3-8      not used
  */
 enum LIBEXE_ACCESS_FLAGS
```

### Comparing `libexe-20240205/include/libexe/types.h.in` & `libexe-20240420/include/libexe/types.h.in`

 * *Files identical despite different names*

### Comparing `libexe-20240205/include/libexe/types.h` & `libexe-20240420/include/libexe/types.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/include/libexe/features.h.in` & `libexe-20240420/include/libexe/features.h.in`

 * *Files identical despite different names*

### Comparing `libexe-20240205/include/libexe/error.h` & `libexe-20240420/include/libexe/error.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/include/libexe/extern.h` & `libexe-20240420/include/libexe/extern.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/include/libexe/features.h` & `libexe-20240420/include/libexe/features.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/include/libexe/codepage.h` & `libexe-20240420/include/libexe/codepage.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/include/libexe.h` & `libexe-20240420/include/libexe.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/include/Makefile.in` & `libexe-20240420/include/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -497,15 +497,20 @@
 
 EXTRA_DIST = \
 	libexe.h.in \
 	libexe/definitions.h.in \
 	libexe/features.h.in \
 	libexe/types.h.in
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	libexe.h \
+	libexe/definitions.h \
+	libexe/features.h \
+	libexe/types.h \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
 	@for dep in $?; do \
@@ -702,23 +707,25 @@
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
@@ -800,17 +807,10 @@
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am uninstall-includeHEADERS \
 	uninstall-pkgincludeHEADERS
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f libexe.h
-	-rm -f libexe/definitions.h
-	-rm -f libexe/features.h
-	-rm -f libexe/types.h
-	-rm -f Makefile
-
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libexe-20240205/include/libexe.h.in` & `libexe-20240420/include/libexe.h.in`

 * *Files identical despite different names*

### Comparing `libexe-20240205/common/config_borlandc.h` & `libexe-20240420/common/config_borlandc.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/common/file_stream.h` & `libexe-20240420/common/file_stream.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/common/memory.h` & `libexe-20240420/common/memory.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/common/byte_stream.h` & `libexe-20240420/common/byte_stream.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/common/common.h` & `libexe-20240420/common/common.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/common/config_winapi.h` & `libexe-20240420/common/config_winapi.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/common/system_string.h` & `libexe-20240420/common/system_string.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/common/types.h.in` & `libexe-20240420/common/types.h.in`

 * *Files identical despite different names*

### Comparing `libexe-20240205/common/types.h` & `libexe-20240420/common/types.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/common/config.h.in` & `libexe-20240420/common/config.h.in`

 * *Files identical despite different names*

### Comparing `libexe-20240205/common/config.h` & `libexe-20240420/common/config.h`

 * *Files 1% similar despite different names*

```diff
@@ -514,24 +514,24 @@
 /* Define to the address where bug reports for this package should be sent. */
 #define PACKAGE_BUGREPORT "joachim.metz@gmail.com"
 
 /* Define to the full name of this package. */
 #define PACKAGE_NAME "libexe"
 
 /* Define to the full name and version of this package. */
-#define PACKAGE_STRING "libexe 20240205"
+#define PACKAGE_STRING "libexe 20240420"
 
 /* Define to the one symbol short name of this package. */
 #define PACKAGE_TARNAME "libexe"
 
 /* Define to the home page for this package. */
 #define PACKAGE_URL ""
 
 /* Define to the version of this package. */
-#define PACKAGE_VERSION "20240205"
+#define PACKAGE_VERSION "20240420"
 
 /* The size of `int', as computed by sizeof. */
 #define SIZEOF_INT 4
 
 /* The size of `long', as computed by sizeof. */
 #define SIZEOF_LONG 8
 
@@ -552,15 +552,15 @@
 /* Define to 1 if strerror_r returns char *. */
 /* #undef STRERROR_R_CHAR_P */
 
 /* Define to 1 if your <sys/time.h> declares `struct tm'. */
 /* #undef TM_IN_SYS_TIME */
 
 /* Version number of package */
-#define VERSION "20240205"
+#define VERSION "20240420"
 
 /* Number of bits in a file offset, on hosts where this is settable. */
 /* #undef _FILE_OFFSET_BITS */
 
 /* Define for large files, on AIX-style hosts. */
 /* #undef _LARGE_FILES */
```

### Comparing `libexe-20240205/common/wide_string.h` & `libexe-20240420/common/wide_string.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/common/narrow_string.h` & `libexe-20240420/common/narrow_string.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/common/config_msc.h` & `libexe-20240420/common/config_msc.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/common/Makefile.in` & `libexe-20240420/common/Makefile.in`

 * *Files 0% similar despite different names*

```diff
@@ -450,15 +450,17 @@
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
@@ -466,15 +468,18 @@
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
@@ -642,23 +647,25 @@
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
@@ -738,15 +745,10 @@
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

### Comparing `libexe-20240205/exetools/exetools_signal.h` & `libexe-20240420/exetools/exetools_signal.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/exetools/exetools_output.h` & `libexe-20240420/exetools/exetools_output.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/exetools/info_handle.h` & `libexe-20240420/exetools/info_handle.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/exetools/exetools_i18n.h` & `libexe-20240420/exetools/exetools_i18n.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/exetools/exetools_libuna.h` & `libexe-20240420/exetools/exetools_libuna.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/exetools/exetools_libexe.h` & `libexe-20240420/exetools/exetools_libexe.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/exetools/exetools_libbfio.h` & `libexe-20240420/exetools/exetools_libbfio.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/exetools/exetools_libfdatetime.h` & `libexe-20240420/exetools/exetools_libfdatetime.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/exetools/exetools_output.c` & `libexe-20240420/exetools/exetools_output.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/exetools/Makefile.am` & `libexe-20240420/exetools/Makefile.am`

 * *Files 10% similar despite different names*

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
@@ -40,17 +40,15 @@
 	@LIBUNA_LIBADD@ \
 	@LIBCNOTIFY_LIBADD@ \
 	@LIBCLOCALE_LIBADD@ \
 	../libexe/libexe.la \
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
 	@echo "Running splint on exeinfo ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(exeinfo_SOURCES)
```

### Comparing `libexe-20240205/exetools/exetools_libclocale.h` & `libexe-20240420/exetools/exetools_libclocale.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/exetools/info_handle.c` & `libexe-20240420/exetools/info_handle.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/exetools/exetools_libcerror.h` & `libexe-20240420/exetools/exetools_libcerror.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/exetools/exetools_getopt.c` & `libexe-20240420/exetools/exetools_getopt.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/exetools/exetools_libcnotify.h` & `libexe-20240420/exetools/exetools_libcnotify.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/exetools/exetools_getopt.h` & `libexe-20240420/exetools/exetools_getopt.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/exetools/exetools_signal.c` & `libexe-20240420/exetools/exetools_signal.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/exetools/exetools_unused.h` & `libexe-20240420/exetools/exetools_unused.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/exetools/Makefile.in` & `libexe-20240420/exetools/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -487,16 +487,16 @@
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
@@ -528,15 +528,16 @@
 	@LIBUNA_LIBADD@ \
 	@LIBCNOTIFY_LIBADD@ \
 	@LIBCLOCALE_LIBADD@ \
 	../libexe/libexe.la \
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
@@ -782,23 +783,30 @@
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
+		-rm -f ./$(DEPDIR)/exeinfo.Po
+	-rm -f ./$(DEPDIR)/exetools_getopt.Po
+	-rm -f ./$(DEPDIR)/exetools_output.Po
+	-rm -f ./$(DEPDIR)/exetools_signal.Po
+	-rm -f ./$(DEPDIR)/info_handle.Po
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -886,17 +894,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am uninstall-binPROGRAMS
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 splint-local:
 	@echo "Running splint on exeinfo ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(exeinfo_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libexe-20240205/exetools/exeinfo.c` & `libexe-20240420/exetools/exeinfo.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libclocale/libclocale_wide_string.c` & `libexe-20240420/libclocale/libclocale_wide_string.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libclocale/libclocale_support.h` & `libexe-20240420/libclocale/libclocale_support.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libclocale/Makefile.am` & `libexe-20240420/libclocale/Makefile.am`

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

### Comparing `libexe-20240205/libclocale/libclocale_definitions.h` & `libexe-20240420/libclocale/libclocale_definitions.h`

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

### Comparing `libexe-20240205/libclocale/libclocale_unused.h` & `libexe-20240420/libclocale/libclocale_unused.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libclocale/libclocale_libcerror.h` & `libexe-20240420/libclocale/libclocale_libcerror.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libclocale/libclocale_locale.h` & `libexe-20240420/libclocale/libclocale_locale.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libclocale/libclocale_support.c` & `libexe-20240420/libclocale/libclocale_support.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libclocale/libclocale_codepage.c` & `libexe-20240420/libclocale/libclocale_codepage.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libclocale/libclocale_locale.c` & `libexe-20240420/libclocale/libclocale_locale.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libclocale/Makefile.in` & `libexe-20240420/libclocale/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -496,30 +496,31 @@
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
@@ -722,24 +723,30 @@
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
 
@@ -826,17 +833,14 @@
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

### Comparing `libexe-20240205/libclocale/libclocale_extern.h` & `libexe-20240420/libclocale/libclocale_extern.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libclocale/libclocale_wide_string.h` & `libexe-20240420/libclocale/libclocale_wide_string.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libclocale/libclocale_codepage.h` & `libexe-20240420/libclocale/libclocale_codepage.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libfcache/libfcache_libcdata.h` & `libexe-20240420/libfcache/libfcache_libcdata.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libfcache/libfcache_types.h` & `libexe-20240420/libfcache/libfcache_types.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libfcache/libfcache_cache_value.c` & `libexe-20240420/libfcache/libfcache_cache_value.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libfcache/libfcache_unused.h` & `libexe-20240420/libfcache/libfcache_unused.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libfcache/Makefile.am` & `libexe-20240420/libfcache/Makefile.am`

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

### Comparing `libexe-20240205/libfcache/libfcache_support.h` & `libexe-20240420/libfcache/libfcache_support.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libfcache/libfcache_error.h` & `libexe-20240420/libfcache/libfcache_error.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libfcache/libfcache_support.c` & `libexe-20240420/libfcache/libfcache_support.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libfcache/libfcache_cache.h` & `libexe-20240420/libfcache/libfcache_cache.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libfcache/libfcache_error.c` & `libexe-20240420/libfcache/libfcache_error.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libfcache/libfcache_libcerror.h` & `libexe-20240420/libfcache/libfcache_libcerror.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libfcache/libfcache_date_time.c` & `libexe-20240420/libfcache/libfcache_date_time.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libfcache/libfcache_extern.h` & `libexe-20240420/libfcache/libfcache_extern.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libfcache/libfcache_cache_value.h` & `libexe-20240420/libfcache/libfcache_cache_value.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libfcache/Makefile.in` & `libexe-20240420/libfcache/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -498,16 +498,16 @@
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
@@ -519,15 +519,16 @@
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
@@ -731,24 +732,31 @@
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
 
@@ -836,17 +844,14 @@
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

### Comparing `libexe-20240205/libfcache/libfcache_date_time.h` & `libexe-20240420/libfcache/libfcache_date_time.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libfcache/libfcache_definitions.h` & `libexe-20240420/libfcache/libfcache_definitions.h`

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

### Comparing `libexe-20240205/libfcache/libfcache_cache.c` & `libexe-20240420/libfcache/libfcache_cache.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/Makefile.am` & `libexe-20240420/Makefile.am`

 * *Files 20% similar despite different names*

```diff
@@ -58,16 +58,23 @@
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
+	libexe.pc \
+	libexe.spec \
+	Makefile \
+	Makefile.in \
+	po/Makevars
 
 pkgconfigdir = $(libdir)/pkgconfig
 
 pkgconfig_DATA = \
 	libexe.pc
 
 libtool: @LIBTOOL_DEPS@
@@ -89,19 +96,7 @@
 	(cd $(srcdir)/libbfio && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libfcache && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libfdata && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libfdatetime && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libexe && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/po && $(MAKE) $(AM_MAKEFLAGS))
 
-distclean: clean
-	-rm -f Makefile
-	-rm -f config.status
-	-rm -f config.cache
-	-rm -f config.log
-	-rm -f libexe.pc
-	-rm -f libexe.spec
-	@for dir in ${subdirs}; do \
-		(cd $$dir && $(MAKE) distclean) \
-		|| case "$(MFLAGS)" in *k*) fail=yes;; *) exit 1;; esac; \
-	done && test -z "$$fail"
-
```

### Comparing `libexe-20240205/libbfio/libbfio_file_range.h` & `libexe-20240420/libbfio/libbfio_file_range.h`

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

### Comparing `libexe-20240205/libbfio/libbfio_file_range_io_handle.c` & `libexe-20240420/libbfio/libbfio_file_range_io_handle.c`

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

### Comparing `libexe-20240205/libbfio/libbfio_support.c` & `libexe-20240420/libbfio/libbfio_support.c`

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

### Comparing `libexe-20240205/libbfio/libbfio_libcpath.h` & `libexe-20240420/libbfio/libbfio_libcpath.h`

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

### Comparing `libexe-20240205/libbfio/libbfio_error.h` & `libexe-20240420/libbfio/libbfio_error.h`

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

### Comparing `libexe-20240205/libbfio/libbfio_libclocale.h` & `libexe-20240420/libbfio/libbfio_libclocale.h`

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

### Comparing `libexe-20240205/libbfio/libbfio_error.c` & `libexe-20240420/libbfio/libbfio_error.c`

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

### Comparing `libexe-20240205/libbfio/libbfio_libuna.h` & `libexe-20240420/libbfio/libbfio_libuna.h`

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

### Comparing `libexe-20240205/libbfio/libbfio_file_io_handle.h` & `libexe-20240420/libbfio/libbfio_file_io_handle.h`

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

### Comparing `libexe-20240205/libbfio/libbfio_file_pool.h` & `libexe-20240420/libbfio/libbfio_file_pool.h`

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

### Comparing `libexe-20240205/libbfio/libbfio_file_range.c` & `libexe-20240420/libbfio/libbfio_file_range.c`

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

### Comparing `libexe-20240205/libbfio/libbfio_types.h` & `libexe-20240420/libbfio/libbfio_types.h`

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

### Comparing `libexe-20240205/libbfio/libbfio_unused.h` & `libexe-20240420/libbfio/libbfio_unused.h`

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

### Comparing `libexe-20240205/libbfio/libbfio_libcdata.h` & `libexe-20240420/libbfio/libbfio_libcdata.h`

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

### Comparing `libexe-20240205/libbfio/libbfio_file.h` & `libexe-20240420/libbfio/libbfio_file.h`

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

### Comparing `libexe-20240205/libbfio/Makefile.am` & `libexe-20240420/libbfio/Makefile.am`

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

### Comparing `libexe-20240205/libbfio/libbfio_libcfile.h` & `libexe-20240420/libbfio/libbfio_libcfile.h`

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

### Comparing `libexe-20240205/libbfio/libbfio_definitions.h` & `libexe-20240420/libbfio/libbfio_definitions.h`

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

### Comparing `libexe-20240205/libbfio/libbfio_codepage.h` & `libexe-20240420/libbfio/libbfio_codepage.h`

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

### Comparing `libexe-20240205/libbfio/libbfio_file_io_handle.c` & `libexe-20240420/libbfio/libbfio_file_io_handle.c`

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

### Comparing `libexe-20240205/libbfio/libbfio_support.h` & `libexe-20240420/libbfio/libbfio_support.h`

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

### Comparing `libexe-20240205/libbfio/libbfio_memory_range.h` & `libexe-20240420/libbfio/libbfio_memory_range.h`

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

### Comparing `libexe-20240205/libbfio/libbfio_file_pool.c` & `libexe-20240420/libbfio/libbfio_file_pool.c`

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

### Comparing `libexe-20240205/libbfio/libbfio_file_range_io_handle.h` & `libexe-20240420/libbfio/libbfio_file_range_io_handle.h`

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

### Comparing `libexe-20240205/libbfio/libbfio_libcthreads.h` & `libexe-20240420/libbfio/libbfio_libcthreads.h`

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

### Comparing `libexe-20240205/libbfio/libbfio_system_string.h` & `libexe-20240420/libbfio/libbfio_system_string.h`

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

### Comparing `libexe-20240205/libbfio/libbfio_memory_range_io_handle.c` & `libexe-20240420/libbfio/libbfio_memory_range_io_handle.c`

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

### Comparing `libexe-20240205/libbfio/libbfio_handle.c` & `libexe-20240420/libbfio/libbfio_handle.c`

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

### Comparing `libexe-20240205/libbfio/libbfio_file.c` & `libexe-20240420/libbfio/libbfio_file.c`

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

### Comparing `libexe-20240205/libbfio/libbfio_handle.h` & `libexe-20240420/libbfio/libbfio_handle.h`

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

### Comparing `libexe-20240205/libbfio/libbfio_memory_range.c` & `libexe-20240420/libbfio/libbfio_memory_range.c`

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

### Comparing `libexe-20240205/libbfio/libbfio_pool.c` & `libexe-20240420/libbfio/libbfio_pool.c`

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

### Comparing `libexe-20240205/libbfio/libbfio_libcerror.h` & `libexe-20240420/libbfio/libbfio_libcerror.h`

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

### Comparing `libexe-20240205/libbfio/Makefile.in` & `libexe-20240420/libbfio/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -516,16 +516,16 @@
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
@@ -556,15 +556,16 @@
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
@@ -775,24 +776,38 @@
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
 
@@ -861,14 +876,16 @@
 
 ps-am:
 
 sources: sources-am
 
 sources-am: sources-local
 
+splint: splint-am
+
 splint-am: splint-local
 
 uninstall-am:
 
 .MAKE: install-am install-strip
 
 .PHONY: CTAGS GTAGS TAGS all all-am am--depfiles check check-am clean \
@@ -879,23 +896,22 @@
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

### Comparing `libexe-20240205/libbfio/libbfio_system_string.c` & `libexe-20240420/libbfio/libbfio_system_string.c`

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

### Comparing `libexe-20240205/libbfio/libbfio_memory_range_io_handle.h` & `libexe-20240420/libbfio/libbfio_memory_range_io_handle.h`

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

### Comparing `libexe-20240205/libbfio/libbfio_extern.h` & `libexe-20240420/libbfio/libbfio_extern.h`

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

### Comparing `libexe-20240205/libbfio/libbfio_pool.h` & `libexe-20240420/libbfio/libbfio_pool.h`

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

### Comparing `libexe-20240205/config.guess` & `libexe-20240420/config.guess`

 * *Files identical despite different names*

### Comparing `libexe-20240205/dpkg/copyright` & `libexe-20240420/dpkg/copyright`

 * *Files identical despite different names*

### Comparing `libexe-20240205/dpkg/control` & `libexe-20240420/dpkg/control`

 * *Files identical despite different names*

### Comparing `libexe-20240205/dpkg/rules` & `libexe-20240420/dpkg/rules`

 * *Files identical despite different names*

### Comparing `libexe-20240205/COPYING.LESSER` & `libexe-20240420/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `libexe-20240205/configure` & `libexe-20240420/configure`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #! /bin/sh
 # Guess values for system-dependent variables and create Makefiles.
-# Generated by GNU Autoconf 2.71 for libexe 20240205.
+# Generated by GNU Autoconf 2.71 for libexe 20240420.
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
 PACKAGE_NAME='libexe'
 PACKAGE_TARNAME='libexe'
-PACKAGE_VERSION='20240205'
-PACKAGE_STRING='libexe 20240205'
+PACKAGE_VERSION='20240420'
+PACKAGE_STRING='libexe 20240420'
 PACKAGE_BUGREPORT='joachim.metz@gmail.com'
 PACKAGE_URL=''
 
 ac_unique_file="include/libexe.h.in"
 # Factoring default headers for most tests.
 ac_includes_default="\
 #include <stddef.h>
@@ -1625,15 +1625,15 @@
 #
 # Report the --help message.
 #
 if test "$ac_init_help" = "long"; then
   # Omit some internal or obsolete options to make the list less imposing.
   # This message is too long to be a string in the A/UX 3.1 sh.
   cat <<_ACEOF
-\`configure' configures libexe 20240205 to adapt to many kinds of systems.
+\`configure' configures libexe 20240420 to adapt to many kinds of systems.
 
 Usage: $0 [OPTION]... [VAR=VALUE]...
 
 To assign environment variables (e.g., CC, CFLAGS...), specify them as
 VAR=VALUE.  See below for descriptions of some of the useful variables.
 
 Defaults for the options are specified in brackets.
@@ -1696,15 +1696,15 @@
   --build=BUILD     configure for building on BUILD [guessed]
   --host=HOST       cross-compile to build programs to run on HOST [BUILD]
 _ACEOF
 fi
 
 if test -n "$ac_init_help"; then
   case $ac_init_help in
-     short | recursive ) echo "Configuration of libexe 20240205:";;
+     short | recursive ) echo "Configuration of libexe 20240420:";;
    esac
   cat <<\_ACEOF
 
 Optional Features:
   --disable-option-checking  ignore unrecognized --enable/--with options
   --disable-FEATURE       do not include FEATURE (same as --enable-FEATURE=no)
   --enable-FEATURE[=ARG]  include FEATURE [ARG=yes]
@@ -1934,15 +1934,15 @@
     cd "$ac_pwd" || { ac_status=$?; break; }
   done
 fi
 
 test -n "$ac_init_help" && exit $ac_status
 if $ac_init_version; then
   cat <<\_ACEOF
-libexe configure 20240205
+libexe configure 20240420
 generated by GNU Autoconf 2.71
 
 Copyright (C) 2021 Free Software Foundation, Inc.
 This configure script is free software; the Free Software Foundation
 gives unlimited permission to copy, distribute and modify it.
 _ACEOF
   exit
@@ -2655,15 +2655,15 @@
     ac_configure_args_raw=`      printf "%s\n" "$ac_configure_args_raw" | sed "$ac_safe_unquote"`;;
 esac
 
 cat >config.log <<_ACEOF
 This file contains any messages produced by compilers while
 running configure, to aid debugging if configure makes a mistake.
 
-It was created by libexe $as_me 20240205, which was
+It was created by libexe $as_me 20240420, which was
 generated by GNU Autoconf 2.71.  Invocation command line was
 
   $ $0$ac_configure_args_raw
 
 _ACEOF
 exec 5>>config.log
 {
@@ -4144,15 +4144,15 @@
     CYGPATH_W=echo
   fi
 fi
 
 
 # Define the identity of the package.
  PACKAGE='libexe'
- VERSION='20240205'
+ VERSION='20240420'
 
 
 printf "%s\n" "#define PACKAGE \"$PACKAGE\"" >>confdefs.h
 
 
 printf "%s\n" "#define VERSION \"$VERSION\"" >>confdefs.h
 
@@ -23739,15 +23739,15 @@
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
@@ -24238,15 +24238,16 @@
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
@@ -24388,15 +24389,15 @@
 as_fn_error 1 "Missing functions: strerror_r and strerror
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
 
 fi
 
-  ac_cv_libcerror_CPPFLAGS="-I../libcerror";
+  ac_cv_libcerror_CPPFLAGS="-I../libcerror -I\$(top_srcdir)/libcerror";
   ac_cv_libcerror_LIBADD="../libcerror/libcerror.la";
 
   ac_cv_libcerror=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCERROR 1" >>confdefs.h
@@ -24490,15 +24491,15 @@
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
@@ -26130,15 +26131,15 @@
 
 
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
@@ -26192,47 +26193,52 @@
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
@@ -26266,15 +26272,15 @@
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
@@ -26308,15 +26314,15 @@
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
@@ -26351,15 +26357,15 @@
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
@@ -26393,15 +26399,15 @@
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
@@ -26435,15 +26441,15 @@
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
@@ -26477,15 +26483,15 @@
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
@@ -26519,15 +26525,15 @@
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
@@ -26562,15 +26568,15 @@
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
@@ -26604,15 +26610,15 @@
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
@@ -26646,15 +26652,15 @@
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
@@ -26688,15 +26694,15 @@
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
@@ -26730,15 +26736,15 @@
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
@@ -26773,15 +26779,15 @@
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
@@ -26815,15 +26821,15 @@
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
@@ -26857,15 +26863,15 @@
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
@@ -26899,15 +26905,15 @@
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
@@ -26941,15 +26947,15 @@
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
@@ -26984,67 +26990,76 @@
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
 
-   ac_cv_pthread_LIBADD="-lpthread";
+        ac_cv_pthread_LIBADD="-lpthread";
+
+fi
+
+    if test "x$ac_cv_with_pthread" != x && test "x$ac_cv_with_pthread" != xauto-detect && test "x$ac_cv_with_pthread" != xyes
+then :
+  { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
+printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
+as_fn_error 1 "unable to find supported pthread in directory: $ac_cv_with_pthread
+See \`config.log' for more details" "$LINENO" 5; }
 
 fi
 
 fi
 
- if test "x$ac_cv_pthread" = xpthread
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
 
@@ -27132,15 +27147,15 @@
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
@@ -30911,15 +30926,16 @@
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
@@ -30944,15 +30960,15 @@
 
 fi
 
 
     if test "x$ac_cv_libcdata" != xyes
 then :
 
-  ac_cv_libcdata_CPPFLAGS="-I../libcdata";
+  ac_cv_libcdata_CPPFLAGS="-I../libcdata -I\$(top_srcdir)/libcdata";
   ac_cv_libcdata_LIBADD="../libcdata/libcdata.la";
 
   ac_cv_libcdata=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCDATA 1" >>confdefs.h
@@ -31022,15 +31038,15 @@
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
@@ -31577,15 +31593,16 @@
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
@@ -31741,15 +31758,15 @@
 
 printf "%s\n" "#define HAVE_LANGINFO_CODESET 1" >>confdefs.h
 
 
 fi
 
 
-  ac_cv_libclocale_CPPFLAGS="-I../libclocale";
+  ac_cv_libclocale_CPPFLAGS="-I../libclocale -I\$(top_srcdir)/libclocale";
   ac_cv_libclocale_LIBADD="../libclocale/libclocale.la";
 
   ac_cv_libclocale=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCLOCALE 1" >>confdefs.h
@@ -31819,15 +31836,15 @@
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
@@ -32277,15 +32294,16 @@
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
@@ -32340,15 +32358,15 @@
 if test "x$ac_cv_header_errno_h" = xyes
 then :
   printf "%s\n" "#define HAVE_ERRNO_H 1" >>confdefs.h
 
 fi
 
 
-  ac_cv_libcnotify_CPPFLAGS="-I../libcnotify";
+  ac_cv_libcnotify_CPPFLAGS="-I../libcnotify -I\$(top_srcdir)/libcnotify";
   ac_cv_libcnotify_LIBADD="../libcnotify/libcnotify.la";
 
   ac_cv_libcnotify=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCNOTIFY 1" >>confdefs.h
@@ -32418,15 +32436,15 @@
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
@@ -33141,15 +33159,16 @@
 
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
@@ -33174,15 +33193,15 @@
 
 fi
 
 
     if test "x$ac_cv_libcsplit" != xyes
 then :
 
-  ac_cv_libcsplit_CPPFLAGS="-I../libcsplit";
+  ac_cv_libcsplit_CPPFLAGS="-I../libcsplit -I\$(top_srcdir)/libcsplit";
   ac_cv_libcsplit_LIBADD="../libcsplit/libcsplit.la";
 
   ac_cv_libcsplit=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCSPLIT 1" >>confdefs.h
@@ -33252,15 +33271,15 @@
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
@@ -40462,15 +40481,16 @@
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
@@ -40495,15 +40515,15 @@
 
 fi
 
 
     if test "x$ac_cv_libuna" != xyes
 then :
 
-  ac_cv_libuna_CPPFLAGS="-I../libuna";
+  ac_cv_libuna_CPPFLAGS="-I../libuna -I\$(top_srcdir)/libuna";
   ac_cv_libuna_LIBADD="../libuna/libuna.la";
 
   ac_cv_libuna=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBUNA 1" >>confdefs.h
@@ -40573,15 +40593,15 @@
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
@@ -41762,15 +41782,16 @@
 
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
@@ -42084,15 +42105,15 @@
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
@@ -42162,15 +42183,15 @@
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
@@ -42967,15 +42988,16 @@
 
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
@@ -43165,15 +43187,15 @@
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "Missing function: mkdir
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
 
 
-  ac_cv_libcpath_CPPFLAGS="-I../libcpath";
+  ac_cv_libcpath_CPPFLAGS="-I../libcpath -I\$(top_srcdir)/libcpath";
   ac_cv_libcpath_LIBADD="../libcpath/libcpath.la";
 
   ac_cv_libcpath=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCPATH 1" >>confdefs.h
@@ -43243,15 +43265,15 @@
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
@@ -45361,15 +45383,16 @@
 
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
@@ -45394,15 +45417,15 @@
 
 fi
 
 
     if test "x$ac_cv_libbfio" != xyes
 then :
 
-  ac_cv_libbfio_CPPFLAGS="-I../libbfio";
+  ac_cv_libbfio_CPPFLAGS="-I../libbfio -I\$(top_srcdir)/libbfio";
   ac_cv_libbfio_LIBADD="../libbfio/libbfio.la";
 
   ac_cv_libbfio=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBBFIO 1" >>confdefs.h
@@ -45472,15 +45495,15 @@
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
@@ -46392,15 +46415,16 @@
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
@@ -46493,15 +46517,15 @@
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
@@ -46571,15 +46595,15 @@
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
@@ -49859,15 +49883,16 @@
 
 
 
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
@@ -49892,15 +49917,15 @@
 
 fi
 
 
     if test "x$ac_cv_libfdata" != xyes
 then :
 
-  ac_cv_libfdata_CPPFLAGS="-I../libfdata";
+  ac_cv_libfdata_CPPFLAGS="-I../libfdata -I\$(top_srcdir)/libfdata";
   ac_cv_libfdata_LIBADD="../libfdata/libfdata.la";
 
   ac_cv_libfdata=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBFDATA 1" >>confdefs.h
@@ -49970,15 +49995,15 @@
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
@@ -53414,15 +53439,16 @@
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
@@ -53447,15 +53473,15 @@
 
 fi
 
 
     if test "x$ac_cv_libfdatetime" != xyes
 then :
 
-  ac_cv_libfdatetime_CPPFLAGS="-I../libfdatetime";
+  ac_cv_libfdatetime_CPPFLAGS="-I../libfdatetime -I\$(top_srcdir)/libfdatetime";
   ac_cv_libfdatetime_LIBADD="../libfdatetime/libfdatetime.la";
 
   ac_cv_libfdatetime=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBFDATETIME 1" >>confdefs.h
@@ -53766,16 +53792,20 @@
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
 
@@ -54780,15 +54810,15 @@
 test $as_write_fail = 0 && chmod +x $CONFIG_STATUS || ac_write_fail=1
 
 cat >>$CONFIG_STATUS <<\_ACEOF || ac_write_fail=1
 # Save the log message, to keep $0 and so on meaningful, and to
 # report actual input values of CONFIG_FILES etc. instead of their
 # values after options handling.
 ac_log="
-This file was extended by libexe $as_me 20240205, which was
+This file was extended by libexe $as_me 20240420, which was
 generated by GNU Autoconf 2.71.  Invocation command line was
 
   CONFIG_FILES    = $CONFIG_FILES
   CONFIG_HEADERS  = $CONFIG_HEADERS
   CONFIG_LINKS    = $CONFIG_LINKS
   CONFIG_COMMANDS = $CONFIG_COMMANDS
   $ $0 $@
@@ -54848,15 +54878,15 @@
 
 _ACEOF
 ac_cs_config=`printf "%s\n" "$ac_configure_args" | sed "$ac_safe_unquote"`
 ac_cs_config_escaped=`printf "%s\n" "$ac_cs_config" | sed "s/^ //; s/'/'\\\\\\\\''/g"`
 cat >>$CONFIG_STATUS <<_ACEOF || ac_write_fail=1
 ac_cs_config='$ac_cs_config_escaped'
 ac_cs_version="\\
-libexe config.status 20240205
+libexe config.status 20240420
 configured by $0, generated by GNU Autoconf 2.71,
   with options \\"\$ac_cs_config\\"
 
 Copyright (C) 2021 Free Software Foundation, Inc.
 This config.status script is free software; the Free Software Foundation
 gives unlimited permission to copy, distribute and modify it."
```

### Comparing `libexe-20240205/compile` & `libexe-20240420/compile`

 * *Files identical despite different names*

### Comparing `libexe-20240205/missing` & `libexe-20240420/missing`

 * *Files identical despite different names*

### Comparing `libexe-20240205/msvscpp/libfdata/libfdata.vcproj` & `libexe-20240420/msvscpp/libfdata/libfdata.vcproj`

 * *Files identical despite different names*

### Comparing `libexe-20240205/msvscpp/libexe/libexe.vcproj` & `libexe-20240420/msvscpp/libexe/libexe.vcproj`

 * *Files identical despite different names*

### Comparing `libexe-20240205/msvscpp/exe_test_error/exe_test_error.vcproj` & `libexe-20240420/msvscpp/exe_test_error/exe_test_error.vcproj`

 * *Files identical despite different names*

### Comparing `libexe-20240205/msvscpp/exeinfo/exeinfo.vcproj` & `libexe-20240420/msvscpp/exeinfo/exeinfo.vcproj`

 * *Files identical despite different names*

### Comparing `libexe-20240205/msvscpp/exe_test_tools_info_handle/exe_test_tools_info_handle.vcproj` & `libexe-20240420/msvscpp/exe_test_tools_info_handle/exe_test_tools_info_handle.vcproj`

 * *Files identical despite different names*

### Comparing `libexe-20240205/msvscpp/exe_test_coff_optional_header/exe_test_coff_optional_header.vcproj` & `libexe-20240420/msvscpp/exe_test_coff_optional_header/exe_test_coff_optional_header.vcproj`

 * *Files identical despite different names*

### Comparing `libexe-20240205/msvscpp/libclocale/libclocale.vcproj` & `libexe-20240420/msvscpp/libclocale/libclocale.vcproj`

 * *Files identical despite different names*

### Comparing `libexe-20240205/msvscpp/exe_test_import_table/exe_test_import_table.vcproj` & `libexe-20240420/msvscpp/exe_test_import_table/exe_test_import_table.vcproj`

 * *Files identical despite different names*

### Comparing `libexe-20240205/msvscpp/libfcache/libfcache.vcproj` & `libexe-20240420/msvscpp/libfcache/libfcache.vcproj`

 * *Files identical despite different names*

### Comparing `libexe-20240205/msvscpp/Makefile.am` & `libexe-20240420/msvscpp/Makefile.am`

 * *Files 3% similar despite different names*

```diff
@@ -36,13 +36,11 @@
 	libuna/libuna.vcproj \
 	pyexe/pyexe.vcproj \
 	libexe.sln
 
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

### Comparing `libexe-20240205/msvscpp/libbfio/libbfio.vcproj` & `libexe-20240420/msvscpp/libbfio/libbfio.vcproj`

 * *Files identical despite different names*

### Comparing `libexe-20240205/msvscpp/exe_test_le_header/exe_test_le_header.vcproj` & `libexe-20240420/msvscpp/exe_test_le_header/exe_test_le_header.vcproj`

 * *Files identical despite different names*

### Comparing `libexe-20240205/msvscpp/libexe.sln` & `libexe-20240420/msvscpp/libexe.sln`

 * *Files identical despite different names*

### Comparing `libexe-20240205/msvscpp/exe_test_tools_signal/exe_test_tools_signal.vcproj` & `libexe-20240420/msvscpp/exe_test_tools_signal/exe_test_tools_signal.vcproj`

 * *Files identical despite different names*

### Comparing `libexe-20240205/msvscpp/exe_test_mz_header/exe_test_mz_header.vcproj` & `libexe-20240420/msvscpp/exe_test_mz_header/exe_test_mz_header.vcproj`

 * *Files identical despite different names*

### Comparing `libexe-20240205/msvscpp/exe_test_support/exe_test_support.vcproj` & `libexe-20240420/msvscpp/exe_test_support/exe_test_support.vcproj`

 * *Files identical despite different names*

### Comparing `libexe-20240205/msvscpp/libcfile/libcfile.vcproj` & `libexe-20240420/msvscpp/libcfile/libcfile.vcproj`

 * *Files identical despite different names*

### Comparing `libexe-20240205/msvscpp/exe_test_debug_data/exe_test_debug_data.vcproj` & `libexe-20240420/msvscpp/exe_test_debug_data/exe_test_debug_data.vcproj`

 * *Files identical despite different names*

### Comparing `libexe-20240205/msvscpp/exe_test_tools_output/exe_test_tools_output.vcproj` & `libexe-20240420/msvscpp/exe_test_tools_output/exe_test_tools_output.vcproj`

 * *Files identical despite different names*

### Comparing `libexe-20240205/msvscpp/libcdata/libcdata.vcproj` & `libexe-20240420/msvscpp/libcdata/libcdata.vcproj`

 * *Files identical despite different names*

### Comparing `libexe-20240205/msvscpp/exe_test_io_handle/exe_test_io_handle.vcproj` & `libexe-20240420/msvscpp/exe_test_io_handle/exe_test_io_handle.vcproj`

 * *Files identical despite different names*

### Comparing `libexe-20240205/msvscpp/exe_test_file/exe_test_file.vcproj` & `libexe-20240420/msvscpp/exe_test_file/exe_test_file.vcproj`

 * *Files identical despite different names*

### Comparing `libexe-20240205/msvscpp/exe_test_ne_header/exe_test_ne_header.vcproj` & `libexe-20240420/msvscpp/exe_test_ne_header/exe_test_ne_header.vcproj`

 * *Files identical despite different names*

### Comparing `libexe-20240205/msvscpp/libcthreads/libcthreads.vcproj` & `libexe-20240420/msvscpp/libcthreads/libcthreads.vcproj`

 * *Files identical despite different names*

### Comparing `libexe-20240205/msvscpp/exe_test_coff_header/exe_test_coff_header.vcproj` & `libexe-20240420/msvscpp/exe_test_coff_header/exe_test_coff_header.vcproj`

 * *Files identical despite different names*

### Comparing `libexe-20240205/msvscpp/exe_test_data_directory_descriptor/exe_test_data_directory_descriptor.vcproj` & `libexe-20240420/msvscpp/exe_test_data_directory_descriptor/exe_test_data_directory_descriptor.vcproj`

 * *Files identical despite different names*

### Comparing `libexe-20240205/msvscpp/exe_test_notify/exe_test_notify.vcproj` & `libexe-20240420/msvscpp/exe_test_notify/exe_test_notify.vcproj`

 * *Files identical despite different names*

### Comparing `libexe-20240205/msvscpp/libcpath/libcpath.vcproj` & `libexe-20240420/msvscpp/libcpath/libcpath.vcproj`

 * *Files identical despite different names*

### Comparing `libexe-20240205/msvscpp/exe_test_section_io_handle/exe_test_section_io_handle.vcproj` & `libexe-20240420/msvscpp/exe_test_section_io_handle/exe_test_section_io_handle.vcproj`

 * *Files identical despite different names*

### Comparing `libexe-20240205/msvscpp/exe_test_section/exe_test_section.vcproj` & `libexe-20240420/msvscpp/exe_test_section/exe_test_section.vcproj`

 * *Files identical despite different names*

### Comparing `libexe-20240205/msvscpp/libcsplit/libcsplit.vcproj` & `libexe-20240420/msvscpp/libcsplit/libcsplit.vcproj`

 * *Files identical despite different names*

### Comparing `libexe-20240205/msvscpp/libuna/libuna.vcproj` & `libexe-20240420/msvscpp/libuna/libuna.vcproj`

 * *Files identical despite different names*

### Comparing `libexe-20240205/msvscpp/Makefile.in` & `libexe-20240420/msvscpp/Makefile.in`

 * *Files 0% similar despite different names*

```diff
@@ -474,15 +474,16 @@
 	libuna/libuna.vcproj \
 	pyexe/pyexe.vcproj \
 	libexe.sln
 
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
@@ -586,23 +587,25 @@
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
@@ -681,13 +684,10 @@
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

### Comparing `libexe-20240205/msvscpp/pyexe/pyexe.vcproj` & `libexe-20240420/msvscpp/pyexe/pyexe.vcproj`

 * *Files identical despite different names*

### Comparing `libexe-20240205/msvscpp/libcnotify/libcnotify.vcproj` & `libexe-20240420/msvscpp/libcnotify/libcnotify.vcproj`

 * *Files identical despite different names*

### Comparing `libexe-20240205/msvscpp/libcerror/libcerror.vcproj` & `libexe-20240420/msvscpp/libcerror/libcerror.vcproj`

 * *Files identical despite different names*

### Comparing `libexe-20240205/msvscpp/exe_test_section_descriptor/exe_test_section_descriptor.vcproj` & `libexe-20240420/msvscpp/exe_test_section_descriptor/exe_test_section_descriptor.vcproj`

 * *Files identical despite different names*

### Comparing `libexe-20240205/msvscpp/libfdatetime/libfdatetime.vcproj` & `libexe-20240420/msvscpp/libfdatetime/libfdatetime.vcproj`

 * *Files identical despite different names*

### Comparing `libexe-20240205/msvscpp/exe_test_export_table/exe_test_export_table.vcproj` & `libexe-20240420/msvscpp/exe_test_export_table/exe_test_export_table.vcproj`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libcfile/libcfile_extern.h` & `libexe-20240420/libcfile/libcfile_extern.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libcfile/libcfile_support.h` & `libexe-20240420/libcfile/libcfile_support.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libcfile/libcfile_unused.h` & `libexe-20240420/libcfile/libcfile_unused.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libcfile/libcfile_notify.h` & `libexe-20240420/libcfile/libcfile_notify.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libcfile/libcfile_support.c` & `libexe-20240420/libcfile/libcfile_support.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libcfile/libcfile_types.h` & `libexe-20240420/libcfile/libcfile_types.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libcfile/Makefile.am` & `libexe-20240420/libcfile/Makefile.am`

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

### Comparing `libexe-20240205/libcfile/libcfile_notify.c` & `libexe-20240420/libcfile/libcfile_notify.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libcfile/libcfile_system_string.h` & `libexe-20240420/libcfile/libcfile_system_string.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libcfile/libcfile_file.h` & `libexe-20240420/libcfile/libcfile_file.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libcfile/libcfile_libcnotify.h` & `libexe-20240420/libcfile/libcfile_libcnotify.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libcfile/libcfile_system_string.c` & `libexe-20240420/libcfile/libcfile_system_string.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libcfile/libcfile_error.h` & `libexe-20240420/libcfile/libcfile_error.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libcfile/libcfile_libcerror.h` & `libexe-20240420/libcfile/libcfile_libcerror.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libcfile/libcfile_file.c` & `libexe-20240420/libcfile/libcfile_file.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libcfile/libcfile_libclocale.h` & `libexe-20240420/libcfile/libcfile_libclocale.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libcfile/libcfile_winapi.h` & `libexe-20240420/libcfile/libcfile_winapi.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libcfile/Makefile.in` & `libexe-20240420/libcfile/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -498,16 +498,16 @@
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
@@ -522,15 +522,16 @@
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
@@ -735,24 +736,32 @@
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
 
@@ -841,17 +850,14 @@
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

### Comparing `libexe-20240205/libcfile/libcfile_error.c` & `libexe-20240420/libcfile/libcfile_error.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libcfile/libcfile_libuna.h` & `libexe-20240420/libcfile/libcfile_libuna.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libcfile/libcfile_winapi.c` & `libexe-20240420/libcfile/libcfile_winapi.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libcfile/libcfile_definitions.h` & `libexe-20240420/libcfile/libcfile_definitions.h`

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

### Comparing `libexe-20240205/README` & `libexe-20240420/README`

 * *Files identical despite different names*

### Comparing `libexe-20240205/INSTALL` & `libexe-20240420/INSTALL`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libcdata/libcdata_list_element.h` & `libexe-20240420/libcdata/libcdata_list_element.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libcdata/libcdata_array.h` & `libexe-20240420/libcdata/libcdata_array.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libcdata/libcdata_definitions.h` & `libexe-20240420/libcdata/libcdata_definitions.h`

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

### Comparing `libexe-20240205/libcdata/libcdata_libcerror.h` & `libexe-20240420/libcdata/libcdata_libcerror.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libcdata/libcdata_unused.h` & `libexe-20240420/libcdata/libcdata_unused.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libcdata/libcdata_btree.h` & `libexe-20240420/libcdata/libcdata_btree.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libcdata/libcdata_btree.c` & `libexe-20240420/libcdata/libcdata_btree.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libcdata/libcdata_support.c` & `libexe-20240420/libcdata/libcdata_support.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libcdata/libcdata_list.c` & `libexe-20240420/libcdata/libcdata_list.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libcdata/libcdata_extern.h` & `libexe-20240420/libcdata/libcdata_extern.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libcdata/libcdata_list.h` & `libexe-20240420/libcdata/libcdata_list.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libcdata/libcdata_btree_values_list.h` & `libexe-20240420/libcdata/libcdata_btree_values_list.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libcdata/Makefile.am` & `libexe-20240420/libcdata/Makefile.am`

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

### Comparing `libexe-20240205/libcdata/libcdata_btree_node.h` & `libexe-20240420/libcdata/libcdata_btree_node.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libcdata/libcdata_range_list_value.h` & `libexe-20240420/libcdata/libcdata_range_list_value.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libcdata/libcdata_range_list.h` & `libexe-20240420/libcdata/libcdata_range_list.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libcdata/libcdata_range_list.c` & `libexe-20240420/libcdata/libcdata_range_list.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libcdata/libcdata_array.c` & `libexe-20240420/libcdata/libcdata_array.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libcdata/libcdata_list_element.c` & `libexe-20240420/libcdata/libcdata_list_element.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libcdata/libcdata_libcthreads.h` & `libexe-20240420/libcdata/libcdata_libcthreads.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libcdata/libcdata_tree_node.h` & `libexe-20240420/libcdata/libcdata_tree_node.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libcdata/libcdata_error.h` & `libexe-20240420/libcdata/libcdata_error.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libcdata/libcdata_types.h` & `libexe-20240420/libcdata/libcdata_types.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libcdata/libcdata_btree_node.c` & `libexe-20240420/libcdata/libcdata_btree_node.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libcdata/libcdata_tree_node.c` & `libexe-20240420/libcdata/libcdata_tree_node.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libcdata/libcdata_support.h` & `libexe-20240420/libcdata/libcdata_support.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libcdata/Makefile.in` & `libexe-20240420/libcdata/Makefile.in`

 * *Files 3% similar despite different names*

```diff
@@ -512,16 +512,16 @@
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
@@ -538,15 +538,16 @@
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
@@ -756,24 +757,37 @@
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
 
@@ -867,17 +881,14 @@
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

### Comparing `libexe-20240205/libcdata/libcdata_range_list_value.c` & `libexe-20240420/libcdata/libcdata_range_list_value.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libcdata/libcdata_btree_values_list.c` & `libexe-20240420/libcdata/libcdata_btree_values_list.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libcdata/libcdata_error.c` & `libexe-20240420/libcdata/libcdata_error.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/config.sub` & `libexe-20240420/config.sub`

 * *Files identical despite different names*

### Comparing `libexe-20240205/setup.py` & `libexe-20240420/setup.py`

 * *Files identical despite different names*

### Comparing `libexe-20240205/acinclude.m4` & `libexe-20240420/acinclude.m4`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libexe.spec` & `libexe-20240420/libexe.spec`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 Name: libexe
-Version: 20240205
+Version: 20240420
 Release: 1
 Summary: Library to access the executable (EXE) format
 Group: System Environment/Libraries
 License: LGPL-3.0-or-later
 Source: %{name}-%{version}.tar.gz
 URL: https://github.com/libyal/libexe
              
@@ -90,10 +90,10 @@
 %files -n libexe-tools
 %license COPYING COPYING.LESSER
 %doc AUTHORS README
 %{_bindir}/*
 %{_mandir}/man1/*
 
 %changelog
-* Mon Feb  5 2024 Joachim Metz <joachim.metz@gmail.com> 20240205-1
+* Sat Apr 20 2024 Joachim Metz <joachim.metz@gmail.com> 20240420-1
 - Auto-generated
```

### Comparing `libexe-20240205/config.rpath` & `libexe-20240420/config.rpath`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libcthreads/libcthreads_thread.h` & `libexe-20240420/libcthreads/libcthreads_thread.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libcthreads/libcthreads_read_write_lock.h` & `libexe-20240420/libcthreads/libcthreads_read_write_lock.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libcthreads/libcthreads_thread.c` & `libexe-20240420/libcthreads/libcthreads_thread.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libcthreads/libcthreads_thread_pool.h` & `libexe-20240420/libcthreads/libcthreads_thread_pool.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libcthreads/libcthreads_support.h` & `libexe-20240420/libcthreads/libcthreads_support.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libcthreads/libcthreads_lock.h` & `libexe-20240420/libcthreads/libcthreads_lock.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libcthreads/libcthreads_unused.h` & `libexe-20240420/libcthreads/libcthreads_unused.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libcthreads/libcthreads_lock.c` & `libexe-20240420/libcthreads/libcthreads_lock.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libcthreads/libcthreads_condition.h` & `libexe-20240420/libcthreads/libcthreads_condition.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libcthreads/libcthreads_repeating_thread.h` & `libexe-20240420/libcthreads/libcthreads_repeating_thread.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libcthreads/Makefile.am` & `libexe-20240420/libcthreads/Makefile.am`

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

### Comparing `libexe-20240205/libcthreads/libcthreads_support.c` & `libexe-20240420/libcthreads/libcthreads_support.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libcthreads/libcthreads_mutex.c` & `libexe-20240420/libcthreads/libcthreads_mutex.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libcthreads/libcthreads_queue.c` & `libexe-20240420/libcthreads/libcthreads_queue.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libcthreads/libcthreads_mutex.h` & `libexe-20240420/libcthreads/libcthreads_mutex.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libcthreads/libcthreads_types.h` & `libexe-20240420/libcthreads/libcthreads_types.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libcthreads/libcthreads_thread_attributes.h` & `libexe-20240420/libcthreads/libcthreads_thread_attributes.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libcthreads/libcthreads_condition.c` & `libexe-20240420/libcthreads/libcthreads_condition.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libcthreads/libcthreads_error.c` & `libexe-20240420/libcthreads/libcthreads_error.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libcthreads/libcthreads_read_write_lock.c` & `libexe-20240420/libcthreads/libcthreads_read_write_lock.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libcthreads/libcthreads_libcerror.h` & `libexe-20240420/libcthreads/libcthreads_libcerror.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libcthreads/libcthreads_definitions.h` & `libexe-20240420/libcthreads/libcthreads_definitions.h`

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

### Comparing `libexe-20240205/libcthreads/libcthreads_thread_pool.c` & `libexe-20240420/libcthreads/libcthreads_thread_pool.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libcthreads/libcthreads_error.h` & `libexe-20240420/libcthreads/libcthreads_error.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libcthreads/libcthreads_thread_attributes.c` & `libexe-20240420/libcthreads/libcthreads_thread_attributes.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libcthreads/libcthreads_extern.h` & `libexe-20240420/libcthreads/libcthreads_extern.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libcthreads/libcthreads_repeating_thread.c` & `libexe-20240420/libcthreads/libcthreads_repeating_thread.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libcthreads/Makefile.in` & `libexe-20240420/libcthreads/Makefile.in`

 * *Files 6% similar despite different names*

```diff
@@ -516,16 +516,16 @@
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
@@ -540,15 +540,16 @@
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
@@ -758,24 +759,37 @@
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
 
@@ -869,17 +883,14 @@
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

### Comparing `libexe-20240205/libcthreads/libcthreads_queue.h` & `libexe-20240420/libcthreads/libcthreads_queue.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/test-driver` & `libexe-20240420/test-driver`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libcpath/libcpath_support.c` & `libexe-20240420/libcpath/libcpath_support.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libcpath/libcpath_libcerror.h` & `libexe-20240420/libcpath/libcpath_libcerror.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libcpath/libcpath_definitions.h` & `libexe-20240420/libcpath/libcpath_definitions.h`

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

### Comparing `libexe-20240205/libcpath/Makefile.am` & `libexe-20240420/libcpath/Makefile.am`

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

### Comparing `libexe-20240205/libcpath/libcpath_error.c` & `libexe-20240420/libcpath/libcpath_error.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libcpath/libcpath_extern.h` & `libexe-20240420/libcpath/libcpath_extern.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libcpath/libcpath_system_string.h` & `libexe-20240420/libcpath/libcpath_system_string.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libcpath/libcpath_support.h` & `libexe-20240420/libcpath/libcpath_support.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libcpath/libcpath_libcsplit.h` & `libexe-20240420/libcpath/libcpath_libcsplit.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libcpath/libcpath_system_string.c` & `libexe-20240420/libcpath/libcpath_system_string.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libcpath/libcpath_libclocale.h` & `libexe-20240420/libcpath/libcpath_libclocale.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libcpath/libcpath_error.h` & `libexe-20240420/libcpath/libcpath_error.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libcpath/Makefile.in` & `libexe-20240420/libcpath/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -492,16 +492,16 @@
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
@@ -513,15 +513,16 @@
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
@@ -724,24 +725,30 @@
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
 
@@ -828,17 +835,14 @@
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

### Comparing `libexe-20240205/libcpath/libcpath_libuna.h` & `libexe-20240420/libcpath/libcpath_libuna.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libcpath/libcpath_unused.h` & `libexe-20240420/libcpath/libcpath_unused.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libcpath/libcpath_path.c` & `libexe-20240420/libcpath/libcpath_path.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libcpath/libcpath_path.h` & `libexe-20240420/libcpath/libcpath_path.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libexe.spec.in` & `libexe-20240420/libexe.spec.in`

 * *Files identical despite different names*

### Comparing `libexe-20240205/manuals/exeinfo.1` & `libexe-20240420/manuals/exeinfo.1`

 * *Files identical despite different names*

### Comparing `libexe-20240205/manuals/libexe.3` & `libexe-20240420/manuals/libexe.3`

 * *Files identical despite different names*

### Comparing `libexe-20240205/manuals/Makefile.in` & `libexe-20240420/manuals/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -472,15 +472,16 @@
 	exeinfo.1 \
 	libexe.3
 
 EXTRA_DIST = \
 	exeinfo.1 \
 	libexe.3
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
 	@for dep in $?; do \
@@ -673,23 +674,25 @@
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
@@ -771,13 +774,10 @@
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

### Comparing `libexe-20240205/tests/exe_test_unused.h` & `libexe-20240420/tests/exe_test_unused.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/tests/exe_test_libbfio.h` & `libexe-20240420/tests/exe_test_libbfio.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/tests/exe_test_mz_header.c` & `libexe-20240420/tests/exe_test_mz_header.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/tests/exe_test_tools_signal.c` & `libexe-20240420/tests/exe_test_tools_signal.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/tests/exe_test_tools_info_handle.c` & `libexe-20240420/tests/exe_test_tools_info_handle.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/tests/exe_test_coff_optional_header.c` & `libexe-20240420/tests/exe_test_coff_optional_header.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/tests/exe_test_section_io_handle.c` & `libexe-20240420/tests/exe_test_section_io_handle.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/tests/exe_test_file.c` & `libexe-20240420/tests/exe_test_file.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/tests/test_tools.sh` & `libexe-20240420/tests/test_tools.sh`

 * *Files 2% similar despite different names*

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
 
 TOOLS_TESTS="info_handle output signal";
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

### Comparing `libexe-20240205/tests/exe_test_io_handle.c` & `libexe-20240420/tests/exe_test_io_handle.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/tests/exe_test_ne_header.c` & `libexe-20240420/tests/exe_test_ne_header.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/tests/exe_test_export_table.c` & `libexe-20240420/tests/exe_test_export_table.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/tests/exe_test_libuna.h` & `libexe-20240420/tests/exe_test_libuna.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/tests/exe_test_memory.h` & `libexe-20240420/tests/exe_test_memory.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/tests/exe_test_libexe.h` & `libexe-20240420/tests/exe_test_libexe.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/tests/Makefile.am` & `libexe-20240420/tests/Makefile.am`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 AUTOMAKE_OPTIONS = subdir-objects
 
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCTHREADS_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBCSPLIT_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ \
@@ -326,13 +326,12 @@
 	exe_test_tools_signal.c \
 	exe_test_unused.h
 
 exe_test_tools_signal_LDADD = \
 	../libexe/libexe.la \
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

### Comparing `libexe-20240205/tests/exe_test_notify.c` & `libexe-20240420/tests/exe_test_notify.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/tests/exe_test_coff_header.c` & `libexe-20240420/tests/exe_test_coff_header.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/tests/exe_test_section_descriptor.c` & `libexe-20240420/tests/exe_test_section_descriptor.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/tests/exe_test_import_table.c` & `libexe-20240420/tests/exe_test_import_table.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/tests/pyexe_test_support.py` & `libexe-20240420/tests/pyexe_test_support.py`

 * *Files identical despite different names*

### Comparing `libexe-20240205/tests/exe_test_functions.h` & `libexe-20240420/tests/exe_test_functions.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/tests/exe_test_error.c` & `libexe-20240420/tests/exe_test_error.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/tests/exe_test_libcerror.h` & `libexe-20240420/tests/exe_test_libcerror.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/tests/exe_test_support.c` & `libexe-20240420/tests/exe_test_support.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/tests/test_python_module.sh` & `libexe-20240420/tests/test_python_module.sh`

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
 
+LIBRARY_NAME="libexe";
+PYTHON_MODULE="pyexe";
+
 test_python_function()
 {
 	local TEST_FUNCTION=$1;
 
 	local TEST_DESCRIPTION="Testing Python-bindings functions: ${TEST_FUNCTION}";
-	local TEST_SCRIPT="${TEST_TOOL_DIRECTORY}/pyexe_test_${TEST_FUNCTION}.py";
+	local TEST_SCRIPT="${TEST_TOOL_DIRECTORY}/${PYTHON_MODULE}_test_${TEST_FUNCTION}.py";
 
 	run_test_with_arguments "${TEST_DESCRIPTION}" "${TEST_SCRIPT}";
 	local RESULT=$?;
 
 	return ${RESULT};
 }
 
 test_python_function_with_input()
 {
 	local TEST_FUNCTION=$1;
 
 	local TEST_DESCRIPTION="Testing Python-bindings functions: ${TEST_FUNCTION}";
-	local TEST_SCRIPT="${TEST_TOOL_DIRECTORY}/pyexe_test_${TEST_FUNCTION}.py";
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
 
-	local TEST_PROFILE_DIRECTORY=$(get_test_profile_directory "input" "pyexe");
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

### Comparing `libexe-20240205/tests/exe_test_le_header.c` & `libexe-20240420/tests/exe_test_le_header.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/tests/exe_test_debug_data.c` & `libexe-20240420/tests/exe_test_debug_data.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/tests/exe_test_libcnotify.h` & `libexe-20240420/tests/exe_test_libcnotify.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/tests/test_runner.sh` & `libexe-20240420/tests/test_runner.sh`

 * *Files identical despite different names*

### Comparing `libexe-20240205/tests/exe_test_getopt.c` & `libexe-20240420/tests/exe_test_getopt.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/tests/exe_test_libclocale.h` & `libexe-20240420/tests/exe_test_libclocale.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/tests/test_exeinfo.sh` & `libexe-20240420/tests/test_exeinfo.sh`

 * *Files 4% similar despite different names*

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
 
 PROFILES=("exeinfo");
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

### Comparing `libexe-20240205/tests/exe_test_functions.c` & `libexe-20240420/tests/exe_test_functions.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/tests/exe_test_memory.c` & `libexe-20240420/tests/exe_test_memory.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/tests/exe_test_tools_output.c` & `libexe-20240420/tests/exe_test_tools_output.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/tests/exe_test_data_directory_descriptor.c` & `libexe-20240420/tests/exe_test_data_directory_descriptor.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/tests/exe_test_section.c` & `libexe-20240420/tests/exe_test_section.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/tests/Makefile.in` & `libexe-20240420/tests/Makefile.in`

 * *Files 3% similar despite different names*

```diff
@@ -837,16 +837,16 @@
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
 	@LIBCTHREADS_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBCSPLIT_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ \
@@ -1142,16 +1142,18 @@
 	exe_test_tools_signal.c \
 	exe_test_unused.h
 
 exe_test_tools_signal_LDADD = \
 	../libexe/libexe.la \
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
@@ -1657,24 +1659,52 @@
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
 	-rm -f ../exetools/$(DEPDIR)/$(am__dirstamp)
 	-rm -f ../exetools/$(am__dirstamp)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-checkPROGRAMS clean-generic clean-libtool \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ../exetools/$(DEPDIR)/exetools_output.Po
+	-rm -f ../exetools/$(DEPDIR)/exetools_signal.Po
+	-rm -f ../exetools/$(DEPDIR)/info_handle.Po
+	-rm -f ./$(DEPDIR)/exe_test_coff_header.Po
+	-rm -f ./$(DEPDIR)/exe_test_coff_optional_header.Po
+	-rm -f ./$(DEPDIR)/exe_test_data_directory_descriptor.Po
+	-rm -f ./$(DEPDIR)/exe_test_debug_data.Po
+	-rm -f ./$(DEPDIR)/exe_test_error.Po
+	-rm -f ./$(DEPDIR)/exe_test_export_table.Po
+	-rm -f ./$(DEPDIR)/exe_test_file.Po
+	-rm -f ./$(DEPDIR)/exe_test_functions.Po
+	-rm -f ./$(DEPDIR)/exe_test_getopt.Po
+	-rm -f ./$(DEPDIR)/exe_test_import_table.Po
+	-rm -f ./$(DEPDIR)/exe_test_io_handle.Po
+	-rm -f ./$(DEPDIR)/exe_test_le_header.Po
+	-rm -f ./$(DEPDIR)/exe_test_memory.Po
+	-rm -f ./$(DEPDIR)/exe_test_mz_header.Po
+	-rm -f ./$(DEPDIR)/exe_test_ne_header.Po
+	-rm -f ./$(DEPDIR)/exe_test_notify.Po
+	-rm -f ./$(DEPDIR)/exe_test_section.Po
+	-rm -f ./$(DEPDIR)/exe_test_section_descriptor.Po
+	-rm -f ./$(DEPDIR)/exe_test_section_io_handle.Po
+	-rm -f ./$(DEPDIR)/exe_test_support.Po
+	-rm -f ./$(DEPDIR)/exe_test_tools_info_handle.Po
+	-rm -f ./$(DEPDIR)/exe_test_tools_output.Po
+	-rm -f ./$(DEPDIR)/exe_test_tools_signal.Po
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -1783,13 +1813,10 @@
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

### Comparing `libexe-20240205/tests/exe_test_getopt.h` & `libexe-20240420/tests/exe_test_getopt.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/tests/pyexe_test_file.py` & `libexe-20240420/tests/pyexe_test_file.py`

 * *Files identical despite different names*

### Comparing `libexe-20240205/tests/exe_test_macros.h` & `libexe-20240420/tests/exe_test_macros.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/tests/test_library.sh` & `libexe-20240420/tests/test_library.sh`

 * *Files 9% similar despite different names*

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
 
 LIBRARY_TESTS="data_directory_descriptor debug_data error export_table import_table io_handle le_header mz_header ne_header notify section section_descriptor section_io_handle";
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

### Comparing `libexe-20240205/ossfuzz/ossfuzz_libexe.h` & `libexe-20240420/ossfuzz/ossfuzz_libexe.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/ossfuzz/ossfuzz_libbfio.h` & `libexe-20240420/ossfuzz/ossfuzz_libbfio.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/ossfuzz/file_fuzzer.cc` & `libexe-20240420/ossfuzz/file_fuzzer.cc`

 * *Files identical despite different names*

### Comparing `libexe-20240205/ossfuzz/Makefile.in` & `libexe-20240420/ossfuzz/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -505,16 +505,16 @@
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
@@ -534,15 +534,16 @@
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBCDATA_LIBADD@ \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	../libexe/libexe.la \
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
@@ -784,23 +785,26 @@
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
+		-rm -f ./$(DEPDIR)/file_fuzzer.Po
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -884,17 +888,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am uninstall-binPROGRAMS
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 splint-local:
 	@echo "Running splint on file_fuzzer ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(file_fuzzer_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libexe-20240205/ltmain.sh` & `libexe-20240420/ltmain.sh`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libcsplit/libcsplit_narrow_string.c` & `libexe-20240420/libcsplit/libcsplit_narrow_string.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libcsplit/libcsplit_definitions.h` & `libexe-20240420/libcsplit/libcsplit_definitions.h`

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

### Comparing `libexe-20240205/libcsplit/libcsplit_types.h` & `libexe-20240420/libcsplit/libcsplit_types.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libcsplit/libcsplit_wide_split_string.c` & `libexe-20240420/libcsplit/libcsplit_wide_split_string.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libcsplit/libcsplit_support.h` & `libexe-20240420/libcsplit/libcsplit_support.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libcsplit/Makefile.am` & `libexe-20240420/libcsplit/Makefile.am`

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

### Comparing `libexe-20240205/libcsplit/libcsplit_libcerror.h` & `libexe-20240420/libcsplit/libcsplit_libcerror.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libcsplit/libcsplit_wide_string.c` & `libexe-20240420/libcsplit/libcsplit_wide_string.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libcsplit/libcsplit_unused.h` & `libexe-20240420/libcsplit/libcsplit_unused.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libcsplit/libcsplit_wide_split_string.h` & `libexe-20240420/libcsplit/libcsplit_wide_split_string.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libcsplit/libcsplit_error.c` & `libexe-20240420/libcsplit/libcsplit_error.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libcsplit/libcsplit_narrow_split_string.c` & `libexe-20240420/libcsplit/libcsplit_narrow_split_string.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libcsplit/libcsplit_extern.h` & `libexe-20240420/libcsplit/libcsplit_extern.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libcsplit/libcsplit_error.h` & `libexe-20240420/libcsplit/libcsplit_error.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libcsplit/libcsplit_support.c` & `libexe-20240420/libcsplit/libcsplit_support.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libcsplit/libcsplit_wide_string.h` & `libexe-20240420/libcsplit/libcsplit_wide_string.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libcsplit/Makefile.in` & `libexe-20240420/libcsplit/Makefile.in`

 * *Files 3% similar despite different names*

```diff
@@ -502,16 +502,16 @@
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
@@ -520,15 +520,16 @@
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
@@ -733,24 +734,32 @@
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
 
@@ -839,17 +848,14 @@
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

### Comparing `libexe-20240205/libcsplit/libcsplit_narrow_split_string.h` & `libexe-20240420/libcsplit/libcsplit_narrow_split_string.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libcsplit/libcsplit_narrow_string.h` & `libexe-20240420/libcsplit/libcsplit_narrow_string.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/po/remove-potcdate.sin` & `libexe-20240420/po/remove-potcdate.sin`

 * *Files identical despite different names*

### Comparing `libexe-20240205/po/Makefile.in.in` & `libexe-20240420/po/Makefile.in.in`

 * *Files identical despite different names*

### Comparing `libexe-20240205/po/en@quot.header` & `libexe-20240420/po/en@quot.header`

 * *Files identical despite different names*

### Comparing `libexe-20240205/po/en@boldquot.header` & `libexe-20240420/po/en@boldquot.header`

 * *Files identical despite different names*

### Comparing `libexe-20240205/po/insert-header.sin` & `libexe-20240420/po/insert-header.sin`

 * *Files identical despite different names*

### Comparing `libexe-20240205/po/Makevars` & `libexe-20240420/po/Makevars`

 * *Files identical despite different names*

### Comparing `libexe-20240205/po/Makevars.in` & `libexe-20240420/po/Makevars.in`

 * *Files identical despite different names*

### Comparing `libexe-20240205/po/Rules-quot` & `libexe-20240420/po/Rules-quot`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libuna/libuna_codepage_windows_1251.c` & `libexe-20240420/libuna/libuna_codepage_windows_1251.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libuna/libuna_utf16_string.c` & `libexe-20240420/libuna/libuna_utf16_string.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libuna/libuna_base16_stream.c` & `libexe-20240420/libuna/libuna_base16_stream.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libuna/libuna_utf8_stream.h` & `libexe-20240420/libuna/libuna_utf8_stream.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libuna/libuna_codepage_iso_8859_2.h` & `libexe-20240420/libuna/libuna_codepage_iso_8859_2.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libuna/libuna_codepage_windows_932.c` & `libexe-20240420/libuna/libuna_codepage_windows_932.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libuna/libuna_codepage_mac_dingbats.h` & `libexe-20240420/libuna/libuna_codepage_mac_dingbats.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libuna/libuna_utf8_string.c` & `libexe-20240420/libuna/libuna_utf8_string.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libuna/libuna_base64_stream.c` & `libexe-20240420/libuna/libuna_base64_stream.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libuna/libuna_error.h` & `libexe-20240420/libuna/libuna_error.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libuna/libuna_codepage_mac_turkish.h` & `libexe-20240420/libuna/libuna_codepage_mac_turkish.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libuna/libuna_unicode_character.c` & `libexe-20240420/libuna/libuna_unicode_character.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libuna/libuna_codepage_mac_gaelic.c` & `libexe-20240420/libuna/libuna_codepage_mac_gaelic.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libuna/libuna_codepage_mac_arabic.h` & `libexe-20240420/libuna/libuna_codepage_mac_arabic.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libuna/libuna_codepage_mac_thai.c` & `libexe-20240420/libuna/libuna_codepage_mac_thai.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libuna/libuna_codepage_windows_874.h` & `libexe-20240420/libuna/libuna_codepage_windows_874.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libuna/libuna_codepage_iso_8859_15.h` & `libexe-20240420/libuna/libuna_codepage_iso_8859_15.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libuna/libuna_utf8_string.h` & `libexe-20240420/libuna/libuna_utf8_string.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libuna/libuna_codepage_iso_8859_16.c` & `libexe-20240420/libuna/libuna_codepage_iso_8859_16.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libuna/libuna_codepage_windows_1255.c` & `libexe-20240420/libuna/libuna_codepage_windows_1255.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libuna/libuna_utf7_stream.c` & `libexe-20240420/libuna/libuna_utf7_stream.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libuna/libuna_byte_stream.h` & `libexe-20240420/libuna/libuna_byte_stream.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libuna/libuna_codepage_koi8_u.c` & `libexe-20240420/libuna/libuna_codepage_koi8_u.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libuna/libuna_unused.h` & `libexe-20240420/libuna/libuna_unused.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libuna/libuna_codepage_iso_8859_6.c` & `libexe-20240420/libuna/libuna_codepage_iso_8859_6.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libuna/libuna_codepage_iso_8859_14.c` & `libexe-20240420/libuna/libuna_codepage_iso_8859_14.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libuna/libuna_base64_stream.h` & `libexe-20240420/libuna/libuna_base64_stream.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libuna/libuna_error.c` & `libexe-20240420/libuna/libuna_error.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libuna/libuna_codepage_mac_centraleurroman.h` & `libexe-20240420/libuna/libuna_codepage_mac_centraleurroman.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libuna/libuna_codepage_mac_romanian.c` & `libexe-20240420/libuna/libuna_codepage_mac_romanian.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libuna/libuna_codepage_iso_8859_6.h` & `libexe-20240420/libuna/libuna_codepage_iso_8859_6.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libuna/libuna_codepage_iso_8859_9.c` & `libexe-20240420/libuna/libuna_codepage_iso_8859_9.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libuna/libuna_codepage_mac_russian.h` & `libexe-20240420/libuna/libuna_codepage_mac_russian.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libuna/libuna_codepage_mac_dingbats.c` & `libexe-20240420/libuna/libuna_codepage_mac_dingbats.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libuna/libuna_codepage_iso_8859_15.c` & `libexe-20240420/libuna/libuna_codepage_iso_8859_15.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libuna/libuna_codepage_windows_936.c` & `libexe-20240420/libuna/libuna_codepage_windows_936.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libuna/libuna_codepage_mac_croatian.h` & `libexe-20240420/libuna/libuna_codepage_mac_croatian.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libuna/libuna_scsu.h` & `libexe-20240420/libuna/libuna_scsu.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libuna/Makefile.am` & `libexe-20240420/libuna/Makefile.am`

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

### Comparing `libexe-20240205/libuna/libuna_utf32_stream.c` & `libexe-20240420/libuna/libuna_utf32_stream.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libuna/libuna_codepage_windows_936.h` & `libexe-20240420/libuna/libuna_codepage_windows_936.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libuna/libuna_codepage_iso_8859_10.c` & `libexe-20240420/libuna/libuna_codepage_iso_8859_10.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libuna/libuna_codepage_mac_roman.c` & `libexe-20240420/libuna/libuna_codepage_mac_roman.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libuna/libuna_utf7_stream.h` & `libexe-20240420/libuna/libuna_utf7_stream.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libuna/libuna_codepage_iso_8859_3.h` & `libexe-20240420/libuna/libuna_codepage_iso_8859_3.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libuna/libuna_codepage_mac_thai.h` & `libexe-20240420/libuna/libuna_codepage_mac_thai.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libuna/libuna_codepage_mac_farsi.h` & `libexe-20240420/libuna/libuna_codepage_mac_farsi.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libuna/libuna_codepage_mac_ukrainian.c` & `libexe-20240420/libuna/libuna_codepage_mac_ukrainian.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libuna/libuna_codepage_mac_inuit.c` & `libexe-20240420/libuna/libuna_codepage_mac_inuit.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libuna/libuna_codepage_windows_932.h` & `libexe-20240420/libuna/libuna_codepage_windows_932.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libuna/libuna_codepage_windows_874.c` & `libexe-20240420/libuna/libuna_codepage_windows_874.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libuna/libuna_codepage_iso_8859_5.c` & `libexe-20240420/libuna/libuna_codepage_iso_8859_5.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libuna/libuna_codepage_iso_8859_10.h` & `libexe-20240420/libuna/libuna_codepage_iso_8859_10.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libuna/libuna_definitions.h` & `libexe-20240420/libuna/libuna_definitions.h`

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

### Comparing `libexe-20240205/libuna/libuna_url_stream.h` & `libexe-20240420/libuna/libuna_url_stream.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libuna/libuna_codepage_mac_icelandic.h` & `libexe-20240420/libuna/libuna_codepage_mac_icelandic.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libuna/libuna_codepage_koi8_u.h` & `libexe-20240420/libuna/libuna_codepage_koi8_u.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libuna/libuna_utf16_stream.c` & `libexe-20240420/libuna/libuna_utf16_stream.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libuna/libuna_codepage_windows_1253.c` & `libexe-20240420/libuna/libuna_codepage_windows_1253.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libuna/libuna_codepage_iso_8859_4.h` & `libexe-20240420/libuna/libuna_codepage_iso_8859_4.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libuna/libuna_codepage_mac_greek.c` & `libexe-20240420/libuna/libuna_codepage_mac_greek.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libuna/libuna_libcerror.h` & `libexe-20240420/libuna/libuna_libcerror.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libuna/libuna_codepage_mac_centraleurroman.c` & `libexe-20240420/libuna/libuna_codepage_mac_centraleurroman.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libuna/libuna_codepage_windows_1254.c` & `libexe-20240420/libuna/libuna_codepage_windows_1254.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libuna/libuna_codepage_iso_8859_13.h` & `libexe-20240420/libuna/libuna_codepage_iso_8859_13.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libuna/libuna_codepage_iso_8859_7.h` & `libexe-20240420/libuna/libuna_codepage_iso_8859_7.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libuna/libuna_codepage_windows_1255.h` & `libexe-20240420/libuna/libuna_codepage_windows_1255.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libuna/libuna_unicode_character.h` & `libexe-20240420/libuna/libuna_unicode_character.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libuna/libuna_codepage_iso_8859_8.h` & `libexe-20240420/libuna/libuna_codepage_iso_8859_8.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libuna/libuna_codepage_iso_8859_13.c` & `libexe-20240420/libuna/libuna_codepage_iso_8859_13.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libuna/libuna_codepage_windows_949.h` & `libexe-20240420/libuna/libuna_codepage_windows_949.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libuna/libuna_codepage_mac_cyrillic.c` & `libexe-20240420/libuna/libuna_codepage_mac_cyrillic.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libuna/libuna_codepage_mac_celtic.c` & `libexe-20240420/libuna/libuna_codepage_mac_celtic.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libuna/libuna_support.h` & `libexe-20240420/libuna/libuna_support.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libuna/libuna_codepage_iso_8859_4.c` & `libexe-20240420/libuna/libuna_codepage_iso_8859_4.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libuna/libuna_codepage_windows_949.c` & `libexe-20240420/libuna/libuna_codepage_windows_949.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libuna/libuna_utf16_stream.h` & `libexe-20240420/libuna/libuna_utf16_stream.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libuna/libuna_codepage_mac_symbol.c` & `libexe-20240420/libuna/libuna_codepage_mac_symbol.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libuna/libuna_codepage_mac_roman.h` & `libexe-20240420/libuna/libuna_codepage_mac_roman.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libuna/libuna_codepage_windows_1257.c` & `libexe-20240420/libuna/libuna_codepage_windows_1257.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libuna/libuna_codepage_windows_1254.h` & `libexe-20240420/libuna/libuna_codepage_windows_1254.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libuna/libuna_codepage_windows_950.c` & `libexe-20240420/libuna/libuna_codepage_windows_950.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libuna/libuna_extern.h` & `libexe-20240420/libuna/libuna_extern.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libuna/libuna_codepage_windows_1256.c` & `libexe-20240420/libuna/libuna_codepage_windows_1256.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libuna/libuna_types.h` & `libexe-20240420/libuna/libuna_types.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libuna/libuna_base32_stream.h` & `libexe-20240420/libuna/libuna_base32_stream.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libuna/libuna_codepage_windows_1253.h` & `libexe-20240420/libuna/libuna_codepage_windows_1253.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libuna/libuna_codepage_iso_8859_16.h` & `libexe-20240420/libuna/libuna_codepage_iso_8859_16.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libuna/libuna_utf8_stream.c` & `libexe-20240420/libuna/libuna_utf8_stream.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libuna/libuna_codepage_windows_1250.h` & `libexe-20240420/libuna/libuna_codepage_windows_1250.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libuna/libuna_codepage_iso_8859_2.c` & `libexe-20240420/libuna/libuna_codepage_iso_8859_2.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libuna/libuna_support.c` & `libexe-20240420/libuna/libuna_support.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libuna/libuna_codepage_koi8_r.c` & `libexe-20240420/libuna/libuna_codepage_koi8_r.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libuna/libuna_codepage_iso_8859_5.h` & `libexe-20240420/libuna/libuna_codepage_iso_8859_5.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libuna/libuna_utf16_string.h` & `libexe-20240420/libuna/libuna_utf16_string.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libuna/libuna_utf32_string.c` & `libexe-20240420/libuna/libuna_utf32_string.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libuna/libuna_codepage_mac_icelandic.c` & `libexe-20240420/libuna/libuna_codepage_mac_icelandic.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libuna/libuna_codepage_windows_1256.h` & `libexe-20240420/libuna/libuna_codepage_windows_1256.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libuna/libuna_utf32_string.h` & `libexe-20240420/libuna/libuna_utf32_string.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libuna/libuna_codepage_mac_romanian.h` & `libexe-20240420/libuna/libuna_codepage_mac_romanian.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libuna/libuna_codepage_iso_8859_8.c` & `libexe-20240420/libuna/libuna_codepage_iso_8859_8.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libuna/libuna_codepage_koi8_r.h` & `libexe-20240420/libuna/libuna_codepage_koi8_r.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libuna/libuna_codepage_mac_cyrillic.h` & `libexe-20240420/libuna/libuna_codepage_mac_cyrillic.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libuna/libuna_codepage_mac_arabic.c` & `libexe-20240420/libuna/libuna_codepage_mac_arabic.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libuna/libuna_codepage_mac_croatian.c` & `libexe-20240420/libuna/libuna_codepage_mac_croatian.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libuna/libuna_codepage_iso_8859_9.h` & `libexe-20240420/libuna/libuna_codepage_iso_8859_9.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libuna/libuna_codepage_mac_greek.h` & `libexe-20240420/libuna/libuna_codepage_mac_greek.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libuna/libuna_codepage_windows_1258.h` & `libexe-20240420/libuna/libuna_codepage_windows_1258.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libuna/libuna_codepage_iso_8859_7.c` & `libexe-20240420/libuna/libuna_codepage_iso_8859_7.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libuna/Makefile.in` & `libexe-20240420/libuna/Makefile.in`

 * *Files 11% similar despite different names*

```diff
@@ -670,16 +670,16 @@
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
@@ -745,15 +745,16 @@
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
@@ -1015,24 +1016,89 @@
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
 
@@ -1178,17 +1244,14 @@
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

### Comparing `libexe-20240205/libuna/libuna_codepage_iso_8859_3.c` & `libexe-20240420/libuna/libuna_codepage_iso_8859_3.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libuna/libuna_codepage_windows_1250.c` & `libexe-20240420/libuna/libuna_codepage_windows_1250.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libuna/libuna_scsu.c` & `libexe-20240420/libuna/libuna_scsu.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libuna/libuna_codepage_windows_1252.c` & `libexe-20240420/libuna/libuna_codepage_windows_1252.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libuna/libuna_codepage_mac_turkish.c` & `libexe-20240420/libuna/libuna_codepage_mac_turkish.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libuna/libuna_codepage_mac_ukrainian.h` & `libexe-20240420/libuna/libuna_codepage_mac_ukrainian.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libuna/libuna_codepage_mac_russian.c` & `libexe-20240420/libuna/libuna_codepage_mac_russian.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libuna/libuna_codepage_windows_1258.c` & `libexe-20240420/libuna/libuna_codepage_windows_1258.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libuna/libuna_codepage_mac_celtic.h` & `libexe-20240420/libuna/libuna_codepage_mac_celtic.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libuna/libuna_byte_stream.c` & `libexe-20240420/libuna/libuna_byte_stream.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libuna/libuna_codepage_mac_gaelic.h` & `libexe-20240420/libuna/libuna_codepage_mac_gaelic.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libuna/libuna_utf32_stream.h` & `libexe-20240420/libuna/libuna_utf32_stream.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libuna/libuna_codepage_mac_symbol.h` & `libexe-20240420/libuna/libuna_codepage_mac_symbol.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libuna/libuna_codepage_windows_1257.h` & `libexe-20240420/libuna/libuna_codepage_windows_1257.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libuna/libuna_codepage_mac_inuit.h` & `libexe-20240420/libuna/libuna_codepage_mac_inuit.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libuna/libuna_codepage_mac_farsi.c` & `libexe-20240420/libuna/libuna_codepage_mac_farsi.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libuna/libuna_codepage_windows_950.h` & `libexe-20240420/libuna/libuna_codepage_windows_950.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libuna/libuna_url_stream.c` & `libexe-20240420/libuna/libuna_url_stream.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libuna/libuna_codepage_windows_1251.h` & `libexe-20240420/libuna/libuna_codepage_windows_1251.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libuna/libuna_codepage_windows_1252.h` & `libexe-20240420/libuna/libuna_codepage_windows_1252.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libuna/libuna_codepage_iso_8859_14.h` & `libexe-20240420/libuna/libuna_codepage_iso_8859_14.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libuna/libuna_base16_stream.h` & `libexe-20240420/libuna/libuna_base16_stream.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libuna/libuna_base32_stream.c` & `libexe-20240420/libuna/libuna_base32_stream.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/Makefile.in` & `libexe-20240420/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -614,16 +614,23 @@
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
+	libexe.pc \
+	libexe.spec \
+	Makefile \
+	Makefile.in \
+	po/Makevars
 
 pkgconfigdir = $(libdir)/pkgconfig
 pkgconfig_DATA = \
 	libexe.pc
 
 all: all-recursive
 
@@ -1040,23 +1047,26 @@
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
 
@@ -1166,22 +1176,10 @@
 	(cd $(srcdir)/libbfio && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libfcache && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libfdata && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libfdatetime && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libexe && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/po && $(MAKE) $(AM_MAKEFLAGS))
 
-distclean: clean
-	-rm -f Makefile
-	-rm -f config.status
-	-rm -f config.cache
-	-rm -f config.log
-	-rm -f libexe.pc
-	-rm -f libexe.spec
-	@for dir in ${subdirs}; do \
-		(cd $$dir && $(MAKE) distclean) \
-		|| case "$(MFLAGS)" in *k*) fail=yes;; *) exit 1;; esac; \
-	done && test -z "$$fail"
-
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libexe-20240205/pyexe/pyexe_file.h` & `libexe-20240420/pyexe/pyexe_file.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/pyexe/pyexe_sections.h` & `libexe-20240420/pyexe/pyexe_sections.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/pyexe/pyexe_file_object_io_handle.c` & `libexe-20240420/pyexe/pyexe_file_object_io_handle.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/pyexe/pyexe_datetime.c` & `libexe-20240420/pyexe/pyexe_datetime.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/pyexe/pyexe_libcerror.h` & `libexe-20240420/pyexe/pyexe_libcerror.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/pyexe/pyexe_section.h` & `libexe-20240420/pyexe/pyexe_section.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/pyexe/pyexe_codepage.h` & `libexe-20240420/pyexe/pyexe_codepage.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/pyexe/pyexe_libbfio.h` & `libexe-20240420/pyexe/pyexe_libbfio.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/pyexe/Makefile.am` & `libexe-20240420/pyexe/Makefile.am`

 * *Files 16% similar despite different names*

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
@@ -43,13 +43,11 @@
 	@LIBBFIO_LIBADD@
 
 pyexe_la_CPPFLAGS = $(PYTHON_CPPFLAGS)
 pyexe_la_LDFLAGS  = -module -avoid-version $(PYTHON_LDFLAGS)
 
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
```

### Comparing `libexe-20240205/pyexe/pyexe_error.c` & `libexe-20240420/pyexe/pyexe_error.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/pyexe/pyexe_unused.h` & `libexe-20240420/pyexe/pyexe_unused.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/pyexe/pyexe.c` & `libexe-20240420/pyexe/pyexe.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/pyexe/pyexe_integer.h` & `libexe-20240420/pyexe/pyexe_integer.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/pyexe/pyexe_libexe.h` & `libexe-20240420/pyexe/pyexe_libexe.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/pyexe/pyexe_python.h` & `libexe-20240420/pyexe/pyexe_python.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/pyexe/pyexe_libclocale.h` & `libexe-20240420/pyexe/pyexe_libclocale.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/pyexe/pyexe.h` & `libexe-20240420/pyexe/pyexe.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/pyexe/pyexe_integer.c` & `libexe-20240420/pyexe/pyexe_integer.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/pyexe/pyexe_codepage.c` & `libexe-20240420/pyexe/pyexe_codepage.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/pyexe/pyexe_file_object_io_handle.h` & `libexe-20240420/pyexe/pyexe_file_object_io_handle.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/pyexe/pyexe_file.c` & `libexe-20240420/pyexe/pyexe_file.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/pyexe/pyexe_sections.c` & `libexe-20240420/pyexe/pyexe_sections.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/pyexe/pyexe_datetime.h` & `libexe-20240420/pyexe/pyexe_datetime.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/pyexe/pyexe_section.c` & `libexe-20240420/pyexe/pyexe_section.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/pyexe/Makefile.in` & `libexe-20240420/pyexe/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -537,16 +537,16 @@
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
@@ -580,15 +580,16 @@
 @HAVE_PYTHON_TRUE@	@LIBUNA_LIBADD@ \
 @HAVE_PYTHON_TRUE@	@LIBCFILE_LIBADD@ \
 @HAVE_PYTHON_TRUE@	@LIBCPATH_LIBADD@ \
 @HAVE_PYTHON_TRUE@	@LIBBFIO_LIBADD@
 
 @HAVE_PYTHON_TRUE@pyexe_la_CPPFLAGS = $(PYTHON_CPPFLAGS)
 @HAVE_PYTHON_TRUE@pyexe_la_LDFLAGS = -module -avoid-version $(PYTHON_LDFLAGS)
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -886,24 +887,35 @@
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
+		-rm -f ./$(DEPDIR)/pyexe_la-pyexe.Plo
+	-rm -f ./$(DEPDIR)/pyexe_la-pyexe_codepage.Plo
+	-rm -f ./$(DEPDIR)/pyexe_la-pyexe_datetime.Plo
+	-rm -f ./$(DEPDIR)/pyexe_la-pyexe_error.Plo
+	-rm -f ./$(DEPDIR)/pyexe_la-pyexe_file.Plo
+	-rm -f ./$(DEPDIR)/pyexe_la-pyexe_file_object_io_handle.Plo
+	-rm -f ./$(DEPDIR)/pyexe_la-pyexe_integer.Plo
+	-rm -f ./$(DEPDIR)/pyexe_la-pyexe_section.Plo
+	-rm -f ./$(DEPDIR)/pyexe_la-pyexe_sections.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -996,13 +1008,10 @@
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

### Comparing `libexe-20240205/pyexe/pyexe_error.h` & `libexe-20240420/pyexe/pyexe_error.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libcnotify/libcnotify_definitions.h` & `libexe-20240420/libcnotify/libcnotify_definitions.h`

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

### Comparing `libexe-20240205/libcnotify/libcnotify_extern.h` & `libexe-20240420/libcnotify/libcnotify_extern.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libcnotify/libcnotify_support.c` & `libexe-20240420/libcnotify/libcnotify_support.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libcnotify/libcnotify_stream.h` & `libexe-20240420/libcnotify/libcnotify_stream.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libcnotify/Makefile.am` & `libexe-20240420/libcnotify/Makefile.am`

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

### Comparing `libexe-20240205/libcnotify/libcnotify_unused.h` & `libexe-20240420/libcnotify/libcnotify_unused.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libcnotify/libcnotify_verbose.h` & `libexe-20240420/libcnotify/libcnotify_verbose.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libcnotify/libcnotify_print.h` & `libexe-20240420/libcnotify/libcnotify_print.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libcnotify/libcnotify_stream.c` & `libexe-20240420/libcnotify/libcnotify_stream.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libcnotify/libcnotify_support.h` & `libexe-20240420/libcnotify/libcnotify_support.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libcnotify/libcnotify_verbose.c` & `libexe-20240420/libcnotify/libcnotify_verbose.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libcnotify/Makefile.in` & `libexe-20240420/libcnotify/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -494,30 +494,31 @@
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
@@ -720,24 +721,30 @@
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
 
@@ -824,17 +831,14 @@
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

### Comparing `libexe-20240205/libcnotify/libcnotify_libcerror.h` & `libexe-20240420/libcnotify/libcnotify_libcerror.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libcnotify/libcnotify_print.c` & `libexe-20240420/libcnotify/libcnotify_print.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libcerror/libcerror_system.c` & `libexe-20240420/libcerror/libcerror_system.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libcerror/libcerror_error.c` & `libexe-20240420/libcerror/libcerror_error.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libcerror/libcerror_extern.h` & `libexe-20240420/libcerror/libcerror_extern.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libcerror/Makefile.am` & `libexe-20240420/libcerror/Makefile.am`

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

### Comparing `libexe-20240205/libcerror/libcerror_types.h` & `libexe-20240420/libcerror/libcerror_types.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libcerror/libcerror_support.h` & `libexe-20240420/libcerror/libcerror_support.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libcerror/libcerror_error.h` & `libexe-20240420/libcerror/libcerror_error.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libcerror/libcerror_system.h` & `libexe-20240420/libcerror/libcerror_system.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libcerror/libcerror_definitions.h` & `libexe-20240420/libcerror/libcerror_definitions.h`

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

### Comparing `libexe-20240205/libcerror/libcerror_support.c` & `libexe-20240420/libcerror/libcerror_support.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libcerror/libcerror_unused.h` & `libexe-20240420/libcerror/libcerror_unused.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libcerror/Makefile.in` & `libexe-20240420/libcerror/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -491,28 +491,29 @@
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
@@ -714,24 +715,29 @@
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
 
@@ -817,17 +823,14 @@
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

### Comparing `libexe-20240205/libfdatetime/libfdatetime_floatingtime.h` & `libexe-20240420/libfdatetime/libfdatetime_floatingtime.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libfdatetime/libfdatetime_nsf_timedate.c` & `libexe-20240420/libfdatetime/libfdatetime_nsf_timedate.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libfdatetime/libfdatetime_error.h` & `libexe-20240420/libfdatetime/libfdatetime_error.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libfdatetime/libfdatetime_floatingtime.c` & `libexe-20240420/libfdatetime/libfdatetime_floatingtime.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libfdatetime/libfdatetime_support.h` & `libexe-20240420/libfdatetime/libfdatetime_support.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libfdatetime/libfdatetime_hfs_time.h` & `libexe-20240420/libfdatetime/libfdatetime_hfs_time.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libfdatetime/libfdatetime_definitions.h` & `libexe-20240420/libfdatetime/libfdatetime_definitions.h`

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

### Comparing `libexe-20240205/libfdatetime/libfdatetime_hfs_time.c` & `libexe-20240420/libfdatetime/libfdatetime_hfs_time.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libfdatetime/Makefile.am` & `libexe-20240420/libfdatetime/Makefile.am`

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

### Comparing `libexe-20240205/libfdatetime/libfdatetime_filetime.c` & `libexe-20240420/libfdatetime/libfdatetime_filetime.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libfdatetime/libfdatetime_systemtime.h` & `libexe-20240420/libfdatetime/libfdatetime_systemtime.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libfdatetime/libfdatetime_extern.h` & `libexe-20240420/libfdatetime/libfdatetime_extern.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libfdatetime/libfdatetime_posix_time.c` & `libexe-20240420/libfdatetime/libfdatetime_posix_time.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libfdatetime/libfdatetime_unused.h` & `libexe-20240420/libfdatetime/libfdatetime_unused.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libfdatetime/libfdatetime_fat_date_time.h` & `libexe-20240420/libfdatetime/libfdatetime_fat_date_time.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libfdatetime/libfdatetime_systemtime.c` & `libexe-20240420/libfdatetime/libfdatetime_systemtime.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libfdatetime/libfdatetime_nsf_timedate.h` & `libexe-20240420/libfdatetime/libfdatetime_nsf_timedate.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libfdatetime/libfdatetime_libcerror.h` & `libexe-20240420/libfdatetime/libfdatetime_libcerror.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libfdatetime/libfdatetime_support.c` & `libexe-20240420/libfdatetime/libfdatetime_support.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libfdatetime/libfdatetime_error.c` & `libexe-20240420/libfdatetime/libfdatetime_error.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libfdatetime/libfdatetime_posix_time.h` & `libexe-20240420/libfdatetime/libfdatetime_posix_time.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libfdatetime/libfdatetime_date_time_values.h` & `libexe-20240420/libfdatetime/libfdatetime_date_time_values.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libfdatetime/libfdatetime_filetime.h` & `libexe-20240420/libfdatetime/libfdatetime_filetime.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libfdatetime/libfdatetime_date_time_values.c` & `libexe-20240420/libfdatetime/libfdatetime_date_time_values.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libfdatetime/libfdatetime_types.h` & `libexe-20240420/libfdatetime/libfdatetime_types.h`

 * *Files identical despite different names*

### Comparing `libexe-20240205/libfdatetime/Makefile.in` & `libexe-20240420/libfdatetime/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -513,16 +513,16 @@
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
@@ -535,15 +535,16 @@
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
@@ -752,24 +753,36 @@
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
 
@@ -862,17 +875,14 @@
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

### Comparing `libexe-20240205/libfdatetime/libfdatetime_fat_date_time.c` & `libexe-20240420/libfdatetime/libfdatetime_fat_date_time.c`

 * *Files identical despite different names*

### Comparing `libexe-20240205/aclocal.m4` & `libexe-20240420/aclocal.m4`

 * *Files identical despite different names*

### Comparing `libexe-20240205/configure.ac` & `libexe-20240420/configure.ac`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 AC_PREREQ([2.71])
 
 AC_INIT(
  [libexe],
- [20240205],
+ [20240420],
  [joachim.metz@gmail.com])
 
 AC_CONFIG_SRCDIR(
  [include/libexe.h.in])
 
 AM_INIT_AUTOMAKE([gnu 1.6 tar-ustar])
 AM_EXTRA_RECURSIVE_TARGETS([sources splint])
```

