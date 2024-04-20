# Comparing `tmp/glytrait-0.1.0.tar.gz` & `tmp/glytrait-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glytrait-0.1.0.tar", max compression
+gzip compressed data, was "glytrait-0.1.1.tar", max compression
```

## Comparing `glytrait-0.1.0.tar` & `glytrait-0.1.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1063 2023-06-01 11:46:23.327576 glytrait-0.1.0/LICENSE
--rw-r--r--   0        0        0    12405 2024-04-16 07:50:39.141303 glytrait-0.1.0/README.md
--rw-r--r--   0        0        0     1190 2024-04-14 11:59:39.762252 glytrait-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       74 2024-04-14 11:59:27.621443 glytrait-0.1.0/src/glytrait/__init__.py
--rw-r--r--   0        0        0    10396 2024-04-16 02:38:14.413421 glytrait-0.1.0/src/glytrait/api.py
--rw-r--r--   0        0        0     4748 2024-02-10 13:59:57.519954 glytrait-0.1.0/src/glytrait/cli.py
--rw-r--r--   0        0        0     2683 2024-04-14 11:59:08.462417 glytrait-0.1.0/src/glytrait/data_export.py
--rw-r--r--   0        0        0      923 2023-12-30 06:44:57.217908 glytrait-0.1.0/src/glytrait/data_type.py
--rw-r--r--   0        0        0      812 2024-04-14 11:59:08.463548 glytrait-0.1.0/src/glytrait/exception.py
--rw-r--r--   0        0        0    27518 2024-04-16 02:38:14.593722 glytrait-0.1.0/src/glytrait/formula.py
--rw-r--r--   0        0        0    13768 2024-02-10 13:59:57.574326 glytrait-0.1.0/src/glytrait/glycan.py
--rw-r--r--   0        0        0    14569 2024-03-08 09:00:51.155221 glytrait-0.1.0/src/glytrait/load_data.py
--rw-r--r--   0        0        0    18283 2024-04-14 11:59:08.464441 glytrait-0.1.0/src/glytrait/meta_property.py
--rw-r--r--   0        0        0     6664 2024-04-14 11:59:08.464921 glytrait-0.1.0/src/glytrait/post_filtering.py
--rw-r--r--   0        0        0     4621 2024-02-10 13:59:57.532082 glytrait-0.1.0/src/glytrait/preprocessing.py
--rw-r--r--   0        0        0     8081 2024-04-14 11:59:08.465266 glytrait-0.1.0/src/glytrait/resources/comp_formula.txt
--rw-r--r--   0        0        0    55082 2024-04-14 11:59:08.465614 glytrait-0.1.0/src/glytrait/resources/struc_formula.txt
--rw-r--r--   0        0        0     3767 2024-04-15 11:39:53.052570 glytrait-0.1.0/src/glytrait/stat.py
--rw-r--r--   0        0        0     1665 2023-12-30 06:44:57.220052 glytrait-0.1.0/src/glytrait/trait.py
--rw-r--r--   0        0        0    12818 1970-01-01 00:00:00.000000 glytrait-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-06-01 11:46:23.327576 glytrait-0.1.1/LICENSE
+-rw-r--r--   0        0        0    13933 2024-04-20 04:25:00.882511 glytrait-0.1.1/README.md
+-rw-r--r--   0        0        0     1263 2024-04-20 04:23:15.911626 glytrait-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0       74 2024-04-20 04:08:28.908891 glytrait-0.1.1/src/glytrait/__init__.py
+-rw-r--r--   0        0        0    10712 2024-04-20 03:37:48.972694 glytrait-0.1.1/src/glytrait/api.py
+-rw-r--r--   0        0        0     4748 2024-02-10 13:59:57.519954 glytrait-0.1.1/src/glytrait/cli.py
+-rw-r--r--   0        0        0     2683 2024-04-14 11:59:08.462417 glytrait-0.1.1/src/glytrait/data_export.py
+-rw-r--r--   0        0        0      923 2023-12-30 06:44:57.217908 glytrait-0.1.1/src/glytrait/data_type.py
+-rw-r--r--   0        0        0      812 2024-04-14 11:59:08.463548 glytrait-0.1.1/src/glytrait/exception.py
+-rw-r--r--   0        0        0    27106 2024-04-20 03:32:01.149878 glytrait-0.1.1/src/glytrait/formula.py
+-rw-r--r--   0        0        0    13768 2024-02-10 13:59:57.574326 glytrait-0.1.1/src/glytrait/glycan.py
+-rw-r--r--   0        0        0    14569 2024-03-08 09:00:51.155221 glytrait-0.1.1/src/glytrait/load_data.py
+-rw-r--r--   0        0        0    18283 2024-04-14 11:59:08.464441 glytrait-0.1.1/src/glytrait/meta_property.py
+-rw-r--r--   0        0        0     6664 2024-04-14 11:59:08.464921 glytrait-0.1.1/src/glytrait/post_filtering.py
+-rw-r--r--   0        0        0     4621 2024-02-10 13:59:57.532082 glytrait-0.1.1/src/glytrait/preprocessing.py
+-rw-r--r--   0        0        0     8081 2024-04-14 11:59:08.465266 glytrait-0.1.1/src/glytrait/resources/comp_formula.txt
+-rw-r--r--   0        0        0    55082 2024-04-14 11:59:08.465614 glytrait-0.1.1/src/glytrait/resources/struc_formula.txt
+-rw-r--r--   0        0        0     3743 2024-04-20 03:31:49.134440 glytrait-0.1.1/src/glytrait/stat.py
+-rw-r--r--   0        0        0     1665 2023-12-30 06:44:57.220052 glytrait-0.1.1/src/glytrait/trait.py
+-rw-r--r--   0        0        0    14358 1970-01-01 00:00:00.000000 glytrait-0.1.1/PKG-INFO
```

### Comparing `glytrait-0.1.0/LICENSE` & `glytrait-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `glytrait-0.1.0/README.md` & `glytrait-0.1.1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,102 +1,140 @@
 ![logo](img/logo.png)
 
 # GlyTrait
 
+[![PyPI - Version](https://img.shields.io/pypi/v/glytrait)](https://pypi.org/project/glytrait/)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/glytrait)
+[![GitHub License](https://img.shields.io/github/license/fubin1999/glytrait)](https://github.com/fubin1999/glytrait/blob/main/LICENSE)
+[![Coverage Status](https://coveralls.io/repos/github/fubin1999/glytrait/badge.svg?branch=main)](https://coveralls.io/github/fubin1999/glytrait?branch=main)
+[![Codacy Badge](https://app.codacy.com/project/badge/Grade/e3e6a19dccb749f786264247738fa585)](https://app.codacy.com/gh/fubin1999/glytrait/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_grade)
+
 ## Overview
 
-Glycan derived trait is a more insightful way to analysis glycomics data.
-However, currently there lacks a tool for automatically calculating derived traits,
-while mannual calculating is cumbersome, time-consuming and error-prone.
-GlyTrait is a tool designed for calculating N-glycan traits merely from abundance information and
-glycan structures.
+*Q: What is GlyTrait?*
+
+*A: GlyTrait is a tool for calculating derived traits for N-glycomic data.*
+
+*Q: Sounds cool! So..., what are derived traits again?*
+
+*A: Well, derived traits are artificial variables that summarize certain aspects of 
+the glycome. 
+For example, the proportion of core-fucosylated glycans, 
+the average number of sialic acids per glycan, 
+or the proportion of bisected glycans within bi-antennary complex glycans, etc. 
+Derived traits are more biologically relavant 
+and have been used a lot in the glycomics community.*
+
+*Q: So, GlyTrait does the dirty work for me, 
+saving my time and energy for more interesting analysis?*
+
+*A: You bet!*
 
 ## Contents
 
 - [Installation](#installation)
     - [Requirement](#requirement)
     - [Using pipx (recommended)](#using-pipx-recommended)
 - [Usage](#usage)
     - [Quick start](#quick-start)
     - [Options](#options)
     - [Mode](#mode)
     - [Input file format](#input-file-format)
-    - [Specify output path](#specify-output-path)
-    - [Structure file](#structure-file)
+    - [Specify output path](#specify-the-output-path)
     - [Preprocessing](#preprocessing)
     - [Sialic-acid-linkage traits](#sialic-acid-linkage-traits)
     - [Post-filtering](#post-filtering)
 - [License](#license)
 
+## Web app
+
+> Let there be no command line apps!
+> 
+> -- my colleagues
+
+A web app version of GlyTrait is on its way here...
+Ready to say goodbye to the command line?
+
 ## Installation
 
 ### Requirement
 
 ```
 python >= 3.10
 ```
 
-If python hasn't been install, download it from
-its [its website](https://www.bing.com/search?q=python&form=APMCS1&PC=APMC), or
-use [Anaconda](https://www.anaconda.com/download/) if you like.
+If python hasn't been installed, 
+download it from [its website](https://www.bing.com/search?q=python&form=APMCS1&PC=APMC),
+or use [Anaconda](https://www.anaconda.com/download/) if you like.
 
-### Using pipx (recommended)
+### Option 1: Using pipx (recommended)
 
-pipx is a tool to help you install and run end-user applications written in Python.
+`pipx` is a tool to help you install and run end-user applications written in Python.
 It's roughly similar to macOS's brew, JavaScript's npx, and Linux's apt.
 
 #### Install pipx
 
 Install pipx following its [Document](https://pypa.github.io/pipx/installation/).
 
 #### Install GlyTrait from PyPi
 
 ```shell
 pipx install glytrait
 ```
 
-### Using Conda environment
+### Option 2: Using pip
 
-#### Create a new environment
+#### 1. Create a new conda environment (optional)
 
 ```shell
 conda create -n glytrait python=3.10
 ```
 
-#### Activate the environment
+and activate the environment.
 
 ```shell
 conda activate glytrait
 ```
 
-#### Install GlyTrait from PyPi
+#### 2. Install GlyTrait from PyPi
 
 ```shell
 pip install glytrait
 ```
 
 ## Usage
 
 ### Quick start
 
-Download the example files: (to be added).
+1. Download the [example files](https://github.com/fubin1999/glytrait/tree/main/example_data)
+to a new directory: `glytrait_example`.
+
+2. Open a terminal and navigate to the directory:
+
+```shell
+cd glytrait_example
+```
+
+3. Run the following command:
 
 ```shell
 glytrait abundance.csv structures.csv
 ```
 
 That's it! 
 If everything goes well, a folder named "abundance_glytrait" will be created
 in the same directory with the abundnce.csv file.
 Inside the directory are four files:
 
-1. `derived_traits.csv`: the derived traits calculated by GlyTrait.
-2. `glycan_abundance_processed.csv`: the glycan abundance after preprocessing.
-3. `meta_properties.csv`: the meta properties of all glycans.
-4. `formulas.txt`: the definations of all derived traits.
+1. `derived_traits.csv`: all derived traits calculated by GlyTrait.
+2. `derived_traits_filtered.csv`: derived traits after post-filtering 
+   (see [Post-filtering](#post-filtering)).
+3. `glycan_abundance_processed.csv`: the glycan abundance after preprocessing
+   (see [Preprocessing](#preprocessing)).
+4. `meta_properties.csv`: the meta-properties of all glycans.
 
 The detailed format of the input file will be introduced in the
 [Input file format](#input-file-format) section.
 
 ### Options
 
 *This section is intended to give an overview of the CLI interface.
@@ -131,15 +169,16 @@
 Note that the "composition" mode has uncertainties to some extent. Specifically:
 
 1. Estimating the number of Gal based on composition is not possible for hybrid glycans,
    so GlyTrait will calculate the number of Gal assuming there are no hybrid glycans.
    kily, hybrid glycans are usually in low abundance,
    so the algorithm is a good approximation for most cases.
 2. Estimating the number of branches is not possible based on composition,
-   so GlyTrait will roughly classify glycans into 2 categories: low-branching and high-branching.
+   so GlyTrait will roughly classify glycans into two categories: 
+   low-branching and high-branching.
    Glycans with N > 4 (including bisecting diantenary glycans) are considered as high-branching,
    while others as low-branching.
 3. Telling hybrid glycans from mono-antenary complex glycans is not possible based on composition,
    so GlyTrait will not classify glycans into complex, hybrid and high-mannose.
 
 Due to the ambiguities above, we recommend using the "structure" mode if possible.
 
@@ -165,23 +204,23 @@
 At least two files are needed for GlyTrait to work:
 
 #### 1. The abundance file
 
 A csv file with samples as rows and glycan IDs as columns.
 An example file would be like:
 
-| Sample | Glycan1 | Glycan2 | Glycan3 |
-|--------|---------|---------|---------|
+| Sample  | Glycan1 | Glycan2 | Glycan3 |
+|---------|---------|---------|---------|
 | Sample1 | 0.0417  | 0.0503  | 0.0354  |
 | Sample2 | 0.0233  | 0.0533  | 0.0593  |
 | Sample3 | 0.0123  | 0.0133  | 0.0194  |
 
 The header of the first column should be "Sample",
 and the header of the other columns should be glycan IDs.
-Glycan IDs can be any string, e.g. the composition strings ("H3N4").
+Glycan IDs can be any string, e.g., the composition strings ("H3N4").
 
 **Both glycan IDs and samples should be unique.**
 
 #### 2. The structure file (or the composition file)
 
 A csv file with two columns: "GlycanID" and "Structure" (or "Composition").
 An example file would be like:
@@ -195,15 +234,15 @@
 The "GlycanID" column should contain all glycan IDs in the abundance file.
 The "Structure" column should contain the structure strings of the glycans.
 For now, only the GlycoCT format is supported.
 In the "composition" mode, the second column should be "Composition" instead of "Structure",
 and the composition strings should be used instead of the structure strings.
 Condensed format ("H3N4F1S1") is supported.
 
-### Specify output path
+### Specify the output path
 
 You might have noticed before that GlyTrait saves the output file to the same directory 
 as the abundance file with a "_glytrait" suffix.
 You can specify the output file path by using the "-o" or "--output-file" option:
 
 ```shell
 glytrait abundance.csv structure.csv -o output
@@ -227,15 +266,15 @@
 glytrait abundance.csv structure.csv -r 0.5
 ```
 
 The imputation method could be specified by the "-i" or the "--impute-method" option.
 The default method is "zero",
 which means missing values will be imputed by 0.
 Other supported methods are "mean", "median", "zero", "lod".
-You can change imputation method to "min" by:
+You can change the imputation method to "min" by:
 
 ```shell
 glytrait abundance.csv structure.csv -i min
 ```
 
 A full list of supported imputation methods are:
 
@@ -244,61 +283,61 @@
 - "median": impute missing values by the median value of a glycan within all samples.
 - "zero": impute missing values by 0.
 - "lod": impute missing values by the limit of detection (LOD) of the equipment. The LOD of a
   glycan is defined as the minimum value of the glycan within all samples divided by 5.
 
 ### Sialic-acid-linkage traits
 
-Sialic acids can have different linkages for N-glycans (e.g. α2,3 and α2,6).
+Sialic acids can have different linkages for N-glycans (e.g., α2,3 and α2,6).
 Different sialic acid linkage has different biological functions.
 GlyTrait supports calculating derived traits regarding these linkages.
 To use this feature, you need to have siaic acid linkage information.
 
 In the structure mode, the "Structure" column or the structure file should contain the linkage
 information.
 Only linkage information about sialic acids is needed.
 This can be easily done using GlycoWorkbench.
 
 In the composition mode, the "Composition" column must contain the linkage information.
 GlyTrait uses a common notation for sialic acid with different linkages:
 "E" for a2,6-linked sialic acids, and "L" a2,3-linked sialic acids.
-For example, "H5N4F1E1L1" contains 2 sialic acids, one is a2,6-linked and the other is
-a2,3-linked.
+For example, "H5N4F1E1L1" contains two sialic acids, one is a2,6-linked, 
+and the other is a2,3-linked.
 
 You can use the "-l" or "--sia-linkage" option to include sialic-acid-linkage traits:
 
 ```shell
 glytrait abundance.csv structure.csv -l
 ```
 
 Note that if you use this option, all glycans with sialic acids should have linkage information.
-That is to say all structure strings should have structure information in the structure mode and
+That is to say, all structure strings should have structure information in the structure mode and
 no "S" in composition strings in the composition mode.
 
 ### Post-Filtering
 
 Not all derived traits are informative.
 For example, some traits might have the same value for all samples.
 Some traits might be highly correlated with others.
 
 GlyTrait carries out a two-step post-filtering process to remove these uninformative traits.
 First, traits with the same value for all samples will be removed.
 Second, highly correlated traits will be pruned,
 keeping only the traits considering more glycans.
 
 GlyTrait filters out highly correlated traits, using a "trait family tree" filtering method.
-Briefly, for a two correlated traits, the "parent" trait,
+Briefly, for two correlated traits, the "parent" trait,
 which normally considers more glycans, will be kept.
-For example, for the two high correlated traits: A2FG and A2G, the latter will be kept,
+For example, for the two high-correlated traits: A2FG and A2G, the latter will be kept 
 because it is more general, and more robust for considering more glycans.
 Thanks to the dynamic "trait family tree" generated by GlyTrait,
 user-defined traits will also be considered in this filtering process.
 
-By default, GlyTrait only filtering trarits with Pearson correlation coefficient of 1,
-i.e. traits with perfect collinearity.
+By default, GlyTrait only filters trarits with Pearson correlation coefficient of 1,
+i.e., traits with perfect collinearity.
 This threshold can be changed by the "-c" or "--corr-threshold" option:
 
 ```shell
 glytrait abundance.csv structure.csv -c 0.9
 ```
 
 Setting the threshold to -1 will turn off the colinearity filtering.
```

### Comparing `glytrait-0.1.0/pyproject.toml` & `glytrait-0.1.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "glytrait"
-version = "0.1.0"
-description = ""
+version = "0.1.1"
+description = "A tool for calculating derived traits for N-glycome"
 authors = ["fubin1999 <65430559+fubin1999@users.noreply.github.com>"]
 readme = "README.md"
 
 [[tool.poetry.source]]
 name = "aliyun"
 url = "http://mirrors.aliyun.com/pypi/simple"
 priority = "default"
@@ -33,14 +33,15 @@
 pytest = "^7.3.1"
 coverage = "^7.2.6"
 pytest-mock = "^3.10.0"
 mypy = "^1.7.1"
 pandas-stubs = "^2.1.1.230928"
 black = "^24.1.1"
 hypothesis = "^6.100.1"
+pytest-cov = "^5.0.0"
 
 [tool.poetry.scripts]
 glytrait = "glytrait.cli:cli"
 
 [tool.mypy]
 
 [[tool.mypy.overrides]]
```

### Comparing `glytrait-0.1.0/src/glytrait/api.py` & `glytrait-0.1.1/src/glytrait/api.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-from typing import Literal, Optional
+from typing import cast, Literal, Optional
 
 import pandas as pd
 from attrs import define, field
 
 from glytrait.data_export import export_all
-from glytrait.data_type import MetaPropertyTable, DerivedTraitTable
-from glytrait.formula import TraitFormula, load_formulas
+from glytrait.data_type import MetaPropertyTable, DerivedTraitTable, GroupSeries
+from glytrait.formula import TraitFormula, load_formulas, load_default_formulas
 from glytrait.load_data import load_input_data_from_csv, GlyTraitInputData
 from glytrait.meta_property import build_meta_property_table
 from glytrait.post_filtering import post_filter
 from glytrait.preprocessing import preprocess
 from glytrait.trait import calcu_derived_trait
 from glytrait.stat import t_test, anova
 
@@ -54,19 +54,23 @@
         ...     glycan_file="glycan_structure.csv",
         ...     group_file="group.csv",
         ... )
     """
 
     def __init__(self, **kwargs):
         self._config = _Config(**kwargs)
-        self._formulas: list[TraitFormula] = load_formulas(
-            self._config.mode,
-            self._config.custom_formula_file,
-            self._config.sia_linkage,
-        )
+        self._formulas = self._init_formulas()
+
+    def _init_formulas(self) -> list[TraitFormula]:
+        if self._config.custom_formula_file is not None:
+            return load_formulas(
+                self._config.custom_formula_file, self._config.sia_linkage
+            )
+        else:
+            return load_default_formulas(self._config.mode, self._config.sia_linkage)
 
     def run(
         self,
         output_dir: str,
         abundance_file: str,
         glycan_file: str,
         group_file: Optional[str] = None,
@@ -152,21 +156,23 @@
             trait_df=derived_trait_table,
             threshold=self._config.correlation_threshold,
             method="pearson",
         )
 
     def _diff_analysis(
         self,
-        derived_trait_table: DerivedTraitTable,
+        derived_trait_table: DerivedTraitTable | None,
         input_data: GlyTraitInputData,
     ) -> dict[str, pd.DataFrame]:
-        if input_data.groups.unique().size == 2:
-            return {"t_test.csv": t_test(derived_trait_table, input_data.groups)}
+        groups = cast(GroupSeries, input_data.groups)
+        trait_table = cast(DerivedTraitTable, derived_trait_table)
+        if groups.unique().size == 2:
+            return {"t_test.csv": t_test(trait_table, groups)}
         else:  # groups size > 2
-            anova_df, post_hoc_df = anova(derived_trait_table, input_data.groups)
+            anova_df, post_hoc_df = anova(trait_table, groups)
             return {"anova.csv": anova_df, "post_hoc.csv": post_hoc_df}
 
     def _export_data(
         self,
         output_dir: str,
         input_data: GlyTraitInputData,
         meta_property_table: MetaPropertyTable,
```

### Comparing `glytrait-0.1.0/src/glytrait/cli.py` & `glytrait-0.1.1/src/glytrait/cli.py`

 * *Files identical despite different names*

### Comparing `glytrait-0.1.0/src/glytrait/data_export.py` & `glytrait-0.1.1/src/glytrait/data_export.py`

 * *Files identical despite different names*

### Comparing `glytrait-0.1.0/src/glytrait/data_type.py` & `glytrait-0.1.1/src/glytrait/data_type.py`

 * *Files identical despite different names*

### Comparing `glytrait-0.1.0/src/glytrait/exception.py` & `glytrait-0.1.1/src/glytrait/exception.py`

 * *Files identical despite different names*

### Comparing `glytrait-0.1.0/src/glytrait/formula.py` & `glytrait-0.1.1/src/glytrait/formula.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 from attrs import field, define
 
 from glytrait.data_type import AbundanceTable, MetaPropertyTable
 
 __all__ = [
     "TraitFormula",
     "load_formulas",
+    "load_default_formulas",
     "save_builtin_formula",
 ]
 
 from glytrait.exception import GlyTraitError
 
 default_struc_formula_file = files("glytrait.resources").joinpath("struc_formula.txt")
 default_comp_formula_file = files("glytrait.resources").joinpath("comp_formula.txt")
@@ -759,68 +760,59 @@
         if description is not None:
             raise FormulaFileError(
                 f"No expression follows description '{description}'."
             )
 
 
 def load_formulas(
-    type_: Literal["structure", "composition"],
-    user_file: Optional[str] = None,
+    file: str,
     sia_linkage: bool = False,
 ) -> list[TraitFormula]:
-    """Load both the default formulas and the user-defined formulas.
+    """Load formulas from a formula file.
 
     Args:
-        type_ (Literal["structure", "composition"]): The type of the formulas.
-        user_file (Optional[str], optional): The path of the user-defined formula file.
-            Defaults to None.
-        sia_linkage (bool, optional): Whether to include formulas with sia-linkage
+        file: The path of the formula file.
+        sia_linkage: Whether to include formulas with sia-linkage
             meta-properties. Defaults to False.
 
     Returns:
         list[TraitFormula]: The formulas.
 
     Raises:
         FormulaFileError: If the formula file is in a wrong format.
         FormulaParseError: If a formula string cannot be parsed.
     """
-    formulas = list(load_default_formulas(type_=type_))
-
-    if user_file is not None:
-        default_formula_names = {f.name for f in formulas}
-        user_formulas = FormulaFileParser().parse(user_file)
-        for f in user_formulas:
-            if f.name in default_formula_names:
-                continue
-            formulas.append(f)
-
+    formulas = [f for f in FormulaFileParser().parse(file)]
     if not sia_linkage:
         formulas = [f for f in formulas if not f.sia_linkage]
     return formulas
 
 
 def load_default_formulas(
-    type_: Literal["structure", "composition"]
-) -> Generator[TraitFormula, None, None]:
+    mode: Literal["structure", "composition"],
+    sia_linkage: bool = False,
+) -> list[TraitFormula]:
     """Load the default formulas.
 
     Args:
-        type_ (Literal["structure", "composition"]): The type of the formulas.
+        mode: The type of the formulas.
+        sia_linkage: Whether to include formulas with sia-linkage
+            meta-properties. Defaults to False.
 
-    Yields:
-        The formulas parsed.
+    Returns:
+        list[TraitFormula]: The formulas.
     """
-    if type_ == "composition":
+    if mode == "composition":
         file_traversable = default_comp_formula_file
-    elif type_ == "structure":
+    elif mode == "structure":
         file_traversable = default_struc_formula_file
     else:
         raise ValueError("Invalid formula type.")
     with as_file(file_traversable) as file:
-        yield from FormulaFileParser().parse(str(file))
+        return load_formulas(str(file), sia_linkage=sia_linkage)
 
 
 def save_builtin_formula(dirpath: str | Path) -> None:
     """Copy the builtin formula file to the given path.
 
     Args:
         dirpath (str): The path to save the built-in formula file.
```

### Comparing `glytrait-0.1.0/src/glytrait/glycan.py` & `glytrait-0.1.1/src/glytrait/glycan.py`

 * *Files identical despite different names*

### Comparing `glytrait-0.1.0/src/glytrait/load_data.py` & `glytrait-0.1.1/src/glytrait/load_data.py`

 * *Files identical despite different names*

### Comparing `glytrait-0.1.0/src/glytrait/meta_property.py` & `glytrait-0.1.1/src/glytrait/meta_property.py`

 * *Files identical despite different names*

### Comparing `glytrait-0.1.0/src/glytrait/post_filtering.py` & `glytrait-0.1.1/src/glytrait/post_filtering.py`

 * *Files identical despite different names*

### Comparing `glytrait-0.1.0/src/glytrait/preprocessing.py` & `glytrait-0.1.1/src/glytrait/preprocessing.py`

 * *Files identical despite different names*

### Comparing `glytrait-0.1.0/src/glytrait/resources/comp_formula.txt` & `glytrait-0.1.1/src/glytrait/resources/comp_formula.txt`

 * *Files identical despite different names*

### Comparing `glytrait-0.1.0/src/glytrait/resources/struc_formula.txt` & `glytrait-0.1.1/src/glytrait/resources/struc_formula.txt`

 * *Files identical despite different names*

### Comparing `glytrait-0.1.0/src/glytrait/stat.py` & `glytrait-0.1.1/src/glytrait/stat.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,16 +58,15 @@
 
 
 def _prepare_for_anova(
     trait_df: DerivedTraitTable, groups: GroupSeries
 ) -> pd.DataFrame:
     """Combine the trait data and group information."""
     groups = groups.rename("group")
-    trait_df = trait_df.merge(groups, left_index=True, right_index=True)
-    return trait_df
+    return trait_df.merge(groups, left_index=True, right_index=True)
 
 
 def _anova(prepared_df: pd.DataFrame, trait_names: list[str]) -> pd.DataFrame:
     """Perform ANOVA for the trait data.
 
     Args:
         prepared_df: Dataframe containing the trait data and group information.
```

### Comparing `glytrait-0.1.0/src/glytrait/trait.py` & `glytrait-0.1.1/src/glytrait/trait.py`

 * *Files identical despite different names*

### Comparing `glytrait-0.1.0/PKG-INFO` & `glytrait-0.1.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: glytrait
-Version: 0.1.0
-Summary: 
+Version: 0.1.1
+Summary: A tool for calculating derived traits for N-glycome
 Author: fubin1999
 Author-email: 65430559+fubin1999@users.noreply.github.com
 Requires-Python: >=3.10,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
@@ -19,105 +19,143 @@
 Requires-Dist: pingouin (>=0.5.3,<0.6.0)
 Description-Content-Type: text/markdown
 
 ![logo](img/logo.png)
 
 # GlyTrait
 
+[![PyPI - Version](https://img.shields.io/pypi/v/glytrait)](https://pypi.org/project/glytrait/)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/glytrait)
+[![GitHub License](https://img.shields.io/github/license/fubin1999/glytrait)](https://github.com/fubin1999/glytrait/blob/main/LICENSE)
+[![Coverage Status](https://coveralls.io/repos/github/fubin1999/glytrait/badge.svg?branch=main)](https://coveralls.io/github/fubin1999/glytrait?branch=main)
+[![Codacy Badge](https://app.codacy.com/project/badge/Grade/e3e6a19dccb749f786264247738fa585)](https://app.codacy.com/gh/fubin1999/glytrait/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_grade)
+
 ## Overview
 
-Glycan derived trait is a more insightful way to analysis glycomics data.
-However, currently there lacks a tool for automatically calculating derived traits,
-while mannual calculating is cumbersome, time-consuming and error-prone.
-GlyTrait is a tool designed for calculating N-glycan traits merely from abundance information and
-glycan structures.
+*Q: What is GlyTrait?*
+
+*A: GlyTrait is a tool for calculating derived traits for N-glycomic data.*
+
+*Q: Sounds cool! So..., what are derived traits again?*
+
+*A: Well, derived traits are artificial variables that summarize certain aspects of 
+the glycome. 
+For example, the proportion of core-fucosylated glycans, 
+the average number of sialic acids per glycan, 
+or the proportion of bisected glycans within bi-antennary complex glycans, etc. 
+Derived traits are more biologically relavant 
+and have been used a lot in the glycomics community.*
+
+*Q: So, GlyTrait does the dirty work for me, 
+saving my time and energy for more interesting analysis?*
+
+*A: You bet!*
 
 ## Contents
 
 - [Installation](#installation)
     - [Requirement](#requirement)
     - [Using pipx (recommended)](#using-pipx-recommended)
 - [Usage](#usage)
     - [Quick start](#quick-start)
     - [Options](#options)
     - [Mode](#mode)
     - [Input file format](#input-file-format)
-    - [Specify output path](#specify-output-path)
-    - [Structure file](#structure-file)
+    - [Specify output path](#specify-the-output-path)
     - [Preprocessing](#preprocessing)
     - [Sialic-acid-linkage traits](#sialic-acid-linkage-traits)
     - [Post-filtering](#post-filtering)
 - [License](#license)
 
+## Web app
+
+> Let there be no command line apps!
+> 
+> -- my colleagues
+
+A web app version of GlyTrait is on its way here...
+Ready to say goodbye to the command line?
+
 ## Installation
 
 ### Requirement
 
 ```
 python >= 3.10
 ```
 
-If python hasn't been install, download it from
-its [its website](https://www.bing.com/search?q=python&form=APMCS1&PC=APMC), or
-use [Anaconda](https://www.anaconda.com/download/) if you like.
+If python hasn't been installed, 
+download it from [its website](https://www.bing.com/search?q=python&form=APMCS1&PC=APMC),
+or use [Anaconda](https://www.anaconda.com/download/) if you like.
 
-### Using pipx (recommended)
+### Option 1: Using pipx (recommended)
 
-pipx is a tool to help you install and run end-user applications written in Python.
+`pipx` is a tool to help you install and run end-user applications written in Python.
 It's roughly similar to macOS's brew, JavaScript's npx, and Linux's apt.
 
 #### Install pipx
 
 Install pipx following its [Document](https://pypa.github.io/pipx/installation/).
 
 #### Install GlyTrait from PyPi
 
 ```shell
 pipx install glytrait
 ```
 
-### Using Conda environment
+### Option 2: Using pip
 
-#### Create a new environment
+#### 1. Create a new conda environment (optional)
 
 ```shell
 conda create -n glytrait python=3.10
 ```
 
-#### Activate the environment
+and activate the environment.
 
 ```shell
 conda activate glytrait
 ```
 
-#### Install GlyTrait from PyPi
+#### 2. Install GlyTrait from PyPi
 
 ```shell
 pip install glytrait
 ```
 
 ## Usage
 
 ### Quick start
 
-Download the example files: (to be added).
+1. Download the [example files](https://github.com/fubin1999/glytrait/tree/main/example_data)
+to a new directory: `glytrait_example`.
+
+2. Open a terminal and navigate to the directory:
+
+```shell
+cd glytrait_example
+```
+
+3. Run the following command:
 
 ```shell
 glytrait abundance.csv structures.csv
 ```
 
 That's it! 
 If everything goes well, a folder named "abundance_glytrait" will be created
 in the same directory with the abundnce.csv file.
 Inside the directory are four files:
 
-1. `derived_traits.csv`: the derived traits calculated by GlyTrait.
-2. `glycan_abundance_processed.csv`: the glycan abundance after preprocessing.
-3. `meta_properties.csv`: the meta properties of all glycans.
-4. `formulas.txt`: the definations of all derived traits.
+1. `derived_traits.csv`: all derived traits calculated by GlyTrait.
+2. `derived_traits_filtered.csv`: derived traits after post-filtering 
+   (see [Post-filtering](#post-filtering)).
+3. `glycan_abundance_processed.csv`: the glycan abundance after preprocessing
+   (see [Preprocessing](#preprocessing)).
+4. `meta_properties.csv`: the meta-properties of all glycans.
 
 The detailed format of the input file will be introduced in the
 [Input file format](#input-file-format) section.
 
 ### Options
 
 *This section is intended to give an overview of the CLI interface.
@@ -152,15 +190,16 @@
 Note that the "composition" mode has uncertainties to some extent. Specifically:
 
 1. Estimating the number of Gal based on composition is not possible for hybrid glycans,
    so GlyTrait will calculate the number of Gal assuming there are no hybrid glycans.
    kily, hybrid glycans are usually in low abundance,
    so the algorithm is a good approximation for most cases.
 2. Estimating the number of branches is not possible based on composition,
-   so GlyTrait will roughly classify glycans into 2 categories: low-branching and high-branching.
+   so GlyTrait will roughly classify glycans into two categories: 
+   low-branching and high-branching.
    Glycans with N > 4 (including bisecting diantenary glycans) are considered as high-branching,
    while others as low-branching.
 3. Telling hybrid glycans from mono-antenary complex glycans is not possible based on composition,
    so GlyTrait will not classify glycans into complex, hybrid and high-mannose.
 
 Due to the ambiguities above, we recommend using the "structure" mode if possible.
 
@@ -186,23 +225,23 @@
 At least two files are needed for GlyTrait to work:
 
 #### 1. The abundance file
 
 A csv file with samples as rows and glycan IDs as columns.
 An example file would be like:
 
-| Sample | Glycan1 | Glycan2 | Glycan3 |
-|--------|---------|---------|---------|
+| Sample  | Glycan1 | Glycan2 | Glycan3 |
+|---------|---------|---------|---------|
 | Sample1 | 0.0417  | 0.0503  | 0.0354  |
 | Sample2 | 0.0233  | 0.0533  | 0.0593  |
 | Sample3 | 0.0123  | 0.0133  | 0.0194  |
 
 The header of the first column should be "Sample",
 and the header of the other columns should be glycan IDs.
-Glycan IDs can be any string, e.g. the composition strings ("H3N4").
+Glycan IDs can be any string, e.g., the composition strings ("H3N4").
 
 **Both glycan IDs and samples should be unique.**
 
 #### 2. The structure file (or the composition file)
 
 A csv file with two columns: "GlycanID" and "Structure" (or "Composition").
 An example file would be like:
@@ -216,15 +255,15 @@
 The "GlycanID" column should contain all glycan IDs in the abundance file.
 The "Structure" column should contain the structure strings of the glycans.
 For now, only the GlycoCT format is supported.
 In the "composition" mode, the second column should be "Composition" instead of "Structure",
 and the composition strings should be used instead of the structure strings.
 Condensed format ("H3N4F1S1") is supported.
 
-### Specify output path
+### Specify the output path
 
 You might have noticed before that GlyTrait saves the output file to the same directory 
 as the abundance file with a "_glytrait" suffix.
 You can specify the output file path by using the "-o" or "--output-file" option:
 
 ```shell
 glytrait abundance.csv structure.csv -o output
@@ -248,15 +287,15 @@
 glytrait abundance.csv structure.csv -r 0.5
 ```
 
 The imputation method could be specified by the "-i" or the "--impute-method" option.
 The default method is "zero",
 which means missing values will be imputed by 0.
 Other supported methods are "mean", "median", "zero", "lod".
-You can change imputation method to "min" by:
+You can change the imputation method to "min" by:
 
 ```shell
 glytrait abundance.csv structure.csv -i min
 ```
 
 A full list of supported imputation methods are:
 
@@ -265,61 +304,61 @@
 - "median": impute missing values by the median value of a glycan within all samples.
 - "zero": impute missing values by 0.
 - "lod": impute missing values by the limit of detection (LOD) of the equipment. The LOD of a
   glycan is defined as the minimum value of the glycan within all samples divided by 5.
 
 ### Sialic-acid-linkage traits
 
-Sialic acids can have different linkages for N-glycans (e.g. α2,3 and α2,6).
+Sialic acids can have different linkages for N-glycans (e.g., α2,3 and α2,6).
 Different sialic acid linkage has different biological functions.
 GlyTrait supports calculating derived traits regarding these linkages.
 To use this feature, you need to have siaic acid linkage information.
 
 In the structure mode, the "Structure" column or the structure file should contain the linkage
 information.
 Only linkage information about sialic acids is needed.
 This can be easily done using GlycoWorkbench.
 
 In the composition mode, the "Composition" column must contain the linkage information.
 GlyTrait uses a common notation for sialic acid with different linkages:
 "E" for a2,6-linked sialic acids, and "L" a2,3-linked sialic acids.
-For example, "H5N4F1E1L1" contains 2 sialic acids, one is a2,6-linked and the other is
-a2,3-linked.
+For example, "H5N4F1E1L1" contains two sialic acids, one is a2,6-linked, 
+and the other is a2,3-linked.
 
 You can use the "-l" or "--sia-linkage" option to include sialic-acid-linkage traits:
 
 ```shell
 glytrait abundance.csv structure.csv -l
 ```
 
 Note that if you use this option, all glycans with sialic acids should have linkage information.
-That is to say all structure strings should have structure information in the structure mode and
+That is to say, all structure strings should have structure information in the structure mode and
 no "S" in composition strings in the composition mode.
 
 ### Post-Filtering
 
 Not all derived traits are informative.
 For example, some traits might have the same value for all samples.
 Some traits might be highly correlated with others.
 
 GlyTrait carries out a two-step post-filtering process to remove these uninformative traits.
 First, traits with the same value for all samples will be removed.
 Second, highly correlated traits will be pruned,
 keeping only the traits considering more glycans.
 
 GlyTrait filters out highly correlated traits, using a "trait family tree" filtering method.
-Briefly, for a two correlated traits, the "parent" trait,
+Briefly, for two correlated traits, the "parent" trait,
 which normally considers more glycans, will be kept.
-For example, for the two high correlated traits: A2FG and A2G, the latter will be kept,
+For example, for the two high-correlated traits: A2FG and A2G, the latter will be kept 
 because it is more general, and more robust for considering more glycans.
 Thanks to the dynamic "trait family tree" generated by GlyTrait,
 user-defined traits will also be considered in this filtering process.
 
-By default, GlyTrait only filtering trarits with Pearson correlation coefficient of 1,
-i.e. traits with perfect collinearity.
+By default, GlyTrait only filters trarits with Pearson correlation coefficient of 1,
+i.e., traits with perfect collinearity.
 This threshold can be changed by the "-c" or "--corr-threshold" option:
 
 ```shell
 glytrait abundance.csv structure.csv -c 0.9
 ```
 
 Setting the threshold to -1 will turn off the colinearity filtering.
```

