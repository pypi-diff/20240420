# Comparing `tmp/adaptix-3.0.0b4.tar.gz` & `tmp/adaptix-3.0.0b5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adaptix-3.0.0b4.tar", last modified: Sat Mar 30 14:09:36 2024, max compression
+gzip compressed data, was "adaptix-3.0.0b5.tar", last modified: Sat Apr 20 08:07:26 2024, max compression
```

## Comparing `adaptix-3.0.0b4.tar` & `adaptix-3.0.0b5.tar`

### file list

```diff
@@ -1,137 +1,149 @@
-drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2024-03-30 14:09:36.576219 adaptix-3.0.0b4/
--rw-rw-r--   0 pavel     (1000) pavel     (1000)    11357 2021-06-13 21:15:36.000000 adaptix-3.0.0b4/LICENSE
--rw-r--r--   0 pavel     (1000) pavel     (1000)     6548 2024-03-30 14:09:36.576219 adaptix-3.0.0b4/PKG-INFO
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     4522 2024-03-30 14:01:32.000000 adaptix-3.0.0b4/README.md
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     5043 2024-03-30 14:01:32.000000 adaptix-3.0.0b4/pyproject.toml
--rw-rw-r--   0 pavel     (1000) pavel     (1000)       38 2024-03-30 14:09:36.576219 adaptix-3.0.0b4/setup.cfg
-drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2024-03-30 14:09:36.564219 adaptix-3.0.0b4/src/
-drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2024-03-30 14:09:36.564219 adaptix-3.0.0b4/src/adaptix/
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     2128 2024-03-30 13:12:56.000000 adaptix-3.0.0b4/src/adaptix/__init__.py
-drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2024-03-30 14:09:36.568219 adaptix-3.0.0b4/src/adaptix/_internal/
--rw-rw-r--   0 pavel     (1000) pavel     (1000)        0 2024-03-17 07:48:08.000000 adaptix-3.0.0b4/src/adaptix/_internal/__init__.py
-drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2024-03-30 14:09:36.568219 adaptix-3.0.0b4/src/adaptix/_internal/code_tools/
--rw-rw-r--   0 pavel     (1000) pavel     (1000)        0 2024-03-17 07:48:08.000000 adaptix-3.0.0b4/src/adaptix/_internal/code_tools/__init__.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)      619 2024-03-30 13:54:05.000000 adaptix-3.0.0b4/src/adaptix/_internal/code_tools/ast_templater.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     3045 2024-03-30 13:54:05.000000 adaptix-3.0.0b4/src/adaptix/_internal/code_tools/cascade_namespace.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     2920 2024-03-30 13:54:05.000000 adaptix-3.0.0b4/src/adaptix/_internal/code_tools/code_builder.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     2634 2024-03-30 13:54:05.000000 adaptix-3.0.0b4/src/adaptix/_internal/code_tools/compiler.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)      558 2024-03-17 07:48:08.000000 adaptix-3.0.0b4/src/adaptix/_internal/code_tools/name_sanitizer.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     2718 2024-03-30 13:54:05.000000 adaptix-3.0.0b4/src/adaptix/_internal/code_tools/utils.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)      639 2024-03-30 13:54:05.000000 adaptix-3.0.0b4/src/adaptix/_internal/common.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)      322 2024-03-17 07:48:08.000000 adaptix-3.0.0b4/src/adaptix/_internal/compat.py
-drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2024-03-30 14:09:36.568219 adaptix-3.0.0b4/src/adaptix/_internal/conversion/
--rw-rw-r--   0 pavel     (1000) pavel     (1000)        0 2024-03-17 07:48:08.000000 adaptix-3.0.0b4/src/adaptix/_internal/conversion/__init__.py
-drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2024-03-30 14:09:36.568219 adaptix-3.0.0b4/src/adaptix/_internal/conversion/broaching/
--rw-rw-r--   0 pavel     (1000) pavel     (1000)        0 2024-03-17 07:48:08.000000 adaptix-3.0.0b4/src/adaptix/_internal/conversion/broaching/__init__.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     7760 2024-03-30 13:54:05.000000 adaptix-3.0.0b4/src/adaptix/_internal/conversion/broaching/code_generator.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     1187 2024-03-17 07:48:08.000000 adaptix-3.0.0b4/src/adaptix/_internal/conversion/broaching/definitions.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)    10709 2024-03-30 13:54:05.000000 adaptix-3.0.0b4/src/adaptix/_internal/conversion/coercer_provider.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     6976 2024-03-30 13:54:05.000000 adaptix-3.0.0b4/src/adaptix/_internal/conversion/converter_provider.py
-drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2024-03-30 14:09:36.568219 adaptix-3.0.0b4/src/adaptix/_internal/conversion/facade/
--rw-rw-r--   0 pavel     (1000) pavel     (1000)        0 2024-03-17 07:48:08.000000 adaptix-3.0.0b4/src/adaptix/_internal/conversion/facade/__init__.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)      749 2024-03-30 13:54:05.000000 adaptix-3.0.0b4/src/adaptix/_internal/conversion/facade/checker.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     2311 2024-03-17 07:48:08.000000 adaptix-3.0.0b4/src/adaptix/_internal/conversion/facade/func.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     3855 2024-03-30 13:54:05.000000 adaptix-3.0.0b4/src/adaptix/_internal/conversion/facade/provider.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     6216 2024-03-30 13:54:05.000000 adaptix-3.0.0b4/src/adaptix/_internal/conversion/facade/retort.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     2661 2024-03-30 13:54:05.000000 adaptix-3.0.0b4/src/adaptix/_internal/conversion/linking_provider.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)    11225 2024-03-30 13:54:05.000000 adaptix-3.0.0b4/src/adaptix/_internal/conversion/model_coercer_provider.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)      594 2024-03-17 07:48:08.000000 adaptix-3.0.0b4/src/adaptix/_internal/conversion/policy_provider.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     1068 2024-03-30 13:54:05.000000 adaptix-3.0.0b4/src/adaptix/_internal/conversion/provider_template.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     1928 2024-03-30 13:54:05.000000 adaptix-3.0.0b4/src/adaptix/_internal/conversion/request_cls.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     7757 2024-03-30 13:54:05.000000 adaptix-3.0.0b4/src/adaptix/_internal/datastructures.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)      108 2024-03-17 07:48:08.000000 adaptix-3.0.0b4/src/adaptix/_internal/definitions.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     5323 2024-03-17 07:48:08.000000 adaptix-3.0.0b4/src/adaptix/_internal/feature_requirement.py
-drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2024-03-30 14:09:36.568219 adaptix-3.0.0b4/src/adaptix/_internal/model_tools/
--rw-rw-r--   0 pavel     (1000) pavel     (1000)        0 2024-03-17 07:48:08.000000 adaptix-3.0.0b4/src/adaptix/_internal/model_tools/__init__.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)    10098 2024-03-30 13:54:05.000000 adaptix-3.0.0b4/src/adaptix/_internal/model_tools/definitions.py
-drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2024-03-30 14:09:36.568219 adaptix-3.0.0b4/src/adaptix/_internal/model_tools/introspection/
--rw-rw-r--   0 pavel     (1000) pavel     (1000)        0 2024-03-17 07:48:08.000000 adaptix-3.0.0b4/src/adaptix/_internal/model_tools/introspection/__init__.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     4861 2024-03-30 13:54:05.000000 adaptix-3.0.0b4/src/adaptix/_internal/model_tools/introspection/attrs.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     3484 2024-03-30 13:54:05.000000 adaptix-3.0.0b4/src/adaptix/_internal/model_tools/introspection/callable.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)      497 2024-03-30 13:54:05.000000 adaptix-3.0.0b4/src/adaptix/_internal/model_tools/introspection/class_init.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     3812 2024-03-30 13:54:05.000000 adaptix-3.0.0b4/src/adaptix/_internal/model_tools/introspection/dataclass.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     2207 2024-03-30 13:54:05.000000 adaptix-3.0.0b4/src/adaptix/_internal/model_tools/introspection/named_tuple.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     7894 2024-03-30 13:54:05.000000 adaptix-3.0.0b4/src/adaptix/_internal/model_tools/introspection/sqlalchemy.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     4342 2024-03-30 13:54:05.000000 adaptix-3.0.0b4/src/adaptix/_internal/model_tools/introspection/typed_dict.py
-drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2024-03-30 14:09:36.572219 adaptix-3.0.0b4/src/adaptix/_internal/morphing/
--rw-rw-r--   0 pavel     (1000) pavel     (1000)        0 2024-03-17 07:48:08.000000 adaptix-3.0.0b4/src/adaptix/_internal/morphing/__init__.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)    12164 2024-03-30 13:54:05.000000 adaptix-3.0.0b4/src/adaptix/_internal/morphing/concrete_provider.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)    12270 2024-03-30 13:54:05.000000 adaptix-3.0.0b4/src/adaptix/_internal/morphing/constant_length_tuple_provider.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)    10886 2024-03-30 13:54:05.000000 adaptix-3.0.0b4/src/adaptix/_internal/morphing/dict_provider.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)    12333 2024-03-30 13:54:05.000000 adaptix-3.0.0b4/src/adaptix/_internal/morphing/enum_provider.py
-drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2024-03-30 14:09:36.572219 adaptix-3.0.0b4/src/adaptix/_internal/morphing/facade/
--rw-rw-r--   0 pavel     (1000) pavel     (1000)        0 2024-03-17 07:48:08.000000 adaptix-3.0.0b4/src/adaptix/_internal/morphing/facade/__init__.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)      618 2024-03-17 07:48:08.000000 adaptix-3.0.0b4/src/adaptix/_internal/morphing/facade/func.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)    16413 2024-03-30 13:54:05.000000 adaptix-3.0.0b4/src/adaptix/_internal/morphing/facade/provider.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     9436 2024-03-30 13:54:05.000000 adaptix-3.0.0b4/src/adaptix/_internal/morphing/facade/retort.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)    17074 2024-03-30 13:54:05.000000 adaptix-3.0.0b4/src/adaptix/_internal/morphing/generic_provider.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)    10078 2024-03-30 13:54:05.000000 adaptix-3.0.0b4/src/adaptix/_internal/morphing/iterable_provider.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     3869 2024-03-30 13:54:05.000000 adaptix-3.0.0b4/src/adaptix/_internal/morphing/load_error.py
-drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2024-03-30 14:09:36.572219 adaptix-3.0.0b4/src/adaptix/_internal/morphing/model/
--rw-rw-r--   0 pavel     (1000) pavel     (1000)        0 2024-03-17 07:48:08.000000 adaptix-3.0.0b4/src/adaptix/_internal/morphing/model/__init__.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     7648 2024-03-30 13:54:05.000000 adaptix-3.0.0b4/src/adaptix/_internal/morphing/model/basic_gen.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     4313 2024-03-17 07:48:08.000000 adaptix-3.0.0b4/src/adaptix/_internal/morphing/model/crown_definitions.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)    23272 2024-03-30 13:54:05.000000 adaptix-3.0.0b4/src/adaptix/_internal/morphing/model/dumper_gen.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     6031 2024-03-30 13:54:05.000000 adaptix-3.0.0b4/src/adaptix/_internal/morphing/model/dumper_provider.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)    28138 2024-03-30 13:54:05.000000 adaptix-3.0.0b4/src/adaptix/_internal/morphing/model/loader_gen.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     7907 2024-03-30 13:54:05.000000 adaptix-3.0.0b4/src/adaptix/_internal/morphing/model/loader_provider.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)      696 2024-03-17 07:48:08.000000 adaptix-3.0.0b4/src/adaptix/_internal/morphing/model/request_filtering.py
-drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2024-03-30 14:09:36.572219 adaptix-3.0.0b4/src/adaptix/_internal/morphing/name_layout/
--rw-rw-r--   0 pavel     (1000) pavel     (1000)        0 2024-03-17 07:48:08.000000 adaptix-3.0.0b4/src/adaptix/_internal/morphing/name_layout/__init__.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     2313 2024-03-17 07:48:08.000000 adaptix-3.0.0b4/src/adaptix/_internal/morphing/name_layout/base.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)    16012 2024-03-30 13:54:05.000000 adaptix-3.0.0b4/src/adaptix/_internal/morphing/name_layout/component.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     5803 2024-03-17 07:48:08.000000 adaptix-3.0.0b4/src/adaptix/_internal/morphing/name_layout/crown_builder.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     3654 2024-03-17 07:48:08.000000 adaptix-3.0.0b4/src/adaptix/_internal/morphing/name_layout/name_mapping.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     4223 2024-03-17 07:48:08.000000 adaptix-3.0.0b4/src/adaptix/_internal/morphing/name_layout/provider.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     2492 2024-03-30 13:54:05.000000 adaptix-3.0.0b4/src/adaptix/_internal/morphing/provider_template.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)      281 2024-03-17 07:48:08.000000 adaptix-3.0.0b4/src/adaptix/_internal/morphing/request_cls.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     2875 2024-03-17 07:48:08.000000 adaptix-3.0.0b4/src/adaptix/_internal/name_style.py
-drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2024-03-30 14:09:36.572219 adaptix-3.0.0b4/src/adaptix/_internal/provider/
--rw-rw-r--   0 pavel     (1000) pavel     (1000)        0 2024-03-17 07:48:08.000000 adaptix-3.0.0b4/src/adaptix/_internal/provider/__init__.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     6700 2024-03-30 13:54:05.000000 adaptix-3.0.0b4/src/adaptix/_internal/provider/essential.py
-drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2024-03-30 14:09:36.572219 adaptix-3.0.0b4/src/adaptix/_internal/provider/facade/
--rw-rw-r--   0 pavel     (1000) pavel     (1000)        0 2024-03-17 07:48:08.000000 adaptix-3.0.0b4/src/adaptix/_internal/provider/facade/__init__.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)      757 2024-03-17 07:48:08.000000 adaptix-3.0.0b4/src/adaptix/_internal/provider/facade/provider.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)      905 2024-03-30 13:54:05.000000 adaptix-3.0.0b4/src/adaptix/_internal/provider/fields.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)    11995 2024-03-30 13:54:05.000000 adaptix-3.0.0b4/src/adaptix/_internal/provider/loc_stack_filtering.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     1818 2024-03-30 13:54:05.000000 adaptix-3.0.0b4/src/adaptix/_internal/provider/location.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     4226 2024-03-30 13:54:05.000000 adaptix-3.0.0b4/src/adaptix/_internal/provider/overlay_schema.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     1586 2024-03-30 13:54:05.000000 adaptix-3.0.0b4/src/adaptix/_internal/provider/provider_template.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     3878 2024-03-17 07:48:08.000000 adaptix-3.0.0b4/src/adaptix/_internal/provider/provider_wrapper.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     1535 2024-03-30 13:54:05.000000 adaptix-3.0.0b4/src/adaptix/_internal/provider/request_cls.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     7878 2024-03-30 13:54:05.000000 adaptix-3.0.0b4/src/adaptix/_internal/provider/shape_provider.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     6268 2024-03-30 13:54:05.000000 adaptix-3.0.0b4/src/adaptix/_internal/provider/static_provider.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)        0 2024-03-17 07:48:08.000000 adaptix-3.0.0b4/src/adaptix/_internal/py.typed
-drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2024-03-30 14:09:36.572219 adaptix-3.0.0b4/src/adaptix/_internal/retort/
--rw-rw-r--   0 pavel     (1000) pavel     (1000)        0 2024-03-17 07:48:08.000000 adaptix-3.0.0b4/src/adaptix/_internal/retort/__init__.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     3210 2024-03-30 13:54:05.000000 adaptix-3.0.0b4/src/adaptix/_internal/retort/base_retort.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     3159 2024-03-17 07:48:08.000000 adaptix-3.0.0b4/src/adaptix/_internal/retort/mediator.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     6457 2024-03-30 13:54:05.000000 adaptix-3.0.0b4/src/adaptix/_internal/retort/operating_retort.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     5812 2024-03-30 13:54:05.000000 adaptix-3.0.0b4/src/adaptix/_internal/retort/routing.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)      723 2024-03-30 13:54:05.000000 adaptix-3.0.0b4/src/adaptix/_internal/special_cases_optimization.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     3063 2024-03-30 13:54:05.000000 adaptix-3.0.0b4/src/adaptix/_internal/struct_trail.py
-drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2024-03-30 14:09:36.576219 adaptix-3.0.0b4/src/adaptix/_internal/type_tools/
--rw-rw-r--   0 pavel     (1000) pavel     (1000)      540 2024-03-17 07:48:08.000000 adaptix-3.0.0b4/src/adaptix/_internal/type_tools/__init__.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     4786 2024-03-30 13:54:05.000000 adaptix-3.0.0b4/src/adaptix/_internal/type_tools/basic_utils.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)      994 2024-03-30 13:54:05.000000 adaptix-3.0.0b4/src/adaptix/_internal/type_tools/constants.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     3878 2024-03-17 07:48:08.000000 adaptix-3.0.0b4/src/adaptix/_internal/type_tools/generic_resolver.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     1828 2024-03-17 07:48:08.000000 adaptix-3.0.0b4/src/adaptix/_internal/type_tools/implicit_params.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     1059 2024-03-17 07:48:08.000000 adaptix-3.0.0b4/src/adaptix/_internal/type_tools/norm_utils.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)    25491 2024-03-30 13:54:05.000000 adaptix-3.0.0b4/src/adaptix/_internal/type_tools/normalize_type.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     5928 2024-03-30 13:54:05.000000 adaptix-3.0.0b4/src/adaptix/_internal/utils.py
-drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2024-03-30 14:09:36.576219 adaptix-3.0.0b4/src/adaptix/conversion/
--rw-rw-r--   0 pavel     (1000) pavel     (1000)      678 2024-03-30 13:54:05.000000 adaptix-3.0.0b4/src/adaptix/conversion/__init__.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     1564 2024-03-17 07:48:08.000000 adaptix-3.0.0b4/src/adaptix/load_error.py
-drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2024-03-30 14:09:36.576219 adaptix-3.0.0b4/src/adaptix/provider/
--rw-rw-r--   0 pavel     (1000) pavel     (1000)      472 2024-03-17 07:48:08.000000 adaptix-3.0.0b4/src/adaptix/provider/__init__.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)        0 2024-03-17 07:48:08.000000 adaptix-3.0.0b4/src/adaptix/py.typed
--rw-rw-r--   0 pavel     (1000) pavel     (1000)      232 2024-03-30 13:12:41.000000 adaptix-3.0.0b4/src/adaptix/retort.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)      386 2024-03-17 07:48:08.000000 adaptix-3.0.0b4/src/adaptix/struct_trail.py
-drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2024-03-30 14:09:36.576219 adaptix-3.0.0b4/src/adaptix.egg-info/
--rw-r--r--   0 pavel     (1000) pavel     (1000)     6548 2024-03-30 14:09:36.000000 adaptix-3.0.0b4/src/adaptix.egg-info/PKG-INFO
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     5225 2024-03-30 14:09:36.000000 adaptix-3.0.0b4/src/adaptix.egg-info/SOURCES.txt
--rw-rw-r--   0 pavel     (1000) pavel     (1000)        1 2024-03-30 14:09:36.000000 adaptix-3.0.0b4/src/adaptix.egg-info/dependency_links.txt
--rw-rw-r--   0 pavel     (1000) pavel     (1000)      238 2024-03-30 14:09:36.000000 adaptix-3.0.0b4/src/adaptix.egg-info/requires.txt
--rw-rw-r--   0 pavel     (1000) pavel     (1000)        8 2024-03-30 14:09:36.000000 adaptix-3.0.0b4/src/adaptix.egg-info/top_level.txt
-drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2024-03-30 14:09:36.576219 adaptix-3.0.0b4/tests/
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     1287 2024-03-17 07:48:08.000000 adaptix-3.0.0b4/tests/test_doc.py
+drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2024-04-20 08:07:26.543075 adaptix-3.0.0b5/
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)    11357 2021-06-13 21:15:36.000000 adaptix-3.0.0b5/LICENSE
+-rw-r--r--   0 pavel     (1000) pavel     (1000)     6741 2024-04-20 08:07:26.543075 adaptix-3.0.0b5/PKG-INFO
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     4539 2024-04-20 08:07:18.000000 adaptix-3.0.0b5/README.md
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     5162 2024-04-20 08:07:18.000000 adaptix-3.0.0b5/pyproject.toml
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)       38 2024-04-20 08:07:26.543075 adaptix-3.0.0b5/setup.cfg
+drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2024-04-20 08:07:26.527075 adaptix-3.0.0b5/src/
+drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2024-04-20 08:07:26.531075 adaptix-3.0.0b5/src/adaptix/
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     2128 2024-03-30 13:12:56.000000 adaptix-3.0.0b5/src/adaptix/__init__.py
+drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2024-04-20 08:07:26.531075 adaptix-3.0.0b5/src/adaptix/_internal/
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)        0 2024-03-17 07:48:08.000000 adaptix-3.0.0b5/src/adaptix/_internal/__init__.py
+drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2024-04-20 08:07:26.531075 adaptix-3.0.0b5/src/adaptix/_internal/code_tools/
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)        0 2024-03-17 07:48:08.000000 adaptix-3.0.0b5/src/adaptix/_internal/code_tools/__init__.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)      619 2024-03-30 13:54:05.000000 adaptix-3.0.0b5/src/adaptix/_internal/code_tools/ast_templater.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     3045 2024-03-30 13:54:05.000000 adaptix-3.0.0b5/src/adaptix/_internal/code_tools/cascade_namespace.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     2920 2024-03-30 13:54:05.000000 adaptix-3.0.0b5/src/adaptix/_internal/code_tools/code_builder.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     2634 2024-03-30 13:54:05.000000 adaptix-3.0.0b5/src/adaptix/_internal/code_tools/compiler.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)      558 2024-03-17 07:48:08.000000 adaptix-3.0.0b5/src/adaptix/_internal/code_tools/name_sanitizer.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     2718 2024-03-30 13:54:05.000000 adaptix-3.0.0b5/src/adaptix/_internal/code_tools/utils.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)      639 2024-03-30 13:54:05.000000 adaptix-3.0.0b5/src/adaptix/_internal/common.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)      322 2024-03-17 07:48:08.000000 adaptix-3.0.0b5/src/adaptix/_internal/compat.py
+drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2024-04-20 08:07:26.531075 adaptix-3.0.0b5/src/adaptix/_internal/conversion/
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)        0 2024-03-17 07:48:08.000000 adaptix-3.0.0b5/src/adaptix/_internal/conversion/__init__.py
+drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2024-04-20 08:07:26.531075 adaptix-3.0.0b5/src/adaptix/_internal/conversion/broaching/
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)        0 2024-03-17 07:48:08.000000 adaptix-3.0.0b5/src/adaptix/_internal/conversion/broaching/__init__.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     7760 2024-03-30 13:54:05.000000 adaptix-3.0.0b5/src/adaptix/_internal/conversion/broaching/code_generator.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     1187 2024-03-17 07:48:08.000000 adaptix-3.0.0b5/src/adaptix/_internal/conversion/broaching/definitions.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)    10709 2024-03-30 13:54:05.000000 adaptix-3.0.0b5/src/adaptix/_internal/conversion/coercer_provider.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     6976 2024-03-30 13:54:05.000000 adaptix-3.0.0b5/src/adaptix/_internal/conversion/converter_provider.py
+drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2024-04-20 08:07:26.531075 adaptix-3.0.0b5/src/adaptix/_internal/conversion/facade/
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)        0 2024-03-17 07:48:08.000000 adaptix-3.0.0b5/src/adaptix/_internal/conversion/facade/__init__.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)      749 2024-03-30 13:54:05.000000 adaptix-3.0.0b5/src/adaptix/_internal/conversion/facade/checker.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     2311 2024-03-17 07:48:08.000000 adaptix-3.0.0b5/src/adaptix/_internal/conversion/facade/func.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     3855 2024-03-30 13:54:05.000000 adaptix-3.0.0b5/src/adaptix/_internal/conversion/facade/provider.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     6216 2024-03-30 13:54:05.000000 adaptix-3.0.0b5/src/adaptix/_internal/conversion/facade/retort.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     2661 2024-03-30 13:54:05.000000 adaptix-3.0.0b5/src/adaptix/_internal/conversion/linking_provider.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)    11225 2024-03-30 13:54:05.000000 adaptix-3.0.0b5/src/adaptix/_internal/conversion/model_coercer_provider.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)      594 2024-03-17 07:48:08.000000 adaptix-3.0.0b5/src/adaptix/_internal/conversion/policy_provider.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     1068 2024-03-30 13:54:05.000000 adaptix-3.0.0b5/src/adaptix/_internal/conversion/provider_template.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     1928 2024-03-30 13:54:05.000000 adaptix-3.0.0b5/src/adaptix/_internal/conversion/request_cls.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     7757 2024-03-30 13:54:05.000000 adaptix-3.0.0b5/src/adaptix/_internal/datastructures.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)      108 2024-03-17 07:48:08.000000 adaptix-3.0.0b5/src/adaptix/_internal/definitions.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     5460 2024-04-20 08:07:18.000000 adaptix-3.0.0b5/src/adaptix/_internal/feature_requirement.py
+drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2024-04-20 08:07:26.531075 adaptix-3.0.0b5/src/adaptix/_internal/integrations/
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)        0 2024-04-20 08:07:18.000000 adaptix-3.0.0b5/src/adaptix/_internal/integrations/__init__.py
+drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2024-04-20 08:07:26.535075 adaptix-3.0.0b5/src/adaptix/_internal/integrations/pydantic/
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)        0 2024-04-20 08:07:18.000000 adaptix-3.0.0b5/src/adaptix/_internal/integrations/pydantic/__init__.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     6017 2024-04-20 08:07:18.000000 adaptix-3.0.0b5/src/adaptix/_internal/integrations/pydantic/native.py
+drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2024-04-20 08:07:26.535075 adaptix-3.0.0b5/src/adaptix/_internal/model_tools/
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)        0 2024-03-17 07:48:08.000000 adaptix-3.0.0b5/src/adaptix/_internal/model_tools/__init__.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)    10048 2024-04-20 08:07:18.000000 adaptix-3.0.0b5/src/adaptix/_internal/model_tools/definitions.py
+drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2024-04-20 08:07:26.535075 adaptix-3.0.0b5/src/adaptix/_internal/model_tools/introspection/
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)        0 2024-03-17 07:48:08.000000 adaptix-3.0.0b5/src/adaptix/_internal/model_tools/introspection/__init__.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     4861 2024-03-30 13:54:05.000000 adaptix-3.0.0b5/src/adaptix/_internal/model_tools/introspection/attrs.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     3484 2024-03-30 13:54:05.000000 adaptix-3.0.0b5/src/adaptix/_internal/model_tools/introspection/callable.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)      497 2024-03-30 13:54:05.000000 adaptix-3.0.0b5/src/adaptix/_internal/model_tools/introspection/class_init.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     3810 2024-04-20 08:03:28.000000 adaptix-3.0.0b5/src/adaptix/_internal/model_tools/introspection/dataclass.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     2207 2024-03-30 13:54:05.000000 adaptix-3.0.0b5/src/adaptix/_internal/model_tools/introspection/named_tuple.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     8028 2024-04-20 08:07:18.000000 adaptix-3.0.0b5/src/adaptix/_internal/model_tools/introspection/pydantic.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     7912 2024-04-20 08:07:18.000000 adaptix-3.0.0b5/src/adaptix/_internal/model_tools/introspection/sqlalchemy.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     4342 2024-03-30 13:54:05.000000 adaptix-3.0.0b5/src/adaptix/_internal/model_tools/introspection/typed_dict.py
+drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2024-04-20 08:07:26.535075 adaptix-3.0.0b5/src/adaptix/_internal/morphing/
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)        0 2024-03-17 07:48:08.000000 adaptix-3.0.0b5/src/adaptix/_internal/morphing/__init__.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)    13218 2024-04-20 08:07:18.000000 adaptix-3.0.0b5/src/adaptix/_internal/morphing/concrete_provider.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)    12270 2024-03-30 13:54:05.000000 adaptix-3.0.0b5/src/adaptix/_internal/morphing/constant_length_tuple_provider.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)    10886 2024-03-30 13:54:05.000000 adaptix-3.0.0b5/src/adaptix/_internal/morphing/dict_provider.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)    12333 2024-03-30 13:54:05.000000 adaptix-3.0.0b5/src/adaptix/_internal/morphing/enum_provider.py
+drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2024-04-20 08:07:26.535075 adaptix-3.0.0b5/src/adaptix/_internal/morphing/facade/
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)        0 2024-03-17 07:48:08.000000 adaptix-3.0.0b5/src/adaptix/_internal/morphing/facade/__init__.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)      618 2024-03-17 07:48:08.000000 adaptix-3.0.0b5/src/adaptix/_internal/morphing/facade/func.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)    16413 2024-03-30 13:54:05.000000 adaptix-3.0.0b5/src/adaptix/_internal/morphing/facade/provider.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     9701 2024-04-20 08:07:18.000000 adaptix-3.0.0b5/src/adaptix/_internal/morphing/facade/retort.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)    18431 2024-04-20 08:07:18.000000 adaptix-3.0.0b5/src/adaptix/_internal/morphing/generic_provider.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)    10078 2024-03-30 13:54:05.000000 adaptix-3.0.0b5/src/adaptix/_internal/morphing/iterable_provider.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     3869 2024-03-30 13:54:05.000000 adaptix-3.0.0b5/src/adaptix/_internal/morphing/load_error.py
+drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2024-04-20 08:07:26.535075 adaptix-3.0.0b5/src/adaptix/_internal/morphing/model/
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)        0 2024-03-17 07:48:08.000000 adaptix-3.0.0b5/src/adaptix/_internal/morphing/model/__init__.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     7579 2024-04-20 08:07:18.000000 adaptix-3.0.0b5/src/adaptix/_internal/morphing/model/basic_gen.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     4313 2024-03-17 07:48:08.000000 adaptix-3.0.0b5/src/adaptix/_internal/morphing/model/crown_definitions.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)    23272 2024-03-30 13:54:05.000000 adaptix-3.0.0b5/src/adaptix/_internal/morphing/model/dumper_gen.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     6031 2024-03-30 13:54:05.000000 adaptix-3.0.0b5/src/adaptix/_internal/morphing/model/dumper_provider.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)    28138 2024-03-30 13:54:05.000000 adaptix-3.0.0b5/src/adaptix/_internal/morphing/model/loader_gen.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     7907 2024-03-30 13:54:05.000000 adaptix-3.0.0b5/src/adaptix/_internal/morphing/model/loader_provider.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)      696 2024-03-17 07:48:08.000000 adaptix-3.0.0b5/src/adaptix/_internal/morphing/model/request_filtering.py
+drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2024-04-20 08:07:26.535075 adaptix-3.0.0b5/src/adaptix/_internal/morphing/name_layout/
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)        0 2024-03-17 07:48:08.000000 adaptix-3.0.0b5/src/adaptix/_internal/morphing/name_layout/__init__.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     2313 2024-03-17 07:48:08.000000 adaptix-3.0.0b5/src/adaptix/_internal/morphing/name_layout/base.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)    16012 2024-03-30 13:54:05.000000 adaptix-3.0.0b5/src/adaptix/_internal/morphing/name_layout/component.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     5803 2024-03-17 07:48:08.000000 adaptix-3.0.0b5/src/adaptix/_internal/morphing/name_layout/crown_builder.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     4034 2024-04-20 08:07:18.000000 adaptix-3.0.0b5/src/adaptix/_internal/morphing/name_layout/name_mapping.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     4223 2024-03-17 07:48:08.000000 adaptix-3.0.0b5/src/adaptix/_internal/morphing/name_layout/provider.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     2492 2024-03-30 13:54:05.000000 adaptix-3.0.0b5/src/adaptix/_internal/morphing/provider_template.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)      281 2024-03-17 07:48:08.000000 adaptix-3.0.0b5/src/adaptix/_internal/morphing/request_cls.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     2875 2024-03-17 07:48:08.000000 adaptix-3.0.0b5/src/adaptix/_internal/name_style.py
+drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2024-04-20 08:07:26.539075 adaptix-3.0.0b5/src/adaptix/_internal/provider/
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)        0 2024-03-17 07:48:08.000000 adaptix-3.0.0b5/src/adaptix/_internal/provider/__init__.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     6700 2024-03-30 13:54:05.000000 adaptix-3.0.0b5/src/adaptix/_internal/provider/essential.py
+drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2024-04-20 08:07:26.539075 adaptix-3.0.0b5/src/adaptix/_internal/provider/facade/
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)        0 2024-03-17 07:48:08.000000 adaptix-3.0.0b5/src/adaptix/_internal/provider/facade/__init__.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)      757 2024-03-17 07:48:08.000000 adaptix-3.0.0b5/src/adaptix/_internal/provider/facade/provider.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)      905 2024-03-30 13:54:05.000000 adaptix-3.0.0b5/src/adaptix/_internal/provider/fields.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)    12210 2024-04-20 08:07:18.000000 adaptix-3.0.0b5/src/adaptix/_internal/provider/loc_stack_filtering.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     1818 2024-03-30 13:54:05.000000 adaptix-3.0.0b5/src/adaptix/_internal/provider/location.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     4226 2024-03-30 13:54:05.000000 adaptix-3.0.0b5/src/adaptix/_internal/provider/overlay_schema.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     1586 2024-03-30 13:54:05.000000 adaptix-3.0.0b5/src/adaptix/_internal/provider/provider_template.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     3878 2024-03-17 07:48:08.000000 adaptix-3.0.0b5/src/adaptix/_internal/provider/provider_wrapper.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     1535 2024-03-30 13:54:05.000000 adaptix-3.0.0b5/src/adaptix/_internal/provider/request_cls.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     7985 2024-04-20 08:07:18.000000 adaptix-3.0.0b5/src/adaptix/_internal/provider/shape_provider.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     6268 2024-03-30 13:54:05.000000 adaptix-3.0.0b5/src/adaptix/_internal/provider/static_provider.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)        0 2024-03-17 07:48:08.000000 adaptix-3.0.0b5/src/adaptix/_internal/py.typed
+drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2024-04-20 08:07:26.539075 adaptix-3.0.0b5/src/adaptix/_internal/retort/
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)        0 2024-03-17 07:48:08.000000 adaptix-3.0.0b5/src/adaptix/_internal/retort/__init__.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     3210 2024-03-30 13:54:05.000000 adaptix-3.0.0b5/src/adaptix/_internal/retort/base_retort.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     3159 2024-03-17 07:48:08.000000 adaptix-3.0.0b5/src/adaptix/_internal/retort/mediator.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     6653 2024-04-20 08:07:18.000000 adaptix-3.0.0b5/src/adaptix/_internal/retort/operating_retort.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     5812 2024-03-30 13:54:05.000000 adaptix-3.0.0b5/src/adaptix/_internal/retort/routing.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)      723 2024-03-30 13:54:05.000000 adaptix-3.0.0b5/src/adaptix/_internal/special_cases_optimization.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     3063 2024-03-30 13:54:05.000000 adaptix-3.0.0b5/src/adaptix/_internal/struct_trail.py
+drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2024-04-20 08:07:26.539075 adaptix-3.0.0b5/src/adaptix/_internal/type_tools/
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)      609 2024-04-20 08:07:18.000000 adaptix-3.0.0b5/src/adaptix/_internal/type_tools/__init__.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     4141 2024-04-20 08:07:18.000000 adaptix-3.0.0b5/src/adaptix/_internal/type_tools/basic_utils.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)      994 2024-03-30 13:54:05.000000 adaptix-3.0.0b5/src/adaptix/_internal/type_tools/constants.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     1530 2024-04-20 08:07:18.000000 adaptix-3.0.0b5/src/adaptix/_internal/type_tools/fundamentals.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     3907 2024-04-20 08:07:18.000000 adaptix-3.0.0b5/src/adaptix/_internal/type_tools/generic_resolver.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     1828 2024-03-17 07:48:08.000000 adaptix-3.0.0b5/src/adaptix/_internal/type_tools/implicit_params.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     1059 2024-03-17 07:48:08.000000 adaptix-3.0.0b5/src/adaptix/_internal/type_tools/norm_utils.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)    25528 2024-04-20 08:07:18.000000 adaptix-3.0.0b5/src/adaptix/_internal/type_tools/normalize_type.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     5928 2024-03-30 13:54:05.000000 adaptix-3.0.0b5/src/adaptix/_internal/utils.py
+drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2024-04-20 08:07:26.539075 adaptix-3.0.0b5/src/adaptix/conversion/
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)      678 2024-03-30 13:54:05.000000 adaptix-3.0.0b5/src/adaptix/conversion/__init__.py
+drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2024-04-20 08:07:26.539075 adaptix-3.0.0b5/src/adaptix/integrations/
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)        0 2024-04-20 08:07:18.000000 adaptix-3.0.0b5/src/adaptix/integrations/__init__.py
+drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2024-04-20 08:07:26.539075 adaptix-3.0.0b5/src/adaptix/integrations/pydantic/
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)      113 2024-04-20 08:07:18.000000 adaptix-3.0.0b5/src/adaptix/integrations/pydantic/__init__.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     1564 2024-03-17 07:48:08.000000 adaptix-3.0.0b5/src/adaptix/load_error.py
+drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2024-04-20 08:07:26.539075 adaptix-3.0.0b5/src/adaptix/provider/
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)      472 2024-03-17 07:48:08.000000 adaptix-3.0.0b5/src/adaptix/provider/__init__.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)        0 2024-03-17 07:48:08.000000 adaptix-3.0.0b5/src/adaptix/py.typed
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)      232 2024-03-30 13:12:41.000000 adaptix-3.0.0b5/src/adaptix/retort.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)      386 2024-03-17 07:48:08.000000 adaptix-3.0.0b5/src/adaptix/struct_trail.py
+drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2024-04-20 08:07:26.539075 adaptix-3.0.0b5/src/adaptix.egg-info/
+-rw-r--r--   0 pavel     (1000) pavel     (1000)     6741 2024-04-20 08:07:26.000000 adaptix-3.0.0b5/src/adaptix.egg-info/PKG-INFO
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     5593 2024-04-20 08:07:26.000000 adaptix-3.0.0b5/src/adaptix.egg-info/SOURCES.txt
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)        1 2024-04-20 08:07:26.000000 adaptix-3.0.0b5/src/adaptix.egg-info/dependency_links.txt
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)      309 2024-04-20 08:07:26.000000 adaptix-3.0.0b5/src/adaptix.egg-info/requires.txt
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)        8 2024-04-20 08:07:26.000000 adaptix-3.0.0b5/src/adaptix.egg-info/top_level.txt
+drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2024-04-20 08:07:26.539075 adaptix-3.0.0b5/tests/
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     1838 2024-04-20 08:07:18.000000 adaptix-3.0.0b5/tests/test_doc.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)      237 2024-04-20 08:07:18.000000 adaptix-3.0.0b5/tests/test_meta.py
```

### Comparing `adaptix-3.0.0b4/LICENSE` & `adaptix-3.0.0b5/LICENSE`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0b4/PKG-INFO` & `adaptix-3.0.0b5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adaptix
-Version: 3.0.0b4
+Version: 3.0.0b5
 Summary: An extremely flexible and configurable data model conversion library
 Author-email: "A. Tikhonov" <17@itishka.org>
 Project-URL: Homepage, https://github.com/reagento/adaptix
 Project-URL: Bug Tracker, https://github.com/reagento/adaptix/issues
 Project-URL: Documentation, https://adaptix.readthedocs.io/en/latest/
 Project-URL: Changelog, https://adaptix.readthedocs.io/en/latest/reference/changelog.html
 Project-URL: Source, https://github.com/reagento/adaptix/
@@ -35,19 +35,23 @@
 Requires-Dist: attrs>=21.3.0; extra == "attrs"
 Provides-Extra: attrs-strict
 Requires-Dist: attrs<=23.2.0,>=21.3.0; extra == "attrs-strict"
 Provides-Extra: sqlalchemy
 Requires-Dist: sqlalchemy>=2.0.0; extra == "sqlalchemy"
 Provides-Extra: sqlalchemy-strict
 Requires-Dist: sqlalchemy<=2.0.29,>=2.0.0; extra == "sqlalchemy-strict"
+Provides-Extra: pydantic
+Requires-Dist: pydantic>=2.0.0; extra == "pydantic"
+Provides-Extra: pydantic-strict
+Requires-Dist: pydantic<=2.7.0,>=2.0.0; extra == "pydantic-strict"
 
 <div align="center">
   <picture>
-    <source media="(prefers-color-scheme: dark)" srcset="https://github.com/reagento/adaptix/blob/v3.0.0b4/docs/logo/adaptix-with-title-dark.png?raw=true">
-    <source media="(prefers-color-scheme: light)" srcset="https://github.com/reagento/adaptix/blob/v3.0.0b4/docs/logo/adaptix-with-title-light.png?raw=true">
+    <source media="(prefers-color-scheme: dark)" srcset="https://github.com/reagento/adaptix/blob/v3.0.0b5/docs/logo/adaptix-with-title-dark.png?raw=true">
+    <source media="(prefers-color-scheme: light)" srcset="https://github.com/reagento/adaptix/blob/v3.0.0b5/docs/logo/adaptix-with-title-light.png?raw=true">
     <img alt="adaptix logo" src="https://raw.githubusercontent.com/reagento/adaptix/v3.0.0b2/docs/logo/adaptix-with-title-light.png?raw=true">
   </picture>
 
   <hr>
 
   [![PyPI version](https://img.shields.io/pypi/v/adaptix.svg?color=blue)](https://pypi.org/project/adaptix/)
   [![downloads](https://img.shields.io/pypi/dm/adaptix.svg)](https://pypistats.org/packages/adaptix)
@@ -63,30 +67,29 @@
 
 📚 [Documentation](https://adaptix.readthedocs.io/)
 
 ## TL;DR
 
 Install
 ```bash
-pip install adaptix==3.0.0b4
+pip install adaptix==3.0.0b5
 ```
 
 Use for model loading and dumping.
 
 ```python
 from dataclasses import dataclass
 
 from adaptix import Retort
 
 
 @dataclass
 class Book:
     title: str
     price: int
-    author: str = "Unknown author"
 
 
 data = {
     "title": "Fahrenheit 451",
     "price": 100,
 }
 
@@ -153,15 +156,15 @@
   that allow preserving [SRP](https://blog.cleancoder.com/uncle-bob/2014/05/08/SingleReponsibilityPrinciple.html)
   and have different representations for one model.
 * Speed. It is one of the fastest data parsing and serialization libraries.
 * There is no forced model representation, adaptix can adjust to your needs.
 * Support [dozens](https://adaptix.readthedocs.io/en/latest/loading-and-dumping/specific-types-behavior.html) of types,
   including different model kinds:
   ``@dataclass``, ``TypedDict``, ``NamedTuple``,
-  [``attrs``](https://www.attrs.org/en/stable/) and [``sqlalchemy``](https://docs.sqlalchemy.org/en/20/)
+  [``attrs``](https://www.attrs.org/en/stable/), [``sqlalchemy``](https://docs.sqlalchemy.org/en/20/) and [``pydantic``](https://docs.pydantic.dev/latest/).
 * Working with self-referenced data types (such as linked lists or trees).
 * Saving [path](https://adaptix.readthedocs.io/en/latest/loading-and-dumping/tutorial.html#error-handling)
   where an exception is raised (including unexpected errors).
 * Machine-readable [errors](https://adaptix.readthedocs.io/en/latest/loading-and-dumping/tutorial.html#error-handling)
   that could be dumped.
 * Support for user-defined generic models.
 * Automatic name style conversion (e.g. `snake_case` to `camelCase`).
```

### Comparing `adaptix-3.0.0b4/README.md` & `adaptix-3.0.0b5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 <div align="center">
   <picture>
-    <source media="(prefers-color-scheme: dark)" srcset="https://github.com/reagento/adaptix/blob/v3.0.0b4/docs/logo/adaptix-with-title-dark.png?raw=true">
-    <source media="(prefers-color-scheme: light)" srcset="https://github.com/reagento/adaptix/blob/v3.0.0b4/docs/logo/adaptix-with-title-light.png?raw=true">
+    <source media="(prefers-color-scheme: dark)" srcset="https://github.com/reagento/adaptix/blob/v3.0.0b5/docs/logo/adaptix-with-title-dark.png?raw=true">
+    <source media="(prefers-color-scheme: light)" srcset="https://github.com/reagento/adaptix/blob/v3.0.0b5/docs/logo/adaptix-with-title-light.png?raw=true">
     <img alt="adaptix logo" src="https://raw.githubusercontent.com/reagento/adaptix/v3.0.0b2/docs/logo/adaptix-with-title-light.png?raw=true">
   </picture>
 
   <hr>
 
   [![PyPI version](https://img.shields.io/pypi/v/adaptix.svg?color=blue)](https://pypi.org/project/adaptix/)
   [![downloads](https://img.shields.io/pypi/dm/adaptix.svg)](https://pypistats.org/packages/adaptix)
@@ -21,30 +21,29 @@
 
 📚 [Documentation](https://adaptix.readthedocs.io/)
 
 ## TL;DR
 
 Install
 ```bash
-pip install adaptix==3.0.0b4
+pip install adaptix==3.0.0b5
 ```
 
 Use for model loading and dumping.
 
 ```python
 from dataclasses import dataclass
 
 from adaptix import Retort
 
 
 @dataclass
 class Book:
     title: str
     price: int
-    author: str = "Unknown author"
 
 
 data = {
     "title": "Fahrenheit 451",
     "price": 100,
 }
 
@@ -111,15 +110,15 @@
   that allow preserving [SRP](https://blog.cleancoder.com/uncle-bob/2014/05/08/SingleReponsibilityPrinciple.html)
   and have different representations for one model.
 * Speed. It is one of the fastest data parsing and serialization libraries.
 * There is no forced model representation, adaptix can adjust to your needs.
 * Support [dozens](https://adaptix.readthedocs.io/en/latest/loading-and-dumping/specific-types-behavior.html) of types,
   including different model kinds:
   ``@dataclass``, ``TypedDict``, ``NamedTuple``,
-  [``attrs``](https://www.attrs.org/en/stable/) and [``sqlalchemy``](https://docs.sqlalchemy.org/en/20/)
+  [``attrs``](https://www.attrs.org/en/stable/), [``sqlalchemy``](https://docs.sqlalchemy.org/en/20/) and [``pydantic``](https://docs.pydantic.dev/latest/).
 * Working with self-referenced data types (such as linked lists or trees).
 * Saving [path](https://adaptix.readthedocs.io/en/latest/loading-and-dumping/tutorial.html#error-handling)
   where an exception is raised (including unexpected errors).
 * Machine-readable [errors](https://adaptix.readthedocs.io/en/latest/loading-and-dumping/tutorial.html#error-handling)
   that could be dumped.
 * Support for user-defined generic models.
 * Automatic name style conversion (e.g. `snake_case` to `camelCase`).
```

### Comparing `adaptix-3.0.0b4/pyproject.toml` & `adaptix-3.0.0b5/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ['setuptools==69.1.0']
 build-backend = 'setuptools.build_meta'
 
 [project]
 name = 'adaptix'
-version = '3.0.0b4'
+version = '3.0.0b5'
 description = 'An extremely flexible and configurable data model conversion library'
 readme = 'README.md'
 requires-python = '>=3.8'
 dependencies = [
     'exceptiongroup>=1.1.3; python_version<"3.11"',
     'astunparse>=1.6.3; python_version<="3.8"',
 ]
@@ -34,14 +34,16 @@
 ]
 
 [project.optional-dependencies]
 attrs = ['attrs >= 21.3.0']
 attrs-strict = ['attrs >= 21.3.0, <= 23.2.0']
 sqlalchemy = ['sqlalchemy >= 2.0.0']
 sqlalchemy-strict = ['sqlalchemy >= 2.0.0, <= 2.0.29']
+pydantic = ['pydantic >= 2.0.0']
+pydantic-strict = ['pydantic >= 2.0.0, <= 2.7.0']
 
 [project.urls]
 'Homepage' = 'https://github.com/reagento/adaptix'
 'Bug Tracker' = 'https://github.com/reagento/adaptix/issues'
 'Documentation' = 'https://adaptix.readthedocs.io/en/latest/'
 'Changelog' = 'https://adaptix.readthedocs.io/en/latest/reference/changelog.html'
 'Source' = 'https://github.com/reagento/adaptix/'
@@ -59,15 +61,21 @@
 
 #   ┌             ┐
 #   │   TESTING   │
 #   └             ┘
 
 [tool.pytest.ini_options]
 python_classes = 'WeDoNotUseClassTestCase'
-python_files = ['test_*.py', '*_test.py', 'bench_[!nexus]*.py', 'tests_helpers.py', 'local_helpers.py']
+python_files = [
+  'test_*.py',
+  '*_test.py',
+  'bench_[!nexus]*.py',
+  'tests/tests_helpers/tests_helpers/*.py',
+  'local_helpers.py',
+]
 testpaths = ['tests', 'examples']
 filterwarnings = ['ignore::adaptix.TypedDictAt38Warning']
 
 [tool.coverage.run]
 branch = true
 relative_files = true
 include = ["src/**"]
@@ -185,15 +193,15 @@
 #   └             ┘
 
 
 [tool.towncrier]
 package = 'adaptix'
 filename = 'docs/changelog/changelog_body.rst'
 template = 'docs/changelog/template.rst.jinja2'
-issue_format = '`#{issue} <https://github.com/reagento/adaptix/issues/{issue}>`_'
+issue_format = '`#{issue} <https://github.com/reagento/adaptix/issues/{issue}>`__'
 directory = 'docs/changelog/fragments'
 
 type = [
   { name = "Features",         directory = "feature",     showcontent = true },
   { name = "Breaking Changes", directory = "breaking",    showcontent = true },
   { name = "Deprecations",     directory = "deprecation", showcontent = true },
   { name = "Bug Fixes",        directory = "bugfix",      showcontent = true },
```

### Comparing `adaptix-3.0.0b4/src/adaptix/__init__.py` & `adaptix-3.0.0b5/src/adaptix/__init__.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0b4/src/adaptix/_internal/code_tools/ast_templater.py` & `adaptix-3.0.0b5/src/adaptix/_internal/code_tools/ast_templater.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0b4/src/adaptix/_internal/code_tools/cascade_namespace.py` & `adaptix-3.0.0b5/src/adaptix/_internal/code_tools/cascade_namespace.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0b4/src/adaptix/_internal/code_tools/code_builder.py` & `adaptix-3.0.0b5/src/adaptix/_internal/code_tools/code_builder.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0b4/src/adaptix/_internal/code_tools/compiler.py` & `adaptix-3.0.0b5/src/adaptix/_internal/code_tools/compiler.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0b4/src/adaptix/_internal/code_tools/name_sanitizer.py` & `adaptix-3.0.0b5/src/adaptix/_internal/code_tools/name_sanitizer.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0b4/src/adaptix/_internal/code_tools/utils.py` & `adaptix-3.0.0b5/src/adaptix/_internal/code_tools/utils.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0b4/src/adaptix/_internal/common.py` & `adaptix-3.0.0b5/src/adaptix/_internal/common.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0b4/src/adaptix/_internal/conversion/broaching/code_generator.py` & `adaptix-3.0.0b5/src/adaptix/_internal/conversion/broaching/code_generator.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0b4/src/adaptix/_internal/conversion/broaching/definitions.py` & `adaptix-3.0.0b5/src/adaptix/_internal/conversion/broaching/definitions.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0b4/src/adaptix/_internal/conversion/coercer_provider.py` & `adaptix-3.0.0b5/src/adaptix/_internal/conversion/coercer_provider.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0b4/src/adaptix/_internal/conversion/converter_provider.py` & `adaptix-3.0.0b5/src/adaptix/_internal/conversion/converter_provider.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0b4/src/adaptix/_internal/conversion/facade/checker.py` & `adaptix-3.0.0b5/src/adaptix/_internal/conversion/facade/checker.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0b4/src/adaptix/_internal/conversion/facade/func.py` & `adaptix-3.0.0b5/src/adaptix/_internal/conversion/facade/func.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0b4/src/adaptix/_internal/conversion/facade/provider.py` & `adaptix-3.0.0b5/src/adaptix/_internal/conversion/facade/provider.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0b4/src/adaptix/_internal/conversion/facade/retort.py` & `adaptix-3.0.0b5/src/adaptix/_internal/conversion/facade/retort.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0b4/src/adaptix/_internal/conversion/linking_provider.py` & `adaptix-3.0.0b5/src/adaptix/_internal/conversion/linking_provider.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0b4/src/adaptix/_internal/conversion/model_coercer_provider.py` & `adaptix-3.0.0b5/src/adaptix/_internal/conversion/model_coercer_provider.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0b4/src/adaptix/_internal/conversion/policy_provider.py` & `adaptix-3.0.0b5/src/adaptix/_internal/conversion/policy_provider.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0b4/src/adaptix/_internal/conversion/provider_template.py` & `adaptix-3.0.0b5/src/adaptix/_internal/conversion/provider_template.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0b4/src/adaptix/_internal/conversion/request_cls.py` & `adaptix-3.0.0b5/src/adaptix/_internal/conversion/request_cls.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0b4/src/adaptix/_internal/datastructures.py` & `adaptix-3.0.0b5/src/adaptix/_internal/datastructures.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0b4/src/adaptix/_internal/feature_requirement.py` & `adaptix-3.0.0b5/src/adaptix/_internal/feature_requirement.py`

 * *Files 4% similar despite different names*

```diff
@@ -170,9 +170,12 @@
 
 HAS_SUPPORTED_ATTRS_PKG = DistributionVersionRequirement("attrs", "21.3.0")
 HAS_ATTRS_PKG = DistributionRequirement("attrs")
 
 HAS_SUPPORTED_SQLALCHEMY_PKG = DistributionVersionRequirement("sqlalchemy", "2.0.0")
 HAS_SQLALCHEMY_PKG = DistributionRequirement("sqlalchemy")
 
+HAS_SUPPORTED_PYDANTIC_PKG = DistributionVersionRequirement("pydantic", "2.0.0")
+HAS_PYDANTIC_PKG = DistributionRequirement("pydantic")
+
 IS_CPYTHON = PythonImplementationRequirement("cpython")
 IS_PYPY = PythonImplementationRequirement("pypy")
```

### Comparing `adaptix-3.0.0b4/src/adaptix/_internal/model_tools/definitions.py` & `adaptix-3.0.0b5/src/adaptix/_internal/model_tools/definitions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from abc import ABC, abstractmethod
 from dataclasses import dataclass, field
 from enum import Enum
-from keyword import iskeyword
 from typing import Any, Callable, FrozenSet, Generic, Hashable, Mapping, Optional, TypeVar, Union
 
 from ..common import Catchable, TypeHint, VarTuple
 from ..feature_requirement import DistributionRequirement, DistributionVersionRequirement
 from ..struct_trail import Attr, TrailElement
 from ..utils import SingletonMeta, pairs
 
@@ -143,15 +142,15 @@
         key=key,
         access_error=access_error,
         path_element=key,
     )
 
 
 def is_valid_field_id(value: str) -> bool:
-    return value.isidentifier() or iskeyword(value)
+    return value.isidentifier()
 
 
 @dataclass(frozen=True)
 class BaseField:
     id: str
     type: TypeHint
     default: Default
```

### Comparing `adaptix-3.0.0b4/src/adaptix/_internal/model_tools/introspection/attrs.py` & `adaptix-3.0.0b5/src/adaptix/_internal/model_tools/introspection/attrs.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0b4/src/adaptix/_internal/model_tools/introspection/callable.py` & `adaptix-3.0.0b5/src/adaptix/_internal/model_tools/introspection/callable.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0b4/src/adaptix/_internal/model_tools/introspection/dataclass.py` & `adaptix-3.0.0b5/src/adaptix/_internal/model_tools/introspection/dataclass.py`

 * *Files 5% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     if field.default is not DC_MISSING:
         return DefaultValue(field.default)
     if field.default_factory is not DC_MISSING:
         return DefaultFactory(field.default_factory)
     return NoDefault()
 
 
-def _create_inp_field_from_dc_fields(dc_field: DCField, type_hints):
+def _create_inp_field_from_dc_field(dc_field: DCField, type_hints):
     default = _get_default(dc_field)
     return InputField(
         type=type_hints[dc_field.name],
         id=dc_field.name,
         default=default,
         is_required=default == NoDefault(),
         metadata=dc_field.metadata,
@@ -79,15 +79,15 @@
     )[1:]
     type_hints = get_all_type_hints(tp)
 
     return Shape(
         input=InputShape(
             constructor=tp,
             fields=tuple(
-                _create_inp_field_from_dc_fields(dc_field, type_hints)
+                _create_inp_field_from_dc_field(dc_field, type_hints)
                 for dc_field in name_to_dc_field.values()
                 if dc_field.init and not is_class_var(normalize_type(type_hints[dc_field.name]))
             ),
             params=tuple(
                 Param(
                     field_id=field_id,
                     name=field_id,
```

### Comparing `adaptix-3.0.0b4/src/adaptix/_internal/model_tools/introspection/named_tuple.py` & `adaptix-3.0.0b5/src/adaptix/_internal/model_tools/introspection/named_tuple.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0b4/src/adaptix/_internal/model_tools/introspection/sqlalchemy.py` & `adaptix-3.0.0b5/src/adaptix/_internal/model_tools/introspection/sqlalchemy.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import inspect
-from typing import Any, Generic, List, Mapping, Optional, TypeVar, get_args, get_origin
+from typing import Any, Generic, List, Mapping, Optional, TypeVar
 
 from ...common import TypeHint
 
 try:
     import sqlalchemy
     from sqlalchemy import Column, ColumnCollection
     from sqlalchemy.exc import NoInspectionAvailable
@@ -16,15 +16,15 @@
         Table,
     )
     from sqlalchemy.util import ReadOnlyProperties
 except ImportError:
     pass
 
 from ...feature_requirement import HAS_SQLALCHEMY_PKG, HAS_SUPPORTED_SQLALCHEMY_PKG
-from ...type_tools import get_all_type_hints
+from ...type_tools import get_all_type_hints, get_generic_args, strip_alias
 from ..definitions import (
     ClarifiedIntrospectionError,
     DefaultFactory,
     DefaultValue,
     FullShape,
     InputField,
     InputShape,
@@ -63,16 +63,16 @@
         return True
 
     parameters = inspect.signature(wrapped_callable).parameters
     return len(parameters) > 0
 
 
 def _unwrap_mapped_annotation(type_hint: TypeHint) -> TypeHint:
-    if get_origin(type_hint) == Mapped:
-        return get_args(type_hint)[0]
+    if strip_alias(type_hint) == Mapped:
+        return get_generic_args(type_hint)[0]
     return type_hint
 
 
 def _get_type_for_column(column: "ColumnElement", type_hints: Mapping[str, TypeHint]):
     try:
         return _unwrap_mapped_annotation(type_hints[column.name])
     except KeyError:
```

### Comparing `adaptix-3.0.0b4/src/adaptix/_internal/model_tools/introspection/typed_dict.py` & `adaptix-3.0.0b5/src/adaptix/_internal/model_tools/introspection/typed_dict.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0b4/src/adaptix/_internal/morphing/concrete_provider.py` & `adaptix-3.0.0b5/src/adaptix/_internal/morphing/concrete_provider.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import re
 import typing
 from binascii import a2b_base64, b2a_base64
 from dataclasses import dataclass, replace
 from datetime import date, datetime, time, timedelta
 from decimal import Decimal, InvalidOperation
 from fractions import Fraction
+from io import BytesIO
 from typing import Generic, Type, TypeVar, Union
 
 from ..common import Dumper, Loader
 from ..feature_requirement import HAS_PY_311, HAS_SELF_TYPE
 from ..provider.essential import CannotProvide, Mediator
 from ..provider.loc_stack_filtering import P, create_loc_stack_checker
 from ..provider.provider_template import for_predicate
@@ -134,14 +135,43 @@
                 return a2b_base64(encoded)
             except binascii.Error as e:
                 raise ValueLoadError(str(e), data)
 
         return bytes_base64_loader
 
 
+@for_predicate(BytesIO)
+class BytesIOBase64Provider(BytesBase64Provider):
+    def _provide_loader(self, mediator: Mediator, request: LoaderRequest) -> Loader:
+        bytes_base64_loader = super()._provide_loader(mediator, request)
+
+        def bytes_io_base64_loader(data):
+            return BytesIO(bytes_base64_loader(data))
+
+        return bytes_io_base64_loader
+
+    def _provide_dumper(self, mediator: Mediator, request: DumperRequest) -> Dumper:
+        def bytes_io_base64_dumper(data: BytesIO):
+            return b2a_base64(data.getvalue(), newline=False).decode("ascii")
+
+        return bytes_io_base64_dumper
+
+
+@for_predicate(typing.IO[bytes])
+class IOBytesBase64Provider(BytesIOBase64Provider):
+    def _provide_dumper(self, mediator: Mediator, request: DumperRequest) -> Dumper:
+        def io_bytes_base64_dumper(data: typing.IO[bytes]):
+            if data.seekable():
+                data.seek(0)
+
+            return b2a_base64(data.read(), newline=False).decode("ascii")
+
+        return io_bytes_base64_dumper
+
+
 @for_predicate(bytearray)
 class BytearrayBase64Provider(LoaderProvider, Base64DumperMixin):
     _BYTES_PROVIDER = BytesBase64Provider()
 
     def _provide_loader(self, mediator: Mediator, request: LoaderRequest) -> Loader:
         bytes_loader = self._BYTES_PROVIDER.apply_provider(
             mediator,
```

### Comparing `adaptix-3.0.0b4/src/adaptix/_internal/morphing/constant_length_tuple_provider.py` & `adaptix-3.0.0b5/src/adaptix/_internal/morphing/constant_length_tuple_provider.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0b4/src/adaptix/_internal/morphing/dict_provider.py` & `adaptix-3.0.0b5/src/adaptix/_internal/morphing/dict_provider.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0b4/src/adaptix/_internal/morphing/enum_provider.py` & `adaptix-3.0.0b5/src/adaptix/_internal/morphing/enum_provider.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0b4/src/adaptix/_internal/morphing/facade/func.py` & `adaptix-3.0.0b5/src/adaptix/_internal/morphing/facade/func.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0b4/src/adaptix/_internal/morphing/facade/provider.py` & `adaptix-3.0.0b5/src/adaptix/_internal/morphing/facade/provider.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0b4/src/adaptix/_internal/morphing/facade/retort.py` & `adaptix-3.0.0b5/src/adaptix/_internal/morphing/facade/retort.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,14 +24,16 @@
     DECIMAL_LOADER_PROVIDER,
     FLOAT_LOADER_PROVIDER,
     FRACTION_LOADER_PROVIDER,
     INT_LOADER_PROVIDER,
     STR_LOADER_PROVIDER,
     BytearrayBase64Provider,
     BytesBase64Provider,
+    BytesIOBase64Provider,
+    IOBytesBase64Provider,
     IsoFormatProvider,
     LiteralStringProvider,
     NoneProvider,
     RegexPatternProvider,
     SecondsTimedeltaProvider,
     SelfTypeProvider,
 )
@@ -46,14 +48,15 @@
     UnionProvider,
 )
 from ..iterable_provider import IterableProvider
 from ..model.crown_definitions import ExtraSkip
 from ..model.dumper_provider import ModelDumperProvider
 from ..model.loader_provider import ModelLoaderProvider
 from ..name_layout.component import BuiltinExtraMoveAndPoliciesMaker, BuiltinSievesMaker, BuiltinStructureMaker
+from ..name_layout.name_mapping import SkipPrivateFieldsNameMappingProvider
 from ..name_layout.provider import BuiltinNameLayoutProvider
 from ..provider_template import ABCProxy
 from ..request_cls import DumperRequest, LoaderRequest
 from .provider import as_is_dumper, as_is_loader, dumper, enum_by_exact_value, flag_by_exact_value, loader, name_mapping
 
 
 class FilledRetort(OperatingRetort, ABC):
@@ -93,14 +96,16 @@
         FRACTION_LOADER_PROVIDER,
         dumper(Fraction, Fraction.__str__),
 
         COMPLEX_LOADER_PROVIDER,
         dumper(complex, complex.__str__),
 
         BytesBase64Provider(),
+        BytesIOBase64Provider(),
+        IOBytesBase64Provider(),
         BytearrayBase64Provider(),
 
         *chain.from_iterable(
             (
                 loader(tp, tp),
                 dumper(tp, tp.__str__),  # type: ignore[arg-type]
             )
@@ -138,15 +143,17 @@
         ABCProxy(MutableMapping, dict),
         ABCProxy(ByteString, bytes),
 
         name_mapping(
             chain=None,
             skip=(),
             only=P.ANY,
-            map={},
+            map=[
+                SkipPrivateFieldsNameMappingProvider(),
+            ],
             trim_trailing_underscore=True,
             name_style=None,
             as_list=False,
             omit_default=False,
             extra_in=ExtraSkip(),
             extra_out=ExtraSkip(),
         ),
```

### Comparing `adaptix-3.0.0b4/src/adaptix/_internal/morphing/generic_provider.py` & `adaptix-3.0.0b5/src/adaptix/_internal/morphing/generic_provider.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import collections.abc
 from dataclasses import dataclass, replace
 from enum import Enum
 from os import PathLike
 from pathlib import Path
-from typing import Any, Collection, Dict, Iterable, Literal, Sequence, Set, Type, Union
+from typing import Any, Collection, Dict, Iterable, Literal, Optional, Sequence, Set, Type, Union
 
 from ..common import Dumper, Loader
 from ..compat import CompatExceptionGroup
 from ..datastructures import ClassDispatcher
 from ..definitions import DebugTrail
 from ..feature_requirement import HAS_PY_39
 from ..provider.essential import CannotProvide, Mediator
@@ -378,18 +378,23 @@
                 ),
                 lambda x: "Cannot create dumper for union. Dumpers for some union cases cannot be created",
             )
             if not_none_dumper == as_is_stub:
                 return as_is_stub
             return self._get_single_optional_dumper(not_none_dumper)
 
-        non_class_origins = [case.source for case in norm.args if not self._is_class_origin(case.origin)]
-        if non_class_origins:
+        forbidden_origins = [
+            case.source
+            for case in norm.args
+            if not self._is_class_origin(case.origin) and case.origin != Literal
+        ]
+
+        if forbidden_origins:
             raise CannotProvide(
-                f"All cases of union must be class, but found {non_class_origins}",
+                f"All cases of union must be class or Literal, but found {forbidden_origins}",
                 is_terminal=True,
                 is_demonstrative=True,
             )
 
         dumpers = mediator.mandatory_provide_by_iterable(
             [
                 DumperRequest(
@@ -406,22 +411,59 @@
         )
         if all(dumper == as_is_stub for dumper in dumpers):
             return as_is_stub
 
         dumper_type_dispatcher = ClassDispatcher(
             {type(None) if case.origin is None else case.origin: dumper for case, dumper in zip(norm.args, dumpers)},
         )
-        return self._get_dumper(dumper_type_dispatcher)
 
-    def _get_dumper(self, dumper_type_dispatcher: ClassDispatcher[Any, Dumper]) -> Dumper:
+        literal_dumper = self._get_dumper_for_literal(norm, dumpers, dumper_type_dispatcher)
+
+        if literal_dumper:
+            return literal_dumper
+
+        return self._produce_dumper(dumper_type_dispatcher)
+
+    def _produce_dumper(self, dumper_type_dispatcher: ClassDispatcher[Any, Dumper]) -> Dumper:
         def union_dumper(data):
             return dumper_type_dispatcher.dispatch(type(data))(data)
 
         return union_dumper
 
+    def _produce_dumper_for_literal(
+        self,
+        dumper_type_dispatcher: ClassDispatcher[Any, Dumper],
+        literal_dumper: Dumper,
+        literal_cases: Sequence[Any],
+    ) -> Dumper:
+        def union_dumper_with_literal(data):
+            if data in literal_cases:
+                return literal_dumper(data)
+            return dumper_type_dispatcher.dispatch(type(data))(data)
+
+        return union_dumper_with_literal
+
+    def _get_dumper_for_literal(
+        self,
+        norm: BaseNormType,
+        dumpers: Iterable[Any],
+        dumper_type_dispatcher: ClassDispatcher[Any, Dumper],
+    ) -> Optional[Dumper]:
+        try:
+            literal_type, literal_dumper = next(
+                (union_case, dumper) for union_case, dumper
+                in zip(norm.args, dumpers)
+                if union_case.origin is Literal
+            )
+        except StopIteration:
+            return None
+
+        literal_cases = [strip_annotated(arg) for arg in literal_type.args]
+        return self._produce_dumper_for_literal(dumper_type_dispatcher, literal_dumper, literal_cases)
+
     def _get_single_optional_dumper(self, dumper: Dumper) -> Dumper:
         def optional_dumper(data):
             if data is None:
                 return None
             return dumper(data)
 
         return optional_dumper
```

### Comparing `adaptix-3.0.0b4/src/adaptix/_internal/morphing/iterable_provider.py` & `adaptix-3.0.0b5/src/adaptix/_internal/morphing/iterable_provider.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0b4/src/adaptix/_internal/morphing/load_error.py` & `adaptix-3.0.0b5/src/adaptix/_internal/morphing/load_error.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0b4/src/adaptix/_internal/morphing/model/basic_gen.py` & `adaptix-3.0.0b5/src/adaptix/_internal/morphing/model/basic_gen.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,17 +81,16 @@
             self.list.append((request, data))
 
         return hook
 
     @property
     def code_pairs(self):
         return [
-            (request.loc_stack[-2].loc.type, hook_data.source)
+            (request.last_loc.type, hook_data.source)
             for request, hook_data in self.list
-            if len(request.loc_stack) >= 2  # noqa: PLR2004
         ]
 
     @property
     def code_dict(self):
         return dict(self.code_pairs)
```

### Comparing `adaptix-3.0.0b4/src/adaptix/_internal/morphing/model/crown_definitions.py` & `adaptix-3.0.0b5/src/adaptix/_internal/morphing/model/crown_definitions.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0b4/src/adaptix/_internal/morphing/model/dumper_gen.py` & `adaptix-3.0.0b5/src/adaptix/_internal/morphing/model/dumper_gen.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0b4/src/adaptix/_internal/morphing/model/dumper_provider.py` & `adaptix-3.0.0b5/src/adaptix/_internal/morphing/model/dumper_provider.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0b4/src/adaptix/_internal/morphing/model/loader_gen.py` & `adaptix-3.0.0b5/src/adaptix/_internal/morphing/model/loader_gen.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0b4/src/adaptix/_internal/morphing/model/loader_provider.py` & `adaptix-3.0.0b5/src/adaptix/_internal/morphing/model/loader_provider.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0b4/src/adaptix/_internal/morphing/model/request_filtering.py` & `adaptix-3.0.0b5/src/adaptix/_internal/morphing/model/request_filtering.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0b4/src/adaptix/_internal/morphing/name_layout/base.py` & `adaptix-3.0.0b5/src/adaptix/_internal/morphing/name_layout/base.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0b4/src/adaptix/_internal/morphing/name_layout/component.py` & `adaptix-3.0.0b5/src/adaptix/_internal/morphing/name_layout/component.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0b4/src/adaptix/_internal/morphing/name_layout/crown_builder.py` & `adaptix-3.0.0b5/src/adaptix/_internal/morphing/name_layout/crown_builder.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0b4/src/adaptix/_internal/morphing/name_layout/name_mapping.py` & `adaptix-3.0.0b5/src/adaptix/_internal/morphing/name_layout/name_mapping.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 from dataclasses import dataclass
 from typing import Callable, Iterable, Mapping, Optional, Tuple, Union
 
 from ...common import EllipsisType
-from ...model_tools.definitions import BaseField, BaseShape, is_valid_field_id
+from ...model_tools.definitions import BaseField, BaseShape, OutputField, is_valid_field_id
 from ...provider.essential import CannotProvide, Mediator, Provider
 from ...provider.loc_stack_filtering import LocStackChecker, Pred
 from ...provider.provider_wrapper import ProviderWithLSC
 from ...provider.request_cls import LocatedRequest
 from ...provider.static_provider import StaticProvider, static_provision_action
 from .base import Key, KeyPath
 
@@ -55,15 +55,15 @@
         if invalid_keys:
             raise ValueError(
                 "Keys of dict name mapping must be valid field_id (valid python identifier)."
                 f" Keys {invalid_keys!r} does not meet this condition.",
             )
 
     @static_provision_action
-    def _provide_input_name_layout(self, mediator: Mediator, request: NameMappingRequest) -> Optional[KeyPath]:
+    def _provide_name_mapping(self, mediator: Mediator, request: NameMappingRequest) -> Optional[KeyPath]:
         try:
             map_result = self._name_map[request.field.id]
         except KeyError:
             raise CannotProvide
         return resolve_map_result(request.generated_key, map_result)
 
 
@@ -72,25 +72,35 @@
         self._loc_stack_checker = loc_stack_checker
         self._result = result
 
     def get_loc_stack_checker(self) -> Optional[LocStackChecker]:
         return self._loc_stack_checker
 
     @static_provision_action
-    def _provide_input_name_layout(self, mediator: Mediator, request: NameMappingRequest) -> Optional[KeyPath]:
+    def _provide_name_mapping(self, mediator: Mediator, request: NameMappingRequest) -> Optional[KeyPath]:
         self._apply_loc_stack_checker(mediator, request)
         return resolve_map_result(request.generated_key, self._result)
 
 
 class FuncNameMappingProvider(StaticProvider, ProviderWithLSC):
     def __init__(self, loc_stack_checker: LocStackChecker, func: Callable[[BaseShape, BaseField], MapResult]):
         self._loc_stack_checker = loc_stack_checker
         self._func = func
 
     def get_loc_stack_checker(self) -> Optional[LocStackChecker]:
         return self._loc_stack_checker
 
     @static_provision_action
-    def _provide_input_name_layout(self, mediator: Mediator, request: NameMappingRequest) -> Optional[KeyPath]:
+    def _provide_name_mapping(self, mediator: Mediator, request: NameMappingRequest) -> Optional[KeyPath]:
         self._apply_loc_stack_checker(mediator, request)
         result = self._func(request.shape, request.field)
         return resolve_map_result(request.generated_key, result)
+
+
+class SkipPrivateFieldsNameMappingProvider(StaticProvider):
+    @static_provision_action
+    def _provide_name_mapping(self, mediator: Mediator, request: NameMappingRequest) -> Optional[KeyPath]:
+        if not isinstance(request.field, OutputField):
+            raise CannotProvide
+        if request.field.id.startswith("_"):
+            return None
+        raise CannotProvide
```

### Comparing `adaptix-3.0.0b4/src/adaptix/_internal/morphing/name_layout/provider.py` & `adaptix-3.0.0b5/src/adaptix/_internal/morphing/name_layout/provider.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0b4/src/adaptix/_internal/morphing/provider_template.py` & `adaptix-3.0.0b5/src/adaptix/_internal/morphing/provider_template.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0b4/src/adaptix/_internal/name_style.py` & `adaptix-3.0.0b5/src/adaptix/_internal/name_style.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0b4/src/adaptix/_internal/provider/essential.py` & `adaptix-3.0.0b5/src/adaptix/_internal/provider/essential.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0b4/src/adaptix/_internal/provider/facade/provider.py` & `adaptix-3.0.0b5/src/adaptix/_internal/provider/facade/provider.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0b4/src/adaptix/_internal/provider/fields.py` & `adaptix-3.0.0b5/src/adaptix/_internal/provider/fields.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0b4/src/adaptix/_internal/provider/loc_stack_filtering.py` & `adaptix-3.0.0b5/src/adaptix/_internal/provider/loc_stack_filtering.py`

 * *Files 1% similar despite different names*

```diff
@@ -279,20 +279,27 @@
         return _create_loc_stack_checker_by_origin(norm.origin)   # this is only an optimization
     return ExactTypeLSC(norm)
 
 
 Pat = TypeVar("Pat", bound="LocStackPattern")
 
 
-class LocStackPattern:
-    ANY = AnyLocStackChecker()
+_ANY = AnyLocStackChecker()
+
 
+class LocStackPattern:
     def __init__(self, stack: VarTuple[LocStackChecker]):
         self._stack = stack
 
+    @property
+    def ANY(self) -> AnyLocStackChecker:  # noqa: N802
+        if self._stack:
+            raise AttributeError("You must access to ANY only via `P.ANY`, other usage is misleading")
+        return _ANY
+
     @classmethod
     def _from_lsc(cls: Type[Pat], lsc: LocStackChecker) -> Pat:
         return cls((lsc, ))
 
     def _extend_stack(self: Pat, elements: Iterable[LocStackChecker]) -> Pat:
         self_copy = copy(self)
         self_copy._stack = self._stack + tuple(elements)
```

### Comparing `adaptix-3.0.0b4/src/adaptix/_internal/provider/location.py` & `adaptix-3.0.0b5/src/adaptix/_internal/provider/location.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0b4/src/adaptix/_internal/provider/overlay_schema.py` & `adaptix-3.0.0b5/src/adaptix/_internal/provider/overlay_schema.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0b4/src/adaptix/_internal/provider/provider_template.py` & `adaptix-3.0.0b5/src/adaptix/_internal/provider/provider_template.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0b4/src/adaptix/_internal/provider/provider_wrapper.py` & `adaptix-3.0.0b5/src/adaptix/_internal/provider/provider_wrapper.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0b4/src/adaptix/_internal/provider/request_cls.py` & `adaptix-3.0.0b5/src/adaptix/_internal/provider/request_cls.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0b4/src/adaptix/_internal/provider/shape_provider.py` & `adaptix-3.0.0b5/src/adaptix/_internal/provider/shape_provider.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     ShapeIntrospector,
     TooOldPackageError,
 )
 from ..model_tools.introspection.attrs import get_attrs_shape
 from ..model_tools.introspection.class_init import get_class_init_shape
 from ..model_tools.introspection.dataclass import get_dataclass_shape
 from ..model_tools.introspection.named_tuple import get_named_tuple_shape
+from ..model_tools.introspection.pydantic import get_pydantic_shape
 from ..model_tools.introspection.sqlalchemy import get_sqlalchemy_shape
 from ..model_tools.introspection.typed_dict import get_typed_dict_shape
 from ..provider.essential import CannotProvide, Mediator
 from ..provider.loc_stack_filtering import create_loc_stack_checker
 from ..type_tools.generic_resolver import GenericResolver, MembersStorage
 from .provider_template import ProviderWithAttachableLSC
 from .provider_wrapper import ConcatProvider
@@ -75,14 +76,15 @@
 
 BUILTIN_SHAPE_PROVIDER = ConcatProvider(
     ShapeProvider(get_named_tuple_shape),
     ShapeProvider(get_typed_dict_shape),
     ShapeProvider(get_dataclass_shape),
     ShapeProvider(get_attrs_shape),
     ShapeProvider(get_sqlalchemy_shape),
+    ShapeProvider(get_pydantic_shape),
     # class init introspection must be the last
     ShapeProvider(get_class_init_shape),
 )
 
 
 class PropertyExtender(StaticProvider):
     def __init__(
```

### Comparing `adaptix-3.0.0b4/src/adaptix/_internal/provider/static_provider.py` & `adaptix-3.0.0b5/src/adaptix/_internal/provider/static_provider.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0b4/src/adaptix/_internal/retort/base_retort.py` & `adaptix-3.0.0b5/src/adaptix/_internal/retort/base_retort.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0b4/src/adaptix/_internal/retort/mediator.py` & `adaptix-3.0.0b5/src/adaptix/_internal/retort/mediator.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0b4/src/adaptix/_internal/retort/operating_retort.py` & `adaptix-3.0.0b5/src/adaptix/_internal/retort/operating_retort.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from ..common import TypeHint, VarTuple
 from ..conversion.request_cls import CoercerRequest, ConversionDestItem, ConversionSourceItem, LinkingRequest
 from ..morphing.request_cls import DumperRequest, LoaderRequest
 from ..provider.essential import AggregateCannotProvide, CannotProvide, Mediator, Provider, Request
 from ..provider.location import AnyLoc, FieldLoc
 from ..provider.request_cls import LocatedRequest, LocStack
 from ..type_tools import is_parametrized
-from ..utils import copy_exception_dunders, with_module
+from ..utils import add_note, copy_exception_dunders, with_module
 from .base_retort import BaseRetort
 from .mediator import ErrorRepresentor, RecursionResolver, T
 
 
 class FuncWrapper:
     __slots__ = ("__call__",)
 
@@ -125,15 +125,18 @@
         return self._provide_from_recipe(request)
 
     def _facade_provide(self, request: Request[T], *, error_message: str) -> T:
         try:
             return self._provide_from_recipe(request)
         except CannotProvide as e:
             cause = self._get_exception_cause(e)
-            raise NoSuitableProvider(error_message) from cause
+            exception = NoSuitableProvider(error_message)
+            if cause is not None:
+                add_note(exception, "Note: The attached exception above contains verbose description of the problem")
+            raise exception from cause
 
     def _get_exception_cause(self, exc: CannotProvide) -> Optional[CannotProvide]:
         if isinstance(exc, AggregateCannotProvide):
             return self._extract_demonstrative_exc(exc)
         return exc if exc.is_demonstrative else None
 
     def _extract_demonstrative_exc(self, exc: AggregateCannotProvide) -> Optional[CannotProvide]:
```

### Comparing `adaptix-3.0.0b4/src/adaptix/_internal/retort/routing.py` & `adaptix-3.0.0b5/src/adaptix/_internal/retort/routing.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0b4/src/adaptix/_internal/special_cases_optimization.py` & `adaptix-3.0.0b5/src/adaptix/_internal/special_cases_optimization.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0b4/src/adaptix/_internal/struct_trail.py` & `adaptix-3.0.0b5/src/adaptix/_internal/struct_trail.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0b4/src/adaptix/_internal/type_tools/__init__.py` & `adaptix-3.0.0b5/src/adaptix/_internal/type_tools/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 from .basic_utils import (
     create_union,
-    get_all_type_hints,
     is_bare_generic,
     is_generic,
     is_generic_class,
     is_named_tuple_class,
     is_new_type,
     is_parametrized,
     is_protocol,
     is_subclass_soft,
     is_typed_dict_class,
     is_user_defined_generic,
-    strip_alias,
 )
+from .fundamentals import get_all_type_hints, get_generic_args, get_type_vars, is_pydantic_class, strip_alias
 from .norm_utils import is_class_var, strip_tags
 from .normalize_type import (
     AnyNormTypeVarLike,
     BaseNormType,
     NormParamSpecMarker,
     NormTV,
     NormTVTuple,
```

### Comparing `adaptix-3.0.0b4/src/adaptix/_internal/type_tools/basic_utils.py` & `adaptix-3.0.0b5/src/adaptix/_internal/type_tools/basic_utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,100 +1,65 @@
 import types
 import typing
-from typing import (
-    Any,
-    Dict,
-    ForwardRef,
-    Generic,
-    Iterable,
-    Protocol,
-    TypedDict,
-    TypeVar,
-    Union,
-    get_args,
-    get_origin,
-    get_type_hints,
-)
+from typing import Any, Dict, ForwardRef, Generic, NewType, Protocol, TypedDict, TypeVar, Union
 
 from ..common import TypeHint, VarTuple
 from ..feature_requirement import HAS_ANNOTATED, HAS_PY_39, HAS_PY_312, HAS_STD_CLASSES_GENERICS
 from .constants import BUILTIN_ORIGIN_TO_TYPEVARS
-
-TYPED_DICT_MCS = type(types.new_class("_TypedDictSample", (TypedDict,), {}))
-
-
-def strip_alias(type_hint: TypeHint) -> TypeHint:
-    origin = get_origin(type_hint)
-    return type_hint if origin is None else origin
+from .fundamentals import get_generic_args, get_type_vars, strip_alias
 
 
 def is_subclass_soft(cls, classinfo) -> bool:
-    """Acts like builtin issubclass,
-     but returns False instead of rising TypeError
-    """
+    """Acts like builtin issubclass, but returns False instead of rising TypeError"""
     try:
         return issubclass(cls, classinfo)
     except TypeError:
         return False
 
 
-def has_attrs(obj, attrs: Iterable[str]) -> bool:
-    return all(
-        hasattr(obj, attr_name)
-        for attr_name in attrs
-    )
+_NEW_TYPE_CLS = type(NewType("", None))
 
 
 def is_new_type(tp) -> bool:
-    return has_attrs(tp, ["__supertype__", "__name__"])
+    return isinstance(tp, _NEW_TYPE_CLS)
+
+
+_TYPED_DICT_MCS = type(types.new_class("_TypedDictSample", (TypedDict,), {}))
 
 
 def is_typed_dict_class(tp) -> bool:
-    return isinstance(tp, TYPED_DICT_MCS)
+    return isinstance(tp, _TYPED_DICT_MCS)
 
 
-NAMED_TUPLE_METHODS = ("_fields", "_field_defaults", "_make", "_replace", "_asdict")
+_NAMED_TUPLE_METHODS = ("_fields", "_field_defaults", "_make", "_replace", "_asdict")
 
 
 def is_named_tuple_class(tp) -> bool:
     return (
         is_subclass_soft(tp, tuple)
-        and
-        has_attrs(tp, NAMED_TUPLE_METHODS)
+        and all(
+            hasattr(tp, attr_name)
+            for attr_name in _NAMED_TUPLE_METHODS
+        )
     )
 
 
 def is_protocol(tp):
     if not isinstance(tp, type):
         return False
 
     return Protocol in tp.__bases__
 
 
 def create_union(args: tuple):
     return Union[args]
 
 
-if HAS_ANNOTATED:
-    def get_all_type_hints(obj, globalns=None, localns=None):
-        return get_type_hints(obj, globalns, localns, include_extras=True)
-else:
-    get_all_type_hints = get_type_hints
-
-
 def is_parametrized(tp: TypeHint) -> bool:
-    return bool(get_args(tp))
-
-
-def get_type_vars(tp: TypeHint) -> VarTuple[TypeVar]:
-    type_vars = getattr(tp, "__parameters__", ())
-    # UnionType object contains descriptor inside `__parameters__`
-    if not isinstance(type_vars, tuple):
-        return ()
-    return type_vars
+    return bool(get_generic_args(tp))
 
 
 if HAS_PY_312:
     def is_user_defined_generic(tp: TypeHint) -> bool:
         return (
             bool(get_type_vars(tp))
             and (
@@ -120,15 +85,16 @@
             and not is_parametrized(tp)
             and (
                 bool(HAS_STD_CLASSES_GENERICS) or not isinstance(tp, type)
             )
         )
         or (
             bool(HAS_ANNOTATED)
-            and get_origin(tp) == typing.Annotated
+            and strip_alias(tp) == typing.Annotated
+            and tp != typing.Annotated
             and is_generic(tp.__origin__)
         )
     )
 
 
 def is_bare_generic(tp: TypeHint) -> bool:
     """Check if the type could be parameterized, excluding type aliases (list[T] etc.)"""
@@ -155,24 +121,22 @@
             issubclass(cls, Generic)  # type: ignore[arg-type]
             and bool(cls.__parameters__)  # type: ignore[attr-defined]
         )
     )
 
 
 def get_type_vars_of_parametrized(tp: TypeHint) -> VarTuple[TypeVar]:
-    try:
-        params = tp.__parameters__
-    except AttributeError:
+    params = get_type_vars(tp)
+    if not params:
         return ()
-
     if isinstance(tp, type):
         if HAS_STD_CLASSES_GENERICS and isinstance(tp, types.GenericAlias):
             return params
         return ()
-    if get_origin(tp) is not None and get_args(tp) == ():
+    if strip_alias(tp) != tp and get_generic_args(tp) == ():
         return ()
     return params
 
 
 if HAS_PY_39:
     def eval_forward_ref(namespace: Dict[str, Any], forward_ref: ForwardRef):
         return forward_ref._evaluate(namespace, None, frozenset())
```

### Comparing `adaptix-3.0.0b4/src/adaptix/_internal/type_tools/constants.py` & `adaptix-3.0.0b5/src/adaptix/_internal/type_tools/constants.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0b4/src/adaptix/_internal/type_tools/generic_resolver.py` & `adaptix-3.0.0b5/src/adaptix/_internal/type_tools/generic_resolver.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import typing
 from dataclasses import dataclass, replace
 from itertools import chain
-from typing import Callable, Collection, Dict, Generic, Hashable, Mapping, TypeVar, get_args
+from typing import Callable, Collection, Dict, Generic, Hashable, Mapping, TypeVar
 
 from ..common import TypeHint
 from ..feature_requirement import HAS_TV_TUPLE, HAS_UNPACK
+from . import get_generic_args
 from .basic_utils import get_type_vars, get_type_vars_of_parametrized, is_generic, is_parametrized, strip_alias
 from .implicit_params import fill_implicit_params
 from .normalize_type import normalize_type
 
 M = TypeVar("M")
 K = TypeVar("K", bound=Hashable)
 
@@ -32,15 +33,15 @@
         return self._get_members_by_parents(tp)
 
     def _get_members_of_parametrized_generic(self, parametrized_generic) -> MembersStorage[K, M]:
         origin = strip_alias(parametrized_generic)
         members_storage = self._get_members_by_parents(origin)
         type_var_to_actual = self._get_type_var_to_actual(
             get_type_vars(origin),
-            self._unpack_args(get_args(parametrized_generic)),
+            self._unpack_args(get_generic_args(parametrized_generic)),
         )
         return replace(
             members_storage,
             members={
                 key: self._parametrize_by_dict(type_var_to_actual, tp)
                 for key, tp in members_storage.members.items()
             },
```

### Comparing `adaptix-3.0.0b4/src/adaptix/_internal/type_tools/implicit_params.py` & `adaptix-3.0.0b5/src/adaptix/_internal/type_tools/implicit_params.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0b4/src/adaptix/_internal/type_tools/norm_utils.py` & `adaptix-3.0.0b5/src/adaptix/_internal/type_tools/norm_utils.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0b4/src/adaptix/_internal/type_tools/normalize_type.py` & `adaptix-3.0.0b5/src/adaptix/_internal/type_tools/normalize_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,14 @@
     NoReturn,
     Optional,
     Sequence,
     Tuple,
     Type,
     TypeVar,
     Union,
-    get_args,
     overload,
 )
 
 from ..common import TypeHint, VarTuple
 from ..feature_requirement import (
     HAS_ANNOTATED,
     HAS_PARAM_SPEC,
@@ -45,14 +44,15 @@
     HAS_TYPE_ALIAS,
     HAS_TYPE_GUARD,
     HAS_TYPE_UNION_OP,
     HAS_TYPED_DICT_REQUIRED,
     HAS_UNPACK,
 )
 from .basic_utils import create_union, eval_forward_ref, is_new_type, is_subclass_soft, strip_alias
+from .fundamentals import get_generic_args
 from .implicit_params import ImplicitParamsGetter
 
 
 class BaseNormType(Hashable, ABC):
     @property
     @abstractmethod
     def origin(self) -> Any:
@@ -523,15 +523,15 @@
 
     @overload
     def normalize(self, tp: TypeHint) -> BaseNormType:
         ...
 
     def normalize(self, tp: TypeHint) -> BaseNormType:
         origin = strip_alias(tp)
-        args = get_args(tp)
+        args = get_generic_args(tp)
 
         result = self._norm_forward_ref(tp)
         if result is not None:
             return result
 
         for attr_name in self._aspect_storage:
             result = getattr(self, attr_name)(tp, origin, args)
```

### Comparing `adaptix-3.0.0b4/src/adaptix/_internal/utils.py` & `adaptix-3.0.0b5/src/adaptix/_internal/utils.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0b4/src/adaptix/conversion/__init__.py` & `adaptix-3.0.0b5/src/adaptix/conversion/__init__.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0b4/src/adaptix/load_error.py` & `adaptix-3.0.0b5/src/adaptix/load_error.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0b4/src/adaptix.egg-info/PKG-INFO` & `adaptix-3.0.0b5/src/adaptix.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adaptix
-Version: 3.0.0b4
+Version: 3.0.0b5
 Summary: An extremely flexible and configurable data model conversion library
 Author-email: "A. Tikhonov" <17@itishka.org>
 Project-URL: Homepage, https://github.com/reagento/adaptix
 Project-URL: Bug Tracker, https://github.com/reagento/adaptix/issues
 Project-URL: Documentation, https://adaptix.readthedocs.io/en/latest/
 Project-URL: Changelog, https://adaptix.readthedocs.io/en/latest/reference/changelog.html
 Project-URL: Source, https://github.com/reagento/adaptix/
@@ -35,19 +35,23 @@
 Requires-Dist: attrs>=21.3.0; extra == "attrs"
 Provides-Extra: attrs-strict
 Requires-Dist: attrs<=23.2.0,>=21.3.0; extra == "attrs-strict"
 Provides-Extra: sqlalchemy
 Requires-Dist: sqlalchemy>=2.0.0; extra == "sqlalchemy"
 Provides-Extra: sqlalchemy-strict
 Requires-Dist: sqlalchemy<=2.0.29,>=2.0.0; extra == "sqlalchemy-strict"
+Provides-Extra: pydantic
+Requires-Dist: pydantic>=2.0.0; extra == "pydantic"
+Provides-Extra: pydantic-strict
+Requires-Dist: pydantic<=2.7.0,>=2.0.0; extra == "pydantic-strict"
 
 <div align="center">
   <picture>
-    <source media="(prefers-color-scheme: dark)" srcset="https://github.com/reagento/adaptix/blob/v3.0.0b4/docs/logo/adaptix-with-title-dark.png?raw=true">
-    <source media="(prefers-color-scheme: light)" srcset="https://github.com/reagento/adaptix/blob/v3.0.0b4/docs/logo/adaptix-with-title-light.png?raw=true">
+    <source media="(prefers-color-scheme: dark)" srcset="https://github.com/reagento/adaptix/blob/v3.0.0b5/docs/logo/adaptix-with-title-dark.png?raw=true">
+    <source media="(prefers-color-scheme: light)" srcset="https://github.com/reagento/adaptix/blob/v3.0.0b5/docs/logo/adaptix-with-title-light.png?raw=true">
     <img alt="adaptix logo" src="https://raw.githubusercontent.com/reagento/adaptix/v3.0.0b2/docs/logo/adaptix-with-title-light.png?raw=true">
   </picture>
 
   <hr>
 
   [![PyPI version](https://img.shields.io/pypi/v/adaptix.svg?color=blue)](https://pypi.org/project/adaptix/)
   [![downloads](https://img.shields.io/pypi/dm/adaptix.svg)](https://pypistats.org/packages/adaptix)
@@ -63,30 +67,29 @@
 
 📚 [Documentation](https://adaptix.readthedocs.io/)
 
 ## TL;DR
 
 Install
 ```bash
-pip install adaptix==3.0.0b4
+pip install adaptix==3.0.0b5
 ```
 
 Use for model loading and dumping.
 
 ```python
 from dataclasses import dataclass
 
 from adaptix import Retort
 
 
 @dataclass
 class Book:
     title: str
     price: int
-    author: str = "Unknown author"
 
 
 data = {
     "title": "Fahrenheit 451",
     "price": 100,
 }
 
@@ -153,15 +156,15 @@
   that allow preserving [SRP](https://blog.cleancoder.com/uncle-bob/2014/05/08/SingleReponsibilityPrinciple.html)
   and have different representations for one model.
 * Speed. It is one of the fastest data parsing and serialization libraries.
 * There is no forced model representation, adaptix can adjust to your needs.
 * Support [dozens](https://adaptix.readthedocs.io/en/latest/loading-and-dumping/specific-types-behavior.html) of types,
   including different model kinds:
   ``@dataclass``, ``TypedDict``, ``NamedTuple``,
-  [``attrs``](https://www.attrs.org/en/stable/) and [``sqlalchemy``](https://docs.sqlalchemy.org/en/20/)
+  [``attrs``](https://www.attrs.org/en/stable/), [``sqlalchemy``](https://docs.sqlalchemy.org/en/20/) and [``pydantic``](https://docs.pydantic.dev/latest/).
 * Working with self-referenced data types (such as linked lists or trees).
 * Saving [path](https://adaptix.readthedocs.io/en/latest/loading-and-dumping/tutorial.html#error-handling)
   where an exception is raised (including unexpected errors).
 * Machine-readable [errors](https://adaptix.readthedocs.io/en/latest/loading-and-dumping/tutorial.html#error-handling)
   that could be dumped.
 * Support for user-defined generic models.
 * Automatic name style conversion (e.g. `snake_case` to `camelCase`).
```

### Comparing `adaptix-3.0.0b4/src/adaptix.egg-info/SOURCES.txt` & `adaptix-3.0.0b5/src/adaptix.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -41,22 +41,26 @@
 src/adaptix/_internal/conversion/broaching/code_generator.py
 src/adaptix/_internal/conversion/broaching/definitions.py
 src/adaptix/_internal/conversion/facade/__init__.py
 src/adaptix/_internal/conversion/facade/checker.py
 src/adaptix/_internal/conversion/facade/func.py
 src/adaptix/_internal/conversion/facade/provider.py
 src/adaptix/_internal/conversion/facade/retort.py
+src/adaptix/_internal/integrations/__init__.py
+src/adaptix/_internal/integrations/pydantic/__init__.py
+src/adaptix/_internal/integrations/pydantic/native.py
 src/adaptix/_internal/model_tools/__init__.py
 src/adaptix/_internal/model_tools/definitions.py
 src/adaptix/_internal/model_tools/introspection/__init__.py
 src/adaptix/_internal/model_tools/introspection/attrs.py
 src/adaptix/_internal/model_tools/introspection/callable.py
 src/adaptix/_internal/model_tools/introspection/class_init.py
 src/adaptix/_internal/model_tools/introspection/dataclass.py
 src/adaptix/_internal/model_tools/introspection/named_tuple.py
+src/adaptix/_internal/model_tools/introspection/pydantic.py
 src/adaptix/_internal/model_tools/introspection/sqlalchemy.py
 src/adaptix/_internal/model_tools/introspection/typed_dict.py
 src/adaptix/_internal/morphing/__init__.py
 src/adaptix/_internal/morphing/concrete_provider.py
 src/adaptix/_internal/morphing/constant_length_tuple_provider.py
 src/adaptix/_internal/morphing/dict_provider.py
 src/adaptix/_internal/morphing/enum_provider.py
@@ -100,14 +104,18 @@
 src/adaptix/_internal/retort/base_retort.py
 src/adaptix/_internal/retort/mediator.py
 src/adaptix/_internal/retort/operating_retort.py
 src/adaptix/_internal/retort/routing.py
 src/adaptix/_internal/type_tools/__init__.py
 src/adaptix/_internal/type_tools/basic_utils.py
 src/adaptix/_internal/type_tools/constants.py
+src/adaptix/_internal/type_tools/fundamentals.py
 src/adaptix/_internal/type_tools/generic_resolver.py
 src/adaptix/_internal/type_tools/implicit_params.py
 src/adaptix/_internal/type_tools/norm_utils.py
 src/adaptix/_internal/type_tools/normalize_type.py
 src/adaptix/conversion/__init__.py
+src/adaptix/integrations/__init__.py
+src/adaptix/integrations/pydantic/__init__.py
 src/adaptix/provider/__init__.py
-tests/test_doc.py
+tests/test_doc.py
+tests/test_meta.py
```

