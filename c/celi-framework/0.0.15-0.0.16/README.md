# Comparing `tmp/celi_framework-0.0.15.tar.gz` & `tmp/celi_framework-0.0.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "celi_framework-0.0.15.tar", max compression
+gzip compressed data, was "celi_framework-0.0.16.tar", max compression
```

## Comparing `celi_framework-0.0.15.tar` & `celi_framework-0.0.16.tar`

### file list

```diff
@@ -1,56 +1,56 @@
--rw-r--r--   0        0        0     1084 2024-04-19 04:39:20.595103 celi_framework-0.0.15/LICENSE
--rw-r--r--   0        0        0    12809 2024-04-19 04:39:20.595103 celi_framework-0.0.15/README.md
--rw-r--r--   0        0        0    10399 2024-04-19 04:39:20.595103 celi_framework-0.0.15/celi_framework/core/job_description.py
--rw-r--r--   0        0        0    23124 2024-04-19 04:39:20.595103 celi_framework-0.0.15/celi_framework/core/monitor.py
--rw-r--r--   0        0        0    11301 2024-04-19 04:39:20.595103 celi_framework-0.0.15/celi_framework/core/mt_factory.py
--rw-r--r--   0        0        0    14719 2024-04-19 04:39:20.595103 celi_framework-0.0.15/celi_framework/core/post_monitor.py
--rw-r--r--   0        0        0    59120 2024-04-19 04:39:20.595103 celi_framework-0.0.15/celi_framework/core/processor.py
--rw-r--r--   0        0        0     3060 2024-04-19 04:39:20.595103 celi_framework-0.0.15/celi_framework/core/runner.py
--rw-r--r--   0        0        0    23630 2024-04-19 04:39:20.595103 celi_framework-0.0.15/celi_framework/core/templates.py
--rw-r--r--   0        0        0    13793 2024-04-19 04:39:20.595103 celi_framework-0.0.15/celi_framework/examples/reporting_template/job_description.py
--rw-r--r--   0        0        0    10317 2024-04-19 04:39:20.595103 celi_framework-0.0.15/celi_framework/examples/reporting_template/tools.py
--rw-r--r--   0        0        0     6133 2024-04-19 04:39:20.595103 celi_framework-0.0.15/celi_framework/examples/wikipedia/Index_cache.py
--rw-r--r--   0        0        0     7694 2024-04-19 04:39:20.595103 celi_framework-0.0.15/celi_framework/examples/wikipedia/caching_beautiful_soup_reader.py
--rw-r--r--   0        0        0     5552 2024-04-19 04:39:20.595103 celi_framework-0.0.15/celi_framework/examples/wikipedia/eval/run_eval.py
--rw-r--r--   0        0        0      530 2024-04-19 04:39:20.595103 celi_framework-0.0.15/celi_framework/examples/wikipedia/eval/test_sets.json
--rw-r--r--   0        0        0      851 2024-04-19 04:39:20.595103 celi_framework-0.0.15/celi_framework/examples/wikipedia/eval/test_sets_large.json
--rw-r--r--   0        0        0      161 2024-04-19 04:39:20.595103 celi_framework-0.0.15/celi_framework/examples/wikipedia/example_config.json
--rw-r--r--   0        0        0    13742 2024-04-19 04:39:20.595103 celi_framework-0.0.15/celi_framework/examples/wikipedia/index.py
--rw-r--r--   0        0        0    13330 2024-04-19 04:39:20.595103 celi_framework-0.0.15/celi_framework/examples/wikipedia/job_description.py
--rw-r--r--   0        0        0     7111 2024-04-19 04:39:20.595103 celi_framework-0.0.15/celi_framework/examples/wikipedia/loader.py
--rw-r--r--   0        0        0    14758 2024-04-19 04:39:20.595103 celi_framework-0.0.15/celi_framework/examples/wikipedia/tools.py
--rw-r--r--   0        0        0      549 2024-04-19 04:39:20.595103 celi_framework-0.0.15/celi_framework/examples/wikipedia/wikipedia_utils.py
--rw-r--r--   0        0        0    12668 2024-04-19 04:39:20.595103 celi_framework-0.0.15/celi_framework/experimental/embeddor.py
--rw-r--r--   0        0        0     7936 2024-04-19 04:39:20.595103 celi_framework-0.0.15/celi_framework/experimental/mapper.py
--rw-r--r--   0        0        0     1354 2024-04-19 04:39:20.595103 celi_framework-0.0.15/celi_framework/experimental/mechanic.py
--rw-r--r--   0        0        0        0 2024-04-19 04:39:20.595103 celi_framework-0.0.15/celi_framework/experimental/preprocessing/__init__.py
--rw-r--r--   0        0        0    23634 2024-04-19 04:39:20.595103 celi_framework-0.0.15/celi_framework/experimental/preprocessing/pre-processor.py
--rw-r--r--   0        0        0       94 2024-04-19 04:39:20.595103 celi_framework-0.0.15/celi_framework/experimental/preprocessing/word_pdf_extractors/__init__.py
--rw-r--r--   0        0        0     8832 2024-04-19 04:39:20.595103 celi_framework-0.0.15/celi_framework/experimental/preprocessing/word_pdf_extractors/extract_pdf_tables.py
--rw-r--r--   0        0        0     2056 2024-04-19 04:39:20.595103 celi_framework-0.0.15/celi_framework/experimental/preprocessing/word_pdf_extractors/extractor_helpers.py
--rw-r--r--   0        0        0    10669 2024-04-19 04:39:20.595103 celi_framework-0.0.15/celi_framework/experimental/preprocessing/word_pdf_extractors/pdf_extractor.py
--rw-r--r--   0        0        0     7835 2024-04-19 04:39:20.595103 celi_framework-0.0.15/celi_framework/experimental/preprocessing/word_pdf_extractors/word_extractor.py
--rw-r--r--   0        0        0     5471 2024-04-19 04:39:20.599103 celi_framework-0.0.15/celi_framework/experimental/task_builder/factory.py
--rw-r--r--   0        0        0     4242 2024-04-19 04:39:20.599103 celi_framework-0.0.15/celi_framework/experimental/task_builder/llm_helper_funcs.py
--rw-r--r--   0        0        0     4352 2024-04-19 04:39:20.599103 celi_framework-0.0.15/celi_framework/experimental/task_builder/llms.py
--rw-r--r--   0        0        0     5939 2024-04-19 04:39:20.599103 celi_framework-0.0.15/celi_framework/experimental/task_builder/template.py
--rw-r--r--   0        0        0     9914 2024-04-19 04:39:20.599103 celi_framework-0.0.15/celi_framework/experimental/utils/ada.py
--rw-r--r--   0        0        0    19041 2024-04-19 04:39:20.599103 celi_framework-0.0.15/celi_framework/experimental/utils/mapper_utils.py
--rw-r--r--   0        0        0    13615 2024-04-19 04:39:20.599103 celi_framework-0.0.15/celi_framework/experimental/utils/nougat_preprocessing/preprocess.py
--rw-r--r--   0        0        0     5118 2024-04-19 04:39:20.599103 celi_framework-0.0.15/celi_framework/experimental/utils/nougat_preprocessing/preprocessing_templates.py
--rw-r--r--   0        0        0     5458 2024-04-19 04:39:20.599103 celi_framework-0.0.15/celi_framework/experimental/utils/postprocessor_utils.py
--rw-r--r--   0        0        0     9091 2024-04-19 04:39:20.599103 celi_framework-0.0.15/celi_framework/experimental/utils/synthetic_data.py
--rw-r--r--   0        0        0     1350 2024-04-19 04:39:20.599103 celi_framework-0.0.15/celi_framework/logging_config.json
--rw-r--r--   0        0        0     2171 2024-04-19 04:39:20.599103 celi_framework-0.0.15/celi_framework/logging_setup.py
--rw-r--r--   0        0        0     6749 2024-04-19 04:39:20.599103 celi_framework-0.0.15/celi_framework/main.py
--rw-r--r--   0        0        0        0 2024-04-19 04:39:20.599103 celi_framework-0.0.15/celi_framework/utils/__init__.py
--rw-r--r--   0        0        0    10889 2024-04-19 04:39:20.599103 celi_framework-0.0.15/celi_framework/utils/codex.py
--rw-r--r--   0        0        0      461 2024-04-19 04:39:20.599103 celi_framework-0.0.15/celi_framework/utils/exceptions.py
--rw-r--r--   0        0        0    22485 2024-04-19 04:39:20.599103 celi_framework-0.0.15/celi_framework/utils/llmcore_utils.py
--rw-r--r--   0        0        0    10021 2024-04-19 04:39:20.599103 celi_framework-0.0.15/celi_framework/utils/llms.py
--rw-r--r--   0        0        0       77 2024-04-19 04:39:20.599103 celi_framework-0.0.15/celi_framework/utils/log.py
--rw-r--r--   0        0        0    10717 2024-04-19 04:39:20.599103 celi_framework-0.0.15/celi_framework/utils/sql_utils.py
--rw-r--r--   0        0        0    10871 2024-04-19 04:39:20.599103 celi_framework-0.0.15/celi_framework/utils/token_counters.py
--rw-r--r--   0        0        0    28482 2024-04-19 04:39:20.599103 celi_framework-0.0.15/celi_framework/utils/utils.py
--rw-r--r--   0        0        0     1758 2024-04-19 04:39:51.667319 celi_framework-0.0.15/pyproject.toml
--rw-r--r--   0        0        0    14245 1970-01-01 00:00:00.000000 celi_framework-0.0.15/PKG-INFO
+-rw-r--r--   0        0        0     1084 2024-04-20 10:52:01.230640 celi_framework-0.0.16/LICENSE
+-rw-r--r--   0        0        0    12984 2024-04-20 10:52:01.230640 celi_framework-0.0.16/README.md
+-rw-r--r--   0        0        0    10399 2024-04-20 10:52:01.230640 celi_framework-0.0.16/celi_framework/core/job_description.py
+-rw-r--r--   0        0        0    23124 2024-04-20 10:52:01.230640 celi_framework-0.0.16/celi_framework/core/monitor.py
+-rw-r--r--   0        0        0    11301 2024-04-20 10:52:01.230640 celi_framework-0.0.16/celi_framework/core/mt_factory.py
+-rw-r--r--   0        0        0    14719 2024-04-20 10:52:01.230640 celi_framework-0.0.16/celi_framework/core/post_monitor.py
+-rw-r--r--   0        0        0    59120 2024-04-20 10:52:01.230640 celi_framework-0.0.16/celi_framework/core/processor.py
+-rw-r--r--   0        0        0     3060 2024-04-20 10:52:01.230640 celi_framework-0.0.16/celi_framework/core/runner.py
+-rw-r--r--   0        0        0    23630 2024-04-20 10:52:01.230640 celi_framework-0.0.16/celi_framework/core/templates.py
+-rw-r--r--   0        0        0    13793 2024-04-20 10:52:01.230640 celi_framework-0.0.16/celi_framework/examples/reporting_template/job_description.py
+-rw-r--r--   0        0        0    10317 2024-04-20 10:52:01.230640 celi_framework-0.0.16/celi_framework/examples/reporting_template/tools.py
+-rw-r--r--   0        0        0     6133 2024-04-20 10:52:01.230640 celi_framework-0.0.16/celi_framework/examples/wikipedia/Index_cache.py
+-rw-r--r--   0        0        0     7694 2024-04-20 10:52:01.230640 celi_framework-0.0.16/celi_framework/examples/wikipedia/caching_beautiful_soup_reader.py
+-rw-r--r--   0        0        0     5552 2024-04-20 10:52:01.230640 celi_framework-0.0.16/celi_framework/examples/wikipedia/eval/run_eval.py
+-rw-r--r--   0        0        0      530 2024-04-20 10:52:01.230640 celi_framework-0.0.16/celi_framework/examples/wikipedia/eval/test_sets.json
+-rw-r--r--   0        0        0      851 2024-04-20 10:52:01.230640 celi_framework-0.0.16/celi_framework/examples/wikipedia/eval/test_sets_large.json
+-rw-r--r--   0        0        0      161 2024-04-20 10:52:01.230640 celi_framework-0.0.16/celi_framework/examples/wikipedia/example_config.json
+-rw-r--r--   0        0        0    13876 2024-04-20 10:52:01.230640 celi_framework-0.0.16/celi_framework/examples/wikipedia/index.py
+-rw-r--r--   0        0        0    13330 2024-04-20 10:52:01.230640 celi_framework-0.0.16/celi_framework/examples/wikipedia/job_description.py
+-rw-r--r--   0        0        0     7111 2024-04-20 10:52:01.230640 celi_framework-0.0.16/celi_framework/examples/wikipedia/loader.py
+-rw-r--r--   0        0        0    14758 2024-04-20 10:52:01.230640 celi_framework-0.0.16/celi_framework/examples/wikipedia/tools.py
+-rw-r--r--   0        0        0      549 2024-04-20 10:52:01.230640 celi_framework-0.0.16/celi_framework/examples/wikipedia/wikipedia_utils.py
+-rw-r--r--   0        0        0    12668 2024-04-20 10:52:01.230640 celi_framework-0.0.16/celi_framework/experimental/embeddor.py
+-rw-r--r--   0        0        0     7936 2024-04-20 10:52:01.230640 celi_framework-0.0.16/celi_framework/experimental/mapper.py
+-rw-r--r--   0        0        0     1354 2024-04-20 10:52:01.230640 celi_framework-0.0.16/celi_framework/experimental/mechanic.py
+-rw-r--r--   0        0        0        0 2024-04-20 10:52:01.230640 celi_framework-0.0.16/celi_framework/experimental/preprocessing/__init__.py
+-rw-r--r--   0        0        0    23634 2024-04-20 10:52:01.230640 celi_framework-0.0.16/celi_framework/experimental/preprocessing/pre-processor.py
+-rw-r--r--   0        0        0       94 2024-04-20 10:52:01.230640 celi_framework-0.0.16/celi_framework/experimental/preprocessing/word_pdf_extractors/__init__.py
+-rw-r--r--   0        0        0     8832 2024-04-20 10:52:01.230640 celi_framework-0.0.16/celi_framework/experimental/preprocessing/word_pdf_extractors/extract_pdf_tables.py
+-rw-r--r--   0        0        0     2056 2024-04-20 10:52:01.230640 celi_framework-0.0.16/celi_framework/experimental/preprocessing/word_pdf_extractors/extractor_helpers.py
+-rw-r--r--   0        0        0    10669 2024-04-20 10:52:01.230640 celi_framework-0.0.16/celi_framework/experimental/preprocessing/word_pdf_extractors/pdf_extractor.py
+-rw-r--r--   0        0        0     7835 2024-04-20 10:52:01.230640 celi_framework-0.0.16/celi_framework/experimental/preprocessing/word_pdf_extractors/word_extractor.py
+-rw-r--r--   0        0        0     5471 2024-04-20 10:52:01.230640 celi_framework-0.0.16/celi_framework/experimental/task_builder/factory.py
+-rw-r--r--   0        0        0     4242 2024-04-20 10:52:01.230640 celi_framework-0.0.16/celi_framework/experimental/task_builder/llm_helper_funcs.py
+-rw-r--r--   0        0        0     4352 2024-04-20 10:52:01.230640 celi_framework-0.0.16/celi_framework/experimental/task_builder/llms.py
+-rw-r--r--   0        0        0     5939 2024-04-20 10:52:01.230640 celi_framework-0.0.16/celi_framework/experimental/task_builder/template.py
+-rw-r--r--   0        0        0     9914 2024-04-20 10:52:01.234640 celi_framework-0.0.16/celi_framework/experimental/utils/ada.py
+-rw-r--r--   0        0        0    19041 2024-04-20 10:52:01.234640 celi_framework-0.0.16/celi_framework/experimental/utils/mapper_utils.py
+-rw-r--r--   0        0        0    13615 2024-04-20 10:52:01.234640 celi_framework-0.0.16/celi_framework/experimental/utils/nougat_preprocessing/preprocess.py
+-rw-r--r--   0        0        0     5118 2024-04-20 10:52:01.234640 celi_framework-0.0.16/celi_framework/experimental/utils/nougat_preprocessing/preprocessing_templates.py
+-rw-r--r--   0        0        0     5458 2024-04-20 10:52:01.234640 celi_framework-0.0.16/celi_framework/experimental/utils/postprocessor_utils.py
+-rw-r--r--   0        0        0     9091 2024-04-20 10:52:01.234640 celi_framework-0.0.16/celi_framework/experimental/utils/synthetic_data.py
+-rw-r--r--   0        0        0     1350 2024-04-20 10:52:01.234640 celi_framework-0.0.16/celi_framework/logging_config.json
+-rw-r--r--   0        0        0     2171 2024-04-20 10:52:01.234640 celi_framework-0.0.16/celi_framework/logging_setup.py
+-rw-r--r--   0        0        0     6867 2024-04-20 10:52:01.234640 celi_framework-0.0.16/celi_framework/main.py
+-rw-r--r--   0        0        0        0 2024-04-20 10:52:01.234640 celi_framework-0.0.16/celi_framework/utils/__init__.py
+-rw-r--r--   0        0        0    10889 2024-04-20 10:52:01.234640 celi_framework-0.0.16/celi_framework/utils/codex.py
+-rw-r--r--   0        0        0      461 2024-04-20 10:52:01.234640 celi_framework-0.0.16/celi_framework/utils/exceptions.py
+-rw-r--r--   0        0        0    22485 2024-04-20 10:52:01.234640 celi_framework-0.0.16/celi_framework/utils/llmcore_utils.py
+-rw-r--r--   0        0        0    10021 2024-04-20 10:52:01.234640 celi_framework-0.0.16/celi_framework/utils/llms.py
+-rw-r--r--   0        0        0       77 2024-04-20 10:52:01.234640 celi_framework-0.0.16/celi_framework/utils/log.py
+-rw-r--r--   0        0        0    10717 2024-04-20 10:52:01.234640 celi_framework-0.0.16/celi_framework/utils/sql_utils.py
+-rw-r--r--   0        0        0    10871 2024-04-20 10:52:01.234640 celi_framework-0.0.16/celi_framework/utils/token_counters.py
+-rw-r--r--   0        0        0    28482 2024-04-20 10:52:01.234640 celi_framework-0.0.16/celi_framework/utils/utils.py
+-rw-r--r--   0        0        0     1758 2024-04-20 10:52:32.826746 celi_framework-0.0.16/pyproject.toml
+-rw-r--r--   0        0        0    14420 1970-01-01 00:00:00.000000 celi_framework-0.0.16/PKG-INFO
```

### Comparing `celi_framework-0.0.15/LICENSE` & `celi_framework-0.0.16/LICENSE`

 * *Files identical despite different names*

### Comparing `celi_framework-0.0.15/README.md` & `celi_framework-0.0.16/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,17 @@
 
 - **Scalability:** Designed to accommodate projects of any scale, CELI efficiently processes massive datasets and documents, and produces output of any size, making it an ideal solution for both targeted tasks and large-scale knowledge work automation.
 
 - **Streamlined Document Lifecycle Management:** CELI optimizes the entire lifecycle of document processing, encompassing pre-processing, embedding, synthesis, content generation, and quality monitoring.
 
 - **Development Flexibility:** CELI is architecturally designed to support developers in creating bespoke applications that conform to specific industry standards, including compliance, methodological rigor, and auditing requirements. This fosters innovation in the field of automated knowledge work by providing a scalable framework that integrates seamlessly into enterprise ecosystems.
 
-[Join our Discord server](https://discord.gg/C5SQNdzV) to ask questions or get involved in our project!
+Join our [Discord server](https://discord.gg/C5SQNdzV) to ask questions or get involved in our project!
+
+Read through [our documentation](https://celi.readthedocs.io/en/latest/) for detailed explanations of our codebase.
 
 Note: CELI is currently in alpha. If there are any issues installing, running, or utilizing CELI in your projects please let us know on Discord or create an issue or pull request. We will get back to you promptly.
 
 ## Goals
 
 The CELI (Controller-Embedded Language Interactions) framework aims to empower users across various industries and domains with tools to automate routine and complex tasks efficiently. Our objectives are encapsulated in the following goals:
 
@@ -142,15 +144,15 @@
 Note that running this takes around 30 minutes (give or take).
 
 <!-- end getting-started -->
 
 ## Documentation
 
 Explore the rest of the documentation to learn more about CELI.
-* [Getting Started]() - Learn more about the various ways to run CELI.
+* [Getting Started](https://celi.readthedocs.io/en/stable/getting_started.html) - Learn more about the various ways to run CELI.
 * [Running CELI](https://celi.readthedocs.io/en/stable/running_celi.html) - Learn more about the various ways to run CELI.
 * [New Use Cases](https://celi.readthedocs.io/en/stable/new_use_cases.html) - Learn how to apply CELI to your own use case.
 * [API Reference](https://celi.readthedocs.io/en/stable/reference/index.html) - If you are into reading API docs directly.
 
 ## Discord Server
 
 [Join our Discord server](https://discord.gg/C5SQNdzV) to discuss the project with users, contributors, and project authors.
```

### Comparing `celi_framework-0.0.15/celi_framework/core/job_description.py` & `celi_framework-0.0.16/celi_framework/core/job_description.py`

 * *Files identical despite different names*

### Comparing `celi_framework-0.0.15/celi_framework/core/monitor.py` & `celi_framework-0.0.16/celi_framework/core/monitor.py`

 * *Files identical despite different names*

### Comparing `celi_framework-0.0.15/celi_framework/core/mt_factory.py` & `celi_framework-0.0.16/celi_framework/core/mt_factory.py`

 * *Files identical despite different names*

### Comparing `celi_framework-0.0.15/celi_framework/core/post_monitor.py` & `celi_framework-0.0.16/celi_framework/core/post_monitor.py`

 * *Files identical despite different names*

### Comparing `celi_framework-0.0.15/celi_framework/core/processor.py` & `celi_framework-0.0.16/celi_framework/core/processor.py`

 * *Files identical despite different names*

### Comparing `celi_framework-0.0.15/celi_framework/core/runner.py` & `celi_framework-0.0.16/celi_framework/core/runner.py`

 * *Files identical despite different names*

### Comparing `celi_framework-0.0.15/celi_framework/core/templates.py` & `celi_framework-0.0.16/celi_framework/core/templates.py`

 * *Files identical despite different names*

### Comparing `celi_framework-0.0.15/celi_framework/examples/reporting_template/job_description.py` & `celi_framework-0.0.16/celi_framework/examples/reporting_template/job_description.py`

 * *Files identical despite different names*

### Comparing `celi_framework-0.0.15/celi_framework/examples/reporting_template/tools.py` & `celi_framework-0.0.16/celi_framework/examples/reporting_template/tools.py`

 * *Files identical despite different names*

### Comparing `celi_framework-0.0.15/celi_framework/examples/wikipedia/Index_cache.py` & `celi_framework-0.0.16/celi_framework/examples/wikipedia/Index_cache.py`

 * *Files identical despite different names*

### Comparing `celi_framework-0.0.15/celi_framework/examples/wikipedia/caching_beautiful_soup_reader.py` & `celi_framework-0.0.16/celi_framework/examples/wikipedia/caching_beautiful_soup_reader.py`

 * *Files identical despite different names*

### Comparing `celi_framework-0.0.15/celi_framework/examples/wikipedia/eval/run_eval.py` & `celi_framework-0.0.16/celi_framework/examples/wikipedia/eval/run_eval.py`

 * *Files identical despite different names*

### Comparing `celi_framework-0.0.15/celi_framework/examples/wikipedia/eval/test_sets.json` & `celi_framework-0.0.16/celi_framework/examples/wikipedia/eval/test_sets.json`

 * *Files identical despite different names*

### Comparing `celi_framework-0.0.15/celi_framework/examples/wikipedia/eval/test_sets_large.json` & `celi_framework-0.0.16/celi_framework/examples/wikipedia/eval/test_sets_large.json`

 * *Files identical despite different names*

### Comparing `celi_framework-0.0.15/celi_framework/examples/wikipedia/index.py` & `celi_framework-0.0.16/celi_framework/examples/wikipedia/index.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,21 +77,26 @@
         index = index_cache.get_index()
     else:
         logger.info(
             f"Building a new index for {url} named {index_cache.name}.  Last index creation date: {index_cache_created_at} Last content date: {content_cached_at}"
         )
         storage_context = index_cache.get_storage_context()
         index_cache.remove_storage()
-        index = index_wikipedia_url_with_references(
-            url,
-            storage_context=storage_context,
-            include_content=include_content,
-            include_references=include_references,
-        )
-        index_cache.persist()
+        try:
+            index = index_wikipedia_url_with_references(
+                url,
+                storage_context=storage_context,
+                include_content=include_content,
+                include_references=include_references,
+            )
+            index_cache.persist()
+        except Exception as e:
+            index_cache.remove_storage()
+            raise e
+
     return index
 
 
 def index_wikipedia_url_with_references(
     url: str,
     storage_context: Optional[StorageContext] = None,
     include_references: bool = True,
```

### Comparing `celi_framework-0.0.15/celi_framework/examples/wikipedia/job_description.py` & `celi_framework-0.0.16/celi_framework/examples/wikipedia/job_description.py`

 * *Files identical despite different names*

### Comparing `celi_framework-0.0.15/celi_framework/examples/wikipedia/loader.py` & `celi_framework-0.0.16/celi_framework/examples/wikipedia/loader.py`

 * *Files identical despite different names*

### Comparing `celi_framework-0.0.15/celi_framework/examples/wikipedia/tools.py` & `celi_framework-0.0.16/celi_framework/examples/wikipedia/tools.py`

 * *Files identical despite different names*

### Comparing `celi_framework-0.0.15/celi_framework/examples/wikipedia/wikipedia_utils.py` & `celi_framework-0.0.16/celi_framework/examples/wikipedia/wikipedia_utils.py`

 * *Files identical despite different names*

### Comparing `celi_framework-0.0.15/celi_framework/experimental/embeddor.py` & `celi_framework-0.0.16/celi_framework/experimental/embeddor.py`

 * *Files identical despite different names*

### Comparing `celi_framework-0.0.15/celi_framework/experimental/mapper.py` & `celi_framework-0.0.16/celi_framework/experimental/mapper.py`

 * *Files identical despite different names*

### Comparing `celi_framework-0.0.15/celi_framework/experimental/mechanic.py` & `celi_framework-0.0.16/celi_framework/experimental/mechanic.py`

 * *Files identical despite different names*

### Comparing `celi_framework-0.0.15/celi_framework/experimental/preprocessing/pre-processor.py` & `celi_framework-0.0.16/celi_framework/experimental/preprocessing/pre-processor.py`

 * *Files identical despite different names*

### Comparing `celi_framework-0.0.15/celi_framework/experimental/preprocessing/word_pdf_extractors/extract_pdf_tables.py` & `celi_framework-0.0.16/celi_framework/experimental/preprocessing/word_pdf_extractors/extract_pdf_tables.py`

 * *Files identical despite different names*

### Comparing `celi_framework-0.0.15/celi_framework/experimental/preprocessing/word_pdf_extractors/extractor_helpers.py` & `celi_framework-0.0.16/celi_framework/experimental/preprocessing/word_pdf_extractors/extractor_helpers.py`

 * *Files identical despite different names*

### Comparing `celi_framework-0.0.15/celi_framework/experimental/preprocessing/word_pdf_extractors/pdf_extractor.py` & `celi_framework-0.0.16/celi_framework/experimental/preprocessing/word_pdf_extractors/pdf_extractor.py`

 * *Files identical despite different names*

### Comparing `celi_framework-0.0.15/celi_framework/experimental/preprocessing/word_pdf_extractors/word_extractor.py` & `celi_framework-0.0.16/celi_framework/experimental/preprocessing/word_pdf_extractors/word_extractor.py`

 * *Files identical despite different names*

### Comparing `celi_framework-0.0.15/celi_framework/experimental/task_builder/factory.py` & `celi_framework-0.0.16/celi_framework/experimental/task_builder/factory.py`

 * *Files identical despite different names*

### Comparing `celi_framework-0.0.15/celi_framework/experimental/task_builder/llm_helper_funcs.py` & `celi_framework-0.0.16/celi_framework/experimental/task_builder/llm_helper_funcs.py`

 * *Files identical despite different names*

### Comparing `celi_framework-0.0.15/celi_framework/experimental/task_builder/llms.py` & `celi_framework-0.0.16/celi_framework/experimental/task_builder/llms.py`

 * *Files identical despite different names*

### Comparing `celi_framework-0.0.15/celi_framework/experimental/task_builder/template.py` & `celi_framework-0.0.16/celi_framework/experimental/task_builder/template.py`

 * *Files identical despite different names*

### Comparing `celi_framework-0.0.15/celi_framework/experimental/utils/ada.py` & `celi_framework-0.0.16/celi_framework/experimental/utils/ada.py`

 * *Files identical despite different names*

### Comparing `celi_framework-0.0.15/celi_framework/experimental/utils/mapper_utils.py` & `celi_framework-0.0.16/celi_framework/experimental/utils/mapper_utils.py`

 * *Files identical despite different names*

### Comparing `celi_framework-0.0.15/celi_framework/experimental/utils/nougat_preprocessing/preprocess.py` & `celi_framework-0.0.16/celi_framework/experimental/utils/nougat_preprocessing/preprocess.py`

 * *Files identical despite different names*

### Comparing `celi_framework-0.0.15/celi_framework/experimental/utils/nougat_preprocessing/preprocessing_templates.py` & `celi_framework-0.0.16/celi_framework/experimental/utils/nougat_preprocessing/preprocessing_templates.py`

 * *Files identical despite different names*

### Comparing `celi_framework-0.0.15/celi_framework/experimental/utils/postprocessor_utils.py` & `celi_framework-0.0.16/celi_framework/experimental/utils/postprocessor_utils.py`

 * *Files identical despite different names*

### Comparing `celi_framework-0.0.15/celi_framework/experimental/utils/synthetic_data.py` & `celi_framework-0.0.16/celi_framework/experimental/utils/synthetic_data.py`

 * *Files identical despite different names*

### Comparing `celi_framework-0.0.15/celi_framework/logging_config.json` & `celi_framework-0.0.16/celi_framework/logging_config.json`

 * *Files identical despite different names*

### Comparing `celi_framework-0.0.15/celi_framework/logging_setup.py` & `celi_framework-0.0.16/celi_framework/logging_setup.py`

 * *Files identical despite different names*

### Comparing `celi_framework-0.0.15/celi_framework/main.py` & `celi_framework-0.0.16/celi_framework/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -109,26 +109,28 @@
     directories = Directories.create(args.output_dir)
     mongo_config = instantiate_with_argparse_args(args, MongoDBConfig)
 
     job_description = get_obj_by_name(args.job_description)
 
     # If the tool_config_json file doesn't exist, try to find it relative to the root of the installed package.
     # This allows examples packaged with celi to work correctly.
-    if os.path.exists(args.tool_config_json):
-        tool_config_json = args.tool_config_json
+    if args.tool_config_json:
+        if os.path.exists(args.tool_config_json):
+            tool_config_json = args.tool_config_json
+        else:
+            # Find the root of the installed package
+            root_dir = os.path.dirname(os.path.dirname(os.path.abspath(__file__)))
+            tool_config_json = os.path.join(root_dir, args.tool_config_json)
+            if not os.path.exists(tool_config_json):
+                raise FileNotFoundError(
+                    f"Could not find {args.tool_config_json} or {tool_config_json}"
+                )
+        tool_config = read_json_from_file(tool_config_json)
     else:
-        # Find the root of the installed package
-        root_dir = os.path.dirname(os.path.dirname(os.path.abspath(__file__)))
-        tool_config_json = os.path.join(root_dir, args.tool_config_json)
-        if not os.path.exists(tool_config_json):
-            raise FileNotFoundError(
-                f"Could not find {args.tool_config_json} or {tool_config_json}"
-            )
-
-    tool_config = read_json_from_file(tool_config_json)
+        args.tool_config_json = {}
 
     tool_implementations = job_description.tool_implementations_class(**tool_config)
 
     llm_cache = not args.no_cache
     use_monitor = not args.no_monitor
 
     # Instantiate the class, passing parser_model as a parameter
```

### Comparing `celi_framework-0.0.15/celi_framework/utils/codex.py` & `celi_framework-0.0.16/celi_framework/utils/codex.py`

 * *Files identical despite different names*

### Comparing `celi_framework-0.0.15/celi_framework/utils/llmcore_utils.py` & `celi_framework-0.0.16/celi_framework/utils/llmcore_utils.py`

 * *Files identical despite different names*

### Comparing `celi_framework-0.0.15/celi_framework/utils/llms.py` & `celi_framework-0.0.16/celi_framework/utils/llms.py`

 * *Files identical despite different names*

### Comparing `celi_framework-0.0.15/celi_framework/utils/sql_utils.py` & `celi_framework-0.0.16/celi_framework/utils/sql_utils.py`

 * *Files identical despite different names*

### Comparing `celi_framework-0.0.15/celi_framework/utils/token_counters.py` & `celi_framework-0.0.16/celi_framework/utils/token_counters.py`

 * *Files identical despite different names*

### Comparing `celi_framework-0.0.15/celi_framework/utils/utils.py` & `celi_framework-0.0.16/celi_framework/utils/utils.py`

 * *Files identical despite different names*

### Comparing `celi_framework-0.0.15/pyproject.toml` & `celi_framework-0.0.16/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "celi-framework"
-version = "0.0.15"
+version = "0.0.16"
 description = "Controller-Embedded Language Interactions - facilitates the entire lifecycle of document processing, from pre-processing and embedding to post-monitoring and quality assessment."
 authors = ["Jan-Samuel Wagner <jwab@genmab.com>","Dave DeCaprio <daved@alum.mit.edu>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/x3n0cr4735/celi"
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
```

### Comparing `celi_framework-0.0.15/PKG-INFO` & `celi_framework-0.0.16/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: celi-framework
-Version: 0.0.15
+Version: 0.0.16
 Summary: Controller-Embedded Language Interactions - facilitates the entire lifecycle of document processing, from pre-processing and embedding to post-monitoring and quality assessment.
 Home-page: https://github.com/x3n0cr4735/celi
 License: MIT
 Author: Jan-Samuel Wagner
 Author-email: jwab@genmab.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -49,15 +49,17 @@
 
 - **Scalability:** Designed to accommodate projects of any scale, CELI efficiently processes massive datasets and documents, and produces output of any size, making it an ideal solution for both targeted tasks and large-scale knowledge work automation.
 
 - **Streamlined Document Lifecycle Management:** CELI optimizes the entire lifecycle of document processing, encompassing pre-processing, embedding, synthesis, content generation, and quality monitoring.
 
 - **Development Flexibility:** CELI is architecturally designed to support developers in creating bespoke applications that conform to specific industry standards, including compliance, methodological rigor, and auditing requirements. This fosters innovation in the field of automated knowledge work by providing a scalable framework that integrates seamlessly into enterprise ecosystems.
 
-[Join our Discord server](https://discord.gg/C5SQNdzV) to ask questions or get involved in our project!
+Join our [Discord server](https://discord.gg/C5SQNdzV) to ask questions or get involved in our project!
+
+Read through [our documentation](https://celi.readthedocs.io/en/latest/) for detailed explanations of our codebase.
 
 Note: CELI is currently in alpha. If there are any issues installing, running, or utilizing CELI in your projects please let us know on Discord or create an issue or pull request. We will get back to you promptly.
 
 ## Goals
 
 The CELI (Controller-Embedded Language Interactions) framework aims to empower users across various industries and domains with tools to automate routine and complex tasks efficiently. Our objectives are encapsulated in the following goals:
 
@@ -175,15 +177,15 @@
 Note that running this takes around 30 minutes (give or take).
 
 <!-- end getting-started -->
 
 ## Documentation
 
 Explore the rest of the documentation to learn more about CELI.
-* [Getting Started]() - Learn more about the various ways to run CELI.
+* [Getting Started](https://celi.readthedocs.io/en/stable/getting_started.html) - Learn more about the various ways to run CELI.
 * [Running CELI](https://celi.readthedocs.io/en/stable/running_celi.html) - Learn more about the various ways to run CELI.
 * [New Use Cases](https://celi.readthedocs.io/en/stable/new_use_cases.html) - Learn how to apply CELI to your own use case.
 * [API Reference](https://celi.readthedocs.io/en/stable/reference/index.html) - If you are into reading API docs directly.
 
 ## Discord Server
 
 [Join our Discord server](https://discord.gg/C5SQNdzV) to discuss the project with users, contributors, and project authors.
```

