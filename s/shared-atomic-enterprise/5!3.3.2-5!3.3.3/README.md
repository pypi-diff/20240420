# Comparing `tmp/shared_atomic_enterprise-5!3.3.2-pp39-none-win_amd64.whl.zip` & `tmp/shared_atomic_enterprise-5!3.3.3-cp37-none-win_amd64.whl.zip`

## zipinfo -v {}

 * *Differences in extra fields detected; using output from zipinfo -v*

```diff
@@ -1,22 +1,22 @@
 There is no zipfile comment.
 
 End-of-central-directory record:
 -------------------------------
 
-  Zip archive file size:                   6254582 (00000000005F6FF6h)
-  Actual end-cent-dir record offset:       6254560 (00000000005F6FE0h)
-  Expected end-cent-dir record offset:     6254560 (00000000005F6FE0h)
+  Zip archive file size:                   2659129 (0000000000289339h)
+  Actual end-cent-dir record offset:       2659107 (0000000000289323h)
+  Expected end-cent-dir record offset:     2659107 (0000000000289323h)
   (based on the length of the central directory and its expected offset)
 
   This zipfile constitutes the sole disk of a single-part archive; its
-  central directory contains 47 entries.
-  The central directory is 4875 (000000000000130Bh) bytes long,
+  central directory contains 36 entries.
+  The central directory is 3697 (0000000000000E71h) bytes long,
   and its (expected) offset in bytes from the beginning of the zipfile
-  is 6249685 (00000000005F5CD5h).
+  is 2655410 (00000000002884B2h).
 
 
 Central directory entry #1:
 ---------------------------
 
   shared_atomic/
 
@@ -25,205 +25,168 @@
   file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   1.0
   compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Sep 7 21:06:08
-  file last modified on (UT extra field modtime): 2023 Sep 7 13:06:07 local
-  file last modified on (UT extra field modtime): 2023 Sep 7 13:06:07 UTC
+  file last modified on (DOS date/time):          2024 Apr 20 13:29:28
+  file last modified on (UT extra field modtime): 2024 Apr 20 05:29:28 local
+  file last modified on (UT extra field modtime): 2024 Apr 20 05:29:28 UTC
   32-bit CRC value (hex):                         00000000
   compressed size:                                0 bytes
   uncompressed size:                              0 bytes
   length of filename:                             14 characters
   length of extra field:                          17 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             binary
   non-MSDOS external file attributes:             000000 hex
   MS-DOS file attributes (10 hex):                dir 
 
   The central-directory extra field contains:
   - A subfield with ID 0x4453 (Security Descriptor) and 4 data bytes.
-    The local extra field has 152 bytes of NT security descriptor data.
+    The local extra field has 164 bytes of NT security descriptor data.
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access/creation times.
 
   There is no file comment.
 
 Central directory entry #2:
 ---------------------------
 
-  shared_atomic/atomic_activation.pypy39-pp73-win_amd64.pyd
+  shared_atomic/atomic_activation.cp37-win_amd64.pyd
 
   offset of local header from start of archive:   158
                                                   (000000000000009Eh) bytes
   file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Sep 7 21:00:20
-  file last modified on (UT extra field modtime): 2023 Sep 7 13:00:19 local
-  file last modified on (UT extra field modtime): 2023 Sep 7 13:00:19 UTC
-  32-bit CRC value (hex):                         a32dcc78
-  compressed size:                                163972 bytes
-  uncompressed size:                              412672 bytes
-  length of filename:                             57 characters
+  file last modified on (DOS date/time):          2024 Apr 20 13:26:22
+  file last modified on (UT extra field modtime): 2024 Apr 20 05:26:22 local
+  file last modified on (UT extra field modtime): 2024 Apr 20 05:26:22 UTC
+  32-bit CRC value (hex):                         31179710
+  compressed size:                                432308 bytes
+  uncompressed size:                              1147392 bytes
+  length of filename:                             50 characters
   length of extra field:                          17 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             binary
   non-MSDOS external file attributes:             000000 hex
   MS-DOS file attributes (20 hex):                arc 
 
   The central-directory extra field contains:
   - A subfield with ID 0x4453 (Security Descriptor) and 4 data bytes.
-    The local extra field has 152 bytes of NT security descriptor data.
+    The local extra field has 164 bytes of NT security descriptor data.
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access/creation times.
 
   There is no file comment.
 
 Central directory entry #3:
 ---------------------------
 
-  shared_atomic/atomic_activation_cpython.cp39-win_amd64.pyd
+  shared_atomic/atomic_async_activation_check.cp37-win_amd64.pyd
 
-  offset of local header from start of archive:   164331
-                                                  (00000000000281EBh) bytes
+  offset of local header from start of archive:   432660
+                                                  (0000000000069A14h) bytes
   file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Sep 7 20:58:24
-  file last modified on (UT extra field modtime): 2023 Sep 7 12:58:24 local
-  file last modified on (UT extra field modtime): 2023 Sep 7 12:58:24 UTC
-  32-bit CRC value (hex):                         aae6cc8b
-  compressed size:                                271389 bytes
-  uncompressed size:                              677376 bytes
-  length of filename:                             58 characters
+  file last modified on (DOS date/time):          2024 Apr 20 13:27:28
+  file last modified on (UT extra field modtime): 2024 Apr 20 05:27:27 local
+  file last modified on (UT extra field modtime): 2024 Apr 20 05:27:27 UTC
+  32-bit CRC value (hex):                         31f5e4ef
+  compressed size:                                209265 bytes
+  uncompressed size:                              552448 bytes
+  length of filename:                             62 characters
   length of extra field:                          17 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             binary
   non-MSDOS external file attributes:             000000 hex
   MS-DOS file attributes (20 hex):                arc 
 
   The central-directory extra field contains:
   - A subfield with ID 0x4453 (Security Descriptor) and 4 data bytes.
-    The local extra field has 152 bytes of NT security descriptor data.
+    The local extra field has 164 bytes of NT security descriptor data.
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access/creation times.
 
   There is no file comment.
 
 Central directory entry #4:
 ---------------------------
 
-  shared_atomic/atomic_activation_cpython_wrapper.exe
+  shared_atomic/atomic_boolfloat.cp37-win_amd64.pyd
 
-  offset of local header from start of archive:   435922
-                                                  (000000000006A6D2h) bytes
+  offset of local header from start of archive:   642131
+                                                  (000000000009CC53h) bytes
   file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Sep 7 20:58:28
-  file last modified on (UT extra field modtime): 2023 Sep 7 12:58:28 local
-  file last modified on (UT extra field modtime): 2023 Sep 7 12:58:28 UTC
-  32-bit CRC value (hex):                         17f6b166
-  compressed size:                                7197 bytes
-  uncompressed size:                              15872 bytes
-  length of filename:                             51 characters
+  file last modified on (DOS date/time):          2024 Apr 20 13:28:10
+  file last modified on (UT extra field modtime): 2024 Apr 20 05:28:10 local
+  file last modified on (UT extra field modtime): 2024 Apr 20 05:28:10 UTC
+  32-bit CRC value (hex):                         7c8184de
+  compressed size:                                34179 bytes
+  uncompressed size:                              76800 bytes
+  length of filename:                             49 characters
   length of extra field:                          17 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             binary
   non-MSDOS external file attributes:             000000 hex
   MS-DOS file attributes (20 hex):                arc 
 
   The central-directory extra field contains:
   - A subfield with ID 0x4453 (Security Descriptor) and 4 data bytes.
-    The local extra field has 152 bytes of NT security descriptor data.
+    The local extra field has 164 bytes of NT security descriptor data.
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access/creation times.
 
   There is no file comment.
 
 Central directory entry #5:
 ---------------------------
 
-  shared_atomic/atomic_async_activation_check.pypy39-pp73-win_amd64.pyd
-
-  offset of local header from start of archive:   443314
-                                                  (000000000006C3B2h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   3.0
-  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   2.0
-  compression method:                             deflated
-  compression sub-type (deflation):               normal
-  file security status:                           not encrypted
-  extended local header:                          no
-  file last modified on (DOS date/time):          2023 Sep 7 21:01:20
-  file last modified on (UT extra field modtime): 2023 Sep 7 13:01:20 local
-  file last modified on (UT extra field modtime): 2023 Sep 7 13:01:20 UTC
-  32-bit CRC value (hex):                         b5966db4
-  compressed size:                                168877 bytes
-  uncompressed size:                              425984 bytes
-  length of filename:                             69 characters
-  length of extra field:                          17 bytes
-  length of file comment:                         0 characters
-  disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  non-MSDOS external file attributes:             000000 hex
-  MS-DOS file attributes (20 hex):                arc 
-
-  The central-directory extra field contains:
-  - A subfield with ID 0x4453 (Security Descriptor) and 4 data bytes.
-    The local extra field has 152 bytes of NT security descriptor data.
-  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
-    The local extra field has UTC/GMT modification/access/creation times.
-
-  There is no file comment.
-
-Central directory entry #6:
----------------------------
-
   shared_atomic/atomic_boolfloat.pxd
 
-  offset of local header from start of archive:   612404
-                                                  (0000000000095834h) bytes
+  offset of local header from start of archive:   676503
+                                                  (00000000000A5297h) bytes
   file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Aug 22 19:58:12
-  file last modified on (UT extra field modtime): 2023 Aug 22 11:58:11 local
-  file last modified on (UT extra field modtime): 2023 Aug 22 11:58:11 UTC
-  32-bit CRC value (hex):                         2bb0260d
-  compressed size:                                307 bytes
-  uncompressed size:                              1208 bytes
+  file last modified on (DOS date/time):          2023 May 21 15:11:28
+  file last modified on (UT extra field modtime): 2023 May 21 07:11:27 local
+  file last modified on (UT extra field modtime): 2023 May 21 07:11:27 UTC
+  32-bit CRC value (hex):                         062e805b
+  compressed size:                                202 bytes
+  uncompressed size:                              696 bytes
   length of filename:                             34 characters
   length of extra field:                          17 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   non-MSDOS external file attributes:             000000 hex
   MS-DOS file attributes (20 hex):                arc 
@@ -232,72 +195,72 @@
   - A subfield with ID 0x4453 (Security Descriptor) and 4 data bytes.
     The local extra field has 152 bytes of NT security descriptor data.
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access/creation times.
 
   There is no file comment.
 
-Central directory entry #7:
+Central directory entry #6:
 ---------------------------
 
-  shared_atomic/atomic_boolfloat.pypy39-pp73-win_amd64.pyd
+  shared_atomic/atomic_bytearray.cp37-win_amd64.pyd
 
-  offset of local header from start of archive:   612889
-                                                  (0000000000095A19h) bytes
+  offset of local header from start of archive:   676883
+                                                  (00000000000A5413h) bytes
   file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Sep 7 21:02:48
-  file last modified on (UT extra field modtime): 2023 Sep 7 13:02:47 local
-  file last modified on (UT extra field modtime): 2023 Sep 7 13:02:47 UTC
-  32-bit CRC value (hex):                         ac77f743
-  compressed size:                                27052 bytes
-  uncompressed size:                              61952 bytes
-  length of filename:                             56 characters
+  file last modified on (DOS date/time):          2024 Apr 20 13:28:22
+  file last modified on (UT extra field modtime): 2024 Apr 20 05:28:21 local
+  file last modified on (UT extra field modtime): 2024 Apr 20 05:28:21 UTC
+  32-bit CRC value (hex):                         aa0033bd
+  compressed size:                                61722 bytes
+  uncompressed size:                              168960 bytes
+  length of filename:                             49 characters
   length of extra field:                          17 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             binary
   non-MSDOS external file attributes:             000000 hex
   MS-DOS file attributes (20 hex):                arc 
 
   The central-directory extra field contains:
   - A subfield with ID 0x4453 (Security Descriptor) and 4 data bytes.
-    The local extra field has 152 bytes of NT security descriptor data.
+    The local extra field has 164 bytes of NT security descriptor data.
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access/creation times.
 
   There is no file comment.
 
-Central directory entry #8:
+Central directory entry #7:
 ---------------------------
 
   shared_atomic/atomic_bytearray.pxd
 
-  offset of local header from start of archive:   640141
-                                                  (000000000009C48Dh) bytes
+  offset of local header from start of archive:   738798
+                                                  (00000000000B45EEh) bytes
   file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Aug 22 19:58:12
-  file last modified on (UT extra field modtime): 2023 Aug 22 11:58:11 local
-  file last modified on (UT extra field modtime): 2023 Aug 22 11:58:11 UTC
-  32-bit CRC value (hex):                         fbc55022
-  compressed size:                                534 bytes
-  uncompressed size:                              3164 bytes
+  file last modified on (DOS date/time):          2023 Jun 1 11:02:56
+  file last modified on (UT extra field modtime): 2023 Jun 1 03:02:56 local
+  file last modified on (UT extra field modtime): 2023 Jun 1 03:02:56 UTC
+  32-bit CRC value (hex):                         e7f8dc6e
+  compressed size:                                421 bytes
+  uncompressed size:                              2659 bytes
   length of filename:                             34 characters
   length of extra field:                          17 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   non-MSDOS external file attributes:             000000 hex
   MS-DOS file attributes (20 hex):                arc 
@@ -306,146 +269,109 @@
   - A subfield with ID 0x4453 (Security Descriptor) and 4 data bytes.
     The local extra field has 152 bytes of NT security descriptor data.
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access/creation times.
 
   There is no file comment.
 
-Central directory entry #9:
----------------------------
-
-  shared_atomic/atomic_bytearray.pypy39-pp73-win_amd64.pyd
-
-  offset of local header from start of archive:   640853
-                                                  (000000000009C755h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   3.0
-  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   2.0
-  compression method:                             deflated
-  compression sub-type (deflation):               normal
-  file security status:                           not encrypted
-  extended local header:                          no
-  file last modified on (DOS date/time):          2023 Sep 7 21:03:18
-  file last modified on (UT extra field modtime): 2023 Sep 7 13:03:17 local
-  file last modified on (UT extra field modtime): 2023 Sep 7 13:03:17 UTC
-  32-bit CRC value (hex):                         84fdd747
-  compressed size:                                51728 bytes
-  uncompressed size:                              139776 bytes
-  length of filename:                             56 characters
-  length of extra field:                          17 bytes
-  length of file comment:                         0 characters
-  disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  non-MSDOS external file attributes:             000000 hex
-  MS-DOS file attributes (20 hex):                arc 
-
-  The central-directory extra field contains:
-  - A subfield with ID 0x4453 (Security Descriptor) and 4 data bytes.
-    The local extra field has 152 bytes of NT security descriptor data.
-  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
-    The local extra field has UTC/GMT modification/access/creation times.
-
-  There is no file comment.
-
-Central directory entry #10:
+Central directory entry #8:
 ---------------------------
 
-  shared_atomic/atomic_decryption_.cp39-win_amd64.pyd
+  shared_atomic/atomic_decryption_.cp37-win_amd64.pyd
 
-  offset of local header from start of archive:   692781
-                                                  (00000000000A922Dh) bytes
+  offset of local header from start of archive:   739397
+                                                  (00000000000B4845h) bytes
   file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Sep 7 20:57:38
-  file last modified on (UT extra field modtime): 2023 Sep 7 12:57:37 local
-  file last modified on (UT extra field modtime): 2023 Sep 7 12:57:37 UTC
-  32-bit CRC value (hex):                         46cbf7f5
-  compressed size:                                13739 bytes
-  uncompressed size:                              35328 bytes
+  file last modified on (DOS date/time):          2024 Apr 20 13:25:30
+  file last modified on (UT extra field modtime): 2024 Apr 20 05:25:30 local
+  file last modified on (UT extra field modtime): 2024 Apr 20 05:25:30 UTC
+  32-bit CRC value (hex):                         15b0443a
+  compressed size:                                13512 bytes
+  uncompressed size:                              34816 bytes
   length of filename:                             51 characters
   length of extra field:                          17 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             binary
   non-MSDOS external file attributes:             000000 hex
   MS-DOS file attributes (20 hex):                arc 
 
   The central-directory extra field contains:
   - A subfield with ID 0x4453 (Security Descriptor) and 4 data bytes.
-    The local extra field has 152 bytes of NT security descriptor data.
+    The local extra field has 164 bytes of NT security descriptor data.
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access/creation times.
 
   There is no file comment.
 
-Central directory entry #11:
+Central directory entry #9:
 ---------------------------
 
-  shared_atomic/atomic_decryption_.pypy39-pp73-win_amd64.pyd
+  shared_atomic/atomic_int.cp37-win_amd64.pyd
 
-  offset of local header from start of archive:   706715
-                                                  (00000000000AC89Bh) bytes
+  offset of local header from start of archive:   753104
+                                                  (00000000000B7DD0h) bytes
   file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Sep 7 20:57:26
-  file last modified on (UT extra field modtime): 2023 Sep 7 12:57:25 local
-  file last modified on (UT extra field modtime): 2023 Sep 7 12:57:25 UTC
-  32-bit CRC value (hex):                         274cd774
-  compressed size:                                6797 bytes
-  uncompressed size:                              15872 bytes
-  length of filename:                             58 characters
+  file last modified on (DOS date/time):          2024 Apr 20 13:28:34
+  file last modified on (UT extra field modtime): 2024 Apr 20 05:28:33 local
+  file last modified on (UT extra field modtime): 2024 Apr 20 05:28:33 UTC
+  32-bit CRC value (hex):                         2fdb81f9
+  compressed size:                                40313 bytes
+  uncompressed size:                              103424 bytes
+  length of filename:                             43 characters
   length of extra field:                          17 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             binary
   non-MSDOS external file attributes:             000000 hex
   MS-DOS file attributes (20 hex):                arc 
 
   The central-directory extra field contains:
   - A subfield with ID 0x4453 (Security Descriptor) and 4 data bytes.
-    The local extra field has 152 bytes of NT security descriptor data.
+    The local extra field has 164 bytes of NT security descriptor data.
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access/creation times.
 
   There is no file comment.
 
-Central directory entry #12:
+Central directory entry #10:
 ---------------------------
 
   shared_atomic/atomic_int.pxd
 
-  offset of local header from start of archive:   713714
-                                                  (00000000000AE3F2h) bytes
+  offset of local header from start of archive:   793604
+                                                  (00000000000C1C04h) bytes
   file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Aug 22 19:58:32
-  file last modified on (UT extra field modtime): 2023 Aug 22 11:58:32 local
-  file last modified on (UT extra field modtime): 2023 Aug 22 11:58:32 UTC
-  32-bit CRC value (hex):                         91e6488a
-  compressed size:                                459 bytes
-  uncompressed size:                              2905 bytes
+  file last modified on (DOS date/time):          2023 May 18 13:56:40
+  file last modified on (UT extra field modtime): 2023 May 18 05:56:39 local
+  file last modified on (UT extra field modtime): 2023 May 18 05:56:39 UTC
+  32-bit CRC value (hex):                         21630272
+  compressed size:                                351 bytes
+  uncompressed size:                              2402 bytes
   length of filename:                             28 characters
   length of extra field:                          17 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   non-MSDOS external file attributes:             000000 hex
   MS-DOS file attributes (20 hex):                arc 
@@ -454,72 +380,72 @@
   - A subfield with ID 0x4453 (Security Descriptor) and 4 data bytes.
     The local extra field has 152 bytes of NT security descriptor data.
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access/creation times.
 
   There is no file comment.
 
-Central directory entry #13:
+Central directory entry #11:
 ---------------------------
 
-  shared_atomic/atomic_int.pypy39-pp73-win_amd64.pyd
+  shared_atomic/atomic_list.cp37-win_amd64.pyd
 
-  offset of local header from start of archive:   714345
-                                                  (00000000000AE669h) bytes
+  offset of local header from start of archive:   794127
+                                                  (00000000000C1E0Fh) bytes
   file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Sep 7 21:03:46
-  file last modified on (UT extra field modtime): 2023 Sep 7 13:03:45 local
-  file last modified on (UT extra field modtime): 2023 Sep 7 13:03:45 UTC
-  32-bit CRC value (hex):                         396341b2
-  compressed size:                                33364 bytes
-  uncompressed size:                              86016 bytes
-  length of filename:                             50 characters
+  file last modified on (DOS date/time):          2024 Apr 20 13:28:42
+  file last modified on (UT extra field modtime): 2024 Apr 20 05:28:41 local
+  file last modified on (UT extra field modtime): 2024 Apr 20 05:28:41 UTC
+  32-bit CRC value (hex):                         dc1c8b58
+  compressed size:                                50783 bytes
+  uncompressed size:                              119296 bytes
+  length of filename:                             44 characters
   length of extra field:                          17 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             binary
   non-MSDOS external file attributes:             000000 hex
   MS-DOS file attributes (20 hex):                arc 
 
   The central-directory extra field contains:
   - A subfield with ID 0x4453 (Security Descriptor) and 4 data bytes.
-    The local extra field has 152 bytes of NT security descriptor data.
+    The local extra field has 164 bytes of NT security descriptor data.
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access/creation times.
 
   There is no file comment.
 
-Central directory entry #14:
+Central directory entry #12:
 ---------------------------
 
   shared_atomic/atomic_list.pxd
 
-  offset of local header from start of archive:   747903
-                                                  (00000000000B697Fh) bytes
+  offset of local header from start of archive:   845098
+                                                  (00000000000CE52Ah) bytes
   file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Aug 22 19:58:40
-  file last modified on (UT extra field modtime): 2023 Aug 22 11:58:39 local
-  file last modified on (UT extra field modtime): 2023 Aug 22 11:58:39 UTC
-  32-bit CRC value (hex):                         fb132af9
-  compressed size:                                501 bytes
-  uncompressed size:                              1893 bytes
+  file last modified on (DOS date/time):          2023 Aug 22 10:34:48
+  file last modified on (UT extra field modtime): 2023 Aug 22 02:34:48 local
+  file last modified on (UT extra field modtime): 2023 Aug 22 02:34:48 UTC
+  32-bit CRC value (hex):                         e40441f0
+  compressed size:                                391 bytes
+  uncompressed size:                              1389 bytes
   length of filename:                             29 characters
   length of extra field:                          17 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   non-MSDOS external file attributes:             000000 hex
   MS-DOS file attributes (20 hex):                arc 
@@ -528,72 +454,72 @@
   - A subfield with ID 0x4453 (Security Descriptor) and 4 data bytes.
     The local extra field has 152 bytes of NT security descriptor data.
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access/creation times.
 
   There is no file comment.
 
-Central directory entry #15:
+Central directory entry #13:
 ---------------------------
 
-  shared_atomic/atomic_list.pypy39-pp73-win_amd64.pyd
+  shared_atomic/atomic_object.cp37-win_amd64.pyd
 
-  offset of local header from start of archive:   748577
-                                                  (00000000000B6C21h) bytes
+  offset of local header from start of archive:   845662
+                                                  (00000000000CE75Eh) bytes
   file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Sep 7 21:04:04
-  file last modified on (UT extra field modtime): 2023 Sep 7 13:04:03 local
-  file last modified on (UT extra field modtime): 2023 Sep 7 13:04:03 UTC
-  32-bit CRC value (hex):                         5fd14ecd
-  compressed size:                                39969 bytes
-  uncompressed size:                              94208 bytes
-  length of filename:                             51 characters
+  file last modified on (DOS date/time):          2024 Apr 20 13:27:58
+  file last modified on (UT extra field modtime): 2024 Apr 20 05:27:58 local
+  file last modified on (UT extra field modtime): 2024 Apr 20 05:27:58 UTC
+  32-bit CRC value (hex):                         bd07a28e
+  compressed size:                                14482 bytes
+  uncompressed size:                              36864 bytes
+  length of filename:                             46 characters
   length of extra field:                          17 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             binary
   non-MSDOS external file attributes:             000000 hex
   MS-DOS file attributes (20 hex):                arc 
 
   The central-directory extra field contains:
   - A subfield with ID 0x4453 (Security Descriptor) and 4 data bytes.
-    The local extra field has 152 bytes of NT security descriptor data.
+    The local extra field has 164 bytes of NT security descriptor data.
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access/creation times.
 
   There is no file comment.
 
-Central directory entry #16:
+Central directory entry #14:
 ---------------------------
 
   shared_atomic/atomic_object.pxd
 
-  offset of local header from start of archive:   788741
-                                                  (00000000000C0905h) bytes
+  offset of local header from start of archive:   860334
+                                                  (00000000000D20AEh) bytes
   file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Aug 22 20:21:44
-  file last modified on (UT extra field modtime): 2023 Aug 22 12:21:44 local
-  file last modified on (UT extra field modtime): 2023 Aug 22 12:21:44 UTC
-  32-bit CRC value (hex):                         af6a0e31
-  compressed size:                                411 bytes
-  uncompressed size:                              4095 bytes
+  file last modified on (DOS date/time):          2023 Aug 22 10:38:00
+  file last modified on (UT extra field modtime): 2023 Aug 22 02:37:59 local
+  file last modified on (UT extra field modtime): 2023 Aug 22 02:37:59 UTC
+  32-bit CRC value (hex):                         c949d1ff
+  compressed size:                                421 bytes
+  uncompressed size:                              4153 bytes
   length of filename:                             31 characters
   length of extra field:                          17 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   non-MSDOS external file attributes:             000000 hex
   MS-DOS file attributes (20 hex):                arc 
@@ -602,72 +528,72 @@
   - A subfield with ID 0x4453 (Security Descriptor) and 4 data bytes.
     The local extra field has 152 bytes of NT security descriptor data.
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access/creation times.
 
   There is no file comment.
 
-Central directory entry #17:
+Central directory entry #15:
 ---------------------------
 
-  shared_atomic/atomic_object.pypy39-pp73-win_amd64.pyd
+  shared_atomic/atomic_object_backend.cp37-win_amd64.pyd
 
-  offset of local header from start of archive:   789327
-                                                  (00000000000C0B4Fh) bytes
+  offset of local header from start of archive:   860930
+                                                  (00000000000D2302h) bytes
   file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Sep 7 21:02:22
-  file last modified on (UT extra field modtime): 2023 Sep 7 13:02:22 local
-  file last modified on (UT extra field modtime): 2023 Sep 7 13:02:22 UTC
-  32-bit CRC value (hex):                         9d6b8b5d
-  compressed size:                                14224 bytes
-  uncompressed size:                              34816 bytes
-  length of filename:                             53 characters
+  file last modified on (DOS date/time):          2024 Apr 20 13:27:46
+  file last modified on (UT extra field modtime): 2024 Apr 20 05:27:46 local
+  file last modified on (UT extra field modtime): 2024 Apr 20 05:27:46 UTC
+  32-bit CRC value (hex):                         74c324cb
+  compressed size:                                87529 bytes
+  uncompressed size:                              246272 bytes
+  length of filename:                             54 characters
   length of extra field:                          17 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             binary
   non-MSDOS external file attributes:             000000 hex
   MS-DOS file attributes (20 hex):                arc 
 
   The central-directory extra field contains:
   - A subfield with ID 0x4453 (Security Descriptor) and 4 data bytes.
-    The local extra field has 152 bytes of NT security descriptor data.
+    The local extra field has 164 bytes of NT security descriptor data.
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access/creation times.
 
   There is no file comment.
 
-Central directory entry #18:
+Central directory entry #16:
 ---------------------------
 
   shared_atomic/atomic_object_backend.pxd
 
-  offset of local header from start of archive:   803748
-                                                  (00000000000C43A4h) bytes
+  offset of local header from start of archive:   948657
+                                                  (00000000000E79B1h) bytes
   file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Aug 29 17:25:06
-  file last modified on (UT extra field modtime): 2023 Aug 29 09:25:05 local
-  file last modified on (UT extra field modtime): 2023 Aug 29 09:25:05 UTC
-  32-bit CRC value (hex):                         07e3bd42
-  compressed size:                                770 bytes
-  uncompressed size:                              4251 bytes
+  file last modified on (DOS date/time):          2023 Aug 29 16:59:56
+  file last modified on (UT extra field modtime): 2023 Aug 29 08:59:55 local
+  file last modified on (UT extra field modtime): 2023 Aug 29 08:59:55 UTC
+  32-bit CRC value (hex):                         bd49a093
+  compressed size:                                754 bytes
+  uncompressed size:                              4111 bytes
   length of filename:                             39 characters
   length of extra field:                          17 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   non-MSDOS external file attributes:             000000 hex
   MS-DOS file attributes (20 hex):                arc 
@@ -676,72 +602,72 @@
   - A subfield with ID 0x4453 (Security Descriptor) and 4 data bytes.
     The local extra field has 152 bytes of NT security descriptor data.
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access/creation times.
 
   There is no file comment.
 
-Central directory entry #19:
+Central directory entry #17:
 ---------------------------
 
-  shared_atomic/atomic_object_backend.pypy39-pp73-win_amd64.pyd
+  shared_atomic/atomic_set.cp37-win_amd64.pyd
 
-  offset of local header from start of archive:   804701
-                                                  (00000000000C475Dh) bytes
+  offset of local header from start of archive:   949594
+                                                  (00000000000E7D5Ah) bytes
   file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Sep 7 21:02:10
-  file last modified on (UT extra field modtime): 2023 Sep 7 13:02:09 local
-  file last modified on (UT extra field modtime): 2023 Sep 7 13:02:09 UTC
-  32-bit CRC value (hex):                         4f8333a5
-  compressed size:                                76047 bytes
-  uncompressed size:                              209408 bytes
-  length of filename:                             61 characters
+  file last modified on (DOS date/time):          2024 Apr 20 13:28:50
+  file last modified on (UT extra field modtime): 2024 Apr 20 05:28:50 local
+  file last modified on (UT extra field modtime): 2024 Apr 20 05:28:50 UTC
+  32-bit CRC value (hex):                         494d8aa8
+  compressed size:                                50801 bytes
+  uncompressed size:                              118784 bytes
+  length of filename:                             43 characters
   length of extra field:                          17 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             binary
   non-MSDOS external file attributes:             000000 hex
   MS-DOS file attributes (20 hex):                arc 
 
   The central-directory extra field contains:
   - A subfield with ID 0x4453 (Security Descriptor) and 4 data bytes.
-    The local extra field has 152 bytes of NT security descriptor data.
+    The local extra field has 164 bytes of NT security descriptor data.
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access/creation times.
 
   There is no file comment.
 
-Central directory entry #20:
+Central directory entry #18:
 ---------------------------
 
   shared_atomic/atomic_set.pxd
 
-  offset of local header from start of archive:   880953
-                                                  (00000000000D7139h) bytes
+  offset of local header from start of archive:   1000582
+                                                  (00000000000F4486h) bytes
   file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Aug 22 19:58:48
-  file last modified on (UT extra field modtime): 2023 Aug 22 11:58:47 local
-  file last modified on (UT extra field modtime): 2023 Aug 22 11:58:47 UTC
-  32-bit CRC value (hex):                         b9ad1f78
-  compressed size:                                485 bytes
-  uncompressed size:                              1791 bytes
+  file last modified on (DOS date/time):          2023 Aug 22 10:39:46
+  file last modified on (UT extra field modtime): 2023 Aug 22 02:39:46 local
+  file last modified on (UT extra field modtime): 2023 Aug 22 02:39:46 UTC
+  32-bit CRC value (hex):                         695fc0fb
+  compressed size:                                373 bytes
+  uncompressed size:                              1287 bytes
   length of filename:                             28 characters
   length of extra field:                          17 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   non-MSDOS external file attributes:             000000 hex
   MS-DOS file attributes (20 hex):                arc 
@@ -750,72 +676,72 @@
   - A subfield with ID 0x4453 (Security Descriptor) and 4 data bytes.
     The local extra field has 152 bytes of NT security descriptor data.
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access/creation times.
 
   There is no file comment.
 
-Central directory entry #21:
+Central directory entry #19:
 ---------------------------
 
-  shared_atomic/atomic_set.pypy39-pp73-win_amd64.pyd
+  shared_atomic/atomic_shared_memory.cp37-win_amd64.pyd
 
-  offset of local header from start of archive:   881610
-                                                  (00000000000D73CAh) bytes
+  offset of local header from start of archive:   1001127
+                                                  (00000000000F46A7h) bytes
   file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Sep 7 21:04:24
-  file last modified on (UT extra field modtime): 2023 Sep 7 13:04:24 local
-  file last modified on (UT extra field modtime): 2023 Sep 7 13:04:24 UTC
-  32-bit CRC value (hex):                         ac394ebe
-  compressed size:                                39981 bytes
-  uncompressed size:                              94208 bytes
-  length of filename:                             50 characters
+  file last modified on (DOS date/time):          2024 Apr 20 13:29:28
+  file last modified on (UT extra field modtime): 2024 Apr 20 05:29:28 local
+  file last modified on (UT extra field modtime): 2024 Apr 20 05:29:28 UTC
+  32-bit CRC value (hex):                         7eff0f6e
+  compressed size:                                160577 bytes
+  uncompressed size:                              458752 bytes
+  length of filename:                             53 characters
   length of extra field:                          17 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             binary
   non-MSDOS external file attributes:             000000 hex
   MS-DOS file attributes (20 hex):                arc 
 
   The central-directory extra field contains:
   - A subfield with ID 0x4453 (Security Descriptor) and 4 data bytes.
-    The local extra field has 152 bytes of NT security descriptor data.
+    The local extra field has 164 bytes of NT security descriptor data.
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access/creation times.
 
   There is no file comment.
 
-Central directory entry #22:
+Central directory entry #20:
 ---------------------------
 
   shared_atomic/atomic_shared_memory.pxd
 
-  offset of local header from start of archive:   921785
-                                                  (00000000000E10B9h) bytes
+  offset of local header from start of archive:   1161901
+                                                  (000000000011BAADh) bytes
   file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Aug 22 19:58:12
-  file last modified on (UT extra field modtime): 2023 Aug 22 11:58:11 local
-  file last modified on (UT extra field modtime): 2023 Aug 22 11:58:11 UTC
-  32-bit CRC value (hex):                         a431020f
-  compressed size:                                896 bytes
-  uncompressed size:                              6021 bytes
+  file last modified on (DOS date/time):          2024 Apr 19 16:15:20
+  file last modified on (UT extra field modtime): 2024 Apr 19 08:15:20 local
+  file last modified on (UT extra field modtime): 2024 Apr 19 08:15:20 UTC
+  32-bit CRC value (hex):                         a0cae6a8
+  compressed size:                                921 bytes
+  uncompressed size:                              6050 bytes
   length of filename:                             38 characters
   length of extra field:                          17 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   non-MSDOS external file attributes:             000000 hex
   MS-DOS file attributes (20 hex):                arc 
@@ -824,72 +750,72 @@
   - A subfield with ID 0x4453 (Security Descriptor) and 4 data bytes.
     The local extra field has 152 bytes of NT security descriptor data.
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access/creation times.
 
   There is no file comment.
 
-Central directory entry #23:
+Central directory entry #21:
 ---------------------------
 
-  shared_atomic/atomic_shared_memory.pypy39-pp73-win_amd64.pyd
+  shared_atomic/atomic_string.cp37-win_amd64.pyd
 
-  offset of local header from start of archive:   922863
-                                                  (00000000000E14EFh) bytes
+  offset of local header from start of archive:   1163004
+                                                  (000000000011BEFCh) bytes
   file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Sep 7 21:06:08
-  file last modified on (UT extra field modtime): 2023 Sep 7 13:06:07 local
-  file last modified on (UT extra field modtime): 2023 Sep 7 13:06:07 UTC
-  32-bit CRC value (hex):                         26f98333
-  compressed size:                                145370 bytes
-  uncompressed size:                              412672 bytes
-  length of filename:                             60 characters
+  file last modified on (DOS date/time):          2024 Apr 20 13:29:00
+  file last modified on (UT extra field modtime): 2024 Apr 20 05:29:00 local
+  file last modified on (UT extra field modtime): 2024 Apr 20 05:29:00 UTC
+  32-bit CRC value (hex):                         bc6d145a
+  compressed size:                                48763 bytes
+  uncompressed size:                              113664 bytes
+  length of filename:                             46 characters
   length of extra field:                          17 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             binary
   non-MSDOS external file attributes:             000000 hex
   MS-DOS file attributes (20 hex):                arc 
 
   The central-directory extra field contains:
   - A subfield with ID 0x4453 (Security Descriptor) and 4 data bytes.
-    The local extra field has 152 bytes of NT security descriptor data.
+    The local extra field has 164 bytes of NT security descriptor data.
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access/creation times.
 
   There is no file comment.
 
-Central directory entry #24:
+Central directory entry #22:
 ---------------------------
 
   shared_atomic/atomic_string.pxd
 
-  offset of local header from start of archive:   1068437
-                                                  (0000000000104D95h) bytes
+  offset of local header from start of archive:   1211957
+                                                  (0000000000127E35h) bytes
   file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Aug 22 19:58:58
-  file last modified on (UT extra field modtime): 2023 Aug 22 11:58:57 local
-  file last modified on (UT extra field modtime): 2023 Aug 22 11:58:57 UTC
-  32-bit CRC value (hex):                         88a7b5ee
-  compressed size:                                477 bytes
-  uncompressed size:                              1755 bytes
+  file last modified on (DOS date/time):          2023 Aug 22 15:17:12
+  file last modified on (UT extra field modtime): 2023 Aug 22 07:17:11 local
+  file last modified on (UT extra field modtime): 2023 Aug 22 07:17:11 UTC
+  32-bit CRC value (hex):                         92ebbd38
+  compressed size:                                376 bytes
+  uncompressed size:                              1252 bytes
   length of filename:                             31 characters
   length of extra field:                          17 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   non-MSDOS external file attributes:             000000 hex
   MS-DOS file attributes (20 hex):                arc 
@@ -898,852 +824,521 @@
   - A subfield with ID 0x4453 (Security Descriptor) and 4 data bytes.
     The local extra field has 152 bytes of NT security descriptor data.
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access/creation times.
 
   There is no file comment.
 
-Central directory entry #25:
----------------------------
-
-  shared_atomic/atomic_string.pypy39-pp73-win_amd64.pyd
-
-  offset of local header from start of archive:   1069089
-                                                  (0000000000105021h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   3.0
-  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   2.0
-  compression method:                             deflated
-  compression sub-type (deflation):               normal
-  file security status:                           not encrypted
-  extended local header:                          no
-  file last modified on (DOS date/time):          2023 Sep 7 21:04:46
-  file last modified on (UT extra field modtime): 2023 Sep 7 13:04:45 local
-  file last modified on (UT extra field modtime): 2023 Sep 7 13:04:45 UTC
-  32-bit CRC value (hex):                         ac86c0d9
-  compressed size:                                39357 bytes
-  uncompressed size:                              90624 bytes
-  length of filename:                             53 characters
-  length of extra field:                          17 bytes
-  length of file comment:                         0 characters
-  disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  non-MSDOS external file attributes:             000000 hex
-  MS-DOS file attributes (20 hex):                arc 
-
-  The central-directory extra field contains:
-  - A subfield with ID 0x4453 (Security Descriptor) and 4 data bytes.
-    The local extra field has 152 bytes of NT security descriptor data.
-  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
-    The local extra field has UTC/GMT modification/access/creation times.
-
-  There is no file comment.
-
-Central directory entry #26:
+Central directory entry #23:
 ---------------------------
 
   shared_atomic/atomic_tools.py
 
-  offset of local header from start of archive:   1108643
-                                                  (000000000010EAA3h) bytes
+  offset of local header from start of archive:   1212508
+                                                  (000000000012805Ch) bytes
   file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Sep 7 21:06:08
-  file last modified on (UT extra field modtime): 2023 Sep 7 13:06:07 local
-  file last modified on (UT extra field modtime): 2023 Sep 7 13:06:07 UTC
-  32-bit CRC value (hex):                         8d990fa9
-  compressed size:                                408 bytes
-  uncompressed size:                              807 bytes
+  file last modified on (DOS date/time):          2024 Apr 20 13:29:28
+  file last modified on (UT extra field modtime): 2024 Apr 20 05:29:28 local
+  file last modified on (UT extra field modtime): 2024 Apr 20 05:29:28 UTC
+  32-bit CRC value (hex):                         446ec06d
+  compressed size:                                427 bytes
+  uncompressed size:                              893 bytes
   length of filename:                             29 characters
   length of extra field:                          17 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   non-MSDOS external file attributes:             000000 hex
   MS-DOS file attributes (20 hex):                arc 
 
   The central-directory extra field contains:
   - A subfield with ID 0x4453 (Security Descriptor) and 4 data bytes.
-    The local extra field has 152 bytes of NT security descriptor data.
-  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
-    The local extra field has UTC/GMT modification/access/creation times.
-
-  There is no file comment.
-
-Central directory entry #27:
----------------------------
-
-  shared_atomic/cpython_libs.zip
-
-  offset of local header from start of archive:   1109224
-                                                  (000000000010ECE8h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   3.0
-  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   1.0
-  compression method:                             none (stored)
-  file security status:                           not encrypted
-  extended local header:                          no
-  file last modified on (DOS date/time):          2023 Aug 1 15:50:58
-  file last modified on (UT extra field modtime): 2023 Aug 1 07:50:57 local
-  file last modified on (UT extra field modtime): 2023 Aug 1 07:50:57 UTC
-  32-bit CRC value (hex):                         9b818705
-  compressed size:                                1117653 bytes
-  uncompressed size:                              1117653 bytes
-  length of filename:                             30 characters
-  length of extra field:                          17 bytes
-  length of file comment:                         0 characters
-  disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  non-MSDOS external file attributes:             000000 hex
-  MS-DOS file attributes (20 hex):                arc 
-
-  The central-directory extra field contains:
-  - A subfield with ID 0x4453 (Security Descriptor) and 4 data bytes.
-    The local extra field has 152 bytes of NT security descriptor data.
+    The local extra field has 164 bytes of NT security descriptor data.
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access/creation times.
 
   There is no file comment.
 
-Central directory entry #28:
+Central directory entry #24:
 ---------------------------
 
   shared_atomic/end_user_license_agreement.txt
 
-  offset of local header from start of archive:   2227051
-                                                  (000000000021FB6Bh) bytes
+  offset of local header from start of archive:   1213108
+                                                  (00000000001282B4h) bytes
   file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Sep 7 21:06:08
-  file last modified on (UT extra field modtime): 2023 Sep 7 13:06:07 local
-  file last modified on (UT extra field modtime): 2023 Sep 7 13:06:07 UTC
-  32-bit CRC value (hex):                         1a5ee3e0
-  compressed size:                                15630 bytes
-  uncompressed size:                              49645 bytes
+  file last modified on (DOS date/time):          2024 Apr 20 13:29:28
+  file last modified on (UT extra field modtime): 2024 Apr 20 05:29:28 local
+  file last modified on (UT extra field modtime): 2024 Apr 20 05:29:28 UTC
+  32-bit CRC value (hex):                         998933ec
+  compressed size:                                13858 bytes
+  uncompressed size:                              43829 bytes
   length of filename:                             44 characters
   length of extra field:                          17 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   non-MSDOS external file attributes:             000000 hex
   MS-DOS file attributes (20 hex):                arc 
 
   The central-directory extra field contains:
   - A subfield with ID 0x4453 (Security Descriptor) and 4 data bytes.
-    The local extra field has 152 bytes of NT security descriptor data.
-  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
-    The local extra field has UTC/GMT modification/access/creation times.
-
-  There is no file comment.
-
-Central directory entry #29:
----------------------------
-
-  shared_atomic/lib/
-
-  offset of local header from start of archive:   2242869
-                                                  (0000000000223935h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   3.0
-  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   1.0
-  compression method:                             none (stored)
-  file security status:                           not encrypted
-  extended local header:                          no
-  file last modified on (DOS date/time):          2023 Apr 4 12:29:26
-  file last modified on (UT extra field modtime): 2023 Apr 4 04:29:26 local
-  file last modified on (UT extra field modtime): 2023 Apr 4 04:29:26 UTC
-  32-bit CRC value (hex):                         00000000
-  compressed size:                                0 bytes
-  uncompressed size:                              0 bytes
-  length of filename:                             18 characters
-  length of extra field:                          17 bytes
-  length of file comment:                         0 characters
-  disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  non-MSDOS external file attributes:             000000 hex
-  MS-DOS file attributes (10 hex):                dir 
-
-  The central-directory extra field contains:
-  - A subfield with ID 0x4453 (Security Descriptor) and 4 data bytes.
-    The local extra field has 152 bytes of NT security descriptor data.
+    The local extra field has 164 bytes of NT security descriptor data.
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access/creation times.
 
   There is no file comment.
 
-Central directory entry #30:
+Central directory entry #25:
 ---------------------------
 
   shared_atomic/libdecryption.dll
 
-  offset of local header from start of archive:   2243031
-                                                  (00000000002239D7h) bytes
+  offset of local header from start of archive:   1227154
+                                                  (000000000012B992h) bytes
   file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Sep 7 20:57:16
-  file last modified on (UT extra field modtime): 2023 Sep 7 12:57:15 local
-  file last modified on (UT extra field modtime): 2023 Sep 7 12:57:15 UTC
-  32-bit CRC value (hex):                         debf53e2
-  compressed size:                                1335871 bytes
+  file last modified on (DOS date/time):          2024 Apr 20 13:25:26
+  file last modified on (UT extra field modtime): 2024 Apr 20 05:25:26 local
+  file last modified on (UT extra field modtime): 2024 Apr 20 05:25:26 UTC
+  32-bit CRC value (hex):                         d2f36e07
+  compressed size:                                1335872 bytes
   uncompressed size:                              3496448 bytes
   length of filename:                             31 characters
   length of extra field:                          17 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             binary
   non-MSDOS external file attributes:             000000 hex
   MS-DOS file attributes (20 hex):                arc 
 
   The central-directory extra field contains:
   - A subfield with ID 0x4453 (Security Descriptor) and 4 data bytes.
-    The local extra field has 152 bytes of NT security descriptor data.
+    The local extra field has 164 bytes of NT security descriptor data.
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access/creation times.
 
   There is no file comment.
 
-Central directory entry #31:
+Central directory entry #26:
 ---------------------------
 
   shared_atomic/libdecryption11.dll
 
-  offset of local header from start of archive:   3579077
-                                                  (0000000000369CC5h) bytes
+  offset of local header from start of archive:   2563201
+                                                  (0000000000271C81h) bytes
   file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Sep 7 20:57:16
-  file last modified on (UT extra field modtime): 2023 Sep 7 12:57:16 local
-  file last modified on (UT extra field modtime): 2023 Sep 7 12:57:16 UTC
-  32-bit CRC value (hex):                         6bcf316e
+  file last modified on (DOS date/time):          2024 Apr 20 13:25:26
+  file last modified on (UT extra field modtime): 2024 Apr 20 05:25:26 local
+  file last modified on (UT extra field modtime): 2024 Apr 20 05:25:26 UTC
+  32-bit CRC value (hex):                         cf507dfa
   compressed size:                                4011 bytes
   uncompressed size:                              9728 bytes
   length of filename:                             33 characters
   length of extra field:                          17 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             binary
   non-MSDOS external file attributes:             000000 hex
   MS-DOS file attributes (20 hex):                arc 
 
   The central-directory extra field contains:
   - A subfield with ID 0x4453 (Security Descriptor) and 4 data bytes.
-    The local extra field has 152 bytes of NT security descriptor data.
+    The local extra field has 164 bytes of NT security descriptor data.
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access/creation times.
 
   There is no file comment.
 
-Central directory entry #32:
----------------------------
-
-  shared_atomic/python3.dll
-
-  offset of local header from start of archive:   3583265
-                                                  (000000000036AD21h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   3.0
-  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   2.0
-  compression method:                             deflated
-  compression sub-type (deflation):               normal
-  file security status:                           not encrypted
-  extended local header:                          no
-  file last modified on (DOS date/time):          2022 May 17 16:46:04
-  file last modified on (UT extra field modtime): 2022 May 17 08:46:04 local
-  file last modified on (UT extra field modtime): 2022 May 17 08:46:04 UTC
-  32-bit CRC value (hex):                         ae4f95ee
-  compressed size:                                20281 bytes
-  uncompressed size:                              61432 bytes
-  length of filename:                             25 characters
-  length of extra field:                          17 bytes
-  length of file comment:                         0 characters
-  disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  non-MSDOS external file attributes:             000000 hex
-  MS-DOS file attributes (20 hex):                arc 
-
-  The central-directory extra field contains:
-  - A subfield with ID 0x4453 (Security Descriptor) and 4 data bytes.
-    The local extra field has 152 bytes of NT security descriptor data.
-  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
-    The local extra field has UTC/GMT modification/access/creation times.
-
-  There is no file comment.
-
-Central directory entry #33:
----------------------------
-
-  shared_atomic/python39.dll
-
-  offset of local header from start of archive:   3603715
-                                                  (000000000036FD03h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   3.0
-  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   2.0
-  compression method:                             deflated
-  compression sub-type (deflation):               normal
-  file security status:                           not encrypted
-  extended local header:                          no
-  file last modified on (DOS date/time):          2022 May 17 16:46:04
-  file last modified on (UT extra field modtime): 2022 May 17 08:46:04 local
-  file last modified on (UT extra field modtime): 2022 May 17 08:46:04 UTC
-  32-bit CRC value (hex):                         85fa642a
-  compressed size:                                2008848 bytes
-  uncompressed size:                              4527096 bytes
-  length of filename:                             26 characters
-  length of extra field:                          17 bytes
-  length of file comment:                         0 characters
-  disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  non-MSDOS external file attributes:             000000 hex
-  MS-DOS file attributes (20 hex):                arc 
-
-  The central-directory extra field contains:
-  - A subfield with ID 0x4453 (Security Descriptor) and 4 data bytes.
-    The local extra field has 152 bytes of NT security descriptor data.
-  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
-    The local extra field has UTC/GMT modification/access/creation times.
-
-  There is no file comment.
-
-Central directory entry #34:
+Central directory entry #27:
 ---------------------------
 
   shared_atomic/readme.txt
 
-  offset of local header from start of archive:   5612733
-                                                  (000000000055A4BDh) bytes
+  offset of local header from start of archive:   2567389
+                                                  (0000000000272CDDh) bytes
   file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Sep 7 21:06:08
-  file last modified on (UT extra field modtime): 2023 Sep 7 13:06:07 local
-  file last modified on (UT extra field modtime): 2023 Sep 7 13:06:07 UTC
+  file last modified on (DOS date/time):          2024 Apr 20 13:29:28
+  file last modified on (UT extra field modtime): 2024 Apr 20 05:29:28 local
+  file last modified on (UT extra field modtime): 2024 Apr 20 05:29:28 UTC
   32-bit CRC value (hex):                         ba5f87e5
   compressed size:                                370 bytes
   uncompressed size:                              622 bytes
   length of filename:                             24 characters
   length of extra field:                          17 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   non-MSDOS external file attributes:             000000 hex
   MS-DOS file attributes (20 hex):                arc 
 
   The central-directory extra field contains:
   - A subfield with ID 0x4453 (Security Descriptor) and 4 data bytes.
-    The local extra field has 152 bytes of NT security descriptor data.
+    The local extra field has 164 bytes of NT security descriptor data.
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access/creation times.
 
   There is no file comment.
 
-Central directory entry #35:
+Central directory entry #28:
 ---------------------------
 
-  shared_atomic/select.pyd
+  shared_atomic/setup.py
 
-  offset of local header from start of archive:   5613271
-                                                  (000000000055A6D7h) bytes
+  offset of local header from start of archive:   2567927
+                                                  (0000000000272EF7h) bytes
   file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2022 May 17 16:46:02
-  file last modified on (UT extra field modtime): 2022 May 17 08:46:02 local
-  file last modified on (UT extra field modtime): 2022 May 17 08:46:02 UTC
-  32-bit CRC value (hex):                         dd7e6338
-  compressed size:                                17169 bytes
-  uncompressed size:                              30712 bytes
-  length of filename:                             24 characters
+  file last modified on (DOS date/time):          2024 Apr 20 13:29:28
+  file last modified on (UT extra field modtime): 2024 Apr 20 05:29:28 local
+  file last modified on (UT extra field modtime): 2024 Apr 20 05:29:28 UTC
+  32-bit CRC value (hex):                         800a1c12
+  compressed size:                                928 bytes
+  uncompressed size:                              2754 bytes
+  length of filename:                             22 characters
   length of extra field:                          17 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  non-MSDOS external file attributes:             000000 hex
-  MS-DOS file attributes (20 hex):                arc 
-
-  The central-directory extra field contains:
-  - A subfield with ID 0x4453 (Security Descriptor) and 4 data bytes.
-    The local extra field has 152 bytes of NT security descriptor data.
-  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
-    The local extra field has UTC/GMT modification/access/creation times.
-
-  There is no file comment.
-
-Central directory entry #36:
----------------------------
-
-  shared_atomic/unicodedata.pyd
-
-  offset of local header from start of archive:   5630608
-                                                  (000000000055EA90h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   3.0
-  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   2.0
-  compression method:                             deflated
-  compression sub-type (deflation):               normal
-  file security status:                           not encrypted
-  extended local header:                          no
-  file last modified on (DOS date/time):          2022 May 17 16:46:04
-  file last modified on (UT extra field modtime): 2022 May 17 08:46:04 local
-  file last modified on (UT extra field modtime): 2022 May 17 08:46:04 UTC
-  32-bit CRC value (hex):                         bd6c26a1
-  compressed size:                                409871 bytes
-  uncompressed size:                              1123832 bytes
-  length of filename:                             29 characters
-  length of extra field:                          17 bytes
-  length of file comment:                         0 characters
-  disk number on which file begins:               disk 1
-  apparent file type:                             binary
+  apparent file type:                             text
   non-MSDOS external file attributes:             000000 hex
   MS-DOS file attributes (20 hex):                arc 
 
   The central-directory extra field contains:
   - A subfield with ID 0x4453 (Security Descriptor) and 4 data bytes.
-    The local extra field has 152 bytes of NT security descriptor data.
+    The local extra field has 164 bytes of NT security descriptor data.
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access/creation times.
 
   There is no file comment.
 
-Central directory entry #37:
+Central directory entry #29:
 ---------------------------
 
   shared_atomic/urwid_win_patch.py
 
-  offset of local header from start of archive:   6040652
-                                                  (00000000005C2C4Ch) bytes
+  offset of local header from start of archive:   2569021
+                                                  (000000000027333Dh) bytes
   file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Sep 7 21:06:08
-  file last modified on (UT extra field modtime): 2023 Sep 7 13:06:07 local
-  file last modified on (UT extra field modtime): 2023 Sep 7 13:06:07 UTC
-  32-bit CRC value (hex):                         86741696
-  compressed size:                                1224 bytes
-  uncompressed size:                              3423 bytes
+  file last modified on (DOS date/time):          2024 Apr 20 13:29:28
+  file last modified on (UT extra field modtime): 2024 Apr 20 05:29:28 local
+  file last modified on (UT extra field modtime): 2024 Apr 20 05:29:28 UTC
+  32-bit CRC value (hex):                         ecc3f14e
+  compressed size:                                1469 bytes
+  uncompressed size:                              4070 bytes
   length of filename:                             32 characters
   length of extra field:                          17 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   non-MSDOS external file attributes:             000000 hex
   MS-DOS file attributes (20 hex):                arc 
 
   The central-directory extra field contains:
   - A subfield with ID 0x4453 (Security Descriptor) and 4 data bytes.
-    The local extra field has 152 bytes of NT security descriptor data.
-  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
-    The local extra field has UTC/GMT modification/access/creation times.
-
-  There is no file comment.
-
-Central directory entry #38:
----------------------------
-
-  shared_atomic/_cffi_backend.cp39-win_amd64.pyd
-
-  offset of local header from start of archive:   6042052
-                                                  (00000000005C31C4h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   3.0
-  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   2.0
-  compression method:                             deflated
-  compression sub-type (deflation):               normal
-  file security status:                           not encrypted
-  extended local header:                          no
-  file last modified on (DOS date/time):          2022 Oct 24 17:24:38
-  file last modified on (UT extra field modtime): 2022 Oct 24 09:24:38 local
-  file last modified on (UT extra field modtime): 2022 Oct 24 09:24:38 UTC
-  32-bit CRC value (hex):                         8a34aa66
-  compressed size:                                82369 bytes
-  uncompressed size:                              183296 bytes
-  length of filename:                             46 characters
-  length of extra field:                          17 bytes
-  length of file comment:                         0 characters
-  disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  non-MSDOS external file attributes:             000000 hex
-  MS-DOS file attributes (20 hex):                arc 
-
-  The central-directory extra field contains:
-  - A subfield with ID 0x4453 (Security Descriptor) and 4 data bytes.
-    The local extra field has 152 bytes of NT security descriptor data.
-  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
-    The local extra field has UTC/GMT modification/access/creation times.
-
-  There is no file comment.
-
-Central directory entry #39:
----------------------------
-
-  shared_atomic/_curses.cp39-win_amd64.pyd
-
-  offset of local header from start of archive:   6124611
-                                                  (00000000005D7443h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   3.0
-  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   2.0
-  compression method:                             deflated
-  compression sub-type (deflation):               normal
-  file security status:                           not encrypted
-  extended local header:                          no
-  file last modified on (DOS date/time):          2022 Nov 18 15:48:24
-  file last modified on (UT extra field modtime): 2022 Nov 18 07:48:23 local
-  file last modified on (UT extra field modtime): 2022 Nov 18 07:48:23 UTC
-  32-bit CRC value (hex):                         13bd25c0
-  compressed size:                                70392 bytes
-  uncompressed size:                              171008 bytes
-  length of filename:                             40 characters
-  length of extra field:                          17 bytes
-  length of file comment:                         0 characters
-  disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  non-MSDOS external file attributes:             000000 hex
-  MS-DOS file attributes (20 hex):                arc 
-
-  The central-directory extra field contains:
-  - A subfield with ID 0x4453 (Security Descriptor) and 4 data bytes.
-    The local extra field has 152 bytes of NT security descriptor data.
+    The local extra field has 164 bytes of NT security descriptor data.
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access/creation times.
 
   There is no file comment.
 
-Central directory entry #40:
+Central directory entry #30:
 ---------------------------
 
-  shared_atomic/_curses_panel.cp39-win_amd64.pyd
+  shared_atomic/_cffi_backend.cp37-win_amd64.pyd
 
-  offset of local header from start of archive:   6195187
-                                                  (00000000005E87F3h) bytes
+  offset of local header from start of archive:   2570666
+                                                  (00000000002739AAh) bytes
   file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2022 Nov 18 15:48:24
-  file last modified on (UT extra field modtime): 2022 Nov 18 07:48:23 local
-  file last modified on (UT extra field modtime): 2022 Nov 18 07:48:23 UTC
-  32-bit CRC value (hex):                         9ae10466
-  compressed size:                                11882 bytes
-  uncompressed size:                              27648 bytes
+  file last modified on (DOS date/time):          2022 Oct 24 16:55:38
+  file last modified on (UT extra field modtime): 2022 Oct 24 08:55:38 local
+  file last modified on (UT extra field modtime): 2022 Oct 24 08:55:38 UTC
+  32-bit CRC value (hex):                         e00b0373
+  compressed size:                                81088 bytes
+  uncompressed size:                              181248 bytes
   length of filename:                             46 characters
   length of extra field:                          17 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             binary
   non-MSDOS external file attributes:             000000 hex
   MS-DOS file attributes (20 hex):                arc 
 
   The central-directory extra field contains:
   - A subfield with ID 0x4453 (Security Descriptor) and 4 data bytes.
-    The local extra field has 152 bytes of NT security descriptor data.
-  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
-    The local extra field has UTC/GMT modification/access/creation times.
-
-  There is no file comment.
-
-Central directory entry #41:
----------------------------
-
-  shared_atomic/_socket.pyd
-
-  offset of local header from start of archive:   6207259
-                                                  (00000000005EB71Bh) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   3.0
-  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   2.0
-  compression method:                             deflated
-  compression sub-type (deflation):               normal
-  file security status:                           not encrypted
-  extended local header:                          no
-  file last modified on (DOS date/time):          2022 May 17 16:46:02
-  file last modified on (UT extra field modtime): 2022 May 17 08:46:02 local
-  file last modified on (UT extra field modtime): 2022 May 17 08:46:02 UTC
-  32-bit CRC value (hex):                         56944ef3
-  compressed size:                                38791 bytes
-  uncompressed size:                              81912 bytes
-  length of filename:                             25 characters
-  length of extra field:                          17 bytes
-  length of file comment:                         0 characters
-  disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  non-MSDOS external file attributes:             000000 hex
-  MS-DOS file attributes (20 hex):                arc 
-
-  The central-directory extra field contains:
-  - A subfield with ID 0x4453 (Security Descriptor) and 4 data bytes.
-    The local extra field has 152 bytes of NT security descriptor data.
+    The local extra field has 164 bytes of NT security descriptor data.
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access/creation times.
 
   There is no file comment.
 
-Central directory entry #42:
+Central directory entry #31:
 ---------------------------
 
   shared_atomic/__init__.py
 
-  offset of local header from start of archive:   6246219
-                                                  (00000000005F4F4Bh) bytes
+  offset of local header from start of archive:   2651944
+                                                  (0000000000287728h) bytes
   file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   1.0
   compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Sep 7 21:06:08
-  file last modified on (UT extra field modtime): 2023 Sep 7 13:06:07 local
-  file last modified on (UT extra field modtime): 2023 Sep 7 13:06:07 UTC
+  file last modified on (DOS date/time):          2024 Apr 20 13:29:28
+  file last modified on (UT extra field modtime): 2024 Apr 20 05:29:28 local
+  file last modified on (UT extra field modtime): 2024 Apr 20 05:29:28 UTC
   32-bit CRC value (hex):                         00000000
   compressed size:                                0 bytes
   uncompressed size:                              0 bytes
   length of filename:                             25 characters
   length of extra field:                          17 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             binary
   non-MSDOS external file attributes:             000000 hex
   MS-DOS file attributes (20 hex):                arc 
 
   The central-directory extra field contains:
   - A subfield with ID 0x4453 (Security Descriptor) and 4 data bytes.
-    The local extra field has 152 bytes of NT security descriptor data.
+    The local extra field has 164 bytes of NT security descriptor data.
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access/creation times.
 
   There is no file comment.
 
-Central directory entry #43:
+Central directory entry #32:
 ---------------------------
 
-  shared_atomic_enterprise-5!3.3.2.dist-info/
+  shared_atomic_enterprise-5!3.3.3.dist-info/
 
-  offset of local header from start of archive:   6246388
-                                                  (00000000005F4FF4h) bytes
+  offset of local header from start of archive:   2652113
+                                                  (00000000002877D1h) bytes
   file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   1.0
   compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Sep 7 21:06:08
-  file last modified on (UT extra field modtime): 2023 Sep 7 13:06:07 local
-  file last modified on (UT extra field modtime): 2023 Sep 7 13:06:07 UTC
+  file last modified on (DOS date/time):          2024 Apr 20 13:29:28
+  file last modified on (UT extra field modtime): 2024 Apr 20 05:29:28 local
+  file last modified on (UT extra field modtime): 2024 Apr 20 05:29:28 UTC
   32-bit CRC value (hex):                         00000000
   compressed size:                                0 bytes
   uncompressed size:                              0 bytes
   length of filename:                             43 characters
   length of extra field:                          17 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             binary
   non-MSDOS external file attributes:             000000 hex
   MS-DOS file attributes (10 hex):                dir 
 
   The central-directory extra field contains:
   - A subfield with ID 0x4453 (Security Descriptor) and 4 data bytes.
-    The local extra field has 152 bytes of NT security descriptor data.
+    The local extra field has 164 bytes of NT security descriptor data.
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access/creation times.
 
   There is no file comment.
 
-Central directory entry #44:
+Central directory entry #33:
 ---------------------------
 
-  shared_atomic_enterprise-5!3.3.2.dist-info/METADATA
+  shared_atomic_enterprise-5!3.3.3.dist-info/METADATA
 
-  offset of local header from start of archive:   6246575
-                                                  (00000000005F50AFh) bytes
+  offset of local header from start of archive:   2652300
+                                                  (000000000028788Ch) bytes
   file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Sep 7 21:06:08
-  file last modified on (UT extra field modtime): 2023 Sep 7 13:06:07 local
-  file last modified on (UT extra field modtime): 2023 Sep 7 13:06:07 UTC
-  32-bit CRC value (hex):                         1a56f945
-  compressed size:                                1158 bytes
-  uncompressed size:                              2981 bytes
+  file last modified on (DOS date/time):          2024 Apr 20 13:29:28
+  file last modified on (UT extra field modtime): 2024 Apr 20 05:29:28 local
+  file last modified on (UT extra field modtime): 2024 Apr 20 05:29:28 UTC
+  32-bit CRC value (hex):                         a1a5f5ce
+  compressed size:                                1121 bytes
+  uncompressed size:                              2779 bytes
   length of filename:                             51 characters
   length of extra field:                          17 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   non-MSDOS external file attributes:             000000 hex
   MS-DOS file attributes (20 hex):                arc 
 
   The central-directory extra field contains:
   - A subfield with ID 0x4453 (Security Descriptor) and 4 data bytes.
-    The local extra field has 152 bytes of NT security descriptor data.
+    The local extra field has 164 bytes of NT security descriptor data.
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access/creation times.
 
   There is no file comment.
 
-Central directory entry #45:
+Central directory entry #34:
 ---------------------------
 
-  shared_atomic_enterprise-5!3.3.2.dist-info/RECORD
+  shared_atomic_enterprise-5!3.3.3.dist-info/RECORD
 
-  offset of local header from start of archive:   6247928
-                                                  (00000000005F55F8h) bytes
+  offset of local header from start of archive:   2653616
+                                                  (0000000000287DB0h) bytes
   file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Sep 7 21:06:08
-  file last modified on (UT extra field modtime): 2023 Sep 7 13:06:07 local
-  file last modified on (UT extra field modtime): 2023 Sep 7 13:06:07 UTC
-  32-bit CRC value (hex):                         ae8d852c
-  compressed size:                                1059 bytes
-  uncompressed size:                              1982 bytes
+  file last modified on (DOS date/time):          2024 Apr 20 13:29:28
+  file last modified on (UT extra field modtime): 2024 Apr 20 05:29:28 local
+  file last modified on (UT extra field modtime): 2024 Apr 20 05:29:28 UTC
+  32-bit CRC value (hex):                         a71ccd31
+  compressed size:                                1096 bytes
+  uncompressed size:                              2014 bytes
   length of filename:                             49 characters
   length of extra field:                          17 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   non-MSDOS external file attributes:             000000 hex
   MS-DOS file attributes (20 hex):                arc 
 
   The central-directory extra field contains:
   - A subfield with ID 0x4453 (Security Descriptor) and 4 data bytes.
-    The local extra field has 152 bytes of NT security descriptor data.
+    The local extra field has 164 bytes of NT security descriptor data.
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access/creation times.
 
   There is no file comment.
 
-Central directory entry #46:
+Central directory entry #35:
 ---------------------------
 
-  shared_atomic_enterprise-5!3.3.2.dist-info/top_level.txt
+  shared_atomic_enterprise-5!3.3.3.dist-info/top_level.txt
 
-  offset of local header from start of archive:   6249180
-                                                  (00000000005F5ADCh) bytes
+  offset of local header from start of archive:   2654905
+                                                  (00000000002882B9h) bytes
   file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   1.0
   compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Sep 7 21:06:08
-  file last modified on (UT extra field modtime): 2023 Sep 7 13:06:07 local
-  file last modified on (UT extra field modtime): 2023 Sep 7 13:06:07 UTC
+  file last modified on (DOS date/time):          2024 Apr 20 13:29:28
+  file last modified on (UT extra field modtime): 2024 Apr 20 05:29:28 local
+  file last modified on (UT extra field modtime): 2024 Apr 20 05:29:28 UTC
   32-bit CRC value (hex):                         3ae435d8
   compressed size:                                14 bytes
   uncompressed size:                              14 bytes
   length of filename:                             56 characters
   length of extra field:                          17 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   non-MSDOS external file attributes:             000000 hex
   MS-DOS file attributes (20 hex):                arc 
 
   The central-directory extra field contains:
   - A subfield with ID 0x4453 (Security Descriptor) and 4 data bytes.
-    The local extra field has 152 bytes of NT security descriptor data.
+    The local extra field has 164 bytes of NT security descriptor data.
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access/creation times.
 
   There is no file comment.
 
-Central directory entry #47:
+Central directory entry #36:
 ---------------------------
 
-  shared_atomic_enterprise-5!3.3.2.dist-info/WHEEL
+  shared_atomic_enterprise-5!3.3.3.dist-info/WHEEL
 
-  offset of local header from start of archive:   6249394
-                                                  (00000000005F5BB2h) bytes
+  offset of local header from start of archive:   2655119
+                                                  (000000000028838Fh) bytes
   file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   1.0
   compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Sep 7 21:06:08
-  file last modified on (UT extra field modtime): 2023 Sep 7 13:06:07 local
-  file last modified on (UT extra field modtime): 2023 Sep 7 13:06:07 UTC
-  32-bit CRC value (hex):                         31fa862c
+  file last modified on (DOS date/time):          2024 Apr 20 13:29:28
+  file last modified on (UT extra field modtime): 2024 Apr 20 05:29:28 local
+  file last modified on (UT extra field modtime): 2024 Apr 20 05:29:28 UTC
+  32-bit CRC value (hex):                         af57acfb
   compressed size:                                99 bytes
   uncompressed size:                              99 bytes
   length of filename:                             48 characters
   length of extra field:                          17 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   non-MSDOS external file attributes:             000000 hex
   MS-DOS file attributes (20 hex):                arc 
 
   The central-directory extra field contains:
   - A subfield with ID 0x4453 (Security Descriptor) and 4 data bytes.
-    The local extra field has 152 bytes of NT security descriptor data.
+    The local extra field has 164 bytes of NT security descriptor data.
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access/creation times.
 
   There is no file comment.
```

## zipnote {}

```diff
@@ -1,142 +1,109 @@
 Filename: shared_atomic/
 Comment: 
 
-Filename: shared_atomic/atomic_activation.pypy39-pp73-win_amd64.pyd
+Filename: shared_atomic/atomic_activation.cp37-win_amd64.pyd
 Comment: 
 
-Filename: shared_atomic/atomic_activation_cpython.cp39-win_amd64.pyd
+Filename: shared_atomic/atomic_async_activation_check.cp37-win_amd64.pyd
 Comment: 
 
-Filename: shared_atomic/atomic_activation_cpython_wrapper.exe
-Comment: 
-
-Filename: shared_atomic/atomic_async_activation_check.pypy39-pp73-win_amd64.pyd
+Filename: shared_atomic/atomic_boolfloat.cp37-win_amd64.pyd
 Comment: 
 
 Filename: shared_atomic/atomic_boolfloat.pxd
 Comment: 
 
-Filename: shared_atomic/atomic_boolfloat.pypy39-pp73-win_amd64.pyd
+Filename: shared_atomic/atomic_bytearray.cp37-win_amd64.pyd
 Comment: 
 
 Filename: shared_atomic/atomic_bytearray.pxd
 Comment: 
 
-Filename: shared_atomic/atomic_bytearray.pypy39-pp73-win_amd64.pyd
-Comment: 
-
-Filename: shared_atomic/atomic_decryption_.cp39-win_amd64.pyd
+Filename: shared_atomic/atomic_decryption_.cp37-win_amd64.pyd
 Comment: 
 
-Filename: shared_atomic/atomic_decryption_.pypy39-pp73-win_amd64.pyd
+Filename: shared_atomic/atomic_int.cp37-win_amd64.pyd
 Comment: 
 
 Filename: shared_atomic/atomic_int.pxd
 Comment: 
 
-Filename: shared_atomic/atomic_int.pypy39-pp73-win_amd64.pyd
+Filename: shared_atomic/atomic_list.cp37-win_amd64.pyd
 Comment: 
 
 Filename: shared_atomic/atomic_list.pxd
 Comment: 
 
-Filename: shared_atomic/atomic_list.pypy39-pp73-win_amd64.pyd
+Filename: shared_atomic/atomic_object.cp37-win_amd64.pyd
 Comment: 
 
 Filename: shared_atomic/atomic_object.pxd
 Comment: 
 
-Filename: shared_atomic/atomic_object.pypy39-pp73-win_amd64.pyd
+Filename: shared_atomic/atomic_object_backend.cp37-win_amd64.pyd
 Comment: 
 
 Filename: shared_atomic/atomic_object_backend.pxd
 Comment: 
 
-Filename: shared_atomic/atomic_object_backend.pypy39-pp73-win_amd64.pyd
+Filename: shared_atomic/atomic_set.cp37-win_amd64.pyd
 Comment: 
 
 Filename: shared_atomic/atomic_set.pxd
 Comment: 
 
-Filename: shared_atomic/atomic_set.pypy39-pp73-win_amd64.pyd
+Filename: shared_atomic/atomic_shared_memory.cp37-win_amd64.pyd
 Comment: 
 
 Filename: shared_atomic/atomic_shared_memory.pxd
 Comment: 
 
-Filename: shared_atomic/atomic_shared_memory.pypy39-pp73-win_amd64.pyd
+Filename: shared_atomic/atomic_string.cp37-win_amd64.pyd
 Comment: 
 
 Filename: shared_atomic/atomic_string.pxd
 Comment: 
 
-Filename: shared_atomic/atomic_string.pypy39-pp73-win_amd64.pyd
-Comment: 
-
 Filename: shared_atomic/atomic_tools.py
 Comment: 
 
-Filename: shared_atomic/cpython_libs.zip
-Comment: 
-
 Filename: shared_atomic/end_user_license_agreement.txt
 Comment: 
 
-Filename: shared_atomic/lib/
-Comment: 
-
 Filename: shared_atomic/libdecryption.dll
 Comment: 
 
 Filename: shared_atomic/libdecryption11.dll
 Comment: 
 
-Filename: shared_atomic/python3.dll
-Comment: 
-
-Filename: shared_atomic/python39.dll
-Comment: 
-
 Filename: shared_atomic/readme.txt
 Comment: 
 
-Filename: shared_atomic/select.pyd
-Comment: 
-
-Filename: shared_atomic/unicodedata.pyd
+Filename: shared_atomic/setup.py
 Comment: 
 
 Filename: shared_atomic/urwid_win_patch.py
 Comment: 
 
-Filename: shared_atomic/_cffi_backend.cp39-win_amd64.pyd
-Comment: 
-
-Filename: shared_atomic/_curses.cp39-win_amd64.pyd
-Comment: 
-
-Filename: shared_atomic/_curses_panel.cp39-win_amd64.pyd
-Comment: 
-
-Filename: shared_atomic/_socket.pyd
+Filename: shared_atomic/_cffi_backend.cp37-win_amd64.pyd
 Comment: 
 
 Filename: shared_atomic/__init__.py
 Comment: 
 
-Filename: shared_atomic_enterprise-5!3.3.2.dist-info/
+Filename: shared_atomic_enterprise-5!3.3.3.dist-info/
 Comment: 
 
-Filename: shared_atomic_enterprise-5!3.3.2.dist-info/METADATA
+Filename: shared_atomic_enterprise-5!3.3.3.dist-info/METADATA
 Comment: 
 
-Filename: shared_atomic_enterprise-5!3.3.2.dist-info/RECORD
+Filename: shared_atomic_enterprise-5!3.3.3.dist-info/RECORD
 Comment: 
 
-Filename: shared_atomic_enterprise-5!3.3.2.dist-info/top_level.txt
+Filename: shared_atomic_enterprise-5!3.3.3.dist-info/top_level.txt
 Comment: 
 
-Filename: shared_atomic_enterprise-5!3.3.2.dist-info/WHEEL
+Filename: shared_atomic_enterprise-5!3.3.3.dist-info/WHEEL
 Comment: 
 
 Zip file comment:
```

## shared_atomic/atomic_boolfloat.pxd

```diff
@@ -5,17 +5,9 @@
 cpdef void bool_set(subprocess_reference reference, bint n) except *
 cpdef bint bool_get_and_set(subprocess_reference reference, bint n) except *
 cpdef bint bool_compare_and_set_value(subprocess_reference reference, bint e, bint n) except *
 
 cdef class atomic_bool(atomic_object):
     cpdef bint get(self) except *
     cpdef void set(self, bint value) except*
-    cpdef void y2(self,
-                                            object_id: int,
-                                            bint windows_unix_compatibility,
-                                            long long reference_m,
-                                            size_t size,
-                                            int creation_pid,
-                                            size_t total_size_including_ending_zeros=*,
-                                            str encoding=*) except *
     cpdef bint bool_get_and_set(self, bint n) except *
     cpdef bint bool_compare_and_set_value(self, bint e, bint n) except *
```

## shared_atomic/atomic_bytearray.pxd

```diff
@@ -1,14 +1,13 @@
 from shared_atomic.atomic_object_backend cimport atomic_object
 from shared_atomic.atomic_object_backend cimport subprocess_reference
 from libc.limits cimport ULLONG_MAX
 
 
 cpdef size_t array_get_int(atomic_bytearray array, subprocess_reference reference) except ?ULLONG_MAX
-
 cpdef bytes array_get_bytes(atomic_bytearray array, subprocess_reference reference, trim=*)
 cpdef void array_set_bytes(atomic_bytearray array, subprocess_reference reference, bytes data) except *
 cpdef bytes array_get_and_set(atomic_bytearray array, subprocess_reference reference, bytes data, bint trim=*)
 cpdef bytes array_compare_and_set_value(atomic_bytearray array, subprocess_reference reference, bytes i , bytes n , bint trim=*)
 cpdef bytes array_add_and_fetch(atomic_bytearray array, subprocess_reference reference, bytes n, bint trim=*)
 cpdef bytes array_sub_and_fetch(atomic_bytearray array, subprocess_reference reference, bytes n, bint trim=*)
 cpdef bytes array_fetch_and_add(atomic_bytearray array, subprocess_reference reference, bytes n, bint trim=*)
@@ -17,22 +16,14 @@
 cpdef bytes array_fetch_and_or(atomic_bytearray array, subprocess_reference reference, bytes n, bint trim=*)
 cpdef bytes array_fetch_and_xor(atomic_bytearray array, subprocess_reference reference, bytes n, bint trim=*)
 cpdef bint array_bittest_and_set(atomic_bytearray array, subprocess_reference reference, char offset) except *
 cpdef bint array_bittest_and_reset(atomic_bytearray array, subprocess_reference reference, char offset) except *
 
 cdef class atomic_bytearray(atomic_object):
     cdef readonly char initial_length
-    cpdef void y2(self,
-                                            object_id: int,
-                                            bint windows_unix_compatibility,
-                                            long long reference_m,
-                                            size_t size,
-                                            int creation_pid,
-                                            size_t total_size_including_ending_zeros=*,
-                                            str encoding=*) except *
     cpdef size_t get_int(self) except ?ULLONG_MAX
     cpdef bytes get_bytes(self, bint trim=*)
     cpdef void set_bytes(self, bytes data) except *
     cpdef bint array_bittest_and_set(self, char offset) except *
     cpdef bint array_bittest_and_reset(self, char offset) except *
     cpdef bytes array_get_and_set(self, bytes data, bint trim=*)
     cpdef bytes array_compare_and_set_value(self, bytes i, bytes n, bint trim=*)
```

## shared_atomic/atomic_int.pxd

```diff
@@ -13,22 +13,15 @@
 cpdef long long int_fetch_and_and(subprocess_reference reference, long long n) except? LLONG_MAX
 cpdef long long int_fetch_and_or(subprocess_reference reference, long long n) except? LLONG_MAX
 cpdef long long int_fetch_and_xor(subprocess_reference reference, long long n) except? LLONG_MAX
 cpdef long long int_bittest_and_set(subprocess_reference reference, long long offset) except 2
 cpdef unsigned char int_bittest_and_reset(subprocess_reference reference, long long offset) except 2
 
 cdef class atomic_int(atomic_object):
-    cpdef void y2(self,
-                                            object_id: int,
-                                            bint windows_unix_compatibility,
-                                            long long reference_m,
-                                            size_t size,
-                                            int creation_pid,
-                                            size_t total_size_including_ending_zeros=*,
-                                            str encoding=*) except *
+
     cpdef long long get(self) except ?LLONG_MAX
     cpdef void set(self, long long value) except *
     cpdef long long int_get_and_set(self, long long n) except ?LLONG_MAX
     cpdef long long int_compare_and_set_value(self, long long e, long long n) except ?LLONG_MAX
     cpdef long long int_add_and_fetch(self, long long n) except ?LLONG_MAX
     cpdef long long int_sub_and_fetch(self, long long n) except ?LLONG_MAX
     cpdef long long int_fetch_and_add(self, long long n) except ?LLONG_MAX
```

## shared_atomic/atomic_list.pxd

```diff
@@ -10,23 +10,15 @@
 cpdef list list_compare_and_set_value(atomic_list input_list, subprocess_reference reference, list i, list n)
 
 cdef class atomic_list(atomic_object):
     cdef readonly char x13
     cdef readonly str x14
     cdef list l1(self, bytes bits_in_bytes)
     cdef tuple l2(self, list input_list)
-    cpdef void y2(self,
-                                            object_id: int,
-                                            bint windows_unix_compatibility,
-                                            long long reference_m,
-                                            size_t size,
-                                            int creation_pid,
-                                            size_t total_size_including_ending_zeros=*,
-                                            str encoding=*) except *
-    cdef tuple l4(self, size_t data_prefix, char accumulate_length, char input_length, char kind)
+    cdef tuple l3(self, size_t data_prefix, char accumulate_length, char input_length, char kind)
     cpdef size_t get_int(self) except ?ULLONG_MAX
     cpdef void set_int(self, size_t integer) except *
     cpdef list get_list(self)
     cpdef void set_list(self, list data) except *
     cpdef list list_get_and_set(self, list data)
     cpdef list list_compare_and_set_value(self, list i, list n)
     cpdef void reencode(self, str newencode) except *
```

## shared_atomic/atomic_object.pxd

```diff
@@ -66,7 +66,9 @@
 from shared_atomic.atomic_shared_memory cimport shared_memory_offset_fetch_and_sub
 from shared_atomic.atomic_shared_memory cimport shared_memory_offset_fetch_and_and
 from shared_atomic.atomic_shared_memory cimport shared_memory_offset_fetch_and_or
 from shared_atomic.atomic_shared_memory cimport shared_memory_offset_fetch_and_xor
 
 from shared_atomic.atomic_shared_memory cimport shared_memory_offset_bittest_and_set
 from shared_atomic.atomic_shared_memory cimport shared_memory_offset_bittest_and_reset
+
+from shared_atomic.atomic_object_backend cimport array2d
```

## shared_atomic/atomic_object_backend.pxd

```diff
@@ -37,103 +37,113 @@
 
 
 
 
 
 
 cdef class atomic_object:
+
     cdef readonly str mode
     cdef readonly size_t size
     cdef bint x3
     cdef long x4
     cdef long x5
     cdef int x6
     cdef long long x7
     cdef long long x8
 
 
     cdef dict x12
-    cpdef void delete(self) except *
     cdef bytes y1(self, long long input, size_t length, bint threadlocal=*)
     cpdef void y2(self,
                                             object_id: int,
                                             bint windows_unix_compatibility,
                                             long long reference_m,
                                             size_t size,
                                             int creation_pid,
-                                            size_t total_size_including_ending_zeros=*,
-                                            str encoding=*) except *
+                                            size_t total_size_including_ending_zeros=*) except *
     cpdef void change_mode(self, str newmode=*, bint windows_unix_compatibility=*) except*
     cdef size_t y3(self, long long input)
     cdef long long y4(self, size_t input)
     cdef  void y5(self) except *
     cdef y6(self, bint windows_unix_compatibility)
 
-
 cdef class subprocess_reference:
     cdef long long x1
     cdef long long x2
 
-    cdef char y41(self) except? CHAR_MAX
-    cdef void y42(self, char n) except *
-    cdef char y43(self, char n) except? CHAR_MAX
-    cdef char y44(self, char e, char n) except? CHAR_MAX
-    cdef char y45(self, char n) except? CHAR_MAX
-    cdef char y46(self, char n) except? CHAR_MAX
-    cdef char y47(self, char n) except? CHAR_MAX
-    cdef char y48(self, char n) except? CHAR_MAX
-    cdef char y49(self, char n) except? CHAR_MAX
-
-    cdef long long y1(self) except? LLONG_MAX
-    cdef void y2(self, long long n) except *
-    cdef long long y3(self, long long n) except? LLONG_MAX
-    cdef long long y4(self, long long e, long long n)  except? LLONG_MAX
-    cdef long long y5(self, long long n) except? LLONG_MAX
-    cdef long long y6(self, long long n) except? LLONG_MAX
-    cdef long long y7(self, long long n) except? LLONG_MAX
-    cdef long long y8(self, long long n) except? LLONG_MAX
-    cdef long long y9(self, long long n) except? LLONG_MAX
-    cdef long long y10(self, long long n) except? LLONG_MAX
-    cdef long long y11(self, long long n) except? LLONG_MAX
-    cdef unsigned char y12(self, long long offset) except 2
-    cdef unsigned char y13(self, long long offset) except 2
-    cdef short y14(self) except? SHRT_MAX
-    cdef void y15(self, short n) except *
-    cdef short y16(self, short n) except? SHRT_MAX
-    cdef short y17(self, short e, short n) except? SHRT_MAX
-
-    cdef short y18(self, short n) except? SHRT_MAX
-    cdef short y19(self, short n) except? SHRT_MAX
-    cdef short y20(self, short n) except? SHRT_MAX
-    cdef short y21(self, short n) except? SHRT_MAX
-    cdef short y22(self, short n) except? SHRT_MAX
-
-    cdef long y23(self) except? INT_MAX
-    cdef void y24(self, long n) except *
-    cdef long y25(self, long n) except? INT_MAX
-    cdef long y26(self, long e, long n) except? INT_MAX
-    cdef long y27(self, long n) except? INT_MAX
-    cdef long y28(self, long n) except? INT_MAX
-    cdef long y29(self, long n) except? INT_MAX
-    cdef long y30(self, long n) except? INT_MAX
-    cdef long y34(self, long n) except? INT_MAX
-    cdef long y35(self, long n) except? INT_MAX
-    cdef long y36(self, long n) except? INT_MAX
-    cdef unsigned char y37(self, long offset) except 2
-    cdef unsigned char y38(self, long offset) except 2
-    cdef int y39(self, int size,
-                                                     char *i, int i_length,  char * n, int n_length,
-                                                     char * out) except -1
-    cdef int y40(self,  char *i,  char *n,
-                                                   size_t offset, size_t size, size_t total_size_including_ending_zeros, int length,
-                                                    char * result) except -1
+    cdef char y1(self) except? 0
+    cdef void y2(self, char n) except*
+    cdef char y3(self, char n) except? 0
+    cdef char y4(self, char e, char n) except? 0
+    cdef char y5(self, char n) except? 0
+    cdef char y6(self, char n) except? 0
+    cdef char y7(self, char n) except? 0
+    cdef char y8(self, char n) except? 0
+    cdef char y9(self, char n) except? 0
+
+    cdef long long y10(self) except? 0
+    cdef void y11(self, long long n) except*
+    cdef long long y12(self, long long n) except? 0
+    cdef long long y13(self, long long e, long long n)  except? 0
+    cdef long long y14(self, long long n) except? 0
+    cdef long long y15(self, long long n) except? 0
+    cdef long long y16(self, long long n) except? 0
+    cdef long long y17(self, long long n) except? 0
+    cdef long long y18(self, long long n) except? 0
+    cdef long long y19(self, long long n) except? 0
+    cdef long long y20(self, long long n) except? 0
+    cdef unsigned char y21(self, long long offset) except 2
+    cdef unsigned char y22(self, long long offset) except 2
+    cdef short y23(self) except? 0
+    cdef void y24(self, short n) except*
+    cdef short y25(self, short n) except? 0
+    cdef short y27(self, short e, short n) except? 0
+
+    cdef short y28(self, short n) except? 0
+    cdef short y29(self, short n) except? 0
+    cdef short y30(self, short n) except? 0
+    cdef short y31(self, short n) except? 0
+    cdef short y32(self, short n) except? 0
+
+    cdef long y33(self) except? 0
+    cdef void y34(self, long n) except*
+    cdef long y35(self, long n) except? 0
+    cdef long y36(self, long e, long n) except? 0
+    cdef long y37(self, long n) except? 0
+    cdef long y38(self, long n) except? 0
+    cdef long y39(self, long n) except? 0
+    cdef long y40(self, long n) except? 0
+    cdef long y41(self, long n) except? 0
+    cdef long y42(self, long n) except? 0
+    cdef long y43(self, long n) except? 0
+    cdef unsigned char y44(self, long offset) except 2
+    cdef unsigned char y45(self, long offset) except 2
+    cdef int y46(self, int size,
+                                           char *i, int i_length, char * n, int n_length,
+                                           char * out) except -1
+    cdef int y47(self, char *i, char *n,
+                                                         size_t offset, size_t size,
+                                                         size_t total_size_including_ending_zeros, int length,
+                                                         char * result) except -1
+
+
+
 
 cdef class multiprocessing_reference(subprocess_reference):
     cdef long long x3
     cdef dict x4
 
     cdef void close_reference(self, bint windows_unix_compatibility) except *
 
 
 cpdef subprocess_reference get_reference(atomic_object a)
 cpdef void release_reference(subprocess_reference a) except *
 
+cdef class array2d:
+    cdef void * x1
+    cdef bint x2
+    cdef size_t x3
+    cdef size_t x4
+    cdef size_t x5
+    cdef Py_ssize_t x6[2]
+    cdef Py_ssize_t z7[2]
```

## shared_atomic/atomic_set.pxd

```diff
@@ -9,23 +9,15 @@
 cpdef void set_set_set(atomic_set intput_set, subprocess_reference reference, set data) except*
 cpdef set set_get_and_set(atomic_set intput_set, subprocess_reference reference, set data)
 cpdef set set_compare_and_set_value(atomic_set intput_set, subprocess_reference reference, set i, set n)
 
 cdef class atomic_set(atomic_object):
     cdef set s1(self, bytes bits_in_bytes)
     cdef tuple s2(self, set input_set)
-    cpdef void y2(self,
-                                            object_id: int,
-                                            bint windows_unix_compatibility,
-                                            long long reference_m,
-                                            size_t size,
-                                            int creation_pid,
-                                            size_t total_size_including_ending_zeros=*,
-                                            str encoding=*) except *
-    cdef tuple s4(self, size_t data_prefix, char accumulate_length,char input_length, char kind)
+    cdef tuple s3(self, size_t data_prefix, char accumulate_length,char input_length, char kind)
     cpdef size_t get_int(self) except ?ULLONG_MAX
     cpdef void set_int(self, size_t integer) except*
     cpdef set get_set(self)
     cpdef void set_set(self, set data) except*
     cpdef set set_get_and_set(self, set data)
     cpdef set set_compare_and_set_value(self, set i, set n)
     cpdef void reencode(self, str newencode) except*
```

## shared_atomic/atomic_shared_memory.pxd

```diff
@@ -20,24 +20,25 @@
     cdef readonly bint x13
     cdef long long x14
     cdef public bint x15
     cdef str x16
     cdef Py_ssize_t x18[1]
     cdef Py_ssize_t x19[1]
     cdef size_t x20
-
-    cpdef void delete(self) except *
+    cdef bytes y3(self, str previous_shared_memory_path)
+    cdef list y4(self, size_t length)
+    cdef int y5(self) except -1
     cpdef void y2(self,
                                             object_id: int,
                                             bint windows_unix_compatibility,
                                             long long reference_m,
                                             size_t size,
                                             int creation_pid,
-                                            size_t total_size_including_ending_zeros=*,
-                                            str encoding=*) except*
+                                            size_t total_size_including_ending_zeros=*) except*
+
     cpdef int file_sync(self, bint async=*, size_t start=*, size_t length=*) except -1
     cdef int s2(self, char operation_length) except -1
 
     cpdef void offset_memmove(self, mv:memoryview, size_t offset = *, str io_flags = *) except *
     cpdef bytes offset_get(self, size_t offset  = *, char length = *)
     cpdef bytes offset_get_and_set(self, bytes value, size_t offset  = *)
     cpdef bytes offset_compare_and_set_value(self, bytes i, bytes n, size_t offset  = *)
@@ -67,15 +68,14 @@
     cpdef char [: , ::1] offset_fetch_and_ands(self, const char[:, :] values, const size_t[:] offsets, const char[:] lengths, size_t parallelism=*) except *
     cpdef char [: , ::1] offset_fetch_and_ors(self, const char[:, :] values, const size_t[:] offsets, const char[:] lengths, size_t parallelism=*) except *
     cpdef char [: , ::1] offset_fetch_and_xors(self, const char[:, :] values, const size_t[:] offsets, const char[:] lengths, size_t parallelism=*) except *
 
     cpdef unsigned char [::1] offset_bittest_and_sets(self, const size_t[:] left_offsets, size_t parallelism=*) except *
     cpdef unsigned char [::1] offset_bittest_and_resets(self, const size_t[:] left_offsets, size_t parallelism=*) except *
 
-
     cdef void s3(self,  unsigned char[:] mv, unsigned char * reference, size_t length) except *
     cdef void s4(self,  const unsigned char[:] mv, unsigned char * reference, size_t length) except *
     cpdef void offset_memmove(self, mv: memoryview, size_t offset = *, str io_flags =*) except *
     cpdef size_t memdump(self, str file_path, size_t start=*, size_t length=*) except ?ULLONG_MAX
     cdef tuple s5(self, size_t start, size_t length)
```

## shared_atomic/atomic_string.pxd

```diff
@@ -10,28 +10,21 @@
 cpdef void string_set_string(atomic_string string, subprocess_reference reference, str data) except *
 cpdef str string_get_and_set(atomic_string string, subprocess_reference reference, str data)
 cpdef str string_compare_and_set_value(atomic_string string, subprocess_reference reference, str i, str n)
 
 cdef class atomic_string(atomic_object):
     cdef readonly str x13
     cdef readonly char x14
-    cpdef void y2(self,
-                                            object_id: int,
-                                            bint windows_unix_compatibility,
-                                            long long reference_m,
-                                            size_t size,
-                                            int creation_pid,
-                                            size_t total_size_including_ending_zeros=*,
-                                            str encoding=*) except *
-    cdef str s2(self, long long input)
-    cdef  size_t  s3(self) except ?ULLONG_MAX
+
+    cdef str s1(self, long long input)
+    cdef  size_t  s2(self) except ?ULLONG_MAX
     cpdef str get_string(self)
     cpdef void set_string(self, str data) except *
-    cdef void s4(self, size_t input) except *
-    cdef void s5(self, bytes data) except *
+    cdef void s3(self, size_t input) except *
+    cdef void s4(self, bytes data) except *
     cpdef str string_compare_and_set_value(self, str i, str n)
     cpdef str string_get_and_set(self, str data)
     cpdef void resize(self, char newlength,
                 str paddingdirection = *,
                 str paddingstr  = *,
                 str trimming_direction  = *) except *
     cpdef void reencode(self, str newencode) except*
```

## shared_atomic/atomic_tools.py

```diff
@@ -1,30 +1,32 @@
 import sys
 from pathlib import Path
 importpath = str(Path(__file__).parent.parent)
 sys.path[0] = importpath
 import argparse
-from shared_atomic.atomic_activation import modify_proxy
+from shared_atomic.atomic_activation import activation, modify_proxy
 
 if sys.platform not in ('darwin', 'linux','win32'):
     raise NotImplementedError('Unsupported platform!')
 
 def test_activation():
     activation()
 
 
 if __name__ == "__main__":
 
     parser = argparse.ArgumentParser(description="user tools for Shared Atomic Enterprise")
     parser.add_argument('-a','--action',
-                        choices=['p'],
-                        help="p for proxy setting",
+                        choices=['a','p'],
+                        help="a for activation, p for proxy setting",
                         required=True,
                         dest='action')
     parsed = parser.parse_args()
+    if parsed.action == 'a':
+        activation()
 
-    if parsed.action == 'p':
+    elif parsed.action == 'p':
         modify_proxy()
     else:
         print("Invalid action!")
         exit()
```

## shared_atomic/end_user_license_agreement.txt

```diff
@@ -87,15 +87,15 @@
 The service agreement could be found at https://sharedatomic.top/enterprise_service.html
 
 20) Complete term:
 This EULA includs supplement terms and terms in the external links, because they are all components of this EULA.
 After installation and activation, licensee could still read it by restart the activation process, and click "Read End User Licence Agreement" Button
 
 21) Other authors:
-The embedded urwid_win_patch.py and code under urwid in cpython_libs.zip is under following GNU LESSER GENERAL PUBLIC LICENSE.
+The embedded urwid_win_patch.py is under following GNU LESSER GENERAL PUBLIC LICENSE.
 
               GNU LESSER GENERAL PUBLIC LICENSE
                    Version 2.1, February 1999
 
      Copyright (C) 1991, 1999 Free Software Foundation, Inc.
      51 Franklin Street, Fifth Floor, Boston, MA  02110-1301  USA
      Everyone is permitted to copy and distribute verbatim copies
@@ -592,15 +592,15 @@
       library `Frob' (a library for tweaking knobs) written by James Random Hacker.
 
       <signature of Ty Coon>, 1 April 1990
       Ty Coon, President of Vice
 
     That's all there is to it!
 
-The embedded cffi, whose author is Armin Rigo and Maciej Fijalkowski, as a dependency named _cffi_backend.cp39-win_amd64.pyd, is under following MIT licence.
+The embedded cffi, whose author is Armin Rigo and Maciej Fijalkowski, as a dependency named _cffi_backend.cp37-win_amd64.pyd, is under following MIT licence.
 
     The MIT License
 
     Permission is hereby granted, free of charge, to any person
     obtaining a copy of this software and associated documentation
     files (the "Software"), to deal in the Software without
     restriction, including without limitation the rights to use,
@@ -623,120 +623,15 @@
     distribute, sublicense, and/or sell copies of the Software, and to
     permit persons to whom the Software is furnished to do so, subject to
     the following conditions:
 
     The above copyright notice and this permission notice shall be
     included in all copies or substantial portions of the Software.
 
-The embedded python, which are named as python3.dll, python39.dll,
-_socket.pyd, select.pyd, unicodedata.pyd and zipped in cpython_libs.zip except urwid
-and urwid_win_patch.py as well as the embedded windows_curses dependencies as
-_curses_panel.cp39-win_amd64.pyd and _curses.cp39-win_amd64.pyd are under PYTHON SOFTWARE FOUNDATION LICENSE VERSION 2.
-the posix module in the dependency uses the OpenSSL library for added performance. The OpenSSL library is under the Openssl Licence
-and Original SSLeay License which has been stated bellow.
-
-    PYTHON SOFTWARE FOUNDATION LICENSE VERSION 2
-    --------------------------------------------
-
-    1. This LICENSE AGREEMENT is between the Python Software Foundation
-    ("PSF"), and the Individual or Organization ("Licensee") accessing and
-    otherwise using this software ("Python") in source or binary form and
-    its associated documentation.
-
-    2. Subject to the terms and conditions of this License Agreement, PSF hereby
-    grants Licensee a nonexclusive, royalty-free, world-wide license to reproduce,
-    analyze, test, perform and/or display publicly, prepare derivative works,
-    distribute, and otherwise use Python alone or in any derivative version,
-    provided, however, that PSF's License Agreement and PSF's notice of copyright,
-    i.e., "Copyright (c) 2001, 2002, 2003, 2004, 2005, 2006, 2007, 2008, 2009, 2010,
-    2011, 2012, 2013, 2014, 2015, 2016, 2017, 2018, 2019, 2020 Python Software Foundation;
-    All Rights Reserved" are retained in Python alone or in any derivative version
-    prepared by Licensee.
-
-    3. In the event Licensee prepares a derivative work that is based on
-    or incorporates Python or any part thereof, and wants to make
-    the derivative work available to others as provided herein, then
-    Licensee hereby agrees to include in any such work a brief summary of
-    the changes made to Python.
-
-    4. PSF is making Python available to Licensee on an "AS IS"
-    basis.  PSF MAKES NO REPRESENTATIONS OR WARRANTIES, EXPRESS OR
-    IMPLIED.  BY WAY OF EXAMPLE, BUT NOT LIMITATION, PSF MAKES NO AND
-    DISCLAIMS ANY REPRESENTATION OR WARRANTY OF MERCHANTABILITY OR FITNESS
-    FOR ANY PARTICULAR PURPOSE OR THAT THE USE OF PYTHON WILL NOT
-    INFRINGE ANY THIRD PARTY RIGHTS.
-
-    5. PSF SHALL NOT BE LIABLE TO LICENSEE OR ANY OTHER USERS OF PYTHON
-    FOR ANY INCIDENTAL, SPECIAL, OR CONSEQUENTIAL DAMAGES OR LOSS AS
-    A RESULT OF MODIFYING, DISTRIBUTING, OR OTHERWISE USING PYTHON,
-    OR ANY DERIVATIVE THEREOF, EVEN IF ADVISED OF THE POSSIBILITY THEREOF.
-
-    6. This License Agreement will automatically terminate upon a material
-    breach of its terms and conditions.
-
-    7. Nothing in this License Agreement shall be deemed to create any
-    relationship of agency, partnership, or joint venture between PSF and
-    Licensee.  This License Agreement does not grant permission to use PSF
-    trademarks or trade name in a trademark sense to endorse or promote
-    products or services of Licensee, or any third party.
-
-    8. By copying, installing or otherwise using Python, Licensee
-    agrees to be bound by the terms and conditions of this License
-    Agreement.
-
-    SipHash24
-    Files mentioned above, contains
-    Marek Majkowski's implementation of Dan Bernstein's SipHash24 algorithm. It contains the following note:
-    <MIT License>
-    Copyright (c) 2013  Marek Majkowski <marek@popcount.org>
-
-    Permission is hereby granted, free of charge, to any person obtaining a copy
-    of this software and associated documentation files (the "Software"), to deal
-    in the Software without restriction, including without limitation the rights
-    to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-    copies of the Software, and to permit persons to whom the Software is
-    furnished to do so, subject to the following conditions:
-
-    The above copyright notice and this permission notice shall be included in
-    all copies or substantial portions of the Software.
-    </MIT License>
-
-    Original location:
-       https://github.com/majek/csiphash/
-
-    Solution inspired by code from:
-       Samuel Neves (supercop/crypto_auth/siphash24/little)
-       djb (supercop/crypto_auth/siphash24/little2)
-       Jean-Philippe Aumasson (https://131002.net/siphash/siphash24.c)
-
-    strtod and dtoa
-    Files mentioned above, contains C functions dtoa and strtod for conversion of C
-    doubles to and from strings,
-    is derived from the file of the same name by David M. Gay, currently available
-    from https://web.archive.org/web/20220517033456/http://www.netlib.org/fp/dtoa.c.
-    The original file, as retrieved on March 16, 2009, contains the following copyright
-    and licensing notice:
-    /****************************************************************
-     *
-     * The author of this software is David M. Gay.
-     *
-     * Copyright (c) 1991, 2000, 2001 by Lucent Technologies.
-     *
-     * Permission to use, copy, modify, and distribute this software for any
-     * purpose without fee is hereby granted, provided that this entire notice
-     * is included in all copies of any software which is or includes a copy
-     * or modification of this software and in all copies of the supporting
-     * documentation for such software.
-     *
-     * THIS SOFTWARE IS BEING PROVIDED "AS IS", WITHOUT ANY EXPRESS OR IMPLIED
-     * WARRANTY.  IN PARTICULAR, NEITHER THE AUTHOR NOR LUCENT MAKES ANY
-     * REPRESENTATION OR WARRANTY OF ANY KIND CONCERNING THE MERCHANTABILITY
-     * OF THIS SOFTWARE OR ITS FITNESS FOR ANY PARTICULAR PURPOSE.
-     *
-     ***************************************************************/
+
 
 The embedded openssl, embedded in libdecryption11.dll and libdecryption.dll, is under following double licences.
 
       OpenSSL License
       ---------------
     /* ====================================================================
      * Copyright (c) 1998-2019 The OpenSSL Project.  All rights reserved.
```

## shared_atomic/libdecryption.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x0000000180283860
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Thu Sep  7 12:57:15 2023
+Time/Date		Sat Apr 20 05:25:26 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	29
 SizeOfCode		0000000000285000
 SizeOfInitializedData	00000000000d2e00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000283860
@@ -948342,16 +948342,17 @@
 	...
    18031f188:	and    %bl,0x180(%rbx,%rsi,1)
    18031f18f:	add    %al,%al
    18031f191:	pushf
    18031f192:	xor    0x1(%rax),%eax
    18031f198:	add    %al,(%rax)
    18031f19a:	add    %al,(%rax)
-   18031f19c:	stos   %eax,%es:(%rdi)
-   18031f19d:	enter  $0x64f9,$0x0
+   18031f19c:	(bad)
+   18031f19d:	push   %rcx
+   18031f19e:	and    0x0(%rsi),%esp
    18031f1a1:	add    %al,(%rax)
    18031f1a3:	add    %cl,0x7c000000(%rip)        # 0x1fc31f1a9
    18031f1a9:	add    (%rax),%al
    18031f1ab:	add    %cl,%al
    18031f1ad:	clc
    18031f1ae:	xor    %eax,(%rax)
    18031f1b0:	enter  $0x31ec,$0x0
```

## shared_atomic/libdecryption11.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x0000000180001320
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Thu Sep  7 12:57:16 2023
+Time/Date		Sat Apr 20 05:25:26 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	29
 SizeOfCode		0000000000000e00
 SizeOfInitializedData	0000000000001400
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000001320
@@ -1464,17 +1464,19 @@
    18000215a:	(bad)
    18000215b:	(bad)
    18000215c:	(bad)
    18000215d:	(bad)
    18000215e:	(bad)
    18000215f:	incl   (%rax)
    180002161:	add    %al,(%rax)
-   180002163:	add    %ch,0x64f9(%rax,%rcx,8)
-   18000216a:	add    %al,(%rax)
-   18000216c:	or     $0x58000000,%eax
+   180002163:	add    %al,%dh
+   180002165:	push   %rcx
+   180002166:	and    0x0(%rsi),%esp
+   180002169:	add    %al,(%rax)
+   18000216b:	add    %cl,0x58000000(%rip)        # 0x1d8002171
    180002171:	add    (%rax),%al
    180002173:	add    %bl,(%rax)
    180002175:	and    (%rax),%eax
    180002177:	add    %bl,(%rax)
    180002179:	adc    $0x0,%eax
    18000217e:	add    %al,(%rax)
    180002180:	cmp    %al,(%rcx)
```

## shared_atomic/urwid_win_patch.py

```diff
@@ -1,20 +1,34 @@
 """
 Patch urwid on Windows and WSL.
 
 On Windows, install the package "windows-curses".
 """
 import curses
+import platform
+import re
 
 import urwid
 import urwid.curses_display
 import urwid.raw_display
 
-IS_WSL = False
-IS_WINDOWS = True
+IS_WSL = ("Linux" in platform.platform()) and ("Microsoft" in platform.platform())
+IS_WINDOWS = ("Windows" in platform.platform()) and ("Linux" not in platform.platform())
+
+if IS_WSL:
+    # Filter out SI/SO under WSL. See:
+    # https://github.com/mitmproxy/mitmproxy/blob/8dfb8a9a7471e00b0f723de66d3b63bd089e9802/mitmproxy/tools/console/window.py#L316-L323
+    wsl_patch_orig_write = urwid.raw_display.Screen.write
+    wsl_patch_write_re = re.compile("[\x0e\x0f]")
+
+    def wsl_patch_write(self, data):
+        data = wsl_patch_write_re.sub("", data)
+        return wsl_patch_orig_write(self, data)
+
+    urwid.raw_display.Screen.write = wsl_patch_write
 
 if IS_WINDOWS:
     def win_patch_tty_signal_keys(self, intr=None, quit=None, start=None, stop=None, susp=None, fileno=None):
         pass  # no signals on Windows; not needed for resize
     urwid.display_common.RealTerminal.tty_signal_keys = win_patch_tty_signal_keys
 
     win_patch_orig__start = urwid.curses_display.Screen._start
```

## Comparing `shared_atomic_enterprise-5!3.3.2.dist-info/METADATA` & `shared_atomic_enterprise-5!3.3.3.dist-info/METADATA`

 * *Files 24% similar despite different names*

```diff
@@ -1,106 +1,107 @@
-Metadata-Version: 2.1
-Name: shared-atomic-enterprise
-Version: 5!3.3.2
-Summary: Shared atomicity with multiprocessing or multiple threads
-Home-page: https://sharedatomic.top/
-Author: Xiquan Ren
-Author-email: xiquanren@yandex.com
-Requires-Python: >=3.6
-
-This package provided a second way to access those shared data types with atomic operations.
-can be used on
-
- - macOS x86_64,
-
- - Microsoft Windows 10 x64, Windows Server 2019 x64
-
- - Centos7,9/RHEL7,9 x86_64,
-
- - Ubuntu Linux 18, 20, 22 x86_64 and
-
- - Suse Linux Enterprise Server 12, 15 x86_84.
-
-
-This is copyright software, you should buy it at https://sharedatomic.top/enterprise/payment to get a licence to use it. For the price and details, please check
-https://sharedatomic.top/enterprise/payment.
-
-Included Datatypes
-
- - atomic_int
-
- - atomic_uint
-
- - atomic_float
-
- - atomic_bool
-
- - atomic_bytearray
-
- - atomic_string
-
- - atomic_shared_memory
-
- - atomic_set, package bitarray >= 2.4.0 is needed.
-
- - atomic_list, package bitarray >= 2.4.0 is needed.
-
-LINUX/macOS
-
- - CPython 3.6 - 3.11, if compiled by the user, for CPython3.6 --enable-shared should be added in the configuration parameter
-
- - Pypy 3.8 - 3.10(numpy should be installed to use the atomic_shared_memory)
-
- - The package requires libatomic and libgomp installed on the Linux platforms
-
- - bitarray if you need to use atomic_set or atomic_list
-
- - urwid==2.1.2 to activate the package
-
-Windows
-
- - CPython 3.6 - 3.11
-
- - Pypy 3.8 - 3.10(numpy should be installed to use the atomic_shared_memory)
-
- - Microsoft Visual C++ 2019 Redistributable(X64)
-
- - bitarray if you need to use atomic_set or atomic_list
-
- - for CPython, windows-curses==2.3.1 and urwid==2.1.2 to activate the package on windows
-
-
-Installation
-
-To install shared_atomic, use pip:
-
-The binary distribution of the software is compiled and delivered in different epochs.
-
- - macOS only x86_64 platform supported, silicon not supported
-        epoch 1: version 1!3.3.2
-
- - Redhat or Centos Linux, only centos7,9/rhel7,9 on x86_64 platform supported.
-        epoch 2: version 2!3.3.2
-
- - Ubuntu Linux 18, 20, 22 on x86_64 platform supported
-        epoch 3: version 3!3.3.2
-
- - Suse Linux Enterprise Server 12, 15 on x86_64 platform supported
-        epoch 4: version 4!3.3.2
-
- - Microsoft Windows x64, Windows 10 and Windows server 2019 supported
-        epoch 5: version 5!3.3.2
-
-On Linux, you need assistance from the root user,
-
-    If you are a root user, it is ok, then only root can run this package.
-    If you are not root user, in the activation process you will need assistance from the root user.
-
-    cd (the directory where the package is installed )
-    chown root shared_atomic/atomic_python_suid
-    chmod u+s shared_atomic/atomic_python_suid
-
-    then the user who installed the package can run the package.
-
-For documentation, please go to:
-
- https://sharedatomic.top/
+Metadata-Version: 2.1
+Name: shared-atomic-enterprise
+Version: 5!3.3.3
+Summary: Shared atomicity with multiprocessing or multiple threads
+Home-page: https://sharedatomic.top/
+Author: Xiquan Ren
+Author-email: xiquanren@yandex.com
+Requires-Python: >=3.6
+Requires-Dist: urwid (>=2.1.2)
+Requires-Dist: windows-curses (==2.3.1)
+
+This package provided a second way to access those shared data types with atomic operations.
+can be used on
+
+ - macOS x86_64,
+
+ - Microsoft Windows 10 x64, Windows Server 2019 x64
+
+ - Centos7,9/RHEL7,9 x86_64,
+
+ - Ubuntu Linux 18, 20, 22 x86_64 and
+
+ - Suse Linux Enterprise Server 12, 15 x86_84.
+
+
+This is copyright software, you should buy it at https://sharedatomic.top/enterprise/payment to get a licence to use it. For the price and details, please check
+https://sharedatomic.top/enterprise/payment.
+
+Included Datatypes
+
+ - atomic_int
+
+ - atomic_uint
+
+ - atomic_float
+
+ - atomic_bool
+
+ - atomic_bytearray
+
+ - atomic_string
+
+ - atomic_shared_memory
+
+ - atomic_set, package bitarray >= 2.4.0 is needed.
+
+ - atomic_list, package bitarray >= 2.4.0 is needed.
+
+LINUX/macOS
+
+ - CPython 3.7 - 3.11
+
+ - Pypy 3.8 - 3.10(numpy should be installed to use the atomic_shared_memory)
+
+ - The package requires libatomic and libgomp installed on the Linux platforms
+
+ - bitarray if you need to use atomic_set or atomic_list
+
+ - urwid==2.1.2 to activate the package
+
+Windows
+
+ - CPython 3.7 - 3.11
+
+ - Pypy TBD
+
+ - Microsoft Visual C++ 2019 Redistributable(X64)
+
+ - bitarray if you need to use atomic_set or atomic_list
+
+ - for CPython, windows-curses==2.3.1 and urwid==2.1.2 to activate the package on windows
+
+Installation
+
+To install shared_atomic, use pip:
+
+The binary distribution of the software is compiled and delivered in different epochs.
+
+ - macOS only x86_64 platform supported, silicon not supported
+        epoch 1: version 1!3.3.2
+
+ - Redhat or Centos Linux, only centos7,9/rhel7,9 on x86_64 platform supported.
+        epoch 2: version 2!3.3.2
+
+ - Ubuntu Linux 18, 20, 22 on x86_64 platform supported
+        epoch 3: version 3!3.3.2
+
+ - Suse Linux Enterprise Server 12, 15 on x86_64 platform supported
+        epoch 4: version 4!3.3.2
+
+ - Microsoft Windows x64, Windows 10 and Windows server 2019 supported
+        epoch 5: version **5!3.3.3**
+
+On Linux, you need assistance from the root user,
+
+    If you are a root user, it is ok, then only root can run this package.
+    If you are not root user, in the activation process you will need assistance from the root user.
+
+    cd (the directory where the package is installed )
+    chown root shared_atomic/atomic_python_suid
+    chmod u+s shared_atomic/atomic_python_suid
+
+    then the user who installed the package can run the package.
+
+For documentation, please go to:
+
+ https://sharedatomic.top/
```

## Comparing `shared_atomic_enterprise-5!3.3.2.dist-info/RECORD` & `shared_atomic_enterprise-5!3.3.3.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 shared_atomic/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-shared_atomic/atomic_activation.py,sha256=dw5e-GbjKYCTwJRyN3eNjCKqHQZXQEiSM1dm8YJAQQ0,113519
-shared_atomic/atomic_activation_cpython.py,sha256=jsESjtsiBT7LNaQFl5f0lMjb3e2icGDFWez5uIxcgcU,145362
-shared_atomic/atomic_async_activation_check.py,sha256=d-UZzaC-T7NEzZtvFYQL8tEwcWQAw4T-2ysA0OPD8Y4,120055
+shared_atomic/atomic_activation.py,sha256=v7RPI5HpTz04waJjGBCsX1yMxV6zDOeHHyHru6z1GPU,254730
+shared_atomic/atomic_async_activation_check.py,sha256=cgpU53-WB6b74Wo-FKB4V9RLsjetYpdIDZItiUg2r0I,120057
 shared_atomic/atomic_cffi_compile_steps.py,sha256=MenlES3epvB4UdwbstvsJV8BpAhpM6uELZOCqYsPhfo,9642
-shared_atomic/atomic_decryption.py,sha256=obn311YyyFDWa8YC8zi6c9Zi64ZjG-zU6Hmm7VozoRk,8833
-shared_atomic/atomic_tools.py,sha256=1mAEHss3fmsky8mylMHiXkYXCI8OjfC1LJ0rWNqPdlI,807
-shared_atomic/end_user_license_agreement.txt,sha256=dZhk4sAncMvZyqJGxPtKlOtPClov09o-yPIxBlueFGM,49659
+shared_atomic/atomic_decryption.py,sha256=uGrvezcQS_zmhVyv83K4f0L-gHJ354wB6IlAshZ-uig,10889
+shared_atomic/atomic_tools.py,sha256=UuirDkkB291zP4V0Do8NzvfugKIi_1RgoPrEqspVafk,893
+shared_atomic/end_user_license_agreement.txt,sha256=QE6oBgQpCSOx5oSCIBWRanZWkQz6O-uXa98RnpNags0,43072
 shared_atomic/readme.txt,sha256=6IxCg_jJX7J2obkZOdu5-R7qwFugMxmmbuezfyEtmek,622
-shared_atomic/test_atomic_array_pypy.py,sha256=ksh0oVzOZeg2pJ-rEXXdxur2GXuii4g3vIitnv0Ld1Y,15837
-shared_atomic/test_atomic_boolfloat_pypy.py,sha256=2kfRo69zgqjZ_2NZk6hb6pfkWTgjWp99Xac6H2Syb_8,4923
-shared_atomic/test_atomic_int_pypy.py,sha256=xbrYB7K_vUVbzROfGvGTZR9FBwD2uzptQ4OHGGjDA0w,6894
-shared_atomic/test_atomic_list_pypy.py,sha256=TCvNv6RKgQj1NkOCrKWgB-vehWCpeBBGjhSeqtixu3U,7124
-shared_atomic/test_atomic_set_pypy.py,sha256=8uYEsBNsIYc3gtzMaRQX9Nv9agXM-1BVBBXX2ocJkbI,6873
-shared_atomic/test_atomic_string_pypy.py,sha256=yzTnaOZzW9dqGCXk-MA8PJ8hteTXW3QEV84CvO9cvwg,19659
-shared_atomic/test_shared_atomic_memory_pypy.py,sha256=Zz3EIG2mQ0szsmYxDXRHIOS0X-c0xmTEgVDtHTA7j7w,103712
-shared_atomic/urwid_win_patch.py,sha256=wSfWCi-0-qGSzRhGwtmVFniY05utNBWsLPoEPWK-NOg,3423
-shared_atomic_enterprise-5!3.3.2.dist-info/METADATA,sha256=sHkvxaMnvAfY8fMPRoTaKLMFMZJ6MDaivWZd76xq8hA,2981
-shared_atomic_enterprise-5!3.3.2.dist-info/WHEEL,sha256=sI3GdCDJNQxw9EGj6EdjKhjDI8Yk5MVx4zVQGYccuiA,99
-shared_atomic_enterprise-5!3.3.2.dist-info/top_level.txt,sha256=ECuvZjfIYXkJKlEJiYCjOmL-6tkj6X4Sm8VM3-Fppbc,14
-shared_atomic_enterprise-5!3.3.2.dist-info/RECORD,,
+shared_atomic/setup.py,sha256=7esXb3buxHQwHx0UC_9L8_z3bq5E9AxCW2thX_C_XfI,2754
+shared_atomic/test_all_master.py,sha256=zAvbig_VYlknlZxFoOht980JXwU1Nlw17rlATcX8UHk,1734
+shared_atomic/test_atomic_array.py,sha256=DFDn8yFfiQ8LlDiQcuGawtE9BCivOw2n7j4adeomxmE,15894
+shared_atomic/test_atomic_boolfloat.py,sha256=SafsXCX-Tu5r3ScClv8DVGihN6uVNzBMKf_mibRynh0,5397
+shared_atomic/test_atomic_int.py,sha256=2_62TKHwKHpdm6rCR5Q-nDA5UJDzRBtVfnqFdbOZEA4,7119
+shared_atomic/test_atomic_list.py,sha256=RE8riySb8jFvEgy1zTNFLRX0XKpvbfBtzbXCLJS2vA0,7364
+shared_atomic/test_atomic_set.py,sha256=99gGe8BsvqBeo3DwtOtBp-wG43_YivdQcCliwobfg-Q,7241
+shared_atomic/test_atomic_string.py,sha256=n-HFV0guyNsJFW09vwIdUzmbAQiLBDWXUltes_kRgXg,19709
+shared_atomic/test_shared_atomic_memory.py,sha256=QJKHxwHdTzplRi6FEWBGkoLJiiMoJXCkqWFwymjq5mY,99624
+shared_atomic/urwid_win_patch.py,sha256=MPrVW6fAzv8atOSovjoqbjn8GU0x6fj_fAFbov6t5CU,4070
+shared_atomic_enterprise-5!3.3.3.dist-info/METADATA,sha256=zBRTF_AM0CVHvigeq33m8lsqyaVOxr_mSPe8ncckzRw,2779
+shared_atomic_enterprise-5!3.3.3.dist-info/WHEEL,sha256=d5BRf1hFvJ9Ex5OFln3RMpEurUovL-c8NrP67oLgDUk,99
+shared_atomic_enterprise-5!3.3.3.dist-info/top_level.txt,sha256=ECuvZjfIYXkJKlEJiYCjOmL-6tkj6X4Sm8VM3-Fppbc,14
+shared_atomic_enterprise-5!3.3.3.dist-info/RECORD,,
```

