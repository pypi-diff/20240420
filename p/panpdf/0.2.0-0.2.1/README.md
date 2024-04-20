# Comparing `tmp/panpdf-0.2.0.tar.gz` & `tmp/panpdf-0.2.1.tar.gz`

## Comparing `panpdf-0.2.0.tar` & `panpdf-0.2.1.tar`

### file list

```diff
@@ -1,69 +1,70 @@
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 panpdf-0.2.0/.gitattributes
--rw-r--r--   0        0        0    51052 2020-02-02 00:00:00.000000 panpdf-0.2.0/a.tex
--rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 panpdf-0.2.0/mkdocs.yml
--rw-r--r--   0        0        0     6064 2020-02-02 00:00:00.000000 panpdf-0.2.0/ruff_defaults.toml
--rw-r--r--   0        0        0      955 2020-02-02 00:00:00.000000 panpdf-0.2.0/.devcontainer/devcontainer.json
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 panpdf-0.2.0/.devcontainer/postCreate.sh
--rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 panpdf-0.2.0/.devcontainer/starship.toml
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 panpdf-0.2.0/.devcontainer/features/zotero/devcontainer-feature.json
--rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 panpdf-0.2.0/.devcontainer/features/zotero/install.sh
--rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 panpdf-0.2.0/examples/defaults.yaml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panpdf-0.2.0/examples/include-after-body.tex
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panpdf-0.2.0/examples/include-before-body.tex
--rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 panpdf-0.2.0/examples/include-in-header.tex
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 panpdf-0.2.0/examples/images/figure.tex
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 panpdf-0.2.0/examples/images/header.tex
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 panpdf-0.2.0/examples/src/1.md
--rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 panpdf-0.2.0/examples/src/2.md
--rw-r--r--   0        0        0    37281 2020-02-02 00:00:00.000000 panpdf-0.2.0/notebooks/pdf.ipynb
--rw-r--r--   0        0        0    60992 2020-02-02 00:00:00.000000 panpdf-0.2.0/notebooks/pgf.ipynb
--rw-r--r--   0        0        0    29602 2020-02-02 00:00:00.000000 panpdf-0.2.0/notebooks/png.ipynb
--rw-r--r--   0        0        0    54307 2020-02-02 00:00:00.000000 panpdf-0.2.0/notebooks/seaborn.ipynb
--rw-r--r--   0        0        0    55134 2020-02-02 00:00:00.000000 panpdf-0.2.0/notebooks/svg.ipynb
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 panpdf-0.2.0/src/panpdf/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panpdf-0.2.0/src/panpdf/__init__.py
--rw-r--r--   0        0        0     2940 2020-02-02 00:00:00.000000 panpdf-0.2.0/src/panpdf/formatters.py
--rw-r--r--   0        0        0     8550 2020-02-02 00:00:00.000000 panpdf-0.2.0/src/panpdf/main.py
--rw-r--r--   0        0        0     3963 2020-02-02 00:00:00.000000 panpdf-0.2.0/src/panpdf/stores.py
--rw-r--r--   0        0        0     9878 2020-02-02 00:00:00.000000 panpdf-0.2.0/src/panpdf/tools.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panpdf-0.2.0/src/panpdf/filters/__init__.py
--rw-r--r--   0        0        0     4518 2020-02-02 00:00:00.000000 panpdf-0.2.0/src/panpdf/filters/attribute.py
--rw-r--r--   0        0        0     1947 2020-02-02 00:00:00.000000 panpdf-0.2.0/src/panpdf/filters/crossref.py
--rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 panpdf-0.2.0/src/panpdf/filters/filter.py
--rw-r--r--   0        0        0     5120 2020-02-02 00:00:00.000000 panpdf-0.2.0/src/panpdf/filters/jupyter.py
--rw-r--r--   0        0        0     4342 2020-02-02 00:00:00.000000 panpdf-0.2.0/src/panpdf/filters/layout.py
--rw-r--r--   0        0        0     2996 2020-02-02 00:00:00.000000 panpdf-0.2.0/src/panpdf/filters/verbatim.py
--rw-r--r--   0        0        0     4012 2020-02-02 00:00:00.000000 panpdf-0.2.0/src/panpdf/filters/zotero.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panpdf-0.2.0/tests/__init__.py
--rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 panpdf-0.2.0/tests/conftest.py
--rw-r--r--   0        0        0     1947 2020-02-02 00:00:00.000000 panpdf-0.2.0/tests/test_converters.py
--rw-r--r--   0        0        0     2637 2020-02-02 00:00:00.000000 panpdf-0.2.0/tests/test_formatters.py
--rw-r--r--   0        0        0     4432 2020-02-02 00:00:00.000000 panpdf-0.2.0/tests/test_main.py
--rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 panpdf-0.2.0/tests/test_stores.py
--rw-r--r--   0        0        0     8282 2020-02-02 00:00:00.000000 panpdf-0.2.0/tests/test_tools.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panpdf-0.2.0/tests/filters/__init__.py
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 panpdf-0.2.0/tests/filters/conftest.py
--rw-r--r--   0        0        0     7279 2020-02-02 00:00:00.000000 panpdf-0.2.0/tests/filters/test_attribute.py
--rw-r--r--   0        0        0      918 2020-02-02 00:00:00.000000 panpdf-0.2.0/tests/filters/test_crossref.py
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 panpdf-0.2.0/tests/filters/test_filter.py
--rw-r--r--   0        0        0     4798 2020-02-02 00:00:00.000000 panpdf-0.2.0/tests/filters/test_jupyter.py
--rw-r--r--   0        0        0     4712 2020-02-02 00:00:00.000000 panpdf-0.2.0/tests/filters/test_layout.py
--rw-r--r--   0        0        0     2607 2020-02-02 00:00:00.000000 panpdf-0.2.0/tests/filters/test_verbatim.py
--rw-r--r--   0        0        0     2416 2020-02-02 00:00:00.000000 panpdf-0.2.0/tests/filters/test_zotero.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panpdf-0.2.0/tests/libraries/__init__.py
--rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 panpdf-0.2.0/tests/libraries/test_nbformat.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panpdf-0.2.0/tests/libraries/panflute/__init__.py
--rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 panpdf-0.2.0/tests/libraries/panflute/test_cite.py
--rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 panpdf-0.2.0/tests/libraries/panflute/test_code.py
--rw-r--r--   0        0        0     6171 2020-02-02 00:00:00.000000 panpdf-0.2.0/tests/libraries/panflute/test_figure.py
--rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 panpdf-0.2.0/tests/libraries/panflute/test_math.py
--rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 panpdf-0.2.0/tests/libraries/panflute/test_metadata.py
--rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 panpdf-0.2.0/tests/libraries/panflute/test_raw.py
--rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 panpdf-0.2.0/tests/libraries/panflute/test_section.py
--rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 panpdf-0.2.0/tests/libraries/panflute/test_table.py
--rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 panpdf-0.2.0/tests/libraries/panflute/test_tex.py
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 panpdf-0.2.0/.gitignore
--rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 panpdf-0.2.0/LICENSE.txt
--rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 panpdf-0.2.0/README.md
--rw-r--r--   0        0        0     2609 2020-02-02 00:00:00.000000 panpdf-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1793 2020-02-02 00:00:00.000000 panpdf-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 panpdf-0.2.1/.gitattributes
+-rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 panpdf-0.2.1/mkdocs.yml
+-rw-r--r--   0        0        0     6064 2020-02-02 00:00:00.000000 panpdf-0.2.1/ruff_defaults.toml
+-rw-r--r--   0        0        0      955 2020-02-02 00:00:00.000000 panpdf-0.2.1/.devcontainer/devcontainer.json
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 panpdf-0.2.1/.devcontainer/postCreate.sh
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 panpdf-0.2.1/.devcontainer/starship.toml
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 panpdf-0.2.1/.devcontainer/features/zotero/devcontainer-feature.json
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 panpdf-0.2.1/.devcontainer/features/zotero/install.sh
+-rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 panpdf-0.2.1/examples/defaults.yaml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panpdf-0.2.1/examples/include-after-body.tex
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panpdf-0.2.1/examples/include-before-body.tex
+-rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 panpdf-0.2.1/examples/include-in-header.tex
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 panpdf-0.2.1/examples/images/figure.tex
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 panpdf-0.2.1/examples/images/header.tex
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 panpdf-0.2.1/examples/src/1.md
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 panpdf-0.2.1/examples/src/2.md
+-rw-r--r--   0        0        0    30244 2020-02-02 00:00:00.000000 panpdf-0.2.1/notebooks/backend.ipynb
+-rw-r--r--   0        0        0    28432 2020-02-02 00:00:00.000000 panpdf-0.2.1/notebooks/hvplot.ipynb
+-rw-r--r--   0        0        0    37281 2020-02-02 00:00:00.000000 panpdf-0.2.1/notebooks/pdf.ipynb
+-rw-r--r--   0        0        0    67211 2020-02-02 00:00:00.000000 panpdf-0.2.1/notebooks/pgf.ipynb
+-rw-r--r--   0        0        0    29602 2020-02-02 00:00:00.000000 panpdf-0.2.1/notebooks/png.ipynb
+-rw-r--r--   0        0        0    54421 2020-02-02 00:00:00.000000 panpdf-0.2.1/notebooks/seaborn.ipynb
+-rw-r--r--   0        0        0    55134 2020-02-02 00:00:00.000000 panpdf-0.2.1/notebooks/svg.ipynb
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 panpdf-0.2.1/src/panpdf/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panpdf-0.2.1/src/panpdf/__init__.py
+-rw-r--r--   0        0        0     2940 2020-02-02 00:00:00.000000 panpdf-0.2.1/src/panpdf/formatters.py
+-rw-r--r--   0        0        0     8550 2020-02-02 00:00:00.000000 panpdf-0.2.1/src/panpdf/main.py
+-rw-r--r--   0        0        0     3963 2020-02-02 00:00:00.000000 panpdf-0.2.1/src/panpdf/stores.py
+-rw-r--r--   0        0        0     9878 2020-02-02 00:00:00.000000 panpdf-0.2.1/src/panpdf/tools.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panpdf-0.2.1/src/panpdf/filters/__init__.py
+-rw-r--r--   0        0        0     4518 2020-02-02 00:00:00.000000 panpdf-0.2.1/src/panpdf/filters/attribute.py
+-rw-r--r--   0        0        0     1947 2020-02-02 00:00:00.000000 panpdf-0.2.1/src/panpdf/filters/crossref.py
+-rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 panpdf-0.2.1/src/panpdf/filters/filter.py
+-rw-r--r--   0        0        0     5783 2020-02-02 00:00:00.000000 panpdf-0.2.1/src/panpdf/filters/jupyter.py
+-rw-r--r--   0        0        0     4342 2020-02-02 00:00:00.000000 panpdf-0.2.1/src/panpdf/filters/layout.py
+-rw-r--r--   0        0        0     2996 2020-02-02 00:00:00.000000 panpdf-0.2.1/src/panpdf/filters/verbatim.py
+-rw-r--r--   0        0        0     4012 2020-02-02 00:00:00.000000 panpdf-0.2.1/src/panpdf/filters/zotero.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panpdf-0.2.1/tests/__init__.py
+-rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 panpdf-0.2.1/tests/conftest.py
+-rw-r--r--   0        0        0     1947 2020-02-02 00:00:00.000000 panpdf-0.2.1/tests/test_converters.py
+-rw-r--r--   0        0        0     2637 2020-02-02 00:00:00.000000 panpdf-0.2.1/tests/test_formatters.py
+-rw-r--r--   0        0        0     4432 2020-02-02 00:00:00.000000 panpdf-0.2.1/tests/test_main.py
+-rw-r--r--   0        0        0     3608 2020-02-02 00:00:00.000000 panpdf-0.2.1/tests/test_stores.py
+-rw-r--r--   0        0        0     8282 2020-02-02 00:00:00.000000 panpdf-0.2.1/tests/test_tools.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panpdf-0.2.1/tests/filters/__init__.py
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 panpdf-0.2.1/tests/filters/conftest.py
+-rw-r--r--   0        0        0     7279 2020-02-02 00:00:00.000000 panpdf-0.2.1/tests/filters/test_attribute.py
+-rw-r--r--   0        0        0      918 2020-02-02 00:00:00.000000 panpdf-0.2.1/tests/filters/test_crossref.py
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 panpdf-0.2.1/tests/filters/test_filter.py
+-rw-r--r--   0        0        0     5231 2020-02-02 00:00:00.000000 panpdf-0.2.1/tests/filters/test_jupyter.py
+-rw-r--r--   0        0        0     4712 2020-02-02 00:00:00.000000 panpdf-0.2.1/tests/filters/test_layout.py
+-rw-r--r--   0        0        0     2607 2020-02-02 00:00:00.000000 panpdf-0.2.1/tests/filters/test_verbatim.py
+-rw-r--r--   0        0        0     2416 2020-02-02 00:00:00.000000 panpdf-0.2.1/tests/filters/test_zotero.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panpdf-0.2.1/tests/libraries/__init__.py
+-rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 panpdf-0.2.1/tests/libraries/test_nbformat.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panpdf-0.2.1/tests/libraries/panflute/__init__.py
+-rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 panpdf-0.2.1/tests/libraries/panflute/test_cite.py
+-rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 panpdf-0.2.1/tests/libraries/panflute/test_code.py
+-rw-r--r--   0        0        0     6171 2020-02-02 00:00:00.000000 panpdf-0.2.1/tests/libraries/panflute/test_figure.py
+-rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 panpdf-0.2.1/tests/libraries/panflute/test_math.py
+-rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 panpdf-0.2.1/tests/libraries/panflute/test_metadata.py
+-rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 panpdf-0.2.1/tests/libraries/panflute/test_raw.py
+-rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 panpdf-0.2.1/tests/libraries/panflute/test_section.py
+-rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 panpdf-0.2.1/tests/libraries/panflute/test_table.py
+-rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 panpdf-0.2.1/tests/libraries/panflute/test_tex.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 panpdf-0.2.1/.gitignore
+-rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 panpdf-0.2.1/LICENSE.txt
+-rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 panpdf-0.2.1/README.md
+-rw-r--r--   0        0        0     2694 2020-02-02 00:00:00.000000 panpdf-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     1793 2020-02-02 00:00:00.000000 panpdf-0.2.1/PKG-INFO
```

### Comparing `panpdf-0.2.0/mkdocs.yml` & `panpdf-0.2.1/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `panpdf-0.2.0/ruff_defaults.toml` & `panpdf-0.2.1/ruff_defaults.toml`

 * *Files identical despite different names*

### Comparing `panpdf-0.2.0/.devcontainer/devcontainer.json` & `panpdf-0.2.1/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `panpdf-0.2.0/.devcontainer/starship.toml` & `panpdf-0.2.1/.devcontainer/starship.toml`

 * *Files identical despite different names*

### Comparing `panpdf-0.2.0/examples/defaults.yaml` & `panpdf-0.2.1/examples/defaults.yaml`

 * *Files identical despite different names*

### Comparing `panpdf-0.2.0/examples/include-in-header.tex` & `panpdf-0.2.1/examples/include-in-header.tex`

 * *Files identical despite different names*

### Comparing `panpdf-0.2.0/examples/src/1.md` & `panpdf-0.2.1/examples/src/1.md`

 * *Files identical despite different names*

### Comparing `panpdf-0.2.0/notebooks/pdf.ipynb` & `panpdf-0.2.1/notebooks/pdf.ipynb`

 * *Files identical despite different names*

### Comparing `panpdf-0.2.0/notebooks/png.ipynb` & `panpdf-0.2.1/notebooks/png.ipynb`

 * *Files identical despite different names*

### Comparing `panpdf-0.2.0/notebooks/seaborn.ipynb` & `panpdf-0.2.1/notebooks/seaborn.ipynb`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9456426916754817%*

 * *Differences: {"'cells'": "{0: {'execution_count': 1, 'source': {insert: [(0, 'import matplotlib as mpl\\n'), "*

 * *            '(6, \'set_formatter("seaborn", "pgf")\\n\'), (7, \'\\n\'), (8, \'\\n\'), (9, '*

 * *            '\'mpl.rcParams["pgf.rcfonts"] = False\')], delete: [5]}}, 1: {\'execution_count\': 2, '*

 * *            "'outputs': {0: {'data': {'image/png': "*

 * *            "'iVBORw0KGgoAAAANSUhEUgAABK4AAAN6CAYAAACnkgHIAAAAOXRFWHRTb2Z0d2FyZQBNYXRwbG90bGliIHZlcnNpb24zLjguNCwgaHR0cHM6Ly9tYXRwbG90bGliLm9yZy8fJSN1AAAACXBIWXMAAB2HAA […]*

```diff
@@ -1,31 +1,35 @@
 {
     "cells": [
         {
             "cell_type": "code",
-            "execution_count": 14,
+            "execution_count": 1,
             "metadata": {},
             "outputs": [],
             "source": [
+                "import matplotlib as mpl\n",
                 "import pandas as pd\n",
                 "import seaborn.objects as so\n",
                 "\n",
                 "from panpdf.formatters import set_formatter\n",
                 "\n",
-                "set_formatter(\"seaborn\", \"pgf\")"
+                "set_formatter(\"seaborn\", \"pgf\")\n",
+                "\n",
+                "\n",
+                "mpl.rcParams[\"pgf.rcfonts\"] = False"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 29,
+            "execution_count": 2,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
-                        "image/png": "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W/78z/88733vezNixIgq/IQAAAAAvVddpVKp9PQkesq8efNy9NFHb9C++++/f6688sqMGjVqk8draWnJ1KlT88tf/nKd+w0fPjyf+9zncthhh23yWNXQ0rIsHR2dPTqHjTFixMA0Njakvb0jra3Le3o6sMVY+9Qi655aZN1Ti6x7alFvXvcNDfVpahpU1WPW9BlXSdLU1JSJEydmr732yg477JCRI0dm2LBhefHFF/Pwww/nxhtvzLx58zJnzpycfPLJuemmm9KvX7+NHqezszN/+7d/m1/96ldJktGjR+f/+//+v+yxxx4ZMGBAnn766dxwww25//77s3jx4nz84x/PDTfckD333LPaPzIAAABAr1DTZ1x1dHSkvr5+nZcAtrW1ZerUqbn77ruTJNOmTcsJJ5yw0WP9+Mc/zsc//vEkybhx43LDDTdk8ODBr9vv85//fL72ta8lSd72trfl3/7t3zZ6rGpxxhX0DtY+tci6pxZZ99Qi655a1JvXfXeccVXTN2dvaGhY732r+vTpk9NOO63r6/vuu2+TxpozZ07X9sknn7zGaJUkH/vYx9KnT58kWe8lhQAAAABbs5oOVxtq0KD/q4XLli3bpGO89NJLXdvbb7/9OscaPnz4Zo0FAAAAsDUQrjbA9OnTu7Z32WWXTTrGzjvv3LW9YMGCte63bNmyLF68eLPGAgAAANgaCFdr0NHRkUWLFuXee+/NmWee2XXPqT59+uT444/fpGMeffTRXWdufeMb33jNGVir+4//+I+0tbUlySbdSwsAAABga1HTN2df3fz583PEEUes9fFhw4bl85//fA477LBNHuPnP/95zjjjjCxZsiRjxozJySefnD322CMDBw7s+lTBV++hddJJJ+W8885b7z24ulN7e0ePjb0pGhpeudF+pVLpVTeVh81l7VOLrHtqkXVPLbLuqUW9fd03NjZU9XjC1R+tLVzV19fnlFNOycknn5yRI0du9jjPPvtsvvOd7+Q///M/8/LLL7/u8UMPPTSnnHJK3vKWt2z2WAAAAAC9WWNPT6AUY8aMyYwZM5IknZ2daW1tzdy5c3P99dfnG9/4Rh5//PFcdNFFGT169CaP0dHRkRkzZuSWW25ZY7RKXvkkwWHDhmXs2LHrvIn7luCMK+gdrH1qkXVPLbLuqUXWPbWot697Z1xtYS+99FJOP/303HvvvRk1alSuvfbajBs3bqOPs3LlynzsYx/Lf//3fydJ3vnOd2bKlCnZY4890rdv3zz77LO5/fbb8x//8R9Zvnx5RowYka985SvZd999q/0jbbCWlmW96pdkxIiBaWxsSHt7R1pbl/f0dGCLsfapRdY9tci6pxZZ99Si3rzuGxrq09Q0qKrHdHP29Rg8eHCuuOKK9O/fP4sWLcq0adM26ThXXXVVV7T68Ic/nCuvvDIHHHBABg8enL59+2bs2LH5yEc+kuuuuy59+vRJa2tr/v7v/z6rVq2q5o8DAAAA0GsIVxtgm222yX777ZckmT17dp5//vmNen6lUskNN9yQJBk4cGCmTp261n333nvvHH300UmSBQsWdMUuAAAAgFojXG2gpqamru0FCxZs1HNfeOGFtLa2Jkl233339O/ff53777PPPl3bjz766EaNBQAAALC1EK420HPPPde1PWjQxl2v2dDwfzcma29vX+/+q+/Tp0+fjRoLAAAAYGshXG2A+fPn51e/+lWSVy7122mnnTbq+SNGjMjQoUOTJPPmzUtLS8s697/vvvu6tnfccceNnC0AAADA1qGmw9XNN9+cF198cZ37NDc354wzzkhbW1uSZPLkya+71O/+++/P+PHjM378+EyZMuV1x6irq8sRRxyRJGlra8tFF1201jOvbrvttsyaNSvJK2d2HXzwwRv9cwEAAABsDRp7egI96Zvf/GYuvvjiHH744Zk4cWLGjRuXoUOHpr29PQsXLszs2bMzffr0LFmyJEkyduzYnHXWWZs01umnn5677rorS5cuze23355jjz02xx9/fPbcc8/06dMnzzzzTG6//fbMmDEjlUolSXLGGWdk8ODBVft5AQAAAHqTmg5XSbJixYrMnDkzM2fOXOd+kyZNyqWXXpoRI0Zs0jg77LBDvv71r+eMM87IggUL8sgjj2TatGlr3LdPnz45/fTTc+KJJ27SWAAAAABbg5oOV1dddVXuueeePPDAA3n88cfT3NyclpaWVCqVDBkyJGPHjs2ECRMyefLkTJgwYbPHmzBhQm699dbccsstueuuu/LII4+ktbU1HR0dGTx4cHbeeecceOCBec973rPR99ECAAAA2NrUVV69Lg3+REvLsnR0dPb0NDbYiBED09jYkPb2jrS2Lu/p6cAWY+1Ti6x7apF1Ty2y7qlFvXndNzTUp6lpUFWPWdM3ZwcAAACgXMIVAAAAAEUSrgAAAAAoknAFAAAAQJGEKwAAAACKJFwBAAAAUCThCgAAAIAiCVcAAAAAFEm4AgAAAKBIwhUAAAAARRKuAAAAACiScAUAAABAkYQrAAAAAIokXAEAAABQJOEKAAAAgCIJVwAAAAAUSbgCAAAAoEjCFQAAAABFEq4AAAAAKJJwBQAAAECRhCsAAAAAiiRcAQAAAFAk4QoAAACAIglXAAAAABRJuAIAAACgSMIVAAAAAEUSrgAAAAAoknAFAAAAQJGEKwAAAACKJFwBAAAAUCThCgAAAIAiCVcAAAAAFEm4AgAAAKBIwhUAAAAARRKuAAAAACiScAUAAABAkYQrAAAAAIokXAEAAABQJOEKAAAAgCIJVwAAAAAUSbgCAAAAoEjCFQAAAABFEq4AAAAAKJJwBQAAAECRhCsAAAAAiiRcAQAAAFAk4QoAAACAIglXAAAAABRJuAIAAACgSMIVAAAAAEUSrgAAAAAoknAFAAAAQJGEKwAAAACKJFwBAAAAUCThCgAAAIAiCVcAAAAAFEm4AgAAAKBIwhUAAAAARRKuAAAAACiScAUAAABAkYQrAAAAAIokXAEAAABQJOEKAAAAgCIJVwAAAAAUSbgCAAAAoEjCFQAAAABFEq4AAAAAKJJwBQAAAECRhCsAAAAAiiRcAQAAAFAk4QoAAACAIglXAAAAABRJuAIAAACgSMIVAAAAAEUSrgAAAAAoknAFAAAAQJGEKwAAAACKJFwBAAAAUCThCgAAAIAiCVcAAAAAFEm4AgAAAKBIwhUAAAAARRKuAAAAACiScAUAAABAkYQrAAAAAIokXAEAAABQJOEKAAAAgCIJVwAAAAAUSbgCAAAAoEjCFQAAAABFEq4AAAAAKJJwBQAAAECRhCsAAAAAiiRcAQAAAFAk4QoAAACAIglXAAAAABRJuAIAAACgSMIVAAAAAEUSrgAAAAAoknAFAAAAQJGEKwAAAACKJFwBAAAAUCThCgAAAIAiCVcAAAAAFEm4AgAAAKBIwhUAAAAARRKuAAAAACiScAUAAABAkYQrAAAAAIokXAEAAABQJOEKAAAAgCIJVwAAAAAUSbgCAAAAoEjCFQAAAABFEq4AAAAAKJJwBQAAAECRGnt6Aj1p5cqVueeee/Lggw/moYceyoIFC7J48eIsXbo0ffv2zejRo7P33ntn8uTJmTRpUurq6qo29vLlyzN9+vTcddddefTRR9Pc3Jz+/funqakp48ePz4EHHpijjz46w4YNq9qYAAAAAL1JTYerp556KqeffvoaH2tra8sTTzyRJ554IjNmzMj++++fK6+8MqNGjdrscX/605/m05/+dJ577rnXfH/VqlVZunRpnnzyydx+++3Zfffdc9BBB232eAAAAAC9UU2HqyRpamrKxIkTs9dee2WHHXbIyJEjM2zYsLz44ot5+OGHc+ONN2bevHmZM2dOTj755Nx0003p16/fJo83Y8aMnHvuueno6MjgwYPznve8JwcddFBGjx6dzs7OLFiwIHPmzMmPf/zjKv6UAAAAAL1PXaVSqfT0JHpKR0dH6uvr13kJYFtbW6ZOnZq77747STJt2rSccMIJmzTeI488kve85z1pa2vLPvvsky9/+cvZZptt1jl2nz59NmmsamhpWZaOjs4eG39jjRgxMI2NDWlv70hr6/Keng5sMdY+tci6pxZZ99Qi655a1JvXfUNDfZqaBlX1mDV9c/aGhob13reqT58+Oe2007q+vu+++zZ5vAsvvDBtbW0ZPnz4eqPVq2MDAAAA1KqaDlcbatCg/6uFy5Yt26Rj/PKXv8xvfvObJMkHPvCB9UYrAAAAgFpX8/e42hDTp0/v2t5ll1026Ri33HJL1/bb3/72ru2VK1dm4cKF6du3b0aOHOksKwAAAIA/Eq7WoKOjIy0tLXn00Udzww035NZbb03yyqV7xx9//CYdc+7cuUmSxsbG7L777pk7d26uuuqq3Hvvveno6EiSDBgwIAcffHBOPfXU7L///tX5YQAAAAB6qZq+Ofvq5s+fnyOOOGKtjw8bNiyf//znc9hhh230sSuVSvbaa690dHRkxIgR+cQnPpFLLrkknZ1rvvF5XV1d/u7v/i4f+9jHNnqsampv7+jR8TdWQ8MrN9qvVCq96qbysLmsfWqRdU8tsu6pRdY9tai3r/vGxoaqHk+4+qO1hav6+vqccsopOfnkkzNy5MhNOvaLL76YAw44IMkrZ211dHSkoaEhf/u3f5t3vetdGTNmTF544YXccsstueqqq7Jy5cokyeWXX553v/vdm/wzAQAAAPRmwtUftbW15YknnkiSdHZ2prW1NXPnzs3111+fF154IYcddlguuuiijB49eqOP/dxzz73uTK0r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aunSpbn44oszc+bMJK+cZbXNNtvkkksuyVvf+tbuGBIAAACArUzVw9XPfvazXHDBBVm0aFHXTdXf8Y535OKLL86IESOqPRwAAAAAW6mqhqtPf/rTueGGG5K8cpbV0KFDc+GFF+aYY46p5jAAAAAA1ICqhqvvfe97qaurS6VSyf/7f/8vl112WcaMGVPNIQAAAACoEVW/VLB///4555xzcsIJJ1T70AAAAADUkKqGqze/+c25/PLLs9NOO1XzsAAAAADUoKqGq29/+9upq6ur5iEBAAAAqFH11TyYaAUAAABAtVQ1XAEAAABAtQhXAAAAABRJuAIAAACgSMIVAAAAAEUSrgAAAAAoknAFAAAAQJGEKwAAAACKJFwBAAAAUCThCgAAAIAiCVcAAAAAFEm4AgAAAKBIwhUAAAAARRKuAAAAACiScAUAAABAkYQrAAAAAIokXAEAAABQJOEKAAAAgCIJVwAAAAAUSbgCAAAAoEjCFQAAAABFEq4AAAAAKJJwBQAAAECRhCsAAAAAiiRcAQAAAFAk4QoAAACAIglXAAAAABRJuAIAAACgSMIVAAAAAEUSrgAAAAAoknAFAAAAQJGEKwAAAACKJFwBAAAAUCThCgAAAIAiCVcAAAAAFEm4AgAAAKBIwhUAAAAARRKuAAAAACiScAUAAABAkYQrAAAAAIokXAEAAABQJOEKAAAAgCIJVwAAAAAUSbgCAAAAoEjCFQAAAABFEq4AAAAAKJJwBQAAAECRhCsAAAAAitTY0xPoSStXrsw999yTBx98MA899FAWLFiQxYsXZ+nSpenbt29Gjx6dvffeO5MnT86kSZNSV1fXLfN46qmn8q53vSsrVqxIkmy//faZNWtWt4wFAAAA0FvUdLh66qmncvrpp6/xsba2tjzxxBN54oknMmPGjOy///658sorM2rUqKrOobOzM+eff35XtAIAAADgFTUdrpKkqakpEydOzF577ZUddtghI0eOzLBhw/Liiy/m4Ycfzo033ph58+Zlzpw5Ofnkk3PTTTelX79+VRv/P//zPzNnzpxss802eeGFF6p2XAAAAIDerqbD1a677pqf//zna70E8MADD8wJJ5yQqVOn5u67787vf//73HTTTTnhhBOqMv4TTzyRL37xi0mSadOmZerUqVU5LgAAAMDWoKZvzt7Q0LDe+1b16dMnp512WtfX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OQtaV6S9o5L+feozpF9jBvav6eUNAAAAvV5dpVKp9PQkesq8efNy9NFHb9C++++/f6688sqMGjVqs8b82c9+lrPPPjuLFy9e4+ONjY35xCc+kY985CObNU41tLQsS0dHZ09PY606Oyv59WPN+fGcp/PQk62veayxoS6H7PWGvHW/HTL2DUN6aIawZYwYMTCNjQ1pb+9Ia+vynp4ObBHWPbXIuqcWWffUot687hsa6tPUNKiqx6z5U1KampoyceLE7LXXXtlhhx0ycuTIDBs2LC+++GIefvjh3HjjjZk3b17mzJmTk08+OTfddFP69eu3SWP95je/ydSpU7NixYo0NjZmypQpOfzww9O3b9888MAD+epXv5rm5uZ84QtfyODBg3PCCSdU+afderS+uDL//L0HsmDRstSv4US49o5Kfv7gc/nZr5/NIXuNyclH7pnGBlfGAgAAQG9S02dcdXR0pL6+fp2XALa1tWXq1Km5++67kyTTpk3bpKBUqVRy7LHH5re//W3q6uryb//2bzniiCNes8/8+fNz7LHHZvHixRk4cGDuvPPObLPNNhs9VrWUesZV64sr85n//EWWLm9LZ+f6l299XfKmnZvyd++ZIF6xVerN/yIDm8q6pxZZ99Qi655a1JvXfXeccVXT7+IbGhrWe9+qPn365LTTTuv6+r777tuksX72s5/lt7/9bZLkyCOPfF20SpIddtghf//3f58kWb58ea699tpNGmtr1tlZyb9874ENjlZJ0llJfvtkS264+9Funh0AAABQTTUdrjbUoEH/VwuXLVu2Sce47bbburbf//73r3W/d73rXenfv3+S5Ec/+tEmjbU1+/XjzZm/aNkGR6tXVSrJrP9dkJdWtHXTzAAAAIBqE642wPTp07u2d9lll006xuzZs5Mk/fr1y5vf/Oa17jdgwIDsu+++SZI//OEPee655zZpvK3VXb98eo33tNoQlUol//3rZ6s7IQAAAKDbCFdr0NHRkUWLFuXee+/NmWeema997WtJXrls8Pjjj9/o461YsSLz589PkowdOzZ9+/Zd5/677bZb1/ajj7q87VUtS1/Ob59szUaebNWls5Lc/b/zqzspAAAAoNvU/KcKvmr+/PlrvO/Uq4YNG5bPf/7z2XXXXTf62M8++2xevQf+tttuu979V9/nmWee2ejxqmXo0P49NvaaPNO6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akuu+6effjr33HNP5syZk9/97nd59tlns2rVqgwaNCjjxo3LwQcfnPe+973ZbrvtqjIerEtP/Jn/pxYvXpyjjjoqixYt6vre7373u24dk9rWU+u+ra0tt956a3784x/noYceSnNzcxobG9PU1JRdd901EydOzFFHHZUxY8ZUfWzoiXV/7733Zvr06XnggQeycOHCrFq1KoMHD84uu+ySQw45JO973/uy7bbbVnVMWF1PvO6ulfe2dZVKpdLTk6B2vfvd787DDz+81ser/Zfab3/720ydOjULFixY6z5TpkzJBRdckLq6uqqNC6vbUuv+vPPOy80337ze/fr165czzzwzJ5100maPCeuypf/MX5Ozzjort9xyy2u+J1zRnXpi3f/qV7/K+eefn8cee2yd+332s5/N3/zN31R1bEi27Lp/+eWXc8455+SOO+5Y534DBgzIpz71qRx77LFVGRdW1xOvu2vpva0zruhRq3fTgQMHZo899sgLL7yQP/zhD1Ufa/78+Tn11FPT3NycJDn22GNz5JFHZujQoXnooYfyta99LU8//XSuu+669OvXL+ecc07V5wDJllv3zz33XJKkf//+Ofzww3PggQdmt912y+DBg7No0aLcdddduemmm7Jy5cp89rOfTUdHR0455ZSqzgFWtyX/zF+TO+64I7fcckv69++fhoaGLFu2bIuMS23b0uv+3nvvzcc+9rEsX748ffv2zbvf/e78+Z//ed7whjekrq4uCxcuzAMPPJA777yzW8aHZMuu+09+8pNd0WrYsGE58cQTM2HChAwfPjzPPPNMbr311txxxx1ZsWJFLrjggjQ1NeXwww+v+jyobVv6dXetvbcVruhRxx57bIYPH5699toru+yyS+rr63Peeed1y19ql19+edcv9oUXXpgpU6Z0PTZhwoS8853vzPvf//48+eSTueaaa3LMMcdk/PjxVZ8HbKl1P3r06Jx//vl5z3vek8GDB7/u8cMOOyxHHnlkTj311KxatSpf/OIXM3ny5LzhDW+o6jzgVVvyz/w/1dLSkosuuihJcsYZZ+S6664TrtgituS6X7hwYT7xiU9k+fLl2WmnnfLVr341O++882v22WefffK2t70tZ599dlatWlX1OUCy5db9I488kttvvz1J0tTUlJtvvvk1r2NefY3/7W9/OxdffHEqlUquvPJK4Yqq29Kvu2vtva2bs9OjTjzxxBxzzDHZddddU1/ffcvxscce6/qXmDe/+c2v+cV+1fDhw3PhhRcmSTo7O3P11Vd323yobVtq3X/uc5/LSSedtMa/PF918MEH57jjjkuSrFq1ar2n2cPm2FJrf00uvvjiNDc3Z999982HPvShLTo2tW1LrvvLLrssS5YsSZ8+ffLv//7vr4tWf6pv377dOh9q15Za97/85S+7tt/3vvetNQIcf/zxGT16dJLk4Ycf9g8XVN2WfN1di+9thStqwm233da1/b73vW+t+x166KHZfvvtkySzZs3KypUru31u0NPe8pa3dG0/+eSTPTcR6CYzZ87Mbbfdlr59++ayyy7b4tEMtoQFCxZ0Xf43efLk7L777j08I+h+L730Utf2q6/h16Suru41jwtX9JRqvO6uxfe2XrlRE2bPnt21ffDBB691v7q6uq4bRS5fvjy/+c1vun1u0NNWv1TEG3q2Ns3NzbnkkkuSJB/72Mey22679fCMoHvMnDmz6xPb3v72t3d9f9WqVZk/f36eeeYZlway1Vn9rMJ13aC6Uql0PT5kyJCMHDmyu6cGa1SN1921+N7WOxRqwqOPPpokGTRo0Ho/fnT1NzXr+zQe2Brcd999Xdv+hZ6tzUUXXZTW1tbsueeeOfXUU3t6OtBt5s6d27W955575rHHHsvUqVOz33775Ygjjsjhhx+e/fbbLyeeeGLuvvvuHpwpVM/hhx/edXngDTfckIULF65xv+9+97t5/vnnkyTHHXdcGhoattgcYXXVeN1di+9t3Zydrd6qVavywgsvJEm23Xbb9e6/+j7PPPNMt80LSvD000/nBz/4QZJXPvVn9X+lh95uxowZueOOO9LY2JjLLrssjY1e9rD1mjdvXtf2Aw88kPPPP/91l4W0tbXl/vvvz/3335/3v//9ufjii3v9R6RT2/r165cvf/nL+ehHP5pnn302Rx99dE488cTsu+++GTZsWJ555pnMnDmz6wbuRx55ZP7u7/6uh2dNrarG6+5afW/rFRxbvdWvfR80aNB69199H9e/szVbtWpVzj333CxfvjxJcuqpp6apqamHZwXVsWjRolx66aVJkg9/+MN505ve1MMzgu61ZMmSru3zzz8/q1atyoknnpjjjjsuO+64Y5YsWZI777wzX/ziF7NkyZJcf/31GTNmTD7+8Y/34Kxh8+255565+eab873vfS/XXHNNvvSlL71un3333TennHJK/vIv/7IHZgjVe91dq+9tXSrIVm/1f23s06fPevdf/RN2VqxY0S1zghJMmzYtc+bMSZIceOCBOe2003p4RlA9n/70p7N48eLstttu3phTE1Z/Q7Jy5cp88pOfzAUXXJBdd901ffv2zahRo3LCCSfk2muv7Xqt85WvfKXrX+6hN7vzzjszY8aMLF68eI2PP/TQQ7n55pvzyCOPbNmJwR9V63V3rb63Fa7Y6vXr169ru62tbb37r37DvAEDBnTLnKCnXX755fn+97+fJBk3bly++MUvut8DW40f/OAHmTVrVurr63PZZZe95kUbbK1Wf72z44475qSTTlrjfnvssUfe//73J3nlDdCrl1BBb1SpVHLeeeflU5/6VH7/+9/nkEMOyde//vX84he/yIMPPpi7774706ZNy9ChQ3P33XfnuOOOy6xZs3p62tSYar7urtX3tsIVW73Bgwd3bW/I6ZGvnr6ZbNjpl9DbfOELX8g111yTJBk7dmy++c1v+nQdthoLFy7MP/7jPyZJPvShD2Xfffft4RnBlrH6a5a/+Iu/WOenVU2aNKlr+9e//nV3Tgu61fXXX5+bb745ySv3r/rGN76RQw89NEOHDk2fPn2y3Xbb5YQTTsj3vve9DB8+PCtWrMjZZ5+dlpaWHp45taLar7tr9b2te1yx1evbt29GjhyZ5ubmPPvss+vdf/Wb1m3IDe+gN/nnf/7nXH311Ule+cvzuuuuy5gxY3p4VlA91157bZYuXZp+/fplt912y6233rrG/VZ/Ibf6Pu94xzs26NR7KM3222+fRYsWJVn/65fVP4Wqubm5W+cF3el73/te1/YnP/nJtX7YwA477JApU6bkS1/6UpYtW5Zbb701U6ZM2VLTpEZ1x+vuWn1vK1xRE3bfffc0Nzdn2bJleeaZZ9b5saGvfrxo8tqPD4Xe7oorrshXv/rVJMlOO+2Ua6+9VrRiq/PqKfErV67MBRdcsEHPOfPMM7u2f/GLXwhX9EpvfOMb88ADDyRJOjs717nv6o/7tE16s9///vdJkm222Wa9b8r32Wefru3VX+9Dd+jO1921+N7WpYLUhIkTJ3Zt33fffWvdr1Kp5P7770/yykeU7r333t0+N9gSPve5z73mL8/rrrsub3jDG3p4VgBUy0EHHdS1/eSTT65z39Uf9w8Y9Gavhtf29vb17rv6Pv6Bgu7U3a+7a/G9rXBFTfirv/qrru3VTyn+U//93/+dBQsWJHnl/g/9+/fv9rlBd7v88svz9a9/Pcn/naYsWrG1uuCCC/K73/1uvf/Zfvvtu56z+veHDh3ag7OHTXf44Yd33Xj3Jz/5yWs+eepP/ehHP+raXj14QW+z4447JkkWL1683k8MXP0N/qvPg2rbEq+7a/G9rXBFrzd//vyMHz8+48ePz1vf+tY17rPrrrvmbW97W5Jk7ty5+da3vvW6fRYvXpxLL700SVJfX7/JH1EKW8KGrPvklb88X70h5M477yxa0ett6NqHrcmGrPtBgwZ1fZJgS0tL14cU/Km77rqr675u2267bdfrIyjNhqz7t7/97V3bF1988WvuX7i6OXPm5Prrr0+SNDQ05PDDD6/+hKl51Xjd7b3tmrmonR711FNPZc6cOa/73qt+9rOfdVXiV/3N3/zNJo113nnnZc6cOWltbc1nPvOZPPzww5k8eXIGDx6cRx55JFdffXWefvrpJMlJJ52UPfbYY5PGgfXZUuv+iiuu6PrLc9iwYfnUpz6VJUuWZMmSJWt9zoABA/wrJN1mS/6ZD6XYkuv+Ix/5SH7yk5/k4YcfzvXXX5+nn34673//+7PTTjtlyZIlufPOO3P99denUqmkoaEh//iP/5i+fftu0liwLltq3Z900kn5/ve/n2eeeSb/+7//m2OOOSYf/OAHs88++2TgwIF5/vnn85Of/CQ33HBD2trakiRTpkzJTjvttAk/Fazdln7dXWvvbesqlUqlpydB7fr+97+f888/f6Oe87vf/e41X8+fPz9HHHFEklc+UWfWrFlrfe5vfvObTJ06dZ2fwHDCCSfk05/+9Fo/lQQ215Za929961tf96JwfQ488MBcd911G/Uc2FBb+s/8dVn99+NPx4Bq2tLr/oUXXsjpp5+euXPnrnWfwYMH53Of+1zXMaHatuS6f+qppzJ16tT1/lleV1eXD3zgA7ngggtSX+/CI6qrWq+7vbddM2dcUVP22Wef3HLLLfn2t7+dO++8M3/4wx+yfPnyjBo1Kvvtt1/e97735cADD+zpaQIAbJJtttkm3/72t3PLLbfk1ltvzcMPP5yWlpYMGDAgO++8c/7iL/4iH/jAB9LU1NTTU4WqGDt2bG666abceeedue222/LQQw+lubk5q1atyqBBg7LDDjtkv/32y3ve855ef9YJrK6W3ts64woAAACAIjlHEgAAAIAiCVcAAAAAFEm4AgAAAKBIwhUAAAAARRKuAAAAACiScAUAAABAkYQrAAAAAIokXAEAAABQJOEKAAAAgCIJVwAAAAAUSbgCAAAAoEjCFQAAAABFEq4AAAAAKJJwBQAAAECRhCsAAAAAiiRcAQAAAFAk4QoAAACAIglXAAC8xllnnZXx48dn/Pjx+dCHPpRKpbJBz/vxj3/c9bw3v/nNefrpp7t5pgDA1k64AgDgNT71qU9l1KhRSZL77rsv//Vf/7Xe57S0tOTTn/5019fnnntudtxxx26bIwBQG4QrAABeY/jw4bn00ku7vr7iiivy1FNPrfM5F110UZqbm5Mkhx56aI477rhunSMAUBuEKwAAXmfSpEk59thjkyQrVqzIeeedl87OzjXu+8Mf/jC33357kmTo0KG57LLLttg8AYCtm3AFAMAa/cM//EO22267JMn//u//5pprrnndPgsXLnzN2VkXXHBBxowZs8XmCABs3YQrAADWaPDgwbnssstSV1eXJLnyyivz6KOPvmafCy64IEuWLEmSvO1tb8u73/3uLT1NAGArJlwBALBWhxxySE444YQkyapVq3Luueemvb09SfLd7343P/vZz5IkI0aMyCWXXNJj8wQAtk51lQ39fGMAAGrS8uXL8653vSt/+MMfkiRTp07Nu971rhxzzDFZvnx5klfOxnrnO9/Zk9MEALZCwhUAAOv1y1/+MlOmTElnZ2f69OmTcePG5Xe/+12S5KijjsoXvvCFHp4hALA1Eq4AANggl19++etu0D5q1KjccsstGT58eM9MCgDYqglXAABskJUrV+Yd73hHnnvuua7vfeUrX8mkSZN6blIAwFbNzdkBANggc+fOzcKFC7u+rqury5AhQ3pwRgDA1s4ZVwAArNdLL72UY445JgsWLHjN93feeedMnz49/fv376GZAQBbM2dcAQCwXv/0T//UFa3222+/jB8/Pkny5JNP5p//+Z97cmoAwFbMGVcAAKzTT3/603zkIx9JkgwYMCDTp0/PsmXL8t73vjft7e2pr6/PddddlwMOOKCHZwoAbG2ccQUAwFotXbo0F154YdfXZ599dsaOHZs3velNOe2005IknZ2d+Yd/+IesWLGip6YJAGylhCsAANbqkksuyfPPP58kOeigg/KBD3yg67GPfvSj2XPPPZMkTz31VL7whS/0yBwBgK2XcAUAwBrdeeedmTFjRpJk0KBB+exnP5u6urqux/v06ZN/+qd/Sp8+fZIk3/rWt/KLX/yiR+YKAGydhCsAAF6npaUln/70p7u+Pu+887L99tu/br899tgjH/3oR5MklUol559/fpYvX77F5gkAbN2EKwAAXueiiy5KS0tLkuTQQw/N+973vrXue9ppp2WvvfZKkjz99NMuGQQAqka4AgDgNWbMmJHbb789STJ06NBcdtll69y/sbHxNZcM/td//Vfuv//+bp8nALD1E64AAOjy/PPP59JLL+36+oILLsiYMWPW+7w3vvGNOf3005O8csngP/zDP7hkEADYbMIVAABdPvWpT2Xx4sVJkre+9a1597vfvcHPPfXUU7PPPvskSebPn5/Pfe5z3TBDAKCW1FUqlUpPTwIAAAAA/pQzrgAAAAAoknAFAAAAQJGEKwAAAACKJFwBAAAAUCThCgAAAIAiCVcAAAAAFEm4AgAAAKBIwhUAAAAARRKuAAAAACiScAUAAABAkYQrAAAAAIokXAEAAABQJOEKAAAAgCIJVwAAAAAUSbgCAAAAoEjCFQAAAABFEq4AAAAAKJJwBQAAAECRhCsAAAAAiiRcAQAAAFAk4QoAAACAIglXAAAAABRJuAIAAACgSMIVAAAAAEX6/wGKXLaZGoY/GAAAAABJRU5ErkJggg==",
+                        "image/png": "iVBORw0KGgoAAAANSUhEUgAABK4AAAN6CAYAAACnkgHIAAAAOXRFWHRTb2Z0d2FyZQBNYXRwbG90bGliIHZlcnNpb24zLjguNCwgaHR0cHM6Ly9tYXRwbG90bGliLm9yZy8fJSN1AAAACXBIWXMAAB2HAAAdhwGP5fFlAABXTElEQVR4nO39e5zXdZ3//9/nwEFAYAYBzQOKGpqKpaHWz1Ky2lay2sVzYfIxc7dkc8VSv7ahZe5W7pabu1tW1mqfXFNTQkkzsbRNpfhAHtDMs+AJhuEgIMzh/fvDnDA5M8w8h/f1ernsZV8wr3m9nrP7QN7vG6/X611TqVQqAQAAAIDC1Hb3AgAAAABgbYQrAAAAAIokXAEAAABQJOEKAAAAgCIJVwAAAAAUSbgCAAAAoEjCFQAAAABFEq4AAAAAKJJwBQAAAECRhCsAAAAAiiRcAQAAAFAk4QoAAACAIglXAAAAABRJuAIAAACgSMIVAAAAAEUSrgAAAAAoknAFAAAAQJGEKwAAAACKJFwBAAAAUKT67l4A5VqyZEXa2irdvYyNNnBg39TX16W1tS1Ll77S3cuBLmP2qUbmnmpk7qlG5p5q1JPnvq6uJoMG9evUYwpXrFNbWyVtbe3dvYzN0lPXDVvK7FONzD3VyNxTjcw91ajnzX3n39jnVkEAAAAAiiRcAQAAAFAk4QoAAACAIglXAAAAABRJuAIAAACgSMIVAAAAAEUSrgAAAAAoknAFAAAAQJGEKwAAAACKJFwBAAAAUCThCgAAAIAiCVcAAAAAFEm4AgAAAKBIwhUAAAAARRKuAAAAACiScAUAAABAkYQrAAAAAIokXAEAAABQJOEKAAAAgCIJVwAAAAAUSbgCAAAAoEjCFQAAAABFqu/uBZRq8eLF+eAHP5gFCxZ0/N4f/vCHTjn2yy+/nGuuuSa33357nn766axcuTI77LBD3v72t+e4447LmDFjOuU8AAAAQPlaWtsz69GX8qvZz2XhkleyurUt2/Wpz147D8pRB++SPXYa2N1L7DbC1Tp86Utfel206iwPPfRQJk2alPnz57/u9+fPn5/58+dn6tSpmTBhQi644ILU1NR0+vkBAACAMlQqldx63zO55d6ns+KV1tTUJJXKq19btqIlC5e8kt88+EJ2Gdo/H3v/qLx518Hdut7uIFytxc9//vPcfPPN6du3b+rq6rJ8+fJOOe68efNy+umnp6mpKUkyfvz4HH300Rk4cGDmzp2b7373u3n22Wdz9dVXp0+fPvnsZz/bKecFAAAAytLeXsl3b56be+e+2PF7r0WrNfdJkvkLl+er18zOGR/aL2P2GdaVy+x2nnH1FxYtWpQLL7wwSXLWWWdl8ODBnXbsr3zlKx3R6vOf/3wuueSSHH744Rk9enROPPHEXH/99dl9992TJFdeeWWn3ZoIAAAAlOWaO/6Y+x5+ccM75tWg1d5eybenPpiHn27eyisri3D1Fy666KI0NTXlwAMPzMc//vFOO+7jjz+en//850mSt73tbZkwYcIb9hk8eHA+//nPJ0na29tzxRVXdNr5AQAAgDI88+Ky3DFr3huusNqQSiX57589ksqmfmMPJlytYfr06bn11lvTu3fvXHLJJamt7bz/89x6660d28cff/w69zv88MOz8847J0lmzJiRVatWddoaAAAAgO535+z5qavd9OdaV5K8tHhlHnlmcaevqVTC1Z80NTXli1/8YpLkU5/6VPbaa69OPf7MmTM7tg877LB17ldTU5NDDz00SbJixYo88MADnboOAAAAoPuseKU1v3nghbS1b95VU7W1Nbnjd8928qrKJVz9yYUXXpjm5ubsu+++Of300zv9+I899liSpH///nnTm9603n3XjGaPP/54p68FAAAA6B5Pv7gsLW3tm/397e2VqrriyqcKJpk2bVp+/vOfp76+Ppdccknq6zv3/yyrV6/OwoULkyQ77bTTBvdfc5/nnnuuU9eyKQYO7Ntt594cdXW1Hf+7oaFfN68Guo7ZpxqZe6qRuacamXu2RbXzl2zxMV5paauaPxNVH64WLFiQiy++OEnyiU98Im95y1s6/Rwvv/xyx3b//v03uP+a+yxfvrzT17Ox6uvruu3cW6KmpqbHrh22hNmnGpl7qpG5pxqZe7Ylffv02uJj1NdVz5+Jqg9XX/jCF7J48eLstdde+fSnP71VzrHmA9Z79drwgPbu3btje+XKlVtlTRujtbWt2869OerqalNTU5NKpZK2LbjsEnoas081MvdUI3NPNTL3bIsaBvTe8E4b0Diwb7Hv2Ts7qFV1uLrpppsyY8aM1NbW5pJLLnldMOpMffr06dhuaWnZ4P6rV6/u2N5uu+22ypo2xtKlr/SovxwaGvqlvr4ubW3taW5e0d3LgS5j9qlG5p5qZO6pRuaebdH2feqy89D+eW7B8mzO49lra5LDD9ipyD8TdXW1aWzc8J1mm6JqH87+4osv5stf/nKS5OMf/3gOPPDArXauAQMGdGxvzK1/K1b8efg25tZCAAAAoGeoqanJ+96+a1Kz2QfI4aM3/PzsbUXVXnF11VVXZenSpenTp0/22muv3HLLLWvdb82ItOY+73//+zfqtr/k1Vv/hgwZkqampjz//PMb3H/NB7JvzMPcAQAAgJ7j0H2H5ye/ejwvr2xJ+yZcdvXq1VY7ZmC/rXPHWImqNly9djveqlWrcsEFF2zU95x99tkd27/97W83Olwlyd57752mpqYsX748zz33XN70pjetc9/HHnusY3uvvfba6HMAAAAA5evTuy5nn/DWXHL1rLS2tW9UvKqtrcnuO26fj77vzVt/gQWp2lsFu9qYMWM6tu+999517lepVHLfffclSfr165f9999/q68NAAAA6Fq7Dd8+53/s4PTv2ys167ltsPZPX3zLiIacc+Jb06tKPk3wNTWVSmVzngVWNd7znvdk/vz5SZI//OEPm32cxx9/PEcffXSS5G1ve1v+53/+Z6373X333fnEJz6RJDn66KPz9a9/fbPPuaUWLVreIx/O3traVuRD6mBrMftUI3NPNTL3VCNzTzVY8UpL/veBF3L7757NwiWvpCZJTW1N2v90Gdb+ezTmqIN3yQF7DumIWKXaGg9nr9pbBTvTvHnzctRRRyVJdt5558yYMeMN++y5555573vfm1/84heZPXt2fvjDH+ZjH/vY6/ZZvHhxLr744iRJbW1tzjjjjK2/eAAAAKDb9OvbK+8bs2ve+/Zd8sd5S7KipT2t7ZX07VWbYYP6Ztjg7bp7id1KuOpC5513XmbNmpXm5uZ86UtfysMPP5xx48ZlwIABeeSRR3LFFVfk2WefTZKceuqp2Weffbp5xQAAAEBXqKmpyZt3HexKw78gXHWhXXfdNd/5zncyadKkPP/887n++utz/fXXv2G/k08+OZ/73Oe6YYUAAAAA5RCuutgBBxyQm2++OT/60Y9y++2355lnnsmKFSsydOjQHHTQQTn++ONzyCGHdPcyAQAAALqdh7OzTh7ODj2D2acamXuqkbmnGpl7qlFPnvut8XD22k49GgAAAAB0EuEKAAAAgCIJVwAAAAAUSbgCAAAAoEjCFQAAAABFEq4AAAAAKJJwBQAAAECRhCsAAAAAiiRcAQAAAFAk4QoAAACAIglXAAAAABRJuAIAAACgSMIVAAAAAEUSrgAAAAAoknAFAAAAQJGEKwAAAACKJFwBAAAAUCThCgAAAIAiCVcAAAAAFEm4AgAAAKBIwhUAAAAARRKuAAAAACiScAUAAABAkYQrAAAAAIokXAEAAABQJOEKAAAAgCIJVwAAAAAUSbgCAAAAoEjCFQAAAABFEq4AAAAAKJJwBQAAAECRhCsAAAAAiiRcAQAAAFAk4QoAAACAIglXAAAAABRJuAIAAACgSMIVAAAAAEUSrgAAAAAoknAFAAAAQJGEKwAAAACKJFwBAAAAUCThCgAAAIAiCVcAAAAAFEm4AgAAAKBIwhUAAAAARRKuAAAAACiScAUAAABAkYQrAAAAAIokXAEAAABQJOEKAAAAgCIJVwAAAAAUSbgCAAAAoEjCFQAAAABFEq4AAAAAKJJwBQAAAECRhCsAAAAAiiRcAQAAAFAk4QoAAACAIglXAAAAABRJuAIAAACgSMIVAAAAAEUSrgAAAAAoknAFAAAAQJGEKwAAAACKJFwBAAAAUCThCgAAAIAiCVcAAAAAFEm4AgAAAKBIwhUAAAAARRKuAAAAACiScAUAAABAkYQrAAAAAIokXAEAAABQJOEKAAAAgCIJVwAAAAAUSbgCAAAAoEjCFQAAAABFEq4AAAAAKJJwBQAAAECRhCsAAAAAiiRcAQAAAFAk4QoAAACAIglXAAAAABRJuAIAAACgSMIVAAAAAEUSrgAAAAAoknAFAAAAQJGEKwAAAACKJFwBAAAAUCThCgAAAIAiCVcAAAAAFEm4AgAAAKBIwhUAAAAARRKuAAAAACiScAUAAABAkYQrAAAAAIokXAEAAABQJOEKAAAAgCIJVwAAAAAUSbgCAAAAoEjCFQAAAABFEq4AAAAAKJJwBQAAAECRhCsAAAAAiiRcAQAAAFAk4QoAAACAIglXAAAAABRJuAIAAACgSMIVAAAAAEUSrgAAAAAoknAFAAAAQJGEKwAAAACKJFwBAAAAUCThCgAAAIAiCVcAAAAAFKm+uxfQnVatWpW77rorDz74YObOnZv58+dn8eLFWbp0aXr37p1hw4Zl//33z7hx43LkkUempqZmi89ZqVRyxx135Oabb86DDz6YhQsXprW1Ndtvv3322muvvOtd78pxxx2XhoaGTvgJAQAAAHqumkqlUunuRXSXRx99NMccc8xG7XvwwQfnsssuy9ChQzf7fIsWLcqkSZPyu9/9br37DR48OF/96ldzxBFHbPa5OsOiRcvT1tberWvYFA0N/VJfX5fW1rY0N6/o7uVAlzH7VCNzTzUy91Qjc0816slzX1dXm8bG/p16zKq+4ipJGhsbM2bMmOy3337ZZZddMmTIkAwaNCjLli3Lww8/nOuvvz6PPvpoZs2alYkTJ+aGG25Inz59Nvk87e3t+bu/+7v8/ve/T5IMGzYs/+f//J/ss88+2W677fLss8/muuuuy3333ZfFixfn05/+dK677rrsu+++nf0jAwAAAPQIVX3FVVtbW2pra9d7C2BLS0smTZqUO++8M0kyZcqUnHzyyZt8rl/84hf59Kc/nSQZOXJkrrvuugwYMOAN+33ta1/Ld7/73STJe9/73vzHf/zHJp+rs7jiCnoGs081MvdUI3NPNTL3VKOePPdb44qrqn44e11d3QafW9WrV6+cccYZHb++9957N+tcs2bN6tieOHHiWqNVknzqU59Kr169kmSDtxQCAAAAbMuqOlxtrP79/1wLly9fvlnHePnllzu2d9555/Wea/DgwVt0LgAAAIBtgXC1EaZOndqxvccee2zWMXbfffeO7fnz569zv+XLl2fx4sVbdC4AAACAbYFwtRZtbW1ZsGBB7rnnnpx99tkdz5zq1atXTjrppM065jHHHNNx5db3v//9112Btab/+q//SktLS5Js1rO0AAAAALYVVf1w9jXNmzcvRx111Dq/PmjQoHzta1/LEUccsdnn+M1vfpOzzjorS5YsyfDhwzNx4sTss88+6devX8enCr72DK1TTz0155133gafwbU1tba2ddu5N0dd3asP2q9UKj3qofKwpcw+1cjcU43MPdXI3FONevrc19fXderxhKs/WVe4qq2tzWmnnZaJEydmyJAhW3ye559/Ptdcc03++7//O6+88sobvn744YfntNNOyzvf+c4tPhcAAABAT1bf3QsoxfDhwzNt2rQkSXt7e5qbmzN79uxce+21+f73v58nnngiF154YYYNG7bZ52hra8u0adNy8803rzVaJa9+kuCgQYMyYsSI9T7EvSu44gp6BrNPNTL3VCNzTzUy91Sjnj73rrjqYi+//HLOPPPM3HPPPRk6dGiuuuqqjBw5cpOPs2rVqnzqU5/Kr3/96yTJBz7wgUyYMCH77LNPevfuneeffz633XZb/uu//isrVqxIQ0NDvv3tb+fAAw/s7B9poy1atLxH/SFpaOiX+vq6tLa2pbl5RXcvB7qM2acamXuqkbmnGpl7qlFPnvu6uto0Nvbv1GN6OPsGDBgwIJdeemn69u2bBQsWZMqUKZt1nMsvv7wjWn3iE5/IZZddlre//e0ZMGBAevfunREjRuSTn/xkrr766vTq1SvNzc35x3/8x6xevbozfxwAAACAHkO42gg77LBDDjrooCTJzJkz89JLL23S91cqlVx33XVJkn79+mXSpEnr3Hf//ffPMccckySZP39+R+wCAAAAqDbC1UZqbGzs2J4/f/4mfe/ChQvT3NycJNl7773Tt2/f9e5/wAEHdGw/9thjm3QuAAAAgG2FcLWRXnjhhY7t/v037X7Nuro/P5istbV1g/uvuU+vXr026VwAAAAA2wrhaiPMmzcvv//975O8eqvfbrvttknf39DQkIEDByZJHn300SxatGi9+997770d27vuuusmrhYAAABg21DV4erGG2/MsmXL1rtPU1NTzjrrrLS0tCRJxo0b94Zb/e67776MGjUqo0aNyoQJE95wjJqamhx11FFJkpaWllx44YXrvPLq1ltvzYwZM5K8emXXYYcdtsk/FwAAAMC2oL67F9CdfvCDH+Siiy7K2LFjM2bMmIwcOTIDBw5Ma2trXnzxxcycOTNTp07NkiVLkiQjRozI5MmTN+tcZ555Zu64444sXbo0t912W8aPH5+TTjop++67b3r16pXnnnsut912W6ZNm5ZKpZIkOeusszJgwIBO+3kBAAAAepKqDldJsnLlykyfPj3Tp09f735HHnlkLr744jQ0NGzWeXbZZZd873vfy1lnnZX58+fnkUceyZQpU9a6b69evXLmmWfmlFNO2axzAQAAAGwLqjpcXX755bnrrrsyZ86cPPHEE2lqasqiRYtSqVSy/fbbZ8SIERk9enTGjRuX0aNHb/H5Ro8enVtuuSU333xz7rjjjjzyyCNpbm5OW1tbBgwYkN133z2HHHJIjj322E1+jhYAAADAtqam8tp9afAXFi1anra29u5exkZraOiX+vq6tLa2pbl5RXcvB7qM2acamXuqkbmnGpl7qlFPnvu6uto0Nvbv1GNW9cPZAQAAACiXcAUAAABAkYQrAAAAAIokXAEAAABQJOEKAAAAgCIJVwAAAAAUSbgCAAAAoEjCFQAAAABFEq4AAAAAKJJwBQAAAECRhCsAAAAAiiRcAQAAAFAk4QoAAACAIglXAAAAABRJuAIAAACgSMIVAAAAAEUSrgAAAAAoknAFAAAAQJGEKwAAAACKJFwBAAAAUCThCgAAAIAiCVcAAAAAFEm4AgAAAKBIwhUAAAAARRKuAAAAACiScAUAAABAkYQrAAAAAIokXAEAAABQJOEKAAAAgCIJVwAAAAAUSbgCAAAAoEjCFQAAAABFEq4AAAAAKJJwBQAAAECRhCsAAAAAiiRcAQAAAFAk4QoAAACAIglXAAAAABRJuAIAAACgSMIVAAAAAEUSrgAAAAAoknAFAAAAQJGEKwAAAACKJFwBAAAAUCThCgAAAIAiCVcAAAAAFEm4AgAAAKBIwhUAAAAARRKuAAAAACiScAUAAABAkYQrAAAAAIokXAEAAABQJOEKAAAAgCIJVwAAAAAUSbgCAAAAoEjCFQAAAABFEq4AAAAAKJJwBQAAAECRhCsAAAAAiiRcAQAAAFAk4QoAAACAIglXAAAAABRJuAIAAACgSMIVAAAAAEUSrgAAAAAoknAFAAAAQJGEKwAAAACKJFwBAAAAUCThCgAAAIAiCVcAAAAAFEm4AgAAAKBIwhUAAAAARRKuAAAAACiScAUAAABAkYQrAAAAAIokXAEAAABQJOEKAAAAgCIJVwAAAAAUSbgCAAAAoEjCFQAAAABFEq4AAAAAKJJwBQAAAECRhCsAAAAAiiRcAQAAAFAk4QoAAACAIglXAAAAABRJuAIAAACgSMIVAAAAAEUSrgAAAAAoknAFAAAAQJGEKwAAAACKJFwBAAAAUCThCgAAAIAiCVcAAAAAFEm4AgAAAKBIwhUAAAAARRKuAAAAACiScAUAAABAkYQrAAAAAIokXAEAAABQJOEKAAAAgCIJVwAAAAAUSbgCAAAAoEjCFQAAAABFEq4AAAAAKJJwBQAAAECRhCsAAAAAiiRcAQAAAFAk4QoAAACAIglXAAAAABRJuAIAAACgSMIVAAAAAEUSrgAAAAAoknAFAAAAQJGEKwAAAACKJFwBAAAAUKT67l5Ad1q1alXuuuuuPPjgg5k7d27mz5+fxYsXZ+nSpendu3eGDRuW/fffP+PGjcuRRx6ZmpqaTjv3ihUrMnXq1Nxxxx157LHH0tTUlL59+6axsTGjRo3KIYcckmOOOSaDBg3qtHMCAAAA9CRVHa6efvrpnHnmmWv9WktLS5588sk8+eSTmTZtWg4++OBcdtllGTp06Baf91e/+lW+8IUv5IUXXnjd769evTpLly7NU089ldtuuy177713Dj300C0+HwAAAEBPVNXhKkkaGxszZsyY7Lffftlll10yZMiQDBo0KMuWLcvDDz+c66+/Po8++mhmzZqViRMn5oYbbkifPn02+3zTpk3Lueeem7a2tgwYMCDHHntsDj300AwbNizt7e2ZP39+Zs2alV/84hed+FMCAAAA9Dw1lUql0t2L6C5tbW2pra1d7y2ALS0tmTRpUu68884kyZQpU3LyySdv1vkeeeSRHHvssWlpackBBxyQb33rW9lhhx3We+5evXpt1rk6w6JFy9PW1t5t599UDQ39Ul9fl9bWtjQ3r+ju5UCXMftUI3NPNTL3VCNzTzXqyXNfV1ebxsb+nXrMqn44e11d3QafW9WrV6+cccYZHb++9957N/t8n//859PS0pLBgwdvMFq9dm4AAACAalXV4Wpj9e//51q4fPnyzTrG7373uzzwwANJko9+9KMbjFYAAAAA1a7qn3G1MaZOndqxvccee2zWMW6++eaO7fe9730d26tWrcqLL76Y3r17Z8iQIa6yAgAAAPgT4Wot2trasmjRojz22GO57rrrcssttyR59da9k046abOOOXv27CRJfX199t5778yePTuXX3557rnnnrS1tSVJtttuuxx22GE5/fTTc/DBB3fODwMAAADQQ1X1w9nXNG/evBx11FHr/PqgQYPyta99LUccccQmH7tSqWS//fZLW1tbGhoa8pnPfCZf/OIX096+9gef19TU5B/+4R/yqU99apPP1ZlaW9u69fybqq7u1QftVyqVHvVQedhSZp9qZO6pRuaeamTuqUY9fe7r6+s69XjC1Z+sK1zV1tbmtNNOy8SJEzNkyJDNOvayZcvy9re/PcmrV221tbWlrq4uf/d3f5cPf/jDGT58eBYuXJibb745l19+eVatWpUk+cpXvpKPfOQjm/0zAQAAAPRkwtWftLS05Mknn0yStLe3p7m5ObNnz861116bhQsX5ogjjsiFF16YYcOGbfKxX3jhhTdc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fvx6r9b60Ic+lKOOOipJ0tzcnP/93//drHMBAAAAbAuqOlxtrP79/1wLly9fvlXP9c53vrNj+6mnntqq5wIAAAAomXC1EaZOndqxvccee2zVc61evbpju66ubqueCwAAAKBkVf9w9rVpa2vLokWL8thjj+W6667LLbfckuTV2wZPOumkrXruNW9F3GuvvbbquQAAAABKVtUPZ1/TvHnzOp4vtTaDBg3K1772tRxxxBFbbQ1z5szJSSedlPb29gwfPjx33HFHevXqtdXOtyGtrW3ddu7NUVf36oP2K5VKj3qoPGwps081MvdUI3NPNTL3VKOePvf19Z1795grrjagtrY2p512WiZOnJghQ4ZstfMsXbo05557btrbXx3KyZMnd2u0Sjp/2LpKTU1Nj107bAmzTzUy91Qjc081MvdUI3P/Kldc/UlLS0uefPLJJEl7e3uam5sze/bsXHvttVm4cGGOOOKIXHjhhRk2bNhWOfcnP/nJ/OY3v0mSHHPMMbn00ks7/TybyhVX0DOYfaqRuacamXuqkbmnGvX0ue/s2CZcbcDLL7+cM888M/fcc0+GDh2aq666KiNHjuy047e1teWcc87J9OnTkyQHH3xwvve972W77bbrtHNsrkWLlveoPyQNDf1SX1+X1ta2NDev6O7lQJcx+1Qjc081MvdUI3NPNerJc19XV5vGxv6dekyfKrgBAwYMyKWXXpq+fftmwYIFmTJlSqcdu729Peeee25HtHrrW9+aK664oohoBQAAANDdhKuNsMMOO+Sggw5KksycOTMvvfTSFh+zra0t5557bqZNm5YkOfDAA/O9730vAwYM2OJjAwAAAGwLhKuN1NjY2LE9f/78LTpWW1tbPve5z+WnP/1pkmT06NGiFQAAAMBf8KmCG+mFF17o2O7ff/Pv12xra8tnP/vZ3HLLLUlejVZXXnlltt9++y1eIwAAAMC2xBVXG2HevHn5/e9/nyTp169fdtttt806zmsPYn8tWh144IGiFQAAAMA6VHW4uvHGG7Ns2bL17tPU1JSzzjorLS0tSZJx48alb9++r9vnvvvuy6hRozJq1KhMmDBhrcdpa2vL5MmTX/cgdtEKAAAAYN2q+lbBH/zgB7nooosyduzYjBkzJiNHjszAgQPT2tqaF198MTNnzszUqVOzZMmSJMmIESMyefLkzTrXOeeck5/9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7P4nmjJvwfKNjlavqVSSGf9vfl5e2bKVVgYAAAB0NuFqI0ydOrVje4899tisY8ycOTNJ0qdPn7ztbW9b537bbbddDjzwwCTJM888kxdeeGGzzretuuN3z671mVYbo1Kp5Nf3P9+5CwIAAAC2GuFqLdra2rJgwYLcc889Ofvss/Pd7343yau3DZ500kmbfLyVK1dm3rx5SZIRI0akd+/e691/r7326th+7DG3t71m0dJX8tBTzdnEi606tFeSO//fvM5dFAAAALDVVP2nCr5m3rx5a33u1GsGDRqUr33ta9lzzz03+djPP/98XnsG/k477bTB/dfc57nnntvk83WWgQP7dtu51+a55pVbfIyFS1/J4MHbbfDZZtCT1P3pQwfq6mrT0NCvm1cDXcPcU43MPdXI3FONzP3rCVcbUFtbm9NOOy0TJ07MkCFDNusYaz4Xa83nZa1LZzxTqzPU19d127nXpnVzL7VaQ6WSpKY29fUuNmTbU1NTU9yfW9jazD3VyNxTjcw91cjcv0q4+pPhw4dn2rRpSZL29vY0Nzdn9uzZufbaa/P9738/TzzxRC688MIMGzZsk4+9atWqju1evXptcP81byVcuXLLrzLaXK2tbd127rXp02vL/8DW19WkJpXifjbYEnV1tampqUmlUklbW3t3Lwe6hLmnGpl7qpG5pxr19Lnv7NgmXP1Jr1698uY3v/l1v/eOd7wjp5xySs4888zccccduf/++3PVVVdl5MiRm3TsPn36dGy3tGz4U+1Wr17dsb3ddttt0rk609KlrxT1h2T73nWpr6tJa9vmXXlVU5OMGL59mptXdPLKoHs1NPRLfX1d2trazTdVw9xTjcw91cjcU4168tzX1dWmsXHDd5ptCvdLbcCAAQNy6aWXpm/fvlmwYEGmTJmyycfY1Fv/Vqz482BuzK2F1aJf3/q8c/8dU7eZHytYqSTvffuunbwqAAAAYGsRrjbCDjvskIMOOihJMnPmzLz00kub9P077bRTx8PAn3/++Q3uv+YD2TfmYe7V5D0H7ZK2zXzWVf++9Tl41NBOXhEAAACwtQhXG6mxsbFje/78+Zv0vdttt1122WWXJMnTTz/9ulsB1+axxx7r2N5777036Vzbut2Gb5937r9jNueiqxOP2jv1dUYeAAAAegrv4jfSCy+80LG9ObfvjRkzJsmrD2qfPXv2OvdbuXJlfv/73ydJdt111+y4446bfK5t3al/vU/esntjajYhXo0/YmT+fwe4eg0AAAB6EuFqI8ybN68jJvXr1y+77bbbJh/jAx/4QMf2tddeu879pk6dmldeeeUN38Of1dfV5jPHjc57375r6mpr1nr11WtRq3/f+pw2bt+Me8fuXbpGAAAAYMtVdbi68cYbs2zZsvXu09TUlLPOOqvj0wDHjRuXvn37vm6f++67L6NGjcqoUaMyYcKEtR7n3e9+d/bbb78kyfTp0zNjxow37DNv3rx8/etfT/JqIDvllFM2+WeqFnW1tTnpqL3z9UmH59gj98rQwX1T+6daVV9Xk5FvGpi/+/B++fqkw11pBQAAAD1UfXcvoDv94Ac/yEUXXZSxY8dmzJgxGTlyZAYOHJjW1ta8+OKLmTlzZqZOnZolS5YkSUaMGJHJkydv1rlqampy4YUXZsKECXnllVcyadKknHLKKRk7dmx69+6dOXPm5IorrsjixYuTJJMnT86wYcM660fdZg3Yrlc+cOhu+cChu2Xw4O2SmtrUpNLjPjIUAAAAeKOqDlfJq8+Umj59eqZPn77e/Y488shcfPHFaWho2OxzjR49Ov/+7/+ez33uc1m8eHGuvPLKXHnlla/bp66uLpMmTcrHPvaxzT5PtaqpqUl9fW1aW9u6eykAAABAJ6jqcHX55Zfnrrvuypw5c/LEE0+kqakpixYtSqVSyfbbb58RI0Zk9OjRGTduXEaPHt0p5zziiCNyyy235Ic//GHuvPPOzJ8/Py0tLRk2bFje8Y535MQTT8xb3vKWTjkXAAAAQE9WU6lUKt29CMq0aNHytLW1d/cyNlpDQ7/U19eltbXNrYJUFbNPNTL3VCNzTzUy91Sjnjz3dXW1aWzs36nHrOqHswMAAABQLuEKAAAAgCIJVwAAAAAUSbgCAAAAoEjCFQAAAABFEq4AAAAAKJJwBQAAAECRhCsAAAAAiiRcAQAAAFAk4QoAAACAIglXAAAAABRJuAIAAACgSMIVAAAAAEUSrgAAAAAoknAFAAAAQJGEKwAAAACKJFwBAAAAUCThCgAAAIAiCVcAAAAAFEm4AgAAAKBI9d29AMpVV1eTnto26+p65rphS5l9qpG5pxqZe6qRuaca9bS5f7UjdK6aSqVS6fSjAgAAAMAW6lnpDgAAAICqIVwBAAAAUCThCgAAAIAiCVcAAAAAFEm4AgAAAKBIwhUAAAAARRKuAAAAACiScAUAAABAkYQrAAAAAIokXAEAAABQJOEKAAAAgCIJVwAAAAAUSbgCAAAAoEjCFQAAAABFEq4AAAAAKJJwBQAAAECRhCsAAAAAiiRcAQAAAFAk4QoAAACAIglXAAAAABRJuAIAAACgSMIVAAAAAEUSrgAAAAAoknAFAAAAQJGEKwAAAACKJFwBAAAAUCThCgAAAIAi1Xf3AqhuL7/8ch5++OE89NBDmTt3bh566KE8+eSTaWtrS5JcddVVOfTQQzv9nNdcc01uv/32PP3001m5cmV22GGHvP3tb89xxx2XMWPGdOr54C915dw/++yzueuuuzJr1qz84Q9/yPPPP5/Vq1enf//+GTlyZA477LAcd9xxedOb3tQp54P16Y7/5v+lxYsX54Mf/GAWLFjQ8Xt/+MMftuo5qW7dNfctLS255ZZb8otf/CJz585NU1NT6uvr09jYmD333DNjxozJBz/4wQwfPrzTzw3dMff33HNPpk6dmjlz5uTFF1/M6tWrM2DAgOyxxx55xzvekeOPPz477bRTp54T1tQdr7ur5b1tTaVSqXT3IqheH/nIR/Lwww+v8+ud/ZfaQw89lEmTJmX+/Pnr3GfChAm54IILUlNT02nnhTV11dyfd955ufHGGze4X58+fXL22Wfn1FNP3eJzwvp09X/z12by5Mm5+eabX/d7whVbU3fM/e9///ucf/75efzxx9e73z//8z/nb//2bzv13JB07dy/8sor+exnP5uf//zn691vu+22yz/90z9l/PjxnXJeWFN3vO6upve2rriiW63ZTfv165d99tknCxcuzDPPPNPp55o3b15OP/30NDU1JUnGjx+fo48+OgMHDszcuXPz3e9+N88++2yuvvrq9OnTJ5/97Gc7fQ2QdN3cv/DCC0mSvn37ZuzYsTnkkEOy1157ZcCAAVmwYEHuuOOO3HDDDVm1alX++Z//OW1tbTnttNM6dQ2wpq78b/7a/PznP8/NN9+cvn37pq6uLsuXL++S81Ldunru77nnnnzqU5/KihUr0rt373zkIx/Ju971ruy4446pqanJiy++mDlz5uT222/fKueHpGvn/nOf+1xHtBo0aFBOOeWUjB49OoMHD85zzz2XW265JT//+c+zcuXKXHDBBWlsbMzYsWM7fR1Ut65+3V1t722FK7rV+PHjM3jw4Oy3337ZY489Ultbm/POO2+r/KX2la98peMP9uc///lMmDCh42ujR4/OBz7wgZxwwgl56qmncuWVV+ZDH/pQRo0a1enrgK6a+2HDhuX888/PsccemwEDBrzh60cccUSOPvronH766Vm9enW+8Y1vZNy4cdlxxx07dR3wmq78b/5fWrRoUS688MIkyVlnnZWrr75auKJLdOXcv/jii/nMZz6TFStWZLfddst3vvOd7L777q/b54ADDsh73/venHPOOVm9enWnrwGSrpv7Rx55JLfddluSpLGxMTfeeOPrXse89hr/Rz/6US666KJUKpVcdtllwhWdrqtfd1fbe1sPZ6dbnXLKKfnQhz6UPffcM7W1W28cH3/88Y5/iXnb2972uj/Yrxk8eHA+//nPJ0na29tzxRVXbLX1UN26au6/+tWv5tRTT13rX56vOeyww3LiiScmSVavXr3By+xhS3TV7K/NRRddlKamphx44IH5+Mc/3qXnprp15dxfcsklWbJkSXr16pX//M//fEO0+ku9e/fequuhenXV3P/ud7/r2D7++OPXGQFOOumkDBs2LEny8MMP+4cLOl1Xvu6uxve2whVV4dZbb+3YPv7449e53+GHH56dd945STJjxoysWrVqq68Nuts73/nOju2nnnqq+xYCW8n06dNz6623pnfv3rnkkku6PJpBV5g/f37H7X/jxo3L3nvv3c0rgq3v5Zdf7th+7TX82tTU1Lzu68IV3aUzXndX43tbr9yoCjNnzuzYPuyww9a5X01NTceDIlesWJEHHnhgq68Nutuat4p4Q8+2pqmpKV/84heTJJ/61Key1157dfOKYOuYPn16xye2ve997+v4/dWrV2fevHl57rnn3BrINmfNqwrX94DqSqXS8fXtt98+Q4YM2dpLg7XqjNfd1fje1jsUqsJjjz2WJOnfv/8GP350zTc1G/o0HtgW3HvvvR3b/oWebc2FF16Y5ubm7Lvvvjn99NO7ezmw1cyePbtje999983jjz+eSZMm5aCDDspRRx2VsWPH5qCDDsopp5ySO++8sxtXCp1n7NixHbcHXnfddXnxxRfXut///M//5KWXXkqSnHjiiamrq+uyNcKaOuN1dzW+t/VwdrZ5q1evzsKFC5MkO+200wb3X3Of5557bqutC0rw7LPP5qabbkry6qf+rPmv9NDTTZs2LT//+c9TX1+fSy65JPX1Xvaw7Xr00Uc7tufMmZPzzz//DbeFtLS05L777st9992XE044IRdddFGP/4h0qlufPn3yrW99K3//93+f559/Psccc0xOOeWUHHjggRk0aFCee+65TJ8+veMB7kcffXT+4R/+oZtXTbXqjNfd1fre1is4tnlr3vvev3//De6/5j7uf2dbtnr16px77rlZsWJFkuT0009PY2NjN68KOseCBQty8cUXJ0k+8YlP5C1veUs3rwi2riVLlnRsn3/++Vm9enVOOeWUnHjiidl1112zZMmS3H777fnGN76RJUuW5Nprr83w4cPz6U9/uhtXDVtu3333zY033pgf//jHufLKK/PNb37zDfsceOCBOe200/JXf/VX3bBC6LzX3dX63tatgmzz1vzXxl69em1w/zU/YWflypVbZU1QgilTpmTWrFlJkkMOOSRnnHFGN68IOs8XvvCFLF68OHvttZc35lSFNd+QrFq1Kp/73OdywQUXZM8990zv3r0zdOjQnHzyybnqqqs6Xut8+9vf7viXe+jJbr/99kybNi2LFy9e69fnzp2bG2+8MY888kjXLgz+pLNed1fre1vhim1enz59OrZbWlo2uP+aD8zbbrvttsqaoLt95StfyU9+8pMkyciRI/ONb3zD8x7YZtx0002ZMWNGamtrc8kll7zuRRtsq9Z8vbPrrrvm1FNPXet+++yzT0444YQkr74Beu0WKuiJKpVKzjvvvPzTP/1T/vjHP+Yd73hHvve97+W3v/1tHnzwwdx5552ZMmVKBg4cmDvvvDMnnnhiZsyY0d3Lpsp05uvuan1vK1yxzRswYEDH9sZcHvna5ZvJxl1+CT3Nv/7rv+bKK69MkowYMSI/+MEPfLoO24wXX3wxX/7yl5MkH//4x3PggQd284qga6z5muXd7373ej+t6sgjj+zYvv/++7fmsmCruvbaa3PjjTcmefX5Vd///vdz+OGHZ+DAgenVq1fe9KY35eSTT86Pf/zjDB48OCtXrsw555yTRYsWdfPKqRad/bq7Wt/besYV27zevXtnyJAhaWpqyvPPP7/B/dd8aN3GPPAOepJ/+7d/yxVXXJHk1b88r7766gwfPrybVwWd56qrrsrSpUvTp0+f7LXXXrnlllvWut+aL+TW3Of973//Rl16D6XZeeeds2DBgiQbfv2y5qdQNTU1bdV1wdb04x//uGP7c5/73Do/bGCXXXbJhAkT8s1vfjPLly/PLbfckgkTJnTVMqlSW+N1d7W+txWuqAp77713mpqasnz58jz33HPr/djQ1z5eNHn9x4dCT3fppZfmO9/5TpJkt912y1VXXSVasc157ZL4VatW5YILLtio7zn77LM7tn/7298KV/RIb37zmzNnzpwkSXt7+3r3XfPrPm2TnuyPf/xjkmSHHXbY4JvyAw44oGN7zdf7sDVszdfd1fje1q2CVIUxY8Z0bN97773r3K9SqeS+++5L8upHlO6///5bfW3QFb761a++7i/Pq6++OjvuuGM3rwqAznLooYd2bD/11FPr3XfNr/sHDHqy18Jra2vrBvddcx//QMHWtLVfd1fje1vhiqrw13/91x3ba15S/Jd+/etfZ/78+Uleff5D3759t/raYGv7yle+ku9973tJ/nyZsmjFtuqCCy7IH/7whw3+z84779zxPWv+/sCBA7tx9bD5xo4d2/Hg3V/+8pev++Spv/Szn/2sY3vN4AU9za677pokWbx48QY/MXDNN/ivfR90tq543V2N722FK3q8efPmZdSoURk1alTe8573rHWfPffcM+9973uTJLNnz84Pf/jDN+yzePHiXHzxxUmS2trazf6IUugKGzP3yat/eb72QMjdd99dtKLH29jZh23Jxsx9//79Oz5JcNGiRR0fUvCX7rjjjo7nuu20004dr4+gNBsz9+973/s6ti+66KLXPb9wTbNmzcq1116bJKmrq8vYsWM7f8FUvc543e297dq5qZ1u9fTTT2fWrFlv+L3X3H333R2V+DV/+7d/u1nnOu+88zJr1qw0NzfnS1/6Uh5++OGMGzcuAwYMyCOPPJIrrrgizz77bJLk1FNPzT777LNZ54EN6aq5v/TSSzv+8hw0aFD+6Z/+KUuWLMmSJUvW+T3bbbedf4Vkq+nK/+ZDKbpy7j/5yU/ml7/8ZR5++OFce+21efbZZ3PCCSdkt912y5IlS3L77bfn2muvTaVSSV1dXb785S+nd+/em3UuWJ+umvtTTz01P/nJT/Lcc8/l//2//5cPfehD+djHPpYDDjgg/fr1y0svvZRf/vKXue6669LS0pIkmTBhQnbbbbfN+Klg3br6dXe1vbetqVQqle5eBNXrJz/5Sc4///xN+p4//OEPr/v1vHnzctRRRyV59RN1ZsyYsc7vfeCBBzJp0qT1fgLDySefnC984Qvr/FQS2FJdNffvec973vCicEMOOeSQXH311Zv0PbCxuvq/+euz5p+PvzwHdKaunvuFCxfmzDPPzOzZs9e5z4ABA/LVr36145jQ2bpy7p9++ulMmjRpg/8tr6mpyUc/+tFccMEFqa114xGdq7Ned3tvu3auuKKqHHDAAbn55pvzox/9KLfffnueeeaZrFixIkOHDs1BBx2U448/Poccckh3LxMAYLPssMMO+dGPfpSbb745t9xySx5++OEsWrQo2223XXbfffe8+93vzkc/+tE0NjZ291KhU4wYMSI33HBDbr/99tx6662ZO3dumpqasnr16vTv3z+77LJLDjrooBx77LE9/qoTWFM1vbd1xRUAAAAARXKNJAAAAABFEq4AAAAAKJJwBQAAAECRhCsAAAAAiiRcAQAAAFAk4QoAAACAIglXAAAAABRJuAIAAACgSMIVAAAAAEUSrgAAAAAoknAFAAAAQJGEKwAAAACKJFwBAAAAUCThCgAAAIAiCVcAAAAAFEm4AgAAAKBI9d29AAAAtl3Lli3L3Llz8+CDD+ahhx7KQw89lKeffjqVSiVJ8s///M/527/9225eJQBQKuEKAICt4le/+lXOOOOMjkgFALCp3CoIAMBW0dLS8oZo1bdv3/Tt27ebVgQA9DSuuAIAYKvo3bt33vrWt2b//ffPfvvtl/322y977bVXTj311MycObO7lwcA9ADCFQAAW8W73/3uvPvd7+7uZQAAPZhbBQEAthGPPvpoRo8enVGjRmXffffNPffcs97977///uy///4ZNWpU9ttvv8yZM6drFgoAsJGEKwCAbcSb3/zmnHvuuUmS9vb2fO5zn0tzc/Na93355ZczefLktLS0JEkmTZqUt771rV21VACAjSJcAQBsQz760Y/mqKOOSpK89NJLOf/889e630UXXZRnnnkmSXLIIYfkk5/8ZJetEQBgYwlXAADbmC9/+csZPnx4kuTOO+/MD3/4w9d9/aabbspPf/rTJMngwYNz6aWXprbWy0IAoDxeoQAAbGMaGhryta99rSNGffWrX80jjzySJHn66afzxS9+sWPfNSMXAEBphCsAgG3QoYce2nH736pVqzJ58uQsW7YskydPzvLly5MkJ554Yt773vd25zIBANZLuAIA2EZNmjQpb3vb25Ikjz32WD70oQ/lgQceSJLstdde63z+FQBAKYQrAIBtVH19fS699NJsv/32SZLnnnsuSdKnT5/827/9W/r27dudywMA2CDhCgBgG7bLLru84RMDzzzzzIwaNaqbVgQAsPGEKwCAbdjSpUtzzTXXvO737r777rS3t3fTigAANp5wBQCwDfv85z/fcYtgTU1NkmTmzJn59re/3Z3LAgDYKMIVAMA26rrrrsttt92WJBk6dGi+/e1vp1evXkmSyy+/PHPmzOnG1QEAbJhwBQCwDXriiSdyySWXJHn1Sqt/+Zd/yRFHHJHPfOYzSZLW1tZMnjw5L7/8cncuEwBgvYQrAIBtzOrVqzN58uSsWLEiSTJx4sQcfvjhSZJPfOITeec735kkmTdvXi688MLuWiYAwAYJVwAA25h//dd/zdy5c5Mk++23X/7xH/+x42s1NTX5yle+koaGhiTJtGnTctNNN3XHMgEANqimUqlUunsRAAB0jrvvvjunn356KpVK+vXrlxtuuCEjR458w34zZszI3//93ydJ+vfvn5tuuim77bZbp6/nwgsvzKJFi173ezNnzkxzc3OSZP/998/OO+/8uq8feuih+ehHP9rpawEAep767l4AAACdo6mpKeedd15e+3fJ/+//+//WGq2S5D3veU9OPvnk/OhHP8ry5cszefLkXHPNNamv79yXh3fddVfmz5+/zq8/+OCDefDBB1/3e/369evUNQAAPZdbBQEAtgGVSiXnnXdeFi5cmCT5q7/6qxx33HHr/Z7zzjsvb37zm5Mk999/fy677LKtvk4AgE3hVkEAAAAAiuSKKwAAAACKJFwBAAAAUCThCgAAAIAiCVcAAAAAFKlzP+8YAIAe6/nnn8/06dO36Bjvfve7s/fee3fSigCAaidcAQCQJHnmmWfy1a9+dYuO0dDQIFwBAJ3GrYIAAAAAFKmmUqlUunsRAAAAAPCXXHEFAAAAQJGEKwAAAACKJFwBAAAAUCThCgAAAIAiCVcAAAAAFEm4AgAAAKBIwhUAAAAARRKuAAAAACiScAUAAABAkYQrAAAAAIokXAEAAABQJOEKAAAAgCIJVwAAAAAUSbgCAAAAoEjCFQAAAABFEq4AAAAAKJJwBQAAAECR/v8tiXpCgXvFdAAAAABJRU5ErkJggg==",
                         "text/plain": [
                             "%% Creator: Matplotlib, PGF backend\n",
                             "%%\n",
                             "%% To include the figure in your LaTeX document, write\n",
                             "%%   \\input{<filename>.pgf}\n",
                             "%%\n",
                             "%% Make sure the required packages are loaded in your preamble\n",
@@ -44,17 +48,14 @@
                             "%%   \\import{<path to file>}{<filename>.pgf}\n",
                             "%%\n",
                             "%% Matplotlib used the following preamble\n",
                             "%%   \\def\\mathdefault#1{#1}\n",
                             "%%   \\everymath=\\expandafter{\\the\\everymath\\displaystyle}\n",
                             "%%   \n",
                             "%%   \\usepackage{fontspec}\n",
-                            "%%   \\setmainfont{DejaVuSerif.ttf}[Path=\\detokenize{/workspaces/panpdf/.hatch/test.py3.12/lib/python3.12/site-packages/matplotlib/mpl-data/fonts/ttf/}]\n",
-                            "%%   \\setsansfont{DejaVuSans.ttf}[Path=\\detokenize{/workspaces/panpdf/.hatch/test.py3.12/lib/python3.12/site-packages/matplotlib/mpl-data/fonts/ttf/}]\n",
-                            "%%   \\setmonofont{DejaVuSansMono.ttf}[Path=\\detokenize{/workspaces/panpdf/.hatch/test.py3.12/lib/python3.12/site-packages/matplotlib/mpl-data/fonts/ttf/}]\n",
                             "%%   \\makeatletter\\@ifpackageloaded{underscore}{}{\\usepackage[strings]{underscore}}\\makeatother\n",
                             "%%\n",
                             "\\begingroup%\n",
                             "\\makeatletter%\n",
                             "\\begin{pgfpicture}%\n",
                             "\\pgfpathrectangle{\\pgfpointorigin}{\\pgfqpoint{6.240000in}{4.640000in}}%\n",
                             "\\pgfusepath{use as bounding box, clip}%\n",
@@ -81,376 +82,383 @@
                             "\\definecolor{currentfill}{rgb}{0.917647,0.917647,0.949020}%\n",
                             "\\pgfsetfillcolor{currentfill}%\n",
                             "\\pgfsetlinewidth{0.000000pt}%\n",
                             "\\definecolor{currentstroke}{rgb}{0.000000,0.000000,0.000000}%\n",
                             "\\pgfsetstrokecolor{currentstroke}%\n",
                             "\\pgfsetstrokeopacity{0.000000}%\n",
                             "\\pgfsetdash{}{0pt}%\n",
-                            "\\pgfpathmoveto{\\pgfqpoint{0.691763in}{0.596649in}}%\n",
-                            "\\pgfpathlineto{\\pgfqpoint{6.140000in}{0.596649in}}%\n",
+                            "\\pgfpathmoveto{\\pgfqpoint{0.626778in}{0.571166in}}%\n",
+                            "\\pgfpathlineto{\\pgfqpoint{6.140000in}{0.571166in}}%\n",
                             "\\pgfpathlineto{\\pgfqpoint{6.140000in}{4.540000in}}%\n",
-                            "\\pgfpathlineto{\\pgfqpoint{0.691763in}{4.540000in}}%\n",
-                            "\\pgfpathlineto{\\pgfqpoint{0.691763in}{0.596649in}}%\n",
+                            "\\pgfpathlineto{\\pgfqpoint{0.626778in}{4.540000in}}%\n",
+                            "\\pgfpathlineto{\\pgfqpoint{0.626778in}{0.571166in}}%\n",
                             "\\pgfpathclose%\n",
                             "\\pgfusepath{fill}%\n",
                             "\\end{pgfscope}%\n",
                             "\\begin{pgfscope}%\n",
-                            "\\pgfpathrectangle{\\pgfqpoint{0.691763in}{0.596649in}}{\\pgfqpoint{5.448237in}{3.943351in}}%\n",
+                            "\\pgfpathrectangle{\\pgfqpoint{0.626778in}{0.571166in}}{\\pgfqpoint{5.513222in}{3.968834in}}%\n",
                             "\\pgfusepath{clip}%\n",
                             "\\pgfsetroundcap%\n",
                             "\\pgfsetroundjoin%\n",
                             "\\pgfsetlinewidth{1.003750pt}%\n",
                             "\\definecolor{currentstroke}{rgb}{1.000000,1.000000,1.000000}%\n",
                             "\\pgfsetstrokecolor{currentstroke}%\n",
                             "\\pgfsetdash{}{0pt}%\n",
-                            "\\pgfpathmoveto{\\pgfqpoint{0.939410in}{0.596649in}}%\n",
-                            "\\pgfpathlineto{\\pgfqpoint{0.939410in}{4.540000in}}%\n",
+                            "\\pgfpathmoveto{\\pgfqpoint{0.877379in}{0.571166in}}%\n",
+                            "\\pgfpathlineto{\\pgfqpoint{0.877379in}{4.540000in}}%\n",
                             "\\pgfusepath{stroke}%\n",
                             "\\end{pgfscope}%\n",
                             "\\begin{pgfscope}%\n",
                             "\\definecolor{textcolor}{rgb}{0.150000,0.150000,0.150000}%\n",
                             "\\pgfsetstrokecolor{textcolor}%\n",
                             "\\pgfsetfillcolor{textcolor}%\n",
-                            "\\pgftext[x=0.939410in,y=0.464705in,,top]{\\color{textcolor}{\\sffamily\\fontsize{11.000000}{13.200000}\\selectfont\\catcode`\\^=\\active\\def^{\\ifmmode\\sp\\else\\^{}\\fi}\\catcode`\\%=\\active\\def%{\\%}1.0}}%\n",
+                            "\\pgftext[x=0.877379in,y=0.439222in,,top]{\\color{textcolor}{\\sffamily\\fontsize{11.000000}{13.200000}\\selectfont\\catcode`\\^=\\active\\def^{\\ifmmode\\sp\\else\\^{}\\fi}\\catcode`\\%=\\active\\def%{\\%}1.0}}%\n",
                             "\\end{pgfscope}%\n",
                             "\\begin{pgfscope}%\n",
-                            "\\pgfpathrectangle{\\pgfqpoint{0.691763in}{0.596649in}}{\\pgfqpoint{5.448237in}{3.943351in}}%\n",
+                            "\\pgfpathrectangle{\\pgfqpoint{0.626778in}{0.571166in}}{\\pgfqpoint{5.513222in}{3.968834in}}%\n",
                             "\\pgfusepath{clip}%\n",
                             "\\pgfsetroundcap%\n",
                             "\\pgfsetroundjoin%\n",
                             "\\pgfsetlinewidth{1.003750pt}%\n",
                             "\\definecolor{currentstroke}{rgb}{1.000000,1.000000,1.000000}%\n",
                             "\\pgfsetstrokecolor{currentstroke}%\n",
                             "\\pgfsetdash{}{0pt}%\n",
-                            "\\pgfpathmoveto{\\pgfqpoint{1.929999in}{0.596649in}}%\n",
-                            "\\pgfpathlineto{\\pgfqpoint{1.929999in}{4.540000in}}%\n",
+                            "\\pgfpathmoveto{\\pgfqpoint{1.879783in}{0.571166in}}%\n",
+                            "\\pgfpathlineto{\\pgfqpoint{1.879783in}{4.540000in}}%\n",
                             "\\pgfusepath{stroke}%\n",
                             "\\end{pgfscope}%\n",
                             "\\begin{pgfscope}%\n",
                             "\\definecolor{textcolor}{rgb}{0.150000,0.150000,0.150000}%\n",
                             "\\pgfsetstrokecolor{textcolor}%\n",
                             "\\pgfsetfillcolor{textcolor}%\n",
-                            "\\pgftext[x=1.929999in,y=0.464705in,,top]{\\color{textcolor}{\\sffamily\\fontsize{11.000000}{13.200000}\\selectfont\\catcode`\\^=\\active\\def^{\\ifmmode\\sp\\else\\^{}\\fi}\\catcode`\\%=\\active\\def%{\\%}1.2}}%\n",
+                            "\\pgftext[x=1.879783in,y=0.439222in,,top]{\\color{textcolor}{\\sffamily\\fontsize{11.000000}{13.200000}\\selectfont\\catcode`\\^=\\active\\def^{\\ifmmode\\sp\\else\\^{}\\fi}\\catcode`\\%=\\active\\def%{\\%}1.2}}%\n",
                             "\\end{pgfscope}%\n",
                             "\\begin{pgfscope}%\n",
-                            "\\pgfpathrectangle{\\pgfqpoint{0.691763in}{0.596649in}}{\\pgfqpoint{5.448237in}{3.943351in}}%\n",
+                            "\\pgfpathrectangle{\\pgfqpoint{0.626778in}{0.571166in}}{\\pgfqpoint{5.513222in}{3.968834in}}%\n",
                             "\\pgfusepath{clip}%\n",
                             "\\pgfsetroundcap%\n",
                             "\\pgfsetroundjoin%\n",
                             "\\pgfsetlinewidth{1.003750pt}%\n",
                             "\\definecolor{currentstroke}{rgb}{1.000000,1.000000,1.000000}%\n",
                             "\\pgfsetstrokecolor{currentstroke}%\n",
                             "\\pgfsetdash{}{0pt}%\n",
-                            "\\pgfpathmoveto{\\pgfqpoint{2.920587in}{0.596649in}}%\n",
-                            "\\pgfpathlineto{\\pgfqpoint{2.920587in}{4.540000in}}%\n",
+                            "\\pgfpathmoveto{\\pgfqpoint{2.882187in}{0.571166in}}%\n",
+                            "\\pgfpathlineto{\\pgfqpoint{2.882187in}{4.540000in}}%\n",
                             "\\pgfusepath{stroke}%\n",
                             "\\end{pgfscope}%\n",
                             "\\begin{pgfscope}%\n",
                             "\\definecolor{textcolor}{rgb}{0.150000,0.150000,0.150000}%\n",
                             "\\pgfsetstrokecolor{textcolor}%\n",
                             "\\pgfsetfillcolor{textcolor}%\n",
-                            "\\pgftext[x=2.920587in,y=0.464705in,,top]{\\color{textcolor}{\\sffamily\\fontsize{11.000000}{13.200000}\\selectfont\\catcode`\\^=\\active\\def^{\\ifmmode\\sp\\else\\^{}\\fi}\\catcode`\\%=\\active\\def%{\\%}1.4}}%\n",
+                            "\\pgftext[x=2.882187in,y=0.439222in,,top]{\\color{textcolor}{\\sffamily\\fontsize{11.000000}{13.200000}\\selectfont\\catcode`\\^=\\active\\def^{\\ifmmode\\sp\\else\\^{}\\fi}\\catcode`\\%=\\active\\def%{\\%}1.4}}%\n",
                             "\\end{pgfscope}%\n",
                             "\\begin{pgfscope}%\n",
-                            "\\pgfpathrectangle{\\pgfqpoint{0.691763in}{0.596649in}}{\\pgfqpoint{5.448237in}{3.943351in}}%\n",
+                            "\\pgfpathrectangle{\\pgfqpoint{0.626778in}{0.571166in}}{\\pgfqpoint{5.513222in}{3.968834in}}%\n",
                             "\\pgfusepath{clip}%\n",
                             "\\pgfsetroundcap%\n",
                             "\\pgfsetroundjoin%\n",
                             "\\pgfsetlinewidth{1.003750pt}%\n",
                             "\\definecolor{currentstroke}{rgb}{1.000000,1.000000,1.000000}%\n",
                             "\\pgfsetstrokecolor{currentstroke}%\n",
                             "\\pgfsetdash{}{0pt}%\n",
-                            "\\pgfpathmoveto{\\pgfqpoint{3.911176in}{0.596649in}}%\n",
-                            "\\pgfpathlineto{\\pgfqpoint{3.911176in}{4.540000in}}%\n",
+                            "\\pgfpathmoveto{\\pgfqpoint{3.884591in}{0.571166in}}%\n",
+                            "\\pgfpathlineto{\\pgfqpoint{3.884591in}{4.540000in}}%\n",
                             "\\pgfusepath{stroke}%\n",
                             "\\end{pgfscope}%\n",
                             "\\begin{pgfscope}%\n",
                             "\\definecolor{textcolor}{rgb}{0.150000,0.150000,0.150000}%\n",
                             "\\pgfsetstrokecolor{textcolor}%\n",
                             "\\pgfsetfillcolor{textcolor}%\n",
-                            "\\pgftext[x=3.911176in,y=0.464705in,,top]{\\color{textcolor}{\\sffamily\\fontsize{11.000000}{13.200000}\\selectfont\\catcode`\\^=\\active\\def^{\\ifmmode\\sp\\else\\^{}\\fi}\\catcode`\\%=\\active\\def%{\\%}1.6}}%\n",
+                            "\\pgftext[x=3.884591in,y=0.439222in,,top]{\\color{textcolor}{\\sffamily\\fontsize{11.000000}{13.200000}\\selectfont\\catcode`\\^=\\active\\def^{\\ifmmode\\sp\\else\\^{}\\fi}\\catcode`\\%=\\active\\def%{\\%}1.6}}%\n",
                             "\\end{pgfscope}%\n",
                             "\\begin{pgfscope}%\n",
-                            "\\pgfpathrectangle{\\pgfqpoint{0.691763in}{0.596649in}}{\\pgfqpoint{5.448237in}{3.943351in}}%\n",
+                            "\\pgfpathrectangle{\\pgfqpoint{0.626778in}{0.571166in}}{\\pgfqpoint{5.513222in}{3.968834in}}%\n",
                             "\\pgfusepath{clip}%\n",
                             "\\pgfsetroundcap%\n",
                             "\\pgfsetroundjoin%\n",
                             "\\pgfsetlinewidth{1.003750pt}%\n",
                             "\\definecolor{currentstroke}{rgb}{1.000000,1.000000,1.000000}%\n",
                             "\\pgfsetstrokecolor{currentstroke}%\n",
                             "\\pgfsetdash{}{0pt}%\n",
-                            "\\pgfpathmoveto{\\pgfqpoint{4.901764in}{0.596649in}}%\n",
-                            "\\pgfpathlineto{\\pgfqpoint{4.901764in}{4.540000in}}%\n",
+                            "\\pgfpathmoveto{\\pgfqpoint{4.886995in}{0.571166in}}%\n",
+                            "\\pgfpathlineto{\\pgfqpoint{4.886995in}{4.540000in}}%\n",
                             "\\pgfusepath{stroke}%\n",
                             "\\end{pgfscope}%\n",
                             "\\begin{pgfscope}%\n",
                             "\\definecolor{textcolor}{rgb}{0.150000,0.150000,0.150000}%\n",
                             "\\pgfsetstrokecolor{textcolor}%\n",
                             "\\pgfsetfillcolor{textcolor}%\n",
-                            "\\pgftext[x=4.901764in,y=0.464705in,,top]{\\color{textcolor}{\\sffamily\\fontsize{11.000000}{13.200000}\\selectfont\\catcode`\\^=\\active\\def^{\\ifmmode\\sp\\else\\^{}\\fi}\\catcode`\\%=\\active\\def%{\\%}1.8}}%\n",
+                            "\\pgftext[x=4.886995in,y=0.439222in,,top]{\\color{textcolor}{\\sffamily\\fontsize{11.000000}{13.200000}\\selectfont\\catcode`\\^=\\active\\def^{\\ifmmode\\sp\\else\\^{}\\fi}\\catcode`\\%=\\active\\def%{\\%}1.8}}%\n",
                             "\\end{pgfscope}%\n",
                             "\\begin{pgfscope}%\n",
-                            "\\pgfpathrectangle{\\pgfqpoint{0.691763in}{0.596649in}}{\\pgfqpoint{5.448237in}{3.943351in}}%\n",
+                            "\\pgfpathrectangle{\\pgfqpoint{0.626778in}{0.571166in}}{\\pgfqpoint{5.513222in}{3.968834in}}%\n",
                             "\\pgfusepath{clip}%\n",
                             "\\pgfsetroundcap%\n",
                             "\\pgfsetroundjoin%\n",
                             "\\pgfsetlinewidth{1.003750pt}%\n",
                             "\\definecolor{currentstroke}{rgb}{1.000000,1.000000,1.000000}%\n",
                             "\\pgfsetstrokecolor{currentstroke}%\n",
                             "\\pgfsetdash{}{0pt}%\n",
-                            "\\pgfpathmoveto{\\pgfqpoint{5.892353in}{0.596649in}}%\n",
-                            "\\pgfpathlineto{\\pgfqpoint{5.892353in}{4.540000in}}%\n",
+                            "\\pgfpathmoveto{\\pgfqpoint{5.889399in}{0.571166in}}%\n",
+                            "\\pgfpathlineto{\\pgfqpoint{5.889399in}{4.540000in}}%\n",
                             "\\pgfusepath{stroke}%\n",
                             "\\end{pgfscope}%\n",
                             "\\begin{pgfscope}%\n",
                             "\\definecolor{textcolor}{rgb}{0.150000,0.150000,0.150000}%\n",
                             "\\pgfsetstrokecolor{textcolor}%\n",
                             "\\pgfsetfillcolor{textcolor}%\n",
-                            "\\pgftext[x=5.892353in,y=0.464705in,,top]{\\color{textcolor}{\\sffamily\\fontsize{11.000000}{13.200000}\\selectfont\\catcode`\\^=\\active\\def^{\\ifmmode\\sp\\else\\^{}\\fi}\\catcode`\\%=\\active\\def%{\\%}2.0}}%\n",
+                            "\\pgftext[x=5.889399in,y=0.439222in,,top]{\\color{textcolor}{\\sffamily\\fontsize{11.000000}{13.200000}\\selectfont\\catcode`\\^=\\active\\def^{\\ifmmode\\sp\\else\\^{}\\fi}\\catcode`\\%=\\active\\def%{\\%}2.0}}%\n",
                             "\\end{pgfscope}%\n",
                             "\\begin{pgfscope}%\n",
                             "\\definecolor{textcolor}{rgb}{0.150000,0.150000,0.150000}%\n",
                             "\\pgfsetstrokecolor{textcolor}%\n",
                             "\\pgfsetfillcolor{textcolor}%\n",
-                            "\\pgftext[x=3.415881in,y=0.261295in,,top]{\\color{textcolor}{\\sffamily\\fontsize{12.000000}{14.400000}\\selectfont\\catcode`\\^=\\active\\def^{\\ifmmode\\sp\\else\\^{}\\fi}\\catcode`\\%=\\active\\def%{\\%}X}}%\n",
+                            "\\pgftext[x=3.383389in,y=0.248000in,,top]{\\color{textcolor}{\\sffamily\\fontsize{12.000000}{14.400000}\\selectfont\\catcode`\\^=\\active\\def^{\\ifmmode\\sp\\else\\^{}\\fi}\\catcode`\\%=\\active\\def%{\\%}x_1}}%\n",
                             "\\end{pgfscope}%\n",
                             "\\begin{pgfscope}%\n",
-                            "\\pgfpathrectangle{\\pgfqpoint{0.691763in}{0.596649in}}{\\pgfqpoint{5.448237in}{3.943351in}}%\n",
+                            "\\pgfpathrectangle{\\pgfqpoint{0.626778in}{0.571166in}}{\\pgfqpoint{5.513222in}{3.968834in}}%\n",
                             "\\pgfusepath{clip}%\n",
                             "\\pgfsetroundcap%\n",
                             "\\pgfsetroundjoin%\n",
                             "\\pgfsetlinewidth{1.003750pt}%\n",
                             "\\definecolor{currentstroke}{rgb}{1.000000,1.000000,1.000000}%\n",
                             "\\pgfsetstrokecolor{currentstroke}%\n",
                             "\\pgfsetdash{}{0pt}%\n",
-                            "\\pgfpathmoveto{\\pgfqpoint{0.691763in}{0.775893in}}%\n",
-                            "\\pgfpathlineto{\\pgfqpoint{6.140000in}{0.775893in}}%\n",
+                            "\\pgfpathmoveto{\\pgfqpoint{0.626778in}{0.751568in}}%\n",
+                            "\\pgfpathlineto{\\pgfqpoint{6.140000in}{0.751568in}}%\n",
                             "\\pgfusepath{stroke}%\n",
                             "\\end{pgfscope}%\n",
                             "\\begin{pgfscope}%\n",
                             "\\definecolor{textcolor}{rgb}{0.150000,0.150000,0.150000}%\n",
                             "\\pgfsetstrokecolor{textcolor}%\n",
                             "\\pgfsetfillcolor{textcolor}%\n",
-                            "\\pgftext[x=0.316851in, y=0.717855in, left, base]{\\color{textcolor}{\\sffamily\\fontsize{11.000000}{13.200000}\\selectfont\\catcode`\\^=\\active\\def^{\\ifmmode\\sp\\else\\^{}\\fi}\\catcode`\\%=\\active\\def%{\\%}3.0}}%\n",
+                            "\\pgftext[x=0.303555in, y=0.698554in, left, base]{\\color{textcolor}{\\sffamily\\fontsize{11.000000}{13.200000}\\selectfont\\catcode`\\^=\\active\\def^{\\ifmmode\\sp\\else\\^{}\\fi}\\catcode`\\%=\\active\\def%{\\%}3.0}}%\n",
                             "\\end{pgfscope}%\n",
                             "\\begin{pgfscope}%\n",
-                            "\\pgfpathrectangle{\\pgfqpoint{0.691763in}{0.596649in}}{\\pgfqpoint{5.448237in}{3.943351in}}%\n",
+                            "\\pgfpathrectangle{\\pgfqpoint{0.626778in}{0.571166in}}{\\pgfqpoint{5.513222in}{3.968834in}}%\n",
                             "\\pgfusepath{clip}%\n",
                             "\\pgfsetroundcap%\n",
                             "\\pgfsetroundjoin%\n",
                             "\\pgfsetlinewidth{1.003750pt}%\n",
                             "\\definecolor{currentstroke}{rgb}{1.000000,1.000000,1.000000}%\n",
                             "\\pgfsetstrokecolor{currentstroke}%\n",
                             "\\pgfsetdash{}{0pt}%\n",
-                            "\\pgfpathmoveto{\\pgfqpoint{0.691763in}{1.492865in}}%\n",
-                            "\\pgfpathlineto{\\pgfqpoint{6.140000in}{1.492865in}}%\n",
+                            "\\pgfpathmoveto{\\pgfqpoint{0.626778in}{1.473174in}}%\n",
+                            "\\pgfpathlineto{\\pgfqpoint{6.140000in}{1.473174in}}%\n",
                             "\\pgfusepath{stroke}%\n",
                             "\\end{pgfscope}%\n",
                             "\\begin{pgfscope}%\n",
                             "\\definecolor{textcolor}{rgb}{0.150000,0.150000,0.150000}%\n",
                             "\\pgfsetstrokecolor{textcolor}%\n",
                             "\\pgfsetfillcolor{textcolor}%\n",
-                            "\\pgftext[x=0.316851in, y=1.434828in, left, base]{\\color{textcolor}{\\sffamily\\fontsize{11.000000}{13.200000}\\selectfont\\catcode`\\^=\\active\\def^{\\ifmmode\\sp\\else\\^{}\\fi}\\catcode`\\%=\\active\\def%{\\%}3.2}}%\n",
+                            "\\pgftext[x=0.303555in, y=1.420160in, left, base]{\\color{textcolor}{\\sffamily\\fontsize{11.000000}{13.200000}\\selectfont\\catcode`\\^=\\active\\def^{\\ifmmode\\sp\\else\\^{}\\fi}\\catcode`\\%=\\active\\def%{\\%}3.2}}%\n",
                             "\\end{pgfscope}%\n",
                             "\\begin{pgfscope}%\n",
-                            "\\pgfpathrectangle{\\pgfqpoint{0.691763in}{0.596649in}}{\\pgfqpoint{5.448237in}{3.943351in}}%\n",
+                            "\\pgfpathrectangle{\\pgfqpoint{0.626778in}{0.571166in}}{\\pgfqpoint{5.513222in}{3.968834in}}%\n",
                             "\\pgfusepath{clip}%\n",
                             "\\pgfsetroundcap%\n",
                             "\\pgfsetroundjoin%\n",
                             "\\pgfsetlinewidth{1.003750pt}%\n",
                             "\\definecolor{currentstroke}{rgb}{1.000000,1.000000,1.000000}%\n",
                             "\\pgfsetstrokecolor{currentstroke}%\n",
                             "\\pgfsetdash{}{0pt}%\n",
-                            "\\pgfpathmoveto{\\pgfqpoint{0.691763in}{2.209838in}}%\n",
-                            "\\pgfpathlineto{\\pgfqpoint{6.140000in}{2.209838in}}%\n",
+                            "\\pgfpathmoveto{\\pgfqpoint{0.626778in}{2.194780in}}%\n",
+                            "\\pgfpathlineto{\\pgfqpoint{6.140000in}{2.194780in}}%\n",
                             "\\pgfusepath{stroke}%\n",
                             "\\end{pgfscope}%\n",
                             "\\begin{pgfscope}%\n",
                             "\\definecolor{textcolor}{rgb}{0.150000,0.150000,0.150000}%\n",
                             "\\pgfsetstrokecolor{textcolor}%\n",
                             "\\pgfsetfillcolor{textcolor}%\n",
-                            "\\pgftext[x=0.316851in, y=2.151801in, left, base]{\\color{textcolor}{\\sffamily\\fontsize{11.000000}{13.200000}\\selectfont\\catcode`\\^=\\active\\def^{\\ifmmode\\sp\\else\\^{}\\fi}\\catcode`\\%=\\active\\def%{\\%}3.4}}%\n",
+                            "\\pgftext[x=0.303555in, y=2.141766in, left, base]{\\color{textcolor}{\\sffamily\\fontsize{11.000000}{13.200000}\\selectfont\\catcode`\\^=\\active\\def^{\\ifmmode\\sp\\else\\^{}\\fi}\\catcode`\\%=\\active\\def%{\\%}3.4}}%\n",
                             "\\end{pgfscope}%\n",
                             "\\begin{pgfscope}%\n",
-                            "\\pgfpathrectangle{\\pgfqpoint{0.691763in}{0.596649in}}{\\pgfqpoint{5.448237in}{3.943351in}}%\n",
+                            "\\pgfpathrectangle{\\pgfqpoint{0.626778in}{0.571166in}}{\\pgfqpoint{5.513222in}{3.968834in}}%\n",
                             "\\pgfusepath{clip}%\n",
                             "\\pgfsetroundcap%\n",
                             "\\pgfsetroundjoin%\n",
                             "\\pgfsetlinewidth{1.003750pt}%\n",
                             "\\definecolor{currentstroke}{rgb}{1.000000,1.000000,1.000000}%\n",
                             "\\pgfsetstrokecolor{currentstroke}%\n",
                             "\\pgfsetdash{}{0pt}%\n",
-                            "\\pgfpathmoveto{\\pgfqpoint{0.691763in}{2.926811in}}%\n",
-                            "\\pgfpathlineto{\\pgfqpoint{6.140000in}{2.926811in}}%\n",
+                            "\\pgfpathmoveto{\\pgfqpoint{0.626778in}{2.916386in}}%\n",
+                            "\\pgfpathlineto{\\pgfqpoint{6.140000in}{2.916386in}}%\n",
                             "\\pgfusepath{stroke}%\n",
                             "\\end{pgfscope}%\n",
                             "\\begin{pgfscope}%\n",
                             "\\definecolor{textcolor}{rgb}{0.150000,0.150000,0.150000}%\n",
                             "\\pgfsetstrokecolor{textcolor}%\n",
                             "\\pgfsetfillcolor{textcolor}%\n",
-                            "\\pgftext[x=0.316851in, y=2.868773in, left, base]{\\color{textcolor}{\\sffamily\\fontsize{11.000000}{13.200000}\\selectfont\\catcode`\\^=\\active\\def^{\\ifmmode\\sp\\else\\^{}\\fi}\\catcode`\\%=\\active\\def%{\\%}3.6}}%\n",
+                            "\\pgftext[x=0.303555in, y=2.863372in, left, base]{\\color{textcolor}{\\sffamily\\fontsize{11.000000}{13.200000}\\selectfont\\catcode`\\^=\\active\\def^{\\ifmmode\\sp\\else\\^{}\\fi}\\catcode`\\%=\\active\\def%{\\%}3.6}}%\n",
                             "\\end{pgfscope}%\n",
                             "\\begin{pgfscope}%\n",
-                            "\\pgfpathrectangle{\\pgfqpoint{0.691763in}{0.596649in}}{\\pgfqpoint{5.448237in}{3.943351in}}%\n",
+                            "\\pgfpathrectangle{\\pgfqpoint{0.626778in}{0.571166in}}{\\pgfqpoint{5.513222in}{3.968834in}}%\n",
                             "\\pgfusepath{clip}%\n",
                             "\\pgfsetroundcap%\n",
                             "\\pgfsetroundjoin%\n",
                             "\\pgfsetlinewidth{1.003750pt}%\n",
                             "\\definecolor{currentstroke}{rgb}{1.000000,1.000000,1.000000}%\n",
                             "\\pgfsetstrokecolor{currentstroke}%\n",
                             "\\pgfsetdash{}{0pt}%\n",
-                            "\\pgfpathmoveto{\\pgfqpoint{0.691763in}{3.643784in}}%\n",
-                            "\\pgfpathlineto{\\pgfqpoint{6.140000in}{3.643784in}}%\n",
+                            "\\pgfpathmoveto{\\pgfqpoint{0.626778in}{3.637992in}}%\n",
+                            "\\pgfpathlineto{\\pgfqpoint{6.140000in}{3.637992in}}%\n",
                             "\\pgfusepath{stroke}%\n",
                             "\\end{pgfscope}%\n",
                             "\\begin{pgfscope}%\n",
                             "\\definecolor{textcolor}{rgb}{0.150000,0.150000,0.150000}%\n",
                             "\\pgfsetstrokecolor{textcolor}%\n",
                             "\\pgfsetfillcolor{textcolor}%\n",
-                            "\\pgftext[x=0.316851in, y=3.585746in, left, base]{\\color{textcolor}{\\sffamily\\fontsize{11.000000}{13.200000}\\selectfont\\catcode`\\^=\\active\\def^{\\ifmmode\\sp\\else\\^{}\\fi}\\catcode`\\%=\\active\\def%{\\%}3.8}}%\n",
+                            "\\pgftext[x=0.303555in, y=3.584978in, left, base]{\\color{textcolor}{\\sffamily\\fontsize{11.000000}{13.200000}\\selectfont\\catcode`\\^=\\active\\def^{\\ifmmode\\sp\\else\\^{}\\fi}\\catcode`\\%=\\active\\def%{\\%}3.8}}%\n",
                             "\\end{pgfscope}%\n",
                             "\\begin{pgfscope}%\n",
-                            "\\pgfpathrectangle{\\pgfqpoint{0.691763in}{0.596649in}}{\\pgfqpoint{5.448237in}{3.943351in}}%\n",
+                            "\\pgfpathrectangle{\\pgfqpoint{0.626778in}{0.571166in}}{\\pgfqpoint{5.513222in}{3.968834in}}%\n",
                             "\\pgfusepath{clip}%\n",
                             "\\pgfsetroundcap%\n",
                             "\\pgfsetroundjoin%\n",
                             "\\pgfsetlinewidth{1.003750pt}%\n",
                             "\\definecolor{currentstroke}{rgb}{1.000000,1.000000,1.000000}%\n",
                             "\\pgfsetstrokecolor{currentstroke}%\n",
                             "\\pgfsetdash{}{0pt}%\n",
-                            "\\pgfpathmoveto{\\pgfqpoint{0.691763in}{4.360757in}}%\n",
-                            "\\pgfpathlineto{\\pgfqpoint{6.140000in}{4.360757in}}%\n",
+                            "\\pgfpathmoveto{\\pgfqpoint{0.626778in}{4.359598in}}%\n",
+                            "\\pgfpathlineto{\\pgfqpoint{6.140000in}{4.359598in}}%\n",
                             "\\pgfusepath{stroke}%\n",
                             "\\end{pgfscope}%\n",
                             "\\begin{pgfscope}%\n",
                             "\\definecolor{textcolor}{rgb}{0.150000,0.150000,0.150000}%\n",
                             "\\pgfsetstrokecolor{textcolor}%\n",
                             "\\pgfsetfillcolor{textcolor}%\n",
-                            "\\pgftext[x=0.316851in, y=4.302719in, left, base]{\\color{textcolor}{\\sffamily\\fontsize{11.000000}{13.200000}\\selectfont\\catcode`\\^=\\active\\def^{\\ifmmode\\sp\\else\\^{}\\fi}\\catcode`\\%=\\active\\def%{\\%}4.0}}%\n",
+                            "\\pgftext[x=0.303555in, y=4.306585in, left, base]{\\color{textcolor}{\\sffamily\\fontsize{11.000000}{13.200000}\\selectfont\\catcode`\\^=\\active\\def^{\\ifmmode\\sp\\else\\^{}\\fi}\\catcode`\\%=\\active\\def%{\\%}4.0}}%\n",
                             "\\end{pgfscope}%\n",
                             "\\begin{pgfscope}%\n",
                             "\\definecolor{textcolor}{rgb}{0.150000,0.150000,0.150000}%\n",
                             "\\pgfsetstrokecolor{textcolor}%\n",
                             "\\pgfsetfillcolor{textcolor}%\n",
-                            "\\pgftext[x=0.261295in,y=2.568325in,,bottom,rotate=90.000000]{\\color{textcolor}{\\sffamily\\fontsize{12.000000}{14.400000}\\selectfont\\catcode`\\^=\\active\\def^{\\ifmmode\\sp\\else\\^{}\\fi}\\catcode`\\%=\\active\\def%{\\%}Y}}%\n",
+                            "\\pgftext[x=0.248000in,y=2.555583in,,bottom,rotate=90.000000]{\\color{textcolor}{\\sffamily\\fontsize{12.000000}{14.400000}\\selectfont\\catcode`\\^=\\active\\def^{\\ifmmode\\sp\\else\\^{}\\fi}\\catcode`\\%=\\active\\def%{\\%}y}}%\n",
                             "\\end{pgfscope}%\n",
                             "\\begin{pgfscope}%\n",
-                            "\\pgfpathrectangle{\\pgfqpoint{0.691763in}{0.596649in}}{\\pgfqpoint{5.448237in}{3.943351in}}%\n",
+                            "\\pgfpathrectangle{\\pgfqpoint{0.626778in}{0.571166in}}{\\pgfqpoint{5.513222in}{3.968834in}}%\n",
                             "\\pgfusepath{clip}%\n",
                             "\\pgfsetbuttcap%\n",
                             "\\pgfsetroundjoin%\n",
                             "\\definecolor{currentfill}{rgb}{0.298039,0.447059,0.690196}%\n",
                             "\\pgfsetfillcolor{currentfill}%\n",
                             "\\pgfsetlinewidth{0.501875pt}%\n",
                             "\\definecolor{currentstroke}{rgb}{0.298039,0.447059,0.690196}%\n",
                             "\\pgfsetstrokecolor{currentstroke}%\n",
                             "\\pgfsetdash{}{0pt}%\n",
-                            "\\pgfpathmoveto{\\pgfqpoint{0.939410in}{0.734226in}}%\n",
-                            "\\pgfpathcurveto{\\pgfqpoint{0.950460in}{0.734226in}}{\\pgfqpoint{0.961059in}{0.738616in}}{\\pgfqpoint{0.968873in}{0.746430in}}%\n",
-                            "\\pgfpathcurveto{\\pgfqpoint{0.976686in}{0.754243in}}{\\pgfqpoint{0.981077in}{0.764843in}}{\\pgfqpoint{0.981077in}{0.775893in}}%\n",
-                            "\\pgfpathcurveto{\\pgfqpoint{0.981077in}{0.786943in}}{\\pgfqpoint{0.976686in}{0.797542in}}{\\pgfqpoint{0.968873in}{0.805355in}}%\n",
-                            "\\pgfpathcurveto{\\pgfqpoint{0.961059in}{0.813169in}}{\\pgfqpoint{0.950460in}{0.817559in}}{\\pgfqpoint{0.939410in}{0.817559in}}%\n",
-                            "\\pgfpathcurveto{\\pgfqpoint{0.928360in}{0.817559in}}{\\pgfqpoint{0.917761in}{0.813169in}}{\\pgfqpoint{0.909947in}{0.805355in}}%\n",
-                            "\\pgfpathcurveto{\\pgfqpoint{0.902134in}{0.797542in}}{\\pgfqpoint{0.897743in}{0.786943in}}{\\pgfqpoint{0.897743in}{0.775893in}}%\n",
-                            "\\pgfpathcurveto{\\pgfqpoint{0.897743in}{0.764843in}}{\\pgfqpoint{0.902134in}{0.754243in}}{\\pgfqpoint{0.909947in}{0.746430in}}%\n",
-                            "\\pgfpathcurveto{\\pgfqpoint{0.917761in}{0.738616in}}{\\pgfqpoint{0.928360in}{0.734226in}}{\\pgfqpoint{0.939410in}{0.734226in}}%\n",
-                            "\\pgfpathlineto{\\pgfqpoint{0.939410in}{0.734226in}}%\n",
+                            "\\pgfpathmoveto{\\pgfqpoint{0.877379in}{0.709901in}}%\n",
+                            "\\pgfpathcurveto{\\pgfqpoint{0.888429in}{0.709901in}}{\\pgfqpoint{0.899028in}{0.714292in}}{\\pgfqpoint{0.906841in}{0.722105in}}%\n",
+                            "\\pgfpathcurveto{\\pgfqpoint{0.914655in}{0.729919in}}{\\pgfqpoint{0.919045in}{0.740518in}}{\\pgfqpoint{0.919045in}{0.751568in}}%\n",
+                            "\\pgfpathcurveto{\\pgfqpoint{0.919045in}{0.762618in}}{\\pgfqpoint{0.914655in}{0.773217in}}{\\pgfqpoint{0.906841in}{0.781031in}}%\n",
+                            "\\pgfpathcurveto{\\pgfqpoint{0.899028in}{0.788844in}}{\\pgfqpoint{0.888429in}{0.793235in}}{\\pgfqpoint{0.877379in}{0.793235in}}%\n",
+                            "\\pgfpathcurveto{\\pgfqpoint{0.866329in}{0.793235in}}{\\pgfqpoint{0.855729in}{0.788844in}}{\\pgfqpoint{0.847916in}{0.781031in}}%\n",
+                            "\\pgfpathcurveto{\\pgfqpoint{0.840102in}{0.773217in}}{\\pgfqpoint{0.835712in}{0.762618in}}{\\pgfqpoint{0.835712in}{0.751568in}}%\n",
+                            "\\pgfpathcurveto{\\pgfqpoint{0.835712in}{0.740518in}}{\\pgfqpoint{0.840102in}{0.729919in}}{\\pgfqpoint{0.847916in}{0.722105in}}%\n",
+                            "\\pgfpathcurveto{\\pgfqpoint{0.855729in}{0.714292in}}{\\pgfqpoint{0.866329in}{0.709901in}}{\\pgfqpoint{0.877379in}{0.709901in}}%\n",
+                            "\\pgfpathlineto{\\pgfqpoint{0.877379in}{0.709901in}}%\n",
                             "\\pgfpathclose%\n",
                             "\\pgfusepath{stroke,fill}%\n",
                             "\\end{pgfscope}%\n",
                             "\\begin{pgfscope}%\n",
-                            "\\pgfpathrectangle{\\pgfqpoint{0.691763in}{0.596649in}}{\\pgfqpoint{5.448237in}{3.943351in}}%\n",
+                            "\\pgfpathrectangle{\\pgfqpoint{0.626778in}{0.571166in}}{\\pgfqpoint{5.513222in}{3.968834in}}%\n",
                             "\\pgfusepath{clip}%\n",
                             "\\pgfsetbuttcap%\n",
                             "\\pgfsetroundjoin%\n",
                             "\\definecolor{currentfill}{rgb}{0.298039,0.447059,0.690196}%\n",
                             "\\pgfsetfillcolor{currentfill}%\n",
                             "\\pgfsetlinewidth{0.501875pt}%\n",
                             "\\definecolor{currentstroke}{rgb}{0.298039,0.447059,0.690196}%\n",
                             "\\pgfsetstrokecolor{currentstroke}%\n",
                             "\\pgfsetdash{}{0pt}%\n",
-                            "\\pgfpathmoveto{\\pgfqpoint{5.892353in}{4.319090in}}%\n",
-                            "\\pgfpathcurveto{\\pgfqpoint{5.903403in}{4.319090in}}{\\pgfqpoint{5.914002in}{4.323480in}}{\\pgfqpoint{5.921816in}{4.331294in}}%\n",
-                            "\\pgfpathcurveto{\\pgfqpoint{5.929629in}{4.339108in}}{\\pgfqpoint{5.934020in}{4.349707in}}{\\pgfqpoint{5.934020in}{4.360757in}}%\n",
-                            "\\pgfpathcurveto{\\pgfqpoint{5.934020in}{4.371807in}}{\\pgfqpoint{5.929629in}{4.382406in}}{\\pgfqpoint{5.921816in}{4.390220in}}%\n",
-                            "\\pgfpathcurveto{\\pgfqpoint{5.914002in}{4.398033in}}{\\pgfqpoint{5.903403in}{4.402423in}}{\\pgfqpoint{5.892353in}{4.402423in}}%\n",
-                            "\\pgfpathcurveto{\\pgfqpoint{5.881303in}{4.402423in}}{\\pgfqpoint{5.870704in}{4.398033in}}{\\pgfqpoint{5.862890in}{4.390220in}}%\n",
-                            "\\pgfpathcurveto{\\pgfqpoint{5.855076in}{4.382406in}}{\\pgfqpoint{5.850686in}{4.371807in}}{\\pgfqpoint{5.850686in}{4.360757in}}%\n",
-                            "\\pgfpathcurveto{\\pgfqpoint{5.850686in}{4.349707in}}{\\pgfqpoint{5.855076in}{4.339108in}}{\\pgfqpoint{5.862890in}{4.331294in}}%\n",
-                            "\\pgfpathcurveto{\\pgfqpoint{5.870704in}{4.323480in}}{\\pgfqpoint{5.881303in}{4.319090in}}{\\pgfqpoint{5.892353in}{4.319090in}}%\n",
-                            "\\pgfpathlineto{\\pgfqpoint{5.892353in}{4.319090in}}%\n",
+                            "\\pgfpathmoveto{\\pgfqpoint{5.889399in}{4.317932in}}%\n",
+                            "\\pgfpathcurveto{\\pgfqpoint{5.900449in}{4.317932in}}{\\pgfqpoint{5.911048in}{4.322322in}}{\\pgfqpoint{5.918862in}{4.330136in}}%\n",
+                            "\\pgfpathcurveto{\\pgfqpoint{5.926675in}{4.337949in}}{\\pgfqpoint{5.931066in}{4.348548in}}{\\pgfqpoint{5.931066in}{4.359598in}}%\n",
+                            "\\pgfpathcurveto{\\pgfqpoint{5.931066in}{4.370649in}}{\\pgfqpoint{5.926675in}{4.381248in}}{\\pgfqpoint{5.918862in}{4.389061in}}%\n",
+                            "\\pgfpathcurveto{\\pgfqpoint{5.911048in}{4.396875in}}{\\pgfqpoint{5.900449in}{4.401265in}}{\\pgfqpoint{5.889399in}{4.401265in}}%\n",
+                            "\\pgfpathcurveto{\\pgfqpoint{5.878349in}{4.401265in}}{\\pgfqpoint{5.867750in}{4.396875in}}{\\pgfqpoint{5.859936in}{4.389061in}}%\n",
+                            "\\pgfpathcurveto{\\pgfqpoint{5.852123in}{4.381248in}}{\\pgfqpoint{5.847732in}{4.370649in}}{\\pgfqpoint{5.847732in}{4.359598in}}%\n",
+                            "\\pgfpathcurveto{\\pgfqpoint{5.847732in}{4.348548in}}{\\pgfqpoint{5.852123in}{4.337949in}}{\\pgfqpoint{5.859936in}{4.330136in}}%\n",
+                            "\\pgfpathcurveto{\\pgfqpoint{5.867750in}{4.322322in}}{\\pgfqpoint{5.878349in}{4.317932in}}{\\pgfqpoint{5.889399in}{4.317932in}}%\n",
+                            "\\pgfpathlineto{\\pgfqpoint{5.889399in}{4.317932in}}%\n",
                             "\\pgfpathclose%\n",
                             "\\pgfusepath{stroke,fill}%\n",
                             "\\end{pgfscope}%\n",
                             "\\begin{pgfscope}%\n",
                             "\\pgfsetrectcap%\n",
                             "\\pgfsetmiterjoin%\n",
                             "\\pgfsetlinewidth{1.254687pt}%\n",
                             "\\definecolor{currentstroke}{rgb}{1.000000,1.000000,1.000000}%\n",
                             "\\pgfsetstrokecolor{currentstroke}%\n",
                             "\\pgfsetdash{}{0pt}%\n",
-                            "\\pgfpathmoveto{\\pgfqpoint{0.691763in}{0.596649in}}%\n",
-                            "\\pgfpathlineto{\\pgfqpoint{0.691763in}{4.540000in}}%\n",
+                            "\\pgfpathmoveto{\\pgfqpoint{0.626778in}{0.571166in}}%\n",
+                            "\\pgfpathlineto{\\pgfqpoint{0.626778in}{4.540000in}}%\n",
                             "\\pgfusepath{stroke}%\n",
                             "\\end{pgfscope}%\n",
                             "\\begin{pgfscope}%\n",
                             "\\pgfsetrectcap%\n",
                             "\\pgfsetmiterjoin%\n",
                             "\\pgfsetlinewidth{1.254687pt}%\n",
                             "\\definecolor{currentstroke}{rgb}{1.000000,1.000000,1.000000}%\n",
                             "\\pgfsetstrokecolor{currentstroke}%\n",
                             "\\pgfsetdash{}{0pt}%\n",
-                            "\\pgfpathmoveto{\\pgfqpoint{6.140000in}{0.596649in}}%\n",
+                            "\\pgfpathmoveto{\\pgfqpoint{6.140000in}{0.571166in}}%\n",
                             "\\pgfpathlineto{\\pgfqpoint{6.140000in}{4.540000in}}%\n",
                             "\\pgfusepath{stroke}%\n",
                             "\\end{pgfscope}%\n",
                             "\\begin{pgfscope}%\n",
                             "\\pgfsetrectcap%\n",
                             "\\pgfsetmiterjoin%\n",
                             "\\pgfsetlinewidth{1.254687pt}%\n",
                             "\\definecolor{currentstroke}{rgb}{1.000000,1.000000,1.000000}%\n",
                             "\\pgfsetstrokecolor{currentstroke}%\n",
                             "\\pgfsetdash{}{0pt}%\n",
-                            "\\pgfpathmoveto{\\pgfqpoint{0.691763in}{0.596649in}}%\n",
-                            "\\pgfpathlineto{\\pgfqpoint{6.140000in}{0.596649in}}%\n",
+                            "\\pgfpathmoveto{\\pgfqpoint{0.626778in}{0.571166in}}%\n",
+                            "\\pgfpathlineto{\\pgfqpoint{6.140000in}{0.571166in}}%\n",
                             "\\pgfusepath{stroke}%\n",
                             "\\end{pgfscope}%\n",
                             "\\begin{pgfscope}%\n",
                             "\\pgfsetrectcap%\n",
                             "\\pgfsetmiterjoin%\n",
                             "\\pgfsetlinewidth{1.254687pt}%\n",
                             "\\definecolor{currentstroke}{rgb}{1.000000,1.000000,1.000000}%\n",
                             "\\pgfsetstrokecolor{currentstroke}%\n",
                             "\\pgfsetdash{}{0pt}%\n",
-                            "\\pgfpathmoveto{\\pgfqpoint{0.691763in}{4.540000in}}%\n",
+                            "\\pgfpathmoveto{\\pgfqpoint{0.626778in}{4.540000in}}%\n",
                             "\\pgfpathlineto{\\pgfqpoint{6.140000in}{4.540000in}}%\n",
                             "\\pgfusepath{stroke}%\n",
                             "\\end{pgfscope}%\n",
                             "\\end{pgfpicture}%\n",
                             "\\makeatother%\n",
                             "\\endgroup%\n"
                         ]
                     },
-                    "execution_count": 29,
+                    "execution_count": 2,
                     "metadata": {
                         "image/png": {
                             "height": 378.25,
                             "width": 509.15
                         }
                     },
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "# #fig:seaborn\n",
                 "# penguins = sns.load_dataset(\"penguins\", cache=False)\n",
                 "# so.Plot(penguins, x=\"bill_length_mm\", y=\"bill_depth_mm\").add(so.Dot())\n",
                 "df = pd.DataFrame({\"x_1\": [1, 2], \"y\": [3, 4]})\n",
-                "so.Plot(df, x=\"x_1\", y=\"y\").add(so.Dot()).label(x=\"X\", y=\"Y\")"
+                "so.Plot(df, x=\"x_1\", y=\"y\").add(so.Dot())"
             ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": []
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "test.py3.12",
             "language": "python",
             "name": "python3"
```

### Comparing `panpdf-0.2.0/notebooks/svg.ipynb` & `panpdf-0.2.1/notebooks/svg.ipynb`

 * *Files identical despite different names*

### Comparing `panpdf-0.2.0/src/panpdf/formatters.py` & `panpdf-0.2.1/src/panpdf/formatters.py`

 * *Files identical despite different names*

### Comparing `panpdf-0.2.0/src/panpdf/main.py` & `panpdf-0.2.1/src/panpdf/main.py`

 * *Files identical despite different names*

### Comparing `panpdf-0.2.0/src/panpdf/stores.py` & `panpdf-0.2.1/src/panpdf/stores.py`

 * *Files identical despite different names*

### Comparing `panpdf-0.2.0/src/panpdf/tools.py` & `panpdf-0.2.1/src/panpdf/tools.py`

 * *Files identical despite different names*

### Comparing `panpdf-0.2.0/src/panpdf/filters/attribute.py` & `panpdf-0.2.1/src/panpdf/filters/attribute.py`

 * *Files identical despite different names*

### Comparing `panpdf-0.2.0/src/panpdf/filters/crossref.py` & `panpdf-0.2.1/src/panpdf/filters/crossref.py`

 * *Files identical despite different names*

### Comparing `panpdf-0.2.0/src/panpdf/filters/filter.py` & `panpdf-0.2.1/src/panpdf/filters/filter.py`

 * *Files identical despite different names*

### Comparing `panpdf-0.2.0/src/panpdf/filters/jupyter.py` & `panpdf-0.2.1/src/panpdf/filters/jupyter.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from __future__ import annotations
 
 import base64
 import io
+import re
 from dataclasses import dataclass, field
 from pathlib import Path
 from typing import Any, ClassVar
 
 import yaml
 from panflute import Doc, Image, Plain, RawInline
 
@@ -19,19 +20,18 @@
 @dataclass(repr=False)
 class Jupyter(Filter):
     types: ClassVar[type[Image]] = Image
     defaults: Path | None = None
     standalone: bool = False
     pandoc_path: Path | None = None
     store: Store = field(default_factory=Store)
+    pgf: bool = field(default=False, init=False)
+    preamble: str = field(default="", init=False)
 
-    # def set_notebooks_dir(self, notebooks_dir: list[Path]):
-    #     self.store.set_notebooks_dir(notebooks_dir)
-
-    def action(self, image: Image, doc: Doc) -> Image:
+    def action(self, image: Image, doc: Doc) -> Image:  # noqa: ARG002
         url = image.url
         identifier = image.identifier
 
         if not identifier or (url and not url.endswith(".ipynb")):
             return image
 
         try:
@@ -42,33 +42,57 @@
 
         if not data:
             return image
 
         if not (url_or_text := create_image_file(data, standalone=self.standalone)):
             return image
 
-        if not url_or_text.startswith(PGF_PREFIX) or not self.standalone:
+        if not url_or_text.startswith(PGF_PREFIX):
             image.url = url_or_text
-            doc.metadata["__pgf__"] = True
+            return image
+
+        text = url_or_text
+
+        if not self.preamble:
+            self.preamble = get_preamble(text)
+
+        if not self.standalone:
+            image.url = text
+            self.pgf = True
             return image
 
         image.url, text = create_image_file_pgf(
-            url_or_text,
-            self.defaults,
-            self.pandoc_path,
+            text,
+            defaults=self.defaults,
+            preamble=self.preamble,
+            pandoc_path=self.pandoc_path,
             description=f"Creating an image for {url}#{identifier}",
         )
         self.store.add_data(url, identifier, "application/pdf", text)
         self.store.save_notebook(url)
         return image
 
     def finalize(self, doc: Doc) -> None:
-        if doc.metadata.pop("__pgf__", None):
-            path = create_temp_file("\\usepackage{pgf}", suffix=".tex")
-            add_metadata_list(doc, "include-in-header", path.as_posix())
+        if not self.pgf:
+            return
+
+        path = create_temp_file(f"\\usepackage{{pgf}}{self.preamble}", suffix=".tex")
+        add_metadata_list(doc, "include-in-header", path.as_posix())
+
+
+PREAMBLE_PATTERN = re.compile(
+    r"^%% Matplotlib used the following preamble\n(.+?)\n%%\n", re.M | re.S
+)
+
+
+def get_preamble(text: str) -> str:
+    if m := PREAMBLE_PATTERN.search(text):
+        return re.sub(r"^%%\s+", "", m.group(1), flags=re.M)
+
+    return ""
 
 
 def create_image_file(data: dict[str, str], *, standalone: bool = False) -> str | None:
     text = data.get("text/plain", "")
     text_pgf = text if text.startswith(PGF_PREFIX) else None
 
     if not standalone and text_pgf:
@@ -107,20 +131,22 @@
     data = path.read_bytes()
     text = base64.b64encode(data).decode()
     return path.as_posix(), text
 
 
 def create_image_file_pgf(
     text: str,
+    *,
     defaults: Path | None = None,
+    preamble: str = "",
     pandoc_path: Path | None = None,
     description: str = "",
 ) -> tuple[str, str]:
     doc = Doc(Plain(RawInline(text, format="latex")))
-    defaults = create_defaults_for_standalone(defaults)
+    defaults = create_defaults_for_standalone(defaults, preamble)
 
     path = create_temp_file(None, suffix=".pdf")
     extra_args = ["--defaults", defaults.as_posix(), "--output", path.as_posix()]
 
     convert_doc(
         doc,
         output_format="pdf",
@@ -131,28 +157,31 @@
     )
 
     data = path.read_bytes()
     text = base64.b64encode(data).decode()
     return path.as_posix(), text
 
 
-def create_defaults_for_standalone(path: Path | None = None) -> Path:
+def create_defaults_for_standalone(path: Path | None = None, preamble: str = "") -> Path:
     if path:
         with path.open(encoding="utf8") as f:
             defaults: dict[str, Any] = yaml.safe_load(f)
     else:
         path = Path(".")
         defaults = {}
 
+    if "\\usepackage{fontspec}" in preamble:
+        defaults.setdefault("pdf-engine", "xelatex")
+
     in_header = defaults.get("include-in-header", [])
 
     if isinstance(in_header, str):
         in_header = [in_header]
 
-    path = create_temp_file("\\usepackage{pgf}", suffix=".tex", dir=path.parent)
+    path = create_temp_file(f"\\usepackage{{pgf}}{preamble}", suffix=".tex", dir=path.parent)
     in_header.append(path.as_posix())
     defaults["include-in-header"] = in_header
 
     for toc in ["table-of-contents", "toc", "toc-depth"]:
         if toc in defaults:
             del defaults[toc]
```

### Comparing `panpdf-0.2.0/src/panpdf/filters/layout.py` & `panpdf-0.2.1/src/panpdf/filters/layout.py`

 * *Files identical despite different names*

### Comparing `panpdf-0.2.0/src/panpdf/filters/verbatim.py` & `panpdf-0.2.1/src/panpdf/filters/verbatim.py`

 * *Files identical despite different names*

### Comparing `panpdf-0.2.0/src/panpdf/filters/zotero.py` & `panpdf-0.2.1/src/panpdf/filters/zotero.py`

 * *Files identical despite different names*

### Comparing `panpdf-0.2.0/tests/conftest.py` & `panpdf-0.2.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `panpdf-0.2.0/tests/test_converters.py` & `panpdf-0.2.1/tests/test_converters.py`

 * *Files identical despite different names*

### Comparing `panpdf-0.2.0/tests/test_formatters.py` & `panpdf-0.2.1/tests/test_formatters.py`

 * *Files identical despite different names*

### Comparing `panpdf-0.2.0/tests/test_main.py` & `panpdf-0.2.1/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `panpdf-0.2.0/tests/test_stores.py` & `panpdf-0.2.1/tests/test_stores.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,26 +42,35 @@
     with pytest.raises(ValueError, match="Unknown identifier"):
         store.get_cell("pgf.ipynb", "fig:png")
 
 
 def test_get_source(store: Store, fmt: str):
     source = store.get_source(f"{fmt}.ipynb", f"fig:{fmt}")
     assert isinstance(source, str)
-    assert source.rstrip() == "import matplotlib.pyplot as plt\n\nplt.plot([-1, 1], [-1, 1])"
+    if fmt != "pgf":
+        assert source.rstrip() == "import matplotlib.pyplot as plt\n\nplt.plot([-1, 1], [-1, 1])"
+    else:
+        assert source.startswith("import matplotlib.pyplot as plt\n\nplt.plot([1, 10, 100],")
 
 
 def test_get_outputs(store: Store, fmt: str):
     outputs = store.get_outputs(f"{fmt}.ipynb", f"fig:{fmt}")
     assert isinstance(outputs, list)
-    assert len(outputs) == 2
-    assert isinstance(outputs[0], dict)
-    assert outputs[0]["output_type"] == "execute_result"
-    assert "text/plain" in outputs[0]["data"]
-    assert isinstance(outputs[1], dict)
-    assert outputs[1]["output_type"] == "display_data"
+    if fmt != "pgf":
+        assert len(outputs) == 2
+        assert isinstance(outputs[0], dict)
+        assert outputs[0]["output_type"] == "execute_result"
+        assert "text/plain" in outputs[0]["data"]
+        assert isinstance(outputs[1], dict)
+        assert outputs[1]["output_type"] == "display_data"
+    else:
+        assert len(outputs) == 1
+        assert isinstance(outputs[0], dict)
+        assert outputs[0]["output_type"] == "display_data"
+        assert "text/plain" in outputs[0]["data"]
 
 
 def test_get_data(store: Store, fmt: str):
     data = store.get_data(f"{fmt}.ipynb", f"fig:{fmt}")
     assert isinstance(data, dict)
     assert len(data) == 3 if fmt in ["pdf", "svg"] else 2
     assert "text/plain" in data
```

### Comparing `panpdf-0.2.0/tests/test_tools.py` & `panpdf-0.2.1/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `panpdf-0.2.0/tests/filters/test_attribute.py` & `panpdf-0.2.1/tests/filters/test_attribute.py`

 * *Files identical despite different names*

### Comparing `panpdf-0.2.0/tests/filters/test_crossref.py` & `panpdf-0.2.1/tests/filters/test_crossref.py`

 * *Files identical despite different names*

### Comparing `panpdf-0.2.0/tests/filters/test_filter.py` & `panpdf-0.2.1/tests/filters/test_filter.py`

 * *Files identical despite different names*

### Comparing `panpdf-0.2.0/tests/filters/test_jupyter.py` & `panpdf-0.2.1/tests/filters/test_jupyter.py`

 * *Files 4% similar despite different names*

```diff
@@ -81,22 +81,34 @@
     assert defaults["variables"] == {"documentclass": "standalone"}
     header = defaults["include-in-header"]
     assert isinstance(header, list)
     assert isinstance(header[0], str)
     assert header[0].endswith(".tex")
 
 
+def test_get_preamble(store: Store):
+    from panpdf.filters.jupyter import get_preamble
+
+    data = store.get_data("pgf.ipynb", "fig:pgf")
+    text = data["text/plain"]
+    preamble = get_preamble(text)
+    assert r"\def\mathdefault#1{#1}" in preamble
+    assert r"\usepackage[strings]{underscore}" in preamble
+    assert r"\setmainfont" not in preamble
+
+
 @pytest.mark.parametrize("use_defaults", [False, True])
 def test_create_image_file_pgf(store: Store, defaults, use_defaults):
-    from panpdf.filters.jupyter import create_image_file_pgf
+    from panpdf.filters.jupyter import create_image_file_pgf, get_preamble
 
     data = store.get_data("pgf.ipynb", "fig:pgf")
     text = data["text/plain"]
     defaults = defaults if use_defaults else None
-    url, text = create_image_file_pgf(text, defaults)
+    preamble = get_preamble(text)
+    url, text = create_image_file_pgf(text, defaults=defaults, preamble=preamble)
 
     path = Path(url)
     assert path.exists()
     assert path.stat().st_size
     assert text.startswith("JVBER")
```

### Comparing `panpdf-0.2.0/tests/filters/test_layout.py` & `panpdf-0.2.1/tests/filters/test_layout.py`

 * *Files identical despite different names*

### Comparing `panpdf-0.2.0/tests/filters/test_verbatim.py` & `panpdf-0.2.1/tests/filters/test_verbatim.py`

 * *Files identical despite different names*

### Comparing `panpdf-0.2.0/tests/filters/test_zotero.py` & `panpdf-0.2.1/tests/filters/test_zotero.py`

 * *Files identical despite different names*

### Comparing `panpdf-0.2.0/tests/libraries/test_nbformat.py` & `panpdf-0.2.1/tests/libraries/test_nbformat.py`

 * *Files identical despite different names*

### Comparing `panpdf-0.2.0/tests/libraries/panflute/test_cite.py` & `panpdf-0.2.1/tests/libraries/panflute/test_cite.py`

 * *Files identical despite different names*

### Comparing `panpdf-0.2.0/tests/libraries/panflute/test_code.py` & `panpdf-0.2.1/tests/libraries/panflute/test_code.py`

 * *Files identical despite different names*

### Comparing `panpdf-0.2.0/tests/libraries/panflute/test_figure.py` & `panpdf-0.2.1/tests/libraries/panflute/test_figure.py`

 * *Files identical despite different names*

### Comparing `panpdf-0.2.0/tests/libraries/panflute/test_math.py` & `panpdf-0.2.1/tests/libraries/panflute/test_math.py`

 * *Files identical despite different names*

### Comparing `panpdf-0.2.0/tests/libraries/panflute/test_metadata.py` & `panpdf-0.2.1/tests/libraries/panflute/test_metadata.py`

 * *Files identical despite different names*

### Comparing `panpdf-0.2.0/tests/libraries/panflute/test_raw.py` & `panpdf-0.2.1/tests/libraries/panflute/test_raw.py`

 * *Files identical despite different names*

### Comparing `panpdf-0.2.0/tests/libraries/panflute/test_section.py` & `panpdf-0.2.1/tests/libraries/panflute/test_section.py`

 * *Files identical despite different names*

### Comparing `panpdf-0.2.0/tests/libraries/panflute/test_table.py` & `panpdf-0.2.1/tests/libraries/panflute/test_table.py`

 * *Files identical despite different names*

### Comparing `panpdf-0.2.0/tests/libraries/panflute/test_tex.py` & `panpdf-0.2.1/tests/libraries/panflute/test_tex.py`

 * *Files identical despite different names*

### Comparing `panpdf-0.2.0/LICENSE.txt` & `panpdf-0.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `panpdf-0.2.0/README.md` & `panpdf-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `panpdf-0.2.0/pyproject.toml` & `panpdf-0.2.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -46,35 +46,41 @@
 exclude = ["/.github", "/docs"]
 [tool.hatch.build.targets.wheel]
 packages = ["src/panpdf"]
 
 [tool.hatch.envs.test]
 dependencies = [
   "cairosvg",
+  "hvplot",
   "matplotlib",
   "pandas",
+  "polars",
+  "pyarrow",
+  "pytest-clarity",
   "pytest-cov",
   "pytest-randomly",
   "seaborn",
 ]
 
 [tool.hatch.envs.test.scripts]
 run = "pytest {args:tests src/panpdf}"
 cov = "coverage report {args:--skip-covered --show-missing}"
 
 [[tool.hatch.envs.test.matrix]]
 python = ["3.10", "3.11", "3.12"]
 
 [tool.pytest.ini_options]
 addopts = [
-  "--verbose",
+  "-vv",
+  "--capture=no",
   "--color=yes",
-  "--doctest-modules",
-  "--cov=panpdf",
   "--cov-report=lcov:lcov.info",
+  "--cov=panpdf",
+  "--doctest-modules",
+  "--tb=short",
 ]
 doctest_optionflags = ["NORMALIZE_WHITESPACE", "IGNORE_EXCEPTION_DETAIL"]
 filterwarnings = ['ignore:setDaemon\(\) is deprecated:DeprecationWarning']
 
 [tool.coverage.run]
 omit = ["src/panpdf/__about__.py"]
```

### Comparing `panpdf-0.2.0/PKG-INFO` & `panpdf-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: panpdf
-Version: 0.2.0
+Version: 0.2.1
 Summary: PDF documentation generator
 Project-URL: Documentation, https://daizutabi.github.io/panpdf
 Project-URL: Source, https://github.com/daizutabi/panpdf
 Project-URL: Issues, https://github.com/daizutabi/panpdf/issues
 Author-email: daizutabi <daizutabi@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
```

