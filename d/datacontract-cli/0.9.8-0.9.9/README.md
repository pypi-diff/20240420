# Comparing `tmp/datacontract-cli-0.9.8.tar.gz` & `tmp/datacontract_cli-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datacontract-cli-0.9.8.tar", last modified: Mon Apr  1 11:03:51 2024, max compression
+gzip compressed data, was "datacontract_cli-0.9.9.tar", last modified: Thu Apr 18 09:17:09 2024, max compression
```

## Comparing `datacontract-cli-0.9.8.tar` & `datacontract_cli-0.9.9.tar`

### file list

```diff
@@ -1,138 +1,140 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 11:03:51.012667 datacontract-cli-0.9.8/
--rw-r--r--   0 runner    (1001) docker     (127)     2210 2024-04-01 11:02:03.000000 datacontract-cli-0.9.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    35510 2024-04-01 11:03:51.012667 datacontract-cli-0.9.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    33646 2024-04-01 11:02:03.000000 datacontract-cli-0.9.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 11:03:50.988667 datacontract-cli-0.9.8/datacontract/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 11:02:03.000000 datacontract-cli-0.9.8/datacontract/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 11:03:50.992667 datacontract-cli-0.9.8/datacontract/breaking/
--rw-r--r--   0 runner    (1001) docker     (127)    11719 2024-04-01 11:02:03.000000 datacontract-cli-0.9.8/datacontract/breaking/breaking.py
--rw-r--r--   0 runner    (1001) docker     (127)     2913 2024-04-01 11:02:03.000000 datacontract-cli-0.9.8/datacontract/breaking/breaking_rules.py
--rw-r--r--   0 runner    (1001) docker     (127)    10515 2024-04-01 11:02:03.000000 datacontract-cli-0.9.8/datacontract/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    21656 2024-04-01 11:02:03.000000 datacontract-cli-0.9.8/datacontract/data_contract.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 11:03:50.992667 datacontract-cli-0.9.8/datacontract/engines/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 11:02:03.000000 datacontract-cli-0.9.8/datacontract/engines/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 11:03:50.992667 datacontract-cli-0.9.8/datacontract/engines/datacontract/
--rw-r--r--   0 runner    (1001) docker     (127)     1565 2024-04-01 11:02:03.000000 datacontract-cli-0.9.8/datacontract/engines/datacontract/check_that_datacontract_contains_valid_servers_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)      665 2024-04-01 11:02:03.000000 datacontract-cli-0.9.8/datacontract/engines/datacontract/check_that_datacontract_file_exists.py
--rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-04-01 11:02:03.000000 datacontract-cli-0.9.8/datacontract/engines/datacontract/check_that_datacontract_str_is_valid.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 11:03:50.992667 datacontract-cli-0.9.8/datacontract/engines/fastjsonschema/
--rw-r--r--   0 runner    (1001) docker     (127)     5754 2024-04-01 11:02:03.000000 datacontract-cli-0.9.8/datacontract/engines/fastjsonschema/check_jsonschema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 11:03:50.992667 datacontract-cli-0.9.8/datacontract/engines/fastjsonschema/s3/
--rw-r--r--   0 runner    (1001) docker     (127)      665 2024-04-01 11:02:03.000000 datacontract-cli-0.9.8/datacontract/engines/fastjsonschema/s3/s3_read_files.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 11:03:50.992667 datacontract-cli-0.9.8/datacontract/engines/soda/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 11:02:03.000000 datacontract-cli-0.9.8/datacontract/engines/soda/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6507 2024-04-01 11:02:03.000000 datacontract-cli-0.9.8/datacontract/engines/soda/check_soda_execute.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 11:03:50.992667 datacontract-cli-0.9.8/datacontract/engines/soda/connections/
--rw-r--r--   0 runner    (1001) docker     (127)      662 2024-04-01 11:02:03.000000 datacontract-cli-0.9.8/datacontract/engines/soda/connections/bigquery.py
--rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-04-01 11:02:03.000000 datacontract-cli-0.9.8/datacontract/engines/soda/connections/dask.py
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-01 11:02:03.000000 datacontract-cli-0.9.8/datacontract/engines/soda/connections/databricks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2340 2024-04-01 11:02:03.000000 datacontract-cli-0.9.8/datacontract/engines/soda/connections/duckdb.py
--rw-r--r--   0 runner    (1001) docker     (127)     5971 2024-04-01 11:02:03.000000 datacontract-cli-0.9.8/datacontract/engines/soda/connections/kafka.py
--rw-r--r--   0 runner    (1001) docker     (127)      626 2024-04-01 11:02:03.000000 datacontract-cli-0.9.8/datacontract/engines/soda/connections/postgres.py
--rw-r--r--   0 runner    (1001) docker     (127)      719 2024-04-01 11:02:03.000000 datacontract-cli-0.9.8/datacontract/engines/soda/connections/snowflake.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 11:03:50.996667 datacontract-cli-0.9.8/datacontract/export/
--rw-r--r--   0 runner    (1001) docker     (127)     2202 2024-04-01 11:02:03.000000 datacontract-cli-0.9.8/datacontract/export/avro_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     9582 2024-04-01 11:02:03.000000 datacontract-cli-0.9.8/datacontract/export/avro_idl_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     8549 2024-04-01 11:02:03.000000 datacontract-cli-0.9.8/datacontract/export/dbt_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4908 2024-04-01 11:02:03.000000 datacontract-cli-0.9.8/datacontract/export/great_expectations_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3153 2024-04-01 11:02:03.000000 datacontract-cli-0.9.8/datacontract/export/jsonschema_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-04-01 11:02:03.000000 datacontract-cli-0.9.8/datacontract/export/odcs_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2974 2024-04-01 11:02:03.000000 datacontract-cli-0.9.8/datacontract/export/protobuf_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5670 2024-04-01 11:02:03.000000 datacontract-cli-0.9.8/datacontract/export/pydantic_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     6108 2024-04-01 11:02:03.000000 datacontract-cli-0.9.8/datacontract/export/rdf_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3197 2024-04-01 11:02:03.000000 datacontract-cli-0.9.8/datacontract/export/sodacl_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3343 2024-04-01 11:02:03.000000 datacontract-cli-0.9.8/datacontract/export/sql_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4627 2024-04-01 11:02:03.000000 datacontract-cli-0.9.8/datacontract/export/sql_type_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-04-01 11:02:03.000000 datacontract-cli-0.9.8/datacontract/export/terraform_converter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 11:03:50.996667 datacontract-cli-0.9.8/datacontract/imports/
--rw-r--r--   0 runner    (1001) docker     (127)     3823 2024-04-01 11:02:03.000000 datacontract-cli-0.9.8/datacontract/imports/avro_importer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-04-01 11:02:03.000000 datacontract-cli-0.9.8/datacontract/imports/sql_importer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 11:03:50.996667 datacontract-cli-0.9.8/datacontract/init/
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-01 11:02:03.000000 datacontract-cli-0.9.8/datacontract/init/download_datacontract_file.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 11:03:50.996667 datacontract-cli-0.9.8/datacontract/integration/
--rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-04-01 11:02:03.000000 datacontract-cli-0.9.8/datacontract/integration/publish_datamesh_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     3830 2024-04-01 11:02:03.000000 datacontract-cli-0.9.8/datacontract/integration/publish_opentelemetry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 11:03:50.996667 datacontract-cli-0.9.8/datacontract/lint/
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-04-01 11:02:03.000000 datacontract-cli-0.9.8/datacontract/lint/files.py
--rw-r--r--   0 runner    (1001) docker     (127)     5076 2024-04-01 11:02:03.000000 datacontract-cli-0.9.8/datacontract/lint/lint.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 11:03:51.000667 datacontract-cli-0.9.8/datacontract/lint/linters/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 11:02:03.000000 datacontract-cli-0.9.8/datacontract/lint/linters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-04-01 11:02:03.000000 datacontract-cli-0.9.8/datacontract/lint/linters/description_linter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3978 2024-04-01 11:02:03.000000 datacontract-cli-0.9.8/datacontract/lint/linters/example_model_linter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-04-01 11:02:03.000000 datacontract-cli-0.9.8/datacontract/lint/linters/field_pattern_linter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-04-01 11:02:03.000000 datacontract-cli-0.9.8/datacontract/lint/linters/field_reference_linter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2135 2024-04-01 11:02:03.000000 datacontract-cli-0.9.8/datacontract/lint/linters/notice_period_linter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-04-01 11:02:03.000000 datacontract-cli-0.9.8/datacontract/lint/linters/primary_field_linter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-04-01 11:02:03.000000 datacontract-cli-0.9.8/datacontract/lint/linters/quality_schema_linter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4915 2024-04-01 11:02:03.000000 datacontract-cli-0.9.8/datacontract/lint/linters/valid_constraints_linter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4863 2024-04-01 11:02:03.000000 datacontract-cli-0.9.8/datacontract/lint/resolve.py
--rw-r--r--   0 runner    (1001) docker     (127)      838 2024-04-01 11:02:03.000000 datacontract-cli-0.9.8/datacontract/lint/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-04-01 11:02:03.000000 datacontract-cli-0.9.8/datacontract/lint/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 11:03:51.000667 datacontract-cli-0.9.8/datacontract/model/
--rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-04-01 11:02:03.000000 datacontract-cli-0.9.8/datacontract/model/breaking_change.py
--rw-r--r--   0 runner    (1001) docker     (127)     3480 2024-04-01 11:02:03.000000 datacontract-cli-0.9.8/datacontract/model/data_contract_specification.py
--rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-04-01 11:02:03.000000 datacontract-cli-0.9.8/datacontract/model/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2563 2024-04-01 11:02:03.000000 datacontract-cli-0.9.8/datacontract/model/run.py
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-04-01 11:02:03.000000 datacontract-cli-0.9.8/datacontract/web.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 11:03:51.008667 datacontract-cli-0.9.8/datacontract_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    35510 2024-04-01 11:03:50.000000 datacontract-cli-0.9.8/datacontract_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4419 2024-04-01 11:03:50.000000 datacontract-cli-0.9.8/datacontract_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 11:03:50.000000 datacontract-cli-0.9.8/datacontract_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-01 11:03:50.000000 datacontract-cli-0.9.8/datacontract_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      741 2024-04-01 11:03:50.000000 datacontract-cli-0.9.8/datacontract_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-01 11:03:50.000000 datacontract-cli-0.9.8/datacontract_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-04-01 11:02:03.000000 datacontract-cli-0.9.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 11:03:51.012667 datacontract-cli-0.9.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 11:03:51.008667 datacontract-cli-0.9.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     5895 2024-04-01 11:02:03.000000 datacontract-cli-0.9.8/tests/test_breaking.py
--rw-r--r--   0 runner    (1001) docker     (127)    30873 2024-04-01 11:02:03.000000 datacontract-cli-0.9.8/tests/test_changelog.py
--rw-r--r--   0 runner    (1001) docker     (127)      466 2024-04-01 11:02:03.000000 datacontract-cli-0.9.8/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 11:02:03.000000 datacontract-cli-0.9.8/tests/test_description_linter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-04-01 11:02:03.000000 datacontract-cli-0.9.8/tests/test_documentation_linter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1884 2024-04-01 11:02:03.000000 datacontract-cli-0.9.8/tests/test_download_datacontract_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     3356 2024-04-01 11:02:03.000000 datacontract-cli-0.9.8/tests/test_example_model_linter.py
--rw-r--r--   0 runner    (1001) docker     (127)      949 2024-04-01 11:02:03.000000 datacontract-cli-0.9.8/tests/test_examples_bigquery.py
--rw-r--r--   0 runner    (1001) docker     (127)      812 2024-04-01 11:02:03.000000 datacontract-cli-0.9.8/tests/test_examples_databricks.py
--rw-r--r--   0 runner    (1001) docker     (127)      835 2024-04-01 11:02:03.000000 datacontract-cli-0.9.8/tests/test_examples_examples_csv.py
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-01 11:02:03.000000 datacontract-cli-0.9.8/tests/test_examples_examples_inline.py
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-04-01 11:02:03.000000 datacontract-cli-0.9.8/tests/test_examples_examples_json.py
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-04-01 11:02:03.000000 datacontract-cli-0.9.8/tests/test_examples_examples_missing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1891 2024-04-01 11:02:03.000000 datacontract-cli-0.9.8/tests/test_examples_kafka.py
--rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-04-01 11:02:03.000000 datacontract-cli-0.9.8/tests/test_examples_kafka_remote.py
--rw-r--r--   0 runner    (1001) docker     (127)      650 2024-04-01 11:02:03.000000 datacontract-cli-0.9.8/tests/test_examples_local_json.py
--rw-r--r--   0 runner    (1001) docker     (127)      806 2024-04-01 11:02:03.000000 datacontract-cli-0.9.8/tests/test_examples_parquet.py
--rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-04-01 11:02:03.000000 datacontract-cli-0.9.8/tests/test_examples_postgres.py
--rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-04-01 11:02:03.000000 datacontract-cli-0.9.8/tests/test_examples_s3_csv.py
--rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-04-01 11:02:03.000000 datacontract-cli-0.9.8/tests/test_examples_s3_json.py
--rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-04-01 11:02:03.000000 datacontract-cli-0.9.8/tests/test_examples_s3_json_complex.py
--rw-r--r--   0 runner    (1001) docker     (127)     1989 2024-04-01 11:02:03.000000 datacontract-cli-0.9.8/tests/test_examples_s3_json_multiple_models.py
--rw-r--r--   0 runner    (1001) docker     (127)      843 2024-04-01 11:02:03.000000 datacontract-cli-0.9.8/tests/test_examples_s3_json_remote.py
--rw-r--r--   0 runner    (1001) docker     (127)      810 2024-04-01 11:02:03.000000 datacontract-cli-0.9.8/tests/test_examples_snowflake.py
--rw-r--r--   0 runner    (1001) docker     (127)     1899 2024-04-01 11:02:03.000000 datacontract-cli-0.9.8/tests/test_export_avro.py
--rw-r--r--   0 runner    (1001) docker     (127)     4558 2024-04-01 11:02:03.000000 datacontract-cli-0.9.8/tests/test_export_avro_idl.py
--rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-04-01 11:02:03.000000 datacontract-cli-0.9.8/tests/test_export_dbt_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     2447 2024-04-01 11:02:03.000000 datacontract-cli-0.9.8/tests/test_export_dbt_sources.py
--rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-04-01 11:02:03.000000 datacontract-cli-0.9.8/tests/test_export_dbt_staging_sql.py
--rw-r--r--   0 runner    (1001) docker     (127)     7944 2024-04-01 11:02:03.000000 datacontract-cli-0.9.8/tests/test_export_great_expectations.py
--rw-r--r--   0 runner    (1001) docker     (127)     4195 2024-04-01 11:02:03.000000 datacontract-cli-0.9.8/tests/test_export_jsonschema.py
--rw-r--r--   0 runner    (1001) docker     (127)     2161 2024-04-01 11:02:03.000000 datacontract-cli-0.9.8/tests/test_export_odcs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-04-01 11:02:03.000000 datacontract-cli-0.9.8/tests/test_export_protobuf.py
--rw-r--r--   0 runner    (1001) docker     (127)     3465 2024-04-01 11:02:03.000000 datacontract-cli-0.9.8/tests/test_export_pydantic.py
--rw-r--r--   0 runner    (1001) docker     (127)     8403 2024-04-01 11:02:03.000000 datacontract-cli-0.9.8/tests/test_export_rdf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-04-01 11:02:03.000000 datacontract-cli-0.9.8/tests/test_export_sodacl.py
--rw-r--r--   0 runner    (1001) docker     (127)     1965 2024-04-01 11:02:03.000000 datacontract-cli-0.9.8/tests/test_export_sql.py
--rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-04-01 11:02:03.000000 datacontract-cli-0.9.8/tests/test_export_sql_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-04-01 11:02:03.000000 datacontract-cli-0.9.8/tests/test_export_terraform.py
--rw-r--r--   0 runner    (1001) docker     (127)     2176 2024-04-01 11:02:03.000000 datacontract-cli-0.9.8/tests/test_field_constraint_linter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-01 11:02:03.000000 datacontract-cli-0.9.8/tests/test_field_pattern_linter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-04-01 11:02:03.000000 datacontract-cli-0.9.8/tests/test_field_reference_linter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1712 2024-04-01 11:02:03.000000 datacontract-cli-0.9.8/tests/test_import_avro.py
--rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-04-01 11:02:03.000000 datacontract-cli-0.9.8/tests/test_import_sql.py
--rw-r--r--   0 runner    (1001) docker     (127)      753 2024-04-01 11:02:03.000000 datacontract-cli-0.9.8/tests/test_integration_datameshmanager.py
--rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-04-01 11:02:03.000000 datacontract-cli-0.9.8/tests/test_integration_opentelemetry.py
--rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-04-01 11:02:03.000000 datacontract-cli-0.9.8/tests/test_lint.py
--rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-04-01 11:02:03.000000 datacontract-cli-0.9.8/tests/test_notice_period_linter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-04-01 11:02:03.000000 datacontract-cli-0.9.8/tests/test_primary_field_linter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-04-01 11:02:03.000000 datacontract-cli-0.9.8/tests/test_quality_schema_linter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-04-01 11:02:03.000000 datacontract-cli-0.9.8/tests/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-01 11:02:03.000000 datacontract-cli-0.9.8/tests/test_web.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:17:09.784568 datacontract_cli-0.9.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     2210 2024-04-18 09:15:49.000000 datacontract_cli-0.9.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    61490 2024-04-18 09:17:09.784568 datacontract_cli-0.9.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    59582 2024-04-18 09:15:49.000000 datacontract_cli-0.9.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:17:09.764568 datacontract_cli-0.9.9/datacontract/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 09:15:49.000000 datacontract_cli-0.9.9/datacontract/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:17:09.764568 datacontract_cli-0.9.9/datacontract/breaking/
+-rw-r--r--   0 runner    (1001) docker     (127)    11719 2024-04-18 09:15:49.000000 datacontract_cli-0.9.9/datacontract/breaking/breaking.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2913 2024-04-18 09:15:49.000000 datacontract_cli-0.9.9/datacontract/breaking/breaking_rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10534 2024-04-18 09:15:49.000000 datacontract_cli-0.9.9/datacontract/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21809 2024-04-18 09:15:49.000000 datacontract_cli-0.9.9/datacontract/data_contract.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:17:09.764568 datacontract_cli-0.9.9/datacontract/engines/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 09:15:49.000000 datacontract_cli-0.9.9/datacontract/engines/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:17:09.768568 datacontract_cli-0.9.9/datacontract/engines/datacontract/
+-rw-r--r--   0 runner    (1001) docker     (127)     1565 2024-04-18 09:15:49.000000 datacontract_cli-0.9.9/datacontract/engines/datacontract/check_that_datacontract_contains_valid_servers_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-04-18 09:15:49.000000 datacontract_cli-0.9.9/datacontract/engines/datacontract/check_that_datacontract_file_exists.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-04-18 09:15:49.000000 datacontract_cli-0.9.9/datacontract/engines/datacontract/check_that_datacontract_str_is_valid.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:17:09.768568 datacontract_cli-0.9.9/datacontract/engines/fastjsonschema/
+-rw-r--r--   0 runner    (1001) docker     (127)     5754 2024-04-18 09:15:49.000000 datacontract_cli-0.9.9/datacontract/engines/fastjsonschema/check_jsonschema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:17:09.768568 datacontract_cli-0.9.9/datacontract/engines/fastjsonschema/s3/
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-04-18 09:15:49.000000 datacontract_cli-0.9.9/datacontract/engines/fastjsonschema/s3/s3_read_files.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:17:09.768568 datacontract_cli-0.9.9/datacontract/engines/soda/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 09:15:49.000000 datacontract_cli-0.9.9/datacontract/engines/soda/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6684 2024-04-18 09:15:49.000000 datacontract_cli-0.9.9/datacontract/engines/soda/check_soda_execute.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:17:09.768568 datacontract_cli-0.9.9/datacontract/engines/soda/connections/
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-04-18 09:15:49.000000 datacontract_cli-0.9.9/datacontract/engines/soda/connections/bigquery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-04-18 09:15:49.000000 datacontract_cli-0.9.9/datacontract/engines/soda/connections/dask.py
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-18 09:15:49.000000 datacontract_cli-0.9.9/datacontract/engines/soda/connections/databricks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3009 2024-04-18 09:15:49.000000 datacontract_cli-0.9.9/datacontract/engines/soda/connections/duckdb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5971 2024-04-18 09:15:49.000000 datacontract_cli-0.9.9/datacontract/engines/soda/connections/kafka.py
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-04-18 09:15:49.000000 datacontract_cli-0.9.9/datacontract/engines/soda/connections/postgres.py
+-rw-r--r--   0 runner    (1001) docker     (127)      719 2024-04-18 09:15:49.000000 datacontract_cli-0.9.9/datacontract/engines/soda/connections/snowflake.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:17:09.772568 datacontract_cli-0.9.9/datacontract/export/
+-rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-04-18 09:15:49.000000 datacontract_cli-0.9.9/datacontract/export/avro_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9582 2024-04-18 09:15:49.000000 datacontract_cli-0.9.9/datacontract/export/avro_idl_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-04-18 09:15:49.000000 datacontract_cli-0.9.9/datacontract/export/csv_type_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8549 2024-04-18 09:15:49.000000 datacontract_cli-0.9.9/datacontract/export/dbt_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4896 2024-04-18 09:15:49.000000 datacontract_cli-0.9.9/datacontract/export/great_expectations_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-04-18 09:15:49.000000 datacontract_cli-0.9.9/datacontract/export/html_export.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3153 2024-04-18 09:15:49.000000 datacontract_cli-0.9.9/datacontract/export/jsonschema_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-04-18 09:15:49.000000 datacontract_cli-0.9.9/datacontract/export/odcs_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2974 2024-04-18 09:15:49.000000 datacontract_cli-0.9.9/datacontract/export/protobuf_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5351 2024-04-18 09:15:49.000000 datacontract_cli-0.9.9/datacontract/export/pydantic_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6108 2024-04-18 09:15:49.000000 datacontract_cli-0.9.9/datacontract/export/rdf_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6744 2024-04-18 09:15:49.000000 datacontract_cli-0.9.9/datacontract/export/sodacl_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3754 2024-04-18 09:15:49.000000 datacontract_cli-0.9.9/datacontract/export/sql_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4627 2024-04-18 09:15:49.000000 datacontract_cli-0.9.9/datacontract/export/sql_type_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-04-18 09:15:49.000000 datacontract_cli-0.9.9/datacontract/export/terraform_converter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:17:09.772568 datacontract_cli-0.9.9/datacontract/imports/
+-rw-r--r--   0 runner    (1001) docker     (127)     4800 2024-04-18 09:15:49.000000 datacontract_cli-0.9.9/datacontract/imports/avro_importer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-04-18 09:15:49.000000 datacontract_cli-0.9.9/datacontract/imports/sql_importer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:17:09.772568 datacontract_cli-0.9.9/datacontract/init/
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-18 09:15:49.000000 datacontract_cli-0.9.9/datacontract/init/download_datacontract_file.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:17:09.772568 datacontract_cli-0.9.9/datacontract/integration/
+-rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-04-18 09:15:49.000000 datacontract_cli-0.9.9/datacontract/integration/publish_datamesh_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3830 2024-04-18 09:15:49.000000 datacontract_cli-0.9.9/datacontract/integration/publish_opentelemetry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:17:09.772568 datacontract_cli-0.9.9/datacontract/lint/
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-04-18 09:15:49.000000 datacontract_cli-0.9.9/datacontract/lint/files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5076 2024-04-18 09:15:49.000000 datacontract_cli-0.9.9/datacontract/lint/lint.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:17:09.772568 datacontract_cli-0.9.9/datacontract/lint/linters/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 09:15:49.000000 datacontract_cli-0.9.9/datacontract/lint/linters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-04-18 09:15:49.000000 datacontract_cli-0.9.9/datacontract/lint/linters/description_linter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3978 2024-04-18 09:15:49.000000 datacontract_cli-0.9.9/datacontract/lint/linters/example_model_linter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-04-18 09:15:49.000000 datacontract_cli-0.9.9/datacontract/lint/linters/field_pattern_linter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-04-18 09:15:49.000000 datacontract_cli-0.9.9/datacontract/lint/linters/field_reference_linter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2135 2024-04-18 09:15:49.000000 datacontract_cli-0.9.9/datacontract/lint/linters/notice_period_linter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-04-18 09:15:49.000000 datacontract_cli-0.9.9/datacontract/lint/linters/quality_schema_linter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4915 2024-04-18 09:15:49.000000 datacontract_cli-0.9.9/datacontract/lint/linters/valid_constraints_linter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6386 2024-04-18 09:15:49.000000 datacontract_cli-0.9.9/datacontract/lint/resolve.py
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-04-18 09:15:49.000000 datacontract_cli-0.9.9/datacontract/lint/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-04-18 09:15:49.000000 datacontract_cli-0.9.9/datacontract/lint/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:17:09.772568 datacontract_cli-0.9.9/datacontract/model/
+-rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-04-18 09:15:49.000000 datacontract_cli-0.9.9/datacontract/model/breaking_change.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3480 2024-04-18 09:15:49.000000 datacontract_cli-0.9.9/datacontract/model/data_contract_specification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-04-18 09:15:49.000000 datacontract_cli-0.9.9/datacontract/model/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2610 2024-04-18 09:15:49.000000 datacontract_cli-0.9.9/datacontract/model/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-04-18 09:15:49.000000 datacontract_cli-0.9.9/datacontract/web.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:17:09.784568 datacontract_cli-0.9.9/datacontract_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    61490 2024-04-18 09:17:09.000000 datacontract_cli-0.9.9/datacontract_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4411 2024-04-18 09:17:09.000000 datacontract_cli-0.9.9/datacontract_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 09:17:09.000000 datacontract_cli-0.9.9/datacontract_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-18 09:17:09.000000 datacontract_cli-0.9.9/datacontract_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      754 2024-04-18 09:17:09.000000 datacontract_cli-0.9.9/datacontract_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-18 09:17:09.000000 datacontract_cli-0.9.9/datacontract_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-04-18 09:15:49.000000 datacontract_cli-0.9.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 09:17:09.784568 datacontract_cli-0.9.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:17:09.784568 datacontract_cli-0.9.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5895 2024-04-18 09:15:49.000000 datacontract_cli-0.9.9/tests/test_breaking.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30873 2024-04-18 09:15:49.000000 datacontract_cli-0.9.9/tests/test_changelog.py
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-04-18 09:15:49.000000 datacontract_cli-0.9.9/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 09:15:49.000000 datacontract_cli-0.9.9/tests/test_description_linter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-04-18 09:15:49.000000 datacontract_cli-0.9.9/tests/test_documentation_linter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1884 2024-04-18 09:15:49.000000 datacontract_cli-0.9.9/tests/test_download_datacontract_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3356 2024-04-18 09:15:49.000000 datacontract_cli-0.9.9/tests/test_example_model_linter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-04-18 09:15:49.000000 datacontract_cli-0.9.9/tests/test_export_avro.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4558 2024-04-18 09:15:49.000000 datacontract_cli-0.9.9/tests/test_export_avro_idl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2256 2024-04-18 09:15:49.000000 datacontract_cli-0.9.9/tests/test_export_dbt_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2445 2024-04-18 09:15:49.000000 datacontract_cli-0.9.9/tests/test_export_dbt_sources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-04-18 09:15:49.000000 datacontract_cli-0.9.9/tests/test_export_dbt_staging_sql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9729 2024-04-18 09:15:49.000000 datacontract_cli-0.9.9/tests/test_export_great_expectations.py
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-04-18 09:15:49.000000 datacontract_cli-0.9.9/tests/test_export_html.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4191 2024-04-18 09:15:49.000000 datacontract_cli-0.9.9/tests/test_export_jsonschema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2159 2024-04-18 09:15:49.000000 datacontract_cli-0.9.9/tests/test_export_odcs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-04-18 09:15:49.000000 datacontract_cli-0.9.9/tests/test_export_protobuf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3227 2024-04-18 09:15:49.000000 datacontract_cli-0.9.9/tests/test_export_pydantic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8399 2024-04-18 09:15:49.000000 datacontract_cli-0.9.9/tests/test_export_rdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2669 2024-04-18 09:15:49.000000 datacontract_cli-0.9.9/tests/test_export_sodacl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2651 2024-04-18 09:15:49.000000 datacontract_cli-0.9.9/tests/test_export_sql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-04-18 09:15:49.000000 datacontract_cli-0.9.9/tests/test_export_sql_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2024-04-18 09:15:49.000000 datacontract_cli-0.9.9/tests/test_export_terraform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2176 2024-04-18 09:15:49.000000 datacontract_cli-0.9.9/tests/test_field_constraint_linter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-18 09:15:49.000000 datacontract_cli-0.9.9/tests/test_field_pattern_linter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-04-18 09:15:49.000000 datacontract_cli-0.9.9/tests/test_field_reference_linter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3799 2024-04-18 09:15:49.000000 datacontract_cli-0.9.9/tests/test_import_avro.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-04-18 09:15:49.000000 datacontract_cli-0.9.9/tests/test_import_sql.py
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2024-04-18 09:15:49.000000 datacontract_cli-0.9.9/tests/test_integration_datameshmanager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-04-18 09:15:49.000000 datacontract_cli-0.9.9/tests/test_integration_opentelemetry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-04-18 09:15:49.000000 datacontract_cli-0.9.9/tests/test_lint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-04-18 09:15:49.000000 datacontract_cli-0.9.9/tests/test_notice_period_linter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-04-18 09:15:49.000000 datacontract_cli-0.9.9/tests/test_quality_schema_linter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-04-18 09:15:49.000000 datacontract_cli-0.9.9/tests/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      946 2024-04-18 09:15:49.000000 datacontract_cli-0.9.9/tests/test_test_bigquery.py
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-04-18 09:15:49.000000 datacontract_cli-0.9.9/tests/test_test_databricks.py
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-04-18 09:15:49.000000 datacontract_cli-0.9.9/tests/test_test_examples_csv.py
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-18 09:15:49.000000 datacontract_cli-0.9.9/tests/test_test_examples_formats_valid.py
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-18 09:15:49.000000 datacontract_cli-0.9.9/tests/test_test_examples_inline.py
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-04-18 09:15:49.000000 datacontract_cli-0.9.9/tests/test_test_examples_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-04-18 09:15:49.000000 datacontract_cli-0.9.9/tests/test_test_examples_missing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-04-18 09:15:49.000000 datacontract_cli-0.9.9/tests/test_test_kafka.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-04-18 09:15:49.000000 datacontract_cli-0.9.9/tests/test_test_kafka_remote.py
+-rw-r--r--   0 runner    (1001) docker     (127)      650 2024-04-18 09:15:49.000000 datacontract_cli-0.9.9/tests/test_test_local_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-18 09:15:49.000000 datacontract_cli-0.9.9/tests/test_test_parquet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-04-18 09:15:49.000000 datacontract_cli-0.9.9/tests/test_test_postgres.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-04-18 09:15:49.000000 datacontract_cli-0.9.9/tests/test_test_s3_csv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-04-18 09:15:49.000000 datacontract_cli-0.9.9/tests/test_test_s3_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-04-18 09:15:49.000000 datacontract_cli-0.9.9/tests/test_test_s3_json_complex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1985 2024-04-18 09:15:49.000000 datacontract_cli-0.9.9/tests/test_test_s3_json_multiple_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-04-18 09:15:49.000000 datacontract_cli-0.9.9/tests/test_test_s3_json_remote.py
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-04-18 09:15:49.000000 datacontract_cli-0.9.9/tests/test_test_snowflake.py
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-18 09:15:49.000000 datacontract_cli-0.9.9/tests/test_web.py
```

### Comparing `datacontract-cli-0.9.8/LICENSE` & `datacontract_cli-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `datacontract-cli-0.9.8/PKG-INFO` & `datacontract_cli-0.9.9/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,53 +1,7 @@
-Metadata-Version: 2.1
-Name: datacontract-cli
-Version: 0.9.8
-Summary: Test data contracts
-Author-email: Jochen Christ <jochen.christ@innoq.com>, Stefan Negele <stefan.negele@innoq.com>
-Project-URL: Homepage, https://cli.datacontract.com
-Project-URL: Issues, https://github.com/datacontract/cli/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: typer[all]<0.13,>=0.9
-Requires-Dist: pydantic<2.7.0,>=2.5.3
-Requires-Dist: pyyaml~=6.0.1
-Requires-Dist: requests~=2.31.0
-Requires-Dist: fastapi==0.110.0
-Requires-Dist: fastparquet==2024.2.0
-Requires-Dist: python-multipart==0.0.9
-Requires-Dist: rich~=13.7.0
-Requires-Dist: simple-ddl-parser==1.0.4
-Requires-Dist: soda-core-bigquery<3.4.0,>=3.3.1
-Requires-Dist: soda-core-duckdb<3.4.0,>=3.3.1
-Requires-Dist: soda-core-postgres<3.4.0,>=3.3.1
-Requires-Dist: soda-core-snowflake<3.4.0,>=3.3.1
-Requires-Dist: soda-core-spark[databricks]<3.4.0,>=3.3.1
-Requires-Dist: soda-core-spark-df<3.4.0,>=3.3.1
-Requires-Dist: snowflake-connector-python[pandas]<3.8,>=3.6
-Requires-Dist: duckdb==0.10.1
-Requires-Dist: fastjsonschema~=2.19.1
-Requires-Dist: python-dotenv~=1.0.0
-Requires-Dist: s3fs==2024.3.1
-Requires-Dist: rdflib==7.0.0
-Requires-Dist: avro==1.11.3
-Requires-Dist: opentelemetry-exporter-otlp-proto-grpc~=1.16.0
-Requires-Dist: opentelemetry-exporter-otlp-proto-http~=1.16.0
-Provides-Extra: dev
-Requires-Dist: httpx==0.27.0; extra == "dev"
-Requires-Dist: ruff; extra == "dev"
-Requires-Dist: pytest; extra == "dev"
-Requires-Dist: testcontainers<4.0; extra == "dev"
-Requires-Dist: testcontainers-minio; extra == "dev"
-Requires-Dist: testcontainers-postgres; extra == "dev"
-Requires-Dist: testcontainers-kafka; extra == "dev"
-
 # Data Contract CLI
 
 <p>
   <a href="https://github.com/datacontract/cli/actions/workflows/ci.yaml?query=branch%3Amain">
     <img alt="Test Workflow" src="https://img.shields.io/github/actions/workflow/status/datacontract/cli/ci.yaml?branch=main"></a>
   <a href="https://github.com/datacontract/cli">
     <img alt="Stars" src="https://img.shields.io/github/stars/datacontract/cli" /></a>
@@ -55,29 +9,21 @@
 </p>
 
 The `datacontract` CLI is an open source command-line tool for working with [Data Contracts](https://datacontract.com/).
 It uses data contract YAML files to lint the data contract, connect to data sources and execute schema and quality tests, detect breaking changes, and export to different formats. The tool is written in Python. It can be used as a standalone CLI tool, in a CI/CD pipeline, or directly as a Python library.
 
 ![Main features of the Data Contract CLI](datacontractcli.png)
 
-<div align="center">
-  <a href="https://www.youtube.com/watch?v=B1dixhgO2vQ">
- <img 
-  src="https://img.youtube.com/vi/B1dixhgO2vQ/0.jpg" 
-  alt="Demo of Data Contract CLI" 
-  style="width:100%;">
-  </a>
-</div>
 
 ## Getting started
 
-Let's look at this data contract:
+Let's look at this data contract:  
 [https://datacontract.com/examples/orders-latest/datacontract.yaml](https://datacontract.com/examples/orders-latest/datacontract.yaml)
 
-We have a _servers_ section with endpoint details to the S3 bucket, _models_ for the structure of the data, and _quality_ attributes that describe the expected freshness and number of rows.
+We have a _servers_ section with endpoint details to the S3 bucket, _models_ for the structure of the data, _servicelevels_ and _quality_ attributes that describe the expected freshness and number of rows.
 
 This data contract contains all information to connect to S3 and check that the actual data meets the defined schema and quality requirements. We can use this information to test if the actual data set in S3 is compliant to the data contract.
 
 Let's use [pip](https://pip.pypa.io/en/stable/getting-started/) to install the CLI (or use the [Docker image](#docker), if you prefer).
 ```bash
 $ python3 -m pip install datacontract-cli
 ```
@@ -116,14 +62,39 @@
 │ passed │ Check that unique field lines_item_id has no duplicate values       │ line_items.lines_item_id      │         │
 ╰────────┴─────────────────────────────────────────────────────────────────────┴───────────────────────────────┴─────────╯
 🟢 data contract is valid. Run 22 checks. Took 6.739514 seconds.
 ```
 
 Voilà, the CLI tested that the _datacontract.yaml_ itself is valid, all records comply with the schema, and all quality attributes are met.
 
+We can also use the datacontract.yaml to export in many [formats](#format), e.g., to SQL:
+
+```bash
+$ datacontract export --format sql https://datacontract.com/examples/orders-latest/datacontract.yaml
+
+# returns:
+-- Data Contract: urn:datacontract:checkout:orders-latest
+-- SQL Dialect: snowflake
+CREATE TABLE orders (
+  order_id TEXT not null primary key,
+  order_timestamp TIMESTAMP_TZ not null,
+  order_total NUMBER not null,
+  customer_id TEXT,
+  customer_email_address TEXT not null,
+  processed_timestamp TIMESTAMP_TZ not null
+);
+CREATE TABLE line_items (
+  lines_item_id TEXT not null primary key,
+  order_id TEXT,
+  sku TEXT
+);
+```
+
+Or generate this [HTML page](https://datacontract.com/examples/orders-latest/datacontract.html).
+
 ## Usage
 
 ```bash
 # create a new data contract from example and write it to datacontract.yaml
 $ datacontract init datacontract.yaml
 
 # lint the datacontract.yaml
@@ -131,90 +102,41 @@
 
 # execute schema and quality checks
 $ datacontract test datacontract.yaml
 
 # execute schema and quality checks on the examples within the contract
 $ datacontract test --examples datacontract.yaml
 
-# find differences between to data contracts (Coming Soon)
+# export data contract as html (other formats: avro, dbt, dbt-sources, dbt-staging-sql, jsonschema, odcs, rdf, sql, sodacl, terraform, ...)
+$ datacontract export --format html datacontract.yaml > datacontract.html
+
+# import avro (other formats: sql, ...)
+$ datacontract import --format avro --source avro_schema.avsc
+
+# find differences between to data contracts
 $ datacontract diff datacontract-v1.yaml datacontract-v2.yaml
 
 # find differences between to data contracts categorized into error, warning, and info.
 $ datacontract changelog datacontract-v1.yaml datacontract-v2.yaml
 
 # fail pipeline on breaking changes. Uses changelog internally and showing only error and warning.
 $ datacontract breaking datacontract-v1.yaml datacontract-v2.yaml
-
-# export model as jsonschema (other formats: avro, dbt, dbt-sources, dbt-staging-sql, jsonschema, odcs, rdf, sql (coming soon), sodacl, terraform)
-$ datacontract export --format jsonschema datacontract.yaml
-
-# import sql
-$ datacontract import --format sql --source my_ddl.sql
-
-# import avro
-$ datacontract import --format avro --source avro_schema.avsc
 ```
 
 ## Programmatic (Python)
 ```python
 from datacontract.data_contract import DataContract
 
 data_contract = DataContract(data_contract_file="datacontract.yaml")
 run = data_contract.test()
 if not run.has_passed():
     print("Data quality validation failed.")
     # Abort pipeline, alert, or take corrective actions...
 ```
 
-## Integrations
-
-
-| Integration       | Option                       | Description                                                                                           |
-|-------------------|------------------------------|-------------------------------------------------------------------------------------------------------|
-| Data Mesh Manager | `--publish`                  | Push full results to the [Data Mesh Manager API](https://api.datamesh-manager.com/swagger/index.html) |
-| OpenTelemetry     | `--publish-to-opentelemetry` | Push result as gauge metrics (logs are planned)                                                       |
-
-### Integration with Data Mesh Manager
-
-If you use [Data Mesh Manager](https://datamesh-manager.com/), you can use the data contract URL and append the `--publish` option to send and display the test results. Set an environment variable for your API key.
-
-```bash
-# Fetch current data contract, execute tests on production, and publish result to data mesh manager
-$ EXPORT DATAMESH_MANAGER_API_KEY=xxx
-$ datacontract test https://demo.datamesh-manager.com/demo279750347121/datacontracts/4df9d6ee-e55d-4088-9598-b635b2fdcbbc/datacontract.yaml --server production --publish
-```
-
-### Integration with OpenTelemetry
-
-If you use OpenTelemetry, you can use the data contract URL and append the `--publish-to-opentelemetry` option to send the test results to your OLTP-compatible instance, e.g., Prometheus.
-
-The metric name is "datacontract.cli.test.result" and it uses the following encoding for the result:
-
-| datacontract.cli.test.result | Description                           |
-|-------|---------------------------------------|
-| 0     | test run passed, no warnings          |
-| 1     | test run has warnings                 |
-| 2     | test run failed                       |
-| 3     | test run not possible due to an error |
-| 4     | test status unknown                   |
-
-
-```bash
-# Fetch current data contract, execute tests on production, and publish result to open telemetry
-$ EXPORT OTEL_SERVICE_NAME=datacontract-cli
-$ EXPORT OTEL_EXPORTER_OTLP_ENDPOINT=https://YOUR_ID.apm.westeurope.azure.elastic-cloud.com:443
-$ EXPORT OTEL_EXPORTER_OTLP_HEADERS=Authorization=Bearer%20secret # Optional, when using SaaS Products
-$ EXPORT OTEL_EXPORTER_OTLP_PROTOCOL=http/protobuf # Optional, default is http/protobuf - use value grpc to use the gRPC protocol instead
-# Send to OpenTelemetry
-$ datacontract test https://demo.datamesh-manager.com/demo279750347121/datacontracts/4df9d6ee-e55d-4088-9598-b635b2fdcbbc/datacontract.yaml --server production --publish-to-opentelemetry
-```
-
-Current limitations:
-- currently, only ConsoleExporter and OTLP Exporter
-- Metrics only, no logs yet (but loosely planned)
 
 ## Installation
 
 Choose the most appropriate installation method for your needs:
 
 ### pip
 Python 3.11 recommended.
@@ -241,44 +163,128 @@
 
 ```bash
 alias datacontract='docker run --rm -v "${PWD}:/home/datacontract" datacontract/cli:latest'
 ```
 
 ## Documentation
 
-### Tests
+Commands
+
+- [init](#init)
+- [lint](#lint)
+- [test](#test)
+- [export](#export)
+- [import](#import)
+- [breaking](#breaking)
+- [changelog](#changelog)
+- [diff](#diff)
+
+### init
+
+```                                                                                                
+ Usage: datacontract init [OPTIONS] [LOCATION]                                                  
+                                                                                                
+ Download a datacontract.yaml template and write it to file.                                    
+                                                                                                
+╭─ Arguments ──────────────────────────────────────────────────────────────────────────────────╮
+│   location      [LOCATION]  The location (url or path) of the data contract yaml to create.  │
+│                             [default: datacontract.yaml]                                     │
+╰──────────────────────────────────────────────────────────────────────────────────────────────╯
+╭─ Options ────────────────────────────────────────────────────────────────────────────────────╮
+│ --template                       TEXT  URL of a template or data contract                    │
+│                                        [default:                                             │
+│                                        https://datacontract.com/datacontract.init.yaml]      │
+│ --overwrite    --no-overwrite          Replace the existing datacontract.yaml                │
+│                                        [default: no-overwrite]                               │
+│ --help                                 Show this message and exit.                           │
+╰──────────────────────────────────────────────────────────────────────────────────────────────╯
+```
+
+### lint
+
+```
+ Usage: datacontract lint [OPTIONS] [LOCATION]                                                                                     
+                                                                                                                                   
+ Validate that the datacontract.yaml is correctly formatted.                                                                       
+                                                                                                                                   
+╭─ Arguments ─────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╮
+│   location      [LOCATION]  The location (url or path) of the data contract yaml. [default: datacontract.yaml]                  │
+╰─────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
+╭─ Options ───────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╮
+│ --schema        TEXT  The location (url or path) of the Data Contract Specification JSON Schema                                 │
+│                       [default: https://datacontract.com/datacontract.schema.json]                                              │
+│ --help                Show this message and exit.                                                                               │
+╰─────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
+```
+
+### test
+
+```
+ Usage: datacontract test [OPTIONS] [LOCATION]                                                                                     
+                                                                                                                                   
+ Run schema and quality tests on configured servers.                                                                               
+                                                                                                                                   
+╭─ Arguments ─────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╮
+│   location      [LOCATION]  The location (url or path) of the data contract yaml. [default: datacontract.yaml]                  │
+╰─────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
+╭─ Options ───────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╮
+│ --schema                                                       TEXT  The location (url or path) of the Data Contract            │
+│                                                                      Specification JSON Schema                                  │
+│                                                                      [default:                                                  │
+│                                                                      https://datacontract.com/datacontract.schema.json]         │
+│ --server                                                       TEXT  The server configuration to run the schema and quality     │
+│                                                                      tests. Use the key of the server object in the data        │
+│                                                                      contract yaml file to refer to a server, e.g.,             │
+│                                                                      `production`, or `all` for all servers (default).          │
+│                                                                      [default: all]                                             │
+│ --examples                    --no-examples                          Run the schema and quality tests on the example data       │
+│                                                                      within the data contract.                                  │
+│                                                                      [default: no-examples]                                     │
+│ --publish                                                      TEXT  The url to publish the results after the test              │
+│                                                                      [default: None]                                            │
+│ --publish-to-opentelemetry    --no-publish-to-opentelemetry          Publish the results to opentelemetry. Use environment      │
+│                                                                      variables to configure the OTLP endpoint, headers, etc.    │
+│                                                                      [default: no-publish-to-opentelemetry]                     │
+│ --logs                        --no-logs                              Print logs [default: no-logs]                              │
+│ --help                                                               Show this message and exit.                                │
+╰─────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
+```
 
 Data Contract CLI can connect to data sources and run schema and quality tests to verify that the data contract is valid.
 
 ```bash
 $ datacontract test --server production datacontract.yaml
 ```
 
 To connect to the databases the `server` block in the datacontract.yaml is used to set up the connection. In addition, credentials, such as username and passwords, may be defined with environment variables.
 
 The application uses different engines, based on the server `type`.
+Internally, it connects with DuckDB, Spark, or a native connection and executes the most tests with soda-core and fastjsonschema. 
+Credentials are read from the environment variables.
+
+Supported server types:
 
-| Type         | Format     | Description                                                               | Status      | Engines                             |
-|--------------|------------|---------------------------------------------------------------------------|-------------|-------------------------------------|
-| `s3`         | `parquet`  | Works for any S3-compliant endpoint., e.g., AWS S3, GCS, MinIO, Ceph, ... | ✅           | soda-core-duckdb                    |
-| `s3`         | `json`     | Support for `new_line` delimited JSON files and one JSON record per file. | ✅           | fastjsonschema<br> soda-core-duckdb |
-| `s3`         | `csv`      |                                                                           | ✅           | soda-core-duckdb                    |
-| `s3`         | `delta`    |                                                                           | Coming soon | TBD                                 |
-| `postgres`   | n/a        |                                                                           | ✅           | soda-core-postgres                  |
-| `snowflake`  | n/a        |                                                                           | ✅           | soda-core-snowflake                 |
-| `bigquery`   | n/a        |                                                                           | ✅           | soda-core-bigquery                  |
-| `redshift`   | n/a        |                                                                           | Coming soon | TBD                                 |
-| `databricks` | n/a        | Support for Databricks SQL with Unity catalog and Hive metastore.         | ✅           | soda-core-spark                     |
-| `databricks` | n/a        | Support for Spark for programmatic use in Notebooks.                      | ✅           | soda-core-spark-df                  |
-| `kafka`      | `json`     | Experimental.                                                             | ✅           | pyspark<br>soda-core-spark-df       |
-| `kafka`      | `avro`     |                                                                           | Coming soon | TBD                                 |
-| `kafka`      | `protobuf` |                                                                           | Coming soon | TBD                                 |
-| `local`      | `parquet`  |                                                                           | ✅           | soda-core-duckdb                    |
-| `local`      | `json`     | Support for `new_line` delimited JSON files and one JSON record per file. | ✅           | fastjsonschema<br> soda-core-duckdb |
-| `local`      | `csv`      |                                                                           | ✅           | soda-core-duckdb                    |
+| Type         | Format     | Status                                                             |
+|--------------|------------|--------------------------------------------------------------------|
+| `s3`         | `parquet`  | ✅                                                                  |
+| `s3`         | `json`     | ✅                                                                  |
+| `s3`         | `csv`      | ✅                                                                  |
+| `s3`         | `delta`    | Coming soon ([#24](https://github.com/datacontract/cli/issues/24)) |
+| `s3`         | `iceberg`  | Coming soon                                                        |
+| `postgres`   | n/a        | ✅                                                                  |
+| `snowflake`  | n/a        | ✅                                                                  |
+| `bigquery`   | n/a        | ✅                                                                  |
+| `redshift`   | n/a        | Coming soon                                                        |
+| `databricks` | n/a        | ✅                                                                  |
+| `kafka`      | `json`     | ✅                                                                  |
+| `kafka`      | `avro`     | Coming soon                                                        |
+| `kafka`      | `protobuf` | Coming soon                                                        |
+| `local`      | `parquet`  | ✅                                                                  |
+| `local`      | `json`     | ✅                                                                  |
+| `local`      | `csv`      | ✅                                                                  |
 
 Feel free to create an issue, if you need support for an additional type.
 
 ### S3
 
 Data Contract CLI can test data that is stored in S3 buckets or any S3-compliant endpoints in various formats.
 
@@ -486,25 +492,54 @@
 | Environment Variable               | Example | Description                 |
 |------------------------------------|---------|-----------------------------|
 | `DATACONTRACT_KAFKA_SASL_USERNAME` | `xxx`   | The SASL username (key).    |
 | `DATACONTRACT_KAFKA_SASL_PASSWORD` | `xxx`   | The SASL password (secret). |
 
 
 
-### Exports
+### export
+
+```
+ Usage: datacontract export [OPTIONS] [LOCATION]                                                                                                                           
+                                                                                                                                                                           
+ Convert data contract to a specific format. console.prints to stdout.                                                                                                     
+                                                                                                                                                                           
+╭─ Arguments ─────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╮
+│   location      [LOCATION]  The location (url or path) of the data contract yaml. [default: datacontract.yaml]                                                          │
+╰─────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
+╭─ Options ───────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╮
+│ *  --format        [html|jsonschema|pydantic-model|sodacl|dbt|dbt-sources|dbt-staging-sql|odcs|rd  The export format. [default: None] [required]                             │
+│                    f|avro|protobuf|great-expectations|terraform|avro-idl|sql|sql-query]                                                                                 │
+│    --server        TEXT                                                                       The server name to export. [default: None]                                │
+│    --model         TEXT                                                                       Use the key of the model in the data contract yaml file to refer to a     │
+│                                                                                               model, e.g., `orders`, or `all` for all models (default).                 │
+│                                                                                               [default: all]                                                            │
+│    --help                                                                                     Show this message and exit.                                               │
+╰─────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
+╭─ RDF Options ───────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╮
+│ --rdf-base        TEXT  [rdf] The base URI used to generate the RDF graph. [default: None]                                                                              │
+╰─────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
+╭─ SQL Options ───────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╮
+│ --sql-server-type        TEXT  [sql] The server type to determine the sql dialect. By default, it uses 'auto' to automatically detect the sql dialect via the specified │
+│                                servers in the data contract.                                                                                                            │
+│                                [default: auto]                                                                                                                          │
+╰─────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
+
+```
 
 ```bash
-# Example export to dbt model
-datacontract export --format dbt
+# Example export data contract as HTML
+datacontract export --format html > datacontract.html
 ```
 
 Available export options:
 
 | Type                 | Description                                             | Status |
 |----------------------|---------------------------------------------------------|--------|
+| `html`               | Export to HTML                                          | ✅      | 
 | `jsonschema`         | Export to JSON Schema                                   | ✅      | 
 | `odcs`               | Export to Open Data Contract Standard (ODCS)            | ✅      | 
 | `sodacl`             | Export to SodaCL quality checks in YAML format          | ✅      |
 | `dbt`                | Export to dbt models in YAML format                     | ✅      |
 | `dbt-sources`        | Export to dbt sources in YAML format                    | ✅      |
 | `dbt-staging-sql`    | Export to dbt staging SQL models                        | ✅      |
 | `rdf`                | Export data contract to RDF representation in N3 format | ✅      |
@@ -512,23 +547,25 @@
 | `protobuf`           | Export to Protobuf                                      | ✅      |
 | `terraform`          | Export to terraform resources                           | ✅      |
 | `sql`                | Export to SQL DDL                                       | ✅      |
 | `sql-query`          | Export to SQL Query                                     | ✅      |
 | `great-expectations` | Export to Great Expectations Suites in JSON Format      | ✅      |
 | `bigquery`           | Export to BigQuery Schemas                              | TBD    |
 | `pydantic`           | Export to pydantic models                               | TBD    |
-| `html`               | Export to HTML page                                     | TBD    |
 | Missing something?   | Please create an issue on GitHub                        | TBD    |
 
 #### Great Expectations
+
 The export function transforms a specified data contract into a comprehensive Great Expectations JSON suite. 
 If the contract includes multiple models, you need to specify the names of the model you wish to export.
+
 ```shell
 datacontract  export datacontract.yaml --format great-expectations --model orders 
 ```
+
 The export creates a list of expectations by utilizing:
 
 - The data from the Model definition with a fixed mapping
 - The expectations provided in the quality field for each model (find here the expectations gallery https://greatexpectations.io/expectations/)
 
 #### RDF
 
@@ -550,16 +587,29 @@
 - Store data contracts inside a knowledge graph
 - Enhance a semantic search to find and retrieve data contracts
 - Linking model elements to already established ontologies and knowledge
 - Using full power of OWL to reason about the graph structure of data contracts
 - Apply graph algorithms on multiple data contracts (Find similar data contracts, find "gatekeeper"
 data products, find the true domain owner of a field attribute)
 
-### Imports
+### import
+
+```
+ Usage: datacontract import [OPTIONS]                                                                              
+                                                                                                                   
+ Create a data contract from the given source file. Prints to stdout.                                              
+                                                                                                                   
+╭─ Options ───────────────────────────────────────────────────────────────────────────────────────────────────────╮
+│ *  --format        [sql|avro]  The format of the source file. [default: None] [required]                        │
+│ *  --source        TEXT        The path to the file that should be imported. [default: None] [required]         │
+│    --help                      Show this message and exit.                                                      │
+╰─────────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
+```
 
+Example: 
 ```bash
 # Example import from SQL DDL
 datacontract import --format sql --source my_ddl.sql
 ```
 
 Available import options:
 
@@ -570,14 +620,111 @@
 | `protobuf`         | Import from Protobuf schemas                   | TBD     |
 | `jsonschema`       | Import from JSON Schemas                       | TBD     |
 | `bigquery`         | Import from BigQuery Schemas                   | TBD     |
 | `dbt`              | Import from dbt models                         | TBD     |
 | `odcs`             | Import from Open Data Contract Standard (ODCS) | TBD     |
 | Missing something? | Please create an issue on GitHub               | TBD     |
 
+
+### breaking
+
+```
+ Usage: datacontract breaking [OPTIONS] LOCATION_OLD LOCATION_NEW                                                            
+                                                                                                                             
+ Identifies breaking changes between data contracts. Prints to stdout.                                                       
+                                                                                                                             
+╭─ Arguments ───────────────────────────────────────────────────────────────────────────────────────────────────────────────╮
+│ *    location_old      TEXT  The location (url or path) of the old data contract yaml. [default: None] [required]         │
+│ *    location_new      TEXT  The location (url or path) of the new data contract yaml. [default: None] [required]         │
+╰───────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
+╭─ Options ─────────────────────────────────────────────────────────────────────────────────────────────────────────────────╮
+│ --help          Show this message and exit.                                                                               │
+╰───────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
+```
+
+### changelog
+
+```
+ Usage: datacontract changelog [OPTIONS] LOCATION_OLD LOCATION_NEW                                                           
+                                                                                                                             
+ Generate a changelog between data contracts. Prints to stdout.                                                              
+                                                                                                                             
+╭─ Arguments ───────────────────────────────────────────────────────────────────────────────────────────────────────────────╮
+│ *    location_old      TEXT  The location (url or path) of the old data contract yaml. [default: None] [required]         │
+│ *    location_new      TEXT  The location (url or path) of the new data contract yaml. [default: None] [required]         │
+╰───────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
+╭─ Options ─────────────────────────────────────────────────────────────────────────────────────────────────────────────────╮
+│ --help          Show this message and exit.                                                                               │
+╰───────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
+```
+
+### diff
+
+```
+ Usage: datacontract diff [OPTIONS] LOCATION_OLD LOCATION_NEW                                                                
+                                                                                                                             
+ PLACEHOLDER. Currently works as 'changelog' does.                                                                           
+                                                                                                                             
+╭─ Arguments ───────────────────────────────────────────────────────────────────────────────────────────────────────────────╮
+│ *    location_old      TEXT  The location (url or path) of the old data contract yaml. [default: None] [required]         │
+│ *    location_new      TEXT  The location (url or path) of the new data contract yaml. [default: None] [required]         │
+╰───────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
+╭─ Options ─────────────────────────────────────────────────────────────────────────────────────────────────────────────────╮
+│ --help          Show this message and exit.                                                                               │
+╰───────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
+```
+
+
+## Integrations
+
+| Integration       | Option                       | Description                                                                                           |
+|-------------------|------------------------------|-------------------------------------------------------------------------------------------------------|
+| Data Mesh Manager | `--publish`                  | Push full results to the [Data Mesh Manager API](https://api.datamesh-manager.com/swagger/index.html) |
+| OpenTelemetry     | `--publish-to-opentelemetry` | Push result as gauge metrics                                                                          |
+
+### Integration with Data Mesh Manager
+
+If you use [Data Mesh Manager](https://datamesh-manager.com/), you can use the data contract URL and append the `--publish` option to send and display the test results. Set an environment variable for your API key.
+
+```bash
+# Fetch current data contract, execute tests on production, and publish result to data mesh manager
+$ EXPORT DATAMESH_MANAGER_API_KEY=xxx
+$ datacontract test https://demo.datamesh-manager.com/demo279750347121/datacontracts/4df9d6ee-e55d-4088-9598-b635b2fdcbbc/datacontract.yaml --server production --publish
+```
+
+### Integration with OpenTelemetry
+
+If you use OpenTelemetry, you can use the data contract URL and append the `--publish-to-opentelemetry` option to send the test results to your OLTP-compatible instance, e.g., Prometheus.
+
+The metric name is "datacontract.cli.test.result" and it uses the following encoding for the result:
+
+| datacontract.cli.test.result | Description                           |
+|-------|---------------------------------------|
+| 0     | test run passed, no warnings          |
+| 1     | test run has warnings                 |
+| 2     | test run failed                       |
+| 3     | test run not possible due to an error |
+| 4     | test status unknown                   |
+
+
+```bash
+# Fetch current data contract, execute tests on production, and publish result to open telemetry
+$ EXPORT OTEL_SERVICE_NAME=datacontract-cli
+$ EXPORT OTEL_EXPORTER_OTLP_ENDPOINT=https://YOUR_ID.apm.westeurope.azure.elastic-cloud.com:443
+$ EXPORT OTEL_EXPORTER_OTLP_HEADERS=Authorization=Bearer%20secret # Optional, when using SaaS Products
+$ EXPORT OTEL_EXPORTER_OTLP_PROTOCOL=http/protobuf # Optional, default is http/protobuf - use value grpc to use the gRPC protocol instead
+# Send to OpenTelemetry
+$ datacontract test https://demo.datamesh-manager.com/demo279750347121/datacontracts/4df9d6ee-e55d-4088-9598-b635b2fdcbbc/datacontract.yaml --server production --publish-to-opentelemetry
+```
+
+Current limitations:
+- currently, only ConsoleExporter and OTLP Exporter
+- Metrics only, no logs yet (but loosely planned)
+
+
 ## Best Practices
 
 We share best practices in using the Data Contract CLI.
 
 ### Data-first Approach
 
 Create a data contract based on the actual data. This is the fastest way to get started and to get feedback from the data consumers.
@@ -693,33 +840,48 @@
 pip install --upgrade pip setuptools wheel
 pip install -e '.[dev]'
 ruff check --fix
 ruff format --check
 pytest
 ```
 
-Release
+
+### Docker Build
 
 ```bash
-git tag v0.9.0
-git push origin v0.9.0
-python3 -m pip install --upgrade build twine
-rm -r dist/
-python3 -m build
-# for now only test.pypi.org
-python3 -m twine upload --repository testpypi dist/*
+docker build -t datacontract/cli .
+docker run --rm -v ${PWD}:/home/datacontract datacontract/cli
 ```
 
-Docker Build
+#### Docker compose integration
+
+We've included a [docker-compose.yml](./docker-compose.yml) configuration to simplify the build, test, and deployment of the image.
+
+##### Building the Image with Docker Compose
+
+To build the Docker image using Docker Compose, run the following command:
 
 ```bash
-docker build -t datacontract/cli .
-docker run --rm -v ${PWD}:/home/datacontract datacontract/cli
+docker compose build
 ```
 
+This command utilizes the `docker-compose.yml` to build the image, leveraging predefined settings such as the build context and Dockerfile location. This approach streamlines the image creation process, avoiding the need for manual build specifications each time.
+
+#### Testing the Image
+
+After building the image, you can test it directly with Docker Compose:
+
+```bash
+docker compose run --rm datacontract --version
+```
+
+This command runs the container momentarily to check the version of the `datacontract` CLI. The `--rm` flag ensures that the container is automatically removed after the command executes, keeping your environment clean.
+
+
+
 ## Release Steps
 
 1. Update the version in `pyproject.toml`
 2. Have a look at the `CHANGELOG.md`
 3. Create release commit manually
 4. Execute `./release`
 5. Wait until GitHub Release is created
```

#### html2text {}

```diff
@@ -1,56 +1,29 @@
-Metadata-Version: 2.1 Name: datacontract-cli Version: 0.9.8 Summary: Test data
-contracts Author-email: Jochen Christ
-innoq.com>, Stefan Negele
-innoq.com> Project-URL: Homepage, https://cli.datacontract.com Project-URL:
-Issues, https://github.com/datacontract/cli/issues Classifier: Programming
-Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent Requires-Python: >=3.10
-Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
-typer[all]<0.13,>=0.9 Requires-Dist: pydantic<2.7.0,>=2.5.3 Requires-Dist:
-pyyaml~=6.0.1 Requires-Dist: requests~=2.31.0 Requires-Dist: fastapi==0.110.0
-Requires-Dist: fastparquet==2024.2.0 Requires-Dist: python-multipart==0.0.9
-Requires-Dist: rich~=13.7.0 Requires-Dist: simple-ddl-parser==1.0.4 Requires-
-Dist: soda-core-bigquery<3.4.0,>=3.3.1 Requires-Dist: soda-core-
-duckdb<3.4.0,>=3.3.1 Requires-Dist: soda-core-postgres<3.4.0,>=3.3.1 Requires-
-Dist: soda-core-snowflake<3.4.0,>=3.3.1 Requires-Dist: soda-core-spark
-[databricks]<3.4.0,>=3.3.1 Requires-Dist: soda-core-spark-df<3.4.0,>=3.3.1
-Requires-Dist: snowflake-connector-python[pandas]<3.8,>=3.6 Requires-Dist:
-duckdb==0.10.1 Requires-Dist: fastjsonschema~=2.19.1 Requires-Dist: python-
-dotenv~=1.0.0 Requires-Dist: s3fs==2024.3.1 Requires-Dist: rdflib==7.0.0
-Requires-Dist: avro==1.11.3 Requires-Dist: opentelemetry-exporter-otlp-proto-
-grpc~=1.16.0 Requires-Dist: opentelemetry-exporter-otlp-proto-http~=1.16.0
-Provides-Extra: dev Requires-Dist: httpx==0.27.0; extra == "dev" Requires-Dist:
-ruff; extra == "dev" Requires-Dist: pytest; extra == "dev" Requires-Dist:
-testcontainers<4.0; extra == "dev" Requires-Dist: testcontainers-minio; extra
-== "dev" Requires-Dist: testcontainers-postgres; extra == "dev" Requires-Dist:
-testcontainers-kafka; extra == "dev" # Data Contract CLI
+# Data Contract CLI
 _[_T_e_s_t_ _W_o_r_k_f_l_o_w_]_[_S_t_a_r_s_]_[_S_l_a_c_k_ _S_t_a_t_u_s_]
 The `datacontract` CLI is an open source command-line tool for working with
 [Data Contracts](https://datacontract.com/). It uses data contract YAML files
 to lint the data contract, connect to data sources and execute schema and
 quality tests, detect breaking changes, and export to different formats. The
 tool is written in Python. It can be used as a standalone CLI tool, in a CI/CD
 pipeline, or directly as a Python library. ![Main features of the Data Contract
-CLI](datacontractcli.png)
-                          _[_D_e_m_o_ _o_f_ _D_a_t_a_ _C_o_n_t_r_a_c_t_ _C_L_I_]
-## Getting started Let's look at this data contract: [https://datacontract.com/
-examples/orders-latest/datacontract.yaml](https://datacontract.com/examples/
-orders-latest/datacontract.yaml) We have a _servers_ section with endpoint
-details to the S3 bucket, _models_ for the structure of the data, and _quality_
-attributes that describe the expected freshness and number of rows. This data
-contract contains all information to connect to S3 and check that the actual
-data meets the defined schema and quality requirements. We can use this
-information to test if the actual data set in S3 is compliant to the data
-contract. Let's use [pip](https://pip.pypa.io/en/stable/getting-started/) to
-install the CLI (or use the [Docker image](#docker), if you prefer). ```bash $
-python3 -m pip install datacontract-cli ``` We run the tests: ```bash $
-datacontract test https://datacontract.com/examples/orders-latest/
-datacontract.yaml # returns: Testing https://datacontract.com/examples/orders-
-latest/datacontract.yaml
+CLI](datacontractcli.png) ## Getting started Let's look at this data contract:
+[https://datacontract.com/examples/orders-latest/datacontract.yaml](https://
+datacontract.com/examples/orders-latest/datacontract.yaml) We have a _servers_
+section with endpoint details to the S3 bucket, _models_ for the structure of
+the data, _servicelevels_ and _quality_ attributes that describe the expected
+freshness and number of rows. This data contract contains all information to
+connect to S3 and check that the actual data meets the defined schema and
+quality requirements. We can use this information to test if the actual data
+set in S3 is compliant to the data contract. Let's use [pip](https://
+pip.pypa.io/en/stable/getting-started/) to install the CLI (or use the [Docker
+image](#docker), if you prefer). ```bash $ python3 -m pip install datacontract-
+cli ``` We run the tests: ```bash $ datacontract test https://datacontract.com/
+examples/orders-latest/datacontract.yaml # returns: Testing https://
+datacontract.com/examples/orders-latest/datacontract.yaml
 â­âââââââââ¬ââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ¬ââââââââââââââââââââââââââââââââ¬ââââââââââ®
 â Result â Check â Field â Details â
 ââââââââââ¼ââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ¼ââââââââââââââââââââââââââââââââ¼ââââââââââ¤
 â passed â Check that JSON has valid schema â orders â â â passed
 â Check that JSON has valid schema â line_items â â â passed â
 Check that field order_id is present â orders â â â passed â Check
 that field order_timestamp is present â orders â â â passed â Check
@@ -74,111 +47,130 @@
 row_count >= 5000 â line_items â â â passed â Check that required
 field lines_item_id has no null values â line_items.lines_item_id â â â
 passed â Check that unique field lines_item_id has no duplicate values â
 line_items.lines_item_id â â
 â°âââââââââ´ââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ´ââââââââââââââââââââââââââââââââ´ââââââââââ¯
 ð¢ data contract is valid. Run 22 checks. Took 6.739514 seconds. ``` VoilÃ ,
 the CLI tested that the _datacontract.yaml_ itself is valid, all records comply
-with the schema, and all quality attributes are met. ## Usage ```bash # create
-a new data contract from example and write it to datacontract.yaml $
-datacontract init datacontract.yaml # lint the datacontract.yaml $ datacontract
-lint datacontract.yaml # execute schema and quality checks $ datacontract test
-datacontract.yaml # execute schema and quality checks on the examples within
-the contract $ datacontract test --examples datacontract.yaml # find
-differences between to data contracts (Coming Soon) $ datacontract diff
-datacontract-v1.yaml datacontract-v2.yaml # find differences between to data
-contracts categorized into error, warning, and info. $ datacontract changelog
-datacontract-v1.yaml datacontract-v2.yaml # fail pipeline on breaking changes.
-Uses changelog internally and showing only error and warning. $ datacontract
-breaking datacontract-v1.yaml datacontract-v2.yaml # export model as jsonschema
-(other formats: avro, dbt, dbt-sources, dbt-staging-sql, jsonschema, odcs, rdf,
-sql (coming soon), sodacl, terraform) $ datacontract export --format jsonschema
-datacontract.yaml # import sql $ datacontract import --format sql --source
-my_ddl.sql # import avro $ datacontract import --format avro --source
-avro_schema.avsc ``` ## Programmatic (Python) ```python from
-datacontract.data_contract import DataContract data_contract = DataContract
+with the schema, and all quality attributes are met. We can also use the
+datacontract.yaml to export in many [formats](#format), e.g., to SQL: ```bash $
+datacontract export --format sql https://datacontract.com/examples/orders-
+latest/datacontract.yaml # returns: -- Data Contract: urn:datacontract:
+checkout:orders-latest -- SQL Dialect: snowflake CREATE TABLE orders ( order_id
+TEXT not null primary key, order_timestamp TIMESTAMP_TZ not null, order_total
+NUMBER not null, customer_id TEXT, customer_email_address TEXT not null,
+processed_timestamp TIMESTAMP_TZ not null ); CREATE TABLE line_items
+( lines_item_id TEXT not null primary key, order_id TEXT, sku TEXT ); ``` Or
+generate this [HTML page](https://datacontract.com/examples/orders-latest/
+datacontract.html). ## Usage ```bash # create a new data contract from example
+and write it to datacontract.yaml $ datacontract init datacontract.yaml # lint
+the datacontract.yaml $ datacontract lint datacontract.yaml # execute schema
+and quality checks $ datacontract test datacontract.yaml # execute schema and
+quality checks on the examples within the contract $ datacontract test --
+examples datacontract.yaml # export data contract as html (other formats: avro,
+dbt, dbt-sources, dbt-staging-sql, jsonschema, odcs, rdf, sql, sodacl,
+terraform, ...) $ datacontract export --format html datacontract.yaml >
+datacontract.html # import avro (other formats: sql, ...) $ datacontract import
+--format avro --source avro_schema.avsc # find differences between to data
+contracts $ datacontract diff datacontract-v1.yaml datacontract-v2.yaml # find
+differences between to data contracts categorized into error, warning, and
+info. $ datacontract changelog datacontract-v1.yaml datacontract-v2.yaml # fail
+pipeline on breaking changes. Uses changelog internally and showing only error
+and warning. $ datacontract breaking datacontract-v1.yaml datacontract-v2.yaml
+``` ## Programmatic (Python) ```python from datacontract.data_contract import
+DataContract data_contract = DataContract
 (data_contract_file="datacontract.yaml") run = data_contract.test() if not
 run.has_passed(): print("Data quality validation failed.") # Abort pipeline,
-alert, or take corrective actions... ``` ## Integrations | Integration | Option
-| Description | |-------------------|------------------------------|-----------
--------------------------------------------------------------------------------
--------------| | Data Mesh Manager | `--publish` | Push full results to the
-[Data Mesh Manager API](https://api.datamesh-manager.com/swagger/index.html) |
-| OpenTelemetry | `--publish-to-opentelemetry` | Push result as gauge metrics
-(logs are planned) | ### Integration with Data Mesh Manager If you use [Data
-Mesh Manager](https://datamesh-manager.com/), you can use the data contract URL
-and append the `--publish` option to send and display the test results. Set an
-environment variable for your API key. ```bash # Fetch current data contract,
-execute tests on production, and publish result to data mesh manager $ EXPORT
-DATAMESH_MANAGER_API_KEY=xxx $ datacontract test https://demo.datamesh-
-manager.com/demo279750347121/datacontracts/4df9d6ee-e55d-4088-9598-
-b635b2fdcbbc/datacontract.yaml --server production --publish ``` ###
-Integration with OpenTelemetry If you use OpenTelemetry, you can use the data
-contract URL and append the `--publish-to-opentelemetry` option to send the
-test results to your OLTP-compatible instance, e.g., Prometheus. The metric
-name is "datacontract.cli.test.result" and it uses the following encoding for
-the result: | datacontract.cli.test.result | Description | |-------|-----------
-----------------------------| | 0 | test run passed, no warnings | | 1 | test
-run has warnings | | 2 | test run failed | | 3 | test run not possible due to
-an error | | 4 | test status unknown | ```bash # Fetch current data contract,
-execute tests on production, and publish result to open telemetry $ EXPORT
-OTEL_SERVICE_NAME=datacontract-cli $ EXPORT OTEL_EXPORTER_OTLP_ENDPOINT=https:/
-/YOUR_ID.apm.westeurope.azure.elastic-cloud.com:443 $ EXPORT
-OTEL_EXPORTER_OTLP_HEADERS=Authorization=Bearer%20secret # Optional, when using
-SaaS Products $ EXPORT OTEL_EXPORTER_OTLP_PROTOCOL=http/protobuf # Optional,
-default is http/protobuf - use value grpc to use the gRPC protocol instead #
-Send to OpenTelemetry $ datacontract test https://demo.datamesh-manager.com/
-demo279750347121/datacontracts/4df9d6ee-e55d-4088-9598-b635b2fdcbbc/
-datacontract.yaml --server production --publish-to-opentelemetry ``` Current
-limitations: - currently, only ConsoleExporter and OTLP Exporter - Metrics
-only, no logs yet (but loosely planned) ## Installation Choose the most
+alert, or take corrective actions... ``` ## Installation Choose the most
 appropriate installation method for your needs: ### pip Python 3.11
 recommended. Python 3.12 available as pre-release release candidate for 0.9.3
 ```bash python3 -m pip install datacontract-cli ``` ### pipx pipx installs into
 an isolated environment. ```bash pipx install datacontract-cli ``` ### Docker
 ```bash docker pull datacontract/cli docker run --rm -v ${PWD}:/home/
 datacontract datacontract/cli ``` Or via an alias that automatically uses the
 latest version: ```bash alias datacontract='docker run --rm -v "${PWD}:/home/
-datacontract" datacontract/cli:latest' ``` ## Documentation ### Tests Data
-Contract CLI can connect to data sources and run schema and quality tests to
-verify that the data contract is valid. ```bash $ datacontract test --server
-production datacontract.yaml ``` To connect to the databases the `server` block
-in the datacontract.yaml is used to set up the connection. In addition,
-credentials, such as username and passwords, may be defined with environment
-variables. The application uses different engines, based on the server `type`.
-| Type | Format | Description | Status | Engines | |--------------|------------
-|---------------------------------------------------------------------------|--
------------|-------------------------------------| | `s3` | `parquet` | Works
-for any S3-compliant endpoint., e.g., AWS S3, GCS, MinIO, Ceph, ... | â |
-soda-core-duckdb | | `s3` | `json` | Support for `new_line` delimited JSON
-files and one JSON record per file. | â | fastjsonschema
-soda-core-duckdb | | `s3` | `csv` | | â | soda-core-duckdb | | `s3` | `delta`
-| | Coming soon | TBD | | `postgres` | n/a | | â | soda-core-postgres | |
-`snowflake` | n/a | | â | soda-core-snowflake | | `bigquery` | n/a | | â |
-soda-core-bigquery | | `redshift` | n/a | | Coming soon | TBD | | `databricks`
-| n/a | Support for Databricks SQL with Unity catalog and Hive metastore. | â
-| soda-core-spark | | `databricks` | n/a | Support for Spark for programmatic
-use in Notebooks. | â | soda-core-spark-df | | `kafka` | `json` |
-Experimental. | â | pyspark
-soda-core-spark-df | | `kafka` | `avro` | | Coming soon | TBD | | `kafka` |
-`protobuf` | | Coming soon | TBD | | `local` | `parquet` | | â | soda-core-
-duckdb | | `local` | `json` | Support for `new_line` delimited JSON files and
-one JSON record per file. | â | fastjsonschema
-soda-core-duckdb | | `local` | `csv` | | â | soda-core-duckdb | Feel free to
-create an issue, if you need support for an additional type. ### S3 Data
-Contract CLI can test data that is stored in S3 buckets or any S3-compliant
-endpoints in various formats. #### Example datacontract.yaml ```yaml servers:
-production: type: s3 endpointUrl: https://minio.example.com # not needed with
-AWS S3 location: s3://bucket-name/path/*/*.json format: json delimiter:
-new_line # new_line, array, or none ``` #### Environment Variables |
-Environment Variable | Example | Description | |-------------------------------
-----|-------------------------------|-----------------------| |
-`DATACONTRACT_S3_REGION` | `eu-central-1` | Region of S3 bucket | |
-`DATACONTRACT_S3_ACCESS_KEY_ID` | `AKIAXV5Q5QABCDEFGH` | AWS Access Key ID | |
-`DATACONTRACT_S3_SECRET_ACCESS_KEY` | `93S7LRrJcqLaaaa/XXXXXXXXXXXXX` | AWS
+datacontract" datacontract/cli:latest' ``` ## Documentation Commands - [init]
+(#init) - [lint](#lint) - [test](#test) - [export](#export) - [import](#import)
+- [breaking](#breaking) - [changelog](#changelog) - [diff](#diff) ### init ```
+Usage: datacontract init [OPTIONS] [LOCATION] Download a datacontract.yaml
+template and write it to file. â­â Arguments
+âââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ®
+â location [LOCATION] The location (url or path) of the data contract yaml to
+create. â â [default: datacontract.yaml] â
+â°âââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ¯
+â­â Options
+âââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ®
+â --template TEXT URL of a template or data contract â â [default: â
+â https://datacontract.com/datacontract.init.yaml] â â --overwrite --no-
+overwrite Replace the existing datacontract.yaml â â [default: no-
+overwrite] â â --help Show this message and exit. â
+â°âââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ¯
+``` ### lint ``` Usage: datacontract lint [OPTIONS] [LOCATION] Validate that
+the datacontract.yaml is correctly formatted. â­â Arguments
+ââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ®
+â location [LOCATION] The location (url or path) of the data contract yaml.
+[default: datacontract.yaml] â
+â°ââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ¯
+â­â Options
+ââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ®
+â --schema TEXT The location (url or path) of the Data Contract Specification
+JSON Schema â â [default: https://datacontract.com/
+datacontract.schema.json] â â --help Show this message and exit. â
+â°ââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ¯
+``` ### test ``` Usage: datacontract test [OPTIONS] [LOCATION] Run schema and
+quality tests on configured servers. â­â Arguments
+ââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ®
+â location [LOCATION] The location (url or path) of the data contract yaml.
+[default: datacontract.yaml] â
+â°ââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ¯
+â­â Options
+ââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ®
+â --schema TEXT The location (url or path) of the Data Contract â â
+Specification JSON Schema â â [default: â â https://datacontract.com/
+datacontract.schema.json] â â --server TEXT The server configuration to run
+the schema and quality â â tests. Use the key of the server object in the
+data â â contract yaml file to refer to a server, e.g., â â
+`production`, or `all` for all servers (default). â â [default: all] â
+â --examples --no-examples Run the schema and quality tests on the example
+data â â within the data contract. â â [default: no-examples] â â -
+-publish TEXT The url to publish the results after the test â â [default:
+None] â â --publish-to-opentelemetry --no-publish-to-opentelemetry Publish
+the results to opentelemetry. Use environment â â variables to configure
+the OTLP endpoint, headers, etc. â â [default: no-publish-to-opentelemetry]
+â â --logs --no-logs Print logs [default: no-logs] â â --help Show this
+message and exit. â
+â°ââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ¯
+``` Data Contract CLI can connect to data sources and run schema and quality
+tests to verify that the data contract is valid. ```bash $ datacontract test --
+server production datacontract.yaml ``` To connect to the databases the
+`server` block in the datacontract.yaml is used to set up the connection. In
+addition, credentials, such as username and passwords, may be defined with
+environment variables. The application uses different engines, based on the
+server `type`. Internally, it connects with DuckDB, Spark, or a native
+connection and executes the most tests with soda-core and fastjsonschema.
+Credentials are read from the environment variables. Supported server types: |
+Type | Format | Status | |--------------|------------|-------------------------
+-------------------------------------------| | `s3` | `parquet` | â | | `s3`
+| `json` | â | | `s3` | `csv` | â | | `s3` | `delta` | Coming soon ([#24]
+(https://github.com/datacontract/cli/issues/24)) | | `s3` | `iceberg` | Coming
+soon | | `postgres` | n/a | â | | `snowflake` | n/a | â | | `bigquery` | n/
+a | â | | `redshift` | n/a | Coming soon | | `databricks` | n/a | â | |
+`kafka` | `json` | â | | `kafka` | `avro` | Coming soon | | `kafka` |
+`protobuf` | Coming soon | | `local` | `parquet` | â | | `local` | `json` |
+â | | `local` | `csv` | â | Feel free to create an issue, if you need
+support for an additional type. ### S3 Data Contract CLI can test data that is
+stored in S3 buckets or any S3-compliant endpoints in various formats. ####
+Example datacontract.yaml ```yaml servers: production: type: s3 endpointUrl:
+https://minio.example.com # not needed with AWS S3 location: s3://bucket-name/
+path/*/*.json format: json delimiter: new_line # new_line, array, or none ```
+#### Environment Variables | Environment Variable | Example | Description | |--
+---------------------------------|-------------------------------|-------------
+----------| | `DATACONTRACT_S3_REGION` | `eu-central-1` | Region of S3 bucket |
+| `DATACONTRACT_S3_ACCESS_KEY_ID` | `AKIAXV5Q5QABCDEFGH` | AWS Access Key ID |
+| `DATACONTRACT_S3_SECRET_ACCESS_KEY` | `93S7LRrJcqLaaaa/XXXXXXXXXXXXX` | AWS
 Secret Access Key | ### Postgres Data Contract CLI can test data in Postgres or
 Postgres-compliant databases (e.g., RisingWave). #### Example datacontract.yaml
 ```yaml servers: postgres: type: postgres host: localhost port: 5432 database:
 postgres schema: public models: my_table_1: # corresponds to a table type:
 table fields: my_column_1: # corresponds to a column type: varchar ``` ####
 Environment Variables | Environment Variable | Example | Description | |-------
 ---------------------------|--------------------|-------------| |
@@ -231,131 +223,242 @@
 Kafka Kafka support is currently considered experimental. #### Example
 datacontract.yaml ```yaml servers: production: type: kafka host: abc-12345.eu-
 central-1.aws.confluent.cloud:9092 topic: my-topic-name format: json ``` ####
 Environment Variables | Environment Variable | Example | Description | |-------
 -----------------------------|---------|-----------------------------| |
 `DATACONTRACT_KAFKA_SASL_USERNAME` | `xxx` | The SASL username (key). | |
 `DATACONTRACT_KAFKA_SASL_PASSWORD` | `xxx` | The SASL password (secret). | ###
-Exports ```bash # Example export to dbt model datacontract export --format dbt
-``` Available export options: | Type | Description | Status | |----------------
-------|---------------------------------------------------------|--------| |
-`jsonschema` | Export to JSON Schema | â | | `odcs` | Export to Open Data
-Contract Standard (ODCS) | â | | `sodacl` | Export to SodaCL quality checks
-in YAML format | â | | `dbt` | Export to dbt models in YAML format | â | |
-`dbt-sources` | Export to dbt sources in YAML format | â | | `dbt-staging-
-sql` | Export to dbt staging SQL models | â | | `rdf` | Export data contract
-to RDF representation in N3 format | â | | `avro` | Export to AVRO models |
-â | | `protobuf` | Export to Protobuf | â | | `terraform` | Export to
-terraform resources | â | | `sql` | Export to SQL DDL | â | | `sql-query` |
-Export to SQL Query | â | | `great-expectations` | Export to Great
-Expectations Suites in JSON Format | â | | `bigquery` | Export to BigQuery
-Schemas | TBD | | `pydantic` | Export to pydantic models | TBD | | `html` |
-Export to HTML page | TBD | | Missing something? | Please create an issue on
-GitHub | TBD | #### Great Expectations The export function transforms a
-specified data contract into a comprehensive Great Expectations JSON suite. If
-the contract includes multiple models, you need to specify the names of the
-model you wish to export. ```shell datacontract export datacontract.yaml --
-format great-expectations --model orders ``` The export creates a list of
-expectations by utilizing: - The data from the Model definition with a fixed
-mapping - The expectations provided in the quality field for each model (find
-here the expectations gallery https://greatexpectations.io/expectations/) ####
-RDF The export function converts a given data contract into a RDF
-representation. You have the option to add a base_url which will be used as the
-default prefix to resolve relative IRIs inside the document. ```shell
-datacontract export --format rdf --rdf-base https://www.example.com/
-datacontract.yaml ``` The data contract is mapped onto the following concepts
-of a yet to be defined Data Contract Ontology named https://datacontract.com/
-DataContractSpecification/ : - DataContract - Server - Model Having the data
-contract inside an RDF Graph gives us access the following use cases: -
-Interoperability with other data contract specification formats - Store data
-contracts inside a knowledge graph - Enhance a semantic search to find and
-retrieve data contracts - Linking model elements to already established
-ontologies and knowledge - Using full power of OWL to reason about the graph
-structure of data contracts - Apply graph algorithms on multiple data contracts
-(Find similar data contracts, find "gatekeeper" data products, find the true
-domain owner of a field attribute) ### Imports ```bash # Example import from
-SQL DDL datacontract import --format sql --source my_ddl.sql ``` Available
-import options: | Type | Description | Status | |--------------------|---------
----------------------------------------|---------| | `sql` | Import from SQL
-DDL | â | | `avro` | Import from AVRO schemas | â | | `protobuf` | Import
-from Protobuf schemas | TBD | | `jsonschema` | Import from JSON Schemas | TBD |
-| `bigquery` | Import from BigQuery Schemas | TBD | | `dbt` | Import from dbt
-models | TBD | | `odcs` | Import from Open Data Contract Standard (ODCS) | TBD
-| | Missing something? | Please create an issue on GitHub | TBD | ## Best
-Practices We share best practices in using the Data Contract CLI. ### Data-
-first Approach Create a data contract based on the actual data. This is the
-fastest way to get started and to get feedback from the data consumers. 1. Use
-an existing physical schema (e.g., SQL DDL) as a starting point to define your
-logical data model in the contract. Double check right after the import whether
-the actual data meets the imported logical data model. Just to be sure. ```bash
-$ datacontract import --format sql ddl.sql $ datacontract test ``` 2. Add
-examples to the `datacontract.yaml`. If you can, use actual data and anonymize.
-Make sure that the examples match the imported logical data model. ```bash $
-datacontract test --examples ``` 3. Add quality checks and additional type
-constraints one by one to the contract and make sure the examples and the
-actual data still adheres to the contract. Check against examples for a very
-fast feedback loop. ```bash $ datacontract test --examples $ datacontract test
-``` 4. Make sure that all the best practices for a `datacontract.yaml` are met
-using the linter. You probably forgot to document some fields and add the terms
-and conditions. ```bash $ datacontract lint ``` 5. Set up a CI pipeline that
-executes daily and reports the results to the [Data Mesh Manager](https://
-datamesh-manager.com). Or to some place else. You can even publish to any
-opentelemetry compatible system. ```bash $ datacontract test --publish https://
-api.datamesh-manager.com/api/runs ``` ### Contract-First Create a data contract
-based on the requirements from use cases. 1. Start with a `datacontract.yaml`
-template. ```bash $ datacontract init ``` 2. Add examples to the
-`datacontract.yaml`. Do not start with the data model, although you are
-probably tempted to do that. Examples are the fastest way to get feedback from
-everybody and not loose someone in the discussion. 3. Create the model based on
-the examples. Test the model against the examples to double-check whether the
-model matches the examples. ```bash $ datacontract test --examples ``` 4. Add
-quality checks and additional type constraints one by one to the contract and
-make sure the examples and the actual data still adheres to the contract. Check
-against examples for a very fast feedback loop. ```bash $ datacontract test --
-examples ``` 5. Fill in the terms, descriptions, etc. Make sure you follow all
-best practices for a `datacontract.yaml` using the linter. ```bash $
-datacontract lint ``` 6. Set up a CI pipeline that lints and tests the examples
-so you make sure that any changes later do not decrease the quality of the
-contract. ```bash $ datacontract lint $ datacontract test --examples ``` 7. Use
-the export function to start building the providing data product as well as the
-integration into the consuming data products. ```bash # data provider $
-datacontract export --format dbt # data consumer $ datacontract export --format
-dbt-sources $ datacontract export --format dbt-staging-sql ``` ### Schema
-Evolution #### Non-breaking Changes Examples: adding models or fields - Add the
-models or fields in the datacontract.yaml - Increment the minor version of the
-datacontract.yaml on any change. Simply edit the datacontract.yaml for this. -
-You need a policy that these changes are non-breaking. That means that one
-cannot use the star expression in SQL to query a table under contract. Make the
-consequences known. - Fail the build in the Pull Request if a datacontract.yaml
-accidentially adds a breaking change even despite only a minor version change
-```bash $ datacontract breaking datacontract-from-pr.yaml datacontract-from-
-main.yaml ``` - Create a changelog of this minor change. ```bash $ datacontract
-changelog datacontract-from-pr.yaml datacontract-from-main.yaml ``` ####
-Breaking Changes Examples: Removing or renaming models and fields. - Remove or
-rename models and fields in the datacontract.yaml, and any other change that
-might be part of this new major version of this data contract. - Increment the
-major version of the datacontract.yaml for this and create a new file for the
-major version. The reason being, that one needs to offer an upgrade path for
-the data consumers from the old to the new major version. - As data consumers
-need to migrate, try to reduce the frequency of major versions by making
-multiple breaking changes together if possible. - Be aware of the notice period
-in the data contract as this is the minimum amount of time you have to offer
-both the old and the new version for a migration path. - Do not fear making
-breaking changes with data contracts. It's okay to do them in this controlled
-way. Really! - Create a changelog of this major change. ```bash $ datacontract
-changelog datacontract-from-pr.yaml datacontract-from-main.yaml ``` ##
-Development Setup Python base interpreter should be 3.11.x (unless working on
-3.12 release candidate). ```bash # create venv python3 -m venv venv source
-venv/bin/activate # Install Requirements pip install --upgrade pip setuptools
-wheel pip install -e '.[dev]' ruff check --fix ruff format --check pytest ```
-Release ```bash git tag v0.9.0 git push origin v0.9.0 python3 -m pip install --
-upgrade build twine rm -r dist/ python3 -m build # for now only test.pypi.org
-python3 -m twine upload --repository testpypi dist/* ``` Docker Build ```bash
-docker build -t datacontract/cli . docker run --rm -v ${PWD}:/home/datacontract
-datacontract/cli ``` ## Release Steps 1. Update the version in `pyproject.toml`
-2. Have a look at the `CHANGELOG.md` 3. Create release commit manually 4.
-Execute `./release` 5. Wait until GitHub Release is created 6. Add the release
-notes to the GitHub Release ## Contribution We are happy to receive your
-contributions. Propose your change in an issue or directly create a pull
-request with your improvements. ## License [MIT License](LICENSE) ## Credits
-Created by [Stefan Negele](https://www.linkedin.com/in/stefan-negele-573153112/
-) and [Jochen Christ](https://www.linkedin.com/in/jochenchrist/).
+export ``` Usage: datacontract export [OPTIONS] [LOCATION] Convert data
+contract to a specific format. console.prints to stdout. â­â Arguments
+ââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ®
+â location [LOCATION] The location (url or path) of the data contract yaml.
+[default: datacontract.yaml] â
+â°ââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ¯
+â­â Options
+ââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ®
+â * --format [html|jsonschema|pydantic-model|sodacl|dbt|dbt-sources|dbt-
+staging-sql|odcs|rd The export format. [default: None] [required] â â
+f|avro|protobuf|great-expectations|terraform|avro-idl|sql|sql-query] â â --
+server TEXT The server name to export. [default: None] â â --model TEXT Use
+the key of the model in the data contract yaml file to refer to a â â
+model, e.g., `orders`, or `all` for all models (default). â â [default:
+all] â â --help Show this message and exit. â
+â°ââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ¯
+â­â RDF Options
+ââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ®
+â --rdf-base TEXT [rdf] The base URI used to generate the RDF graph.
+[default: None] â
+â°ââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ¯
+â­â SQL Options
+ââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ®
+â --sql-server-type TEXT [sql] The server type to determine the sql dialect.
+By default, it uses 'auto' to automatically detect the sql dialect via the
+specified â â servers in the data contract. â â [default: auto] â
+â°ââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ¯
+``` ```bash # Example export data contract as HTML datacontract export --format
+html > datacontract.html ``` Available export options: | Type | Description |
+Status | |----------------------|----------------------------------------------
+-----------|--------| | `html` | Export to HTML | â | | `jsonschema` | Export
+to JSON Schema | â | | `odcs` | Export to Open Data Contract Standard (ODCS)
+| â | | `sodacl` | Export to SodaCL quality checks in YAML format | â | |
+`dbt` | Export to dbt models in YAML format | â | | `dbt-sources` | Export to
+dbt sources in YAML format | â | | `dbt-staging-sql` | Export to dbt staging
+SQL models | â | | `rdf` | Export data contract to RDF representation in N3
+format | â | | `avro` | Export to AVRO models | â | | `protobuf` | Export
+to Protobuf | â | | `terraform` | Export to terraform resources | â | |
+`sql` | Export to SQL DDL | â | | `sql-query` | Export to SQL Query | â | |
+`great-expectations` | Export to Great Expectations Suites in JSON Format | â
+| | `bigquery` | Export to BigQuery Schemas | TBD | | `pydantic` | Export to
+pydantic models | TBD | | Missing something? | Please create an issue on GitHub
+| TBD | #### Great Expectations The export function transforms a specified data
+contract into a comprehensive Great Expectations JSON suite. If the contract
+includes multiple models, you need to specify the names of the model you wish
+to export. ```shell datacontract export datacontract.yaml --format great-
+expectations --model orders ``` The export creates a list of expectations by
+utilizing: - The data from the Model definition with a fixed mapping - The
+expectations provided in the quality field for each model (find here the
+expectations gallery https://greatexpectations.io/expectations/) #### RDF The
+export function converts a given data contract into a RDF representation. You
+have the option to add a base_url which will be used as the default prefix to
+resolve relative IRIs inside the document. ```shell datacontract export --
+format rdf --rdf-base https://www.example.com/ datacontract.yaml ``` The data
+contract is mapped onto the following concepts of a yet to be defined Data
+Contract Ontology named https://datacontract.com/DataContractSpecification/ : -
+DataContract - Server - Model Having the data contract inside an RDF Graph
+gives us access the following use cases: - Interoperability with other data
+contract specification formats - Store data contracts inside a knowledge graph
+- Enhance a semantic search to find and retrieve data contracts - Linking model
+elements to already established ontologies and knowledge - Using full power of
+OWL to reason about the graph structure of data contracts - Apply graph
+algorithms on multiple data contracts (Find similar data contracts, find
+"gatekeeper" data products, find the true domain owner of a field attribute)
+### import ``` Usage: datacontract import [OPTIONS] Create a data contract from
+the given source file. Prints to stdout. â­â Options
+ââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ®
+â * --format [sql|avro] The format of the source file. [default: None]
+[required] â â * --source TEXT The path to the file that should be
+imported. [default: None] [required] â â --help Show this message and exit.
+â
+â°ââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ¯
+``` Example: ```bash # Example import from SQL DDL datacontract import --format
+sql --source my_ddl.sql ``` Available import options: | Type | Description |
+Status | |--------------------|------------------------------------------------
+|---------| | `sql` | Import from SQL DDL | â | | `avro` | Import from AVRO
+schemas | â | | `protobuf` | Import from Protobuf schemas | TBD | |
+`jsonschema` | Import from JSON Schemas | TBD | | `bigquery` | Import from
+BigQuery Schemas | TBD | | `dbt` | Import from dbt models | TBD | | `odcs` |
+Import from Open Data Contract Standard (ODCS) | TBD | | Missing something? |
+Please create an issue on GitHub | TBD | ### breaking ``` Usage: datacontract
+breaking [OPTIONS] LOCATION_OLD LOCATION_NEW Identifies breaking changes
+between data contracts. Prints to stdout. â­â Arguments
+ââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ®
+â * location_old TEXT The location (url or path) of the old data contract
+yaml. [default: None] [required] â â * location_new TEXT The location (url
+or path) of the new data contract yaml. [default: None] [required] â
+â°ââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ¯
+â­â Options
+ââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ®
+â --help Show this message and exit. â
+â°ââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ¯
+``` ### changelog ``` Usage: datacontract changelog [OPTIONS] LOCATION_OLD
+LOCATION_NEW Generate a changelog between data contracts. Prints to stdout.
+â­â Arguments
+ââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ®
+â * location_old TEXT The location (url or path) of the old data contract
+yaml. [default: None] [required] â â * location_new TEXT The location (url
+or path) of the new data contract yaml. [default: None] [required] â
+â°ââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ¯
+â­â Options
+ââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ®
+â --help Show this message and exit. â
+â°ââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ¯
+``` ### diff ``` Usage: datacontract diff [OPTIONS] LOCATION_OLD LOCATION_NEW
+PLACEHOLDER. Currently works as 'changelog' does. â­â Arguments
+ââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ®
+â * location_old TEXT The location (url or path) of the old data contract
+yaml. [default: None] [required] â â * location_new TEXT The location (url
+or path) of the new data contract yaml. [default: None] [required] â
+â°ââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ¯
+â­â Options
+ââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ®
+â --help Show this message and exit. â
+â°ââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ¯
+``` ## Integrations | Integration | Option | Description | |-------------------
+|------------------------------|-----------------------------------------------
+--------------------------------------------------------| | Data Mesh Manager |
+`--publish` | Push full results to the [Data Mesh Manager API](https://
+api.datamesh-manager.com/swagger/index.html) | | OpenTelemetry | `--publish-to-
+opentelemetry` | Push result as gauge metrics | ### Integration with Data Mesh
+Manager If you use [Data Mesh Manager](https://datamesh-manager.com/), you can
+use the data contract URL and append the `--publish` option to send and display
+the test results. Set an environment variable for your API key. ```bash # Fetch
+current data contract, execute tests on production, and publish result to data
+mesh manager $ EXPORT DATAMESH_MANAGER_API_KEY=xxx $ datacontract test https://
+demo.datamesh-manager.com/demo279750347121/datacontracts/4df9d6ee-e55d-4088-
+9598-b635b2fdcbbc/datacontract.yaml --server production --publish ``` ###
+Integration with OpenTelemetry If you use OpenTelemetry, you can use the data
+contract URL and append the `--publish-to-opentelemetry` option to send the
+test results to your OLTP-compatible instance, e.g., Prometheus. The metric
+name is "datacontract.cli.test.result" and it uses the following encoding for
+the result: | datacontract.cli.test.result | Description | |-------|-----------
+----------------------------| | 0 | test run passed, no warnings | | 1 | test
+run has warnings | | 2 | test run failed | | 3 | test run not possible due to
+an error | | 4 | test status unknown | ```bash # Fetch current data contract,
+execute tests on production, and publish result to open telemetry $ EXPORT
+OTEL_SERVICE_NAME=datacontract-cli $ EXPORT OTEL_EXPORTER_OTLP_ENDPOINT=https:/
+/YOUR_ID.apm.westeurope.azure.elastic-cloud.com:443 $ EXPORT
+OTEL_EXPORTER_OTLP_HEADERS=Authorization=Bearer%20secret # Optional, when using
+SaaS Products $ EXPORT OTEL_EXPORTER_OTLP_PROTOCOL=http/protobuf # Optional,
+default is http/protobuf - use value grpc to use the gRPC protocol instead #
+Send to OpenTelemetry $ datacontract test https://demo.datamesh-manager.com/
+demo279750347121/datacontracts/4df9d6ee-e55d-4088-9598-b635b2fdcbbc/
+datacontract.yaml --server production --publish-to-opentelemetry ``` Current
+limitations: - currently, only ConsoleExporter and OTLP Exporter - Metrics
+only, no logs yet (but loosely planned) ## Best Practices We share best
+practices in using the Data Contract CLI. ### Data-first Approach Create a data
+contract based on the actual data. This is the fastest way to get started and
+to get feedback from the data consumers. 1. Use an existing physical schema
+(e.g., SQL DDL) as a starting point to define your logical data model in the
+contract. Double check right after the import whether the actual data meets the
+imported logical data model. Just to be sure. ```bash $ datacontract import --
+format sql ddl.sql $ datacontract test ``` 2. Add examples to the
+`datacontract.yaml`. If you can, use actual data and anonymize. Make sure that
+the examples match the imported logical data model. ```bash $ datacontract test
+--examples ``` 3. Add quality checks and additional type constraints one by one
+to the contract and make sure the examples and the actual data still adheres to
+the contract. Check against examples for a very fast feedback loop. ```bash $
+datacontract test --examples $ datacontract test ``` 4. Make sure that all the
+best practices for a `datacontract.yaml` are met using the linter. You probably
+forgot to document some fields and add the terms and conditions. ```bash $
+datacontract lint ``` 5. Set up a CI pipeline that executes daily and reports
+the results to the [Data Mesh Manager](https://datamesh-manager.com). Or to
+some place else. You can even publish to any opentelemetry compatible system.
+```bash $ datacontract test --publish https://api.datamesh-manager.com/api/runs
+``` ### Contract-First Create a data contract based on the requirements from
+use cases. 1. Start with a `datacontract.yaml` template. ```bash $ datacontract
+init ``` 2. Add examples to the `datacontract.yaml`. Do not start with the data
+model, although you are probably tempted to do that. Examples are the fastest
+way to get feedback from everybody and not loose someone in the discussion. 3.
+Create the model based on the examples. Test the model against the examples to
+double-check whether the model matches the examples. ```bash $ datacontract
+test --examples ``` 4. Add quality checks and additional type constraints one
+by one to the contract and make sure the examples and the actual data still
+adheres to the contract. Check against examples for a very fast feedback loop.
+```bash $ datacontract test --examples ``` 5. Fill in the terms, descriptions,
+etc. Make sure you follow all best practices for a `datacontract.yaml` using
+the linter. ```bash $ datacontract lint ``` 6. Set up a CI pipeline that lints
+and tests the examples so you make sure that any changes later do not decrease
+the quality of the contract. ```bash $ datacontract lint $ datacontract test --
+examples ``` 7. Use the export function to start building the providing data
+product as well as the integration into the consuming data products. ```bash #
+data provider $ datacontract export --format dbt # data consumer $ datacontract
+export --format dbt-sources $ datacontract export --format dbt-staging-sql ```
+### Schema Evolution #### Non-breaking Changes Examples: adding models or
+fields - Add the models or fields in the datacontract.yaml - Increment the
+minor version of the datacontract.yaml on any change. Simply edit the
+datacontract.yaml for this. - You need a policy that these changes are non-
+breaking. That means that one cannot use the star expression in SQL to query a
+table under contract. Make the consequences known. - Fail the build in the Pull
+Request if a datacontract.yaml accidentially adds a breaking change even
+despite only a minor version change ```bash $ datacontract breaking
+datacontract-from-pr.yaml datacontract-from-main.yaml ``` - Create a changelog
+of this minor change. ```bash $ datacontract changelog datacontract-from-
+pr.yaml datacontract-from-main.yaml ``` #### Breaking Changes Examples:
+Removing or renaming models and fields. - Remove or rename models and fields in
+the datacontract.yaml, and any other change that might be part of this new
+major version of this data contract. - Increment the major version of the
+datacontract.yaml for this and create a new file for the major version. The
+reason being, that one needs to offer an upgrade path for the data consumers
+from the old to the new major version. - As data consumers need to migrate, try
+to reduce the frequency of major versions by making multiple breaking changes
+together if possible. - Be aware of the notice period in the data contract as
+this is the minimum amount of time you have to offer both the old and the new
+version for a migration path. - Do not fear making breaking changes with data
+contracts. It's okay to do them in this controlled way. Really! - Create a
+changelog of this major change. ```bash $ datacontract changelog datacontract-
+from-pr.yaml datacontract-from-main.yaml ``` ## Development Setup Python base
+interpreter should be 3.11.x (unless working on 3.12 release candidate).
+```bash # create venv python3 -m venv venv source venv/bin/activate # Install
+Requirements pip install --upgrade pip setuptools wheel pip install -e '.[dev]'
+ruff check --fix ruff format --check pytest ``` ### Docker Build ```bash docker
+build -t datacontract/cli . docker run --rm -v ${PWD}:/home/datacontract
+datacontract/cli ``` #### Docker compose integration We've included a [docker-
+compose.yml](./docker-compose.yml) configuration to simplify the build, test,
+and deployment of the image. ##### Building the Image with Docker Compose To
+build the Docker image using Docker Compose, run the following command: ```bash
+docker compose build ``` This command utilizes the `docker-compose.yml` to
+build the image, leveraging predefined settings such as the build context and
+Dockerfile location. This approach streamlines the image creation process,
+avoiding the need for manual build specifications each time. #### Testing the
+Image After building the image, you can test it directly with Docker Compose:
+```bash docker compose run --rm datacontract --version ``` This command runs
+the container momentarily to check the version of the `datacontract` CLI. The
+`--rm` flag ensures that the container is automatically removed after the
+command executes, keeping your environment clean. ## Release Steps 1. Update
+the version in `pyproject.toml` 2. Have a look at the `CHANGELOG.md` 3. Create
+release commit manually 4. Execute `./release` 5. Wait until GitHub Release is
+created 6. Add the release notes to the GitHub Release ## Contribution We are
+happy to receive your contributions. Propose your change in an issue or
+directly create a pull request with your improvements. ## License [MIT License]
+(LICENSE) ## Credits Created by [Stefan Negele](https://www.linkedin.com/in/
+stefan-negele-573153112/) and [Jochen Christ](https://www.linkedin.com/in/
+jochenchrist/).
```

### Comparing `datacontract-cli-0.9.8/datacontract/breaking/breaking.py` & `datacontract_cli-0.9.9/datacontract/breaking/breaking.py`

 * *Files identical despite different names*

### Comparing `datacontract-cli-0.9.8/datacontract/breaking/breaking_rules.py` & `datacontract_cli-0.9.9/datacontract/breaking/breaking_rules.py`

 * *Files identical despite different names*

### Comparing `datacontract-cli-0.9.8/datacontract/cli.py` & `datacontract_cli-0.9.9/datacontract/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 
 from datacontract.data_contract import DataContract
 from datacontract.init.download_datacontract_file import \
     download_datacontract_file, FileExistsException
 
 console = Console()
 
+
 class OrderedCommands(TyperGroup):
     def list_commands(self, ctx: Context) -> Iterable[str]:
         return self.commands.keys()
 
 
 app = typer.Typer(
     cls=OrderedCommands,
@@ -149,14 +150,15 @@
     avro = "avro"
     protobuf = "protobuf"
     great_expectations = "great-expectations"
     terraform = "terraform"
     avro_idl = "avro-idl"
     sql = "sql"
     sql_query = "sql-query"
+    html = "html"
 
 
 @app.command()
 def export(
     format: Annotated[ExportFormat, typer.Option(help="The export format.")],
     server: Annotated[str, typer.Option(help="The server name to export.")] = None,
     model: Annotated[
```

### Comparing `datacontract-cli-0.9.8/datacontract/data_contract.py` & `datacontract_cli-0.9.9/datacontract/data_contract.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import json
 import logging
 import tempfile
 import typing
 
 import yaml
+from pyspark.sql import SparkSession
 
 from datacontract.breaking.breaking import models_breaking_changes, \
     quality_breaking_changes
 from datacontract.engines.datacontract.check_that_datacontract_contains_valid_servers_configuration import (
     check_that_datacontract_contains_valid_server_configuration,
 )
 from datacontract.engines.fastjsonschema.check_jsonschema import \
@@ -15,14 +16,15 @@
 from datacontract.engines.soda.check_soda_execute import check_soda_execute
 from datacontract.export.avro_converter import to_avro_schema_json
 from datacontract.export.avro_idl_converter import to_avro_idl
 from datacontract.export.dbt_converter import to_dbt_models_yaml, \
     to_dbt_sources_yaml, to_dbt_staging_sql
 from datacontract.export.great_expectations_converter import \
     to_great_expectations
+from datacontract.export.html_export import to_html
 from datacontract.export.jsonschema_converter import to_jsonschema_json
 from datacontract.export.odcs_converter import to_odcs_yaml
 from datacontract.export.protobuf_converter import to_protobuf
 from datacontract.export.pydantic_converter import to_pydantic_model_str
 from datacontract.export.rdf_converter import to_rdf_n3
 from datacontract.export.sodacl_converter import to_sodacl_yaml
 from datacontract.export.sql_converter import to_sql_ddl, to_sql_query
@@ -35,59 +37,38 @@
 from datacontract.lint import resolve
 from datacontract.lint.linters.description_linter import DescriptionLinter
 from datacontract.lint.linters.example_model_linter import ExampleModelLinter
 from datacontract.lint.linters.field_pattern_linter import FieldPatternLinter
 from datacontract.lint.linters.field_reference_linter import \
     FieldReferenceLinter
 from datacontract.lint.linters.notice_period_linter import NoticePeriodLinter
-from datacontract.lint.linters.primary_field_linter import \
-    PrimaryFieldUniqueRequired
 from datacontract.lint.linters.quality_schema_linter import \
     QualityUsesSchemaLinter
 from datacontract.lint.linters.valid_constraints_linter import \
     ValidFieldConstraintsLinter
 from datacontract.model.breaking_change import BreakingChanges, BreakingChange, \
     Severity
 from datacontract.model.data_contract_specification import \
     DataContractSpecification, Server
 from datacontract.model.exceptions import DataContractException
 from datacontract.model.run import Run, Check
 
 
-def _determine_sql_server_type(data_contract, sql_server_type):
-    if sql_server_type == "auto":
-        if data_contract.servers is None or len(data_contract.servers) == 0:
-            raise RuntimeError("Export with server_type='auto' requires servers in the data contract.")
-
-        server_types = set([server.type for server in data_contract.servers.values()])
-        if "snowflake" in server_types:
-            return "snowflake"
-        elif "postgres" in server_types:
-            return "postgres"
-        elif "databricks" in server_types:
-            return "databricks"
-        else:
-            # default to snowflake dialect
-            return "snowflake"
-    else:
-        return sql_server_type
-
-
 class DataContract:
     def __init__(
         self,
         data_contract_file: str = None,
         data_contract_str: str = None,
         data_contract: DataContractSpecification = None,
         schema_location: str = None,
         server: str = None,
         examples: bool = False,
         publish_url: str = None,
         publish_to_opentelemetry: bool = False,
-        spark: str = None,
+        spark: SparkSession = None,
         inline_definitions: bool = False,
     ):
         self._data_contract_file = data_contract_file
         self._data_contract_str = data_contract_str
         self._data_contract = data_contract
         self._schema_location = schema_location
         self._server = server
@@ -98,15 +79,14 @@
         self._inline_definitions = inline_definitions
         self.all_linters = {
             ExampleModelLinter(),
             QualityUsesSchemaLinter(),
             FieldPatternLinter(),
             FieldReferenceLinter(),
             NoticePeriodLinter(),
-            PrimaryFieldUniqueRequired(),
             ValidFieldConstraintsLinter(),
             DescriptionLinter(),
         }
 
     @classmethod
     def init(cls, template: str = "https://datacontract.com/datacontract.init.yaml") -> DataContractSpecification:
         return resolve.resolve_data_contract(data_contract_location=template)
@@ -242,20 +222,20 @@
 
         run.finish()
 
         if self._publish_url is not None:
             try:
                 publish_datamesh_manager(run, self._publish_url)
             except Exception:
-                logging.error("Failed to publish to datamesh manager")
+                run.log_error("Failed to publish to datamesh manager")
         if self._publish_to_opentelemetry:
             try:
                 publish_opentelemetry(run)
             except Exception:
-                logging.error("Failed to publish to opentelemetry")
+                run.log_error("Failed to publish to opentelemetry")
 
         return run
 
     def breaking(self, other: "DataContract") -> BreakingChanges:
         return self.changelog(other, include_severities=[Severity.ERROR, Severity.WARNING])
 
     def changelog(
@@ -381,21 +361,21 @@
 
                 return to_avro_schema_json(model_name, model_value)
         if export_format == "avro-idl":
             return to_avro_idl(data_contract)
         if export_format == "terraform":
             return to_terraform(data_contract)
         if export_format == "sql":
-            server_type = _determine_sql_server_type(data_contract, sql_server_type)
+            server_type = self._determine_sql_server_type(data_contract, sql_server_type)
             return to_sql_ddl(data_contract, server_type=server_type)
         if export_format == "sql-query":
             if data_contract.models is None:
                 raise RuntimeError(f"Export to {export_format} requires models in the data contract.")
 
-            server_type = _determine_sql_server_type(data_contract, sql_server_type)
+            server_type = self._determine_sql_server_type(data_contract, sql_server_type)
 
             model_names = list(data_contract.models.keys())
 
             if model == "all":
                 if len(data_contract.models.items()) != 1:
                     raise RuntimeError(
                         f"Export to {export_format} is model specific. Specify the model via --model $MODEL_NAME. Available models: {model_names}"
@@ -435,18 +415,38 @@
                     raise RuntimeError(
                         f"Model {model_name} not found in the data contract. " f"Available models: {model_names}"
                     )
 
                 return to_great_expectations(data_contract, model_name)
         if export_format == "pydantic-model":
             return to_pydantic_model_str(data_contract)
+        if export_format == "html":
+            return to_html(data_contract)
         else:
             print(f"Export format {export_format} not supported.")
             return ""
 
+    def _determine_sql_server_type(self, data_contract: DataContractSpecification, sql_server_type: str):
+        if sql_server_type == "auto":
+            if data_contract.servers is None or len(data_contract.servers) == 0:
+                raise RuntimeError("Export with server_type='auto' requires servers in the data contract.")
+
+            server_types = set([server.type for server in data_contract.servers.values()])
+            if "snowflake" in server_types:
+                return "snowflake"
+            elif "postgres" in server_types:
+                return "postgres"
+            elif "databricks" in server_types:
+                return "databricks"
+            else:
+                # default to snowflake dialect
+                return "snowflake"
+        else:
+            return sql_server_type
+
     def _get_examples_server(self, data_contract, run, tmp_dir):
         run.log_info(f"Copying examples to files in temporary directory {tmp_dir}")
         format = "json"
         for example in data_contract.examples:
             format = example.type
             p = f"{tmp_dir}/{example.model}.{format}"
             run.log_info(f"Creating example file {p}")
```

### Comparing `datacontract-cli-0.9.8/datacontract/engines/datacontract/check_that_datacontract_contains_valid_servers_configuration.py` & `datacontract_cli-0.9.9/datacontract/engines/datacontract/check_that_datacontract_contains_valid_servers_configuration.py`

 * *Files identical despite different names*

### Comparing `datacontract-cli-0.9.8/datacontract/engines/datacontract/check_that_datacontract_file_exists.py` & `datacontract_cli-0.9.9/datacontract/engines/datacontract/check_that_datacontract_file_exists.py`

 * *Files identical despite different names*

### Comparing `datacontract-cli-0.9.8/datacontract/engines/datacontract/check_that_datacontract_str_is_valid.py` & `datacontract_cli-0.9.9/datacontract/engines/datacontract/check_that_datacontract_str_is_valid.py`

 * *Files identical despite different names*

### Comparing `datacontract-cli-0.9.8/datacontract/engines/fastjsonschema/check_jsonschema.py` & `datacontract_cli-0.9.9/datacontract/engines/fastjsonschema/check_jsonschema.py`

 * *Files identical despite different names*

### Comparing `datacontract-cli-0.9.8/datacontract/engines/fastjsonschema/s3/s3_read_files.py` & `datacontract_cli-0.9.9/datacontract/engines/fastjsonschema/s3/s3_read_files.py`

 * *Files identical despite different names*

### Comparing `datacontract-cli-0.9.8/datacontract/engines/soda/check_soda_execute.py` & `datacontract_cli-0.9.9/datacontract/engines/soda/check_soda_execute.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import logging
 
+from pyspark.sql import SparkSession
 from soda.scan import Scan
 
 from datacontract.engines.soda.connections.bigquery import \
     to_bigquery_soda_configuration
 from datacontract.engines.soda.connections.databricks import \
     to_databricks_soda_configuration
 from datacontract.engines.soda.connections.duckdb import get_duckdb_connection
@@ -15,15 +16,17 @@
     to_snowflake_soda_configuration
 from datacontract.export.sodacl_converter import to_sodacl_yaml
 from datacontract.model.data_contract_specification import \
     DataContractSpecification, Server
 from datacontract.model.run import Run, Check, Log
 
 
-def check_soda_execute(run: Run, data_contract: DataContractSpecification, server: Server, spark, tmp_dir):
+def check_soda_execute(
+    run: Run, data_contract: DataContractSpecification, server: Server, spark: SparkSession, tmp_dir
+):
     if data_contract is None:
         run.log_warn("Cannot run engine soda-core, as data contract is invalid")
         return
 
     run.log_info("Running engine soda-core")
     scan = Scan()
 
@@ -87,14 +90,15 @@
         return
 
     # Don't check types for json format, as they are checked with json schema
     # Don't check types for avro format, as they are checked with avro schema
     # Don't check types for csv format, as they are hard to detect
     server_type = server.type
     check_types = server.format != "json" and server.format != "csv" and server.format != "avro"
+
     sodacl_yaml_str = to_sodacl_yaml(data_contract, server_type, check_types)
     # print("sodacl_yaml_str:\n" + sodacl_yaml_str)
     scan.add_sodacl_yaml_str(sodacl_yaml_str)
 
     # Execute the scan
     logging.info("Starting soda scan")
     scan.execute()
@@ -102,24 +106,21 @@
 
     # pprint.PrettyPrinter(indent=2).pprint(scan.build_scan_results())
 
     scan_results = scan.get_scan_results()
     for c in scan_results.get("checks"):
         check = Check(
             type="schema",
-            result="passed"
-            if c.get("outcome") == "pass"
-            else "failed"
-            if c.get("outcome") == "fail"
-            else c.get("outcome"),
+            result=to_result(c),
             reason=", ".join(c.get("outcomeReasons")),
             name=c.get("name"),
             model=c.get("table"),
             field=c.get("column"),
             engine="soda-core",
+            diagnostics=c.get("diagnostics"),
         )
         update_reason(check, c)
         run.checks.append(check)
 
     for log in scan_results.get("logs"):
         run.logs.append(
             Log(
@@ -139,14 +140,24 @@
                 reason="Engine soda-core has errors. See the logs for details.",
                 engine="soda-core",
             )
         )
         return
 
 
+def to_result(c) -> str:
+    soda_outcome = c.get("outcome")
+    if soda_outcome == "pass":
+        return "passed"
+    elif soda_outcome == "fail":
+        return "failed"
+    else:
+        return soda_outcome
+
+
 def update_reason(check, c):
     """Try to find a reason in diagnostics"""
     if check.result == "passed":
         return
     if check.reason is not None and check.reason != "":
         return
     for block in c["diagnostics"]["blocks"]:
```

### Comparing `datacontract-cli-0.9.8/datacontract/engines/soda/connections/bigquery.py` & `datacontract_cli-0.9.9/datacontract/engines/soda/connections/bigquery.py`

 * *Files identical despite different names*

### Comparing `datacontract-cli-0.9.8/datacontract/engines/soda/connections/dask.py` & `datacontract_cli-0.9.9/datacontract/engines/soda/connections/dask.py`

 * *Files identical despite different names*

### Comparing `datacontract-cli-0.9.8/datacontract/engines/soda/connections/databricks.py` & `datacontract_cli-0.9.9/datacontract/engines/soda/connections/databricks.py`

 * *Files identical despite different names*

### Comparing `datacontract-cli-0.9.8/datacontract/engines/soda/connections/duckdb.py` & `datacontract_cli-0.9.9/datacontract/engines/soda/connections/duckdb.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 import logging
 import os
 
 import duckdb
+from datacontract.export.csv_type_converter import convert_to_duckdb_csv_type
 
 
 def get_duckdb_connection(data_contract, server):
     con = duckdb.connect(database=":memory:")
     path: str = ""
     if server.type == "local":
         path = server.path
     if server.type == "s3":
         path = server.location
     setup_s3_connection(con, server)
-    for model_name in data_contract.models:
+    for model_name, model in data_contract.models.items():
         model_path = path
         if "{model}" in model_path:
             model_path = model_path.format(model=model_name)
         logging.info(f"Creating table {model_name} for {model_path}")
 
         if server.format == "json":
             format = "auto"
@@ -28,20 +29,36 @@
                         CREATE VIEW "{model_name}" AS SELECT * FROM read_json_auto('{model_path}', format='{format}', hive_partitioning=1);
                         """)
         elif server.format == "parquet":
             con.sql(f"""
                         CREATE VIEW "{model_name}" AS SELECT * FROM read_parquet('{model_path}', hive_partitioning=1);
                         """)
         elif server.format == "csv":
-            con.sql(f"""
-                        CREATE VIEW "{model_name}" AS SELECT * FROM read_csv_auto('{model_path}', hive_partitioning=1);
-                        """)
+            columns = to_csv_types(model)
+            if columns is None:
+                con.sql(
+                    f"""CREATE VIEW "{model_name}" AS SELECT * FROM read_csv('{model_path}', hive_partitioning=1);"""
+                )
+            else:
+                con.sql(
+                    f"""CREATE VIEW "{model_name}" AS SELECT * FROM read_csv('{model_path}', hive_partitioning=1, columns={columns});"""
+                )
     return con
 
 
+def to_csv_types(model) -> dict:
+    if model is None:
+        return None
+    columns = {}
+    # ['SQLNULL', 'BOOLEAN', 'BIGINT', 'DOUBLE', 'TIME', 'DATE', 'TIMESTAMP', 'VARCHAR']
+    for field_name, field in model.fields.items():
+        columns[field_name] = convert_to_duckdb_csv_type(field)
+    return columns
+
+
 def setup_s3_connection(con, server):
     s3_region = os.getenv("DATACONTRACT_S3_REGION")
     s3_access_key_id = os.getenv("DATACONTRACT_S3_ACCESS_KEY_ID")
     s3_secret_access_key = os.getenv("DATACONTRACT_S3_SECRET_ACCESS_KEY")
     # con.install_extension("httpfs")
     # con.load_extension("httpfs")
     if server.endpointUrl is not None:
```

### Comparing `datacontract-cli-0.9.8/datacontract/engines/soda/connections/kafka.py` & `datacontract_cli-0.9.9/datacontract/engines/soda/connections/kafka.py`

 * *Files identical despite different names*

### Comparing `datacontract-cli-0.9.8/datacontract/engines/soda/connections/postgres.py` & `datacontract_cli-0.9.9/datacontract/engines/soda/connections/postgres.py`

 * *Files identical despite different names*

### Comparing `datacontract-cli-0.9.8/datacontract/engines/soda/connections/snowflake.py` & `datacontract_cli-0.9.9/datacontract/engines/soda/connections/snowflake.py`

 * *Files identical despite different names*

### Comparing `datacontract-cli-0.9.8/datacontract/export/avro_converter.py` & `datacontract_cli-0.9.9/datacontract/export/avro_converter.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 import json
 
 from datacontract.model.data_contract_specification import Field
 
 
 def to_avro_schema(model_name, model) -> dict:
-    return to_avro_record(model_name, model.fields, model.description)
+    return to_avro_record(model_name, model.fields, model.description, model.namespace)
 
 
 def to_avro_schema_json(model_name, model) -> str:
     schema = to_avro_schema(model_name, model)
     return json.dumps(schema, indent=2, sort_keys=False)
 
 
-def to_avro_record(name, fields, description) -> dict:
+def to_avro_record(name, fields, description, namespace) -> dict:
     schema = {"type": "record", "name": name}
     if description is not None:
         schema["doc"] = description
+    if namespace is not None:
+        schema["namespace"] = namespace
     schema["fields"] = to_avro_fields(fields)
     return schema
 
 
 def to_avro_fields(fields):
     result = []
     for field_name, field in fields.items():
@@ -31,15 +33,15 @@
     avro_field = {"name": field_name}
     if field.description is not None:
         avro_field["doc"] = field.description
     avro_field["type"] = to_avro_type(field, field_name)
     return avro_field
 
 
-def to_avro_type(field: Field, field_name: str):
+def to_avro_type(field: Field, field_name: str) -> str | dict:
     if field.type is None:
         return "null"
     if field.type in ["string", "varchar", "text"]:
         return "string"
     elif field.type in ["number", "decimal", "numeric"]:
         # https://avro.apache.org/docs/1.11.1/specification/#decimal
         return "bytes"
@@ -56,15 +58,15 @@
     elif field.type in ["timestamp_ntz"]:
         return "string"
     elif field.type in ["date"]:
         return "int"
     elif field.type in ["time"]:
         return "long"
     elif field.type in ["object", "record", "struct"]:
-        return to_avro_record(field_name, field.fields, field.description)
+        return to_avro_record(field_name, field.fields, field.description, None)
     elif field.type in ["binary"]:
         return "bytes"
     elif field.type in ["array"]:
         # TODO support array structs
         return "array"
     elif field.type in ["null"]:
         return "null"
```

### Comparing `datacontract-cli-0.9.8/datacontract/export/avro_idl_converter.py` & `datacontract_cli-0.9.9/datacontract/export/avro_idl_converter.py`

 * *Files identical despite different names*

### Comparing `datacontract-cli-0.9.8/datacontract/export/dbt_converter.py` & `datacontract_cli-0.9.9/datacontract/export/dbt_converter.py`

 * *Files identical despite different names*

### Comparing `datacontract-cli-0.9.8/datacontract/export/great_expectations_converter.py` & `datacontract_cli-0.9.9/datacontract/export/great_expectations_converter.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,15 @@
         add_field_expectations(field_name, field, expectations)
     return expectations
 
 
 def add_field_expectations(field_name, field: Field, expectations: List[Dict[str, Any]]) -> List[Dict[str, Any]]:
     if field.type is not None:
         expectations.append(to_column_types_exp(field_name, field.type))
-    if field.unique is not None:
+    if field.unique:
         expectations.append(to_column_unique_exp(field_name))
     if field.maxLength is not None or field.minLength is not None:
         expectations.append(to_column_length_exp(field_name, field.minLength, field.maxLength))
     if field.minimum is not None or field.maximum is not None:
         expectations.append(to_column_min_max_exp(field_name, field.minimum, field.maximum))
 
     # TODO: all constraints
```

### Comparing `datacontract-cli-0.9.8/datacontract/export/jsonschema_converter.py` & `datacontract_cli-0.9.9/datacontract/export/jsonschema_converter.py`

 * *Files identical despite different names*

### Comparing `datacontract-cli-0.9.8/datacontract/export/odcs_converter.py` & `datacontract_cli-0.9.9/datacontract/export/odcs_converter.py`

 * *Files identical despite different names*

### Comparing `datacontract-cli-0.9.8/datacontract/export/protobuf_converter.py` & `datacontract_cli-0.9.9/datacontract/export/protobuf_converter.py`

 * *Files identical despite different names*

### Comparing `datacontract-cli-0.9.8/datacontract/export/pydantic_converter.py` & `datacontract_cli-0.9.9/datacontract/export/pydantic_converter.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,74 +1,75 @@
-import datacontract.model.data_contract_specification as spec
-import typing
 import ast
+import typing
+
+import datacontract.model.data_contract_specification as spec
+
 
 def to_pydantic_model_str(contract: spec.DataContractSpecification) -> str:
     classdefs = [generate_model_class(model_name, model) for (model_name, model) in contract.models.items()]
-    documentation = [ast.Expr(ast.Constant(contract.info.description))] if (
-        contract.info and contract.info.description) else []
-    result = ast.Module(body=[
-        ast.Import(
-            names=[ast.Name("datetime", ctx=ast.Load()),
-                   ast.Name("typing", ctx=ast.Load()),
-                   ast.Name("pydantic", ctx=ast.Load())]),
-        *documentation,
-        *classdefs],
-        type_ignores=[])
+    documentation = (
+        [ast.Expr(ast.Constant(contract.info.description))] if (contract.info and contract.info.description) else []
+    )
+    result = ast.Module(
+        body=[
+            ast.Import(
+                names=[
+                    ast.Name("datetime", ctx=ast.Load()),
+                    ast.Name("typing", ctx=ast.Load()),
+                    ast.Name("pydantic", ctx=ast.Load()),
+                ]
+            ),
+            *documentation,
+            *classdefs,
+        ],
+        type_ignores=[],
+    )
     return ast.unparse(result)
 
+
 def optional_of(node) -> ast.Subscript:
     return ast.Subscript(
-        value=ast.Attribute(
-            ast.Name(id="typing", ctx=ast.Load()),
-            attr="Optional",
-            ctx=ast.Load()),
-        slice=node)
+        value=ast.Attribute(ast.Name(id="typing", ctx=ast.Load()), attr="Optional", ctx=ast.Load()), slice=node
+    )
+
 
 def list_of(node) -> ast.Subscript:
-    return ast.Subscript(
-        value=ast.Name(id="list", ctx=ast.Load()),
-        slice=node)
+    return ast.Subscript(value=ast.Name(id="list", ctx=ast.Load()), slice=node)
+
 
 def product_of(nodes: list[typing.Any]) -> ast.Subscript:
     return ast.Subscript(
-        value=ast.Attribute(
-            value=ast.Name(id="typing", ctx=ast.Load()),
-            attr="Product",
-            ctx=ast.Load()),
-        slice=ast.Tuple(nodes, ctx=ast.Load())
+        value=ast.Attribute(value=ast.Name(id="typing", ctx=ast.Load()), attr="Product", ctx=ast.Load()),
+        slice=ast.Tuple(nodes, ctx=ast.Load()),
     )
 
 
 type_annotation_type = typing.Union[ast.Name, ast.Attribute, ast.Constant, ast.Subscript]
 
-def constant_field_annotation(field_name: str, field: spec.Field)\
-        -> tuple[type_annotation_type,
-                 typing.Optional[ast.ClassDef]]:
+
+def constant_field_annotation(
+    field_name: str, field: spec.Field
+) -> tuple[type_annotation_type, typing.Optional[ast.ClassDef]]:
     match field.type:
-        case "string"|"text"|"varchar":
+        case "string" | "text" | "varchar":
             return (ast.Name("str", ctx=ast.Load()), None)
         case "number", "decimal", "numeric":
             # Either integer or float in specification,
             # so we use float.
             return (ast.Name("float", ctx=ast.Load()), None)
         case "int" | "integer" | "long" | "bigint":
             return (ast.Name("int", ctx=ast.Load()), None)
         case "float" | "double":
             return (ast.Name("float", ctx=ast.Load()), None)
         case "boolean":
             return (ast.Name("bool", ctx=ast.Load()), None)
         case "timestamp" | "timestamp_tz" | "timestamp_ntz":
-            return (ast.Attribute(
-                value=ast.Name(id="datetime", ctx=ast.Load()),
-                attr="datetime"), None)
+            return (ast.Attribute(value=ast.Name(id="datetime", ctx=ast.Load()), attr="datetime"), None)
         case "date":
-            return (ast.Attribute(
-                value=ast.Name(id="datetime", ctx=ast.Load()),
-                attr="date"), None)
+            return (ast.Attribute(value=ast.Name(id="datetime", ctx=ast.Load()), attr="date"), None)
         case "bytes":
             return (ast.Name("bytes", ctx=ast.Load()), None)
         case "null":
             return (ast.Constant("None"), None)
         case "array":
             (annotated_type, new_class) = type_annotation(field_name, field.items)
             return (list_of(annotated_type), new_class)
@@ -82,59 +83,49 @@
 def type_annotation(field_name: str, field: spec.Field) -> tuple[type_annotation_type, typing.Optional[ast.ClassDef]]:
     if field.required:
         return constant_field_annotation(field_name, field)
     else:
         (annotated_type, new_classes) = constant_field_annotation(field_name, field)
         return (optional_of(annotated_type), new_classes)
 
+
 def is_simple_field(field: spec.Field) -> bool:
     return field.type not in set(["object", "record", "struct"])
 
-def field_definitions(fields: dict[str, spec.Field]) ->\
-        tuple[list[ast.Expr],
-              list[ast.ClassDef]]:
+
+def field_definitions(fields: dict[str, spec.Field]) -> tuple[list[ast.Expr], list[ast.ClassDef]]:
     annotations = []
     classes = []
-    for (field_name, field) in fields.items():
+    for field_name, field in fields.items():
         (ann, new_class) = type_annotation(field_name, field)
-        annotations.append(
-            ast.AnnAssign(
-                target=ast.Name(id=field_name, ctx=ast.Store()),
-                annotation=ann,
-                simple=1))
+        annotations.append(ast.AnnAssign(target=ast.Name(id=field_name, ctx=ast.Store()), annotation=ann, simple=1))
         if field.description and is_simple_field(field):
-            annotations.append(
-                ast.Expr(ast.Constant(field.description)))
+            annotations.append(ast.Expr(ast.Constant(field.description)))
         if new_class:
             classes.append(new_class)
     return (annotations, classes)
 
+
 def generate_field_class(field_name: str, field: spec.Field) -> ast.ClassDef:
-    assert(field.type in set(["object", "record", "struct"]))
+    assert field.type in set(["object", "record", "struct"])
     (annotated_type, new_classes) = field_definitions(field.fields)
     documentation = [ast.Expr(ast.Constant(field.description))] if field.description else []
     return ast.ClassDef(
         name=field_name,
-        bases=[ast.Attribute(value=ast.Name(id="pydantic", ctx=ast.Load()),
-                             attr="BaseModel",
-                             ctx=ast.Load())],
-        body=[
-            *documentation,
-            *new_classes,
-            *annotated_type
-        ],
+        bases=[ast.Attribute(value=ast.Name(id="pydantic", ctx=ast.Load()), attr="BaseModel", ctx=ast.Load())],
+        body=[*documentation, *new_classes, *annotated_type],
         keywords=[],
-        decorator_list=[])
+        decorator_list=[],
+    )
 
 
 def generate_model_class(name: str, model_definition: spec.Model) -> ast.ClassDef:
     (field_assignments, nested_classes) = field_definitions(model_definition.fields)
     documentation = [ast.Expr(ast.Constant(model_definition.description))] if model_definition.description else []
     result = ast.ClassDef(
         name=name.capitalize(),
-        bases=[ast.Attribute(value=ast.Name(id="pydantic", ctx=ast.Load()),
-                             attr="BaseModel",
-                             ctx=ast.Load())],
+        bases=[ast.Attribute(value=ast.Name(id="pydantic", ctx=ast.Load()), attr="BaseModel", ctx=ast.Load())],
         body=[*documentation, *nested_classes, *field_assignments],
         keywords=[],
-        decorator_list=[])
+        decorator_list=[],
+    )
     return result
```

### Comparing `datacontract-cli-0.9.8/datacontract/export/rdf_converter.py` & `datacontract_cli-0.9.9/datacontract/export/rdf_converter.py`

 * *Files identical despite different names*

### Comparing `datacontract-cli-0.9.8/datacontract/export/sql_converter.py` & `datacontract_cli-0.9.9/datacontract/export/sql_converter.py`

 * *Files 5% similar despite different names*

```diff
@@ -81,13 +81,24 @@
     for field_name, field in iter(model.fields.items()):
         type = convert_to_sql_type(field, server_type)
         result += f"  {field_name} {type}"
         if field.required:
             result += " not null"
         if field.primary:
             result += " primary key"
+        if server_type == "databricks" and field.description is not None:
+            result += f' COMMENT "{_escape(field.description)}"'
         if current_field_index < fields:
             result += ","
         result += "\n"
         current_field_index += 1
-    result += ");\n"
+    result += ")"
+    if server_type == "databricks" and model.description is not None:
+        result += f' COMMENT "{_escape(model.description)}"'
+    result += ";\n"
     return result
+
+
+def _escape(text: str | None) -> str | None:
+    if text is None:
+        return None
+    return text.replace('"', '\\"')
```

### Comparing `datacontract-cli-0.9.8/datacontract/export/sql_type_converter.py` & `datacontract_cli-0.9.9/datacontract/export/sql_type_converter.py`

 * *Files identical despite different names*

### Comparing `datacontract-cli-0.9.8/datacontract/export/terraform_converter.py` & `datacontract_cli-0.9.9/datacontract/export/terraform_converter.py`

 * *Files identical despite different names*

### Comparing `datacontract-cli-0.9.8/datacontract/imports/sql_importer.py` & `datacontract_cli-0.9.9/datacontract/imports/sql_importer.py`

 * *Files identical despite different names*

### Comparing `datacontract-cli-0.9.8/datacontract/integration/publish_opentelemetry.py` & `datacontract_cli-0.9.9/datacontract/integration/publish_opentelemetry.py`

 * *Files identical despite different names*

### Comparing `datacontract-cli-0.9.8/datacontract/lint/lint.py` & `datacontract_cli-0.9.9/datacontract/lint/lint.py`

 * *Files identical despite different names*

### Comparing `datacontract-cli-0.9.8/datacontract/lint/linters/description_linter.py` & `datacontract_cli-0.9.9/datacontract/lint/linters/description_linter.py`

 * *Files identical despite different names*

### Comparing `datacontract-cli-0.9.8/datacontract/lint/linters/example_model_linter.py` & `datacontract_cli-0.9.9/datacontract/lint/linters/example_model_linter.py`

 * *Files identical despite different names*

### Comparing `datacontract-cli-0.9.8/datacontract/lint/linters/field_pattern_linter.py` & `datacontract_cli-0.9.9/datacontract/lint/linters/field_pattern_linter.py`

 * *Files identical despite different names*

### Comparing `datacontract-cli-0.9.8/datacontract/lint/linters/field_reference_linter.py` & `datacontract_cli-0.9.9/datacontract/lint/linters/field_reference_linter.py`

 * *Files identical despite different names*

### Comparing `datacontract-cli-0.9.8/datacontract/lint/linters/notice_period_linter.py` & `datacontract_cli-0.9.9/datacontract/lint/linters/notice_period_linter.py`

 * *Files identical despite different names*

### Comparing `datacontract-cli-0.9.8/datacontract/lint/linters/quality_schema_linter.py` & `datacontract_cli-0.9.9/datacontract/lint/linters/quality_schema_linter.py`

 * *Files identical despite different names*

### Comparing `datacontract-cli-0.9.8/datacontract/lint/linters/valid_constraints_linter.py` & `datacontract_cli-0.9.9/datacontract/lint/linters/valid_constraints_linter.py`

 * *Files identical despite different names*

### Comparing `datacontract-cli-0.9.8/datacontract/lint/resolve.py` & `datacontract_cli-0.9.9/datacontract/lint/resolve.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import logging
+import os
 
 import fastjsonschema
 import yaml
 from fastjsonschema import JsonSchemaValueException
 
 from datacontract.lint.files import read_file
 from datacontract.lint.schema import fetch_schema
 from datacontract.lint.urls import fetch_resource
 from datacontract.model.data_contract_specification import \
-    DataContractSpecification, Definition
+    DataContractSpecification, Definition, Quality
 from datacontract.model.exceptions import DataContractException
 
 
 def resolve_data_contract(
     data_contract_location: str = None,
     data_contract_str: str = None,
     data_contract: DataContractSpecification = None,
@@ -32,39 +33,39 @@
             name="Check that data contract YAML is valid",
             reason="Data contract needs to be provided",
             engine="datacontract",
         )
 
 
 def resolve_data_contract_from_location(
-    location, schema_location: str = None, inline_definitions: bool = False
+    location, schema_location: str = None, inline_definitions: bool = False, include_quality: bool = True
 ) -> DataContractSpecification:
     if location.startswith("http://") or location.startswith("https://"):
         data_contract_str = fetch_resource(location)
     else:
         data_contract_str = read_file(location)
-    return resolve_data_contract_from_str(data_contract_str, schema_location, inline_definitions)
+    return resolve_data_contract_from_str(data_contract_str, schema_location, inline_definitions, include_quality)
 
 
 def inline_definitions_into_data_contract(spec: DataContractSpecification):
     for model in spec.models.values():
         for field in model.fields.values():
             # If ref_obj is not empty, we've already inlined definitions.
             if not field.ref and not field.ref_obj:
                 continue
 
-            definition = resolve_ref(field.ref, spec.definitions)
+            definition = resolve_definition_ref(field.ref, spec.definitions)
             field.ref_obj = definition
 
             for field_name in field.model_fields.keys():
                 if field_name in definition.model_fields_set and field_name not in field.model_fields_set:
                     setattr(field, field_name, getattr(definition, field_name))
 
 
-def resolve_ref(ref, definitions) -> Definition:
+def resolve_definition_ref(ref, definitions) -> Definition:
     if ref.startswith("http://") or ref.startswith("https://"):
         definition_str = fetch_resource(ref)
         definition_dict = to_yaml(definition_str)
         return Definition(**definition_dict)
 
     elif ref.startswith("#/definitions/"):
         definition_name = ref.split("#/definitions/")[1]
@@ -75,24 +76,62 @@
             result="failed",
             name="Check that data contract YAML is valid",
             reason=f"Cannot resolve reference {ref}",
             engine="datacontract",
         )
 
 
+def resolve_quality_ref(quality: Quality):
+    """
+    Return the content of a ref file path
+    @param quality data contract quality specification
+    """
+    if isinstance(quality.specification, dict):
+        specification = quality.specification
+        if quality.type == "great-expectations":
+            for model, model_quality in specification.items():
+                specification[model] = get_quality_ref_file(model_quality)
+        else:
+            if "$ref" in specification:
+                quality.specification = get_quality_ref_file(specification)
+
+
+def get_quality_ref_file(quality_spec: str | object) -> str | object:
+    """
+    Get the file associated with a quality reference
+    @param quality_spec quality specification
+    @returns: the content of the quality file
+    """
+    if isinstance(quality_spec, dict) and "$ref" in quality_spec:
+        ref = quality_spec["$ref"]
+        if not os.path.exists(ref):
+            raise DataContractException(
+                type="export",
+                result="failed",
+                name="Check that data contract quality is valid",
+                reason=f"Cannot resolve reference {ref}",
+                engine="datacontract",
+            )
+        with open(ref, "r") as file:
+            quality_spec = file.read()
+    return quality_spec
+
+
 def resolve_data_contract_from_str(
-    data_contract_str, schema_location: str = None, inline_definitions: bool = False
+    data_contract_str, schema_location: str = None, inline_definitions: bool = False, include_quality: bool = False
 ) -> DataContractSpecification:
     data_contract_yaml_dict = to_yaml(data_contract_str)
     validate(data_contract_yaml_dict, schema_location)
 
     spec = DataContractSpecification(**data_contract_yaml_dict)
 
     if inline_definitions:
         inline_definitions_into_data_contract(spec)
+    if spec.quality and include_quality:
+        resolve_quality_ref(spec.quality)
 
     return spec
 
 
 def to_yaml(data_contract_str):
     try:
         yaml_dict = yaml.safe_load(data_contract_str)
```

### Comparing `datacontract-cli-0.9.8/datacontract/lint/schema.py` & `datacontract_cli-0.9.9/datacontract/lint/schema.py`

 * *Files identical despite different names*

### Comparing `datacontract-cli-0.9.8/datacontract/lint/urls.py` & `datacontract_cli-0.9.9/datacontract/lint/urls.py`

 * *Files identical despite different names*

### Comparing `datacontract-cli-0.9.8/datacontract/model/breaking_change.py` & `datacontract_cli-0.9.9/datacontract/model/breaking_change.py`

 * *Files identical despite different names*

### Comparing `datacontract-cli-0.9.8/datacontract/model/data_contract_specification.py` & `datacontract_cli-0.9.9/datacontract/model/data_contract_specification.py`

 * *Files identical despite different names*

### Comparing `datacontract-cli-0.9.8/datacontract/model/exceptions.py` & `datacontract_cli-0.9.9/datacontract/model/exceptions.py`

 * *Files identical despite different names*

### Comparing `datacontract-cli-0.9.8/datacontract/model/run.py` & `datacontract_cli-0.9.9/datacontract/model/run.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
     name: Optional[str]
     result: str  # passed, failed, warning, unknown
     engine: str
     reason: Optional[str] = None
     model: Optional[str] = None
     field: Optional[str] = None
     details: Optional[str] = None
+    diagnostics: Optional[dict] = None
 
 
 class Log(BaseModel):
     level: str
     message: str
     timestamp: datetime
 
@@ -65,15 +66,15 @@
         self.logs.append(Log(level="WARN", message=message, timestamp=datetime.now(timezone.utc)))
 
     def log_error(self, message: str):
         logging.error(message)
         self.logs.append(Log(level="ERROR", message=message, timestamp=datetime.now(timezone.utc)))
 
     def pretty(self):
-        return self.model_dump_json()
+        return self.model_dump_json(indent=2)
 
     @staticmethod
     def create_run():
         """
         Factory method to create a new Run instance.
 
         :return: An instance of Run.
```

### Comparing `datacontract-cli-0.9.8/datacontract_cli.egg-info/PKG-INFO` & `datacontract_cli-0.9.9/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: datacontract-cli
-Version: 0.9.8
+Version: 0.9.9
 Summary: Test data contracts
 Author-email: Jochen Christ <jochen.christ@innoq.com>, Stefan Negele <stefan.negele@innoq.com>
 Project-URL: Homepage, https://cli.datacontract.com
 Project-URL: Issues, https://github.com/datacontract/cli/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: typer[all]<0.13,>=0.9
-Requires-Dist: pydantic<2.7.0,>=2.5.3
+Requires-Dist: pydantic<2.8.0,>=2.5.3
 Requires-Dist: pyyaml~=6.0.1
 Requires-Dist: requests~=2.31.0
-Requires-Dist: fastapi==0.110.0
+Requires-Dist: fastapi==0.110.1
 Requires-Dist: fastparquet==2024.2.0
 Requires-Dist: python-multipart==0.0.9
 Requires-Dist: rich~=13.7.0
 Requires-Dist: simple-ddl-parser==1.0.4
 Requires-Dist: soda-core-bigquery<3.4.0,>=3.3.1
 Requires-Dist: soda-core-duckdb<3.4.0,>=3.3.1
 Requires-Dist: soda-core-postgres<3.4.0,>=3.3.1
@@ -35,14 +35,15 @@
 Requires-Dist: avro==1.11.3
 Requires-Dist: opentelemetry-exporter-otlp-proto-grpc~=1.16.0
 Requires-Dist: opentelemetry-exporter-otlp-proto-http~=1.16.0
 Provides-Extra: dev
 Requires-Dist: httpx==0.27.0; extra == "dev"
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
+Requires-Dist: pytest-xdist; extra == "dev"
 Requires-Dist: testcontainers<4.0; extra == "dev"
 Requires-Dist: testcontainers-minio; extra == "dev"
 Requires-Dist: testcontainers-postgres; extra == "dev"
 Requires-Dist: testcontainers-kafka; extra == "dev"
 
 # Data Contract CLI
 
@@ -55,29 +56,21 @@
 </p>
 
 The `datacontract` CLI is an open source command-line tool for working with [Data Contracts](https://datacontract.com/).
 It uses data contract YAML files to lint the data contract, connect to data sources and execute schema and quality tests, detect breaking changes, and export to different formats. The tool is written in Python. It can be used as a standalone CLI tool, in a CI/CD pipeline, or directly as a Python library.
 
 ![Main features of the Data Contract CLI](datacontractcli.png)
 
-<div align="center">
-  <a href="https://www.youtube.com/watch?v=B1dixhgO2vQ">
- <img 
-  src="https://img.youtube.com/vi/B1dixhgO2vQ/0.jpg" 
-  alt="Demo of Data Contract CLI" 
-  style="width:100%;">
-  </a>
-</div>
 
 ## Getting started
 
-Let's look at this data contract:
+Let's look at this data contract:  
 [https://datacontract.com/examples/orders-latest/datacontract.yaml](https://datacontract.com/examples/orders-latest/datacontract.yaml)
 
-We have a _servers_ section with endpoint details to the S3 bucket, _models_ for the structure of the data, and _quality_ attributes that describe the expected freshness and number of rows.
+We have a _servers_ section with endpoint details to the S3 bucket, _models_ for the structure of the data, _servicelevels_ and _quality_ attributes that describe the expected freshness and number of rows.
 
 This data contract contains all information to connect to S3 and check that the actual data meets the defined schema and quality requirements. We can use this information to test if the actual data set in S3 is compliant to the data contract.
 
 Let's use [pip](https://pip.pypa.io/en/stable/getting-started/) to install the CLI (or use the [Docker image](#docker), if you prefer).
 ```bash
 $ python3 -m pip install datacontract-cli
 ```
@@ -116,14 +109,39 @@
 │ passed │ Check that unique field lines_item_id has no duplicate values       │ line_items.lines_item_id      │         │
 ╰────────┴─────────────────────────────────────────────────────────────────────┴───────────────────────────────┴─────────╯
 🟢 data contract is valid. Run 22 checks. Took 6.739514 seconds.
 ```
 
 Voilà, the CLI tested that the _datacontract.yaml_ itself is valid, all records comply with the schema, and all quality attributes are met.
 
+We can also use the datacontract.yaml to export in many [formats](#format), e.g., to SQL:
+
+```bash
+$ datacontract export --format sql https://datacontract.com/examples/orders-latest/datacontract.yaml
+
+# returns:
+-- Data Contract: urn:datacontract:checkout:orders-latest
+-- SQL Dialect: snowflake
+CREATE TABLE orders (
+  order_id TEXT not null primary key,
+  order_timestamp TIMESTAMP_TZ not null,
+  order_total NUMBER not null,
+  customer_id TEXT,
+  customer_email_address TEXT not null,
+  processed_timestamp TIMESTAMP_TZ not null
+);
+CREATE TABLE line_items (
+  lines_item_id TEXT not null primary key,
+  order_id TEXT,
+  sku TEXT
+);
+```
+
+Or generate this [HTML page](https://datacontract.com/examples/orders-latest/datacontract.html).
+
 ## Usage
 
 ```bash
 # create a new data contract from example and write it to datacontract.yaml
 $ datacontract init datacontract.yaml
 
 # lint the datacontract.yaml
@@ -131,90 +149,41 @@
 
 # execute schema and quality checks
 $ datacontract test datacontract.yaml
 
 # execute schema and quality checks on the examples within the contract
 $ datacontract test --examples datacontract.yaml
 
-# find differences between to data contracts (Coming Soon)
+# export data contract as html (other formats: avro, dbt, dbt-sources, dbt-staging-sql, jsonschema, odcs, rdf, sql, sodacl, terraform, ...)
+$ datacontract export --format html datacontract.yaml > datacontract.html
+
+# import avro (other formats: sql, ...)
+$ datacontract import --format avro --source avro_schema.avsc
+
+# find differences between to data contracts
 $ datacontract diff datacontract-v1.yaml datacontract-v2.yaml
 
 # find differences between to data contracts categorized into error, warning, and info.
 $ datacontract changelog datacontract-v1.yaml datacontract-v2.yaml
 
 # fail pipeline on breaking changes. Uses changelog internally and showing only error and warning.
 $ datacontract breaking datacontract-v1.yaml datacontract-v2.yaml
-
-# export model as jsonschema (other formats: avro, dbt, dbt-sources, dbt-staging-sql, jsonschema, odcs, rdf, sql (coming soon), sodacl, terraform)
-$ datacontract export --format jsonschema datacontract.yaml
-
-# import sql
-$ datacontract import --format sql --source my_ddl.sql
-
-# import avro
-$ datacontract import --format avro --source avro_schema.avsc
 ```
 
 ## Programmatic (Python)
 ```python
 from datacontract.data_contract import DataContract
 
 data_contract = DataContract(data_contract_file="datacontract.yaml")
 run = data_contract.test()
 if not run.has_passed():
     print("Data quality validation failed.")
     # Abort pipeline, alert, or take corrective actions...
 ```
 
-## Integrations
-
-
-| Integration       | Option                       | Description                                                                                           |
-|-------------------|------------------------------|-------------------------------------------------------------------------------------------------------|
-| Data Mesh Manager | `--publish`                  | Push full results to the [Data Mesh Manager API](https://api.datamesh-manager.com/swagger/index.html) |
-| OpenTelemetry     | `--publish-to-opentelemetry` | Push result as gauge metrics (logs are planned)                                                       |
-
-### Integration with Data Mesh Manager
-
-If you use [Data Mesh Manager](https://datamesh-manager.com/), you can use the data contract URL and append the `--publish` option to send and display the test results. Set an environment variable for your API key.
-
-```bash
-# Fetch current data contract, execute tests on production, and publish result to data mesh manager
-$ EXPORT DATAMESH_MANAGER_API_KEY=xxx
-$ datacontract test https://demo.datamesh-manager.com/demo279750347121/datacontracts/4df9d6ee-e55d-4088-9598-b635b2fdcbbc/datacontract.yaml --server production --publish
-```
-
-### Integration with OpenTelemetry
-
-If you use OpenTelemetry, you can use the data contract URL and append the `--publish-to-opentelemetry` option to send the test results to your OLTP-compatible instance, e.g., Prometheus.
-
-The metric name is "datacontract.cli.test.result" and it uses the following encoding for the result:
-
-| datacontract.cli.test.result | Description                           |
-|-------|---------------------------------------|
-| 0     | test run passed, no warnings          |
-| 1     | test run has warnings                 |
-| 2     | test run failed                       |
-| 3     | test run not possible due to an error |
-| 4     | test status unknown                   |
-
-
-```bash
-# Fetch current data contract, execute tests on production, and publish result to open telemetry
-$ EXPORT OTEL_SERVICE_NAME=datacontract-cli
-$ EXPORT OTEL_EXPORTER_OTLP_ENDPOINT=https://YOUR_ID.apm.westeurope.azure.elastic-cloud.com:443
-$ EXPORT OTEL_EXPORTER_OTLP_HEADERS=Authorization=Bearer%20secret # Optional, when using SaaS Products
-$ EXPORT OTEL_EXPORTER_OTLP_PROTOCOL=http/protobuf # Optional, default is http/protobuf - use value grpc to use the gRPC protocol instead
-# Send to OpenTelemetry
-$ datacontract test https://demo.datamesh-manager.com/demo279750347121/datacontracts/4df9d6ee-e55d-4088-9598-b635b2fdcbbc/datacontract.yaml --server production --publish-to-opentelemetry
-```
-
-Current limitations:
-- currently, only ConsoleExporter and OTLP Exporter
-- Metrics only, no logs yet (but loosely planned)
 
 ## Installation
 
 Choose the most appropriate installation method for your needs:
 
 ### pip
 Python 3.11 recommended.
@@ -241,44 +210,128 @@
 
 ```bash
 alias datacontract='docker run --rm -v "${PWD}:/home/datacontract" datacontract/cli:latest'
 ```
 
 ## Documentation
 
-### Tests
+Commands
+
+- [init](#init)
+- [lint](#lint)
+- [test](#test)
+- [export](#export)
+- [import](#import)
+- [breaking](#breaking)
+- [changelog](#changelog)
+- [diff](#diff)
+
+### init
+
+```                                                                                                
+ Usage: datacontract init [OPTIONS] [LOCATION]                                                  
+                                                                                                
+ Download a datacontract.yaml template and write it to file.                                    
+                                                                                                
+╭─ Arguments ──────────────────────────────────────────────────────────────────────────────────╮
+│   location      [LOCATION]  The location (url or path) of the data contract yaml to create.  │
+│                             [default: datacontract.yaml]                                     │
+╰──────────────────────────────────────────────────────────────────────────────────────────────╯
+╭─ Options ────────────────────────────────────────────────────────────────────────────────────╮
+│ --template                       TEXT  URL of a template or data contract                    │
+│                                        [default:                                             │
+│                                        https://datacontract.com/datacontract.init.yaml]      │
+│ --overwrite    --no-overwrite          Replace the existing datacontract.yaml                │
+│                                        [default: no-overwrite]                               │
+│ --help                                 Show this message and exit.                           │
+╰──────────────────────────────────────────────────────────────────────────────────────────────╯
+```
+
+### lint
+
+```
+ Usage: datacontract lint [OPTIONS] [LOCATION]                                                                                     
+                                                                                                                                   
+ Validate that the datacontract.yaml is correctly formatted.                                                                       
+                                                                                                                                   
+╭─ Arguments ─────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╮
+│   location      [LOCATION]  The location (url or path) of the data contract yaml. [default: datacontract.yaml]                  │
+╰─────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
+╭─ Options ───────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╮
+│ --schema        TEXT  The location (url or path) of the Data Contract Specification JSON Schema                                 │
+│                       [default: https://datacontract.com/datacontract.schema.json]                                              │
+│ --help                Show this message and exit.                                                                               │
+╰─────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
+```
+
+### test
+
+```
+ Usage: datacontract test [OPTIONS] [LOCATION]                                                                                     
+                                                                                                                                   
+ Run schema and quality tests on configured servers.                                                                               
+                                                                                                                                   
+╭─ Arguments ─────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╮
+│   location      [LOCATION]  The location (url or path) of the data contract yaml. [default: datacontract.yaml]                  │
+╰─────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
+╭─ Options ───────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╮
+│ --schema                                                       TEXT  The location (url or path) of the Data Contract            │
+│                                                                      Specification JSON Schema                                  │
+│                                                                      [default:                                                  │
+│                                                                      https://datacontract.com/datacontract.schema.json]         │
+│ --server                                                       TEXT  The server configuration to run the schema and quality     │
+│                                                                      tests. Use the key of the server object in the data        │
+│                                                                      contract yaml file to refer to a server, e.g.,             │
+│                                                                      `production`, or `all` for all servers (default).          │
+│                                                                      [default: all]                                             │
+│ --examples                    --no-examples                          Run the schema and quality tests on the example data       │
+│                                                                      within the data contract.                                  │
+│                                                                      [default: no-examples]                                     │
+│ --publish                                                      TEXT  The url to publish the results after the test              │
+│                                                                      [default: None]                                            │
+│ --publish-to-opentelemetry    --no-publish-to-opentelemetry          Publish the results to opentelemetry. Use environment      │
+│                                                                      variables to configure the OTLP endpoint, headers, etc.    │
+│                                                                      [default: no-publish-to-opentelemetry]                     │
+│ --logs                        --no-logs                              Print logs [default: no-logs]                              │
+│ --help                                                               Show this message and exit.                                │
+╰─────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
+```
 
 Data Contract CLI can connect to data sources and run schema and quality tests to verify that the data contract is valid.
 
 ```bash
 $ datacontract test --server production datacontract.yaml
 ```
 
 To connect to the databases the `server` block in the datacontract.yaml is used to set up the connection. In addition, credentials, such as username and passwords, may be defined with environment variables.
 
 The application uses different engines, based on the server `type`.
+Internally, it connects with DuckDB, Spark, or a native connection and executes the most tests with soda-core and fastjsonschema. 
+Credentials are read from the environment variables.
 
-| Type         | Format     | Description                                                               | Status      | Engines                             |
-|--------------|------------|---------------------------------------------------------------------------|-------------|-------------------------------------|
-| `s3`         | `parquet`  | Works for any S3-compliant endpoint., e.g., AWS S3, GCS, MinIO, Ceph, ... | ✅           | soda-core-duckdb                    |
-| `s3`         | `json`     | Support for `new_line` delimited JSON files and one JSON record per file. | ✅           | fastjsonschema<br> soda-core-duckdb |
-| `s3`         | `csv`      |                                                                           | ✅           | soda-core-duckdb                    |
-| `s3`         | `delta`    |                                                                           | Coming soon | TBD                                 |
-| `postgres`   | n/a        |                                                                           | ✅           | soda-core-postgres                  |
-| `snowflake`  | n/a        |                                                                           | ✅           | soda-core-snowflake                 |
-| `bigquery`   | n/a        |                                                                           | ✅           | soda-core-bigquery                  |
-| `redshift`   | n/a        |                                                                           | Coming soon | TBD                                 |
-| `databricks` | n/a        | Support for Databricks SQL with Unity catalog and Hive metastore.         | ✅           | soda-core-spark                     |
-| `databricks` | n/a        | Support for Spark for programmatic use in Notebooks.                      | ✅           | soda-core-spark-df                  |
-| `kafka`      | `json`     | Experimental.                                                             | ✅           | pyspark<br>soda-core-spark-df       |
-| `kafka`      | `avro`     |                                                                           | Coming soon | TBD                                 |
-| `kafka`      | `protobuf` |                                                                           | Coming soon | TBD                                 |
-| `local`      | `parquet`  |                                                                           | ✅           | soda-core-duckdb                    |
-| `local`      | `json`     | Support for `new_line` delimited JSON files and one JSON record per file. | ✅           | fastjsonschema<br> soda-core-duckdb |
-| `local`      | `csv`      |                                                                           | ✅           | soda-core-duckdb                    |
+Supported server types:
+
+| Type         | Format     | Status                                                             |
+|--------------|------------|--------------------------------------------------------------------|
+| `s3`         | `parquet`  | ✅                                                                  |
+| `s3`         | `json`     | ✅                                                                  |
+| `s3`         | `csv`      | ✅                                                                  |
+| `s3`         | `delta`    | Coming soon ([#24](https://github.com/datacontract/cli/issues/24)) |
+| `s3`         | `iceberg`  | Coming soon                                                        |
+| `postgres`   | n/a        | ✅                                                                  |
+| `snowflake`  | n/a        | ✅                                                                  |
+| `bigquery`   | n/a        | ✅                                                                  |
+| `redshift`   | n/a        | Coming soon                                                        |
+| `databricks` | n/a        | ✅                                                                  |
+| `kafka`      | `json`     | ✅                                                                  |
+| `kafka`      | `avro`     | Coming soon                                                        |
+| `kafka`      | `protobuf` | Coming soon                                                        |
+| `local`      | `parquet`  | ✅                                                                  |
+| `local`      | `json`     | ✅                                                                  |
+| `local`      | `csv`      | ✅                                                                  |
 
 Feel free to create an issue, if you need support for an additional type.
 
 ### S3
 
 Data Contract CLI can test data that is stored in S3 buckets or any S3-compliant endpoints in various formats.
 
@@ -486,25 +539,54 @@
 | Environment Variable               | Example | Description                 |
 |------------------------------------|---------|-----------------------------|
 | `DATACONTRACT_KAFKA_SASL_USERNAME` | `xxx`   | The SASL username (key).    |
 | `DATACONTRACT_KAFKA_SASL_PASSWORD` | `xxx`   | The SASL password (secret). |
 
 
 
-### Exports
+### export
+
+```
+ Usage: datacontract export [OPTIONS] [LOCATION]                                                                                                                           
+                                                                                                                                                                           
+ Convert data contract to a specific format. console.prints to stdout.                                                                                                     
+                                                                                                                                                                           
+╭─ Arguments ─────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╮
+│   location      [LOCATION]  The location (url or path) of the data contract yaml. [default: datacontract.yaml]                                                          │
+╰─────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
+╭─ Options ───────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╮
+│ *  --format        [html|jsonschema|pydantic-model|sodacl|dbt|dbt-sources|dbt-staging-sql|odcs|rd  The export format. [default: None] [required]                             │
+│                    f|avro|protobuf|great-expectations|terraform|avro-idl|sql|sql-query]                                                                                 │
+│    --server        TEXT                                                                       The server name to export. [default: None]                                │
+│    --model         TEXT                                                                       Use the key of the model in the data contract yaml file to refer to a     │
+│                                                                                               model, e.g., `orders`, or `all` for all models (default).                 │
+│                                                                                               [default: all]                                                            │
+│    --help                                                                                     Show this message and exit.                                               │
+╰─────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
+╭─ RDF Options ───────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╮
+│ --rdf-base        TEXT  [rdf] The base URI used to generate the RDF graph. [default: None]                                                                              │
+╰─────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
+╭─ SQL Options ───────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╮
+│ --sql-server-type        TEXT  [sql] The server type to determine the sql dialect. By default, it uses 'auto' to automatically detect the sql dialect via the specified │
+│                                servers in the data contract.                                                                                                            │
+│                                [default: auto]                                                                                                                          │
+╰─────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
+
+```
 
 ```bash
-# Example export to dbt model
-datacontract export --format dbt
+# Example export data contract as HTML
+datacontract export --format html > datacontract.html
 ```
 
 Available export options:
 
 | Type                 | Description                                             | Status |
 |----------------------|---------------------------------------------------------|--------|
+| `html`               | Export to HTML                                          | ✅      | 
 | `jsonschema`         | Export to JSON Schema                                   | ✅      | 
 | `odcs`               | Export to Open Data Contract Standard (ODCS)            | ✅      | 
 | `sodacl`             | Export to SodaCL quality checks in YAML format          | ✅      |
 | `dbt`                | Export to dbt models in YAML format                     | ✅      |
 | `dbt-sources`        | Export to dbt sources in YAML format                    | ✅      |
 | `dbt-staging-sql`    | Export to dbt staging SQL models                        | ✅      |
 | `rdf`                | Export data contract to RDF representation in N3 format | ✅      |
@@ -512,23 +594,25 @@
 | `protobuf`           | Export to Protobuf                                      | ✅      |
 | `terraform`          | Export to terraform resources                           | ✅      |
 | `sql`                | Export to SQL DDL                                       | ✅      |
 | `sql-query`          | Export to SQL Query                                     | ✅      |
 | `great-expectations` | Export to Great Expectations Suites in JSON Format      | ✅      |
 | `bigquery`           | Export to BigQuery Schemas                              | TBD    |
 | `pydantic`           | Export to pydantic models                               | TBD    |
-| `html`               | Export to HTML page                                     | TBD    |
 | Missing something?   | Please create an issue on GitHub                        | TBD    |
 
 #### Great Expectations
+
 The export function transforms a specified data contract into a comprehensive Great Expectations JSON suite. 
 If the contract includes multiple models, you need to specify the names of the model you wish to export.
+
 ```shell
 datacontract  export datacontract.yaml --format great-expectations --model orders 
 ```
+
 The export creates a list of expectations by utilizing:
 
 - The data from the Model definition with a fixed mapping
 - The expectations provided in the quality field for each model (find here the expectations gallery https://greatexpectations.io/expectations/)
 
 #### RDF
 
@@ -550,16 +634,29 @@
 - Store data contracts inside a knowledge graph
 - Enhance a semantic search to find and retrieve data contracts
 - Linking model elements to already established ontologies and knowledge
 - Using full power of OWL to reason about the graph structure of data contracts
 - Apply graph algorithms on multiple data contracts (Find similar data contracts, find "gatekeeper"
 data products, find the true domain owner of a field attribute)
 
-### Imports
+### import
 
+```
+ Usage: datacontract import [OPTIONS]                                                                              
+                                                                                                                   
+ Create a data contract from the given source file. Prints to stdout.                                              
+                                                                                                                   
+╭─ Options ───────────────────────────────────────────────────────────────────────────────────────────────────────╮
+│ *  --format        [sql|avro]  The format of the source file. [default: None] [required]                        │
+│ *  --source        TEXT        The path to the file that should be imported. [default: None] [required]         │
+│    --help                      Show this message and exit.                                                      │
+╰─────────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
+```
+
+Example: 
 ```bash
 # Example import from SQL DDL
 datacontract import --format sql --source my_ddl.sql
 ```
 
 Available import options:
 
@@ -570,14 +667,111 @@
 | `protobuf`         | Import from Protobuf schemas                   | TBD     |
 | `jsonschema`       | Import from JSON Schemas                       | TBD     |
 | `bigquery`         | Import from BigQuery Schemas                   | TBD     |
 | `dbt`              | Import from dbt models                         | TBD     |
 | `odcs`             | Import from Open Data Contract Standard (ODCS) | TBD     |
 | Missing something? | Please create an issue on GitHub               | TBD     |
 
+
+### breaking
+
+```
+ Usage: datacontract breaking [OPTIONS] LOCATION_OLD LOCATION_NEW                                                            
+                                                                                                                             
+ Identifies breaking changes between data contracts. Prints to stdout.                                                       
+                                                                                                                             
+╭─ Arguments ───────────────────────────────────────────────────────────────────────────────────────────────────────────────╮
+│ *    location_old      TEXT  The location (url or path) of the old data contract yaml. [default: None] [required]         │
+│ *    location_new      TEXT  The location (url or path) of the new data contract yaml. [default: None] [required]         │
+╰───────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
+╭─ Options ─────────────────────────────────────────────────────────────────────────────────────────────────────────────────╮
+│ --help          Show this message and exit.                                                                               │
+╰───────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
+```
+
+### changelog
+
+```
+ Usage: datacontract changelog [OPTIONS] LOCATION_OLD LOCATION_NEW                                                           
+                                                                                                                             
+ Generate a changelog between data contracts. Prints to stdout.                                                              
+                                                                                                                             
+╭─ Arguments ───────────────────────────────────────────────────────────────────────────────────────────────────────────────╮
+│ *    location_old      TEXT  The location (url or path) of the old data contract yaml. [default: None] [required]         │
+│ *    location_new      TEXT  The location (url or path) of the new data contract yaml. [default: None] [required]         │
+╰───────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
+╭─ Options ─────────────────────────────────────────────────────────────────────────────────────────────────────────────────╮
+│ --help          Show this message and exit.                                                                               │
+╰───────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
+```
+
+### diff
+
+```
+ Usage: datacontract diff [OPTIONS] LOCATION_OLD LOCATION_NEW                                                                
+                                                                                                                             
+ PLACEHOLDER. Currently works as 'changelog' does.                                                                           
+                                                                                                                             
+╭─ Arguments ───────────────────────────────────────────────────────────────────────────────────────────────────────────────╮
+│ *    location_old      TEXT  The location (url or path) of the old data contract yaml. [default: None] [required]         │
+│ *    location_new      TEXT  The location (url or path) of the new data contract yaml. [default: None] [required]         │
+╰───────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
+╭─ Options ─────────────────────────────────────────────────────────────────────────────────────────────────────────────────╮
+│ --help          Show this message and exit.                                                                               │
+╰───────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
+```
+
+
+## Integrations
+
+| Integration       | Option                       | Description                                                                                           |
+|-------------------|------------------------------|-------------------------------------------------------------------------------------------------------|
+| Data Mesh Manager | `--publish`                  | Push full results to the [Data Mesh Manager API](https://api.datamesh-manager.com/swagger/index.html) |
+| OpenTelemetry     | `--publish-to-opentelemetry` | Push result as gauge metrics                                                                          |
+
+### Integration with Data Mesh Manager
+
+If you use [Data Mesh Manager](https://datamesh-manager.com/), you can use the data contract URL and append the `--publish` option to send and display the test results. Set an environment variable for your API key.
+
+```bash
+# Fetch current data contract, execute tests on production, and publish result to data mesh manager
+$ EXPORT DATAMESH_MANAGER_API_KEY=xxx
+$ datacontract test https://demo.datamesh-manager.com/demo279750347121/datacontracts/4df9d6ee-e55d-4088-9598-b635b2fdcbbc/datacontract.yaml --server production --publish
+```
+
+### Integration with OpenTelemetry
+
+If you use OpenTelemetry, you can use the data contract URL and append the `--publish-to-opentelemetry` option to send the test results to your OLTP-compatible instance, e.g., Prometheus.
+
+The metric name is "datacontract.cli.test.result" and it uses the following encoding for the result:
+
+| datacontract.cli.test.result | Description                           |
+|-------|---------------------------------------|
+| 0     | test run passed, no warnings          |
+| 1     | test run has warnings                 |
+| 2     | test run failed                       |
+| 3     | test run not possible due to an error |
+| 4     | test status unknown                   |
+
+
+```bash
+# Fetch current data contract, execute tests on production, and publish result to open telemetry
+$ EXPORT OTEL_SERVICE_NAME=datacontract-cli
+$ EXPORT OTEL_EXPORTER_OTLP_ENDPOINT=https://YOUR_ID.apm.westeurope.azure.elastic-cloud.com:443
+$ EXPORT OTEL_EXPORTER_OTLP_HEADERS=Authorization=Bearer%20secret # Optional, when using SaaS Products
+$ EXPORT OTEL_EXPORTER_OTLP_PROTOCOL=http/protobuf # Optional, default is http/protobuf - use value grpc to use the gRPC protocol instead
+# Send to OpenTelemetry
+$ datacontract test https://demo.datamesh-manager.com/demo279750347121/datacontracts/4df9d6ee-e55d-4088-9598-b635b2fdcbbc/datacontract.yaml --server production --publish-to-opentelemetry
+```
+
+Current limitations:
+- currently, only ConsoleExporter and OTLP Exporter
+- Metrics only, no logs yet (but loosely planned)
+
+
 ## Best Practices
 
 We share best practices in using the Data Contract CLI.
 
 ### Data-first Approach
 
 Create a data contract based on the actual data. This is the fastest way to get started and to get feedback from the data consumers.
@@ -693,33 +887,48 @@
 pip install --upgrade pip setuptools wheel
 pip install -e '.[dev]'
 ruff check --fix
 ruff format --check
 pytest
 ```
 
-Release
+
+### Docker Build
 
 ```bash
-git tag v0.9.0
-git push origin v0.9.0
-python3 -m pip install --upgrade build twine
-rm -r dist/
-python3 -m build
-# for now only test.pypi.org
-python3 -m twine upload --repository testpypi dist/*
+docker build -t datacontract/cli .
+docker run --rm -v ${PWD}:/home/datacontract datacontract/cli
 ```
 
-Docker Build
+#### Docker compose integration
+
+We've included a [docker-compose.yml](./docker-compose.yml) configuration to simplify the build, test, and deployment of the image.
+
+##### Building the Image with Docker Compose
+
+To build the Docker image using Docker Compose, run the following command:
 
 ```bash
-docker build -t datacontract/cli .
-docker run --rm -v ${PWD}:/home/datacontract datacontract/cli
+docker compose build
 ```
 
+This command utilizes the `docker-compose.yml` to build the image, leveraging predefined settings such as the build context and Dockerfile location. This approach streamlines the image creation process, avoiding the need for manual build specifications each time.
+
+#### Testing the Image
+
+After building the image, you can test it directly with Docker Compose:
+
+```bash
+docker compose run --rm datacontract --version
+```
+
+This command runs the container momentarily to check the version of the `datacontract` CLI. The `--rm` flag ensures that the container is automatically removed after the command executes, keeping your environment clean.
+
+
+
 ## Release Steps
 
 1. Update the version in `pyproject.toml`
 2. Have a look at the `CHANGELOG.md`
 3. Create release commit manually
 4. Execute `./release`
 5. Wait until GitHub Release is created
```

#### html2text {}

```diff
@@ -1,56 +1,55 @@
-Metadata-Version: 2.1 Name: datacontract-cli Version: 0.9.8 Summary: Test data
+Metadata-Version: 2.1 Name: datacontract-cli Version: 0.9.9 Summary: Test data
 contracts Author-email: Jochen Christ
 innoq.com>, Stefan Negele
 innoq.com> Project-URL: Homepage, https://cli.datacontract.com Project-URL:
 Issues, https://github.com/datacontract/cli/issues Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Requires-Python: >=3.10
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
-typer[all]<0.13,>=0.9 Requires-Dist: pydantic<2.7.0,>=2.5.3 Requires-Dist:
-pyyaml~=6.0.1 Requires-Dist: requests~=2.31.0 Requires-Dist: fastapi==0.110.0
+typer[all]<0.13,>=0.9 Requires-Dist: pydantic<2.8.0,>=2.5.3 Requires-Dist:
+pyyaml~=6.0.1 Requires-Dist: requests~=2.31.0 Requires-Dist: fastapi==0.110.1
 Requires-Dist: fastparquet==2024.2.0 Requires-Dist: python-multipart==0.0.9
 Requires-Dist: rich~=13.7.0 Requires-Dist: simple-ddl-parser==1.0.4 Requires-
 Dist: soda-core-bigquery<3.4.0,>=3.3.1 Requires-Dist: soda-core-
 duckdb<3.4.0,>=3.3.1 Requires-Dist: soda-core-postgres<3.4.0,>=3.3.1 Requires-
 Dist: soda-core-snowflake<3.4.0,>=3.3.1 Requires-Dist: soda-core-spark
 [databricks]<3.4.0,>=3.3.1 Requires-Dist: soda-core-spark-df<3.4.0,>=3.3.1
 Requires-Dist: snowflake-connector-python[pandas]<3.8,>=3.6 Requires-Dist:
 duckdb==0.10.1 Requires-Dist: fastjsonschema~=2.19.1 Requires-Dist: python-
 dotenv~=1.0.0 Requires-Dist: s3fs==2024.3.1 Requires-Dist: rdflib==7.0.0
 Requires-Dist: avro==1.11.3 Requires-Dist: opentelemetry-exporter-otlp-proto-
 grpc~=1.16.0 Requires-Dist: opentelemetry-exporter-otlp-proto-http~=1.16.0
 Provides-Extra: dev Requires-Dist: httpx==0.27.0; extra == "dev" Requires-Dist:
 ruff; extra == "dev" Requires-Dist: pytest; extra == "dev" Requires-Dist:
-testcontainers<4.0; extra == "dev" Requires-Dist: testcontainers-minio; extra
-== "dev" Requires-Dist: testcontainers-postgres; extra == "dev" Requires-Dist:
-testcontainers-kafka; extra == "dev" # Data Contract CLI
+pytest-xdist; extra == "dev" Requires-Dist: testcontainers<4.0; extra == "dev"
+Requires-Dist: testcontainers-minio; extra == "dev" Requires-Dist:
+testcontainers-postgres; extra == "dev" Requires-Dist: testcontainers-kafka;
+extra == "dev" # Data Contract CLI
 _[_T_e_s_t_ _W_o_r_k_f_l_o_w_]_[_S_t_a_r_s_]_[_S_l_a_c_k_ _S_t_a_t_u_s_]
 The `datacontract` CLI is an open source command-line tool for working with
 [Data Contracts](https://datacontract.com/). It uses data contract YAML files
 to lint the data contract, connect to data sources and execute schema and
 quality tests, detect breaking changes, and export to different formats. The
 tool is written in Python. It can be used as a standalone CLI tool, in a CI/CD
 pipeline, or directly as a Python library. ![Main features of the Data Contract
-CLI](datacontractcli.png)
-                          _[_D_e_m_o_ _o_f_ _D_a_t_a_ _C_o_n_t_r_a_c_t_ _C_L_I_]
-## Getting started Let's look at this data contract: [https://datacontract.com/
-examples/orders-latest/datacontract.yaml](https://datacontract.com/examples/
-orders-latest/datacontract.yaml) We have a _servers_ section with endpoint
-details to the S3 bucket, _models_ for the structure of the data, and _quality_
-attributes that describe the expected freshness and number of rows. This data
-contract contains all information to connect to S3 and check that the actual
-data meets the defined schema and quality requirements. We can use this
-information to test if the actual data set in S3 is compliant to the data
-contract. Let's use [pip](https://pip.pypa.io/en/stable/getting-started/) to
-install the CLI (or use the [Docker image](#docker), if you prefer). ```bash $
-python3 -m pip install datacontract-cli ``` We run the tests: ```bash $
-datacontract test https://datacontract.com/examples/orders-latest/
-datacontract.yaml # returns: Testing https://datacontract.com/examples/orders-
-latest/datacontract.yaml
+CLI](datacontractcli.png) ## Getting started Let's look at this data contract:
+[https://datacontract.com/examples/orders-latest/datacontract.yaml](https://
+datacontract.com/examples/orders-latest/datacontract.yaml) We have a _servers_
+section with endpoint details to the S3 bucket, _models_ for the structure of
+the data, _servicelevels_ and _quality_ attributes that describe the expected
+freshness and number of rows. This data contract contains all information to
+connect to S3 and check that the actual data meets the defined schema and
+quality requirements. We can use this information to test if the actual data
+set in S3 is compliant to the data contract. Let's use [pip](https://
+pip.pypa.io/en/stable/getting-started/) to install the CLI (or use the [Docker
+image](#docker), if you prefer). ```bash $ python3 -m pip install datacontract-
+cli ``` We run the tests: ```bash $ datacontract test https://datacontract.com/
+examples/orders-latest/datacontract.yaml # returns: Testing https://
+datacontract.com/examples/orders-latest/datacontract.yaml
 â­âââââââââ¬ââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ¬ââââââââââââââââââââââââââââââââ¬ââââââââââ®
 â Result â Check â Field â Details â
 ââââââââââ¼ââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ¼ââââââââââââââââââââââââââââââââ¼ââââââââââ¤
 â passed â Check that JSON has valid schema â orders â â â passed
 â Check that JSON has valid schema â line_items â â â passed â
 Check that field order_id is present â orders â â â passed â Check
 that field order_timestamp is present â orders â â â passed â Check
@@ -74,111 +73,130 @@
 row_count >= 5000 â line_items â â â passed â Check that required
 field lines_item_id has no null values â line_items.lines_item_id â â â
 passed â Check that unique field lines_item_id has no duplicate values â
 line_items.lines_item_id â â
 â°âââââââââ´ââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ´ââââââââââââââââââââââââââââââââ´ââââââââââ¯
 ð¢ data contract is valid. Run 22 checks. Took 6.739514 seconds. ``` VoilÃ ,
 the CLI tested that the _datacontract.yaml_ itself is valid, all records comply
-with the schema, and all quality attributes are met. ## Usage ```bash # create
-a new data contract from example and write it to datacontract.yaml $
-datacontract init datacontract.yaml # lint the datacontract.yaml $ datacontract
-lint datacontract.yaml # execute schema and quality checks $ datacontract test
-datacontract.yaml # execute schema and quality checks on the examples within
-the contract $ datacontract test --examples datacontract.yaml # find
-differences between to data contracts (Coming Soon) $ datacontract diff
-datacontract-v1.yaml datacontract-v2.yaml # find differences between to data
-contracts categorized into error, warning, and info. $ datacontract changelog
-datacontract-v1.yaml datacontract-v2.yaml # fail pipeline on breaking changes.
-Uses changelog internally and showing only error and warning. $ datacontract
-breaking datacontract-v1.yaml datacontract-v2.yaml # export model as jsonschema
-(other formats: avro, dbt, dbt-sources, dbt-staging-sql, jsonschema, odcs, rdf,
-sql (coming soon), sodacl, terraform) $ datacontract export --format jsonschema
-datacontract.yaml # import sql $ datacontract import --format sql --source
-my_ddl.sql # import avro $ datacontract import --format avro --source
-avro_schema.avsc ``` ## Programmatic (Python) ```python from
-datacontract.data_contract import DataContract data_contract = DataContract
+with the schema, and all quality attributes are met. We can also use the
+datacontract.yaml to export in many [formats](#format), e.g., to SQL: ```bash $
+datacontract export --format sql https://datacontract.com/examples/orders-
+latest/datacontract.yaml # returns: -- Data Contract: urn:datacontract:
+checkout:orders-latest -- SQL Dialect: snowflake CREATE TABLE orders ( order_id
+TEXT not null primary key, order_timestamp TIMESTAMP_TZ not null, order_total
+NUMBER not null, customer_id TEXT, customer_email_address TEXT not null,
+processed_timestamp TIMESTAMP_TZ not null ); CREATE TABLE line_items
+( lines_item_id TEXT not null primary key, order_id TEXT, sku TEXT ); ``` Or
+generate this [HTML page](https://datacontract.com/examples/orders-latest/
+datacontract.html). ## Usage ```bash # create a new data contract from example
+and write it to datacontract.yaml $ datacontract init datacontract.yaml # lint
+the datacontract.yaml $ datacontract lint datacontract.yaml # execute schema
+and quality checks $ datacontract test datacontract.yaml # execute schema and
+quality checks on the examples within the contract $ datacontract test --
+examples datacontract.yaml # export data contract as html (other formats: avro,
+dbt, dbt-sources, dbt-staging-sql, jsonschema, odcs, rdf, sql, sodacl,
+terraform, ...) $ datacontract export --format html datacontract.yaml >
+datacontract.html # import avro (other formats: sql, ...) $ datacontract import
+--format avro --source avro_schema.avsc # find differences between to data
+contracts $ datacontract diff datacontract-v1.yaml datacontract-v2.yaml # find
+differences between to data contracts categorized into error, warning, and
+info. $ datacontract changelog datacontract-v1.yaml datacontract-v2.yaml # fail
+pipeline on breaking changes. Uses changelog internally and showing only error
+and warning. $ datacontract breaking datacontract-v1.yaml datacontract-v2.yaml
+``` ## Programmatic (Python) ```python from datacontract.data_contract import
+DataContract data_contract = DataContract
 (data_contract_file="datacontract.yaml") run = data_contract.test() if not
 run.has_passed(): print("Data quality validation failed.") # Abort pipeline,
-alert, or take corrective actions... ``` ## Integrations | Integration | Option
-| Description | |-------------------|------------------------------|-----------
--------------------------------------------------------------------------------
--------------| | Data Mesh Manager | `--publish` | Push full results to the
-[Data Mesh Manager API](https://api.datamesh-manager.com/swagger/index.html) |
-| OpenTelemetry | `--publish-to-opentelemetry` | Push result as gauge metrics
-(logs are planned) | ### Integration with Data Mesh Manager If you use [Data
-Mesh Manager](https://datamesh-manager.com/), you can use the data contract URL
-and append the `--publish` option to send and display the test results. Set an
-environment variable for your API key. ```bash # Fetch current data contract,
-execute tests on production, and publish result to data mesh manager $ EXPORT
-DATAMESH_MANAGER_API_KEY=xxx $ datacontract test https://demo.datamesh-
-manager.com/demo279750347121/datacontracts/4df9d6ee-e55d-4088-9598-
-b635b2fdcbbc/datacontract.yaml --server production --publish ``` ###
-Integration with OpenTelemetry If you use OpenTelemetry, you can use the data
-contract URL and append the `--publish-to-opentelemetry` option to send the
-test results to your OLTP-compatible instance, e.g., Prometheus. The metric
-name is "datacontract.cli.test.result" and it uses the following encoding for
-the result: | datacontract.cli.test.result | Description | |-------|-----------
-----------------------------| | 0 | test run passed, no warnings | | 1 | test
-run has warnings | | 2 | test run failed | | 3 | test run not possible due to
-an error | | 4 | test status unknown | ```bash # Fetch current data contract,
-execute tests on production, and publish result to open telemetry $ EXPORT
-OTEL_SERVICE_NAME=datacontract-cli $ EXPORT OTEL_EXPORTER_OTLP_ENDPOINT=https:/
-/YOUR_ID.apm.westeurope.azure.elastic-cloud.com:443 $ EXPORT
-OTEL_EXPORTER_OTLP_HEADERS=Authorization=Bearer%20secret # Optional, when using
-SaaS Products $ EXPORT OTEL_EXPORTER_OTLP_PROTOCOL=http/protobuf # Optional,
-default is http/protobuf - use value grpc to use the gRPC protocol instead #
-Send to OpenTelemetry $ datacontract test https://demo.datamesh-manager.com/
-demo279750347121/datacontracts/4df9d6ee-e55d-4088-9598-b635b2fdcbbc/
-datacontract.yaml --server production --publish-to-opentelemetry ``` Current
-limitations: - currently, only ConsoleExporter and OTLP Exporter - Metrics
-only, no logs yet (but loosely planned) ## Installation Choose the most
+alert, or take corrective actions... ``` ## Installation Choose the most
 appropriate installation method for your needs: ### pip Python 3.11
 recommended. Python 3.12 available as pre-release release candidate for 0.9.3
 ```bash python3 -m pip install datacontract-cli ``` ### pipx pipx installs into
 an isolated environment. ```bash pipx install datacontract-cli ``` ### Docker
 ```bash docker pull datacontract/cli docker run --rm -v ${PWD}:/home/
 datacontract datacontract/cli ``` Or via an alias that automatically uses the
 latest version: ```bash alias datacontract='docker run --rm -v "${PWD}:/home/
-datacontract" datacontract/cli:latest' ``` ## Documentation ### Tests Data
-Contract CLI can connect to data sources and run schema and quality tests to
-verify that the data contract is valid. ```bash $ datacontract test --server
-production datacontract.yaml ``` To connect to the databases the `server` block
-in the datacontract.yaml is used to set up the connection. In addition,
-credentials, such as username and passwords, may be defined with environment
-variables. The application uses different engines, based on the server `type`.
-| Type | Format | Description | Status | Engines | |--------------|------------
-|---------------------------------------------------------------------------|--
------------|-------------------------------------| | `s3` | `parquet` | Works
-for any S3-compliant endpoint., e.g., AWS S3, GCS, MinIO, Ceph, ... | â |
-soda-core-duckdb | | `s3` | `json` | Support for `new_line` delimited JSON
-files and one JSON record per file. | â | fastjsonschema
-soda-core-duckdb | | `s3` | `csv` | | â | soda-core-duckdb | | `s3` | `delta`
-| | Coming soon | TBD | | `postgres` | n/a | | â | soda-core-postgres | |
-`snowflake` | n/a | | â | soda-core-snowflake | | `bigquery` | n/a | | â |
-soda-core-bigquery | | `redshift` | n/a | | Coming soon | TBD | | `databricks`
-| n/a | Support for Databricks SQL with Unity catalog and Hive metastore. | â
-| soda-core-spark | | `databricks` | n/a | Support for Spark for programmatic
-use in Notebooks. | â | soda-core-spark-df | | `kafka` | `json` |
-Experimental. | â | pyspark
-soda-core-spark-df | | `kafka` | `avro` | | Coming soon | TBD | | `kafka` |
-`protobuf` | | Coming soon | TBD | | `local` | `parquet` | | â | soda-core-
-duckdb | | `local` | `json` | Support for `new_line` delimited JSON files and
-one JSON record per file. | â | fastjsonschema
-soda-core-duckdb | | `local` | `csv` | | â | soda-core-duckdb | Feel free to
-create an issue, if you need support for an additional type. ### S3 Data
-Contract CLI can test data that is stored in S3 buckets or any S3-compliant
-endpoints in various formats. #### Example datacontract.yaml ```yaml servers:
-production: type: s3 endpointUrl: https://minio.example.com # not needed with
-AWS S3 location: s3://bucket-name/path/*/*.json format: json delimiter:
-new_line # new_line, array, or none ``` #### Environment Variables |
-Environment Variable | Example | Description | |-------------------------------
-----|-------------------------------|-----------------------| |
-`DATACONTRACT_S3_REGION` | `eu-central-1` | Region of S3 bucket | |
-`DATACONTRACT_S3_ACCESS_KEY_ID` | `AKIAXV5Q5QABCDEFGH` | AWS Access Key ID | |
-`DATACONTRACT_S3_SECRET_ACCESS_KEY` | `93S7LRrJcqLaaaa/XXXXXXXXXXXXX` | AWS
+datacontract" datacontract/cli:latest' ``` ## Documentation Commands - [init]
+(#init) - [lint](#lint) - [test](#test) - [export](#export) - [import](#import)
+- [breaking](#breaking) - [changelog](#changelog) - [diff](#diff) ### init ```
+Usage: datacontract init [OPTIONS] [LOCATION] Download a datacontract.yaml
+template and write it to file. â­â Arguments
+âââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ®
+â location [LOCATION] The location (url or path) of the data contract yaml to
+create. â â [default: datacontract.yaml] â
+â°âââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ¯
+â­â Options
+âââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ®
+â --template TEXT URL of a template or data contract â â [default: â
+â https://datacontract.com/datacontract.init.yaml] â â --overwrite --no-
+overwrite Replace the existing datacontract.yaml â â [default: no-
+overwrite] â â --help Show this message and exit. â
+â°âââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ¯
+``` ### lint ``` Usage: datacontract lint [OPTIONS] [LOCATION] Validate that
+the datacontract.yaml is correctly formatted. â­â Arguments
+ââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ®
+â location [LOCATION] The location (url or path) of the data contract yaml.
+[default: datacontract.yaml] â
+â°ââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ¯
+â­â Options
+ââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ®
+â --schema TEXT The location (url or path) of the Data Contract Specification
+JSON Schema â â [default: https://datacontract.com/
+datacontract.schema.json] â â --help Show this message and exit. â
+â°ââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ¯
+``` ### test ``` Usage: datacontract test [OPTIONS] [LOCATION] Run schema and
+quality tests on configured servers. â­â Arguments
+ââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ®
+â location [LOCATION] The location (url or path) of the data contract yaml.
+[default: datacontract.yaml] â
+â°ââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ¯
+â­â Options
+ââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ®
+â --schema TEXT The location (url or path) of the Data Contract â â
+Specification JSON Schema â â [default: â â https://datacontract.com/
+datacontract.schema.json] â â --server TEXT The server configuration to run
+the schema and quality â â tests. Use the key of the server object in the
+data â â contract yaml file to refer to a server, e.g., â â
+`production`, or `all` for all servers (default). â â [default: all] â
+â --examples --no-examples Run the schema and quality tests on the example
+data â â within the data contract. â â [default: no-examples] â â -
+-publish TEXT The url to publish the results after the test â â [default:
+None] â â --publish-to-opentelemetry --no-publish-to-opentelemetry Publish
+the results to opentelemetry. Use environment â â variables to configure
+the OTLP endpoint, headers, etc. â â [default: no-publish-to-opentelemetry]
+â â --logs --no-logs Print logs [default: no-logs] â â --help Show this
+message and exit. â
+â°ââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ¯
+``` Data Contract CLI can connect to data sources and run schema and quality
+tests to verify that the data contract is valid. ```bash $ datacontract test --
+server production datacontract.yaml ``` To connect to the databases the
+`server` block in the datacontract.yaml is used to set up the connection. In
+addition, credentials, such as username and passwords, may be defined with
+environment variables. The application uses different engines, based on the
+server `type`. Internally, it connects with DuckDB, Spark, or a native
+connection and executes the most tests with soda-core and fastjsonschema.
+Credentials are read from the environment variables. Supported server types: |
+Type | Format | Status | |--------------|------------|-------------------------
+-------------------------------------------| | `s3` | `parquet` | â | | `s3`
+| `json` | â | | `s3` | `csv` | â | | `s3` | `delta` | Coming soon ([#24]
+(https://github.com/datacontract/cli/issues/24)) | | `s3` | `iceberg` | Coming
+soon | | `postgres` | n/a | â | | `snowflake` | n/a | â | | `bigquery` | n/
+a | â | | `redshift` | n/a | Coming soon | | `databricks` | n/a | â | |
+`kafka` | `json` | â | | `kafka` | `avro` | Coming soon | | `kafka` |
+`protobuf` | Coming soon | | `local` | `parquet` | â | | `local` | `json` |
+â | | `local` | `csv` | â | Feel free to create an issue, if you need
+support for an additional type. ### S3 Data Contract CLI can test data that is
+stored in S3 buckets or any S3-compliant endpoints in various formats. ####
+Example datacontract.yaml ```yaml servers: production: type: s3 endpointUrl:
+https://minio.example.com # not needed with AWS S3 location: s3://bucket-name/
+path/*/*.json format: json delimiter: new_line # new_line, array, or none ```
+#### Environment Variables | Environment Variable | Example | Description | |--
+---------------------------------|-------------------------------|-------------
+----------| | `DATACONTRACT_S3_REGION` | `eu-central-1` | Region of S3 bucket |
+| `DATACONTRACT_S3_ACCESS_KEY_ID` | `AKIAXV5Q5QABCDEFGH` | AWS Access Key ID |
+| `DATACONTRACT_S3_SECRET_ACCESS_KEY` | `93S7LRrJcqLaaaa/XXXXXXXXXXXXX` | AWS
 Secret Access Key | ### Postgres Data Contract CLI can test data in Postgres or
 Postgres-compliant databases (e.g., RisingWave). #### Example datacontract.yaml
 ```yaml servers: postgres: type: postgres host: localhost port: 5432 database:
 postgres schema: public models: my_table_1: # corresponds to a table type:
 table fields: my_column_1: # corresponds to a column type: varchar ``` ####
 Environment Variables | Environment Variable | Example | Description | |-------
 ---------------------------|--------------------|-------------| |
@@ -231,131 +249,242 @@
 Kafka Kafka support is currently considered experimental. #### Example
 datacontract.yaml ```yaml servers: production: type: kafka host: abc-12345.eu-
 central-1.aws.confluent.cloud:9092 topic: my-topic-name format: json ``` ####
 Environment Variables | Environment Variable | Example | Description | |-------
 -----------------------------|---------|-----------------------------| |
 `DATACONTRACT_KAFKA_SASL_USERNAME` | `xxx` | The SASL username (key). | |
 `DATACONTRACT_KAFKA_SASL_PASSWORD` | `xxx` | The SASL password (secret). | ###
-Exports ```bash # Example export to dbt model datacontract export --format dbt
-``` Available export options: | Type | Description | Status | |----------------
-------|---------------------------------------------------------|--------| |
-`jsonschema` | Export to JSON Schema | â | | `odcs` | Export to Open Data
-Contract Standard (ODCS) | â | | `sodacl` | Export to SodaCL quality checks
-in YAML format | â | | `dbt` | Export to dbt models in YAML format | â | |
-`dbt-sources` | Export to dbt sources in YAML format | â | | `dbt-staging-
-sql` | Export to dbt staging SQL models | â | | `rdf` | Export data contract
-to RDF representation in N3 format | â | | `avro` | Export to AVRO models |
-â | | `protobuf` | Export to Protobuf | â | | `terraform` | Export to
-terraform resources | â | | `sql` | Export to SQL DDL | â | | `sql-query` |
-Export to SQL Query | â | | `great-expectations` | Export to Great
-Expectations Suites in JSON Format | â | | `bigquery` | Export to BigQuery
-Schemas | TBD | | `pydantic` | Export to pydantic models | TBD | | `html` |
-Export to HTML page | TBD | | Missing something? | Please create an issue on
-GitHub | TBD | #### Great Expectations The export function transforms a
-specified data contract into a comprehensive Great Expectations JSON suite. If
-the contract includes multiple models, you need to specify the names of the
-model you wish to export. ```shell datacontract export datacontract.yaml --
-format great-expectations --model orders ``` The export creates a list of
-expectations by utilizing: - The data from the Model definition with a fixed
-mapping - The expectations provided in the quality field for each model (find
-here the expectations gallery https://greatexpectations.io/expectations/) ####
-RDF The export function converts a given data contract into a RDF
-representation. You have the option to add a base_url which will be used as the
-default prefix to resolve relative IRIs inside the document. ```shell
-datacontract export --format rdf --rdf-base https://www.example.com/
-datacontract.yaml ``` The data contract is mapped onto the following concepts
-of a yet to be defined Data Contract Ontology named https://datacontract.com/
-DataContractSpecification/ : - DataContract - Server - Model Having the data
-contract inside an RDF Graph gives us access the following use cases: -
-Interoperability with other data contract specification formats - Store data
-contracts inside a knowledge graph - Enhance a semantic search to find and
-retrieve data contracts - Linking model elements to already established
-ontologies and knowledge - Using full power of OWL to reason about the graph
-structure of data contracts - Apply graph algorithms on multiple data contracts
-(Find similar data contracts, find "gatekeeper" data products, find the true
-domain owner of a field attribute) ### Imports ```bash # Example import from
-SQL DDL datacontract import --format sql --source my_ddl.sql ``` Available
-import options: | Type | Description | Status | |--------------------|---------
----------------------------------------|---------| | `sql` | Import from SQL
-DDL | â | | `avro` | Import from AVRO schemas | â | | `protobuf` | Import
-from Protobuf schemas | TBD | | `jsonschema` | Import from JSON Schemas | TBD |
-| `bigquery` | Import from BigQuery Schemas | TBD | | `dbt` | Import from dbt
-models | TBD | | `odcs` | Import from Open Data Contract Standard (ODCS) | TBD
-| | Missing something? | Please create an issue on GitHub | TBD | ## Best
-Practices We share best practices in using the Data Contract CLI. ### Data-
-first Approach Create a data contract based on the actual data. This is the
-fastest way to get started and to get feedback from the data consumers. 1. Use
-an existing physical schema (e.g., SQL DDL) as a starting point to define your
-logical data model in the contract. Double check right after the import whether
-the actual data meets the imported logical data model. Just to be sure. ```bash
-$ datacontract import --format sql ddl.sql $ datacontract test ``` 2. Add
-examples to the `datacontract.yaml`. If you can, use actual data and anonymize.
-Make sure that the examples match the imported logical data model. ```bash $
-datacontract test --examples ``` 3. Add quality checks and additional type
-constraints one by one to the contract and make sure the examples and the
-actual data still adheres to the contract. Check against examples for a very
-fast feedback loop. ```bash $ datacontract test --examples $ datacontract test
-``` 4. Make sure that all the best practices for a `datacontract.yaml` are met
-using the linter. You probably forgot to document some fields and add the terms
-and conditions. ```bash $ datacontract lint ``` 5. Set up a CI pipeline that
-executes daily and reports the results to the [Data Mesh Manager](https://
-datamesh-manager.com). Or to some place else. You can even publish to any
-opentelemetry compatible system. ```bash $ datacontract test --publish https://
-api.datamesh-manager.com/api/runs ``` ### Contract-First Create a data contract
-based on the requirements from use cases. 1. Start with a `datacontract.yaml`
-template. ```bash $ datacontract init ``` 2. Add examples to the
-`datacontract.yaml`. Do not start with the data model, although you are
-probably tempted to do that. Examples are the fastest way to get feedback from
-everybody and not loose someone in the discussion. 3. Create the model based on
-the examples. Test the model against the examples to double-check whether the
-model matches the examples. ```bash $ datacontract test --examples ``` 4. Add
-quality checks and additional type constraints one by one to the contract and
-make sure the examples and the actual data still adheres to the contract. Check
-against examples for a very fast feedback loop. ```bash $ datacontract test --
-examples ``` 5. Fill in the terms, descriptions, etc. Make sure you follow all
-best practices for a `datacontract.yaml` using the linter. ```bash $
-datacontract lint ``` 6. Set up a CI pipeline that lints and tests the examples
-so you make sure that any changes later do not decrease the quality of the
-contract. ```bash $ datacontract lint $ datacontract test --examples ``` 7. Use
-the export function to start building the providing data product as well as the
-integration into the consuming data products. ```bash # data provider $
-datacontract export --format dbt # data consumer $ datacontract export --format
-dbt-sources $ datacontract export --format dbt-staging-sql ``` ### Schema
-Evolution #### Non-breaking Changes Examples: adding models or fields - Add the
-models or fields in the datacontract.yaml - Increment the minor version of the
-datacontract.yaml on any change. Simply edit the datacontract.yaml for this. -
-You need a policy that these changes are non-breaking. That means that one
-cannot use the star expression in SQL to query a table under contract. Make the
-consequences known. - Fail the build in the Pull Request if a datacontract.yaml
-accidentially adds a breaking change even despite only a minor version change
-```bash $ datacontract breaking datacontract-from-pr.yaml datacontract-from-
-main.yaml ``` - Create a changelog of this minor change. ```bash $ datacontract
-changelog datacontract-from-pr.yaml datacontract-from-main.yaml ``` ####
-Breaking Changes Examples: Removing or renaming models and fields. - Remove or
-rename models and fields in the datacontract.yaml, and any other change that
-might be part of this new major version of this data contract. - Increment the
-major version of the datacontract.yaml for this and create a new file for the
-major version. The reason being, that one needs to offer an upgrade path for
-the data consumers from the old to the new major version. - As data consumers
-need to migrate, try to reduce the frequency of major versions by making
-multiple breaking changes together if possible. - Be aware of the notice period
-in the data contract as this is the minimum amount of time you have to offer
-both the old and the new version for a migration path. - Do not fear making
-breaking changes with data contracts. It's okay to do them in this controlled
-way. Really! - Create a changelog of this major change. ```bash $ datacontract
-changelog datacontract-from-pr.yaml datacontract-from-main.yaml ``` ##
-Development Setup Python base interpreter should be 3.11.x (unless working on
-3.12 release candidate). ```bash # create venv python3 -m venv venv source
-venv/bin/activate # Install Requirements pip install --upgrade pip setuptools
-wheel pip install -e '.[dev]' ruff check --fix ruff format --check pytest ```
-Release ```bash git tag v0.9.0 git push origin v0.9.0 python3 -m pip install --
-upgrade build twine rm -r dist/ python3 -m build # for now only test.pypi.org
-python3 -m twine upload --repository testpypi dist/* ``` Docker Build ```bash
-docker build -t datacontract/cli . docker run --rm -v ${PWD}:/home/datacontract
-datacontract/cli ``` ## Release Steps 1. Update the version in `pyproject.toml`
-2. Have a look at the `CHANGELOG.md` 3. Create release commit manually 4.
-Execute `./release` 5. Wait until GitHub Release is created 6. Add the release
-notes to the GitHub Release ## Contribution We are happy to receive your
-contributions. Propose your change in an issue or directly create a pull
-request with your improvements. ## License [MIT License](LICENSE) ## Credits
-Created by [Stefan Negele](https://www.linkedin.com/in/stefan-negele-573153112/
-) and [Jochen Christ](https://www.linkedin.com/in/jochenchrist/).
+export ``` Usage: datacontract export [OPTIONS] [LOCATION] Convert data
+contract to a specific format. console.prints to stdout. â­â Arguments
+ââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ®
+â location [LOCATION] The location (url or path) of the data contract yaml.
+[default: datacontract.yaml] â
+â°ââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ¯
+â­â Options
+ââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ®
+â * --format [html|jsonschema|pydantic-model|sodacl|dbt|dbt-sources|dbt-
+staging-sql|odcs|rd The export format. [default: None] [required] â â
+f|avro|protobuf|great-expectations|terraform|avro-idl|sql|sql-query] â â --
+server TEXT The server name to export. [default: None] â â --model TEXT Use
+the key of the model in the data contract yaml file to refer to a â â
+model, e.g., `orders`, or `all` for all models (default). â â [default:
+all] â â --help Show this message and exit. â
+â°ââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ¯
+â­â RDF Options
+ââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ®
+â --rdf-base TEXT [rdf] The base URI used to generate the RDF graph.
+[default: None] â
+â°ââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ¯
+â­â SQL Options
+ââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ®
+â --sql-server-type TEXT [sql] The server type to determine the sql dialect.
+By default, it uses 'auto' to automatically detect the sql dialect via the
+specified â â servers in the data contract. â â [default: auto] â
+â°ââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ¯
+``` ```bash # Example export data contract as HTML datacontract export --format
+html > datacontract.html ``` Available export options: | Type | Description |
+Status | |----------------------|----------------------------------------------
+-----------|--------| | `html` | Export to HTML | â | | `jsonschema` | Export
+to JSON Schema | â | | `odcs` | Export to Open Data Contract Standard (ODCS)
+| â | | `sodacl` | Export to SodaCL quality checks in YAML format | â | |
+`dbt` | Export to dbt models in YAML format | â | | `dbt-sources` | Export to
+dbt sources in YAML format | â | | `dbt-staging-sql` | Export to dbt staging
+SQL models | â | | `rdf` | Export data contract to RDF representation in N3
+format | â | | `avro` | Export to AVRO models | â | | `protobuf` | Export
+to Protobuf | â | | `terraform` | Export to terraform resources | â | |
+`sql` | Export to SQL DDL | â | | `sql-query` | Export to SQL Query | â | |
+`great-expectations` | Export to Great Expectations Suites in JSON Format | â
+| | `bigquery` | Export to BigQuery Schemas | TBD | | `pydantic` | Export to
+pydantic models | TBD | | Missing something? | Please create an issue on GitHub
+| TBD | #### Great Expectations The export function transforms a specified data
+contract into a comprehensive Great Expectations JSON suite. If the contract
+includes multiple models, you need to specify the names of the model you wish
+to export. ```shell datacontract export datacontract.yaml --format great-
+expectations --model orders ``` The export creates a list of expectations by
+utilizing: - The data from the Model definition with a fixed mapping - The
+expectations provided in the quality field for each model (find here the
+expectations gallery https://greatexpectations.io/expectations/) #### RDF The
+export function converts a given data contract into a RDF representation. You
+have the option to add a base_url which will be used as the default prefix to
+resolve relative IRIs inside the document. ```shell datacontract export --
+format rdf --rdf-base https://www.example.com/ datacontract.yaml ``` The data
+contract is mapped onto the following concepts of a yet to be defined Data
+Contract Ontology named https://datacontract.com/DataContractSpecification/ : -
+DataContract - Server - Model Having the data contract inside an RDF Graph
+gives us access the following use cases: - Interoperability with other data
+contract specification formats - Store data contracts inside a knowledge graph
+- Enhance a semantic search to find and retrieve data contracts - Linking model
+elements to already established ontologies and knowledge - Using full power of
+OWL to reason about the graph structure of data contracts - Apply graph
+algorithms on multiple data contracts (Find similar data contracts, find
+"gatekeeper" data products, find the true domain owner of a field attribute)
+### import ``` Usage: datacontract import [OPTIONS] Create a data contract from
+the given source file. Prints to stdout. â­â Options
+ââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ®
+â * --format [sql|avro] The format of the source file. [default: None]
+[required] â â * --source TEXT The path to the file that should be
+imported. [default: None] [required] â â --help Show this message and exit.
+â
+â°ââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ¯
+``` Example: ```bash # Example import from SQL DDL datacontract import --format
+sql --source my_ddl.sql ``` Available import options: | Type | Description |
+Status | |--------------------|------------------------------------------------
+|---------| | `sql` | Import from SQL DDL | â | | `avro` | Import from AVRO
+schemas | â | | `protobuf` | Import from Protobuf schemas | TBD | |
+`jsonschema` | Import from JSON Schemas | TBD | | `bigquery` | Import from
+BigQuery Schemas | TBD | | `dbt` | Import from dbt models | TBD | | `odcs` |
+Import from Open Data Contract Standard (ODCS) | TBD | | Missing something? |
+Please create an issue on GitHub | TBD | ### breaking ``` Usage: datacontract
+breaking [OPTIONS] LOCATION_OLD LOCATION_NEW Identifies breaking changes
+between data contracts. Prints to stdout. â­â Arguments
+ââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ®
+â * location_old TEXT The location (url or path) of the old data contract
+yaml. [default: None] [required] â â * location_new TEXT The location (url
+or path) of the new data contract yaml. [default: None] [required] â
+â°ââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ¯
+â­â Options
+ââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ®
+â --help Show this message and exit. â
+â°ââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ¯
+``` ### changelog ``` Usage: datacontract changelog [OPTIONS] LOCATION_OLD
+LOCATION_NEW Generate a changelog between data contracts. Prints to stdout.
+â­â Arguments
+ââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ®
+â * location_old TEXT The location (url or path) of the old data contract
+yaml. [default: None] [required] â â * location_new TEXT The location (url
+or path) of the new data contract yaml. [default: None] [required] â
+â°ââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ¯
+â­â Options
+ââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ®
+â --help Show this message and exit. â
+â°ââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ¯
+``` ### diff ``` Usage: datacontract diff [OPTIONS] LOCATION_OLD LOCATION_NEW
+PLACEHOLDER. Currently works as 'changelog' does. â­â Arguments
+ââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ®
+â * location_old TEXT The location (url or path) of the old data contract
+yaml. [default: None] [required] â â * location_new TEXT The location (url
+or path) of the new data contract yaml. [default: None] [required] â
+â°ââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ¯
+â­â Options
+ââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ®
+â --help Show this message and exit. â
+â°ââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ¯
+``` ## Integrations | Integration | Option | Description | |-------------------
+|------------------------------|-----------------------------------------------
+--------------------------------------------------------| | Data Mesh Manager |
+`--publish` | Push full results to the [Data Mesh Manager API](https://
+api.datamesh-manager.com/swagger/index.html) | | OpenTelemetry | `--publish-to-
+opentelemetry` | Push result as gauge metrics | ### Integration with Data Mesh
+Manager If you use [Data Mesh Manager](https://datamesh-manager.com/), you can
+use the data contract URL and append the `--publish` option to send and display
+the test results. Set an environment variable for your API key. ```bash # Fetch
+current data contract, execute tests on production, and publish result to data
+mesh manager $ EXPORT DATAMESH_MANAGER_API_KEY=xxx $ datacontract test https://
+demo.datamesh-manager.com/demo279750347121/datacontracts/4df9d6ee-e55d-4088-
+9598-b635b2fdcbbc/datacontract.yaml --server production --publish ``` ###
+Integration with OpenTelemetry If you use OpenTelemetry, you can use the data
+contract URL and append the `--publish-to-opentelemetry` option to send the
+test results to your OLTP-compatible instance, e.g., Prometheus. The metric
+name is "datacontract.cli.test.result" and it uses the following encoding for
+the result: | datacontract.cli.test.result | Description | |-------|-----------
+----------------------------| | 0 | test run passed, no warnings | | 1 | test
+run has warnings | | 2 | test run failed | | 3 | test run not possible due to
+an error | | 4 | test status unknown | ```bash # Fetch current data contract,
+execute tests on production, and publish result to open telemetry $ EXPORT
+OTEL_SERVICE_NAME=datacontract-cli $ EXPORT OTEL_EXPORTER_OTLP_ENDPOINT=https:/
+/YOUR_ID.apm.westeurope.azure.elastic-cloud.com:443 $ EXPORT
+OTEL_EXPORTER_OTLP_HEADERS=Authorization=Bearer%20secret # Optional, when using
+SaaS Products $ EXPORT OTEL_EXPORTER_OTLP_PROTOCOL=http/protobuf # Optional,
+default is http/protobuf - use value grpc to use the gRPC protocol instead #
+Send to OpenTelemetry $ datacontract test https://demo.datamesh-manager.com/
+demo279750347121/datacontracts/4df9d6ee-e55d-4088-9598-b635b2fdcbbc/
+datacontract.yaml --server production --publish-to-opentelemetry ``` Current
+limitations: - currently, only ConsoleExporter and OTLP Exporter - Metrics
+only, no logs yet (but loosely planned) ## Best Practices We share best
+practices in using the Data Contract CLI. ### Data-first Approach Create a data
+contract based on the actual data. This is the fastest way to get started and
+to get feedback from the data consumers. 1. Use an existing physical schema
+(e.g., SQL DDL) as a starting point to define your logical data model in the
+contract. Double check right after the import whether the actual data meets the
+imported logical data model. Just to be sure. ```bash $ datacontract import --
+format sql ddl.sql $ datacontract test ``` 2. Add examples to the
+`datacontract.yaml`. If you can, use actual data and anonymize. Make sure that
+the examples match the imported logical data model. ```bash $ datacontract test
+--examples ``` 3. Add quality checks and additional type constraints one by one
+to the contract and make sure the examples and the actual data still adheres to
+the contract. Check against examples for a very fast feedback loop. ```bash $
+datacontract test --examples $ datacontract test ``` 4. Make sure that all the
+best practices for a `datacontract.yaml` are met using the linter. You probably
+forgot to document some fields and add the terms and conditions. ```bash $
+datacontract lint ``` 5. Set up a CI pipeline that executes daily and reports
+the results to the [Data Mesh Manager](https://datamesh-manager.com). Or to
+some place else. You can even publish to any opentelemetry compatible system.
+```bash $ datacontract test --publish https://api.datamesh-manager.com/api/runs
+``` ### Contract-First Create a data contract based on the requirements from
+use cases. 1. Start with a `datacontract.yaml` template. ```bash $ datacontract
+init ``` 2. Add examples to the `datacontract.yaml`. Do not start with the data
+model, although you are probably tempted to do that. Examples are the fastest
+way to get feedback from everybody and not loose someone in the discussion. 3.
+Create the model based on the examples. Test the model against the examples to
+double-check whether the model matches the examples. ```bash $ datacontract
+test --examples ``` 4. Add quality checks and additional type constraints one
+by one to the contract and make sure the examples and the actual data still
+adheres to the contract. Check against examples for a very fast feedback loop.
+```bash $ datacontract test --examples ``` 5. Fill in the terms, descriptions,
+etc. Make sure you follow all best practices for a `datacontract.yaml` using
+the linter. ```bash $ datacontract lint ``` 6. Set up a CI pipeline that lints
+and tests the examples so you make sure that any changes later do not decrease
+the quality of the contract. ```bash $ datacontract lint $ datacontract test --
+examples ``` 7. Use the export function to start building the providing data
+product as well as the integration into the consuming data products. ```bash #
+data provider $ datacontract export --format dbt # data consumer $ datacontract
+export --format dbt-sources $ datacontract export --format dbt-staging-sql ```
+### Schema Evolution #### Non-breaking Changes Examples: adding models or
+fields - Add the models or fields in the datacontract.yaml - Increment the
+minor version of the datacontract.yaml on any change. Simply edit the
+datacontract.yaml for this. - You need a policy that these changes are non-
+breaking. That means that one cannot use the star expression in SQL to query a
+table under contract. Make the consequences known. - Fail the build in the Pull
+Request if a datacontract.yaml accidentially adds a breaking change even
+despite only a minor version change ```bash $ datacontract breaking
+datacontract-from-pr.yaml datacontract-from-main.yaml ``` - Create a changelog
+of this minor change. ```bash $ datacontract changelog datacontract-from-
+pr.yaml datacontract-from-main.yaml ``` #### Breaking Changes Examples:
+Removing or renaming models and fields. - Remove or rename models and fields in
+the datacontract.yaml, and any other change that might be part of this new
+major version of this data contract. - Increment the major version of the
+datacontract.yaml for this and create a new file for the major version. The
+reason being, that one needs to offer an upgrade path for the data consumers
+from the old to the new major version. - As data consumers need to migrate, try
+to reduce the frequency of major versions by making multiple breaking changes
+together if possible. - Be aware of the notice period in the data contract as
+this is the minimum amount of time you have to offer both the old and the new
+version for a migration path. - Do not fear making breaking changes with data
+contracts. It's okay to do them in this controlled way. Really! - Create a
+changelog of this major change. ```bash $ datacontract changelog datacontract-
+from-pr.yaml datacontract-from-main.yaml ``` ## Development Setup Python base
+interpreter should be 3.11.x (unless working on 3.12 release candidate).
+```bash # create venv python3 -m venv venv source venv/bin/activate # Install
+Requirements pip install --upgrade pip setuptools wheel pip install -e '.[dev]'
+ruff check --fix ruff format --check pytest ``` ### Docker Build ```bash docker
+build -t datacontract/cli . docker run --rm -v ${PWD}:/home/datacontract
+datacontract/cli ``` #### Docker compose integration We've included a [docker-
+compose.yml](./docker-compose.yml) configuration to simplify the build, test,
+and deployment of the image. ##### Building the Image with Docker Compose To
+build the Docker image using Docker Compose, run the following command: ```bash
+docker compose build ``` This command utilizes the `docker-compose.yml` to
+build the image, leveraging predefined settings such as the build context and
+Dockerfile location. This approach streamlines the image creation process,
+avoiding the need for manual build specifications each time. #### Testing the
+Image After building the image, you can test it directly with Docker Compose:
+```bash docker compose run --rm datacontract --version ``` This command runs
+the container momentarily to check the version of the `datacontract` CLI. The
+`--rm` flag ensures that the container is automatically removed after the
+command executes, keeping your environment clean. ## Release Steps 1. Update
+the version in `pyproject.toml` 2. Have a look at the `CHANGELOG.md` 3. Create
+release commit manually 4. Execute `./release` 5. Wait until GitHub Release is
+created 6. Add the release notes to the GitHub Release ## Contribution We are
+happy to receive your contributions. Propose your change in an issue or
+directly create a pull request with your improvements. ## License [MIT License]
+(LICENSE) ## Credits Created by [Stefan Negele](https://www.linkedin.com/in/
+stefan-negele-573153112/) and [Jochen Christ](https://www.linkedin.com/in/
+jochenchrist/).
```

### Comparing `datacontract-cli-0.9.8/datacontract_cli.egg-info/SOURCES.txt` & `datacontract_cli-0.9.9/datacontract_cli.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -20,16 +20,18 @@
 datacontract/engines/soda/connections/databricks.py
 datacontract/engines/soda/connections/duckdb.py
 datacontract/engines/soda/connections/kafka.py
 datacontract/engines/soda/connections/postgres.py
 datacontract/engines/soda/connections/snowflake.py
 datacontract/export/avro_converter.py
 datacontract/export/avro_idl_converter.py
+datacontract/export/csv_type_converter.py
 datacontract/export/dbt_converter.py
 datacontract/export/great_expectations_converter.py
+datacontract/export/html_export.py
 datacontract/export/jsonschema_converter.py
 datacontract/export/odcs_converter.py
 datacontract/export/protobuf_converter.py
 datacontract/export/pydantic_converter.py
 datacontract/export/rdf_converter.py
 datacontract/export/sodacl_converter.py
 datacontract/export/sql_converter.py
@@ -47,15 +49,14 @@
 datacontract/lint/urls.py
 datacontract/lint/linters/__init__.py
 datacontract/lint/linters/description_linter.py
 datacontract/lint/linters/example_model_linter.py
 datacontract/lint/linters/field_pattern_linter.py
 datacontract/lint/linters/field_reference_linter.py
 datacontract/lint/linters/notice_period_linter.py
-datacontract/lint/linters/primary_field_linter.py
 datacontract/lint/linters/quality_schema_linter.py
 datacontract/lint/linters/valid_constraints_linter.py
 datacontract/model/breaking_change.py
 datacontract/model/data_contract_specification.py
 datacontract/model/exceptions.py
 datacontract/model/run.py
 datacontract_cli.egg-info/PKG-INFO
@@ -67,37 +68,21 @@
 tests/test_breaking.py
 tests/test_changelog.py
 tests/test_cli.py
 tests/test_description_linter.py
 tests/test_documentation_linter.py
 tests/test_download_datacontract_file.py
 tests/test_example_model_linter.py
-tests/test_examples_bigquery.py
-tests/test_examples_databricks.py
-tests/test_examples_examples_csv.py
-tests/test_examples_examples_inline.py
-tests/test_examples_examples_json.py
-tests/test_examples_examples_missing.py
-tests/test_examples_kafka.py
-tests/test_examples_kafka_remote.py
-tests/test_examples_local_json.py
-tests/test_examples_parquet.py
-tests/test_examples_postgres.py
-tests/test_examples_s3_csv.py
-tests/test_examples_s3_json.py
-tests/test_examples_s3_json_complex.py
-tests/test_examples_s3_json_multiple_models.py
-tests/test_examples_s3_json_remote.py
-tests/test_examples_snowflake.py
 tests/test_export_avro.py
 tests/test_export_avro_idl.py
 tests/test_export_dbt_models.py
 tests/test_export_dbt_sources.py
 tests/test_export_dbt_staging_sql.py
 tests/test_export_great_expectations.py
+tests/test_export_html.py
 tests/test_export_jsonschema.py
 tests/test_export_odcs.py
 tests/test_export_protobuf.py
 tests/test_export_pydantic.py
 tests/test_export_rdf.py
 tests/test_export_sodacl.py
 tests/test_export_sql.py
@@ -108,11 +93,28 @@
 tests/test_field_reference_linter.py
 tests/test_import_avro.py
 tests/test_import_sql.py
 tests/test_integration_datameshmanager.py
 tests/test_integration_opentelemetry.py
 tests/test_lint.py
 tests/test_notice_period_linter.py
-tests/test_primary_field_linter.py
 tests/test_quality_schema_linter.py
 tests/test_schema.py
+tests/test_test_bigquery.py
+tests/test_test_databricks.py
+tests/test_test_examples_csv.py
+tests/test_test_examples_formats_valid.py
+tests/test_test_examples_inline.py
+tests/test_test_examples_json.py
+tests/test_test_examples_missing.py
+tests/test_test_kafka.py
+tests/test_test_kafka_remote.py
+tests/test_test_local_json.py
+tests/test_test_parquet.py
+tests/test_test_postgres.py
+tests/test_test_s3_csv.py
+tests/test_test_s3_json.py
+tests/test_test_s3_json_complex.py
+tests/test_test_s3_json_multiple_models.py
+tests/test_test_s3_json_remote.py
+tests/test_test_snowflake.py
 tests/test_web.py
```

### Comparing `datacontract-cli-0.9.8/datacontract_cli.egg-info/requires.txt` & `datacontract_cli-0.9.9/datacontract_cli.egg-info/requires.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 typer[all]<0.13,>=0.9
-pydantic<2.7.0,>=2.5.3
+pydantic<2.8.0,>=2.5.3
 pyyaml~=6.0.1
 requests~=2.31.0
-fastapi==0.110.0
+fastapi==0.110.1
 fastparquet==2024.2.0
 python-multipart==0.0.9
 rich~=13.7.0
 simple-ddl-parser==1.0.4
 soda-core-bigquery<3.4.0,>=3.3.1
 soda-core-duckdb<3.4.0,>=3.3.1
 soda-core-postgres<3.4.0,>=3.3.1
@@ -23,11 +23,12 @@
 opentelemetry-exporter-otlp-proto-grpc~=1.16.0
 opentelemetry-exporter-otlp-proto-http~=1.16.0
 
 [dev]
 httpx==0.27.0
 ruff
 pytest
+pytest-xdist
 testcontainers<4.0
 testcontainers-minio
 testcontainers-postgres
 testcontainers-kafka
```

### Comparing `datacontract-cli-0.9.8/pyproject.toml` & `datacontract_cli-0.9.9/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 [project]
 name = "datacontract-cli"
-version = "0.9.8"
+version = "0.9.9"
 description = "Test data contracts"
 readme = "README.md"
 authors = [
   { name = "Jochen Christ", email = "jochen.christ@innoq.com" },
   { name = "Stefan Negele", email = "stefan.negele@innoq.com" },
 ]
 classifiers = [
   "Programming Language :: Python :: 3",
   "License :: OSI Approved :: MIT License",
   "Operating System :: OS Independent",
 ]
 requires-python = ">=3.10"
 dependencies = [
   "typer[all]>=0.9,<0.13",
-  "pydantic>=2.5.3,<2.7.0",
+  "pydantic>=2.5.3,<2.8.0",
   "pyyaml~=6.0.1",
   "requests~=2.31.0",
-  "fastapi==0.110.0",
+  "fastapi==0.110.1",
   "fastparquet==2024.2.0",
   "python-multipart==0.0.9",
   "rich~=13.7.0",
   "simple-ddl-parser==1.0.4",
   "soda-core-bigquery>=3.3.1,<3.4.0",
   "soda-core-duckdb>=3.3.1,<3.4.0",
   "soda-core-postgres>=3.3.1,<3.4.0",
@@ -41,14 +41,15 @@
 ]
 
 [project.optional-dependencies]
 dev = [
   "httpx==0.27.0",
   "ruff",
   "pytest",
+  "pytest-xdist",
   # testcontainers 4.x have issues with Kafka on arm
   # https://github.com/testcontainers/testcontainers-python/issues/450
   "testcontainers<4.0",
   "testcontainers-minio",
   "testcontainers-postgres",
   "testcontainers-kafka",
 ]
@@ -60,9 +61,12 @@
 [project.scripts]
 datacontract = "datacontract.cli:app"
 
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
+[tool.pytest.ini_options]
+addopts="-n 8"
+
 [tool.ruff]
 line-length = 120
```

### Comparing `datacontract-cli-0.9.8/tests/test_changelog.py` & `datacontract_cli-0.9.9/tests/test_changelog.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,939 +10,939 @@
 
 
 def test_no_changes():
     result = runner.invoke(
         app,
         [
             "changelog",
-            "./examples/breaking/datacontract-fields-v2.yaml",
-            "./examples/breaking/datacontract-fields-v2.yaml",
+            "./fixtures/breaking/datacontract-fields-v2.yaml",
+            "./fixtures/breaking/datacontract-fields-v2.yaml",
         ],
     )
     assert result.exit_code == 0
     assert "0 changes: 0 error, 0 warning, 0 info\n" in result.stdout
 
 
 def test_quality_added():
     result = runner.invoke(
         app,
         [
             "changelog",
-            "./examples/breaking/datacontract-quality-v1.yaml",
-            "./examples/breaking/datacontract-quality-v2.yaml",
+            "./fixtures/breaking/datacontract-quality-v1.yaml",
+            "./fixtures/breaking/datacontract-quality-v2.yaml",
         ],
     )
     output = result.stdout
     assert result.exit_code == 0
     assert "1 changes: 0 error, 0 warning, 1 info\n" in output
     assert (
-        r"""info    [quality_added] at ./examples/breaking/datacontract-quality-v2.yaml
+        r"""info    [quality_added] at ./fixtures/breaking/datacontract-quality-v2.yaml
         in quality
             added quality"""
         in output
     )
 
 
 def test_quality_removed():
     result = runner.invoke(
         app,
         [
             "changelog",
-            "./examples/breaking/datacontract-quality-v2.yaml",
-            "./examples/breaking/datacontract-quality-v1.yaml",
+            "./fixtures/breaking/datacontract-quality-v2.yaml",
+            "./fixtures/breaking/datacontract-quality-v1.yaml",
         ],
     )
     output = result.stdout
     assert result.exit_code == 0
     assert "1 changes: 0 error, 1 warning, 0 info\n" in output
     assert (
-        r"""warning [quality_removed] at ./examples/breaking/datacontract-quality-v1.yaml
+        r"""warning [quality_removed] at ./fixtures/breaking/datacontract-quality-v1.yaml
         in quality
             removed quality"""
         in output
     )
 
 
 def test_quality_updated():
     result = runner.invoke(
         app,
         [
             "changelog",
-            "./examples/breaking/datacontract-quality-v2.yaml",
-            "./examples/breaking/datacontract-quality-v3.yaml",
+            "./fixtures/breaking/datacontract-quality-v2.yaml",
+            "./fixtures/breaking/datacontract-quality-v3.yaml",
         ],
     )
     output = result.stdout
     assert result.exit_code == 0
     assert "2 changes: 0 error, 2 warning, 0 info\n" in output
     assert (
         r"""warning [quality_type_updated] at 
-./examples/breaking/datacontract-quality-v3.yaml
+./fixtures/breaking/datacontract-quality-v3.yaml
         in quality.type
             changed from `SodaCL` to `custom`"""
         in output
     )
     assert (
         r"""warning [quality_specification_updated] at 
-./examples/breaking/datacontract-quality-v3.yaml
+./fixtures/breaking/datacontract-quality-v3.yaml
         in quality.specification
             changed from `checks for orders:
   - freshness(column_1) < 1d` to `checks for orders:
   - freshness(column_1) < 2d`"""
         in output
     )
 
 
 def test_models_added():
     result = runner.invoke(
         app,
         [
             "changelog",
-            "./examples/breaking/datacontract-models-v1.yaml",
-            "./examples/breaking/datacontract-models-v2.yaml",
+            "./fixtures/breaking/datacontract-models-v1.yaml",
+            "./fixtures/breaking/datacontract-models-v2.yaml",
         ],
     )
     output = result.stdout
     assert result.exit_code == 0
     assert "2 changes: 0 error, 0 warning, 2 info\n" in output
     assert (
-        """info    [model_added] at ./examples/breaking/datacontract-models-v2.yaml
+        """info    [model_added] at ./fixtures/breaking/datacontract-models-v2.yaml
         in models.my_table_2
             added the model"""
         in output
     )
     assert (
         """info    [model_description_added] at 
-./examples/breaking/datacontract-models-v2.yaml
+./fixtures/breaking/datacontract-models-v2.yaml
         in models.my_table.description
             added with value: `My Model Description`"""
         in output
     )
 
 
 def test_models_removed():
     result = runner.invoke(
         app,
         [
             "changelog",
-            "./examples/breaking/datacontract-models-v2.yaml",
-            "./examples/breaking/datacontract-models-v1.yaml",
+            "./fixtures/breaking/datacontract-models-v2.yaml",
+            "./fixtures/breaking/datacontract-models-v1.yaml",
         ],
     )
     output = result.stdout
     assert result.exit_code == 0
     assert "2 changes: 1 error, 0 warning, 1 info\n" in output
     assert (
-        r"""error   [model_removed] at ./examples/breaking/datacontract-models-v1.yaml
+        r"""error   [model_removed] at ./fixtures/breaking/datacontract-models-v1.yaml
         in models.my_table_2
             removed the model"""
         in output
     )
     assert (
         """info    [model_description_removed] at 
-./examples/breaking/datacontract-models-v1.yaml
+./fixtures/breaking/datacontract-models-v1.yaml
         in models.my_table.description
             removed model property"""
         in output
     )
 
 
 def test_models_updated():
     result = runner.invoke(
         app,
         [
             "changelog",
-            "./examples/breaking/datacontract-models-v2.yaml",
-            "./examples/breaking/datacontract-models-v3.yaml",
+            "./fixtures/breaking/datacontract-models-v2.yaml",
+            "./fixtures/breaking/datacontract-models-v3.yaml",
         ],
     )
     output = result.stdout
     assert result.exit_code == 0
     assert "2 changes: 1 error, 0 warning, 1 info\n" in output
     assert (
-        r"""error   [model_type_updated] at ./examples/breaking/datacontract-models-v3.yaml
+        r"""error   [model_type_updated] at ./fixtures/breaking/datacontract-models-v3.yaml
         in models.my_table.type
             changed from `table` to `object`"""
         in output
     )
     assert (
         """info    [model_description_updated] at 
-./examples/breaking/datacontract-models-v3.yaml
+./fixtures/breaking/datacontract-models-v3.yaml
         in models.my_table.description
             changed from `My Model Description` to `My Updated Model 
 Description`"""
         in output
     )
 
 
 def test_fields_added():
     result = runner.invoke(
         app,
         [
             "changelog",
-            "./examples/breaking/datacontract-fields-v1.yaml",
-            "./examples/breaking/datacontract-fields-v2.yaml",
+            "./fixtures/breaking/datacontract-fields-v1.yaml",
+            "./fixtures/breaking/datacontract-fields-v2.yaml",
         ],
     )
     assert result.exit_code == 0
     output = result.stdout
     assert "18 changes: 0 error, 14 warning, 4 info\n" in output
     assert (
-        """info    [field_added] at ./examples/breaking/datacontract-fields-v2.yaml
+        """info    [field_added] at ./fixtures/breaking/datacontract-fields-v2.yaml
         in models.my_table.fields.new_field
             added the field"""
         in output
     )
     assert (
         """warning [field_references_added] at 
-./examples/breaking/datacontract-fields-v2.yaml
+./fixtures/breaking/datacontract-fields-v2.yaml
         in models.my_table.fields.field_references.references
             added with value: `my_table.field_type`"""
         in output
     )
     assert (
-        r"""warning [field_type_added] at ./examples/breaking/datacontract-fields-v2.yaml
+        r"""warning [field_type_added] at ./fixtures/breaking/datacontract-fields-v2.yaml
         in models.my_table.fields.field_type.type
             added with value: `string`"""
         in output
     )
     assert (
-        r"""warning [field_format_added] at ./examples/breaking/datacontract-fields-v2.yaml
+        r"""warning [field_format_added] at ./fixtures/breaking/datacontract-fields-v2.yaml
         in models.my_table.fields.field_format.format
             added with value: `email`"""
         in output
     )
     assert (
         """info    [field_description_added] at 
-./examples/breaking/datacontract-fields-v2.yaml
+./fixtures/breaking/datacontract-fields-v2.yaml
         in models.my_table.fields.field_description.description
             added with value: `My Description`"""
         in output
     )
     assert (
-        r"""warning [field_pii_added] at ./examples/breaking/datacontract-fields-v2.yaml
+        r"""warning [field_pii_added] at ./fixtures/breaking/datacontract-fields-v2.yaml
         in models.my_table.fields.field_pii.pii
             added with value: `true`"""
         in output
     )
     assert (
         r"""warning [field_classification_added] at 
-./examples/breaking/datacontract-fields-v2.yaml
+./fixtures/breaking/datacontract-fields-v2.yaml
         in models.my_table.fields.field_classification.classification
             added with value: `sensitive`"""
         in output
     )
     assert (
-        r"""warning [field_pattern_added] at ./examples/breaking/datacontract-fields-v2.yaml
+        r"""warning [field_pattern_added] at ./fixtures/breaking/datacontract-fields-v2.yaml
         in models.my_table.fields.field_pattern.pattern
             added with value: `^[A-Za-z0-9]{8,14}$`"""
         in output
     )
     assert (
         r"""warning [field_min_length_added] at 
-./examples/breaking/datacontract-fields-v2.yaml
+./fixtures/breaking/datacontract-fields-v2.yaml
         in models.my_table.fields.field_minLength.minLength
             added with value: `8`"""
         in output
     )
     assert (
         r"""warning [field_max_length_added] at 
-./examples/breaking/datacontract-fields-v2.yaml
+./fixtures/breaking/datacontract-fields-v2.yaml
         in models.my_table.fields.field_maxLength.maxLength
             added with value: `14`"""
         in output
     )
     assert (
-        r"""warning [field_minimum_added] at ./examples/breaking/datacontract-fields-v2.yaml
+        r"""warning [field_minimum_added] at ./fixtures/breaking/datacontract-fields-v2.yaml
         in models.my_table.fields.field_minimum.minimum
             added with value: `8`"""
         in output
     )
     assert (
         r"""warning [field_exclusive_minimum_added] at 
-./examples/breaking/datacontract-fields-v2.yaml
+./fixtures/breaking/datacontract-fields-v2.yaml
         in models.my_table.fields.field_exclusiveMinimum.exclusiveMinimum
             added with value: `8`"""
         in output
     )
     assert (
-        r"""warning [field_maximum_added] at ./examples/breaking/datacontract-fields-v2.yaml
+        r"""warning [field_maximum_added] at ./fixtures/breaking/datacontract-fields-v2.yaml
         in models.my_table.fields.field_maximum.maximum
             added with value: `14`"""
         in output
     )
     assert (
         r"""warning [field_exclusive_maximum_added] at 
-./examples/breaking/datacontract-fields-v2.yaml
+./fixtures/breaking/datacontract-fields-v2.yaml
         in models.my_table.fields.field_exclusiveMaximum.exclusiveMaximum
             added with value: `14`"""
         in output
     )
     assert (
-        r"""warning [field_enum_added] at ./examples/breaking/datacontract-fields-v2.yaml
+        r"""warning [field_enum_added] at ./fixtures/breaking/datacontract-fields-v2.yaml
         in models.my_table.fields.field_enum.enum
             added with value: `['one']`"""
         in output
     )
     assert (
-        """info    [field_tags_added] at ./examples/breaking/datacontract-fields-v2.yaml
+        """info    [field_tags_added] at ./fixtures/breaking/datacontract-fields-v2.yaml
         in models.my_table.fields.field_tags.tags
             added with value: `['one']`"""
         in output
     )
 
     assert (
-        r"""warning [field_ref_added] at ./examples/breaking/datacontract-fields-v2.yaml
+        r"""warning [field_ref_added] at ./fixtures/breaking/datacontract-fields-v2.yaml
         in models.my_table.fields.field_ref.$ref
             added with value: `#/definitions/my_definition`"""
         in output
     )
 
     assert (
-        """info    [field_added] at ./examples/breaking/datacontract-fields-v2.yaml
+        """info    [field_added] at ./fixtures/breaking/datacontract-fields-v2.yaml
         in models.my_table.fields.field_fields.fields.new_nested_field
             added the field"""
         in output
     )
 
 
 def test_fields_removed():
     result = runner.invoke(
         app,
         [
             "changelog",
-            "./examples/breaking/datacontract-fields-v2.yaml",
-            "./examples/breaking/datacontract-fields-v1.yaml",
+            "./fixtures/breaking/datacontract-fields-v2.yaml",
+            "./fixtures/breaking/datacontract-fields-v1.yaml",
         ],
     )
     output = result.stdout
     assert result.exit_code == 0
     assert "18 changes: 5 error, 10 warning, 3 info\n" in output
     assert (
-        r"""warning [field_type_removed] at ./examples/breaking/datacontract-fields-v1.yaml
+        r"""warning [field_type_removed] at ./fixtures/breaking/datacontract-fields-v1.yaml
         in models.my_table.fields.field_type.type
             removed field property"""
         in output
     )
     assert (
         r"""warning [field_format_removed] at 
-./examples/breaking/datacontract-fields-v1.yaml
+./fixtures/breaking/datacontract-fields-v1.yaml
         in models.my_table.fields.field_format.format
             removed field property"""
         in output
     )
     assert (
         """warning [field_references_removed] at 
-./examples/breaking/datacontract-fields-v1.yaml
+./fixtures/breaking/datacontract-fields-v1.yaml
         in models.my_table.fields.field_references.references
             removed field property"""
         in output
     )
     assert (
         """info    [field_description_removed] at 
-./examples/breaking/datacontract-fields-v1.yaml
+./fixtures/breaking/datacontract-fields-v1.yaml
         in models.my_table.fields.field_description.description
             removed field property"""
         in output
     )
     assert (
-        r"""error   [field_pii_removed] at ./examples/breaking/datacontract-fields-v1.yaml
+        r"""error   [field_pii_removed] at ./fixtures/breaking/datacontract-fields-v1.yaml
         in models.my_table.fields.field_pii.pii
             removed field property"""
         in output
     )
     assert (
         r"""error   [field_classification_removed] at 
-./examples/breaking/datacontract-fields-v1.yaml
+./fixtures/breaking/datacontract-fields-v1.yaml
         in models.my_table.fields.field_classification.classification
             removed field property"""
         in output
     )
     assert (
         r"""error   [field_pattern_removed] at 
-./examples/breaking/datacontract-fields-v1.yaml
+./fixtures/breaking/datacontract-fields-v1.yaml
         in models.my_table.fields.field_pattern.pattern
             removed field property"""
         in output
     )
     assert (
         r"""warning [field_min_length_removed] at 
-./examples/breaking/datacontract-fields-v1.yaml
+./fixtures/breaking/datacontract-fields-v1.yaml
         in models.my_table.fields.field_minLength.minLength
             removed field property"""
         in output
     )
     assert (
         r"""warning [field_max_length_removed] at 
-./examples/breaking/datacontract-fields-v1.yaml
+./fixtures/breaking/datacontract-fields-v1.yaml
         in models.my_table.fields.field_maxLength.maxLength
             removed field property"""
         in output
     )
     assert (
         r"""warning [field_minimum_removed] at 
-./examples/breaking/datacontract-fields-v1.yaml
+./fixtures/breaking/datacontract-fields-v1.yaml
         in models.my_table.fields.field_minimum.minimum
             removed field property"""
         in output
     )
     assert (
         r"""warning [field_exclusive_minimum_removed] at 
-./examples/breaking/datacontract-fields-v1.yaml
+./fixtures/breaking/datacontract-fields-v1.yaml
         in models.my_table.fields.field_exclusiveMinimum.exclusiveMinimum
             removed field property"""
         in output
     )
     assert (
         r"""warning [field_maximum_removed] at 
-./examples/breaking/datacontract-fields-v1.yaml
+./fixtures/breaking/datacontract-fields-v1.yaml
         in models.my_table.fields.field_maximum.maximum
             removed field property"""
         in output
     )
     assert (
         r"""warning [field_exclusive_maximum_removed] at 
-./examples/breaking/datacontract-fields-v1.yaml
+./fixtures/breaking/datacontract-fields-v1.yaml
         in models.my_table.fields.field_exclusiveMaximum.exclusiveMaximum
             removed field property"""
         in output
     )
     assert (
-        r"""warning [field_ref_removed] at ./examples/breaking/datacontract-fields-v1.yaml
+        r"""warning [field_ref_removed] at ./fixtures/breaking/datacontract-fields-v1.yaml
         in models.my_table.fields.field_ref.$ref
             removed field property"""
         in output
     )
     assert (
-        """info    [field_enum_removed] at ./examples/breaking/datacontract-fields-v1.yaml
+        """info    [field_enum_removed] at ./fixtures/breaking/datacontract-fields-v1.yaml
         in models.my_table.fields.field_enum.enum
             removed field property"""
         in output
     )
     assert (
-        """info    [field_tags_removed] at ./examples/breaking/datacontract-fields-v1.yaml
+        """info    [field_tags_removed] at ./fixtures/breaking/datacontract-fields-v1.yaml
         in models.my_table.fields.field_tags.tags
             removed field property"""
         in output
     )
     assert (
-        r"""error   [field_removed] at ./examples/breaking/datacontract-fields-v1.yaml
+        r"""error   [field_removed] at ./fixtures/breaking/datacontract-fields-v1.yaml
         in models.my_table.fields.field_fields.fields.new_nested_field
             removed the field"""
         in output
     )
     assert (
-        r"""error   [field_removed] at ./examples/breaking/datacontract-fields-v1.yaml
+        r"""error   [field_removed] at ./fixtures/breaking/datacontract-fields-v1.yaml
         in models.my_table.fields.new_field
             removed the field"""
         in output
     )
 
 
 def test_fields_updated():
     result = runner.invoke(
         app,
         [
             "changelog",
-            "./examples/breaking/datacontract-fields-v2.yaml",
-            "./examples/breaking/datacontract-fields-v3.yaml",
+            "./fixtures/breaking/datacontract-fields-v2.yaml",
+            "./fixtures/breaking/datacontract-fields-v3.yaml",
         ],
     )
     output = result.stdout
     assert result.exit_code == 0
     assert "20 changes: 15 error, 3 warning, 2 info\n" in output
     assert (
-        r"""error   [field_type_updated] at ./examples/breaking/datacontract-fields-v3.yaml
+        r"""error   [field_type_updated] at ./fixtures/breaking/datacontract-fields-v3.yaml
         in models.my_table.fields.field_type.type
             changed from `string` to `integer`"""
         in output
     )
     assert (
         """error   [field_format_updated] at 
-./examples/breaking/datacontract-fields-v3.yaml
+./fixtures/breaking/datacontract-fields-v3.yaml
         in models.my_table.fields.field_format.format
             changed from `email` to `url`"""
         in output
     )
     assert (
         """error   [field_required_updated] at 
-./examples/breaking/datacontract-fields-v3.yaml
+./fixtures/breaking/datacontract-fields-v3.yaml
         in models.my_table.fields.field_required.required
             changed from `false` to `true`"""
         in output
     )
     assert (
         """warning [field_primary_updated] at 
-./examples/breaking/datacontract-fields-v3.yaml
+./fixtures/breaking/datacontract-fields-v3.yaml
         in models.my_table.fields.field_primary.primary
             changed from `false` to `true`"""
         in output
     )
     assert (
         """warning [field_references_updated] at 
-./examples/breaking/datacontract-fields-v3.yaml
+./fixtures/breaking/datacontract-fields-v3.yaml
         in models.my_table.fields.field_references.references
             changed from `my_table.field_type` to `my_table.field_format`"""
         in output
     )
     assert (
         r"""error   [field_unique_updated] at 
-./examples/breaking/datacontract-fields-v3.yaml
+./fixtures/breaking/datacontract-fields-v3.yaml
         in models.my_table.fields.field_unique.unique
             changed from `false` to `true`"""
         in output
     )
     assert (
         """info    [field_description_updated] at 
-./examples/breaking/datacontract-fields-v3.yaml
+./fixtures/breaking/datacontract-fields-v3.yaml
         in models.my_table.fields.field_description.description
             changed from `My Description` to `My updated Description`"""
         in output
     )
     assert (
-        r"""error   [field_pii_updated] at ./examples/breaking/datacontract-fields-v3.yaml
+        r"""error   [field_pii_updated] at ./fixtures/breaking/datacontract-fields-v3.yaml
         in models.my_table.fields.field_pii.pii
             changed from `true` to `false`"""
         in output
     )
     assert (
         r"""error   [field_classification_updated] at 
-./examples/breaking/datacontract-fields-v3.yaml
+./fixtures/breaking/datacontract-fields-v3.yaml
         in models.my_table.fields.field_classification.classification
             changed from `sensitive` to `restricted`"""
         in output
     )
     assert (
         r"""error   [field_pattern_updated] at 
-./examples/breaking/datacontract-fields-v3.yaml
+./fixtures/breaking/datacontract-fields-v3.yaml
         in models.my_table.fields.field_pattern.pattern
             changed from `^[A-Za-z0-9]{8,14}$` to `^[A-Za-z0-9]$`"""
         in output
     )
     assert (
         r"""error   [field_min_length_updated] at 
-./examples/breaking/datacontract-fields-v3.yaml
+./fixtures/breaking/datacontract-fields-v3.yaml
         in models.my_table.fields.field_minLength.minLength
             changed from `8` to `10`"""
         in output
     )
     assert (
         r"""error   [field_max_length_updated] at 
-./examples/breaking/datacontract-fields-v3.yaml
+./fixtures/breaking/datacontract-fields-v3.yaml
         in models.my_table.fields.field_maxLength.maxLength
             changed from `14` to `20`"""
         in output
     )
     assert (
         r"""error   [field_minimum_updated] at 
-./examples/breaking/datacontract-fields-v3.yaml
+./fixtures/breaking/datacontract-fields-v3.yaml
         in models.my_table.fields.field_minimum.minimum
             changed from `8` to `10`"""
         in output
     )
     assert (
         r"""error   [field_exclusive_minimum_updated] at 
-./examples/breaking/datacontract-fields-v3.yaml
+./fixtures/breaking/datacontract-fields-v3.yaml
         in models.my_table.fields.field_exclusiveMinimum.exclusiveMinimum
             changed from `8` to `10`"""
         in output
     )
     assert (
         r"""error   [field_maximum_updated] at 
-./examples/breaking/datacontract-fields-v3.yaml
+./fixtures/breaking/datacontract-fields-v3.yaml
         in models.my_table.fields.field_maximum.maximum
             changed from `14` to `20`"""
         in output
     )
     assert (
         r"""error   [field_exclusive_maximum_updated] at 
-./examples/breaking/datacontract-fields-v3.yaml
+./fixtures/breaking/datacontract-fields-v3.yaml
         in models.my_table.fields.field_exclusiveMaximum.exclusiveMaximum
             changed from `14` to `20`"""
         in output
     )
     assert (
-        r"""error   [field_enum_updated] at ./examples/breaking/datacontract-fields-v3.yaml
+        r"""error   [field_enum_updated] at ./fixtures/breaking/datacontract-fields-v3.yaml
         in models.my_table.fields.field_enum.enum
             changed from `['one']` to `['one', 'two']`"""
         in output
     )
     assert (
-        r"""warning [field_ref_updated] at ./examples/breaking/datacontract-fields-v3.yaml
+        r"""warning [field_ref_updated] at ./fixtures/breaking/datacontract-fields-v3.yaml
         in models.my_table.fields.field_ref.$ref
             changed from `#/definitions/my_definition` to 
 `#/definitions/my_definition_2`"""
         in output
     )
     assert (
-        """info    [field_tags_updated] at ./examples/breaking/datacontract-fields-v3.yaml
+        """info    [field_tags_updated] at ./fixtures/breaking/datacontract-fields-v3.yaml
         in models.my_table.fields.field_tags.tags
             changed from `['one']` to `['one', 'two']`"""
         in output
     )
     assert (
-        r"""error   [field_type_updated] at ./examples/breaking/datacontract-fields-v3.yaml
+        r"""error   [field_type_updated] at ./fixtures/breaking/datacontract-fields-v3.yaml
         in models.my_table.fields.field_fields.fields.nested_field_1.type
             changed from `string` to `integer`"""
         in output
     )
 
 
 def test_definition_added():
     result = runner.invoke(
         app,
         [
             "changelog",
-            "./examples/breaking/datacontract-definitions-v1.yaml",
-            "./examples/breaking/datacontract-definitions-v2.yaml",
+            "./fixtures/breaking/datacontract-definitions-v1.yaml",
+            "./fixtures/breaking/datacontract-definitions-v2.yaml",
         ],
     )
     output = result.stdout
 
     assert result.exit_code == 0
     assert "15 changes: 0 error, 13 warning, 2 info\n" in output
     assert (
         r"""warning [field_ref_added] at 
-./examples/breaking/datacontract-definitions-v2.yaml
+./fixtures/breaking/datacontract-definitions-v2.yaml
         in models.my_table.fields.my_field.$ref
             added with value: `#/definitions/my_definition`"""
         in output
     )
     assert (
         r"""warning [field_type_added] at 
-./examples/breaking/datacontract-definitions-v2.yaml
+./fixtures/breaking/datacontract-definitions-v2.yaml
         in models.my_table.fields.my_field.type
             added with value: `string`"""
         in output
     )
     assert (
         """info    [field_description_added] at 
-./examples/breaking/datacontract-definitions-v2.yaml
+./fixtures/breaking/datacontract-definitions-v2.yaml
         in models.my_table.fields.my_field.description
             added with value: `My Description`"""
         in output
     )
     assert (
         r"""warning [field_format_added] at 
-./examples/breaking/datacontract-definitions-v2.yaml
+./fixtures/breaking/datacontract-definitions-v2.yaml
         in models.my_table.fields.my_field.format
             added with value: `uuid`"""
         in output
     )
     assert (
         r"""warning [field_pii_added] at 
-./examples/breaking/datacontract-definitions-v2.yaml
+./fixtures/breaking/datacontract-definitions-v2.yaml
         in models.my_table.fields.my_field.pii
             added with value: `false`"""
         in output
     )
     assert (
         r"""warning [field_classification_added] at 
-./examples/breaking/datacontract-definitions-v2.yaml
+./fixtures/breaking/datacontract-definitions-v2.yaml
         in models.my_table.fields.my_field.classification
             added with value: `internal`"""
         in output
     )
     assert (
         r"""warning [field_pattern_added] at 
-./examples/breaking/datacontract-definitions-v2.yaml
+./fixtures/breaking/datacontract-definitions-v2.yaml
         in models.my_table.fields.my_field.pattern
             added with value: `.*`"""
         in output
     )
     assert (
         r"""warning [field_min_length_added] at 
-./examples/breaking/datacontract-definitions-v2.yaml
+./fixtures/breaking/datacontract-definitions-v2.yaml
         in models.my_table.fields.my_field.minLength
             added with value: `8`"""
         in output
     )
     assert (
         r"""warning [field_max_length_added] at 
-./examples/breaking/datacontract-definitions-v2.yaml
+./fixtures/breaking/datacontract-definitions-v2.yaml
         in models.my_table.fields.my_field.maxLength
             added with value: `14`"""
         in output
     )
     assert (
         r"""warning [field_minimum_added] at 
-./examples/breaking/datacontract-definitions-v2.yaml
+./fixtures/breaking/datacontract-definitions-v2.yaml
         in models.my_table.fields.my_field.minimum
             added with value: `8`"""
         in output
     )
     assert (
         r"""warning [field_exclusive_minimum_added] at 
-./examples/breaking/datacontract-definitions-v2.yaml
+./fixtures/breaking/datacontract-definitions-v2.yaml
         in models.my_table.fields.my_field.exclusiveMinimum
             added with value: `14`"""
         in output
     )
     assert (
         r"""warning [field_maximum_added] at 
-./examples/breaking/datacontract-definitions-v2.yaml
+./fixtures/breaking/datacontract-definitions-v2.yaml
         in models.my_table.fields.my_field.maximum
             added with value: `14`"""
         in output
     )
     assert (
         r"""warning [field_exclusive_maximum_added] at 
-./examples/breaking/datacontract-definitions-v2.yaml
+./fixtures/breaking/datacontract-definitions-v2.yaml
         in models.my_table.fields.my_field.exclusiveMaximum
             added with value: `8`"""
         in output
     )
     assert (
         """info    [field_tags_added] at 
-./examples/breaking/datacontract-definitions-v2.yaml
+./fixtures/breaking/datacontract-definitions-v2.yaml
         in models.my_table.fields.my_field.tags
             added with value: `['my_tags']`"""
         in output
     )
     assert (
         r"""warning [field_enum_added] at 
-./examples/breaking/datacontract-definitions-v2.yaml
+./fixtures/breaking/datacontract-definitions-v2.yaml
         in models.my_table.fields.my_field.enum
             added with value: `['my_enum']`"""
         in output
     )
 
 
 def test_definition_removed():
     result = runner.invoke(
         app,
         [
             "changelog",
-            "./examples/breaking/datacontract-definitions-v2.yaml",
-            "./examples/breaking/datacontract-definitions-v1.yaml",
+            "./fixtures/breaking/datacontract-definitions-v2.yaml",
+            "./fixtures/breaking/datacontract-definitions-v1.yaml",
         ],
     )
     output = result.stdout
 
     assert result.exit_code == 0
     assert "15 changes: 3 error, 9 warning, 3 info\n" in output
     assert (
         r"""warning [field_ref_removed] at 
-./examples/breaking/datacontract-definitions-v1.yaml
+./fixtures/breaking/datacontract-definitions-v1.yaml
         in models.my_table.fields.my_field.$ref
             removed field property"""
         in output
     )
     assert (
         r"""warning [field_type_removed] at 
-./examples/breaking/datacontract-definitions-v1.yaml
+./fixtures/breaking/datacontract-definitions-v1.yaml
         in models.my_table.fields.my_field.type
             removed field property"""
         in output
     )
     assert (
         """info    [field_description_removed] at 
-./examples/breaking/datacontract-definitions-v1.yaml
+./fixtures/breaking/datacontract-definitions-v1.yaml
         in models.my_table.fields.my_field.description
             removed field property"""
         in output
     )
     assert (
         r"""warning [field_format_removed] at 
-./examples/breaking/datacontract-definitions-v1.yaml
+./fixtures/breaking/datacontract-definitions-v1.yaml
         in models.my_table.fields.my_field.format
             removed field property"""
         in output
     )
     assert (
         r"""error   [field_pii_removed] at 
-./examples/breaking/datacontract-definitions-v1.yaml
+./fixtures/breaking/datacontract-definitions-v1.yaml
         in models.my_table.fields.my_field.pii
             removed field property"""
         in output
     )
     assert (
         r"""error   [field_classification_removed] at 
-./examples/breaking/datacontract-definitions-v1.yaml
+./fixtures/breaking/datacontract-definitions-v1.yaml
         in models.my_table.fields.my_field.classification
             removed field property"""
         in output
     )
     assert (
         r"""error   [field_pattern_removed] at 
-./examples/breaking/datacontract-definitions-v1.yaml
+./fixtures/breaking/datacontract-definitions-v1.yaml
         in models.my_table.fields.my_field.pattern
             removed field property"""
         in output
     )
     assert (
         r"""warning [field_min_length_removed] at 
-./examples/breaking/datacontract-definitions-v1.yaml
+./fixtures/breaking/datacontract-definitions-v1.yaml
         in models.my_table.fields.my_field.minLength
             removed field property"""
         in output
     )
     assert (
         r"""warning [field_max_length_removed] at 
-./examples/breaking/datacontract-definitions-v1.yaml
+./fixtures/breaking/datacontract-definitions-v1.yaml
         in models.my_table.fields.my_field.maxLength
             removed field property"""
         in output
     )
     assert (
         r"""warning [field_minimum_removed] at 
-./examples/breaking/datacontract-definitions-v1.yaml
+./fixtures/breaking/datacontract-definitions-v1.yaml
         in models.my_table.fields.my_field.minimum
             removed field property"""
         in output
     )
     assert (
         r"""warning [field_exclusive_minimum_removed] at 
-./examples/breaking/datacontract-definitions-v1.yaml
+./fixtures/breaking/datacontract-definitions-v1.yaml
         in models.my_table.fields.my_field.exclusiveMinimum
             removed field property"""
         in output
     )
     assert (
         r"""warning [field_maximum_removed] at 
-./examples/breaking/datacontract-definitions-v1.yaml
+./fixtures/breaking/datacontract-definitions-v1.yaml
         in models.my_table.fields.my_field.maximum
             removed field property"""
         in output
     )
     assert (
         r"""warning [field_exclusive_maximum_removed] at 
-./examples/breaking/datacontract-definitions-v1.yaml
+./fixtures/breaking/datacontract-definitions-v1.yaml
         in models.my_table.fields.my_field.exclusiveMaximum
             removed field property"""
         in output
     )
     assert (
         """info    [field_tags_removed] at 
-./examples/breaking/datacontract-definitions-v1.yaml
+./fixtures/breaking/datacontract-definitions-v1.yaml
         in models.my_table.fields.my_field.tags
             removed field property"""
         in output
     )
     assert (
         """info    [field_enum_removed] at 
-./examples/breaking/datacontract-definitions-v1.yaml
+./fixtures/breaking/datacontract-definitions-v1.yaml
         in models.my_table.fields.my_field.enum
             removed field property"""
         in output
     )
 
 
 def test_definition_updated():
     result = runner.invoke(
         app,
         [
             "changelog",
-            "./examples/breaking/datacontract-definitions-v2.yaml",
-            "./examples/breaking/datacontract-definitions-v3.yaml",
+            "./fixtures/breaking/datacontract-definitions-v2.yaml",
+            "./fixtures/breaking/datacontract-definitions-v3.yaml",
         ],
     )
     output = result.stdout
 
     assert result.exit_code == 0
     assert "15 changes: 12 error, 1 warning, 2 info\n" in output
     assert (
         r"""warning [field_ref_updated] at 
-./examples/breaking/datacontract-definitions-v3.yaml
+./fixtures/breaking/datacontract-definitions-v3.yaml
         in models.my_table.fields.my_field.$ref
             changed from `#/definitions/my_definition` to 
 `#/definitions/my_definition_2`"""
         in output
     )
     assert (
         r"""error   [field_type_updated] at 
-./examples/breaking/datacontract-definitions-v3.yaml
+./fixtures/breaking/datacontract-definitions-v3.yaml
         in models.my_table.fields.my_field.type
             changed from `string` to `integer`"""
         in output
     )
     assert (
         """info    [field_description_updated] at 
-./examples/breaking/datacontract-definitions-v3.yaml
+./fixtures/breaking/datacontract-definitions-v3.yaml
         in models.my_table.fields.my_field.description
             changed from `My Description` to `My Description 2`"""
         in output
     )
     assert (
         r"""error   [field_format_updated] at 
-./examples/breaking/datacontract-definitions-v3.yaml
+./fixtures/breaking/datacontract-definitions-v3.yaml
         in models.my_table.fields.my_field.format
             changed from `uuid` to `url`"""
         in output
     )
     assert (
         r"""error   [field_pii_updated] at 
-./examples/breaking/datacontract-definitions-v3.yaml
+./fixtures/breaking/datacontract-definitions-v3.yaml
         in models.my_table.fields.my_field.pii
             changed from `false` to `true`"""
         in output
     )
     assert (
         r"""error   [field_classification_updated] at 
-./examples/breaking/datacontract-definitions-v3.yaml
+./fixtures/breaking/datacontract-definitions-v3.yaml
         in models.my_table.fields.my_field.classification
             changed from `internal` to `sensitive`"""
         in output
     )
     assert (
         r"""error   [field_pattern_updated] at 
-./examples/breaking/datacontract-definitions-v3.yaml
+./fixtures/breaking/datacontract-definitions-v3.yaml
         in models.my_table.fields.my_field.pattern
             changed from `.*` to `.*.*`"""
         in output
     )
     assert (
         r"""error   [field_min_length_updated] at 
-./examples/breaking/datacontract-definitions-v3.yaml
+./fixtures/breaking/datacontract-definitions-v3.yaml
         in models.my_table.fields.my_field.minLength
             changed from `8` to `10`"""
         in output
     )
     assert (
         r"""error   [field_max_length_updated] at 
-./examples/breaking/datacontract-definitions-v3.yaml
+./fixtures/breaking/datacontract-definitions-v3.yaml
         in models.my_table.fields.my_field.maxLength
             changed from `14` to `20`"""
         in output
     )
     assert (
         r"""error   [field_minimum_updated] at 
-./examples/breaking/datacontract-definitions-v3.yaml
+./fixtures/breaking/datacontract-definitions-v3.yaml
         in models.my_table.fields.my_field.minimum
             changed from `8` to `10`"""
         in output
     )
     assert (
         r"""error   [field_exclusive_minimum_updated] at 
-./examples/breaking/datacontract-definitions-v3.yaml
+./fixtures/breaking/datacontract-definitions-v3.yaml
         in models.my_table.fields.my_field.exclusiveMinimum
             changed from `14` to `10`"""
         in output
     )
     assert (
         r"""error   [field_maximum_updated] at 
-./examples/breaking/datacontract-definitions-v3.yaml
+./fixtures/breaking/datacontract-definitions-v3.yaml
         in models.my_table.fields.my_field.maximum
             changed from `14` to `20`"""
         in output
     )
     assert (
         r"""error   [field_exclusive_maximum_updated] at 
-./examples/breaking/datacontract-definitions-v3.yaml
+./fixtures/breaking/datacontract-definitions-v3.yaml
         in models.my_table.fields.my_field.exclusiveMaximum
             changed from `8` to `20`"""
         in output
     )
     assert (
         """info    [field_tags_updated] at 
-./examples/breaking/datacontract-definitions-v3.yaml
+./fixtures/breaking/datacontract-definitions-v3.yaml
         in models.my_table.fields.my_field.tags
             changed from `['my_tags']` to `['my_tags_2']`"""
         in output
     )
     assert (
         """error   [field_enum_updated] at 
-./examples/breaking/datacontract-definitions-v3.yaml
+./fixtures/breaking/datacontract-definitions-v3.yaml
         in models.my_table.fields.my_field.enum
             changed from `['my_enum']` to `['my_enum_2']`"""
         in output
     )
```

### Comparing `datacontract-cli-0.9.8/tests/test_documentation_linter.py` & `datacontract_cli-0.9.9/tests/test_documentation_linter.py`

 * *Files identical despite different names*

### Comparing `datacontract-cli-0.9.8/tests/test_download_datacontract_file.py` & `datacontract_cli-0.9.9/tests/test_download_datacontract_file.py`

 * *Files identical despite different names*

### Comparing `datacontract-cli-0.9.8/tests/test_example_model_linter.py` & `datacontract_cli-0.9.9/tests/test_example_model_linter.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,70 +10,70 @@
     )
 
 
 success_check = Check(type="lint", name="Linter 'Example(s) match model'", result="passed", engine="datacontract")
 
 
 def test_lint_invalid_model():
-    data_contract_file = "examples/lint/datacontract_unknown_model.yaml"
+    data_contract_file = "fixtures/lint/datacontract_unknown_model.yaml"
     contract = resolve.resolve_data_contract_from_location(data_contract_file)
     result = ExampleModelLinter().lint(contract)
     expected = construct_error_check("Example 1 has non-existent model 'orders'")
     assert result == [expected]
 
 
 def test_lint_valid_csv_columns():
-    contract = resolve.resolve_data_contract_from_location("examples/lint/datacontract_csv_lint_base.yaml")
+    contract = resolve.resolve_data_contract_from_location("fixtures/lint/datacontract_csv_lint_base.yaml")
     result = ExampleModelLinter().lint(contract)
     assert result == [success_check]
 
 
 def test_lint_extra_model_columns():
-    base_spec = resolve.resolve_data_contract_from_location("examples/lint/datacontract_csv_lint_base.yaml")
+    base_spec = resolve.resolve_data_contract_from_location("fixtures/lint/datacontract_csv_lint_base.yaml")
     base_spec.models["orders"] = spec.Model(
         fields={
             "column_1": spec.Field(type="str"),
             "column_2": spec.Field(type="str"),
             "column_3": spec.Field(type="str", required=True),
         }
     )
     result = ExampleModelLinter().lint(base_spec)
     expected = construct_error_check("Example 1 is missing field 'column_3' required by model 'orders'")
     assert result == [expected]
 
 
 def test_lint_extra_example_columns():
-    base_spec = resolve.resolve_data_contract_from_location("examples/lint/datacontract_csv_lint_base.yaml")
+    base_spec = resolve.resolve_data_contract_from_location("fixtures/lint/datacontract_csv_lint_base.yaml")
     base_spec.examples[0] = spec.Example(
         type="csv", model="orders", data="column_1, column_2, column_3\nvalue_1, value_2, value_3"
     )
     result = ExampleModelLinter().lint(base_spec)
     expected = construct_error_check("Example 1 has field 'column_3' that's not contained in model 'orders'")
     assert result == [expected]
 
 
 def test_lint_json_example():
-    base_spec = resolve.resolve_data_contract_from_location("examples/lint/datacontract_csv_lint_base.yaml")
+    base_spec = resolve.resolve_data_contract_from_location("fixtures/lint/datacontract_csv_lint_base.yaml")
     base_spec.examples[0] = spec.Example(type="json", model="orders", data='{"column_1": 1, "column_2": 2}')
     result = ExampleModelLinter().lint(base_spec)
     assert result == [success_check]
 
 
 def test_lint_json_example_extra_columns():
-    base_spec = resolve.resolve_data_contract_from_location("examples/lint/datacontract_csv_lint_base.yaml")
+    base_spec = resolve.resolve_data_contract_from_location("fixtures/lint/datacontract_csv_lint_base.yaml")
     base_spec.examples[0] = spec.Example(
         type="json", model="orders", data='{"column_1": 1, "column_2": 2, "column_3": 3}'
     )
     result = ExampleModelLinter().lint(base_spec)
     expected = construct_error_check("Example 1 has field 'column_3' that's not contained in model 'orders'")
     assert result == [expected]
 
 
 def test_lint_yaml_example():
-    base_spec = resolve.resolve_data_contract_from_location("examples/lint/datacontract_csv_lint_base.yaml")
+    base_spec = resolve.resolve_data_contract_from_location("fixtures/lint/datacontract_csv_lint_base.yaml")
     base_spec.examples[0] = spec.Example(
         type="yaml",
         model="orders",
         data="""
 column_1: 1
 column_2: 2
 """,
```

### Comparing `datacontract-cli-0.9.8/tests/test_examples_bigquery.py` & `datacontract_cli-0.9.9/tests/test_test_bigquery.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,26 +4,27 @@
 import pytest
 from dotenv import load_dotenv
 
 from datacontract.data_contract import DataContract
 
 logging.basicConfig(level=logging.INFO, force=True)
 
-datacontract = "examples/bigquery/datacontract.yaml"
+datacontract = "fixtures/bigquery/datacontract.yaml"
 
 load_dotenv(override=True)
 
+
 # Deactivated because the test requires special setup on a non-free BigQuery account.
 # Can activate for testing locally, using a custom account_info file.
 # For the provided datacontract.yaml the data file from s3-csv should be imported in the target BigQuery table.
 @pytest.mark.skipif(
     os.environ.get("DATACONTRACT_BIGQUERY_ACCOUNT_INFO_JSON_PATH") is None,
     reason="Requires DATACONTRACT_BIGQUERY_ACCOUNT_INFO_JSON_PATH to be set",
 )
-def _test_examples_bigquery():
+def _test_test_bigquery():
     data_contract = DataContract(data_contract_file=datacontract)
 
     run = data_contract.test()
 
     print(run)
     assert run.result == "passed"
     assert all(check.result == "passed" for check in run.checks)
```

### Comparing `datacontract-cli-0.9.8/tests/test_examples_databricks.py` & `datacontract_cli-0.9.9/tests/test_test_databricks.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,23 +4,23 @@
 import pytest
 from dotenv import load_dotenv
 
 from datacontract.data_contract import DataContract
 
 logging.basicConfig(level=logging.DEBUG, force=True)
 
-datacontract = "examples/databricks-sql/datacontract.yaml"
+datacontract = "fixtures/databricks-sql/datacontract.yaml"
 
 load_dotenv(override=True)
 
 
 @pytest.mark.skipif(
     os.environ.get("DATACONTRACT_DATABRICKS_TOKEN") is None, reason="Requires DATACONTRACT_DATABRICKS_TOKEN to be set"
 )
-def test_examples_databricks_sql():
+def test_test_databricks_sql():
     # os.environ['DATACONTRACT_DATABRICKS_TOKEN'] = "xxx"
     # os.environ['DATACONTRACT_DATABRICKS_HTTP_PATH'] = "/sql/1.0/warehouses/b053a326fa014fb3"
     data_contract = DataContract(data_contract_file=datacontract)
 
     run = data_contract.test()
 
     print(run)
```

### Comparing `datacontract-cli-0.9.8/tests/test_examples_examples_csv.py` & `datacontract_cli-0.9.9/tests/test_test_examples_csv.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,25 +7,25 @@
 
 runner = CliRunner()
 
 logging.basicConfig(level=logging.DEBUG, force=True)
 
 
 def test_cli():
-    result = runner.invoke(app, ["test", "--examples", "./examples/examples/datacontract_csv.yaml"])
+    result = runner.invoke(app, ["test", "--examples", "./fixtures/examples/datacontract_csv.yaml"])
     assert result.exit_code == 0
 
 
 def test_csv():
-    data_contract = DataContract(data_contract_file="examples/examples/datacontract_csv.yaml", examples=True)
+    data_contract = DataContract(data_contract_file="fixtures/examples/datacontract_csv.yaml", examples=True)
     run = data_contract.test()
     print(run)
     print(run.result)
     assert run.result == "passed"
 
 
 def test_csv_orders():
-    data_contract = DataContract(data_contract_file="examples/s3-json-remote/datacontract.yaml", examples=True)
+    data_contract = DataContract(data_contract_file="fixtures/s3-json-remote/datacontract.yaml", examples=True)
     run = data_contract.test()
     print(run)
     print(run.result)
     assert run.result == "passed"
```

### Comparing `datacontract-cli-0.9.8/tests/test_examples_examples_inline.py` & `datacontract_cli-0.9.9/tests/test_test_examples_inline.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 
 runner = CliRunner()
 
 logging.basicConfig(level=logging.DEBUG, force=True)
 
 
 def test_cli():
-    result = runner.invoke(app, ["test", "--examples", "./examples/examples/datacontract_inline.yaml"])
+    result = runner.invoke(app, ["test", "--examples", "./fixtures/examples/datacontract_inline.yaml"])
     assert result.exit_code == 0
 
 
 def test_json_inline():
-    data_contract = DataContract(data_contract_file="examples/examples/datacontract_inline.yaml", examples=True)
+    data_contract = DataContract(data_contract_file="fixtures/examples/datacontract_inline.yaml", examples=True)
     run = data_contract.test()
     print(run)
     print(run.result)
     assert run.result == "passed"
```

### Comparing `datacontract-cli-0.9.8/tests/test_examples_examples_json.py` & `datacontract_cli-0.9.9/tests/test_test_examples_json.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 
 runner = CliRunner()
 
 logging.basicConfig(level=logging.DEBUG, force=True)
 
 
 def test_cli():
-    result = runner.invoke(app, ["test", "--examples", "./examples/examples/datacontract_json.yaml"])
+    result = runner.invoke(app, ["test", "--examples", "./fixtures/examples/datacontract_json.yaml"])
     assert result.exit_code == 0
 
 
 def test_json():
-    data_contract = DataContract(data_contract_file="examples/examples/datacontract_json.yaml", examples=True)
+    data_contract = DataContract(data_contract_file="fixtures/examples/datacontract_json.yaml", examples=True)
     run = data_contract.test()
     print(run)
     print(run.result)
     assert run.result == "passed"
```

### Comparing `datacontract-cli-0.9.8/tests/test_examples_examples_missing.py` & `datacontract_cli-0.9.9/tests/test_test_examples_missing.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 
 runner = CliRunner()
 
 logging.basicConfig(level=logging.DEBUG, force=True)
 
 
 def test_cli():
-    result = runner.invoke(app, ["test", "--examples", "./examples/examples/datacontract_missing.yaml"])
+    result = runner.invoke(app, ["test", "--examples", "./fixtures/examples/datacontract_missing.yaml"])
     assert result.exit_code == 1
 
 
 def test_missing():
-    data_contract = DataContract(data_contract_file="examples/examples/datacontract_missing.yaml", examples=True)
+    data_contract = DataContract(data_contract_file="fixtures/examples/datacontract_missing.yaml", examples=True)
     run = data_contract.test()
     print(run)
     print(run.result)
     assert run.result == "warning"
```

### Comparing `datacontract-cli-0.9.8/tests/test_examples_kafka.py` & `datacontract_cli-0.9.9/tests/test_test_kafka.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,31 +13,35 @@
 from kafka import KafkaProducer
 from testcontainers.kafka import KafkaContainer
 
 from datacontract.data_contract import DataContract
 
 logging.basicConfig(level=logging.INFO, force=True)
 
-datacontract = "examples/kafka/datacontract.yaml"
+datacontract = "fixtures/kafka/datacontract.yaml"
 
 kafka = KafkaContainer("confluentinc/cp-kafka:7.6.0")
 
 
 @pytest.fixture(scope="module", autouse=True)
 def kafka_container(request):
     kafka.start()
 
     def remove_container():
         kafka.stop()
 
     request.addfinalizer(remove_container)
 
 
-def test_examples_kafka(kafka_container: KafkaContainer):
-    send_messages_to_topic("examples/kafka/data/messages.json", "inventory-events")
+@pytest.mark.skipif(
+    sys.platform == "darwin",
+    reason="Fails on ARM mac, https://github.com/testcontainers/testcontainers-python/issues/450",
+)
+def test_test_kafka(kafka_container: KafkaContainer):
+    send_messages_to_topic("fixtures/kafka/data/messages.json", "inventory-events")
     data_contract_str = _setup_datacontract()
     data_contract = DataContract(data_contract_str=data_contract_str)
 
     run = data_contract.test()
 
     print(run)
     assert run.result == "passed"
```

### Comparing `datacontract-cli-0.9.8/tests/test_examples_kafka_remote.py` & `datacontract_cli-0.9.9/tests/test_test_kafka_remote.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,33 +17,33 @@
 logging.basicConfig(level=logging.INFO, force=True)
 
 
 @pytest.mark.skipif(
     os.environ.get("DATACONTRACT_KAFKA_SASL_USERNAME") is None,
     reason="Requires DATACONTRACT_KAFKA_SASL_USERNAME to be set",
 )
-def _test_examples_kafka_json_remote():
+def _test_test_kafka_json_remote():
     load_dotenv(override=True)
     # os.environ['DATACONTRACT_KAFKA_SASL_USERNAME'] = "xxx"
     # os.environ['DATACONTRACT_KAFKA_SASL_PASSWORD'] = "xxx"
-    data_contract = DataContract(data_contract_file="examples/kafka-json-remote/datacontract.yaml")
+    data_contract = DataContract(data_contract_file="fixtures/kafka-json-remote/datacontract.yaml")
 
     run = data_contract.test()
 
     print(run)
     assert run.result == "passed"
 
 
 @pytest.mark.skipif(
     os.environ.get("DATACONTRACT_KAFKA_SASL_USERNAME") is None,
     reason="Requires DATACONTRACT_KAFKA_SASL_USERNAME to be set",
 )
-def _test_examples_kafka_avro_remote():
+def _test_test_kafka_avro_remote():
     load_dotenv(override=True)
     # os.environ['DATACONTRACT_KAFKA_SASL_USERNAME'] = "xxx"
     # os.environ['DATACONTRACT_KAFKA_SASL_PASSWORD'] = "xxx"
-    data_contract = DataContract(data_contract_file="examples/kafka-avro-remote/datacontract.yaml")
+    data_contract = DataContract(data_contract_file="fixtures/kafka-avro-remote/datacontract.yaml")
 
     run = data_contract.test()
 
     print(run)
     assert run.result == "passed"
```

### Comparing `datacontract-cli-0.9.8/tests/test_examples_local_json.py` & `datacontract_cli-0.9.9/tests/test_integration_datameshmanager.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,23 @@
-import pytest
+import logging
+
 from typer.testing import CliRunner
 
-from datacontract.cli import app
-from datacontract.data_contract import DataContract
+logging.basicConfig(level=logging.DEBUG, force=True)
 
 runner = CliRunner()
 
 
-@pytest.mark.skip(reason="https://github.com/sodadata/soda-core/issues/1992")
-def _test_cli():
-    result = runner.invoke(app, ["test", "./examples/local-json/datacontract.yaml"])
-    assert result.exit_code == 0
-
-
-@pytest.mark.skip(reason="https://github.com/sodadata/soda-core/issues/1992")
-def _test_local_json():
-    data_contract = DataContract(data_contract_file="examples/local-json/datacontract.yaml")
-    run = data_contract.test()
-    print(run)
-    assert run.result == "passed"
+# @pytest.mark.skipif(os.environ.get("DATAMESH_MANAGER_API_KEY") is None, reason="Requires DATAMESH_MANAGER_API_KEY to be set")
+# def test_remote_data_contract():
+#     load_dotenv(override=True)
+#     data_contract = DataContract(
+#         data_contract_file="https://innoq.datamesh-manager.com/checker/datacontracts/6b49c320-aaa2-4d26-bfaf-9f356a711175",
+#         publish_url="https://api.datamesh-manager.com/api/runs"
+#     )
+#
+#     run = data_contract.test()
+#
+#     print(run)
+#     assert run.result == "passed"
+#     assert len(run.checks) == 4
+#     assert all(check.result == "passed" for check in run.checks)
```

### Comparing `datacontract-cli-0.9.8/tests/test_examples_parquet.py` & `datacontract_cli-0.9.9/tests/test_export_html.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,29 +1,25 @@
-import os
+import logging
 
 from typer.testing import CliRunner
 
 from datacontract.cli import app
-from datacontract.data_contract import DataContract
+from datacontract.export.html_export import to_html
+from datacontract.model.data_contract_specification import \
+    DataContractSpecification
 
-runner = CliRunner()
+logging.basicConfig(level=logging.DEBUG, force=True)
 
 
-def test_valid_cli():
-    current_file_path = os.path.abspath(__file__)
-    print("DEBUG Current file path:" + current_file_path)
-
-    result = runner.invoke(app, ["test", "./examples/parquet/datacontract.yaml"])
+def test_cli():
+    runner = CliRunner()
+    result = runner.invoke(app, ["export", "./fixtures/export/datacontract.yaml", "--format", "html"])
     assert result.exit_code == 0
-    assert "Testing ./examples/parquet/datacontract.yaml" in result.stdout
 
 
-def test_valid():
-    data_contract = DataContract(
-        data_contract_file="./examples/parquet/datacontract.yaml",
-        # publish=True,
-    )
-    run = data_contract.test()
-    print(run)
-    assert run.result == "passed"
-    assert len(run.checks) == 4
-    assert all(check.result == "passed" for check in run.checks)
+def test_to_html():
+    data_contract = DataContractSpecification.from_file("fixtures/export/datacontract.yaml")
+    expected_html = """<html"""
+
+    html = to_html(data_contract)
+
+    assert expected_html in html
```

### Comparing `datacontract-cli-0.9.8/tests/test_examples_postgres.py` & `datacontract_cli-0.9.9/tests/test_test_postgres.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 import pytest
 from testcontainers.postgres import PostgresContainer
 
 from datacontract.data_contract import DataContract
 
 logging.basicConfig(level=logging.DEBUG, force=True)
 
-datacontract = "examples/postgres/datacontract.yaml"
-sql_file_path = "examples/postgres/data/data.sql"
+datacontract = "fixtures/postgres/datacontract.yaml"
+sql_file_path = "fixtures/postgres/data/data.sql"
 
 postgres = PostgresContainer("postgres:16")
 
 
 @pytest.fixture(scope="module", autouse=True)
 def postgres_container(request):
     postgres.start()
@@ -23,15 +23,15 @@
         postgres.stop()
 
     request.addfinalizer(remove_container)
     os.environ["DATACONTRACT_POSTGRES_USERNAME"] = postgres.POSTGRES_USER
     os.environ["DATACONTRACT_POSTGRES_PASSWORD"] = postgres.POSTGRES_PASSWORD
 
 
-def test_examples_postgres(postgres_container):
+def test_test_postgres(postgres_container):
     _init_sql()
 
     data_contract_str = _setup_datacontract()
     data_contract = DataContract(data_contract_str=data_contract_str)
 
     run = data_contract.test()
```

### Comparing `datacontract-cli-0.9.8/tests/test_examples_s3_csv.py` & `datacontract_cli-0.9.9/tests/test_test_s3_csv.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,30 +4,30 @@
 import pytest
 from testcontainers.minio import MinioContainer
 
 from datacontract.data_contract import DataContract
 
 logging.basicConfig(level=logging.DEBUG, force=True)
 
-datacontract = "examples/s3-csv/datacontract.yaml"
-file_name = "examples/s3-csv/data/sample_data.csv"
+datacontract = "fixtures/s3-csv/datacontract.yaml"
+file_name = "fixtures/s3-csv/data/sample_data.csv"
 bucket_name = "test-bucket"
 s3_access_key = "test-access"
 s3_secret_access_key = "test-secret"
 
 
 @pytest.fixture(scope="session")
 def minio_container():
     with MinioContainer(
         image="quay.io/minio/minio", access_key=s3_access_key, secret_key=s3_secret_access_key
     ) as minio_container:
         yield minio_container
 
 
-def test_examples_s3_csv(minio_container, monkeypatch):
+def test_test_s3_csv(minio_container, monkeypatch):
     monkeypatch.setenv("DATACONTRACT_S3_ACCESS_KEY_ID", s3_access_key)
     monkeypatch.setenv("DATACONTRACT_S3_SECRET_ACCESS_KEY", s3_secret_access_key)
     data_contract_str = _prepare_s3_files(minio_container)
     data_contract = DataContract(data_contract_str=data_contract_str)
 
     run = data_contract.test()
```

### Comparing `datacontract-cli-0.9.8/tests/test_examples_s3_json.py` & `datacontract_cli-0.9.9/tests/test_test_s3_json_complex.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,38 +1,40 @@
 import os
 
 import pytest
 from testcontainers.minio import MinioContainer
 
 from datacontract.data_contract import DataContract
 
-datacontract = "examples/s3-json/datacontract.yaml"
-file_name = "examples/s3-json/data/inventory/year=2022/month=04/day=20/hour=00/inventory+0+0001327496.json"
-bucket_name = "test-bucket"
+datacontract = "./fixtures/s3-json-complex/datacontract.yaml"
+file_name = "fixtures/s3-json-complex/data/feed.json"
+bucket_name = "feed-bucket"
 s3_access_key = "test-access"
 s3_secret_access_key = "test-secret"
 
 
 @pytest.fixture(scope="session")
 def minio_container():
     with MinioContainer(
         image="quay.io/minio/minio", access_key=s3_access_key, secret_key=s3_secret_access_key
     ) as minio_container:
         yield minio_container
 
 
-def test_examples_s3_json(minio_container, monkeypatch):
-    monkeypatch.setenv("DATACONTRACT_S3_ACCESS_KEY_ID", "test-access")
-    monkeypatch.setenv("DATACONTRACT_S3_SECRET_ACCESS_KEY", "test-secret")
+def test_test_s3_json(minio_container):
+    os.environ["DATACONTRACT_S3_ACCESS_KEY_ID"] = "test-access"
+    os.environ["DATACONTRACT_S3_SECRET_ACCESS_KEY"] = "test-secret"
+
     data_contract_str = _prepare_s3_files(minio_container)
+
     data_contract = DataContract(data_contract_str=data_contract_str)
 
     run = data_contract.test()
 
-    print(run)
+    print(run.pretty())
     assert run.result == "passed"
     assert all(check.result == "passed" for check in run.checks)
 
 
 def _prepare_s3_files(minio_container):
     s3_endpoint_url = f"http://{minio_container.get_container_host_ip()}:{minio_container.get_exposed_port(9000)}"
     minio_client = minio_container.get_client()
```

### Comparing `datacontract-cli-0.9.8/tests/test_examples_s3_json_complex.py` & `datacontract_cli-0.9.9/tests/test_test_s3_json.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,40 +1,38 @@
 import os
 
 import pytest
 from testcontainers.minio import MinioContainer
 
 from datacontract.data_contract import DataContract
 
-datacontract = "./examples/s3-json-complex/datacontract.yaml"
-file_name = "examples/s3-json-complex/data/feed.json"
-bucket_name = "feed-bucket"
+datacontract = "fixtures/s3-json/datacontract.yaml"
+file_name = "fixtures/s3-json/data/inventory/year=2022/month=04/day=20/hour=00/inventory+0+0001327496.json"
+bucket_name = "test-bucket"
 s3_access_key = "test-access"
 s3_secret_access_key = "test-secret"
 
 
 @pytest.fixture(scope="session")
 def minio_container():
     with MinioContainer(
         image="quay.io/minio/minio", access_key=s3_access_key, secret_key=s3_secret_access_key
     ) as minio_container:
         yield minio_container
 
 
-def test_examples_s3_json(minio_container):
-    os.environ["DATACONTRACT_S3_ACCESS_KEY_ID"] = "test-access"
-    os.environ["DATACONTRACT_S3_SECRET_ACCESS_KEY"] = "test-secret"
-
+def test_test_s3_json(minio_container, monkeypatch):
+    monkeypatch.setenv("DATACONTRACT_S3_ACCESS_KEY_ID", "test-access")
+    monkeypatch.setenv("DATACONTRACT_S3_SECRET_ACCESS_KEY", "test-secret")
     data_contract_str = _prepare_s3_files(minio_container)
-
     data_contract = DataContract(data_contract_str=data_contract_str)
 
     run = data_contract.test()
 
-    print(run.pretty())
+    print(run)
     assert run.result == "passed"
     assert all(check.result == "passed" for check in run.checks)
 
 
 def _prepare_s3_files(minio_container):
     s3_endpoint_url = f"http://{minio_container.get_container_host_ip()}:{minio_container.get_exposed_port(9000)}"
     minio_client = minio_container.get_client()
```

### Comparing `datacontract-cli-0.9.8/tests/test_examples_s3_json_multiple_models.py` & `datacontract_cli-0.9.9/tests/test_test_s3_json_multiple_models.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 import os
 
 import pytest
 from testcontainers.minio import MinioContainer
 
 from datacontract.data_contract import DataContract
 
-datacontract = "./examples/s3-json-multiple-models/datacontract.yaml"
-data_directory = "./examples/s3-json-multiple-models/data/"
+datacontract = "./fixtures/s3-json-multiple-models/datacontract.yaml"
+data_directory = "./fixtures/s3-json-multiple-models/data/"
 bucket_name = "multiple-bucket"
 s3_access_key = "test-access"
 s3_secret_access_key = "test-secret"
 
 logging.basicConfig(level=logging.INFO, force=True)
 
 
@@ -19,15 +19,15 @@
 def minio_container():
     with MinioContainer(
         image="quay.io/minio/minio", access_key=s3_access_key, secret_key=s3_secret_access_key
     ) as minio_container:
         yield minio_container
 
 
-def test_examples_s3_json(minio_container):
+def test_test_s3_json(minio_container):
     os.environ["DATACONTRACT_S3_ACCESS_KEY_ID"] = s3_access_key
     os.environ["DATACONTRACT_S3_SECRET_ACCESS_KEY"] = s3_secret_access_key
 
     data_contract_str = _prepare_s3_files(minio_container)
 
     data_contract = DataContract(data_contract_str=data_contract_str)
```

### Comparing `datacontract-cli-0.9.8/tests/test_examples_s3_json_remote.py` & `datacontract_cli-0.9.9/tests/test_test_s3_json_remote.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import logging
 import os
 
 from datacontract.data_contract import DataContract
 
 logging.basicConfig(level=logging.INFO, force=True)
 
-datacontract = "examples/s3-json-remote/datacontract.yaml"
+datacontract = "fixtures/s3-json-remote/datacontract.yaml"
 
 
-def test_examples_s3_json():
+def test_test_s3_json():
     if "AWS_ACCESS_KEY_ID" in os.environ:
         del os.environ["AWS_ACCESS_KEY_ID"]
     if "AWS_SECRET_ACCESS_KEY" in os.environ:
         del os.environ["AWS_SECRET_ACCESS_KEY"]
     if "DATACONTRACT_S3_ACCESS_KEY_ID" in os.environ:
         del os.environ["DATACONTRACT_S3_ACCESS_KEY_ID"]
     if "DATACONTRACT_S3_SECRET_ACCESS_KEY" in os.environ:
```

### Comparing `datacontract-cli-0.9.8/tests/test_examples_snowflake.py` & `datacontract_cli-0.9.9/tests/test_test_snowflake.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import logging
 
 logging.basicConfig(level=logging.INFO, force=True)
 
-datacontract = "examples/snowflake/datacontract.yaml"
+datacontract = "fixtures/snowflake/datacontract.yaml"
 
 
 # @pytest.mark.skipif(os.environ.get("DATACONTRACT_SNOWFLAKE_USERNAME") is None, reason="Requires DATACONTRACT_SNOWFLAKE_USERNAME to be set")
-# def test_examples_snowflake():
+# def test_test_snowflake():
 #     load_dotenv(override=True)
 #     # os.environ['DATACONTRACT_SNOWFLAKE_USERNAME'] = "xxx"
 #     # os.environ['DATACONTRACT_SNOWFLAKE_PASSWORD'] = "xxx"
 #     # os.environ['DATACONTRACT_SNOWFLAKE_ROLE'] = "xxx"
 #     # os.environ['DATACONTRACT_SNOWFLAKE_WAREHOUSE'] = "COMPUTE_WH"
 #     data_contract = DataContract(data_contract_file=datacontract)
 #
```

### Comparing `datacontract-cli-0.9.8/tests/test_export_avro.py` & `datacontract_cli-0.9.9/tests/test_export_avro.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,28 @@
 import json
 import logging
-import os
-import sys
 
 from typer.testing import CliRunner
 
 from datacontract.cli import app
 from datacontract.export.avro_converter import to_avro_schema_json
 from datacontract.model.data_contract_specification import \
     DataContractSpecification
 
 logging.basicConfig(level=logging.DEBUG, force=True)
 
 
 def test_cli():
     runner = CliRunner()
-    result = runner.invoke(app, ["export", "./examples/kafka-avro-remote/datacontract.yaml", "--format", "avro"])
+    result = runner.invoke(app, ["export", "./fixtures/kafka-avro-remote/datacontract.yaml", "--format", "avro"])
     assert result.exit_code == 0
 
 
 def test_to_avro_schema():
-    data_contract = DataContractSpecification.from_file("./examples/kafka-avro-remote/datacontract.yaml")
+    data_contract = DataContractSpecification.from_file("fixtures/kafka-avro-remote/datacontract.yaml")
     expected_avro_schema = """
     {
   "fields": [
     {
       "name": "ordertime",
       "doc": "My Field",
       "type": "long"
@@ -60,25 +58,17 @@
         ],
         "name": "address",
         "type": "record"
       }
     }
   ],
   "name": "orders",
+  "namespace": "com.example.checkout",
   "doc": "My Model",
   "type": "record"
 }
 """
 
     model_name, model = next(iter(data_contract.models.items()))
     result = to_avro_schema_json(model_name, model)
 
     assert json.loads(result) == json.loads(expected_avro_schema)
-
-
-def read_file(data_contract_file):
-    if not os.path.exists(data_contract_file):
-        print(f"The file '{data_contract_file}' does not exist.")
-        sys.exit(1)
-    with open(data_contract_file, "r") as file:
-        file_content = file.read()
-    return file_content
```

### Comparing `datacontract-cli-0.9.8/tests/test_export_avro_idl.py` & `datacontract_cli-0.9.9/tests/test_export_avro_idl.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     to_avro_idl,
 )
 from datacontract.lint.resolve import resolve_data_contract_from_location
 
 
 def test_ir():
     contract = resolve_data_contract_from_location(
-        "examples/lint/valid_datacontract_references.yaml", inline_definitions=True
+        "fixtures/lint/valid_datacontract_references.yaml", inline_definitions=True
     )
     expected = AvroIDLProtocol(
         name="OrdersLatest",
         description="Successful customer orders in the webshop.\n"
         "All orders since 2020-01-01.\n"
         "Orders with their line items are in their current state (no history included).\n",
         model_types=[
@@ -40,15 +40,15 @@
         ],
     )
     assert _contract_to_avro_idl_ir(contract) == expected
 
 
 def test_avro_idl_str():
     contract = resolve_data_contract_from_location(
-        "examples/lint/valid_datacontract_references.yaml", inline_definitions=True
+        "fixtures/lint/valid_datacontract_references.yaml", inline_definitions=True
     )
     expected = dedent(
         """
           /** Successful customer orders in the webshop.
           All orders since 2020-01-01.
           Orders with their line items are in their current state (no history included).
            */
@@ -63,15 +63,15 @@
     ).strip()
     assert to_avro_idl(contract).strip() == expected
 
 
 def test_avro_idl_cli_export():
     runner = CliRunner()
     result = runner.invoke(
-        app, ["export", "./examples/lint/valid_datacontract_references.yaml", "--format", "avro-idl"]
+        app, ["export", "./fixtures/lint/valid_datacontract_references.yaml", "--format", "avro-idl"]
     )
     if result.exit_code:
         print(result.output)
     assert result.exit_code == 0
 
 
 def test_avro_idl_complex_type():
```

### Comparing `datacontract-cli-0.9.8/tests/test_export_dbt_models.py` & `datacontract_cli-0.9.9/tests/test_export_dbt_models.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,20 +11,20 @@
     DataContractSpecification
 
 logging.basicConfig(level=logging.DEBUG, force=True)
 
 
 def test_cli():
     runner = CliRunner()
-    result = runner.invoke(app, ["export", "./examples/export/datacontract.yaml", "--format", "dbt"])
+    result = runner.invoke(app, ["export", "./fixtures/export/datacontract.yaml", "--format", "dbt"])
     assert result.exit_code == 0
 
 
 def test_to_dbt_models():
-    data_contract = DataContractSpecification.from_file("./examples/export/datacontract.yaml")
+    data_contract = DataContractSpecification.from_file("fixtures/export/datacontract.yaml")
     expected_dbt_model = """
 version: 2
 models:
   - name: orders    
     config:
       meta:
         owner: checkout
```

### Comparing `datacontract-cli-0.9.8/tests/test_export_dbt_sources.py` & `datacontract_cli-0.9.9/tests/test_export_dbt_sources.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,22 +10,22 @@
 
 logging.basicConfig(level=logging.DEBUG, force=True)
 
 
 def test_cli():
     runner = CliRunner()
     result = runner.invoke(
-        app, ["export", "./examples/export/datacontract.yaml", "--format", "dbt-sources", "--server", "production"]
+        app, ["export", "./fixtures/export/datacontract.yaml", "--format", "dbt-sources", "--server", "production"]
     )
     print(result.stdout)
     assert result.exit_code == 0
 
 
 def test_to_dbt_sources():
-    data_contract = DataContractSpecification.from_file("./examples/export/datacontract.yaml")
+    data_contract = DataContractSpecification.from_file("fixtures/export/datacontract.yaml")
     expected_dbt_model = """
 version: 2
 sources:
   - name: orders-unit-test
     description: The orders data contract  
     database: my-database
     schema: my-schema
```

### Comparing `datacontract-cli-0.9.8/tests/test_export_dbt_staging_sql.py` & `datacontract_cli-0.9.9/tests/test_export_dbt_staging_sql.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,25 +13,25 @@
 
 def test_cli():
     runner = CliRunner()
     result = runner.invoke(
         app,
         [
             "export",
-            "./examples/export/datacontract.yaml",
+            "./fixtures/export/datacontract.yaml",
             "--format",
             "dbt-staging-sql",
         ],
     )
     print(result.stdout)
     assert result.exit_code == 0
 
 
 def test_to_dbt_staging():
-    data_contract = DataContractSpecification.from_file("./examples/export/datacontract.yaml")
+    data_contract = DataContractSpecification.from_file("fixtures/export/datacontract.yaml")
     expected = """
 select 
     order_id,
     order_total,
     order_status
 from {{ source('orders-unit-test', 'orders') }}
 """
```

### Comparing `datacontract-cli-0.9.8/tests/test_export_jsonschema.py` & `datacontract_cli-0.9.9/tests/test_export_jsonschema.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,20 +11,20 @@
     DataContractSpecification
 
 logging.basicConfig(level=logging.DEBUG, force=True)
 
 
 def test_cli():
     runner = CliRunner()
-    result = runner.invoke(app, ["export", "./examples/local-json/datacontract.yaml", "--format", "jsonschema"])
+    result = runner.invoke(app, ["export", "./fixtures/local-json/datacontract.yaml", "--format", "jsonschema"])
     assert result.exit_code == 0
 
 
 def test_to_jsonschemas():
-    data_contract_file = "./examples/local-json/datacontract.yaml"
+    data_contract_file = "fixtures/local-json/datacontract.yaml"
     file_content = read_file(data_contract_file=data_contract_file)
     data_contract = DataContractSpecification.from_string(file_content)
     expected_json_schema = """{
   "$schema": "http://json-schema.org/draft-07/schema#",
   "type": "object",
   "properties": {
     "Statistik_Code": {
@@ -109,15 +109,15 @@
 
     result = to_jsonschemas(data_contract)
 
     assert result["verbraucherpreisindex"] == json.loads(expected_json_schema)
 
 
 def test_to_jsonschemas_complex():
-    data_contract_file = "./examples/s3-json-complex/datacontract.yaml"
+    data_contract_file = "fixtures/s3-json-complex/datacontract.yaml"
     file_content = read_file(data_contract_file=data_contract_file)
     data_contract = DataContractSpecification.from_string(file_content)
     expected_json_schema = """{
   "$schema": "http://json-schema.org/draft-07/schema#",
   "type": "object",
   "properties": {
       "specversion": {
```

### Comparing `datacontract-cli-0.9.8/tests/test_export_odcs.py` & `datacontract_cli-0.9.9/tests/test_export_odcs.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,20 +11,20 @@
     DataContractSpecification
 
 logging.basicConfig(level=logging.DEBUG, force=True)
 
 
 def test_cli():
     runner = CliRunner()
-    result = runner.invoke(app, ["export", "./examples/export/datacontract.yaml", "--format", "odcs"])
+    result = runner.invoke(app, ["export", "./fixtures/export/datacontract.yaml", "--format", "odcs"])
     assert result.exit_code == 0
 
 
 def test_to_odcs():
-    data_contract = DataContractSpecification.from_string(read_file("./examples/export/datacontract.yaml"))
+    data_contract = DataContractSpecification.from_string(read_file("fixtures/export/datacontract.yaml"))
     expected_odcs_model = """
 kind: DataContract
 apiVersion: 2.3.0
 uuid: orders-unit-test
 version: 1.0.0
 datasetDomain: checkout 
 quantumName: Orders Unit Test
```

### Comparing `datacontract-cli-0.9.8/tests/test_export_protobuf.py` & `datacontract_cli-0.9.9/tests/test_export_protobuf.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,20 +8,20 @@
     DataContractSpecification
 
 logging.basicConfig(level=logging.DEBUG, force=True)
 
 
 def test_cli():
     runner = CliRunner()
-    result = runner.invoke(app, ["export", "./examples/export/datacontract.yaml", "--format", "protobuf"])
+    result = runner.invoke(app, ["export", "./fixtures/export/datacontract.yaml", "--format", "protobuf"])
     assert result.exit_code == 0
 
 
 def test_to_protobuf():
-    data_contract = DataContractSpecification.from_file("./examples/export/datacontract.yaml")
+    data_contract = DataContractSpecification.from_file("fixtures/export/datacontract.yaml")
     expected_protobuf = """
 syntax = "proto3";
 
 /* The orders model */
 message Orders {
   string order_id = 1;
   /* The order_total field */
@@ -32,15 +32,15 @@
 
     result = to_protobuf(data_contract).strip()
 
     assert result == expected_protobuf
 
 
 def test_to_protobuf_nested():
-    data_contract = DataContractSpecification.from_file("./examples/export/datacontract_nested.yaml")
+    data_contract = DataContractSpecification.from_file("fixtures/export/datacontract_nested.yaml")
     expected_protobuf = """
 syntax = "proto3";
 
 /* The orders model */
 message Orders {
   string order_id = 1;
   /* The order_total field */
```

### Comparing `datacontract-cli-0.9.8/tests/test_export_pydantic.py` & `datacontract_cli-0.9.9/tests/test_export_pydantic.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,115 +1,122 @@
-import datacontract.model.data_contract_specification as spec
-import datacontract.export.pydantic_converter as conv
-from textwrap import dedent
 import ast
+from textwrap import dedent
+
+import datacontract.export.pydantic_converter as conv
+import datacontract.model.data_contract_specification as spec
 
 
 # These tests would be easier if AST nodes were comparable.
 # Current string comparisons are very brittle.
 def test_simple_model_export():
-    m = spec.Model(
-        fields={
-            "f": spec.Field(
-                type="string")})
+    m = spec.Model(fields={"f": spec.Field(type="string")})
     ast_class = conv.generate_model_class("Test", m)
-    assert ast.unparse(ast_class) == dedent(
-    """
+    assert (
+        ast.unparse(ast_class)
+        == dedent(
+            """
     class Test(pydantic.BaseModel):
         f: typing.Optional[str]
-    """).strip()
+    """
+        ).strip()
+    )
+
 
 def test_array_model_export():
-    m = spec.Model(
-        fields={
-            "f": spec.Field(
-                type="array",
-                items=spec.Field(
-                    type="string",
-                    required=True))})
+    m = spec.Model(fields={"f": spec.Field(type="array", items=spec.Field(type="string", required=True))})
     ast_class = conv.generate_model_class("Test", m)
-    assert ast.unparse(ast_class) == dedent(
-        """
+    assert (
+        ast.unparse(ast_class)
+        == dedent(
+            """
         class Test(pydantic.BaseModel):
             f: typing.Optional[list[str]]
-        """).strip()
+        """
+        ).strip()
+    )
+
 
 def test_object_model_export():
-    m = spec.Model(
-        fields={
-            "f": spec.Field(
-                type="object",
-                fields={
-                    "f1": spec.Field(
-                        type="string",
-                        required=True)})})
+    m = spec.Model(fields={"f": spec.Field(type="object", fields={"f1": spec.Field(type="string", required=True)})})
     ast_class = conv.generate_model_class("Test", m)
-    assert ast.unparse(ast_class) == dedent(
-        """
+    assert (
+        ast.unparse(ast_class)
+        == dedent(
+            """
         class Test(pydantic.BaseModel):
 
             class F(pydantic.BaseModel):
                 f1: str
             f: typing.Optional[F]
-        """).strip()
+        """
+        ).strip()
+    )
+
 
 def test_model_documentation_export():
     m = spec.Model(
         description="A test model",
         fields={
             "f": spec.Field(
-                type="object",
-                description="A test field",
-                fields={
-                    "f1": spec.Field(
-                        type="string",
-                        required=True)})})
+                type="object", description="A test field", fields={"f1": spec.Field(type="string", required=True)}
+            )
+        },
+    )
     ast_class = conv.generate_model_class("Test", m)
-    assert ast.unparse(ast_class) == dedent(
-        """
+    assert (
+        ast.unparse(ast_class)
+        == dedent(
+            """
         class Test(pydantic.BaseModel):
             \"""A test model\"""
 
             class F(pydantic.BaseModel):
                 \"""A test field\"""
                 f1: str
             f: typing.Optional[F]
-        """).strip()
+        """
+        ).strip()
+    )
+
 
 def test_model_field_description_export():
     m = spec.Model(
-    fields={
-        "f": spec.Field(
-            type="object",
-            fields={
-                "f1": spec.Field(
-                    type="string",
-                    description="A test field",
-                    required=True)})})
+        fields={
+            "f": spec.Field(
+                type="object", fields={"f1": spec.Field(type="string", description="A test field", required=True)}
+            )
+        }
+    )
     ast_class = conv.generate_model_class("Test", m)
-    assert ast.unparse(ast_class) == dedent(
-        """
+    assert (
+        ast.unparse(ast_class)
+        == dedent(
+            """
         class Test(pydantic.BaseModel):
 
             class F(pydantic.BaseModel):
                 f1: str
                 'A test field'
             f: typing.Optional[F]
-        """).strip()
+        """
+        ).strip()
+    )
+
 
 def test_model_description_export():
     m = spec.DataContractSpecification(
         info=spec.Info(description="Contract description"),
-        models={"test_model":
-                spec.Model(
-                    fields={
-                        "f": spec.Field(
-                            type="string")})})
+        models={"test_model": spec.Model(fields={"f": spec.Field(type="string")})},
+    )
     result = conv.to_pydantic_model_str(m)
-    assert result == dedent(
-        """
+    assert (
+        result
+        == dedent(
+            """
         import datetime, typing, pydantic
         'Contract description'
 
         class Test_model(pydantic.BaseModel):
             f: typing.Optional[str]
-        """).strip()
+        """
+        ).strip()
+    )
```

### Comparing `datacontract-cli-0.9.8/tests/test_export_rdf.py` & `datacontract_cli-0.9.9/tests/test_export_rdf.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,27 +13,27 @@
 
 logging.basicConfig(level=logging.DEBUG, force=True)
 
 
 def test_cli():
     runner = CliRunner()
     result = runner.invoke(
-        app, ["export", "./examples/export/rdf/datacontract.yaml", "--format", "rdf", "--rdf-base", "urn:acme:"]
+        app, ["export", "./fixtures/export/rdf/datacontract.yaml", "--format", "rdf", "--rdf-base", "urn:acme:"]
     )
     assert result.exit_code == 0
 
 
 def test_no_rdf_base():
     runner = CliRunner()
-    result = runner.invoke(app, ["export", "./examples/export/rdf/datacontract.yaml", "--format", "rdf"])
+    result = runner.invoke(app, ["export", "./fixtures/export/rdf/datacontract.yaml", "--format", "rdf"])
     assert result.exit_code == 0
 
 
 def test_to_rdf():
-    data_contract_file = "./examples/export/rdf/datacontract.yaml"
+    data_contract_file = "fixtures/export/rdf/datacontract.yaml"
     file_content = read_file(data_contract_file=data_contract_file)
     data_contract = DataContractSpecification.from_string(file_content)
     expected_rdf = """
 @prefix dc1: <https://datacontract.com/DataContractSpecification/0.9.2/> .
 @prefix dcx: <https://datacontract.com/DataContractSpecification/0.9.2/Extension/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
 
@@ -91,15 +91,15 @@
     iso_g1 = to_isomorphic(Graph().parse(data=g.serialize()))
     iso_result = to_isomorphic(Graph().parse(data=result.serialize()))
 
     assert iso_g1 == iso_result
 
 
 def test_to_rdf_complex():
-    data_contract_file = "./examples/export/rdf/datacontract-complex.yaml"
+    data_contract_file = "fixtures/export/rdf/datacontract-complex.yaml"
     file_content = read_file(data_contract_file=data_contract_file)
     data_contract = DataContractSpecification.from_string(file_content)
     expected_rdf = """
 @base <http://test.com/> .
 @prefix dc1: <https://datacontract.com/DataContractSpecification/0.9.2/> .
 @prefix dcx: <https://datacontract.com/DataContractSpecification/0.9.2/Extension/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
@@ -155,15 +155,15 @@
             dc1:usage \"\"\"Data can be used for reports, analytics and machine learning use cases. Order may be linked and joined by other tables
 \"\"\" ] .
 
 <production> a dc1:Server ;
     dcx:endpointUrl "__S3_ENDPOINT_URL__" ;
     dc1:delimiter "new_line" ;
     dc1:format "json" ;
-    dc1:location "s3://multiple-bucket/examples/s3-json-multiple-models/data/{model}/*.json" ;
+    dc1:location "s3://multiple-bucket/fixtures/s3-json-multiple-models/data/{model}/*.json" ;
     dc1:type "s3" .
 
 <line_items> a dc1:Model ;
     dc1:description "A single article that is part of an order." ;
     dc1:field [ a dc1:Field ;
             dc1:description "Primary key of the lines_item_id table" ;
             dc1:name "lines_item_id" ;
```

### Comparing `datacontract-cli-0.9.8/tests/test_export_sodacl.py` & `datacontract_cli-0.9.9/tests/test_export_sodacl.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,54 @@
+import pytest
 import yaml
 
 from datacontract.export.sodacl_converter import to_sodacl_yaml
+from datacontract.lint import resolve
 from datacontract.model.data_contract_specification import \
     DataContractSpecification
 
 
-def test_to_sodacl():
+@pytest.fixture
+def check_expected() -> str:
+    expected = """
+        checks for orders:
+          - schema:
+              name: Check that field order_id is present
+              fail:
+                when required column missing:
+                  - order_id
+          - schema:
+              name: Check that field order_id has type string
+              fail:
+                when wrong column type:
+                  order_id: string
+          - missing_count(order_id) = 0:
+              name: Check that required field order_id has no null values 
+          - schema:
+              name: Check that field processed_timestamp is present
+              fail:
+                when required column missing:
+                  - processed_timestamp
+          - schema:
+              name: Check that field processed_timestamp has type timestamp
+              fail:
+                when wrong column type:
+                  processed_timestamp: timestamp
+          - missing_count(processed_timestamp) = 0:
+              name: Check that required field processed_timestamp has no null values 
+          - freshness(processed_timestamp) < 1d
+          - row_count > 10
+        checks for line_items:
+          - row_count > 10:
+              name: Have at lease 10 line items
+        """
+    return expected
+
+
+def test_to_sodacl(check_expected: str):
     data_contract_specification_str = """
 dataContractSpecification: 0.9.1
 models:
   orders:
     description: test
     fields:
       order_id:
@@ -25,45 +64,23 @@
          - freshness(processed_timestamp) < 1d
          - row_count > 10
       checks for line_items:
          - row_count > 10:
              name: Have at lease 10 line items
     """
 
-    expected = """
-    checks for orders:
-      - schema:
-          name: Check that field order_id is present
-          fail:
-            when required column missing:
-              - order_id
-      - schema:
-          name: Check that field order_id has type string
-          fail:
-            when wrong column type:
-              order_id: string
-      - missing_count(order_id) = 0:
-          name: Check that required field order_id has no null values 
-      - schema:
-          name: Check that field processed_timestamp is present
-          fail:
-            when required column missing:
-              - processed_timestamp
-      - schema:
-          name: Check that field processed_timestamp has type timestamp
-          fail:
-            when wrong column type:
-              processed_timestamp: timestamp
-      - missing_count(processed_timestamp) = 0:
-          name: Check that required field processed_timestamp has no null values 
-      - freshness(processed_timestamp) < 1d
-      - row_count > 10
-    checks for line_items:
-      - row_count > 10:
-          name: Have at lease 10 line items
-    """
     data = yaml.safe_load(data_contract_specification_str)
     data_contract_specification = DataContractSpecification(**data)
 
     result = to_sodacl_yaml(data_contract_specification)
 
-    assert yaml.safe_load(result) == yaml.safe_load(expected)
+    assert yaml.safe_load(result) == yaml.safe_load(check_expected)
+
+
+def test_export_sodacl(check_expected: str):
+    data_contract_specification = resolve.resolve_data_contract_from_location(
+        "./fixtures/sodacl/datacontract.yaml", include_quality=True
+    )
+
+    result = to_sodacl_yaml(data_contract_specification)
+
+    assert yaml.safe_load(result) == yaml.safe_load(check_expected)
```

### Comparing `datacontract-cli-0.9.8/tests/test_export_sql.py` & `datacontract_cli-0.9.9/tests/test_export_sql_query.py`

 * *Files 24% similar despite different names*

```diff
@@ -6,65 +6,39 @@
 from datacontract.data_contract import DataContract
 
 logging.basicConfig(level=logging.DEBUG, force=True)
 
 
 def test_cli():
     runner = CliRunner()
-    result = runner.invoke(app, ["export", "./examples/postgres-export/datacontract.yaml", "--format", "sql"])
+    result = runner.invoke(app, ["export", "./fixtures/postgres-export/datacontract.yaml", "--format", "sql-query"])
     assert result.exit_code == 0
 
 
 def test_to_sql_ddl_postgres():
-    actual = DataContract(data_contract_file="./examples/postgres-export/datacontract.yaml").export("sql")
+    actual = DataContract(data_contract_file="fixtures/postgres-export/datacontract.yaml").export("sql-query")
     expected = """
 -- Data Contract: postgres
 -- SQL Dialect: postgres
-CREATE TABLE my_table (
-  field_one text not null,
-  field_two integer,
-  field_three timestamptz
-);
-""".strip()
-    assert actual == expected
+select
+    field_one,
+    field_two,
+    field_three
+from my_table
+"""
+    assert actual.strip() == expected.strip()
 
 
 def test_to_sql_ddl_snowflake():
-    actual = DataContract(data_contract_file="./examples/snowflake/datacontract.yaml").export("sql")
+    actual = DataContract(data_contract_file="fixtures/snowflake/datacontract.yaml").export("sql-query", model="orders")
     expected = """
 -- Data Contract: urn:datacontract:checkout:snowflake_orders_pii_v2
 -- SQL Dialect: snowflake
-CREATE TABLE orders (
-  ORDER_ID TEXT not null,
-  ORDER_TIMESTAMP TIMESTAMP_TZ not null,
-  ORDER_TOTAL NUMBER not null,
-  CUSTOMER_ID TEXT,
-  CUSTOMER_EMAIL_ADDRESS TEXT not null
-);
-CREATE TABLE line_items (
-  LINE_ITEM_ID TEXT not null,
-  ORDER_ID TEXT,
-  SKU TEXT
-);
-""".strip()
-    assert actual == expected
-
-
-def test_to_sql_ddl_databricks_unity_catalog():
-    actual = DataContract(data_contract_file="./examples/databricks-sql/datacontract.yaml").export("sql")
-    expected = """
--- Data Contract: urn:datacontract:checkout:orders-latest
--- SQL Dialect: databricks
-CREATE OR REPLACE TABLE datacontract_test_2.orders_latest.orders (
-  order_id STRING not null,
-  order_timestamp TIMESTAMP not null,
-  order_total BIGINT not null,
-  customer_id STRING,
-  customer_email_address STRING not null
-);
-CREATE OR REPLACE TABLE datacontract_test_2.orders_latest.line_items (
-  lines_item_id STRING not null,
-  order_id STRING,
-  sku STRING
-);
-""".strip()
-    assert actual == expected
+select
+    ORDER_ID,
+    ORDER_TIMESTAMP,
+    ORDER_TOTAL,
+    CUSTOMER_ID,
+    CUSTOMER_EMAIL_ADDRESS
+from orders
+"""
+    assert actual.strip() == expected.strip()
```

### Comparing `datacontract-cli-0.9.8/tests/test_export_sql_query.py` & `datacontract_cli-0.9.9/tests/test_import_sql.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,46 +1,58 @@
 import logging
 
+import yaml
 from typer.testing import CliRunner
 
 from datacontract.cli import app
 from datacontract.data_contract import DataContract
 
 logging.basicConfig(level=logging.DEBUG, force=True)
 
+datacontract = "fixtures/postgres/datacontract.yaml"
+sql_file_path = "fixtures/postgres/data/data.sql"
+
 
 def test_cli():
     runner = CliRunner()
-    result = runner.invoke(app, ["export", "./examples/postgres-export/datacontract.yaml", "--format", "sql-query"])
+    result = runner.invoke(
+        app,
+        [
+            "import",
+            "--format",
+            "sql",
+            "--source",
+            sql_file_path,
+        ],
+    )
     assert result.exit_code == 0
 
 
-def test_to_sql_ddl_postgres():
-    actual = DataContract(data_contract_file="./examples/postgres-export/datacontract.yaml").export("sql-query")
-    expected = """
--- Data Contract: postgres
--- SQL Dialect: postgres
-select
-    field_one,
-    field_two,
-    field_three
-from my_table
-"""
-    assert actual.strip() == expected.strip()
+def test_import_sql():
+    result = DataContract().import_from_source("sql", sql_file_path)
 
-
-def test_to_sql_ddl_snowflake():
-    actual = DataContract(data_contract_file="./examples/snowflake/datacontract.yaml").export(
-        "sql-query", model="orders"
-    )
     expected = """
--- Data Contract: urn:datacontract:checkout:snowflake_orders_pii_v2
--- SQL Dialect: snowflake
-select
-    ORDER_ID,
-    ORDER_TIMESTAMP,
-    ORDER_TOTAL,
-    CUSTOMER_ID,
-    CUSTOMER_EMAIL_ADDRESS
-from orders
-"""
-    assert actual.strip() == expected.strip()
+dataContractSpecification: 0.9.3
+id: my-data-contract-id
+info:
+  title: My Data Contract
+  version: 0.0.1
+models:
+  my_table:
+    type: table
+    fields:
+      field_one:
+        type: varchar
+        required: true
+        primary: true
+        unique: true
+        maxLength: 10
+      field_two:
+        type: integer
+        required: true
+      field_three:
+        type: timestamp
+    """
+    print("Result", result.to_yaml())
+    assert yaml.safe_load(result.to_yaml()) == yaml.safe_load(expected)
+    # Disable linters so we don't get "missing description" warnings
+    assert DataContract(data_contract_str=expected).lint(enabled_linters=set()).has_passed()
```

### Comparing `datacontract-cli-0.9.8/tests/test_export_terraform.py` & `datacontract_cli-0.9.9/tests/test_export_terraform.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,20 +8,20 @@
     DataContractSpecification
 
 logging.basicConfig(level=logging.DEBUG, force=True)
 
 
 def test_cli():
     runner = CliRunner()
-    result = runner.invoke(app, ["export", "./examples/export/datacontract_s3.yaml", "--format", "terraform"])
+    result = runner.invoke(app, ["export", "./fixtures/export/datacontract_s3.yaml", "--format", "terraform"])
     assert result.exit_code == 0
 
 
 def test_to_terraform():
-    data_contract = DataContractSpecification.from_file("./examples/export/datacontract_s3.yaml")
+    data_contract = DataContractSpecification.from_file("fixtures/export/datacontract_s3.yaml")
     expected_terraform_file = """
 resource "aws_s3_bucket" "orders-unit-test_production" {
   bucket = "datacontract-example-orders-latest"
 
   tags = {
     Name         = "Orders Unit Test"
     DataContract = "orders-unit-test"
```

### Comparing `datacontract-cli-0.9.8/tests/test_field_constraint_linter.py` & `datacontract_cli-0.9.9/tests/test_field_constraint_linter.py`

 * *Files identical despite different names*

### Comparing `datacontract-cli-0.9.8/tests/test_field_pattern_linter.py` & `datacontract_cli-0.9.9/tests/test_field_pattern_linter.py`

 * *Files identical despite different names*

### Comparing `datacontract-cli-0.9.8/tests/test_field_reference_linter.py` & `datacontract_cli-0.9.9/tests/test_field_reference_linter.py`

 * *Files identical despite different names*

### Comparing `datacontract-cli-0.9.8/tests/test_integration_opentelemetry.py` & `datacontract_cli-0.9.9/tests/test_integration_opentelemetry.py`

 * *Files identical despite different names*

### Comparing `datacontract-cli-0.9.8/tests/test_lint.py` & `datacontract_cli-0.9.9/tests/test_lint.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,59 +7,59 @@
 
 logging.basicConfig(level=logging.INFO, force=True)
 
 runner = CliRunner()
 
 
 def test_lint_valid_data_contract():
-    data_contract_file = "examples/lint/valid_datacontract.yaml"
+    data_contract_file = "fixtures/lint/valid_datacontract.yaml"
     data_contract = DataContract(data_contract_file=data_contract_file)
 
     run = data_contract.lint()
     assert run.result == "passed"
 
 
 def test_lint_invalid_data_contract():
-    data_contract_file = "examples/lint/invalid_datacontract.yaml"
+    data_contract_file = "fixtures/lint/invalid_datacontract.yaml"
     data_contract = DataContract(data_contract_file=data_contract_file)
 
     run = data_contract.lint()
 
     assert run.result == "failed"
 
 
 def test_lint_cli_valid():
-    data_contract_file = "examples/lint/valid_datacontract.yaml"
-    expected_output = "🟢 data contract is valid. Run 9 checks."
+    data_contract_file = "fixtures/lint/valid_datacontract.yaml"
+    expected_output = "🟢 data contract is valid. Run 8 checks."
 
     result = runner.invoke(app, ["lint", data_contract_file])
 
     assert result.exit_code == 0
     assert expected_output in result.stdout
 
 
 def test_lint_cli_invalid():
-    data_contract_file = "examples/lint/invalid_datacontract.yaml"
+    data_contract_file = "fixtures/lint/invalid_datacontract.yaml"
     expected_output = (
         "🔴 data contract is invalid, found the following errors:\n1) data must contain ['id'] properties\n"
     )
 
     result = runner.invoke(app, ["lint", data_contract_file])
 
     assert result.exit_code == 1
     assert expected_output in result.stdout
 
 
 def test_lint_custom_schema():
-    data_contract_file = "examples/lint/custom_datacontract.yaml"
-    schema_file = "examples/lint/custom_datacontract.schema.json"
+    data_contract_file = "fixtures/lint/custom_datacontract.yaml"
+    schema_file = "fixtures/lint/custom_datacontract.schema.json"
     data_contract = DataContract(data_contract_file=data_contract_file, schema_location=schema_file)
 
     run = data_contract.lint()
     assert run.result == "passed"
 
 
 def test_lint_with_references():
     data_contract = DataContract(
-        data_contract_file="examples/lint/valid_datacontract_references.yaml", inline_definitions=True
+        data_contract_file="fixtures/lint/valid_datacontract_references.yaml", inline_definitions=True
     )
     DataContractSpecification.model_validate(data_contract.get_data_contract_specification())
```

### Comparing `datacontract-cli-0.9.8/tests/test_notice_period_linter.py` & `datacontract_cli-0.9.9/tests/test_notice_period_linter.py`

 * *Files identical despite different names*

### Comparing `datacontract-cli-0.9.8/tests/test_primary_field_linter.py` & `datacontract_cli-0.9.9/datacontract/export/html_export.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,38 +1,46 @@
-import datacontract.model.data_contract_specification as spec
-from datacontract.lint.linters.primary_field_linter import PrimaryFieldUniqueRequired
-from datacontract.model.run import Check
+import yaml
+from jinja2 import Environment, PackageLoader, select_autoescape
 
+from datacontract.model.data_contract_specification import \
+    DataContractSpecification
 
-def construct_error_check(msg: str) -> Check:
-    return Check(
-        type="lint",
-        name="Linter 'Model primary fields unique and required'",
-        result="warning",
-        engine="datacontract",
-        reason=msg,
-    )
-
-
-success_check = Check(
-    type="lint", name="Linter 'Model primary fields unique and required'", result="passed", engine="datacontract"
-)
 
-linter = PrimaryFieldUniqueRequired()
-
-
-def test_correct_model():
-    specification = spec.DataContractSpecification(
-        models={"test_model": spec.Model(fields={"test_field": spec.Field(primary=True, unique=True, required=True)})}
+def to_html(data_contract_spec: DataContractSpecification) -> str:
+    # Load templates from templates folder
+    package_loader = PackageLoader("datacontract", "templates")
+    env = Environment(
+        loader=package_loader,
+        autoescape=select_autoescape(
+            enabled_extensions=("html", "xml"),
+            default_for_string=True,
+        ),
     )
-    assert linter.lint(specification) == [success_check]
 
+    # Load the required template
+    template = env.get_template("datacontract.html")
 
-def test_incorrect_model():
-    specification = spec.DataContractSpecification(
-        models={"test_model": spec.Model(fields={"test_field": spec.Field(primary=True)})}
+    if data_contract_spec.quality is not None and isinstance(data_contract_spec.quality.specification, str):
+        quality_specification = data_contract_spec.quality.specification
+    elif data_contract_spec.quality is not None and isinstance(data_contract_spec.quality.specification, object):
+        if data_contract_spec.quality.type == "great-expectations":
+            quality_specification = yaml.dump(
+                data_contract_spec.quality.specification, sort_keys=False, default_style="|"
+            )
+        else:
+            quality_specification = yaml.dump(data_contract_spec.quality.specification, sort_keys=False)
+    else:
+        quality_specification = None
+
+    style_content, _, _ = package_loader.get_source(env, "style/output.css")
+
+    datacontract_yaml = data_contract_spec.to_yaml()
+
+    # Render the template with necessary data
+    html_string = template.render(
+        datacontract=data_contract_spec,
+        quality_specification=quality_specification,
+        style=style_content,
+        datacontract_yaml=datacontract_yaml,
     )
-    assert linter.lint(specification) == [
-        construct_error_check(
-            "Field 'test_field' in model 'test_model' is marked as " "primary, but not as unique and required."
-        )
-    ]
+
+    return html_string
```

### Comparing `datacontract-cli-0.9.8/tests/test_quality_schema_linter.py` & `datacontract_cli-0.9.9/tests/test_quality_schema_linter.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,15 +11,15 @@
         engine="datacontract",
         reason=msg,
     )
 
 
 success_check = Check(type="lint", name="Linter 'Quality check(s) use model'", result="passed", engine="datacontract")
 
-data_contract_file = "examples/lint/datacontract_quality_schema.yaml"
+data_contract_file = "fixtures/lint/datacontract_quality_schema.yaml"
 
 
 def test_lint_correct_sodacl():
     base_contract_sodacl = resolve.resolve_data_contract_from_location(data_contract_file)
     result = QualityUsesSchemaLinter().lint(base_contract_sodacl)
     assert result == [success_check]
```

### Comparing `datacontract-cli-0.9.8/tests/test_schema.py` & `datacontract_cli-0.9.9/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `datacontract-cli-0.9.8/tests/test_web.py` & `datacontract_cli-0.9.9/tests/test_web.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 
 from datacontract.web import app
 
 client = TestClient(app)
 
 
 def test_lint():
-    with open("examples/lint/valid_datacontract.yaml", "rb") as f:
+    with open("fixtures/lint/valid_datacontract.yaml", "rb") as f:
         response = client.post(
             url="/lint", files={"file": ("datacontract.yaml", f, "application/yaml")}, params={"linters": "none"}
         )
         assert response.status_code == 200
         print(response.json())
         assert response.json()["result"] == "passed"
-        assert len(response.json()["checks"]) == 9
+        assert len(response.json()["checks"]) == 8
         assert all([check["result"] == "passed" for check in response.json()["checks"]])
```

