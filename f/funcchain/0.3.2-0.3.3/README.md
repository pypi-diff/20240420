# Comparing `tmp/funcchain-0.3.2.tar.gz` & `tmp/funcchain-0.3.3.tar.gz`

## Comparing `funcchain-0.3.2.tar` & `funcchain-0.3.3.tar`

### file list

```diff
@@ -1,150 +1,150 @@
--rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 funcchain-0.3.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 funcchain-0.3.2/.readthedocs.yaml
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 funcchain-0.3.2/CONTRIBUTING.md
--rw-r--r--   0        0        0     1300 2020-02-02 00:00:00.000000 funcchain-0.3.2/MODELS.md
--rwxr-xr-x   0        0        0     1032 2020-02-02 00:00:00.000000 funcchain-0.3.2/dev-setup.sh
--rw-r--r--   0        0        0     3889 2020-02-02 00:00:00.000000 funcchain-0.3.2/mkdocs.yml
--rw-r--r--   0        0        0     8961 2020-02-02 00:00:00.000000 funcchain-0.3.2/requirements-dev.lock
--rw-r--r--   0        0        0     1784 2020-02-02 00:00:00.000000 funcchain-0.3.2/requirements.lock
--rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 funcchain-0.3.2/roadmap.todo
--rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 funcchain-0.3.2/.github/workflows/code-check.yml
--rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 funcchain-0.3.2/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 funcchain-0.3.2/docs/changelog.md
--rw-r--r--   0        0        0     4672 2020-02-02 00:00:00.000000 funcchain-0.3.2/docs/index.md
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 funcchain-0.3.2/docs/requirements.txt
--rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 funcchain-0.3.2/docs/advanced/async.md
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 funcchain-0.3.2/docs/advanced/codebase-scaling.md
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 funcchain-0.3.2/docs/advanced/custom-parser-types.md
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 funcchain-0.3.2/docs/advanced/customization.md
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 funcchain-0.3.2/docs/advanced/runnables.md
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 funcchain-0.3.2/docs/advanced/signature.md
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 funcchain-0.3.2/docs/advanced/stream-parsing.md
--rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 funcchain-0.3.2/docs/concepts/chain.md
--rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 funcchain-0.3.2/docs/concepts/dependencies.md
--rw-r--r--   0        0        0     1491 2020-02-02 00:00:00.000000 funcchain-0.3.2/docs/concepts/errors.md
--rw-r--r--   0        0        0     2697 2020-02-02 00:00:00.000000 funcchain-0.3.2/docs/concepts/input.md
--rw-r--r--   0        0        0     2809 2020-02-02 00:00:00.000000 funcchain-0.3.2/docs/concepts/langchain.md
--rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 funcchain-0.3.2/docs/concepts/local-models.md
--rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 funcchain-0.3.2/docs/concepts/overview.md
--rw-r--r--   0        0        0     3630 2020-02-02 00:00:00.000000 funcchain-0.3.2/docs/concepts/parser.md
--rw-r--r--   0        0        0     2228 2020-02-02 00:00:00.000000 funcchain-0.3.2/docs/concepts/prompting.md
--rw-r--r--   0        0        0     2076 2020-02-02 00:00:00.000000 funcchain-0.3.2/docs/concepts/pydantic.md
--rw-r--r--   0        0        0     1493 2020-02-02 00:00:00.000000 funcchain-0.3.2/docs/concepts/streaming.md
--rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 funcchain-0.3.2/docs/concepts/unions.md
--rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 funcchain-0.3.2/docs/concepts/vision.md
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 funcchain-0.3.2/docs/contributing/codebase-structure.md
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 funcchain-0.3.2/docs/contributing/contributors.md
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 funcchain-0.3.2/docs/contributing/dev-setup.md
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 funcchain-0.3.2/docs/contributing/license.md
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 funcchain-0.3.2/docs/contributing/roadmap.md
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 funcchain-0.3.2/docs/contributing/security.md
--rw-r--r--   0        0        0     1126 2020-02-02 00:00:00.000000 funcchain-0.3.2/docs/css/custom.css
--rw-r--r--   0        0        0     2065 2020-02-02 00:00:00.000000 funcchain-0.3.2/docs/css/termynal.css
--rw-r--r--   0        0        0     7834 2020-02-02 00:00:00.000000 funcchain-0.3.2/docs/features/dynamic_router.md
--rw-r--r--   0        0        0     2581 2020-02-02 00:00:00.000000 funcchain-0.3.2/docs/features/enums.md
--rw-r--r--   0        0        0     2995 2020-02-02 00:00:00.000000 funcchain-0.3.2/docs/features/error_output.md
--rw-r--r--   0        0        0     2487 2020-02-02 00:00:00.000000 funcchain-0.3.2/docs/features/literals.md
--rw-r--r--   0        0        0     3394 2020-02-02 00:00:00.000000 funcchain-0.3.2/docs/features/llamacpp.md
--rw-r--r--   0        0        0     3274 2020-02-02 00:00:00.000000 funcchain-0.3.2/docs/features/ollama.md
--rw-r--r--   0        0        0     2319 2020-02-02 00:00:00.000000 funcchain-0.3.2/docs/features/openai_json_mode.md
--rw-r--r--   0        0        0     3733 2020-02-02 00:00:00.000000 funcchain-0.3.2/docs/features/retry_parsing.md
--rw-r--r--   0        0        0     4357 2020-02-02 00:00:00.000000 funcchain-0.3.2/docs/features/static_router.md
--rw-r--r--   0        0        0     1944 2020-02-02 00:00:00.000000 funcchain-0.3.2/docs/features/stream.md
--rw-r--r--   0        0        0     4043 2020-02-02 00:00:00.000000 funcchain-0.3.2/docs/features/vision.md
--rw-r--r--   0        0        0     3005 2020-02-02 00:00:00.000000 funcchain-0.3.2/docs/getting-started/config.md
--rw-r--r--   0        0        0    12075 2020-02-02 00:00:00.000000 funcchain-0.3.2/docs/getting-started/demos.md
--rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 funcchain-0.3.2/docs/getting-started/installation.md
--rw-r--r--   0        0        0     1429 2020-02-02 00:00:00.000000 funcchain-0.3.2/docs/getting-started/models.md
--rw-r--r--   0        0        0     1272 2020-02-02 00:00:00.000000 funcchain-0.3.2/docs/getting-started/usage.md
--rw-r--r--   0        0        0     4557 2020-02-02 00:00:00.000000 funcchain-0.3.2/docs/js/custom.js
--rw-r--r--   0        0        0     8902 2020-02-02 00:00:00.000000 funcchain-0.3.2/docs/js/termynal.js
--rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 funcchain-0.3.2/examples/chatgpt.py
--rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 funcchain-0.3.2/examples/classify.py
--rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 funcchain-0.3.2/examples/claude3.py
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 funcchain-0.3.2/examples/custom_lc_model.py
--rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 funcchain-0.3.2/examples/custom_model_display.py
--rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 funcchain-0.3.2/examples/decorator.py
--rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 funcchain-0.3.2/examples/dict_type.py
--rw-r--r--   0        0        0     2367 2020-02-02 00:00:00.000000 funcchain-0.3.2/examples/dynamic_router.py
--rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 funcchain-0.3.2/examples/enums.py
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 funcchain-0.3.2/examples/error_output.py
--rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 funcchain-0.3.2/examples/jinja.py
--rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 funcchain-0.3.2/examples/literals.py
--rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 funcchain-0.3.2/examples/llamacpp.py
--rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 funcchain-0.3.2/examples/ollama.py
--rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 funcchain-0.3.2/examples/openai_json_mode.py
--rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 funcchain-0.3.2/examples/primitive_types.py
--rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 funcchain-0.3.2/examples/pydantic_validation.py
--rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 funcchain-0.3.2/examples/rag_with_deps.py
--rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 funcchain-0.3.2/examples/runnable_deps.py
--rw-r--r--   0        0        0     1432 2020-02-02 00:00:00.000000 funcchain-0.3.2/examples/static_router.py
--rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 funcchain-0.3.2/examples/stream.py
--rw-r--r--   0        0        0     2745 2020-02-02 00:00:00.000000 funcchain-0.3.2/examples/stream_runnables.py
--rw-r--r--   0        0        0     1240 2020-02-02 00:00:00.000000 funcchain-0.3.2/examples/union_types.py
--rw-r--r--   0        0        0      955 2020-02-02 00:00:00.000000 funcchain-0.3.2/examples/vision.py
--rw-r--r--   0        0        0   326240 2020-02-02 00:00:00.000000 funcchain-0.3.2/examples/assets/old_chinese_temple.jpg
--rw-r--r--   0        0        0     1354 2020-02-02 00:00:00.000000 funcchain-0.3.2/examples/async/expert_answer.py
--rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 funcchain-0.3.2/examples/async/startup_names.py
--rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 funcchain-0.3.2/examples/experiments/email_answering.py
--rw-r--r--   0        0        0     2971 2020-02-02 00:00:00.000000 funcchain-0.3.2/examples/experiments/generate_pp_and_tos.py
--rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 funcchain-0.3.2/examples/experiments/local_codeblock.py
--rw-r--r--   0        0        0     3741 2020-02-02 00:00:00.000000 funcchain-0.3.2/examples/experiments/parallel_console_streaming.py
--rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 funcchain-0.3.2/examples/simple/gather_infos.py
--rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 funcchain-0.3.2/examples/simple/summary.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 funcchain-0.3.2/examples/simple/task_comparison.py
--rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 funcchain-0.3.2/examples/simple/tutorial.py
--rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 funcchain-0.3.2/src/funcchain/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 funcchain-0.3.2/src/funcchain/py.typed
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 funcchain-0.3.2/src/funcchain/backend/__init__.py
--rw-r--r--   0        0        0    15287 2020-02-02 00:00:00.000000 funcchain-0.3.2/src/funcchain/backend/compiler.py
--rw-r--r--   0        0        0     2552 2020-02-02 00:00:00.000000 funcchain-0.3.2/src/funcchain/backend/meta_inspect.py
--rw-r--r--   0        0        0     5804 2020-02-02 00:00:00.000000 funcchain-0.3.2/src/funcchain/backend/prompt.py
--rw-r--r--   0        0        0     2801 2020-02-02 00:00:00.000000 funcchain-0.3.2/src/funcchain/backend/settings.py
--rw-r--r--   0        0        0     3453 2020-02-02 00:00:00.000000 funcchain-0.3.2/src/funcchain/backend/streaming.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 funcchain-0.3.2/src/funcchain/model/__init__.py
--rw-r--r--   0        0        0     2434 2020-02-02 00:00:00.000000 funcchain-0.3.2/src/funcchain/model/abilities.py
--rw-r--r--   0        0        0     5846 2020-02-02 00:00:00.000000 funcchain-0.3.2/src/funcchain/model/defaults.py
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 funcchain-0.3.2/src/funcchain/model/patches/__init__.py
--rw-r--r--   0        0        0    14195 2020-02-02 00:00:00.000000 funcchain-0.3.2/src/funcchain/model/patches/llamacpp.py
--rw-r--r--   0        0        0     6219 2020-02-02 00:00:00.000000 funcchain-0.3.2/src/funcchain/model/patches/ollama.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 funcchain-0.3.2/src/funcchain/parser/__init__.py
--rw-r--r--   0        0        0     2192 2020-02-02 00:00:00.000000 funcchain-0.3.2/src/funcchain/parser/custom.py
--rw-r--r--   0        0        0     3329 2020-02-02 00:00:00.000000 funcchain-0.3.2/src/funcchain/parser/json_schema.py
--rw-r--r--   0        0        0     6312 2020-02-02 00:00:00.000000 funcchain-0.3.2/src/funcchain/parser/openai_functions.py
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 funcchain-0.3.2/src/funcchain/parser/primitive_types.py
--rw-r--r--   0        0        0     5314 2020-02-02 00:00:00.000000 funcchain-0.3.2/src/funcchain/parser/schema_converter.py
--rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 funcchain-0.3.2/src/funcchain/parser/selector.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 funcchain-0.3.2/src/funcchain/schema/__init__.py
--rw-r--r--   0        0        0     1498 2020-02-02 00:00:00.000000 funcchain-0.3.2/src/funcchain/schema/signature.py
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 funcchain-0.3.2/src/funcchain/schema/types.py
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 funcchain-0.3.2/src/funcchain/syntax/__init__.py
--rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 funcchain-0.3.2/src/funcchain/syntax/decorators.py
--rw-r--r--   0        0        0     4745 2020-02-02 00:00:00.000000 funcchain-0.3.2/src/funcchain/syntax/executable.py
--rw-r--r--   0        0        0     2367 2020-02-02 00:00:00.000000 funcchain-0.3.2/src/funcchain/syntax/input_types.py
--rw-r--r--   0        0        0     1767 2020-02-02 00:00:00.000000 funcchain-0.3.2/src/funcchain/syntax/output_types.py
--rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 funcchain-0.3.2/src/funcchain/syntax/params.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 funcchain-0.3.2/src/funcchain/syntax/components/__init__.py
--rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 funcchain-0.3.2/src/funcchain/syntax/components/handler.py
--rw-r--r--   0        0        0     4511 2020-02-02 00:00:00.000000 funcchain-0.3.2/src/funcchain/syntax/components/router.py
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 funcchain-0.3.2/src/funcchain/utils/__init__.py
--rw-r--r--   0        0        0      918 2020-02-02 00:00:00.000000 funcchain-0.3.2/src/funcchain/utils/image.py
--rw-r--r--   0        0        0     2214 2020-02-02 00:00:00.000000 funcchain-0.3.2/src/funcchain/utils/memory.py
--rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 funcchain-0.3.2/src/funcchain/utils/msg_tools.py
--rw-r--r--   0        0        0     2097 2020-02-02 00:00:00.000000 funcchain-0.3.2/src/funcchain/utils/pydantic.py
--rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 funcchain-0.3.2/src/funcchain/utils/token_counter.py
--rw-r--r--   0        0        0     1458 2020-02-02 00:00:00.000000 funcchain-0.3.2/tests/async_test.py
--rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 funcchain-0.3.2/tests/extraction_test.py
--rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 funcchain-0.3.2/tests/run_examples_test.py
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 funcchain-0.3.2/tests/features/jinja_test.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 funcchain-0.3.2/tests/features/primitive_types_test.py
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 funcchain-0.3.2/tests/features/retry_validation_test.py
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 funcchain-0.3.2/tests/features/router_component_test.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 funcchain-0.3.2/tests/features/streaming_test.py
--rw-r--r--   0        0        0     1823 2020-02-02 00:00:00.000000 funcchain-0.3.2/tests/models/llamacpp_test.py
--rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 funcchain-0.3.2/tests/models/ollama_test.py
--rw-r--r--   0        0        0     1330 2020-02-02 00:00:00.000000 funcchain-0.3.2/tests/models/openai_test.py
--rw-r--r--   0        0        0     3148 2020-02-02 00:00:00.000000 funcchain-0.3.2/.gitignore
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 funcchain-0.3.2/LICENSE
--rw-r--r--   0        0        0     6479 2020-02-02 00:00:00.000000 funcchain-0.3.2/README.md
--rw-r--r--   0        0        0     2348 2020-02-02 00:00:00.000000 funcchain-0.3.2/pyproject.toml
--rw-r--r--   0        0        0     8635 2020-02-02 00:00:00.000000 funcchain-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 funcchain-0.3.3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 funcchain-0.3.3/.readthedocs.yaml
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 funcchain-0.3.3/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1300 2020-02-02 00:00:00.000000 funcchain-0.3.3/MODELS.md
+-rwxr-xr-x   0        0        0     1032 2020-02-02 00:00:00.000000 funcchain-0.3.3/dev-setup.sh
+-rw-r--r--   0        0        0     3889 2020-02-02 00:00:00.000000 funcchain-0.3.3/mkdocs.yml
+-rw-r--r--   0        0        0     8961 2020-02-02 00:00:00.000000 funcchain-0.3.3/requirements-dev.lock
+-rw-r--r--   0        0        0     1784 2020-02-02 00:00:00.000000 funcchain-0.3.3/requirements.lock
+-rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 funcchain-0.3.3/roadmap.todo
+-rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 funcchain-0.3.3/.github/workflows/code-check.yml
+-rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 funcchain-0.3.3/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 funcchain-0.3.3/docs/changelog.md
+-rw-r--r--   0        0        0     4672 2020-02-02 00:00:00.000000 funcchain-0.3.3/docs/index.md
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 funcchain-0.3.3/docs/requirements.txt
+-rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 funcchain-0.3.3/docs/advanced/async.md
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 funcchain-0.3.3/docs/advanced/codebase-scaling.md
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 funcchain-0.3.3/docs/advanced/custom-parser-types.md
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 funcchain-0.3.3/docs/advanced/customization.md
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 funcchain-0.3.3/docs/advanced/runnables.md
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 funcchain-0.3.3/docs/advanced/signature.md
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 funcchain-0.3.3/docs/advanced/stream-parsing.md
+-rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 funcchain-0.3.3/docs/concepts/chain.md
+-rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 funcchain-0.3.3/docs/concepts/dependencies.md
+-rw-r--r--   0        0        0     1491 2020-02-02 00:00:00.000000 funcchain-0.3.3/docs/concepts/errors.md
+-rw-r--r--   0        0        0     2697 2020-02-02 00:00:00.000000 funcchain-0.3.3/docs/concepts/input.md
+-rw-r--r--   0        0        0     2809 2020-02-02 00:00:00.000000 funcchain-0.3.3/docs/concepts/langchain.md
+-rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 funcchain-0.3.3/docs/concepts/local-models.md
+-rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 funcchain-0.3.3/docs/concepts/overview.md
+-rw-r--r--   0        0        0     3630 2020-02-02 00:00:00.000000 funcchain-0.3.3/docs/concepts/parser.md
+-rw-r--r--   0        0        0     2228 2020-02-02 00:00:00.000000 funcchain-0.3.3/docs/concepts/prompting.md
+-rw-r--r--   0        0        0     2076 2020-02-02 00:00:00.000000 funcchain-0.3.3/docs/concepts/pydantic.md
+-rw-r--r--   0        0        0     1493 2020-02-02 00:00:00.000000 funcchain-0.3.3/docs/concepts/streaming.md
+-rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 funcchain-0.3.3/docs/concepts/unions.md
+-rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 funcchain-0.3.3/docs/concepts/vision.md
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 funcchain-0.3.3/docs/contributing/codebase-structure.md
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 funcchain-0.3.3/docs/contributing/contributors.md
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 funcchain-0.3.3/docs/contributing/dev-setup.md
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 funcchain-0.3.3/docs/contributing/license.md
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 funcchain-0.3.3/docs/contributing/roadmap.md
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 funcchain-0.3.3/docs/contributing/security.md
+-rw-r--r--   0        0        0     1126 2020-02-02 00:00:00.000000 funcchain-0.3.3/docs/css/custom.css
+-rw-r--r--   0        0        0     2065 2020-02-02 00:00:00.000000 funcchain-0.3.3/docs/css/termynal.css
+-rw-r--r--   0        0        0     7834 2020-02-02 00:00:00.000000 funcchain-0.3.3/docs/features/dynamic_router.md
+-rw-r--r--   0        0        0     2581 2020-02-02 00:00:00.000000 funcchain-0.3.3/docs/features/enums.md
+-rw-r--r--   0        0        0     2995 2020-02-02 00:00:00.000000 funcchain-0.3.3/docs/features/error_output.md
+-rw-r--r--   0        0        0     2487 2020-02-02 00:00:00.000000 funcchain-0.3.3/docs/features/literals.md
+-rw-r--r--   0        0        0     3394 2020-02-02 00:00:00.000000 funcchain-0.3.3/docs/features/llamacpp.md
+-rw-r--r--   0        0        0     3274 2020-02-02 00:00:00.000000 funcchain-0.3.3/docs/features/ollama.md
+-rw-r--r--   0        0        0     2319 2020-02-02 00:00:00.000000 funcchain-0.3.3/docs/features/openai_json_mode.md
+-rw-r--r--   0        0        0     3733 2020-02-02 00:00:00.000000 funcchain-0.3.3/docs/features/retry_parsing.md
+-rw-r--r--   0        0        0     4357 2020-02-02 00:00:00.000000 funcchain-0.3.3/docs/features/static_router.md
+-rw-r--r--   0        0        0     1944 2020-02-02 00:00:00.000000 funcchain-0.3.3/docs/features/stream.md
+-rw-r--r--   0        0        0     4043 2020-02-02 00:00:00.000000 funcchain-0.3.3/docs/features/vision.md
+-rw-r--r--   0        0        0     2996 2020-02-02 00:00:00.000000 funcchain-0.3.3/docs/getting-started/config.md
+-rw-r--r--   0        0        0    12075 2020-02-02 00:00:00.000000 funcchain-0.3.3/docs/getting-started/demos.md
+-rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 funcchain-0.3.3/docs/getting-started/installation.md
+-rw-r--r--   0        0        0     1429 2020-02-02 00:00:00.000000 funcchain-0.3.3/docs/getting-started/models.md
+-rw-r--r--   0        0        0     1272 2020-02-02 00:00:00.000000 funcchain-0.3.3/docs/getting-started/usage.md
+-rw-r--r--   0        0        0     4557 2020-02-02 00:00:00.000000 funcchain-0.3.3/docs/js/custom.js
+-rw-r--r--   0        0        0     8902 2020-02-02 00:00:00.000000 funcchain-0.3.3/docs/js/termynal.js
+-rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 funcchain-0.3.3/examples/chatgpt.py
+-rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 funcchain-0.3.3/examples/classify.py
+-rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 funcchain-0.3.3/examples/claude3.py
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 funcchain-0.3.3/examples/custom_lc_model.py
+-rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 funcchain-0.3.3/examples/custom_model_display.py
+-rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 funcchain-0.3.3/examples/decorator.py
+-rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 funcchain-0.3.3/examples/dict_type.py
+-rw-r--r--   0        0        0     2367 2020-02-02 00:00:00.000000 funcchain-0.3.3/examples/dynamic_router.py
+-rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 funcchain-0.3.3/examples/enums.py
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 funcchain-0.3.3/examples/error_output.py
+-rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 funcchain-0.3.3/examples/jinja.py
+-rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 funcchain-0.3.3/examples/literals.py
+-rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 funcchain-0.3.3/examples/llamacpp.py
+-rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 funcchain-0.3.3/examples/ollama.py
+-rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 funcchain-0.3.3/examples/openai_json_mode.py
+-rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 funcchain-0.3.3/examples/primitive_types.py
+-rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 funcchain-0.3.3/examples/pydantic_validation.py
+-rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 funcchain-0.3.3/examples/rag_with_deps.py
+-rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 funcchain-0.3.3/examples/runnable_deps.py
+-rw-r--r--   0        0        0     1432 2020-02-02 00:00:00.000000 funcchain-0.3.3/examples/static_router.py
+-rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 funcchain-0.3.3/examples/stream.py
+-rw-r--r--   0        0        0     2745 2020-02-02 00:00:00.000000 funcchain-0.3.3/examples/stream_runnables.py
+-rw-r--r--   0        0        0     1240 2020-02-02 00:00:00.000000 funcchain-0.3.3/examples/union_types.py
+-rw-r--r--   0        0        0      955 2020-02-02 00:00:00.000000 funcchain-0.3.3/examples/vision.py
+-rw-r--r--   0        0        0   326240 2020-02-02 00:00:00.000000 funcchain-0.3.3/examples/assets/old_chinese_temple.jpg
+-rw-r--r--   0        0        0     1354 2020-02-02 00:00:00.000000 funcchain-0.3.3/examples/async/expert_answer.py
+-rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 funcchain-0.3.3/examples/async/startup_names.py
+-rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 funcchain-0.3.3/examples/experiments/email_answering.py
+-rw-r--r--   0        0        0     2971 2020-02-02 00:00:00.000000 funcchain-0.3.3/examples/experiments/generate_pp_and_tos.py
+-rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 funcchain-0.3.3/examples/experiments/local_codeblock.py
+-rw-r--r--   0        0        0     3741 2020-02-02 00:00:00.000000 funcchain-0.3.3/examples/experiments/parallel_console_streaming.py
+-rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 funcchain-0.3.3/examples/simple/gather_infos.py
+-rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 funcchain-0.3.3/examples/simple/summary.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 funcchain-0.3.3/examples/simple/task_comparison.py
+-rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 funcchain-0.3.3/examples/simple/tutorial.py
+-rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 funcchain-0.3.3/src/funcchain/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 funcchain-0.3.3/src/funcchain/py.typed
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 funcchain-0.3.3/src/funcchain/backend/__init__.py
+-rw-r--r--   0        0        0    15287 2020-02-02 00:00:00.000000 funcchain-0.3.3/src/funcchain/backend/compiler.py
+-rw-r--r--   0        0        0     2552 2020-02-02 00:00:00.000000 funcchain-0.3.3/src/funcchain/backend/meta_inspect.py
+-rw-r--r--   0        0        0     5986 2020-02-02 00:00:00.000000 funcchain-0.3.3/src/funcchain/backend/prompt.py
+-rw-r--r--   0        0        0     2801 2020-02-02 00:00:00.000000 funcchain-0.3.3/src/funcchain/backend/settings.py
+-rw-r--r--   0        0        0     3453 2020-02-02 00:00:00.000000 funcchain-0.3.3/src/funcchain/backend/streaming.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 funcchain-0.3.3/src/funcchain/model/__init__.py
+-rw-r--r--   0        0        0     2434 2020-02-02 00:00:00.000000 funcchain-0.3.3/src/funcchain/model/abilities.py
+-rw-r--r--   0        0        0     5846 2020-02-02 00:00:00.000000 funcchain-0.3.3/src/funcchain/model/defaults.py
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 funcchain-0.3.3/src/funcchain/model/patches/__init__.py
+-rw-r--r--   0        0        0    14195 2020-02-02 00:00:00.000000 funcchain-0.3.3/src/funcchain/model/patches/llamacpp.py
+-rw-r--r--   0        0        0     6219 2020-02-02 00:00:00.000000 funcchain-0.3.3/src/funcchain/model/patches/ollama.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 funcchain-0.3.3/src/funcchain/parser/__init__.py
+-rw-r--r--   0        0        0     2192 2020-02-02 00:00:00.000000 funcchain-0.3.3/src/funcchain/parser/custom.py
+-rw-r--r--   0        0        0     3329 2020-02-02 00:00:00.000000 funcchain-0.3.3/src/funcchain/parser/json_schema.py
+-rw-r--r--   0        0        0     6312 2020-02-02 00:00:00.000000 funcchain-0.3.3/src/funcchain/parser/openai_functions.py
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 funcchain-0.3.3/src/funcchain/parser/primitive_types.py
+-rw-r--r--   0        0        0     5314 2020-02-02 00:00:00.000000 funcchain-0.3.3/src/funcchain/parser/schema_converter.py
+-rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 funcchain-0.3.3/src/funcchain/parser/selector.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 funcchain-0.3.3/src/funcchain/schema/__init__.py
+-rw-r--r--   0        0        0     1498 2020-02-02 00:00:00.000000 funcchain-0.3.3/src/funcchain/schema/signature.py
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 funcchain-0.3.3/src/funcchain/schema/types.py
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 funcchain-0.3.3/src/funcchain/syntax/__init__.py
+-rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 funcchain-0.3.3/src/funcchain/syntax/decorators.py
+-rw-r--r--   0        0        0     4913 2020-02-02 00:00:00.000000 funcchain-0.3.3/src/funcchain/syntax/executable.py
+-rw-r--r--   0        0        0     2367 2020-02-02 00:00:00.000000 funcchain-0.3.3/src/funcchain/syntax/input_types.py
+-rw-r--r--   0        0        0     1767 2020-02-02 00:00:00.000000 funcchain-0.3.3/src/funcchain/syntax/output_types.py
+-rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 funcchain-0.3.3/src/funcchain/syntax/params.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 funcchain-0.3.3/src/funcchain/syntax/components/__init__.py
+-rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 funcchain-0.3.3/src/funcchain/syntax/components/handler.py
+-rw-r--r--   0        0        0     4511 2020-02-02 00:00:00.000000 funcchain-0.3.3/src/funcchain/syntax/components/router.py
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 funcchain-0.3.3/src/funcchain/utils/__init__.py
+-rw-r--r--   0        0        0      918 2020-02-02 00:00:00.000000 funcchain-0.3.3/src/funcchain/utils/image.py
+-rw-r--r--   0        0        0     2214 2020-02-02 00:00:00.000000 funcchain-0.3.3/src/funcchain/utils/memory.py
+-rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 funcchain-0.3.3/src/funcchain/utils/msg_tools.py
+-rw-r--r--   0        0        0     2097 2020-02-02 00:00:00.000000 funcchain-0.3.3/src/funcchain/utils/pydantic.py
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 funcchain-0.3.3/src/funcchain/utils/token_counter.py
+-rw-r--r--   0        0        0     1458 2020-02-02 00:00:00.000000 funcchain-0.3.3/tests/async_test.py
+-rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 funcchain-0.3.3/tests/extraction_test.py
+-rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 funcchain-0.3.3/tests/run_examples_test.py
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 funcchain-0.3.3/tests/features/jinja_test.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 funcchain-0.3.3/tests/features/primitive_types_test.py
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 funcchain-0.3.3/tests/features/retry_validation_test.py
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 funcchain-0.3.3/tests/features/router_component_test.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 funcchain-0.3.3/tests/features/streaming_test.py
+-rw-r--r--   0        0        0     1823 2020-02-02 00:00:00.000000 funcchain-0.3.3/tests/models/llamacpp_test.py
+-rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 funcchain-0.3.3/tests/models/ollama_test.py
+-rw-r--r--   0        0        0     1330 2020-02-02 00:00:00.000000 funcchain-0.3.3/tests/models/openai_test.py
+-rw-r--r--   0        0        0     3148 2020-02-02 00:00:00.000000 funcchain-0.3.3/.gitignore
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 funcchain-0.3.3/LICENSE
+-rw-r--r--   0        0        0     6479 2020-02-02 00:00:00.000000 funcchain-0.3.3/README.md
+-rw-r--r--   0        0        0     2348 2020-02-02 00:00:00.000000 funcchain-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0     8936 2020-02-02 00:00:00.000000 funcchain-0.3.3/PKG-INFO
```

### Comparing `funcchain-0.3.2/MODELS.md` & `funcchain-0.3.3/MODELS.md`

 * *Files identical despite different names*

### Comparing `funcchain-0.3.2/dev-setup.sh` & `funcchain-0.3.3/dev-setup.sh`

 * *Files identical despite different names*

### Comparing `funcchain-0.3.2/mkdocs.yml` & `funcchain-0.3.3/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `funcchain-0.3.2/requirements-dev.lock` & `funcchain-0.3.3/requirements-dev.lock`

 * *Files identical despite different names*

### Comparing `funcchain-0.3.2/requirements.lock` & `funcchain-0.3.3/requirements.lock`

 * *Files identical despite different names*

### Comparing `funcchain-0.3.2/roadmap.todo` & `funcchain-0.3.3/roadmap.todo`

 * *Files identical despite different names*

### Comparing `funcchain-0.3.2/.github/workflows/code-check.yml` & `funcchain-0.3.3/.github/workflows/code-check.yml`

 * *Files identical despite different names*

### Comparing `funcchain-0.3.2/.github/workflows/python-publish.yml` & `funcchain-0.3.3/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `funcchain-0.3.2/docs/changelog.md` & `funcchain-0.3.3/docs/changelog.md`

 * *Files identical despite different names*

### Comparing `funcchain-0.3.2/docs/index.md` & `funcchain-0.3.3/docs/index.md`

 * *Files identical despite different names*

### Comparing `funcchain-0.3.2/docs/advanced/async.md` & `funcchain-0.3.3/docs/advanced/async.md`

 * *Files identical despite different names*

### Comparing `funcchain-0.3.2/docs/concepts/chain.md` & `funcchain-0.3.3/docs/concepts/chain.md`

 * *Files identical despite different names*

### Comparing `funcchain-0.3.2/docs/concepts/dependencies.md` & `funcchain-0.3.3/docs/concepts/dependencies.md`

 * *Files identical despite different names*

### Comparing `funcchain-0.3.2/docs/concepts/errors.md` & `funcchain-0.3.3/docs/concepts/errors.md`

 * *Files identical despite different names*

### Comparing `funcchain-0.3.2/docs/concepts/input.md` & `funcchain-0.3.3/docs/concepts/input.md`

 * *Files identical despite different names*

### Comparing `funcchain-0.3.2/docs/concepts/langchain.md` & `funcchain-0.3.3/docs/concepts/langchain.md`

 * *Files identical despite different names*

### Comparing `funcchain-0.3.2/docs/concepts/local-models.md` & `funcchain-0.3.3/docs/concepts/local-models.md`

 * *Files identical despite different names*

### Comparing `funcchain-0.3.2/docs/concepts/overview.md` & `funcchain-0.3.3/docs/concepts/overview.md`

 * *Files identical despite different names*

### Comparing `funcchain-0.3.2/docs/concepts/parser.md` & `funcchain-0.3.3/docs/concepts/parser.md`

 * *Files identical despite different names*

### Comparing `funcchain-0.3.2/docs/concepts/prompting.md` & `funcchain-0.3.3/docs/concepts/prompting.md`

 * *Files identical despite different names*

### Comparing `funcchain-0.3.2/docs/concepts/pydantic.md` & `funcchain-0.3.3/docs/concepts/pydantic.md`

 * *Files identical despite different names*

### Comparing `funcchain-0.3.2/docs/concepts/streaming.md` & `funcchain-0.3.3/docs/concepts/streaming.md`

 * *Files identical despite different names*

### Comparing `funcchain-0.3.2/docs/concepts/unions.md` & `funcchain-0.3.3/docs/concepts/unions.md`

 * *Files identical despite different names*

### Comparing `funcchain-0.3.2/docs/concepts/vision.md` & `funcchain-0.3.3/docs/concepts/vision.md`

 * *Files identical despite different names*

### Comparing `funcchain-0.3.2/docs/css/custom.css` & `funcchain-0.3.3/docs/css/custom.css`

 * *Files identical despite different names*

### Comparing `funcchain-0.3.2/docs/css/termynal.css` & `funcchain-0.3.3/docs/css/termynal.css`

 * *Files identical despite different names*

### Comparing `funcchain-0.3.2/docs/features/dynamic_router.md` & `funcchain-0.3.3/docs/features/dynamic_router.md`

 * *Files identical despite different names*

### Comparing `funcchain-0.3.2/docs/features/enums.md` & `funcchain-0.3.3/docs/features/enums.md`

 * *Files identical despite different names*

### Comparing `funcchain-0.3.2/docs/features/error_output.md` & `funcchain-0.3.3/docs/features/error_output.md`

 * *Files identical despite different names*

### Comparing `funcchain-0.3.2/docs/features/literals.md` & `funcchain-0.3.3/docs/features/literals.md`

 * *Files identical despite different names*

### Comparing `funcchain-0.3.2/docs/features/llamacpp.md` & `funcchain-0.3.3/docs/features/llamacpp.md`

 * *Files identical despite different names*

### Comparing `funcchain-0.3.2/docs/features/ollama.md` & `funcchain-0.3.3/docs/features/ollama.md`

 * *Files identical despite different names*

### Comparing `funcchain-0.3.2/docs/features/openai_json_mode.md` & `funcchain-0.3.3/docs/features/openai_json_mode.md`

 * *Files identical despite different names*

### Comparing `funcchain-0.3.2/docs/features/retry_parsing.md` & `funcchain-0.3.3/docs/features/retry_parsing.md`

 * *Files identical despite different names*

### Comparing `funcchain-0.3.2/docs/features/static_router.md` & `funcchain-0.3.3/docs/features/static_router.md`

 * *Files identical despite different names*

### Comparing `funcchain-0.3.2/docs/features/stream.md` & `funcchain-0.3.3/docs/features/stream.md`

 * *Files identical despite different names*

### Comparing `funcchain-0.3.2/docs/features/vision.md` & `funcchain-0.3.3/docs/features/vision.md`

 * *Files identical despite different names*

### Comparing `funcchain-0.3.2/docs/getting-started/config.md` & `funcchain-0.3.3/docs/getting-started/config.md`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     Analyse the output and determine if the goal is reached.
     """
     return chain(settings_override=settings)
 
 result = analyse_output(
     "healthy outpout",
     "Hello World!",
-    settings_override={"llm": "openai/gpt-4-vision-preview"},
+    settings={"llm": "openai/gpt-4-vision-preview"},
 )
 ```
 
 The `settings_override` argument is a `SettingsOverride` object which is a dict-like object that can be used to override the global settings.
 You will get suggestions from your IDE on what settings you can override due to the type hints.
 
 ## Settings Class Overview
```

### Comparing `funcchain-0.3.2/docs/getting-started/demos.md` & `funcchain-0.3.3/docs/getting-started/demos.md`

 * *Files identical despite different names*

### Comparing `funcchain-0.3.2/docs/getting-started/installation.md` & `funcchain-0.3.3/docs/getting-started/installation.md`

 * *Files identical despite different names*

### Comparing `funcchain-0.3.2/docs/getting-started/models.md` & `funcchain-0.3.3/docs/getting-started/models.md`

 * *Files identical despite different names*

### Comparing `funcchain-0.3.2/docs/getting-started/usage.md` & `funcchain-0.3.3/docs/getting-started/usage.md`

 * *Files identical despite different names*

### Comparing `funcchain-0.3.2/docs/js/custom.js` & `funcchain-0.3.3/docs/js/custom.js`

 * *Files identical despite different names*

### Comparing `funcchain-0.3.2/docs/js/termynal.js` & `funcchain-0.3.3/docs/js/termynal.js`

 * *Files identical despite different names*

### Comparing `funcchain-0.3.2/examples/chatgpt.py` & `funcchain-0.3.3/examples/chatgpt.py`

 * *Files identical despite different names*

### Comparing `funcchain-0.3.2/examples/claude3.py` & `funcchain-0.3.3/examples/claude3.py`

 * *Files identical despite different names*

### Comparing `funcchain-0.3.2/examples/custom_model_display.py` & `funcchain-0.3.3/examples/custom_model_display.py`

 * *Files identical despite different names*

### Comparing `funcchain-0.3.2/examples/decorator.py` & `funcchain-0.3.3/examples/decorator.py`

 * *Files identical despite different names*

### Comparing `funcchain-0.3.2/examples/dynamic_router.py` & `funcchain-0.3.3/examples/dynamic_router.py`

 * *Files identical despite different names*

### Comparing `funcchain-0.3.2/examples/jinja.py` & `funcchain-0.3.3/examples/jinja.py`

 * *Files identical despite different names*

### Comparing `funcchain-0.3.2/examples/llamacpp.py` & `funcchain-0.3.3/examples/llamacpp.py`

 * *Files identical despite different names*

### Comparing `funcchain-0.3.2/examples/ollama.py` & `funcchain-0.3.3/examples/ollama.py`

 * *Files identical despite different names*

### Comparing `funcchain-0.3.2/examples/pydantic_validation.py` & `funcchain-0.3.3/examples/pydantic_validation.py`

 * *Files identical despite different names*

### Comparing `funcchain-0.3.2/examples/rag_with_deps.py` & `funcchain-0.3.3/examples/rag_with_deps.py`

 * *Files identical despite different names*

### Comparing `funcchain-0.3.2/examples/static_router.py` & `funcchain-0.3.3/examples/static_router.py`

 * *Files identical despite different names*

### Comparing `funcchain-0.3.2/examples/stream_runnables.py` & `funcchain-0.3.3/examples/stream_runnables.py`

 * *Files identical despite different names*

### Comparing `funcchain-0.3.2/examples/union_types.py` & `funcchain-0.3.3/examples/union_types.py`

 * *Files identical despite different names*

### Comparing `funcchain-0.3.2/examples/vision.py` & `funcchain-0.3.3/examples/vision.py`

 * *Files identical despite different names*

### Comparing `funcchain-0.3.2/examples/assets/old_chinese_temple.jpg` & `funcchain-0.3.3/examples/assets/old_chinese_temple.jpg`

 * *Files identical despite different names*

### Comparing `funcchain-0.3.2/examples/async/expert_answer.py` & `funcchain-0.3.3/examples/async/expert_answer.py`

 * *Files identical despite different names*

### Comparing `funcchain-0.3.2/examples/async/startup_names.py` & `funcchain-0.3.3/examples/async/startup_names.py`

 * *Files identical despite different names*

### Comparing `funcchain-0.3.2/examples/experiments/email_answering.py` & `funcchain-0.3.3/examples/experiments/email_answering.py`

 * *Files identical despite different names*

### Comparing `funcchain-0.3.2/examples/experiments/generate_pp_and_tos.py` & `funcchain-0.3.3/examples/experiments/generate_pp_and_tos.py`

 * *Files identical despite different names*

### Comparing `funcchain-0.3.2/examples/experiments/parallel_console_streaming.py` & `funcchain-0.3.3/examples/experiments/parallel_console_streaming.py`

 * *Files identical despite different names*

### Comparing `funcchain-0.3.2/examples/simple/gather_infos.py` & `funcchain-0.3.3/examples/simple/gather_infos.py`

 * *Files identical despite different names*

### Comparing `funcchain-0.3.2/examples/simple/task_comparison.py` & `funcchain-0.3.3/examples/simple/task_comparison.py`

 * *Files identical despite different names*

### Comparing `funcchain-0.3.2/examples/simple/tutorial.py` & `funcchain-0.3.3/examples/simple/tutorial.py`

 * *Files identical despite different names*

### Comparing `funcchain-0.3.2/src/funcchain/backend/compiler.py` & `funcchain-0.3.3/src/funcchain/backend/compiler.py`

 * *Files identical despite different names*

### Comparing `funcchain-0.3.2/src/funcchain/backend/meta_inspect.py` & `funcchain-0.3.3/src/funcchain/backend/meta_inspect.py`

 * *Files identical despite different names*

### Comparing `funcchain-0.3.2/src/funcchain/backend/prompt.py` & `funcchain-0.3.3/src/funcchain/backend/prompt.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,14 +19,17 @@
     instruction: str,
     images: list[Image],
     input_kwargs: dict[str, Any],
     format_instructions: Optional[str] = None,
 ) -> "HumanImageMessagePromptTemplate":
     template_format = _determine_format(instruction)
 
+    if template_format == "jinja2" and "\n{format_instructions}" in instruction:
+        instruction = instruction.replace("\n{format_instructions}", "\n{{ format_instructions }}")
+
     required_f_str_vars = _extract_template_vars(instruction, template_format)
 
     _filter_fstring_vars(input_kwargs)
 
     inject_vars = [f"{var.upper()}:\n{{{var}}}\n" for var, _ in input_kwargs.items() if var not in required_f_str_vars]
 
     added_instruction = "\n".join(inject_vars)
```

### Comparing `funcchain-0.3.2/src/funcchain/backend/settings.py` & `funcchain-0.3.3/src/funcchain/backend/settings.py`

 * *Files identical despite different names*

### Comparing `funcchain-0.3.2/src/funcchain/backend/streaming.py` & `funcchain-0.3.3/src/funcchain/backend/streaming.py`

 * *Files identical despite different names*

### Comparing `funcchain-0.3.2/src/funcchain/model/abilities.py` & `funcchain-0.3.3/src/funcchain/model/abilities.py`

 * *Files identical despite different names*

### Comparing `funcchain-0.3.2/src/funcchain/model/defaults.py` & `funcchain-0.3.3/src/funcchain/model/defaults.py`

 * *Files identical despite different names*

### Comparing `funcchain-0.3.2/src/funcchain/model/patches/llamacpp.py` & `funcchain-0.3.3/src/funcchain/model/patches/llamacpp.py`

 * *Files identical despite different names*

### Comparing `funcchain-0.3.2/src/funcchain/model/patches/ollama.py` & `funcchain-0.3.3/src/funcchain/model/patches/ollama.py`

 * *Files identical despite different names*

### Comparing `funcchain-0.3.2/src/funcchain/parser/custom.py` & `funcchain-0.3.3/src/funcchain/parser/custom.py`

 * *Files identical despite different names*

### Comparing `funcchain-0.3.2/src/funcchain/parser/json_schema.py` & `funcchain-0.3.3/src/funcchain/parser/json_schema.py`

 * *Files identical despite different names*

### Comparing `funcchain-0.3.2/src/funcchain/parser/openai_functions.py` & `funcchain-0.3.3/src/funcchain/parser/openai_functions.py`

 * *Files identical despite different names*

### Comparing `funcchain-0.3.2/src/funcchain/parser/primitive_types.py` & `funcchain-0.3.3/src/funcchain/parser/primitive_types.py`

 * *Files identical despite different names*

### Comparing `funcchain-0.3.2/src/funcchain/parser/schema_converter.py` & `funcchain-0.3.3/src/funcchain/parser/schema_converter.py`

 * *Files identical despite different names*

### Comparing `funcchain-0.3.2/src/funcchain/parser/selector.py` & `funcchain-0.3.3/src/funcchain/parser/selector.py`

 * *Files identical despite different names*

### Comparing `funcchain-0.3.2/src/funcchain/schema/signature.py` & `funcchain-0.3.3/src/funcchain/schema/signature.py`

 * *Files identical despite different names*

### Comparing `funcchain-0.3.2/src/funcchain/syntax/decorators.py` & `funcchain-0.3.3/src/funcchain/syntax/decorators.py`

 * *Files 24% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 
 @overload
 def runnable(
     *,
     llm: UniversalChatModel = None,
     settings: SettingsOverride = {},
-) -> Callable[[Callable], Runnable]:
+) -> Callable[[Callable[..., OutputT]], Runnable[dict[str, Any], OutputT]]:
     ...
 
 
 def runnable(
     f: Optional[Callable[..., OutputT]] = None,
     *,
     llm: UniversalChatModel = None,
```

### Comparing `funcchain-0.3.2/src/funcchain/syntax/executable.py` & `funcchain-0.3.3/src/funcchain/syntax/executable.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,27 +23,31 @@
 def chain(
     *,
     system: str | None = None,
     instruction: str | None = None,
     context: list[BaseMessage] = [],
     memory: BaseChatMessageHistory | None = None,
     settings_override: SettingsOverride = {},
+    llm: UniversalChatModel | None = None,
     **input_kwargs: Any,
 ) -> Any:
     """
     Generate response of llm for provided instructions.
     """
     settings = create_local_settings(settings_override)
     callbacks: Callbacks = None
     output_types = get_output_types()
     input_args: list[tuple[str, type]] = args_from_parent()
 
     memory = memory or ChatMessageHistory()
     input_kwargs.update(kwargs_from_parent())
 
+    if llm:
+        settings_override["llm"] = llm
+
     # todo maybe this should be done in the prompt processor?
     system = system or settings.system_prompt
     if system:
         context = [SystemMessage(content=system)] + context
     instruction = instruction or from_docstring()
 
     # temp image handling
@@ -73,27 +77,31 @@
 async def achain(
     *,
     system: str | None = None,
     instruction: str | None = None,
     context: list[BaseMessage] = [],
     memory: BaseChatMessageHistory | None = None,
     settings_override: SettingsOverride = {},
+    llm: UniversalChatModel | None = None,
     **input_kwargs: Any,
 ) -> Any:
     """
     Asyncronously generate response of llm for provided instructions.
     """
     settings = create_local_settings(settings_override)
     callbacks: Callbacks = None
     output_types = get_output_types()
     input_args: list[tuple[str, type]] = args_from_parent()
 
     memory = memory or ChatMessageHistory()
     input_kwargs.update(kwargs_from_parent())
 
+    if llm:
+        settings_override["llm"] = llm
+
     # todo maybe this should be done in the prompt processor?
     system = system or settings.system_prompt
     if system:
         context = [SystemMessage(content=system)] + context
     instruction = instruction or from_docstring()
 
     # temp image handling
@@ -132,15 +140,15 @@
     llm: UniversalChatModel = None,
     system: str = "",
     settings_override: SettingsOverride = {},
 ) -> Runnable[dict[str, Any], ChainOut]:
     """
     On the fly compilation of the funcchain syntax.
     """
-    if settings_override and llm:
+    if llm:
         settings_override["llm"] = llm
     instruction = "\n" + instruction
     settings = create_local_settings(settings_override)
     context = [SystemMessage(content=system)] + context
     _input_args: list[tuple[str, type]] = [(arg, str) for arg in input_args]
 
     sig: Signature = Signature(
```

### Comparing `funcchain-0.3.2/src/funcchain/syntax/input_types.py` & `funcchain-0.3.3/src/funcchain/syntax/input_types.py`

 * *Files identical despite different names*

### Comparing `funcchain-0.3.2/src/funcchain/syntax/output_types.py` & `funcchain-0.3.3/src/funcchain/syntax/output_types.py`

 * *Files identical despite different names*

### Comparing `funcchain-0.3.2/src/funcchain/syntax/components/handler.py` & `funcchain-0.3.3/src/funcchain/syntax/components/handler.py`

 * *Files identical despite different names*

### Comparing `funcchain-0.3.2/src/funcchain/syntax/components/router.py` & `funcchain-0.3.3/src/funcchain/syntax/components/router.py`

 * *Files identical despite different names*

### Comparing `funcchain-0.3.2/src/funcchain/utils/image.py` & `funcchain-0.3.3/src/funcchain/utils/image.py`

 * *Files identical despite different names*

### Comparing `funcchain-0.3.2/src/funcchain/utils/memory.py` & `funcchain-0.3.3/src/funcchain/utils/memory.py`

 * *Files identical despite different names*

### Comparing `funcchain-0.3.2/src/funcchain/utils/msg_tools.py` & `funcchain-0.3.3/src/funcchain/utils/msg_tools.py`

 * *Files identical despite different names*

### Comparing `funcchain-0.3.2/src/funcchain/utils/pydantic.py` & `funcchain-0.3.3/src/funcchain/utils/pydantic.py`

 * *Files identical despite different names*

### Comparing `funcchain-0.3.2/tests/async_test.py` & `funcchain-0.3.3/tests/async_test.py`

 * *Files identical despite different names*

### Comparing `funcchain-0.3.2/tests/extraction_test.py` & `funcchain-0.3.3/tests/extraction_test.py`

 * *Files identical despite different names*

### Comparing `funcchain-0.3.2/tests/run_examples_test.py` & `funcchain-0.3.3/tests/run_examples_test.py`

 * *Files identical despite different names*

### Comparing `funcchain-0.3.2/tests/models/llamacpp_test.py` & `funcchain-0.3.3/tests/models/llamacpp_test.py`

 * *Files identical despite different names*

### Comparing `funcchain-0.3.2/tests/models/ollama_test.py` & `funcchain-0.3.3/tests/models/ollama_test.py`

 * *Files identical despite different names*

### Comparing `funcchain-0.3.2/tests/models/openai_test.py` & `funcchain-0.3.3/tests/models/openai_test.py`

 * *Files identical despite different names*

### Comparing `funcchain-0.3.2/.gitignore` & `funcchain-0.3.3/.gitignore`

 * *Files identical despite different names*

### Comparing `funcchain-0.3.2/LICENSE` & `funcchain-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `funcchain-0.3.2/README.md` & `funcchain-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `funcchain-0.3.2/pyproject.toml` & `funcchain-0.3.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "funcchain"
-version = "0.3.2"
+version = "0.3.3"
 description = "🔖 write prompts as python functions"
 authors = [{ name = "Shroominic", email = "contact@shroominic.com" }]
 dependencies = [
     "langchain-core>=0.1",
     "pydantic-settings>=2",
     "docstring-parser>=0.15",
     "jinja2>=3",
```

### Comparing `funcchain-0.3.2/PKG-INFO` & `funcchain-0.3.3/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: funcchain
-Version: 0.3.2
+Version: 0.3.3
 Summary: 🔖 write prompts as python functions
 Project-URL: Code, https://github.com/shroominic/funcchain
 Project-URL: Documentation, https://shroominic.github.io/funcchain
 Author-email: Shroominic <contact@shroominic.com>
 License-Expression: MIT
 License-File: LICENSE
 Keywords: agent framework,ai,cognitive systems,funcchain,langchain,llm,pydantic,pythonic
@@ -16,21 +16,27 @@
 Requires-Python: <3.13,>=3.10
 Requires-Dist: docstring-parser>=0.15
 Requires-Dist: jinja2>=3
 Requires-Dist: langchain-core>=0.1
 Requires-Dist: langchain-openai>=0.0.8
 Requires-Dist: pydantic-settings>=2
 Provides-Extra: all
-Requires-Dist: funcchain[anthropic]; extra == 'all'
-Requires-Dist: funcchain[extras]; extra == 'all'
-Requires-Dist: funcchain[google]; extra == 'all'
-Requires-Dist: funcchain[image]; extra == 'all'
-Requires-Dist: funcchain[llamacpp]; extra == 'all'
-Requires-Dist: funcchain[ollama]; extra == 'all'
-Requires-Dist: funcchain[openai]; extra == 'all'
+Requires-Dist: beautifulsoup4>=4.12; extra == 'all'
+Requires-Dist: faiss-cpu>=1.7.4; extra == 'all'
+Requires-Dist: huggingface-hub>=0.20; extra == 'all'
+Requires-Dist: langchain-anthropic; extra == 'all'
+Requires-Dist: langchain-community; extra == 'all'
+Requires-Dist: langchain-google-genai; extra == 'all'
+Requires-Dist: langchain-openai; extra == 'all'
+Requires-Dist: langchain>=0.1; extra == 'all'
+Requires-Dist: llama-cpp-python>=0.2.32; extra == 'all'
+Requires-Dist: pdf2image>=1.17.0; extra == 'all'
+Requires-Dist: pdfminer>=20191125; extra == 'all'
+Requires-Dist: pillow; extra == 'all'
+Requires-Dist: unstructured>=0.12.5; extra == 'all'
 Provides-Extra: anthropic
 Requires-Dist: langchain-anthropic; extra == 'anthropic'
 Provides-Extra: extras
 Requires-Dist: beautifulsoup4>=4.12; extra == 'extras'
 Requires-Dist: faiss-cpu>=1.7.4; extra == 'extras'
 Requires-Dist: langchain>=0.1; extra == 'extras'
 Requires-Dist: pdf2image>=1.17.0; extra == 'extras'
```

