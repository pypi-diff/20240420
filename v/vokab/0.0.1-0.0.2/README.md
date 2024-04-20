# Comparing `tmp/vokab-0.0.1.tar.gz` & `tmp/vokab-0.0.2.tar.gz`

## Comparing `vokab-0.0.1.tar` & `vokab-0.0.2.tar`

### file list

```diff
@@ -1,70 +1,70 @@
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 vokab-0.0.1/CHANGELOG.md
--rw-r--r--   0        0        0     3366 2020-02-02 00:00:00.000000 vokab-0.0.1/LLM.md
--rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 vokab-0.0.1/Makefile
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 vokab-0.0.1/activate.sh
--rw-r--r--   0        0        0     5445 2020-02-02 00:00:00.000000 vokab-0.0.1/requirements-dev.txt
--rw-r--r--   0        0        0     3745 2020-02-02 00:00:00.000000 vokab-0.0.1/requirements.txt
--rw-r--r--   0        0        0     2310 2020-02-02 00:00:00.000000 vokab-0.0.1/ui.py
--rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 vokab-0.0.1/src/vokab/__init__.py
--rw-r--r--   0        0        0     2423 2020-02-02 00:00:00.000000 vokab-0.0.1/src/vokab/collection.py
--rw-r--r--   0        0        0     3360 2020-02-02 00:00:00.000000 vokab-0.0.1/src/vokab/config.py
--rw-r--r--   0        0        0     2337 2020-02-02 00:00:00.000000 vokab-0.0.1/src/vokab/const.py
--rw-r--r--   0        0        0     3160 2020-02-02 00:00:00.000000 vokab-0.0.1/src/vokab/entity.py
--rw-r--r--   0        0        0     3021 2020-02-02 00:00:00.000000 vokab-0.0.1/src/vokab/lazy.py
--rw-r--r--   0        0        0     3740 2020-02-02 00:00:00.000000 vokab-0.0.1/src/vokab/loader.py
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 vokab-0.0.1/src/vokab/logging.py
--rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 vokab-0.0.1/src/vokab/protocol.py
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 vokab-0.0.1/src/vokab/cli/__init__.py
--rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 vokab-0.0.1/src/vokab/cli/app.py
--rw-r--r--   0        0        0     1545 2020-02-02 00:00:00.000000 vokab-0.0.1/src/vokab/cli/eval.py
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 vokab-0.0.1/src/vokab/cli/init.py
--rw-r--r--   0        0        0     1869 2020-02-02 00:00:00.000000 vokab-0.0.1/src/vokab/cli/load.py
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 vokab-0.0.1/src/vokab/cli/reindex.py
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 vokab-0.0.1/src/vokab/databases/__init__.py
--rw-r--r--   0        0        0     2797 2020-02-02 00:00:00.000000 vokab-0.0.1/src/vokab/databases/abstract.py
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 vokab-0.0.1/src/vokab/databases/lancedb/__init__.py
--rw-r--r--   0        0        0     2039 2020-02-02 00:00:00.000000 vokab-0.0.1/src/vokab/databases/lancedb/database.py
--rw-r--r--   0        0        0     1424 2020-02-02 00:00:00.000000 vokab-0.0.1/src/vokab/databases/lancedb/entities.py
--rw-r--r--   0        0        0     1291 2020-02-02 00:00:00.000000 vokab-0.0.1/src/vokab/databases/lancedb/table.py
--rw-r--r--   0        0        0     4494 2020-02-02 00:00:00.000000 vokab-0.0.1/src/vokab/databases/lancedb/terms.py
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 vokab-0.0.1/src/vokab/databases/sqlite/__init__.py
--rw-r--r--   0        0        0     4195 2020-02-02 00:00:00.000000 vokab-0.0.1/src/vokab/databases/sqlite/database.py
--rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 vokab-0.0.1/src/vokab/databases/sqlite/sql/exact_search.sql
--rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 vokab-0.0.1/src/vokab/databases/sqlite/sql/fts_search.sql
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 vokab-0.0.1/src/vokab/databases/sqlite/sql/get_entity.sql
--rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 vokab-0.0.1/src/vokab/databases/sqlite/sql/init_tables.sql
--rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 vokab-0.0.1/src/vokab/databases/sqlite/sql/init_triggers.sql
--rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 vokab-0.0.1/src/vokab/databases/sqlite/sql/stats.sql
--rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 vokab-0.0.1/src/vokab/databases/sqlite/sql/upsert.sql
--rw-r--r--   0        0        0     1118 2020-02-02 00:00:00.000000 vokab-0.0.1/src/vokab/databases/sqlite/sql/vss_search.sql
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 vokab-0.0.1/src/vokab/encoders/__init__.py
--rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 vokab-0.0.1/src/vokab/encoders/abstract.py
--rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 vokab-0.0.1/src/vokab/encoders/sbert.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 vokab-0.0.1/src/vokab/fuzz/__init__.py
--rw-r--r--   0        0        0     2200 2020-02-02 00:00:00.000000 vokab-0.0.1/src/vokab/fuzz/abstract.py
--rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 vokab-0.0.1/src/vokab/fuzz/default.py
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 vokab-0.0.1/src/vokab/linkers/__init__.py
--rw-r--r--   0        0        0     3390 2020-02-02 00:00:00.000000 vokab-0.0.1/src/vokab/linkers/abstract.py
--rw-r--r--   0        0        0     1301 2020-02-02 00:00:00.000000 vokab-0.0.1/src/vokab/linkers/default.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 vokab-0.0.1/src/vokab/rerankers/__init__.py
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 vokab-0.0.1/src/vokab/rerankers/abstract.py
--rw-r--r--   0        0        0     1410 2020-02-02 00:00:00.000000 vokab-0.0.1/src/vokab/rerankers/rrf.py
--rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 vokab-0.0.1/tests/conftest.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vokab-0.0.1/tests/test_admin.py
--rw-r--r--   0        0        0     4540 2020-02-02 00:00:00.000000 vokab-0.0.1/tests/test_collection.py
--rw-r--r--   0        0        0     1240 2020-02-02 00:00:00.000000 vokab-0.0.1/tests/test_config.py
--rw-r--r--   0        0        0     3964 2020-02-02 00:00:00.000000 vokab-0.0.1/tests/test_database.py
--rw-r--r--   0        0        0     1373 2020-02-02 00:00:00.000000 vokab-0.0.1/tests/test_entity.py
--rw-r--r--   0        0        0     1281 2020-02-02 00:00:00.000000 vokab-0.0.1/tests/test_fuzz.py
--rw-r--r--   0        0        0     1340 2020-02-02 00:00:00.000000 vokab-0.0.1/tests/test_loader.py
--rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 vokab-0.0.1/tests/test_rerank.py
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 vokab-0.0.1/tests/data/emojis.csv
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 vokab-0.0.1/tests/data/emotions.txt
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 vokab-0.0.1/tests/data/mixed.jsonl
--rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 vokab-0.0.1/tests/data/myths.tsv
--rw-r--r--   0        0        0    17785 2020-02-02 00:00:00.000000 vokab-0.0.1/tests/data/simonw_tags.csv
--rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 vokab-0.0.1/.gitignore
--rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 vokab-0.0.1/LICENSE
--rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 vokab-0.0.1/README.md
--rw-r--r--   0        0        0     2314 2020-02-02 00:00:00.000000 vokab-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     2240 2020-02-02 00:00:00.000000 vokab-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 vokab-0.0.2/CHANGELOG.md
+-rw-r--r--   0        0        0     3366 2020-02-02 00:00:00.000000 vokab-0.0.2/LLM.md
+-rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 vokab-0.0.2/Makefile
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 vokab-0.0.2/activate.sh
+-rw-r--r--   0        0        0     5445 2020-02-02 00:00:00.000000 vokab-0.0.2/requirements-dev.txt
+-rw-r--r--   0        0        0     3745 2020-02-02 00:00:00.000000 vokab-0.0.2/requirements.txt
+-rw-r--r--   0        0        0     2310 2020-02-02 00:00:00.000000 vokab-0.0.2/ui.py
+-rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 vokab-0.0.2/src/vokab/__init__.py
+-rw-r--r--   0        0        0     2423 2020-02-02 00:00:00.000000 vokab-0.0.2/src/vokab/collection.py
+-rw-r--r--   0        0        0     3360 2020-02-02 00:00:00.000000 vokab-0.0.2/src/vokab/config.py
+-rw-r--r--   0        0        0     2337 2020-02-02 00:00:00.000000 vokab-0.0.2/src/vokab/const.py
+-rw-r--r--   0        0        0     3160 2020-02-02 00:00:00.000000 vokab-0.0.2/src/vokab/entity.py
+-rw-r--r--   0        0        0     3021 2020-02-02 00:00:00.000000 vokab-0.0.2/src/vokab/lazy.py
+-rw-r--r--   0        0        0     3740 2020-02-02 00:00:00.000000 vokab-0.0.2/src/vokab/loader.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 vokab-0.0.2/src/vokab/logging.py
+-rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 vokab-0.0.2/src/vokab/protocol.py
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 vokab-0.0.2/src/vokab/cli/__init__.py
+-rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 vokab-0.0.2/src/vokab/cli/app.py
+-rw-r--r--   0        0        0     1545 2020-02-02 00:00:00.000000 vokab-0.0.2/src/vokab/cli/eval.py
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 vokab-0.0.2/src/vokab/cli/init.py
+-rw-r--r--   0        0        0     1869 2020-02-02 00:00:00.000000 vokab-0.0.2/src/vokab/cli/load.py
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 vokab-0.0.2/src/vokab/cli/reindex.py
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 vokab-0.0.2/src/vokab/databases/__init__.py
+-rw-r--r--   0        0        0     2797 2020-02-02 00:00:00.000000 vokab-0.0.2/src/vokab/databases/abstract.py
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 vokab-0.0.2/src/vokab/databases/lancedb/__init__.py
+-rw-r--r--   0        0        0     2039 2020-02-02 00:00:00.000000 vokab-0.0.2/src/vokab/databases/lancedb/database.py
+-rw-r--r--   0        0        0     1424 2020-02-02 00:00:00.000000 vokab-0.0.2/src/vokab/databases/lancedb/entities.py
+-rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 vokab-0.0.2/src/vokab/databases/lancedb/table.py
+-rw-r--r--   0        0        0     4494 2020-02-02 00:00:00.000000 vokab-0.0.2/src/vokab/databases/lancedb/terms.py
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 vokab-0.0.2/src/vokab/databases/sqlite/__init__.py
+-rw-r--r--   0        0        0     4195 2020-02-02 00:00:00.000000 vokab-0.0.2/src/vokab/databases/sqlite/database.py
+-rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 vokab-0.0.2/src/vokab/databases/sqlite/sql/exact_search.sql
+-rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 vokab-0.0.2/src/vokab/databases/sqlite/sql/fts_search.sql
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 vokab-0.0.2/src/vokab/databases/sqlite/sql/get_entity.sql
+-rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 vokab-0.0.2/src/vokab/databases/sqlite/sql/init_tables.sql
+-rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 vokab-0.0.2/src/vokab/databases/sqlite/sql/init_triggers.sql
+-rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 vokab-0.0.2/src/vokab/databases/sqlite/sql/stats.sql
+-rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 vokab-0.0.2/src/vokab/databases/sqlite/sql/upsert.sql
+-rw-r--r--   0        0        0     1118 2020-02-02 00:00:00.000000 vokab-0.0.2/src/vokab/databases/sqlite/sql/vss_search.sql
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 vokab-0.0.2/src/vokab/encoders/__init__.py
+-rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 vokab-0.0.2/src/vokab/encoders/abstract.py
+-rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 vokab-0.0.2/src/vokab/encoders/sbert.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 vokab-0.0.2/src/vokab/fuzz/__init__.py
+-rw-r--r--   0        0        0     2200 2020-02-02 00:00:00.000000 vokab-0.0.2/src/vokab/fuzz/abstract.py
+-rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 vokab-0.0.2/src/vokab/fuzz/default.py
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 vokab-0.0.2/src/vokab/linkers/__init__.py
+-rw-r--r--   0        0        0     3390 2020-02-02 00:00:00.000000 vokab-0.0.2/src/vokab/linkers/abstract.py
+-rw-r--r--   0        0        0     1301 2020-02-02 00:00:00.000000 vokab-0.0.2/src/vokab/linkers/default.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 vokab-0.0.2/src/vokab/rerankers/__init__.py
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 vokab-0.0.2/src/vokab/rerankers/abstract.py
+-rw-r--r--   0        0        0     1410 2020-02-02 00:00:00.000000 vokab-0.0.2/src/vokab/rerankers/rrf.py
+-rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 vokab-0.0.2/tests/conftest.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vokab-0.0.2/tests/test_admin.py
+-rw-r--r--   0        0        0     4540 2020-02-02 00:00:00.000000 vokab-0.0.2/tests/test_collection.py
+-rw-r--r--   0        0        0     1240 2020-02-02 00:00:00.000000 vokab-0.0.2/tests/test_config.py
+-rw-r--r--   0        0        0     3964 2020-02-02 00:00:00.000000 vokab-0.0.2/tests/test_database.py
+-rw-r--r--   0        0        0     1373 2020-02-02 00:00:00.000000 vokab-0.0.2/tests/test_entity.py
+-rw-r--r--   0        0        0     1281 2020-02-02 00:00:00.000000 vokab-0.0.2/tests/test_fuzz.py
+-rw-r--r--   0        0        0     1340 2020-02-02 00:00:00.000000 vokab-0.0.2/tests/test_loader.py
+-rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 vokab-0.0.2/tests/test_rerank.py
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 vokab-0.0.2/tests/data/emojis.csv
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 vokab-0.0.2/tests/data/emotions.txt
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 vokab-0.0.2/tests/data/mixed.jsonl
+-rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 vokab-0.0.2/tests/data/myths.tsv
+-rw-r--r--   0        0        0    17785 2020-02-02 00:00:00.000000 vokab-0.0.2/tests/data/simonw_tags.csv
+-rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 vokab-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 vokab-0.0.2/LICENSE
+-rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 vokab-0.0.2/README.md
+-rw-r--r--   0        0        0     2367 2020-02-02 00:00:00.000000 vokab-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2256 2020-02-02 00:00:00.000000 vokab-0.0.2/PKG-INFO
```

### Comparing `vokab-0.0.1/LLM.md` & `vokab-0.0.2/LLM.md`

 * *Files identical despite different names*

### Comparing `vokab-0.0.1/Makefile` & `vokab-0.0.2/Makefile`

 * *Files identical despite different names*

### Comparing `vokab-0.0.1/requirements-dev.txt` & `vokab-0.0.2/requirements-dev.txt`

 * *Files identical despite different names*

### Comparing `vokab-0.0.1/requirements.txt` & `vokab-0.0.2/requirements.txt`

 * *Files identical despite different names*

### Comparing `vokab-0.0.1/ui.py` & `vokab-0.0.2/ui.py`

 * *Files identical despite different names*

### Comparing `vokab-0.0.1/src/vokab/__init__.py` & `vokab-0.0.2/src/vokab/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.0.1"
+__version__ = "0.0.2"
 
 from .logging import logger
 from . import lazy
 from . import const
 from .const import Confidence, Dicts, Labels, Limit, Strs, Vec
 from .entity import (
     Entity,
```

### Comparing `vokab-0.0.1/src/vokab/collection.py` & `vokab-0.0.2/src/vokab/collection.py`

 * *Files identical despite different names*

### Comparing `vokab-0.0.1/src/vokab/config.py` & `vokab-0.0.2/src/vokab/config.py`

 * *Files identical despite different names*

### Comparing `vokab-0.0.1/src/vokab/const.py` & `vokab-0.0.2/src/vokab/const.py`

 * *Files identical despite different names*

### Comparing `vokab-0.0.1/src/vokab/entity.py` & `vokab-0.0.2/src/vokab/entity.py`

 * *Files identical despite different names*

### Comparing `vokab-0.0.1/src/vokab/lazy.py` & `vokab-0.0.2/src/vokab/lazy.py`

 * *Files identical despite different names*

### Comparing `vokab-0.0.1/src/vokab/loader.py` & `vokab-0.0.2/src/vokab/loader.py`

 * *Files identical despite different names*

### Comparing `vokab-0.0.1/src/vokab/protocol.py` & `vokab-0.0.2/src/vokab/protocol.py`

 * *Files identical despite different names*

### Comparing `vokab-0.0.1/src/vokab/cli/app.py` & `vokab-0.0.2/src/vokab/cli/app.py`

 * *Files identical despite different names*

### Comparing `vokab-0.0.1/src/vokab/cli/eval.py` & `vokab-0.0.2/src/vokab/cli/eval.py`

 * *Files identical despite different names*

### Comparing `vokab-0.0.1/src/vokab/cli/load.py` & `vokab-0.0.2/src/vokab/cli/load.py`

 * *Files identical despite different names*

### Comparing `vokab-0.0.1/src/vokab/databases/abstract.py` & `vokab-0.0.2/src/vokab/databases/abstract.py`

 * *Files identical despite different names*

### Comparing `vokab-0.0.1/src/vokab/databases/lancedb/database.py` & `vokab-0.0.2/src/vokab/databases/lancedb/database.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 import os.path
 from typing import List, Optional
 
-from lancedb import LanceDBConnection, connect
 
-from vokab import Entity, Labels, Limit, Results, Strs, Vec, Entities
+from vokab import Entity, Labels, Limit, Results, Strs, Vec, Entities, lazy
 from . import EntitiesTable, TermsTable
 from .. import AbstractDatabase
 
 
 class LanceDBDatabase(AbstractDatabase):
     name = "lancedb"
 
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
         self._conn = None
         self._terms = None
         self._entities = None
 
     @property
-    def conn(self) -> LanceDBConnection:
+    def conn(self):
         if self._conn is None:
             db_url = self.config.database.url or "db"
             if not os.path.isabs(db_url):
                 db_url = str(self.collection.path / db_url)
+
+            connect = lazy.lazy_import("lancedb", "connect")
             self._conn = connect(uri=db_url)
         return self._conn
 
     @property
     def entities(self) -> EntitiesTable:
         if self._entities is None:
             self._entities = EntitiesTable.connect(self, self.conn)
```

### Comparing `vokab-0.0.1/src/vokab/databases/lancedb/entities.py` & `vokab-0.0.2/src/vokab/databases/lancedb/entities.py`

 * *Files identical despite different names*

### Comparing `vokab-0.0.1/src/vokab/databases/lancedb/table.py` & `vokab-0.0.2/src/vokab/databases/lancedb/table.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 from abc import abstractmethod
 from typing import ClassVar, List
 
 import pyarrow as pa
-from lancedb import LanceDBConnection
-from lancedb.table import LanceTable
 
 from vokab import Dicts, Entity
 from .. import AbstractDatabase
 
 
 class Table:
     name: ClassVar = None
 
-    def __init__(self, database: AbstractDatabase, table: LanceTable):
+    def __init__(self, database: AbstractDatabase, table):
         self.database = database
         self.table = table
 
     def add(self, data: Dicts):
         self.table.add(data)
 
     def count(self) -> int:
@@ -30,18 +28,18 @@
         pass
 
     @classmethod
     def columns(cls, database: AbstractDatabase) -> List[pa.Field]:
         raise NotImplementedError
 
     @classmethod
-    def connect(cls, database: AbstractDatabase, conn: LanceDBConnection):
+    def connect(cls, database: AbstractDatabase, conn):
         if cls.name not in conn.table_names():
             table = cls.construct(database, conn)
         else:
             table = conn.open_table(cls.name)
         return cls(database=database, table=table)
 
     @classmethod
-    def construct(cls, database: AbstractDatabase, conn: LanceDBConnection):
+    def construct(cls, database: AbstractDatabase, conn):
         schema = pa.schema(cls.columns(database))
         return conn.create_table(name=cls.name, schema=schema, exist_ok=True)
```

### Comparing `vokab-0.0.1/src/vokab/databases/lancedb/terms.py` & `vokab-0.0.2/src/vokab/databases/lancedb/terms.py`

 * *Files identical despite different names*

### Comparing `vokab-0.0.1/src/vokab/databases/sqlite/database.py` & `vokab-0.0.2/src/vokab/databases/sqlite/database.py`

 * *Files identical despite different names*

### Comparing `vokab-0.0.1/src/vokab/databases/sqlite/sql/fts_search.sql` & `vokab-0.0.2/src/vokab/databases/sqlite/sql/fts_search.sql`

 * *Files identical despite different names*

### Comparing `vokab-0.0.1/src/vokab/databases/sqlite/sql/init_tables.sql` & `vokab-0.0.2/src/vokab/databases/sqlite/sql/init_tables.sql`

 * *Files identical despite different names*

### Comparing `vokab-0.0.1/src/vokab/databases/sqlite/sql/init_triggers.sql` & `vokab-0.0.2/src/vokab/databases/sqlite/sql/init_triggers.sql`

 * *Files identical despite different names*

### Comparing `vokab-0.0.1/src/vokab/databases/sqlite/sql/vss_search.sql` & `vokab-0.0.2/src/vokab/databases/sqlite/sql/vss_search.sql`

 * *Files identical despite different names*

### Comparing `vokab-0.0.1/src/vokab/encoders/abstract.py` & `vokab-0.0.2/src/vokab/encoders/abstract.py`

 * *Files identical despite different names*

### Comparing `vokab-0.0.1/src/vokab/encoders/sbert.py` & `vokab-0.0.2/src/vokab/encoders/sbert.py`

 * *Files identical despite different names*

### Comparing `vokab-0.0.1/src/vokab/fuzz/abstract.py` & `vokab-0.0.2/src/vokab/fuzz/abstract.py`

 * *Files identical despite different names*

### Comparing `vokab-0.0.1/src/vokab/fuzz/default.py` & `vokab-0.0.2/src/vokab/fuzz/default.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List, Tuple
 
-from rapidfuzz import fuzz
+from rapidfuzz import fuzz, utils
 from rapidfuzz.process import extract
 
 from vokab import Strs
 from . import AbstractFuzz
 
 
 class DefaultFuzz(AbstractFuzz):
@@ -18,13 +18,14 @@
         matches = []
 
         results = extract(
             query=term,
             choices=choices,
             scorer=self.scorer,
             limit=limit,
+            processor=utils.default_process,
         )
 
         for text, score, index in results:
             matches.append((100 - score, index))
 
         return matches
```

### Comparing `vokab-0.0.1/src/vokab/linkers/abstract.py` & `vokab-0.0.2/src/vokab/linkers/abstract.py`

 * *Files identical despite different names*

### Comparing `vokab-0.0.1/src/vokab/linkers/default.py` & `vokab-0.0.2/src/vokab/linkers/default.py`

 * *Files identical despite different names*

### Comparing `vokab-0.0.1/src/vokab/rerankers/abstract.py` & `vokab-0.0.2/src/vokab/rerankers/abstract.py`

 * *Files identical despite different names*

### Comparing `vokab-0.0.1/src/vokab/rerankers/rrf.py` & `vokab-0.0.2/src/vokab/rerankers/rrf.py`

 * *Files identical despite different names*

### Comparing `vokab-0.0.1/tests/conftest.py` & `vokab-0.0.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `vokab-0.0.1/tests/test_collection.py` & `vokab-0.0.2/tests/test_collection.py`

 * *Files identical despite different names*

### Comparing `vokab-0.0.1/tests/test_config.py` & `vokab-0.0.2/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `vokab-0.0.1/tests/test_database.py` & `vokab-0.0.2/tests/test_database.py`

 * *Files identical despite different names*

### Comparing `vokab-0.0.1/tests/test_entity.py` & `vokab-0.0.2/tests/test_entity.py`

 * *Files identical despite different names*

### Comparing `vokab-0.0.1/tests/test_fuzz.py` & `vokab-0.0.2/tests/test_fuzz.py`

 * *Files identical despite different names*

### Comparing `vokab-0.0.1/tests/test_loader.py` & `vokab-0.0.2/tests/test_loader.py`

 * *Files identical despite different names*

### Comparing `vokab-0.0.1/tests/test_rerank.py` & `vokab-0.0.2/tests/test_rerank.py`

 * *Files identical despite different names*

### Comparing `vokab-0.0.1/tests/data/myths.tsv` & `vokab-0.0.2/tests/data/myths.tsv`

 * *Files identical despite different names*

### Comparing `vokab-0.0.1/tests/data/simonw_tags.csv` & `vokab-0.0.2/tests/data/simonw_tags.csv`

 * *Files identical despite different names*

### Comparing `vokab-0.0.1/LICENSE` & `vokab-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `vokab-0.0.1/README.md` & `vokab-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `vokab-0.0.1/pyproject.toml` & `vokab-0.0.2/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -14,15 +14,14 @@
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3",
     "Topic :: Software Development :: Libraries",
 ]
 dependencies = [
-    "aiosql >= 10.1",
     "click >= 8.0.0",
     "pydantic >= 2.6.1",
     "rapidfuzz >= 3.7.0",
     "sentence-transformers >= 2.2.2",
     "streamlit >= 1.33.0",
     "torch >= 2.2.2",
     "tqdm",
@@ -39,15 +38,18 @@
     "build",
     "ipython",
     "pip",
     "setuptools",
     "twine",
 ]
 ext = [
+    # backend: sqlite (+ vss)
+    "aiosql >= 10.1",
     "sqlite-vss",
+    # backend: lancedb
     "lancedb",
     "tantivy",
 ]
 
 [tool.setuptools.package-data]
 
 [project.urls]
```

### Comparing `vokab-0.0.1/PKG-INFO` & `vokab-0.0.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.3
 Name: vokab
-Version: 0.0.1
+Version: 0.0.2
 Summary: vokab: named entity linking through hybrid (lexical and semantic) search engine.
 Author-email: Ian Maurer <ian@genomoncology.com>
 License-File: LICENSE
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.9
-Requires-Dist: aiosql>=10.1
 Requires-Dist: click>=8.0.0
 Requires-Dist: pydantic>=2.6.1
 Requires-Dist: rapidfuzz>=3.7.0
 Requires-Dist: sentence-transformers>=2.2.2
 Requires-Dist: streamlit>=1.33.0
 Requires-Dist: torch>=2.2.2
 Requires-Dist: tqdm
 Provides-Extra: ext
+Requires-Dist: aiosql>=10.1; extra == 'ext'
 Requires-Dist: lancedb; extra == 'ext'
 Requires-Dist: sqlite-vss; extra == 'ext'
 Requires-Dist: tantivy; extra == 'ext'
 Provides-Extra: local
 Requires-Dist: build; extra == 'local'
 Requires-Dist: ipython; extra == 'local'
 Requires-Dist: pip; extra == 'local'
```

