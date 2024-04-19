# Comparing `tmp/graph_validation_tests-0.0.6.tar.gz` & `tmp/graph_validation_tests-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graph_validation_tests-0.0.6.tar", max compression
+gzip compressed data, was "graph_validation_tests-0.0.7.tar", max compression
```

## Comparing `graph_validation_tests-0.0.6.tar` & `graph_validation_tests-0.0.7.tar`

### file list

```diff
@@ -1,43 +1,43 @@
--rw-r--r--   0        0        0     1070 2024-04-18 05:33:13.044415 graph_validation_tests-0.0.6/LICENSE
--rw-r--r--   0        0        0    12009 2024-04-18 05:33:13.044415 graph_validation_tests-0.0.6/README.md
--rw-r--r--   0        0        0    21945 2024-04-18 05:33:13.044415 graph_validation_tests-0.0.6/graph_validation_test/__init__.py
--rw-r--r--   0        0        0    10451 2024-04-18 05:33:13.044415 graph_validation_tests-0.0.6/graph_validation_test/request.py
--rw-r--r--   0        0        0        0 2024-04-18 05:33:13.044415 graph_validation_tests-0.0.6/graph_validation_test/translator/__init__.py
--rw-r--r--   0        0        0    36673 2024-04-18 05:33:13.044415 graph_validation_tests-0.0.6/graph_validation_test/translator/registry/__init__.py
--rw-r--r--   0        0        0    10042 2024-04-18 05:33:13.044415 graph_validation_tests-0.0.6/graph_validation_test/translator/trapi/__init__.py
--rw-r--r--   0        0        0        0 2024-04-18 05:33:13.044415 graph_validation_tests-0.0.6/graph_validation_test/utils/__init__.py
--rw-r--r--   0        0        0      722 2024-04-18 05:33:13.044415 graph_validation_tests-0.0.6/graph_validation_test/utils/asyncio.py
--rw-r--r--   0        0        0      113 2024-04-18 05:33:13.044415 graph_validation_tests-0.0.6/graph_validation_test/utils/constants.py
--rw-r--r--   0        0        0      886 2024-04-18 05:33:13.044415 graph_validation_tests-0.0.6/graph_validation_test/utils/http.py
--rw-r--r--   0        0        0     4267 2024-04-18 05:33:13.044415 graph_validation_tests-0.0.6/graph_validation_test/utils/ontology_kp.py
--rw-r--r--   0        0        0     7957 2024-04-18 05:33:13.044415 graph_validation_tests-0.0.6/graph_validation_test/utils/testsuite.py
--rw-r--r--   0        0        0    18148 2024-04-18 05:33:13.044415 graph_validation_tests-0.0.6/graph_validation_test/utils/unit_test_templates.py
--rw-r--r--   0        0        0     8957 2024-04-18 05:33:13.044415 graph_validation_tests-0.0.6/one_hop_test/__init__.py
--rw-r--r--   0        0        0     2856 2024-04-18 05:33:25.720510 graph_validation_tests-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     4851 2024-04-18 05:33:13.048415 graph_validation_tests-0.0.6/standards_validation_test/__init__.py
--rw-r--r--   0        0        0     1250 2024-04-18 05:33:13.048415 graph_validation_tests-0.0.6/tests/__init__.py
--rw-r--r--   0        0        0        0 2024-04-18 05:33:13.048415 graph_validation_tests-0.0.6/tests/graph_validation_test/__init__.py
--rw-r--r--   0        0        0     3855 2024-04-18 05:33:13.048415 graph_validation_tests-0.0.6/tests/graph_validation_test/test_graph_validation_test.py
--rw-r--r--   0        0        0     5764 2024-04-18 05:33:13.048415 graph_validation_tests-0.0.6/tests/graph_validation_test/test_unit_test_templates.py
--rw-r--r--   0        0        0        0 2024-04-18 05:33:13.048415 graph_validation_tests-0.0.6/tests/graph_validation_test/translator/__init__.py
--rw-r--r--   0        0        0        0 2024-04-18 05:33:13.048415 graph_validation_tests-0.0.6/tests/graph_validation_test/translator/biolink/__init__.py
--rw-r--r--   0        0        0     1065 2024-04-18 05:33:13.048415 graph_validation_tests-0.0.6/tests/graph_validation_test/translator/biolink/test_ontology_kp.py
--rw-r--r--   0        0        0    18030 2024-04-18 05:33:13.048415 graph_validation_tests-0.0.6/tests/graph_validation_test/translator/test_translator_smartapi_registry.py
--rw-r--r--   0        0        0        0 2024-04-18 05:33:13.048415 graph_validation_tests-0.0.6/tests/graph_validation_test/translator/trapi/__init__.py
--rw-r--r--   0        0        0     5061 2024-04-18 05:33:13.048415 graph_validation_tests-0.0.6/tests/graph_validation_test/translator/trapi/test_trapi.py
--rw-r--r--   0        0        0        0 2024-04-18 05:33:13.048415 graph_validation_tests-0.0.6/tests/one_hop_test/__init__.py
--rw-r--r--   0        0        0     3383 2024-04-18 05:33:13.048415 graph_validation_tests-0.0.6/tests/one_hop_test/test_one_hop_test.py
--rw-r--r--   0        0        0    25697 2024-04-18 05:33:13.048415 graph_validation_tests-0.0.6/tests/one_hop_test/test_venv/Scripts/Activate.ps1
--rw-r--r--   0        0        0     2063 2024-04-18 05:33:13.048415 graph_validation_tests-0.0.6/tests/one_hop_test/test_venv/Scripts/activate
--rw-r--r--   0        0        0     1027 2024-04-18 05:33:13.048415 graph_validation_tests-0.0.6/tests/one_hop_test/test_venv/Scripts/activate.bat
--rw-r--r--   0        0        0      371 2024-04-18 05:33:13.048415 graph_validation_tests-0.0.6/tests/one_hop_test/test_venv/Scripts/deactivate.bat
--rw-r--r--   0        0        0   108460 2024-04-18 05:33:13.048415 graph_validation_tests-0.0.6/tests/one_hop_test/test_venv/Scripts/pip.exe
--rw-r--r--   0        0        0   108460 2024-04-18 05:33:13.048415 graph_validation_tests-0.0.6/tests/one_hop_test/test_venv/Scripts/pip3.10.exe
--rw-r--r--   0        0        0   108460 2024-04-18 05:33:13.048415 graph_validation_tests-0.0.6/tests/one_hop_test/test_venv/Scripts/pip3.exe
--rw-r--r--   0        0        0   268568 2024-04-18 05:33:13.052415 graph_validation_tests-0.0.6/tests/one_hop_test/test_venv/Scripts/python.exe
--rw-r--r--   0        0        0   257304 2024-04-18 05:33:13.052415 graph_validation_tests-0.0.6/tests/one_hop_test/test_venv/Scripts/pythonw.exe
--rw-r--r--   0        0        0      164 2024-04-18 05:33:13.052415 graph_validation_tests-0.0.6/tests/one_hop_test/test_venv/pyvenv.cfg
--rw-r--r--   0        0        0       70 2024-04-18 05:33:13.052415 graph_validation_tests-0.0.6/tests/scripts/one_hop_test.cmd
--rw-r--r--   0        0        0        0 2024-04-18 05:33:13.052415 graph_validation_tests-0.0.6/tests/standards_validation_test/__init__.py
--rw-r--r--   0        0        0     1720 2024-04-18 05:33:13.052415 graph_validation_tests-0.0.6/tests/standards_validation_test/test_standards_validation_test.py
--rw-r--r--   0        0        0    14055 1970-01-01 00:00:00.000000 graph_validation_tests-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-04-19 07:30:49.425272 graph_validation_tests-0.0.7/LICENSE
+-rw-r--r--   0        0        0    12009 2024-04-19 07:30:49.425272 graph_validation_tests-0.0.7/README.md
+-rw-r--r--   0        0        0    29096 2024-04-19 07:30:49.425272 graph_validation_tests-0.0.7/graph_validation_test/__init__.py
+-rw-r--r--   0        0        0    10451 2024-04-19 07:30:49.425272 graph_validation_tests-0.0.7/graph_validation_test/request.py
+-rw-r--r--   0        0        0        0 2024-04-19 07:30:49.425272 graph_validation_tests-0.0.7/graph_validation_test/translator/__init__.py
+-rw-r--r--   0        0        0    36673 2024-04-19 07:30:49.425272 graph_validation_tests-0.0.7/graph_validation_test/translator/registry/__init__.py
+-rw-r--r--   0        0        0    10042 2024-04-19 07:30:49.425272 graph_validation_tests-0.0.7/graph_validation_test/translator/trapi/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-19 07:30:49.425272 graph_validation_tests-0.0.7/graph_validation_test/utils/__init__.py
+-rw-r--r--   0        0        0      722 2024-04-19 07:30:49.425272 graph_validation_tests-0.0.7/graph_validation_test/utils/asyncio.py
+-rw-r--r--   0        0        0      113 2024-04-19 07:30:49.425272 graph_validation_tests-0.0.7/graph_validation_test/utils/constants.py
+-rw-r--r--   0        0        0      886 2024-04-19 07:30:49.425272 graph_validation_tests-0.0.7/graph_validation_test/utils/http.py
+-rw-r--r--   0        0        0     4267 2024-04-19 07:30:49.425272 graph_validation_tests-0.0.7/graph_validation_test/utils/ontology_kp.py
+-rw-r--r--   0        0        0     7957 2024-04-19 07:30:49.425272 graph_validation_tests-0.0.7/graph_validation_test/utils/testsuite.py
+-rw-r--r--   0        0        0    18148 2024-04-19 07:30:49.425272 graph_validation_tests-0.0.7/graph_validation_test/utils/unit_test_templates.py
+-rw-r--r--   0        0        0     8957 2024-04-19 07:30:49.425272 graph_validation_tests-0.0.7/one_hop_test/__init__.py
+-rw-r--r--   0        0        0     2856 2024-04-19 07:31:01.985237 graph_validation_tests-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     4851 2024-04-19 07:30:49.425272 graph_validation_tests-0.0.7/standards_validation_test/__init__.py
+-rw-r--r--   0        0        0     1286 2024-04-19 07:30:49.425272 graph_validation_tests-0.0.7/tests/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-19 07:30:49.425272 graph_validation_tests-0.0.7/tests/graph_validation_test/__init__.py
+-rw-r--r--   0        0        0     3625 2024-04-19 07:30:49.425272 graph_validation_tests-0.0.7/tests/graph_validation_test/test_graph_validation_test.py
+-rw-r--r--   0        0        0     5764 2024-04-19 07:30:49.425272 graph_validation_tests-0.0.7/tests/graph_validation_test/test_unit_test_templates.py
+-rw-r--r--   0        0        0        0 2024-04-19 07:30:49.425272 graph_validation_tests-0.0.7/tests/graph_validation_test/translator/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-19 07:30:49.425272 graph_validation_tests-0.0.7/tests/graph_validation_test/translator/biolink/__init__.py
+-rw-r--r--   0        0        0     1065 2024-04-19 07:30:49.425272 graph_validation_tests-0.0.7/tests/graph_validation_test/translator/biolink/test_ontology_kp.py
+-rw-r--r--   0        0        0    18030 2024-04-19 07:30:49.429272 graph_validation_tests-0.0.7/tests/graph_validation_test/translator/test_translator_smartapi_registry.py
+-rw-r--r--   0        0        0        0 2024-04-19 07:30:49.429272 graph_validation_tests-0.0.7/tests/graph_validation_test/translator/trapi/__init__.py
+-rw-r--r--   0        0        0     5061 2024-04-19 07:30:49.429272 graph_validation_tests-0.0.7/tests/graph_validation_test/translator/trapi/test_trapi.py
+-rw-r--r--   0        0        0        0 2024-04-19 07:30:49.429272 graph_validation_tests-0.0.7/tests/one_hop_test/__init__.py
+-rw-r--r--   0        0        0     3383 2024-04-19 07:30:49.429272 graph_validation_tests-0.0.7/tests/one_hop_test/test_one_hop_test.py
+-rw-r--r--   0        0        0    25697 2024-04-19 07:30:49.429272 graph_validation_tests-0.0.7/tests/one_hop_test/test_venv/Scripts/Activate.ps1
+-rw-r--r--   0        0        0     2063 2024-04-19 07:30:49.429272 graph_validation_tests-0.0.7/tests/one_hop_test/test_venv/Scripts/activate
+-rw-r--r--   0        0        0     1027 2024-04-19 07:30:49.429272 graph_validation_tests-0.0.7/tests/one_hop_test/test_venv/Scripts/activate.bat
+-rw-r--r--   0        0        0      371 2024-04-19 07:30:49.429272 graph_validation_tests-0.0.7/tests/one_hop_test/test_venv/Scripts/deactivate.bat
+-rw-r--r--   0        0        0   108460 2024-04-19 07:30:49.429272 graph_validation_tests-0.0.7/tests/one_hop_test/test_venv/Scripts/pip.exe
+-rw-r--r--   0        0        0   108460 2024-04-19 07:30:49.429272 graph_validation_tests-0.0.7/tests/one_hop_test/test_venv/Scripts/pip3.10.exe
+-rw-r--r--   0        0        0   108460 2024-04-19 07:30:49.429272 graph_validation_tests-0.0.7/tests/one_hop_test/test_venv/Scripts/pip3.exe
+-rw-r--r--   0        0        0   268568 2024-04-19 07:30:49.433272 graph_validation_tests-0.0.7/tests/one_hop_test/test_venv/Scripts/python.exe
+-rw-r--r--   0        0        0   257304 2024-04-19 07:30:49.433272 graph_validation_tests-0.0.7/tests/one_hop_test/test_venv/Scripts/pythonw.exe
+-rw-r--r--   0        0        0      164 2024-04-19 07:30:49.433272 graph_validation_tests-0.0.7/tests/one_hop_test/test_venv/pyvenv.cfg
+-rw-r--r--   0        0        0       70 2024-04-19 07:30:49.433272 graph_validation_tests-0.0.7/tests/scripts/one_hop_test.cmd
+-rw-r--r--   0        0        0        0 2024-04-19 07:30:49.433272 graph_validation_tests-0.0.7/tests/standards_validation_test/__init__.py
+-rw-r--r--   0        0        0     1720 2024-04-19 07:30:49.433272 graph_validation_tests-0.0.7/tests/standards_validation_test/test_standards_validation_test.py
+-rw-r--r--   0        0        0    14055 1970-01-01 00:00:00.000000 graph_validation_tests-0.0.7/PKG-INFO
```

### Comparing `graph_validation_tests-0.0.6/LICENSE` & `graph_validation_tests-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `graph_validation_tests-0.0.6/README.md` & `graph_validation_tests-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `graph_validation_tests-0.0.6/graph_validation_test/__init__.py` & `graph_validation_tests-0.0.7/graph_validation_test/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 """
 Abstract base class for the GraphValidation TestRunners
 """
-from typing import Dict, List, Optional
+from typing import Dict, List, Optional, Tuple
 
 from argparse import ArgumentParser
 
 from reasoner_validator.biolink import BiolinkValidator
+from reasoner_validator.message import MESSAGES_BY_TARGET, MESSAGE_CATALOG, MESSAGES_BY_TEST
 from translator_testing_model.datamodel.pydanticmodel import (
     TestAsset,
     TestEnvEnum,
-    ComponentEnum
+    ComponentEnum, TestCaseResultEnum
 )
 
 from graph_validation_test.translator.registry import (
     get_the_registry_data,
     extract_component_test_metadata_from_registry
 )
 from graph_validation_test.utils.asyncio import gather
@@ -86,14 +87,15 @@
         """
         Need to access the TestAsset fields as a dictionary with some
         edge attributes relabelled to reasoner-validator expectations.
         :return: Dict[str,str], reasoner-validator indexed test edge data.
         """
         test_edge: Dict[str, str] = dict()
 
+        # TODO: should "idx" be renamed to "test_asset_id" or will this break the reasoner-validator?
         test_edge["idx"] = self.get_test_asset().id
         test_edge["subject_id"] = self.get_test_asset().input_id
         test_edge["subject_category"] = self.get_test_asset().input_category
         test_edge["predicate_id"] = self.get_test_asset().predicate_id \
             if self.get_test_asset().predicate_id else self.get_predicate_id(self.get_test_asset().predicate_name)
         test_edge["object_id"] = self.get_test_asset().output_id
         test_edge["object_category"] = self.get_test_asset().output_category
@@ -213,41 +215,38 @@
     def get_trapi_generators(self) -> List:
         return self.trapi_generators
 
     def get_runner_settings(self) -> List[str]:
         return self.runner_settings.copy()
 
     @classmethod
-    def generate_test_asset_id(cls) -> str:
-        cls._id += 1
-        return f"TestAsset:{cls._id:0>5}"
-
-    @classmethod
     def build_test_asset(
             cls,
+            test_asset_id: str,
             subject_id: str,
             subject_category: str,
             predicate_id: str,
             object_id: str,
             object_category: str
     ) -> TestAsset:
         """
         Construct a Python TestAsset object.
 
+        :param test_asset_id: str, CURIE identifying the identifier of the subject concept
         :param subject_id: str, CURIE identifying the identifier of the subject concept
         :param subject_category: str, CURIE identifying the category of the subject concept
         :param predicate_id: str, name of Biolink Model predicate defining the statement predicate_id being tested.
         :param object_id: str, CURIE identifying the identifier of the object concept
         :param object_category: str, CURIE identifying the category of the subject concept
         :return: TestAsset object
         """
         # TODO: is the TestAsset absolutely necessary internally inside this test runner,
         #       which directly uses Biolink fields, not the TestAsset fields?
         return TestAsset.construct(
-            id=cls.generate_test_asset_id(),
+            id=test_asset_id,
             input_id=subject_id,
             input_category=subject_category,
             predicate_id=predicate_id,
             predicate_name=predicate_id.replace("biolink:", ""),
             output_id=object_id,
             output_category=object_category
         )
@@ -265,64 +264,196 @@
         raise NotImplementedError("Abstract method, implement in subclass!")
 
     @staticmethod
     async def run_test_cases(test_cases: List[TestCaseRun]):
         # TODO: unsure if one needs to limit concurrent requests here...
         await gather([test_case.run_test_case() for test_case in test_cases])  # , limit=num_concurrent_requests)
 
-    async def process_test_run(self, **kwargs) -> List[Dict]:
+    FAILURE_MODES = ("error", "critical")
+
+    def compute_status(self, tcr: TestCaseRun) -> Tuple[str, TestCaseResultEnum, Dict]:
+        """
+        Method to construct components for a test case result based on
+        the failure mode assessment of non-empty validation messages.
+
+        :param tcr: TestCaseRun containing reasoner-validator style validation message from test execution.
+        :return: Tuple[str, TestCaseResultEnum, Dict], where position 0 is the target,
+                 position 1 is the testcase status (passed/failed/skipped) and
+                 position 2 is a (possible empty) dictionary of non-empty validation messages
+        """
+        target: str = tcr.default_target
+        test: str = tcr.default_test
+        messages_by_target: MESSAGES_BY_TARGET = tcr.get_all_messages()
+        if target in messages_by_target:
+            messages_by_test: MESSAGES_BY_TEST = messages_by_target[target]
+            if test in messages_by_test:
+                message_catalog: MESSAGE_CATALOG = messages_by_test[test]
+                mtype: str
+                messages: Dict
+                non_empty_messages: MESSAGE_CATALOG = {
+                    mtype: messages for mtype, messages in message_catalog.items() if message_catalog[mtype]
+                }
+                # TODO: this first iteration in which FAILURE_MODES are
+                #       immutable (not sensitive to TestRunner parameters)
+                if not non_empty_messages or not any([mtype in non_empty_messages for mtype in self.FAILURE_MODES]):
+                    return target, TestCaseResultEnum.test_passed, non_empty_messages
+                else:
+                    return target, TestCaseResultEnum.test_failed, non_empty_messages
+        # TODO: seems sensible to assumed that if the target or test are
+        #       missing in test results, then the test was skipped?
+        return target, TestCaseResultEnum.test_skipped, {}
+
+    def format_results(self, test_cases: List[TestCaseRun]) -> Dict:
+        """
+        This function normalizes and restructures TestCaseRun
+        results for the upstream consumer of TestRunner results.
+
+        :param test_cases: List[TestCaseRun], list of Test Case runs with results.
+
+        :return: Dict, of structured test message results for all TestCases,
+                       specified by TRAPI generators of a given test run.
+        """
+        # Originally, the results == [tc.get_all_messages() for tc in test_cases], which gives
+        # [
+        #    {
+        #        'molepro': {
+        #            'by_subject': {
+        #                'info': {},
+        #                'skipped': {},
+        #                'warning': {},
+        #                'error': {},
+        #                'critical': {}
+        #            }
+        #        }
+        #    },
+        #    {
+        #        'molepro': {
+        #            'inverse_by_new_subject': {
+        #                'info': {},
+        #                'skipped': {},
+        #                'warning': {},
+        #                'error': {
+        #                    'error.trapi.response.knowledge_graph.missing_expected_edge': {
+        #                        'global': {
+        #                            'TestAsset:00001|(PUBCHEM.COMPOUND:4091#biolink:SmallMolecule)-\
+        #                            [biolink:affects]->\
+        #                            (NCBIGene:2475#biolink:Gene)': None
+        #                        }
+        #                    }
+        #                },
+        #                'critical': {}
+        #            }
+        #        }
+        #    },
+        #    etc...
+        # ]
+        #
+        # with the source test_asset as recorded within the test_case.test_run.test_asset property. Note that all the
+        # test case message blocks have the same testing target component (although that doesn't have to be the case).
+        #
+        # We probably need to return something more like the following (using the source test asset information...):
+        #
+        # results == {
+        #     "<test_case_id_1>": {
+        #         "molepro": <result_1>,
+        #         etc...
+        #     }
+        #     "<test case id 2>": {
+        #         "molepro": <result 2>,
+        #         etc...
+        #     }
+        #     etc...
+        # ]
+        # where the 'test_asset_id_#' is something sensible, probably composite of the test asset identifier and
+        # the identifier of the test template method used to generate the TestCase-specific TRAPI query.
+        #
+        # The <result_#> value could minimally simply be be "PASSED" or "FAILED"; however, perhaps it ought to be
+        # a somewhat more complex informative data value for this TestRunner, accounting for the extensive validation
+        # messages categories provided by reasoner-validator, i.e. 'info', 'skipped', 'warning', 'error', 'critical'.
+        #
+        # How should these messages be binned into test PASSED or FAILED? Should “PASSED” only be tolerant of
+        # “information” messages? Are “skipped test” messages indicative of a failed test?
+        #
+        # Are “Warnings” to also be taken as an indication of a test failure? Could/should we give TestRunner
+        # “stringency” indications which affect whether “skipped” and “warnings” are returned as “PASSED”?
+        #
+        # The above <result_#> could be a 2-Tuple of (<PASSED|FAILED>, <pruned message catalog>) where the message
+        # catelog is a Python dictionary pruned of all empty reasoner-validator validation message partitions,
+        # where the status of the test is determined by the aforementioned stringency rules, however coded.
+        #
+        results: Dict = dict()
+        for tcr in test_cases:
+            # TODO: not sure how robust this is: will the 'id' always be defined?
+            test_asset_id: str = tcr.test_run.test_asset.id
+            test_name: str = tcr.default_test
+            test_case_id: str = f"{test_asset_id}-{test_name}"
+            if test_case_id not in results:
+                results[test_case_id] = dict()
+            target: str
+            status: TestCaseResultEnum
+            messages: MESSAGE_CATALOG
+            target, status, messages = self.compute_status(tcr)
+            # TODO: we blissfully assume that targets only come up once for a given test_case_id
+            results[test_case_id][target] = (status, messages)
+
+        return results
+
+    async def process_test_run(self, **kwargs) -> Dict:
         """
         Applies a TestCase generator giving a specific subclass
         of TestCaseRun, wrapping queries defined by test-specific
         TRAPI query generators, then runs the derived TestCase
         instances as co-routines, returning a list of their results.
 
         :param kwargs: Dict, optional named parameters passed to the TestRunner.
 
-        :return: List[Dict] of structured test message results for all
-                 TestCases specified by trapi generators of a given test run.
+        :return: Dict, of structured test message results for all TestCases,
+                       specified by TRAPI generators of a given test run.
         """
         test_cases: List[TestCaseRun] = [
             self.test_case_wrapper(
                 test,
                 **kwargs
             )
             for test in self.get_trapi_generators()
         ]
 
         await self.run_test_cases(test_cases)
 
         # ... then, return the results
-        return [tc.get_all_messages() for tc in test_cases]
+        return self.format_results(test_cases)
 
     @classmethod
     async def run_tests(
             cls,
+            test_asset_id: str,
             subject_id: str,
             subject_category: str,
             predicate_id: str,
             object_id: str,
             object_category: str,
             trapi_generators: List,
             environment: Optional[TestEnvEnum] = TestEnvEnum.ci,
             components: Optional[List[ComponentEnum]] = None,
             trapi_version: Optional[str] = None,
             biolink_version: Optional[str] = None,
             runner_settings: Optional[List[str]] = None,
             **kwargs
-    ) -> Dict[str, List]:
+    ) -> Dict[str, Dict]:
         """
         Run one or more Graph Validation tests, of specified category of test,
         against all specified components running in a given environment,
         and with test cases derived from a specified test asset.
 
         Parameters provided to specify the test are:
 
-        - TestAsset to be used for test queries.
         :param cls: The target TestRunner subclass of GraphValidationTest of the test type to be run.
+
+        - TestAsset to be used for test queries.
+        :param test_asset_id: str, the identifier of the test asset driving test cases in this run of tests
         :param subject_id: str, CURIE identifying the identifier of the subject concept
         :param subject_category: str, CURIE identifying the category of the subject concept
         :param predicate_id: str, name of Biolink Model predicate defining the statement predicate_id being tested.
         :param object_id: str, CURIE identifying the identifier of the object concept
         :param object_category: str, CURIE identifying the category of the object concept
 
         - TRAPI JSON query generators for the TestCases using the specified TestAsset
@@ -337,28 +468,29 @@
                             one of 'dev', 'ci', 'test' or 'prod' (default: 'ci')
 
         - Metadata globally configuring the test(s) to be run.
         :param trapi_version: Optional[str] = None, target TRAPI version (default: latest public release)
         :param biolink_version: Optional[str] = None, target Biolink Model version (default: Biolink toolkit release)
         :param runner_settings: Optional[List[str]] = None, extra string parameters to the Test Runner
         :param kwargs: Dict, optional extra named parameters to passed to TestCase TestRunner.
-        :return: Dict { "pks": List[<pk>], "results": List[<pk_indexed_results>] }
+        :return: Dict { "pks": Dict[<target>, <pk>], "results": Dict[<test_case_id>, <test_case_results>] }
         """
         if not components:
             components = [ComponentEnum('ars')]
 
         # TODO: (April 2024) short term limitation: can't test ARS endpoints, see the missing ARS code in
         #       the run_trapi_query() method of the graph_validation_test.translator.trapi package module.
         if 'ars' in components:
             logger.error("Default ARS testing is not yet supported by GraphValidationTests")
             return dict()
 
         # Load the internal TestAsset being uniformly served
         # to all TestCase runs against specified components.
         test_asset: TestAsset = GraphValidationTest.build_test_asset(
+            test_asset_id,
             subject_id,
             subject_category,
             predicate_id,
             object_id,
             object_category
         )
 
@@ -423,21 +555,23 @@
         #                 "improving": "Pass",
         #                 "ars": "Pass"
         #             }
         #         }
         #     ]
         # }
         results = {
-            "pks": list(),
-            "results": list()
+            "pks": dict(),
+            "results": dict()
         }
         for tr in test_runs:
-            run_id: str = tr.get_run_id()
-            results["pks"].append(run_id)
-            results["results"].append(await tr.process_test_run(**kwargs))
+            target: str = tr.default_target
+            test_run_id: str = tr.get_run_id()
+            results["pks"].update({target: test_run_id})
+            results["results"].update(await tr.process_test_run(**kwargs))
+
         return results
 
 
 def get_parameters(tool_name: str):
     """Parse CLI args."""
 
     # Sample command line interface parameters:
@@ -470,14 +604,21 @@
         choices=['dev', 'ci', 'test', 'prod'],
         default=None,
         help="Translator execution environment of the Translator Component targeted for testing. " +
              "(Default: if unspecified, run the test within the 'ci' environment)",
     )
 
     parser.add_argument(
+        "--test_asset_id",
+        type=str,
+        required=True,
+        help="Identifier of TestAsset associated with specified test run parameters",
+    )
+
+    parser.add_argument(
         "--subject_id",
         type=str,
         required=True,
         help="Statement subject concept CURIE",
     )
 
     parser.add_argument(
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `graph_validation_tests-0.0.6/graph_validation_test/request.py` & `graph_validation_tests-0.0.7/graph_validation_test/request.py`

 * *Files identical despite different names*

### Comparing `graph_validation_tests-0.0.6/graph_validation_test/translator/registry/__init__.py` & `graph_validation_tests-0.0.7/graph_validation_test/translator/registry/__init__.py`

 * *Files identical despite different names*

### Comparing `graph_validation_tests-0.0.6/graph_validation_test/translator/trapi/__init__.py` & `graph_validation_tests-0.0.7/graph_validation_test/translator/trapi/__init__.py`

 * *Files identical despite different names*

### Comparing `graph_validation_tests-0.0.6/graph_validation_test/utils/asyncio.py` & `graph_validation_tests-0.0.7/graph_validation_test/utils/asyncio.py`

 * *Files identical despite different names*

### Comparing `graph_validation_tests-0.0.6/graph_validation_test/utils/http.py` & `graph_validation_tests-0.0.7/graph_validation_test/utils/http.py`

 * *Files identical despite different names*

### Comparing `graph_validation_tests-0.0.6/graph_validation_test/utils/ontology_kp.py` & `graph_validation_tests-0.0.7/graph_validation_test/utils/ontology_kp.py`

 * *Files identical despite different names*

### Comparing `graph_validation_tests-0.0.6/graph_validation_test/utils/testsuite.py` & `graph_validation_tests-0.0.7/graph_validation_test/utils/testsuite.py`

 * *Files identical despite different names*

### Comparing `graph_validation_tests-0.0.6/graph_validation_test/utils/unit_test_templates.py` & `graph_validation_tests-0.0.7/graph_validation_test/utils/unit_test_templates.py`

 * *Files identical despite different names*

### Comparing `graph_validation_tests-0.0.6/one_hop_test/__init__.py` & `graph_validation_tests-0.0.7/one_hop_test/__init__.py`

 * *Files identical despite different names*

### Comparing `graph_validation_tests-0.0.6/pyproject.toml` & `graph_validation_tests-0.0.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "graph-validation-tests"
-version = "0.0.6"
+version = "0.0.7"
 description = "Validation of Translator Knowledge Graphs - TRAPI, Biolink Model and One Hop navigation"
 authors = [
     "Richard Bruskiewich <richard.bruskiewich@delphinai.com>",
     "Chris Bizon <bizon.renci.org>",
     "Tim Putnam <tim@tislab>"
 ]
 maintainers = ["Richard Bruskiewich <richard.bruskiewich@delphinai.com>"]
```

### Comparing `graph_validation_tests-0.0.6/standards_validation_test/__init__.py` & `graph_validation_tests-0.0.7/standards_validation_test/__init__.py`

 * *Files identical despite different names*

### Comparing `graph_validation_tests-0.0.6/tests/__init__.py` & `graph_validation_tests-0.0.7/tests/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 PROJECT_DIR = os.path.join(os.path.abspath(os.path.dirname(__file__)), "..")
 SCRIPTS_DIR = os.path.join(os.path.abspath(os.path.dirname(__file__)), "scripts")
 
 DEFAULT_TRAPI_VERSION = get_latest_version("1")
 DEFAULT_BMT: Toolkit = get_biolink_model_toolkit()
 SAMPLE_TEST_INPUT_1 = {
     # One test edge (asset)
+    "test_asset_id": "TestAsset_1",
     "subject_id": "DRUGBANK:DB01592",
     "subject_category": "biolink:SmallMolecule",
     "predicate_id": "biolink:has_side_effect",
     "object_id": "MONDO:0011426",
     "object_category": "biolink:Disease",
     #
     #     "environment": environment, # Optional[TestEnvEnum] = None; default: 'TestEnvEnum.ci' if not given
```

### Comparing `graph_validation_tests-0.0.6/tests/graph_validation_test/test_graph_validation_test.py` & `graph_validation_tests-0.0.7/tests/graph_validation_test/test_graph_validation_test.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,38 +14,33 @@
     "subject_id": "DRUGBANK:DB01592",
     "subject_category": "biolink:SmallMolecule",
     "predicate_id": "biolink:treats",
     "object_id": "MONDO:0011426",
     "object_category": "biolink:Disease"
 }
 
-
+TEST_ASSET_ID = "TestAsset_1"
 TEST_SUBJECT_ID = "MONDO:0005301"
 TEST_SUBJECT_CATEGORY = "biolink:Disease"
 TEST_PREDICATE_NAME = "treats"
 TEST_PREDICATE_ID = f"biolink:{TEST_PREDICATE_NAME}"
 TEST_OBJECT_ID = "PUBCHEM.COMPOUND:107970"
 TEST_OBJECT_CATEGORY = "biolink:SmallMolecule"
 SAMPLE_TEST_ASSET: TestAsset = GraphValidationTest.build_test_asset(
-        subject_id=TEST_SUBJECT_ID,
-        subject_category=TEST_SUBJECT_CATEGORY,
-        predicate_id=TEST_PREDICATE_ID,
-        object_id=TEST_OBJECT_ID,
-        object_category=TEST_OBJECT_CATEGORY
+    test_asset_id=TEST_ASSET_ID,
+    subject_id=TEST_SUBJECT_ID,
+    subject_category=TEST_SUBJECT_CATEGORY,
+    predicate_id=TEST_PREDICATE_ID,
+    object_id=TEST_OBJECT_ID,
+    object_category=TEST_OBJECT_CATEGORY
 )
 
 
-def test_generate_test_asset_id():
-    assert GraphValidationTest.generate_test_asset_id() == "TestAsset:00002"
-    assert GraphValidationTest.generate_test_asset_id() == "TestAsset:00003"
-    assert GraphValidationTest.generate_test_asset_id() == "TestAsset:00004"
-
-
 def test_build_test_asset():
-    assert SAMPLE_TEST_ASSET.id == "TestAsset:00001"
+    assert SAMPLE_TEST_ASSET.id == TEST_ASSET_ID
     assert SAMPLE_TEST_ASSET.input_id == TEST_SUBJECT_ID
     assert SAMPLE_TEST_ASSET.input_category == TEST_SUBJECT_CATEGORY
     assert SAMPLE_TEST_ASSET.predicate_id == TEST_PREDICATE_ID
     assert SAMPLE_TEST_ASSET.predicate_name == TEST_PREDICATE_NAME
     assert SAMPLE_TEST_ASSET.output_id == TEST_OBJECT_ID
     assert SAMPLE_TEST_ASSET.output_category == TEST_OBJECT_CATEGORY
     assert SAMPLE_TEST_ASSET.expected_output is None  # not set?
```

### Comparing `graph_validation_tests-0.0.6/tests/graph_validation_test/test_unit_test_templates.py` & `graph_validation_tests-0.0.7/tests/graph_validation_test/test_unit_test_templates.py`

 * *Files identical despite different names*

### Comparing `graph_validation_tests-0.0.6/tests/graph_validation_test/translator/biolink/test_ontology_kp.py` & `graph_validation_tests-0.0.7/tests/graph_validation_test/translator/biolink/test_ontology_kp.py`

 * *Files identical despite different names*

### Comparing `graph_validation_tests-0.0.6/tests/graph_validation_test/translator/test_translator_smartapi_registry.py` & `graph_validation_tests-0.0.7/tests/graph_validation_test/translator/test_translator_smartapi_registry.py`

 * *Files identical despite different names*

### Comparing `graph_validation_tests-0.0.6/tests/graph_validation_test/translator/trapi/test_trapi.py` & `graph_validation_tests-0.0.7/tests/graph_validation_test/translator/trapi/test_trapi.py`

 * *Files identical despite different names*

### Comparing `graph_validation_tests-0.0.6/tests/one_hop_test/test_one_hop_test.py` & `graph_validation_tests-0.0.7/tests/one_hop_test/test_one_hop_test.py`

 * *Files identical despite different names*

### Comparing `graph_validation_tests-0.0.6/tests/one_hop_test/test_venv/Scripts/Activate.ps1` & `graph_validation_tests-0.0.7/tests/one_hop_test/test_venv/Scripts/Activate.ps1`

 * *Files identical despite different names*

### Comparing `graph_validation_tests-0.0.6/tests/one_hop_test/test_venv/Scripts/activate` & `graph_validation_tests-0.0.7/tests/one_hop_test/test_venv/Scripts/activate`

 * *Files identical despite different names*

### Comparing `graph_validation_tests-0.0.6/tests/one_hop_test/test_venv/Scripts/activate.bat` & `graph_validation_tests-0.0.7/tests/one_hop_test/test_venv/Scripts/activate.bat`

 * *Files identical despite different names*

### Comparing `graph_validation_tests-0.0.6/tests/one_hop_test/test_venv/Scripts/pip.exe` & `graph_validation_tests-0.0.7/tests/one_hop_test/test_venv/Scripts/pip.exe`

 * *Files identical despite different names*

### Comparing `graph_validation_tests-0.0.6/tests/one_hop_test/test_venv/Scripts/pip3.10.exe` & `graph_validation_tests-0.0.7/tests/one_hop_test/test_venv/Scripts/pip3.10.exe`

 * *Files identical despite different names*

### Comparing `graph_validation_tests-0.0.6/tests/one_hop_test/test_venv/Scripts/pip3.exe` & `graph_validation_tests-0.0.7/tests/one_hop_test/test_venv/Scripts/pip3.exe`

 * *Files identical despite different names*

### Comparing `graph_validation_tests-0.0.6/tests/one_hop_test/test_venv/Scripts/python.exe` & `graph_validation_tests-0.0.7/tests/one_hop_test/test_venv/Scripts/python.exe`

 * *Files identical despite different names*

### Comparing `graph_validation_tests-0.0.6/tests/one_hop_test/test_venv/Scripts/pythonw.exe` & `graph_validation_tests-0.0.7/tests/one_hop_test/test_venv/Scripts/pythonw.exe`

 * *Files identical despite different names*

### Comparing `graph_validation_tests-0.0.6/tests/standards_validation_test/test_standards_validation_test.py` & `graph_validation_tests-0.0.7/tests/standards_validation_test/test_standards_validation_test.py`

 * *Files identical despite different names*

### Comparing `graph_validation_tests-0.0.6/PKG-INFO` & `graph_validation_tests-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graph-validation-tests
-Version: 0.0.6
+Version: 0.0.7
 Summary: Validation of Translator Knowledge Graphs - TRAPI, Biolink Model and One Hop navigation
 Home-page: https://github.com/TranslatorSRI
 License: MIT
 Keywords: NCATS,Biomedical Data Translator,Translator,ReasonerAPI,TRAPI,validation,Biolink Model
 Author: Richard Bruskiewich
 Author-email: richard.bruskiewich@delphinai.com
 Maintainer: Richard Bruskiewich
```

