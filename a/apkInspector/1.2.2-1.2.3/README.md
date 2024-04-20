# Comparing `tmp/apkinspector-1.2.2.tar.gz` & `tmp/apkinspector-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apkinspector-1.2.2.tar", max compression
+gzip compressed data, was "apkinspector-1.2.3.tar", max compression
```

## Comparing `apkinspector-1.2.2.tar` & `apkinspector-1.2.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    11357 2024-03-17 18:51:52.615383 apkinspector-1.2.2/LICENSE
--rw-r--r--   0        0        0     5522 2024-03-17 18:51:52.619383 apkinspector-1.2.2/README.md
--rw-r--r--   0        0        0       22 2024-03-17 18:51:52.619383 apkinspector-1.2.2/apkInspector/__init__.py
--rw-r--r--   0        0        0    28377 2024-03-17 18:51:52.619383 apkinspector-1.2.2/apkInspector/axml.py
--rw-r--r--   0        0        0     4965 2024-03-17 18:51:52.619383 apkinspector-1.2.2/apkInspector/extract.py
--rw-r--r--   0        0        0    27545 2024-03-17 18:51:52.619383 apkinspector-1.2.2/apkInspector/headers.py
--rw-r--r--   0        0        0     1717 2024-03-17 18:51:52.619383 apkinspector-1.2.2/apkInspector/helpers.py
--rw-r--r--   0        0        0     7135 2024-03-17 18:51:52.619383 apkinspector-1.2.2/apkInspector/indicators.py
--rw-r--r--   0        0        0        1 2024-03-17 18:51:52.619383 apkinspector-1.2.2/apkInspectorCLI/__init__.py
--rw-r--r--   0        0        0     8659 2024-03-17 18:51:52.619383 apkinspector-1.2.2/apkInspectorCLI/main.py
--rw-r--r--   0        0        0      675 2024-03-17 18:51:52.651383 apkinspector-1.2.2/pyproject.toml
--rw-r--r--   0        0        0     6536 1970-01-01 00:00:00.000000 apkinspector-1.2.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-20 01:47:12.264357 apkinspector-1.2.3/LICENSE
+-rw-r--r--   0        0        0     5522 2024-04-20 01:47:12.264357 apkinspector-1.2.3/README.md
+-rw-r--r--   0        0        0       22 2024-04-20 01:47:12.264357 apkinspector-1.2.3/apkInspector/__init__.py
+-rw-r--r--   0        0        0    28608 2024-04-20 01:47:12.264357 apkinspector-1.2.3/apkInspector/axml.py
+-rw-r--r--   0        0        0     5105 2024-04-20 01:47:12.264357 apkinspector-1.2.3/apkInspector/extract.py
+-rw-r--r--   0        0        0    27592 2024-04-20 01:47:12.264357 apkinspector-1.2.3/apkInspector/headers.py
+-rw-r--r--   0        0        0     1717 2024-04-20 01:47:12.264357 apkinspector-1.2.3/apkInspector/helpers.py
+-rw-r--r--   0        0        0     7135 2024-04-20 01:47:12.264357 apkinspector-1.2.3/apkInspector/indicators.py
+-rw-r--r--   0        0        0        1 2024-04-20 01:47:12.264357 apkinspector-1.2.3/apkInspectorCLI/__init__.py
+-rw-r--r--   0        0        0     8659 2024-04-20 01:47:12.264357 apkinspector-1.2.3/apkInspectorCLI/main.py
+-rw-r--r--   0        0        0      675 2024-04-20 01:47:12.300357 apkinspector-1.2.3/pyproject.toml
+-rw-r--r--   0        0        0     6536 1970-01-01 00:00:00.000000 apkinspector-1.2.3/PKG-INFO
```

### Comparing `apkinspector-1.2.2/LICENSE` & `apkinspector-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `apkinspector-1.2.2/README.md` & `apkinspector-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `apkinspector-1.2.2/apkInspector/axml.py` & `apkinspector-1.2.3/apkInspector/axml.py`

 * *Files 1% similar despite different names*

```diff
@@ -108,15 +108,15 @@
         # sanity check as after reading the last string we should be at the end offset as calculated
         if file.tell() != end_absolute_offset:
             logging.warning(
                 f"Current file read:{file.tell()} is not as expected to the start of the stringData:{end_absolute_offset})")
         return string_offsets
 
     @classmethod
-    def decode_stringpool_mixed_string(cls, file, is_utf8):
+    def decode_stringpool_mixed_string(cls, file, is_utf8, end_stringpool_offset):
         """
         Handling the different encoding possibilities that can be met.
 
         :param file: the xml file at the offset where the string is to be read
         :type file: bytesIO
         :param is_utf8: boolean to check if a utf8 string is expected
         :type is_utf8: bool
@@ -129,14 +129,17 @@
             if u16len & 0x8000 == 0:
                 # Regular UTF-16 string
                 content = file.read(u16len * 2).decode('utf-16le')
             else:
                 # UTF-16 string with fixup
                 u16len_fix = struct.unpack('<H', file.read(2))[0]
                 real_length = ((u16len & 0x7FFF) << 16) | u16len_fix
+                if real_length > end_stringpool_offset:
+                    return ""
+                # TODO:a check for non null-terminated strings should be here as well
                 content = file.read(real_length * 2).decode('utf-16le')
         else:
             # Handle UTF-8 encoded strings
             u16len = struct.unpack('B', file.read(1))[0]
             file.read(1)
             u8len = u16len
             content = file.read(u8len).decode('utf-8', errors='replace')
@@ -162,15 +165,15 @@
         strings = []
         for offset in string_offsets:
             # Calculate the absolute offset within the string data +8 for the file header
             absolute_offset = strings_start + offset + 8  # TODO: update this to get the file header size
             # Move the file pointer to the start of the string
             file.seek(absolute_offset)
             # Read the length of the string (in bytes)
-            content = cls.decode_stringpool_mixed_string(file, is_utf8)
+            content = cls.decode_stringpool_mixed_string(file, is_utf8, strings_start + string_offsets[-1])
             strings.append(content)
         return strings
 
     @classmethod
     def parse(cls, file):
         """
         Parse the string pool to acquire the strings used within the axml.
```

### Comparing `apkinspector-1.2.2/apkInspector/extract.py` & `apkinspector-1.2.3/apkInspector/extract.py`

 * *Files 3% similar despite different names*

```diff
@@ -76,17 +76,20 @@
         if os.path.exists(output_dir):
             print("Extraction aborted. Output directory already exists.")
             return 2
         # Create the output directory or overwrite if it already exists
         os.makedirs(output_dir, exist_ok=True)
         # Iterate over central directory entries
         for filename, cd_header_info in central_directory_entries.items():
+            if not filename:
+                # to account for the cases where an empty filename entry is added
+                continue
             # Extract the file using the local header information
             extracted_data = \
-            extract_file_based_on_header_info(apk_file, local_header_entries[filename], cd_header_info)[0]
+                extract_file_based_on_header_info(apk_file, local_header_entries[filename], cd_header_info)[0]
             # Construct the output file path
             output_path = os.path.join(output_dir, filename)
             # Create directories if necessary
             os.makedirs(os.path.dirname(output_path), exist_ok=True)
             # Write the extracted data to the output file
             with open(output_path, 'wb') as output_file:
                 output_file.write(extracted_data)
```

### Comparing `apkinspector-1.2.2/apkInspector/headers.py` & `apkinspector-1.2.3/apkInspector/headers.py`

 * *Files 1% similar despite different names*

```diff
@@ -328,17 +328,20 @@
             file_last_modification_time = struct.unpack('<H', apk_file.read(2))[0]
             file_last_modification_date = struct.unpack('<H', apk_file.read(2))[0]
             crc32_of_uncompressed_data = struct.unpack('<I', apk_file.read(4))[0]
             compressed_size = struct.unpack('<I', apk_file.read(4))[0]
             uncompressed_size = struct.unpack('<I', apk_file.read(4))[0]
             file_name_length = struct.unpack('<H', apk_file.read(2))[0]
             extra_field_length = struct.unpack('<H', apk_file.read(2))[0]
-            filename = struct.unpack(f'<{file_name_length}s', apk_file.read(file_name_length))[0].decode('utf-8')
-            extra_field = struct.unpack(f'<{extra_field_length}s', apk_file.read(extra_field_length))[0].decode('utf-8',
-                                                                                                                'ignore')
+            try:
+                filename = struct.unpack(f'<{file_name_length}s', apk_file.read(file_name_length))[0].decode('utf-8')
+                extra_field = struct.unpack(f'<{extra_field_length}s', apk_file.read(extra_field_length))[0].decode('utf-8', 'ignore')
+            except:
+                filename = entry_of_interest.filename
+                extra_field = entry_of_interest.extra_field
         return cls(
             version_needed_to_extract, general_purpose_bit_flag, compression_method,
             file_last_modification_time, file_last_modification_date, crc32_of_uncompressed_data,
             compressed_size, uncompressed_size, file_name_length, extra_field_length,
             filename, extra_field)
 
     def to_dict(self):
```

### Comparing `apkinspector-1.2.2/apkInspector/helpers.py` & `apkinspector-1.2.3/apkInspector/helpers.py`

 * *Files identical despite different names*

### Comparing `apkinspector-1.2.2/apkInspector/indicators.py` & `apkinspector-1.2.3/apkInspector/indicators.py`

 * *Files identical despite different names*

### Comparing `apkinspector-1.2.2/apkInspectorCLI/main.py` & `apkinspector-1.2.3/apkInspectorCLI/main.py`

 * *Files identical despite different names*

### Comparing `apkinspector-1.2.2/pyproject.toml` & `apkinspector-1.2.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "apkInspector"
-version = "1.2.2"
+version = "1.2.3"
 description = "apkInspector is a tool designed to provide detailed insights into the zip structure of APK files, offering the capability to extract content and decode the AndroidManifest.xml file."
 authors = ["erev0s <projects@erev0s.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 repository = "https://github.com/erev0s/apkInspector"
 
 packages = [
```

### Comparing `apkinspector-1.2.2/PKG-INFO` & `apkinspector-1.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apkInspector
-Version: 1.2.2
+Version: 1.2.3
 Summary: apkInspector is a tool designed to provide detailed insights into the zip structure of APK files, offering the capability to extract content and decode the AndroidManifest.xml file.
 Home-page: https://github.com/erev0s/apkInspector
 License: Apache-2.0
 Author: erev0s
 Author-email: projects@erev0s.com
 Requires-Python: >=3.5,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

