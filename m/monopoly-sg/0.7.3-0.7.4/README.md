# Comparing `tmp/monopoly_sg-0.7.3.tar.gz` & `tmp/monopoly_sg-0.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "monopoly_sg-0.7.3.tar", max compression
+gzip compressed data, was "monopoly_sg-0.7.4.tar", max compression
```

## Comparing `monopoly_sg-0.7.3.tar` & `monopoly_sg-0.7.4.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0     1072 2023-11-25 08:00:21.000000 monopoly_sg-0.7.3/LICENSE.md
--rw-r--r--   0        0        0     2624 2023-12-27 07:15:14.515773 monopoly_sg-0.7.3/README.md
--rw-r--r--   0        0        0     2053 2024-04-19 14:21:07.835415 monopoly_sg-0.7.3/pyproject.toml
--rw-r--r--   0        0        0       59 2023-11-25 08:00:21.000000 monopoly_sg-0.7.3/src/monopoly/__init__.py
--rw-r--r--   0        0        0     8005 2024-02-11 14:35:16.392192 monopoly_sg-0.7.3/src/monopoly/cli.py
--rw-r--r--   0        0        0     3389 2024-01-14 10:44:28.918012 monopoly_sg-0.7.3/src/monopoly/config.py
--rw-r--r--   0        0        0     4005 2024-01-14 09:33:42.855330 monopoly_sg-0.7.3/src/monopoly/constants.py
--rw-r--r--   0        0        0   299608 2023-12-28 09:49:25.899409 monopoly_sg-0.7.3/src/monopoly/examples/example_statement.pdf
--rw-r--r--   0        0        0      620 2023-12-01 13:26:34.000000 monopoly_sg-0.7.3/src/monopoly/examples/multiple_statements.py
--rw-r--r--   0        0        0      742 2023-12-02 13:07:54.000000 monopoly_sg-0.7.3/src/monopoly/examples/single_statement.py
--rw-r--r--   0        0        0      491 2024-01-01 12:59:34.183692 monopoly_sg-0.7.3/src/monopoly/log.py
--rw-r--r--   0        0        0     4585 2024-01-14 07:52:30.958784 monopoly_sg-0.7.3/src/monopoly/pdf.py
--rw-r--r--   0        0        0     3804 2024-04-05 13:52:17.787640 monopoly_sg-0.7.3/src/monopoly/processor.py
--rw-r--r--   0        0        0     2548 2023-12-28 15:35:17.896832 monopoly_sg-0.7.3/src/monopoly/processors/__init__.py
--rw-r--r--   0        0        0     3964 2024-01-14 09:33:55.555328 monopoly_sg-0.7.3/src/monopoly/processors/base.py
--rw-r--r--   0        0        0       55 2023-12-01 13:26:34.000000 monopoly_sg-0.7.3/src/monopoly/processors/citibank/__init__.py
--rw-r--r--   0        0        0     1020 2024-01-14 07:44:48.150290 monopoly_sg-0.7.3/src/monopoly/processors/citibank/citibank.py
--rw-r--r--   0        0        0       40 2023-12-01 13:26:34.000000 monopoly_sg-0.7.3/src/monopoly/processors/dbs/__init__.py
--rw-r--r--   0        0        0     1365 2024-04-19 14:20:45.535418 monopoly_sg-0.7.3/src/monopoly/processors/dbs/dbs.py
--rw-r--r--   0        0        0      964 2024-04-19 14:21:07.835415 monopoly_sg-0.7.3/src/monopoly/processors/example_bank.py
--rw-r--r--   0        0        0       43 2023-12-01 13:26:34.000000 monopoly_sg-0.7.3/src/monopoly/processors/hsbc/__init__.py
--rw-r--r--   0        0        0     1158 2024-01-11 15:47:10.530736 monopoly_sg-0.7.3/src/monopoly/processors/hsbc/hsbc.py
--rw-r--r--   0        0        0       43 2023-12-01 13:26:34.000000 monopoly_sg-0.7.3/src/monopoly/processors/ocbc/__init__.py
--rw-r--r--   0        0        0     1506 2024-04-19 14:18:09.005435 monopoly_sg-0.7.3/src/monopoly/processors/ocbc/ocbc.py
--rw-r--r--   0        0        0       83 2023-12-01 13:26:34.000000 monopoly_sg-0.7.3/src/monopoly/processors/standard_chartered/__init__.py
--rw-r--r--   0        0        0     1007 2024-01-12 14:33:27.070256 monopoly_sg-0.7.3/src/monopoly/processors/standard_chartered/standard_chartered.py
--rw-r--r--   0        0        0      216 2023-12-28 15:35:17.896832 monopoly_sg-0.7.3/src/monopoly/statements/__init__.py
--rw-r--r--   0        0        0     7669 2024-04-19 14:24:09.875401 monopoly_sg-0.7.3/src/monopoly/statements/base.py
--rw-r--r--   0        0        0     3105 2024-02-11 14:35:16.392192 monopoly_sg-0.7.3/src/monopoly/statements/credit_statement.py
--rw-r--r--   0        0        0     4278 2024-02-11 14:35:16.392192 monopoly_sg-0.7.3/src/monopoly/statements/debit_statement.py
--rw-r--r--   0        0        0     1521 2024-04-19 14:24:09.875401 monopoly_sg-0.7.3/src/monopoly/write.py
--rw-r--r--   0        0        0       69 2023-11-25 10:08:54.000000 monopoly_sg-0.7.3/tests/test_utils/__init__.py
--rw-r--r--   0        0        0      790 2023-11-25 10:08:54.000000 monopoly_sg-0.7.3/tests/test_utils/skip.py
--rw-r--r--   0        0        0     3589 1970-01-01 00:00:00.000000 monopoly_sg-0.7.3/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-11-25 08:00:21.000000 monopoly_sg-0.7.4/LICENSE.md
+-rw-r--r--   0        0        0     2624 2023-12-27 07:15:14.515773 monopoly_sg-0.7.4/README.md
+-rw-r--r--   0        0        0     2053 2024-04-19 16:19:42.384741 monopoly_sg-0.7.4/pyproject.toml
+-rw-r--r--   0        0        0       59 2023-11-25 08:00:21.000000 monopoly_sg-0.7.4/src/monopoly/__init__.py
+-rw-r--r--   0        0        0     8005 2024-02-11 14:35:16.392192 monopoly_sg-0.7.4/src/monopoly/cli.py
+-rw-r--r--   0        0        0     3389 2024-01-14 10:44:28.918012 monopoly_sg-0.7.4/src/monopoly/config.py
+-rw-r--r--   0        0        0     4005 2024-01-14 09:33:42.855330 monopoly_sg-0.7.4/src/monopoly/constants.py
+-rw-r--r--   0        0        0   299608 2023-12-28 09:49:25.899409 monopoly_sg-0.7.4/src/monopoly/examples/example_statement.pdf
+-rw-r--r--   0        0        0      620 2023-12-01 13:26:34.000000 monopoly_sg-0.7.4/src/monopoly/examples/multiple_statements.py
+-rw-r--r--   0        0        0      742 2023-12-02 13:07:54.000000 monopoly_sg-0.7.4/src/monopoly/examples/single_statement.py
+-rw-r--r--   0        0        0      491 2024-01-01 12:59:34.183692 monopoly_sg-0.7.4/src/monopoly/log.py
+-rw-r--r--   0        0        0     4585 2024-01-14 07:52:30.958784 monopoly_sg-0.7.4/src/monopoly/pdf.py
+-rw-r--r--   0        0        0     3804 2024-04-05 13:52:17.787640 monopoly_sg-0.7.4/src/monopoly/processor.py
+-rw-r--r--   0        0        0     2743 2024-04-19 16:19:42.384741 monopoly_sg-0.7.4/src/monopoly/processors/__init__.py
+-rw-r--r--   0        0        0     3964 2024-01-14 09:33:55.555328 monopoly_sg-0.7.4/src/monopoly/processors/base.py
+-rw-r--r--   0        0        0       55 2023-12-01 13:26:34.000000 monopoly_sg-0.7.4/src/monopoly/processors/citibank/__init__.py
+-rw-r--r--   0        0        0     1020 2024-01-14 07:44:48.150290 monopoly_sg-0.7.4/src/monopoly/processors/citibank/citibank.py
+-rw-r--r--   0        0        0       40 2023-12-01 13:26:34.000000 monopoly_sg-0.7.4/src/monopoly/processors/dbs/__init__.py
+-rw-r--r--   0        0        0     1365 2024-04-19 14:20:45.535418 monopoly_sg-0.7.4/src/monopoly/processors/dbs/dbs.py
+-rw-r--r--   0        0        0      964 2024-04-19 14:21:07.835415 monopoly_sg-0.7.4/src/monopoly/processors/example_bank.py
+-rw-r--r--   0        0        0       43 2023-12-01 13:26:34.000000 monopoly_sg-0.7.4/src/monopoly/processors/hsbc/__init__.py
+-rw-r--r--   0        0        0     1158 2024-01-11 15:47:10.530736 monopoly_sg-0.7.4/src/monopoly/processors/hsbc/hsbc.py
+-rw-r--r--   0        0        0       43 2023-12-01 13:26:34.000000 monopoly_sg-0.7.4/src/monopoly/processors/ocbc/__init__.py
+-rw-r--r--   0        0        0     1506 2024-04-19 14:18:09.005435 monopoly_sg-0.7.4/src/monopoly/processors/ocbc/ocbc.py
+-rw-r--r--   0        0        0       83 2023-12-01 13:26:34.000000 monopoly_sg-0.7.4/src/monopoly/processors/standard_chartered/__init__.py
+-rw-r--r--   0        0        0     1007 2024-01-12 14:33:27.070256 monopoly_sg-0.7.4/src/monopoly/processors/standard_chartered/standard_chartered.py
+-rw-r--r--   0        0        0      216 2023-12-28 15:35:17.896832 monopoly_sg-0.7.4/src/monopoly/statements/__init__.py
+-rw-r--r--   0        0        0     7669 2024-04-19 14:24:09.875401 monopoly_sg-0.7.4/src/monopoly/statements/base.py
+-rw-r--r--   0        0        0     3105 2024-02-11 14:35:16.392192 monopoly_sg-0.7.4/src/monopoly/statements/credit_statement.py
+-rw-r--r--   0        0        0     4278 2024-02-11 14:35:16.392192 monopoly_sg-0.7.4/src/monopoly/statements/debit_statement.py
+-rw-r--r--   0        0        0     1521 2024-04-19 14:24:09.875401 monopoly_sg-0.7.4/src/monopoly/write.py
+-rw-r--r--   0        0        0       69 2023-11-25 10:08:54.000000 monopoly_sg-0.7.4/tests/test_utils/__init__.py
+-rw-r--r--   0        0        0      790 2023-11-25 10:08:54.000000 monopoly_sg-0.7.4/tests/test_utils/skip.py
+-rw-r--r--   0        0        0     3589 1970-01-01 00:00:00.000000 monopoly_sg-0.7.4/PKG-INFO
```

### Comparing `monopoly_sg-0.7.3/LICENSE.md` & `monopoly_sg-0.7.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `monopoly_sg-0.7.3/README.md` & `monopoly_sg-0.7.4/README.md`

 * *Files identical despite different names*

### Comparing `monopoly_sg-0.7.3/pyproject.toml` & `monopoly_sg-0.7.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "monopoly-sg"
-version = "0.7.3"
+version = "0.7.4"
 description = "PDF parsing for Singaporean banks"
 repository = "https://github.com/benjamin-awd/monopoly"
 authors = ["benjamin-awd <benjamindornel@gmail.com>"]
 packages = [
     { include = "monopoly", from = "src" },
     { include = "test_utils", from = "tests" }
 ]
```

### Comparing `monopoly_sg-0.7.3/src/monopoly/cli.py` & `monopoly_sg-0.7.4/src/monopoly/cli.py`

 * *Files identical despite different names*

### Comparing `monopoly_sg-0.7.3/src/monopoly/config.py` & `monopoly_sg-0.7.4/src/monopoly/config.py`

 * *Files identical despite different names*

### Comparing `monopoly_sg-0.7.3/src/monopoly/constants.py` & `monopoly_sg-0.7.4/src/monopoly/constants.py`

 * *Files identical despite different names*

### Comparing `monopoly_sg-0.7.3/src/monopoly/examples/example_statement.pdf` & `monopoly_sg-0.7.4/src/monopoly/examples/example_statement.pdf`

 * *Files identical despite different names*

### Comparing `monopoly_sg-0.7.3/src/monopoly/examples/multiple_statements.py` & `monopoly_sg-0.7.4/src/monopoly/examples/multiple_statements.py`

 * *Files identical despite different names*

### Comparing `monopoly_sg-0.7.3/src/monopoly/examples/single_statement.py` & `monopoly_sg-0.7.4/src/monopoly/examples/single_statement.py`

 * *Files identical despite different names*

### Comparing `monopoly_sg-0.7.3/src/monopoly/pdf.py` & `monopoly_sg-0.7.4/src/monopoly/pdf.py`

 * *Files identical despite different names*

### Comparing `monopoly_sg-0.7.3/src/monopoly/processor.py` & `monopoly_sg-0.7.4/src/monopoly/processor.py`

 * *Files identical despite different names*

### Comparing `monopoly_sg-0.7.3/src/monopoly/processors/__init__.py` & `monopoly_sg-0.7.4/src/monopoly/processors/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 import logging
 from dataclasses import Field, fields
 from itertools import product
 from pathlib import Path
-from typing import Type
+from typing import Optional, Type
 
+from pydantic import SecretStr
+
+from monopoly.config import PdfConfig
 from monopoly.constants import EncryptionIdentifier, MetadataIdentifier
 from monopoly.pdf import PdfParser
 
 from .base import ProcessorBase
 from .citibank import Citibank
 from .dbs import Dbs
 from .example_bank import ExampleBankProcessor
@@ -24,24 +27,26 @@
     StandardChartered,
 ]
 
 
 logger = logging.getLogger(__name__)
 
 
-def detect_processor(file_path: Path) -> ProcessorBase:
+def detect_processor(
+    file_path: Path, passwords: Optional[list[SecretStr]] = None
+) -> ProcessorBase:
     """
     Reads the encryption metadata or actual metadata (if the PDF is not encrypted),
     and checks for a bank based on unique identifiers.
     """
-    parser = PdfParser(file_path)
+    parser = PdfParser(file_path, pdf_config=PdfConfig(passwords=passwords))
     for processor in processors:
         metadata_items = processor.get_identifiers(parser)
         if is_bank_identified(metadata_items, processor):
-            return processor(file_path=file_path)
+            return processor(file_path=file_path, passwords=passwords)
 
     raise ValueError(f"Could not find a bank for {parser.file_path}")
 
 
 def is_bank_identified(
     metadata_items: list[EncryptionIdentifier | MetadataIdentifier],
     processor: Type[ProcessorBase],
```

### Comparing `monopoly_sg-0.7.3/src/monopoly/processors/base.py` & `monopoly_sg-0.7.4/src/monopoly/processors/base.py`

 * *Files identical despite different names*

### Comparing `monopoly_sg-0.7.3/src/monopoly/processors/citibank/citibank.py` & `monopoly_sg-0.7.4/src/monopoly/processors/citibank/citibank.py`

 * *Files identical despite different names*

### Comparing `monopoly_sg-0.7.3/src/monopoly/processors/dbs/dbs.py` & `monopoly_sg-0.7.4/src/monopoly/processors/dbs/dbs.py`

 * *Files identical despite different names*

### Comparing `monopoly_sg-0.7.3/src/monopoly/processors/example_bank.py` & `monopoly_sg-0.7.4/src/monopoly/processors/example_bank.py`

 * *Files identical despite different names*

### Comparing `monopoly_sg-0.7.3/src/monopoly/processors/hsbc/hsbc.py` & `monopoly_sg-0.7.4/src/monopoly/processors/hsbc/hsbc.py`

 * *Files identical despite different names*

### Comparing `monopoly_sg-0.7.3/src/monopoly/processors/ocbc/ocbc.py` & `monopoly_sg-0.7.4/src/monopoly/processors/ocbc/ocbc.py`

 * *Files identical despite different names*

### Comparing `monopoly_sg-0.7.3/src/monopoly/processors/standard_chartered/standard_chartered.py` & `monopoly_sg-0.7.4/src/monopoly/processors/standard_chartered/standard_chartered.py`

 * *Files identical despite different names*

### Comparing `monopoly_sg-0.7.3/src/monopoly/statements/base.py` & `monopoly_sg-0.7.4/src/monopoly/statements/base.py`

 * *Files identical despite different names*

### Comparing `monopoly_sg-0.7.3/src/monopoly/statements/credit_statement.py` & `monopoly_sg-0.7.4/src/monopoly/statements/credit_statement.py`

 * *Files identical despite different names*

### Comparing `monopoly_sg-0.7.3/src/monopoly/statements/debit_statement.py` & `monopoly_sg-0.7.4/src/monopoly/statements/debit_statement.py`

 * *Files identical despite different names*

### Comparing `monopoly_sg-0.7.3/src/monopoly/write.py` & `monopoly_sg-0.7.4/src/monopoly/write.py`

 * *Files identical despite different names*

### Comparing `monopoly_sg-0.7.3/tests/test_utils/skip.py` & `monopoly_sg-0.7.4/tests/test_utils/skip.py`

 * *Files identical despite different names*

### Comparing `monopoly_sg-0.7.3/PKG-INFO` & `monopoly_sg-0.7.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monopoly-sg
-Version: 0.7.3
+Version: 0.7.4
 Summary: PDF parsing for Singaporean banks
 Home-page: https://github.com/benjamin-awd/monopoly
 License: MIT
 Author: benjamin-awd
 Author-email: benjamindornel@gmail.com
 Requires-Python: >=3.11,<3.12
 Classifier: Development Status :: 3 - Alpha
```

