# Comparing `tmp/a3m-0.7.8.tar.gz` & `tmp/a3m-0.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "a3m-0.7.8.tar", last modified: Mon Feb 12 10:13:32 2024, max compression
+gzip compressed data, was "a3m-0.7.9.tar", last modified: Mon Feb 12 20:11:21 2024, max compression
```

## Comparing `a3m-0.7.8.tar` & `a3m-0.7.9.tar`

### file list

```diff
@@ -1,183 +1,183 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 10:13:32.845698 a3m-0.7.8/
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-02-12 10:13:13.000000 a3m-0.7.8/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (127)    34519 2024-02-12 10:13:13.000000 a3m-0.7.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-02-12 10:13:13.000000 a3m-0.7.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    43994 2024-02-12 10:13:32.845698 a3m-0.7.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-02-12 10:13:13.000000 a3m-0.7.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-02-12 10:13:13.000000 a3m-0.7.8/TRADEMARK
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 10:13:32.817698 a3m-0.7.8/a3m/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-02-12 10:13:13.000000 a3m-0.7.8/a3m/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 10:13:32.809698 a3m-0.7.8/a3m/api/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 10:13:32.809698 a3m-0.7.8/a3m/api/transferservice/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 10:13:32.817698 a3m-0.7.8/a3m/api/transferservice/v1beta1/
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-02-12 10:13:13.000000 a3m-0.7.8/a3m/api/transferservice/v1beta1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7475 2024-02-12 10:13:13.000000 a3m-0.7.8/a3m/api/transferservice/v1beta1/request_response_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    16896 2024-02-12 10:13:13.000000 a3m-0.7.8/a3m/api/transferservice/v1beta1/request_response_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-02-12 10:13:13.000000 a3m-0.7.8/a3m/api/transferservice/v1beta1/request_response_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2598 2024-02-12 10:13:13.000000 a3m-0.7.8/a3m/api/transferservice/v1beta1/service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-02-12 10:13:13.000000 a3m-0.7.8/a3m/api/transferservice/v1beta1/service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8697 2024-02-12 10:13:13.000000 a3m-0.7.8/a3m/api/transferservice/v1beta1/service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     6147 2024-02-12 10:13:13.000000 a3m-0.7.8/a3m/appconfig.py
--rw-r--r--   0 runner    (1001) docker     (127)     8060 2024-02-12 10:13:13.000000 a3m-0.7.8/a3m/archivematicaFunctions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 10:13:32.817698 a3m-0.7.8/a3m/assets/
--rw-r--r--   0 runner    (1001) docker     (127)     4969 2024-02-12 10:13:13.000000 a3m-0.7.8/a3m/assets/workflow-schema-v1.json
--rw-r--r--   0 runner    (1001) docker     (127)   102093 2024-02-12 10:13:13.000000 a3m-0.7.8/a3m/assets/workflow.json
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-02-12 10:13:13.000000 a3m-0.7.8/a3m/bag.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 10:13:32.817698 a3m-0.7.8/a3m/cli/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-02-12 10:13:13.000000 a3m-0.7.8/a3m/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 10:13:32.817698 a3m-0.7.8/a3m/cli/client/
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-02-12 10:13:13.000000 a3m-0.7.8/a3m/cli/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6195 2024-02-12 10:13:13.000000 a3m-0.7.8/a3m/cli/client/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-02-12 10:13:13.000000 a3m-0.7.8/a3m/cli/client/wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-02-12 10:13:13.000000 a3m-0.7.8/a3m/cli/common.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 10:13:32.817698 a3m-0.7.8/a3m/cli/server/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-02-12 10:13:13.000000 a3m-0.7.8/a3m/cli/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-02-12 10:13:13.000000 a3m-0.7.8/a3m/cli/server/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 10:13:32.821698 a3m-0.7.8/a3m/client/
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-02-12 10:13:13.000000 a3m-0.7.8/a3m/client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 10:13:32.813698 a3m-0.7.8/a3m/client/assets/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 10:13:32.821698 a3m-0.7.8/a3m/client/assets/README/
--rw-r--r--   0 runner    (1001) docker     (127)     7246 2024-02-12 10:13:13.000000 a3m-0.7.8/a3m/client/assets/README/README.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 10:13:32.821698 a3m-0.7.8/a3m/client/assets/catalog/
--rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-02-12 10:13:13.000000 a3m-0.7.8/a3m/client/assets/catalog/catalog.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 10:13:32.821698 a3m-0.7.8/a3m/client/assets/mets/
--rw-r--r--   0 runner    (1001) docker     (127)   136472 2024-02-12 10:13:13.000000 a3m-0.7.8/a3m/client/assets/mets/mets.xsd
--rw-r--r--   0 runner    (1001) docker     (127)     3180 2024-02-12 10:13:13.000000 a3m-0.7.8/a3m/client/assets/mets/xlink.xsd
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 10:13:32.821698 a3m-0.7.8/a3m/client/assets/mods/
--rw-r--r--   0 runner    (1001) docker     (127)    61831 2024-02-12 10:13:13.000000 a3m-0.7.8/a3m/client/assets/mods/mods.xsd
--rw-r--r--   0 runner    (1001) docker     (127)     5840 2024-02-12 10:13:13.000000 a3m-0.7.8/a3m/client/assets/mods/xml.xsd
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 10:13:32.821698 a3m-0.7.8/a3m/client/assets/premis/
--rw-r--r--   0 runner    (1001) docker     (127)    65130 2024-02-12 10:13:13.000000 a3m-0.7.8/a3m/client/assets/premis/premis-v2-2.xsd
--rw-r--r--   0 runner    (1001) docker     (127)    52845 2024-02-12 10:13:13.000000 a3m-0.7.8/a3m/client/assets/premis/premis.xsd
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 10:13:32.833698 a3m-0.7.8/a3m/client/clientScripts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 10:13:13.000000 a3m-0.7.8/a3m/client/clientScripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4997 2024-02-12 10:13:13.000000 a3m-0.7.8/a3m/client/clientScripts/a3m_download_transfer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-02-12 10:13:13.000000 a3m-0.7.8/a3m/client/clientScripts/a3m_store_aip.py
--rw-r--r--   0 runner    (1001) docker     (127)     4498 2024-02-12 10:13:13.000000 a3m-0.7.8/a3m/client/clientScripts/archivematicaCreateMETSMetadataCSV.py
--rw-r--r--   0 runner    (1001) docker     (127)    15696 2024-02-12 10:13:13.000000 a3m-0.7.8/a3m/client/clientScripts/archivematicaCreateMETSRights.py
--rw-r--r--   0 runner    (1001) docker     (127)     6452 2024-02-12 10:13:13.000000 a3m-0.7.8/a3m/client/clientScripts/assign_file_uuids.py
--rw-r--r--   0 runner    (1001) docker     (127)     4242 2024-02-12 10:13:13.000000 a3m-0.7.8/a3m/client/clientScripts/assign_uuids_to_directories.py
--rw-r--r--   0 runner    (1001) docker     (127)     3409 2024-02-12 10:13:13.000000 a3m-0.7.8/a3m/client/clientScripts/bag_with_empty_directories.py
--rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-02-12 10:13:13.000000 a3m-0.7.8/a3m/client/clientScripts/change_names.py
--rw-r--r--   0 runner    (1001) docker     (127)     9437 2024-02-12 10:13:13.000000 a3m-0.7.8/a3m/client/clientScripts/change_object_names.py
--rw-r--r--   0 runner    (1001) docker     (127)     4702 2024-02-12 10:13:13.000000 a3m-0.7.8/a3m/client/clientScripts/characterize_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     4047 2024-02-12 10:13:13.000000 a3m-0.7.8/a3m/client/clientScripts/check_for_service_directory.py
--rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-02-12 10:13:13.000000 a3m-0.7.8/a3m/client/clientScripts/check_for_submission_documentation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-02-12 10:13:13.000000 a3m-0.7.8/a3m/client/clientScripts/check_transfer_directory_for_objects.py
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-02-12 10:13:13.000000 a3m-0.7.8/a3m/client/clientScripts/cmd_chmod.py
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-02-12 10:13:13.000000 a3m-0.7.8/a3m/client/clientScripts/cmd_cp.py
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-02-12 10:13:13.000000 a3m-0.7.8/a3m/client/clientScripts/cmd_mkdir.py
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-02-12 10:13:13.000000 a3m-0.7.8/a3m/client/clientScripts/cmd_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-02-12 10:13:13.000000 a3m-0.7.8/a3m/client/clientScripts/cmd_tree.py
--rw-r--r--   0 runner    (1001) docker     (127)     7088 2024-02-12 10:13:13.000000 a3m-0.7.8/a3m/client/clientScripts/compress_aip.py
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-02-12 10:13:13.000000 a3m-0.7.8/a3m/client/clientScripts/copy_submission_docs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2434 2024-02-12 10:13:13.000000 a3m-0.7.8/a3m/client/clientScripts/copy_transfer_submission_documentation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4208 2024-02-12 10:13:13.000000 a3m-0.7.8/a3m/client/clientScripts/copy_transfers_metadata_and_logs.py
--rw-r--r--   0 runner    (1001) docker     (127)    59226 2024-02-12 10:13:13.000000 a3m-0.7.8/a3m/client/clientScripts/create_mets_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3948 2024-02-12 10:13:13.000000 a3m-0.7.8/a3m/client/clientScripts/create_sip_from_transfer_objects.py
--rw-r--r--   0 runner    (1001) docker     (127)     1947 2024-02-12 10:13:13.000000 a3m-0.7.8/a3m/client/clientScripts/create_transfer_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-02-12 10:13:13.000000 a3m-0.7.8/a3m/client/clientScripts/examine_contents.py
--rw-r--r--   0 runner    (1001) docker     (127)    10123 2024-02-12 10:13:13.000000 a3m-0.7.8/a3m/client/clientScripts/extract_contents.py
--rw-r--r--   0 runner    (1001) docker     (127)      659 2024-02-12 10:13:13.000000 a3m-0.7.8/a3m/client/clientScripts/failed_sip_cleanup.py
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-02-12 10:13:13.000000 a3m-0.7.8/a3m/client/clientScripts/failed_transfer_cleanup.py
--rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-02-12 10:13:13.000000 a3m-0.7.8/a3m/client/clientScripts/has_packages.py
--rw-r--r--   0 runner    (1001) docker     (127)     3843 2024-02-12 10:13:13.000000 a3m-0.7.8/a3m/client/clientScripts/identify_file_format.py
--rw-r--r--   0 runner    (1001) docker     (127)     4476 2024-02-12 10:13:13.000000 a3m-0.7.8/a3m/client/clientScripts/json_metadata_to_csv.py
--rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-02-12 10:13:13.000000 a3m-0.7.8/a3m/client/clientScripts/load_dublin_core.py
--rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-02-12 10:13:13.000000 a3m-0.7.8/a3m/client/clientScripts/load_labels_from_csv.py
--rw-r--r--   0 runner    (1001) docker     (127)    29374 2024-02-12 10:13:13.000000 a3m-0.7.8/a3m/client/clientScripts/load_premis_events_from_xml.py
--rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-02-12 10:13:13.000000 a3m-0.7.8/a3m/client/clientScripts/manual_normalization_check_for_manual_normalization_directory.py
--rw-r--r--   0 runner    (1001) docker     (127)     7291 2024-02-12 10:13:13.000000 a3m-0.7.8/a3m/client/clientScripts/manual_normalization_create_metadata_and_restructure.py
--rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-02-12 10:13:13.000000 a3m-0.7.8/a3m/client/clientScripts/manual_normalization_identify_files_included.py
--rw-r--r--   0 runner    (1001) docker     (127)     2458 2024-02-12 10:13:13.000000 a3m-0.7.8/a3m/client/clientScripts/manual_normalization_remove_mn_directories.py
--rw-r--r--   0 runner    (1001) docker     (127)     3317 2024-02-12 10:13:13.000000 a3m-0.7.8/a3m/client/clientScripts/move_or_merge.py
--rw-r--r--   0 runner    (1001) docker     (127)     2065 2024-02-12 10:13:13.000000 a3m-0.7.8/a3m/client/clientScripts/move_sip.py
--rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-02-12 10:13:13.000000 a3m-0.7.8/a3m/client/clientScripts/move_transfer.py
--rw-r--r--   0 runner    (1001) docker     (127)    18485 2024-02-12 10:13:13.000000 a3m-0.7.8/a3m/client/clientScripts/normalize.py
--rw-r--r--   0 runner    (1001) docker     (127)    18843 2024-02-12 10:13:13.000000 a3m-0.7.8/a3m/client/clientScripts/policy_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-02-12 10:13:13.000000 a3m-0.7.8/a3m/client/clientScripts/remove_directories.py
--rw-r--r--   0 runner    (1001) docker     (127)     1922 2024-02-12 10:13:13.000000 a3m-0.7.8/a3m/client/clientScripts/remove_files_without_premis_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-02-12 10:13:13.000000 a3m-0.7.8/a3m/client/clientScripts/remove_hidden_files_and_directories.py
--rw-r--r--   0 runner    (1001) docker     (127)     1590 2024-02-12 10:13:13.000000 a3m-0.7.8/a3m/client/clientScripts/remove_unneeded_files.py
--rw-r--r--   0 runner    (1001) docker     (127)     2180 2024-02-12 10:13:13.000000 a3m-0.7.8/a3m/client/clientScripts/restructure_for_compliance.py
--rw-r--r--   0 runner    (1001) docker     (127)    16354 2024-02-12 10:13:13.000000 a3m-0.7.8/a3m/client/clientScripts/rights_from_csv.py
--rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-02-12 10:13:13.000000 a3m-0.7.8/a3m/client/clientScripts/save_dublin_core.py
--rw-r--r--   0 runner    (1001) docker     (127)     2474 2024-02-12 10:13:13.000000 a3m-0.7.8/a3m/client/clientScripts/store_file_modification_dates.py
--rw-r--r--   0 runner    (1001) docker     (127)     4910 2024-02-12 10:13:13.000000 a3m-0.7.8/a3m/client/clientScripts/transcribe_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     4581 2024-02-12 10:13:13.000000 a3m-0.7.8/a3m/client/clientScripts/update_size_and_checksum.py
--rw-r--r--   0 runner    (1001) docker     (127)    12524 2024-02-12 10:13:13.000000 a3m-0.7.8/a3m/client/clientScripts/validate_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     8663 2024-02-12 10:13:13.000000 a3m-0.7.8/a3m/client/clientScripts/verify_aip.py
--rw-r--r--   0 runner    (1001) docker     (127)    10984 2024-02-12 10:13:13.000000 a3m-0.7.8/a3m/client/clientScripts/verify_checksum.py
--rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-02-12 10:13:13.000000 a3m-0.7.8/a3m/client/clientScripts/verify_mets.py
--rw-r--r--   0 runner    (1001) docker     (127)     2589 2024-02-12 10:13:13.000000 a3m-0.7.8/a3m/client/clientScripts/verify_sip_compliance.py
--rw-r--r--   0 runner    (1001) docker     (127)     2478 2024-02-12 10:13:13.000000 a3m-0.7.8/a3m/client/clientScripts/verify_transfer_compliance.py
--rw-r--r--   0 runner    (1001) docker     (127)     3709 2024-02-12 10:13:13.000000 a3m-0.7.8/a3m/client/job.py
--rw-r--r--   0 runner    (1001) docker     (127)     8354 2024-02-12 10:13:13.000000 a3m-0.7.8/a3m/client/mcp.py
--rw-r--r--   0 runner    (1001) docker     (127)     7672 2024-02-12 10:13:13.000000 a3m-0.7.8/a3m/client/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     1811 2024-02-12 10:13:13.000000 a3m-0.7.8/a3m/common_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     7351 2024-02-12 10:13:13.000000 a3m-0.7.8/a3m/countryCodes.py
--rw-r--r--   0 runner    (1001) docker     (127)     9571 2024-02-12 10:13:13.000000 a3m-0.7.8/a3m/databaseFunctions.py
--rw-r--r--   0 runner    (1001) docker     (127)     8634 2024-02-12 10:13:13.000000 a3m-0.7.8/a3m/dicts.py
--rw-r--r--   0 runner    (1001) docker     (127)    10094 2024-02-12 10:13:13.000000 a3m-0.7.8/a3m/executeOrRunSubProcess.py
--rw-r--r--   0 runner    (1001) docker     (127)     8130 2024-02-12 10:13:13.000000 a3m-0.7.8/a3m/fileOperations.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 10:13:32.833698 a3m-0.7.8/a3m/fpr/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 10:13:13.000000 a3m-0.7.8/a3m/fpr/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 10:13:32.833698 a3m-0.7.8/a3m/fpr/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 10:13:13.000000 a3m-0.7.8/a3m/fpr/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)  2341782 2024-02-12 10:13:13.000000 a3m-0.7.8/a3m/fpr/migrations/initial-data.json
--rw-r--r--   0 runner    (1001) docker     (127)    18206 2024-02-12 10:13:13.000000 a3m-0.7.8/a3m/fpr/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 10:13:32.837698 a3m-0.7.8/a3m/main/
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-02-12 10:13:13.000000 a3m-0.7.8/a3m/main/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-02-12 10:13:13.000000 a3m-0.7.8/a3m/main/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 10:13:32.837698 a3m-0.7.8/a3m/main/management/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 10:13:13.000000 a3m-0.7.8/a3m/main/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 10:13:32.837698 a3m-0.7.8/a3m/main/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)    63688 2024-02-12 10:13:13.000000 a3m-0.7.8/a3m/main/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-02-12 10:13:13.000000 a3m-0.7.8/a3m/main/migrations/0002_initial_data.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 10:13:13.000000 a3m-0.7.8/a3m/main/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5999 2024-02-12 10:13:13.000000 a3m-0.7.8/a3m/main/migrations/initial-data.json
--rw-r--r--   0 runner    (1001) docker     (127)    47453 2024-02-12 10:13:13.000000 a3m-0.7.8/a3m/main/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      655 2024-02-12 10:13:13.000000 a3m-0.7.8/a3m/namespaces.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 10:13:32.841698 a3m-0.7.8/a3m/server/
--rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-02-12 10:13:13.000000 a3m-0.7.8/a3m/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6652 2024-02-12 10:13:13.000000 a3m-0.7.8/a3m/server/db.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 10:13:32.841698 a3m-0.7.8/a3m/server/jobs/
--rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-02-12 10:13:13.000000 a3m-0.7.8/a3m/server/jobs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2851 2024-02-12 10:13:13.000000 a3m-0.7.8/a3m/server/jobs/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3888 2024-02-12 10:13:13.000000 a3m-0.7.8/a3m/server/jobs/chain.py
--rw-r--r--   0 runner    (1001) docker     (127)     6815 2024-02-12 10:13:13.000000 a3m-0.7.8/a3m/server/jobs/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-02-12 10:13:13.000000 a3m-0.7.8/a3m/server/jobs/decisions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3937 2024-02-12 10:13:13.000000 a3m-0.7.8/a3m/server/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    16191 2024-02-12 10:13:13.000000 a3m-0.7.8/a3m/server/packages.py
--rw-r--r--   0 runner    (1001) docker     (127)      794 2024-02-12 10:13:13.000000 a3m-0.7.8/a3m/server/processing.py
--rw-r--r--   0 runner    (1001) docker     (127)    10885 2024-02-12 10:13:13.000000 a3m-0.7.8/a3m/server/queues.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 10:13:32.841698 a3m-0.7.8/a3m/server/rpc/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-02-12 10:13:13.000000 a3m-0.7.8/a3m/server/rpc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3146 2024-02-12 10:13:13.000000 a3m-0.7.8/a3m/server/rpc/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     7066 2024-02-12 10:13:13.000000 a3m-0.7.8/a3m/server/runner.py
--rw-r--r--   0 runner    (1001) docker     (127)      969 2024-02-12 10:13:13.000000 a3m-0.7.8/a3m/server/shared_dirs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 10:13:32.841698 a3m-0.7.8/a3m/server/tasks/
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-02-12 10:13:13.000000 a3m-0.7.8/a3m/server/tasks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 10:13:32.841698 a3m-0.7.8/a3m/server/tasks/backends/
--rw-r--r--   0 runner    (1001) docker     (127)      715 2024-02-12 10:13:13.000000 a3m-0.7.8/a3m/server/tasks/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-02-12 10:13:13.000000 a3m-0.7.8/a3m/server/tasks/backends/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5559 2024-02-12 10:13:13.000000 a3m-0.7.8/a3m/server/tasks/backends/pool_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     3583 2024-02-12 10:13:13.000000 a3m-0.7.8/a3m/server/tasks/task.py
--rw-r--r--   0 runner    (1001) docker     (127)     3359 2024-02-12 10:13:13.000000 a3m-0.7.8/a3m/server/transfer_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     2121 2024-02-12 10:13:13.000000 a3m-0.7.8/a3m/server/translation.py
--rw-r--r--   0 runner    (1001) docker     (127)     6167 2024-02-12 10:13:13.000000 a3m-0.7.8/a3m/server/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 10:13:32.841698 a3m-0.7.8/a3m/settings/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 10:13:13.000000 a3m-0.7.8/a3m/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9645 2024-02-12 10:13:13.000000 a3m-0.7.8/a3m/settings/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-02-12 10:13:13.000000 a3m-0.7.8/a3m/settings/test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 10:13:32.841698 a3m-0.7.8/a3m.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    43994 2024-02-12 10:13:32.000000 a3m-0.7.8/a3m.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5531 2024-02-12 10:13:32.000000 a3m-0.7.8/a3m.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-12 10:13:32.000000 a3m-0.7.8/a3m.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-02-12 10:13:32.000000 a3m-0.7.8/a3m.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      557 2024-02-12 10:13:32.000000 a3m-0.7.8/a3m.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-02-12 10:13:32.000000 a3m-0.7.8/a3m.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5084 2024-02-12 10:13:13.000000 a3m-0.7.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-12 10:13:32.845698 a3m-0.7.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 10:13:32.841698 a3m-0.7.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3142 2024-02-12 10:13:13.000000 a3m-0.7.8/tests/test_registry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 20:11:21.854666 a3m-0.7.9/
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-02-12 20:11:03.000000 a3m-0.7.9/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (127)    34519 2024-02-12 20:11:03.000000 a3m-0.7.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-02-12 20:11:03.000000 a3m-0.7.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    43994 2024-02-12 20:11:21.854666 a3m-0.7.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-02-12 20:11:03.000000 a3m-0.7.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-02-12 20:11:03.000000 a3m-0.7.9/TRADEMARK
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 20:11:21.826665 a3m-0.7.9/a3m/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-02-12 20:11:03.000000 a3m-0.7.9/a3m/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 20:11:21.818666 a3m-0.7.9/a3m/api/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 20:11:21.818666 a3m-0.7.9/a3m/api/transferservice/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 20:11:21.826665 a3m-0.7.9/a3m/api/transferservice/v1beta1/
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-02-12 20:11:03.000000 a3m-0.7.9/a3m/api/transferservice/v1beta1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7475 2024-02-12 20:11:03.000000 a3m-0.7.9/a3m/api/transferservice/v1beta1/request_response_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16896 2024-02-12 20:11:03.000000 a3m-0.7.9/a3m/api/transferservice/v1beta1/request_response_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-02-12 20:11:03.000000 a3m-0.7.9/a3m/api/transferservice/v1beta1/request_response_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2598 2024-02-12 20:11:03.000000 a3m-0.7.9/a3m/api/transferservice/v1beta1/service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-02-12 20:11:03.000000 a3m-0.7.9/a3m/api/transferservice/v1beta1/service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8697 2024-02-12 20:11:03.000000 a3m-0.7.9/a3m/api/transferservice/v1beta1/service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6147 2024-02-12 20:11:03.000000 a3m-0.7.9/a3m/appconfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8060 2024-02-12 20:11:03.000000 a3m-0.7.9/a3m/archivematicaFunctions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 20:11:21.826665 a3m-0.7.9/a3m/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)     4969 2024-02-12 20:11:03.000000 a3m-0.7.9/a3m/assets/workflow-schema-v1.json
+-rw-r--r--   0 runner    (1001) docker     (127)   102093 2024-02-12 20:11:03.000000 a3m-0.7.9/a3m/assets/workflow.json
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-02-12 20:11:03.000000 a3m-0.7.9/a3m/bag.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 20:11:21.826665 a3m-0.7.9/a3m/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-02-12 20:11:03.000000 a3m-0.7.9/a3m/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 20:11:21.826665 a3m-0.7.9/a3m/cli/client/
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-02-12 20:11:03.000000 a3m-0.7.9/a3m/cli/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6195 2024-02-12 20:11:03.000000 a3m-0.7.9/a3m/cli/client/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-02-12 20:11:03.000000 a3m-0.7.9/a3m/cli/client/wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-02-12 20:11:03.000000 a3m-0.7.9/a3m/cli/common.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 20:11:21.830666 a3m-0.7.9/a3m/cli/server/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-02-12 20:11:03.000000 a3m-0.7.9/a3m/cli/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-02-12 20:11:03.000000 a3m-0.7.9/a3m/cli/server/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 20:11:21.830666 a3m-0.7.9/a3m/client/
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-02-12 20:11:03.000000 a3m-0.7.9/a3m/client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 20:11:21.818666 a3m-0.7.9/a3m/client/assets/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 20:11:21.830666 a3m-0.7.9/a3m/client/assets/README/
+-rw-r--r--   0 runner    (1001) docker     (127)     7246 2024-02-12 20:11:03.000000 a3m-0.7.9/a3m/client/assets/README/README.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 20:11:21.830666 a3m-0.7.9/a3m/client/assets/catalog/
+-rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-02-12 20:11:03.000000 a3m-0.7.9/a3m/client/assets/catalog/catalog.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 20:11:21.830666 a3m-0.7.9/a3m/client/assets/mets/
+-rw-r--r--   0 runner    (1001) docker     (127)   136472 2024-02-12 20:11:03.000000 a3m-0.7.9/a3m/client/assets/mets/mets.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     3180 2024-02-12 20:11:03.000000 a3m-0.7.9/a3m/client/assets/mets/xlink.xsd
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 20:11:21.830666 a3m-0.7.9/a3m/client/assets/mods/
+-rw-r--r--   0 runner    (1001) docker     (127)    61831 2024-02-12 20:11:03.000000 a3m-0.7.9/a3m/client/assets/mods/mods.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     5840 2024-02-12 20:11:03.000000 a3m-0.7.9/a3m/client/assets/mods/xml.xsd
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 20:11:21.830666 a3m-0.7.9/a3m/client/assets/premis/
+-rw-r--r--   0 runner    (1001) docker     (127)    65130 2024-02-12 20:11:03.000000 a3m-0.7.9/a3m/client/assets/premis/premis-v2-2.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)    52845 2024-02-12 20:11:03.000000 a3m-0.7.9/a3m/client/assets/premis/premis.xsd
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 20:11:21.842666 a3m-0.7.9/a3m/client/clientScripts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 20:11:03.000000 a3m-0.7.9/a3m/client/clientScripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4997 2024-02-12 20:11:03.000000 a3m-0.7.9/a3m/client/clientScripts/a3m_download_transfer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-02-12 20:11:03.000000 a3m-0.7.9/a3m/client/clientScripts/a3m_store_aip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4498 2024-02-12 20:11:03.000000 a3m-0.7.9/a3m/client/clientScripts/archivematicaCreateMETSMetadataCSV.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15696 2024-02-12 20:11:03.000000 a3m-0.7.9/a3m/client/clientScripts/archivematicaCreateMETSRights.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6452 2024-02-12 20:11:03.000000 a3m-0.7.9/a3m/client/clientScripts/assign_file_uuids.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4242 2024-02-12 20:11:03.000000 a3m-0.7.9/a3m/client/clientScripts/assign_uuids_to_directories.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3409 2024-02-12 20:11:03.000000 a3m-0.7.9/a3m/client/clientScripts/bag_with_empty_directories.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-02-12 20:11:03.000000 a3m-0.7.9/a3m/client/clientScripts/change_names.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9437 2024-02-12 20:11:03.000000 a3m-0.7.9/a3m/client/clientScripts/change_object_names.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4702 2024-02-12 20:11:03.000000 a3m-0.7.9/a3m/client/clientScripts/characterize_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4047 2024-02-12 20:11:03.000000 a3m-0.7.9/a3m/client/clientScripts/check_for_service_directory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-02-12 20:11:03.000000 a3m-0.7.9/a3m/client/clientScripts/check_for_submission_documentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-02-12 20:11:03.000000 a3m-0.7.9/a3m/client/clientScripts/check_transfer_directory_for_objects.py
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-02-12 20:11:03.000000 a3m-0.7.9/a3m/client/clientScripts/cmd_chmod.py
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-02-12 20:11:03.000000 a3m-0.7.9/a3m/client/clientScripts/cmd_cp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-02-12 20:11:03.000000 a3m-0.7.9/a3m/client/clientScripts/cmd_mkdir.py
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-02-12 20:11:03.000000 a3m-0.7.9/a3m/client/clientScripts/cmd_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-02-12 20:11:03.000000 a3m-0.7.9/a3m/client/clientScripts/cmd_tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7088 2024-02-12 20:11:03.000000 a3m-0.7.9/a3m/client/clientScripts/compress_aip.py
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-02-12 20:11:03.000000 a3m-0.7.9/a3m/client/clientScripts/copy_submission_docs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2434 2024-02-12 20:11:03.000000 a3m-0.7.9/a3m/client/clientScripts/copy_transfer_submission_documentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4208 2024-02-12 20:11:03.000000 a3m-0.7.9/a3m/client/clientScripts/copy_transfers_metadata_and_logs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59226 2024-02-12 20:11:03.000000 a3m-0.7.9/a3m/client/clientScripts/create_mets_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3948 2024-02-12 20:11:03.000000 a3m-0.7.9/a3m/client/clientScripts/create_sip_from_transfer_objects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1947 2024-02-12 20:11:03.000000 a3m-0.7.9/a3m/client/clientScripts/create_transfer_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-02-12 20:11:03.000000 a3m-0.7.9/a3m/client/clientScripts/examine_contents.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10123 2024-02-12 20:11:03.000000 a3m-0.7.9/a3m/client/clientScripts/extract_contents.py
+-rw-r--r--   0 runner    (1001) docker     (127)      659 2024-02-12 20:11:03.000000 a3m-0.7.9/a3m/client/clientScripts/failed_sip_cleanup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-02-12 20:11:03.000000 a3m-0.7.9/a3m/client/clientScripts/failed_transfer_cleanup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-02-12 20:11:03.000000 a3m-0.7.9/a3m/client/clientScripts/has_packages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3843 2024-02-12 20:11:03.000000 a3m-0.7.9/a3m/client/clientScripts/identify_file_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4476 2024-02-12 20:11:03.000000 a3m-0.7.9/a3m/client/clientScripts/json_metadata_to_csv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-02-12 20:11:03.000000 a3m-0.7.9/a3m/client/clientScripts/load_dublin_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-02-12 20:11:03.000000 a3m-0.7.9/a3m/client/clientScripts/load_labels_from_csv.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29374 2024-02-12 20:11:03.000000 a3m-0.7.9/a3m/client/clientScripts/load_premis_events_from_xml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-02-12 20:11:03.000000 a3m-0.7.9/a3m/client/clientScripts/manual_normalization_check_for_manual_normalization_directory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7291 2024-02-12 20:11:03.000000 a3m-0.7.9/a3m/client/clientScripts/manual_normalization_create_metadata_and_restructure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-02-12 20:11:03.000000 a3m-0.7.9/a3m/client/clientScripts/manual_normalization_identify_files_included.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2458 2024-02-12 20:11:03.000000 a3m-0.7.9/a3m/client/clientScripts/manual_normalization_remove_mn_directories.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3317 2024-02-12 20:11:03.000000 a3m-0.7.9/a3m/client/clientScripts/move_or_merge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2065 2024-02-12 20:11:03.000000 a3m-0.7.9/a3m/client/clientScripts/move_sip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-02-12 20:11:03.000000 a3m-0.7.9/a3m/client/clientScripts/move_transfer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18485 2024-02-12 20:11:03.000000 a3m-0.7.9/a3m/client/clientScripts/normalize.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18843 2024-02-12 20:11:03.000000 a3m-0.7.9/a3m/client/clientScripts/policy_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-02-12 20:11:03.000000 a3m-0.7.9/a3m/client/clientScripts/remove_directories.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1922 2024-02-12 20:11:03.000000 a3m-0.7.9/a3m/client/clientScripts/remove_files_without_premis_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-02-12 20:11:03.000000 a3m-0.7.9/a3m/client/clientScripts/remove_hidden_files_and_directories.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1590 2024-02-12 20:11:03.000000 a3m-0.7.9/a3m/client/clientScripts/remove_unneeded_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2180 2024-02-12 20:11:03.000000 a3m-0.7.9/a3m/client/clientScripts/restructure_for_compliance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16354 2024-02-12 20:11:03.000000 a3m-0.7.9/a3m/client/clientScripts/rights_from_csv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-02-12 20:11:03.000000 a3m-0.7.9/a3m/client/clientScripts/save_dublin_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2474 2024-02-12 20:11:03.000000 a3m-0.7.9/a3m/client/clientScripts/store_file_modification_dates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4910 2024-02-12 20:11:03.000000 a3m-0.7.9/a3m/client/clientScripts/transcribe_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4581 2024-02-12 20:11:03.000000 a3m-0.7.9/a3m/client/clientScripts/update_size_and_checksum.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12524 2024-02-12 20:11:03.000000 a3m-0.7.9/a3m/client/clientScripts/validate_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8663 2024-02-12 20:11:03.000000 a3m-0.7.9/a3m/client/clientScripts/verify_aip.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10984 2024-02-12 20:11:03.000000 a3m-0.7.9/a3m/client/clientScripts/verify_checksum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-02-12 20:11:03.000000 a3m-0.7.9/a3m/client/clientScripts/verify_mets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2589 2024-02-12 20:11:03.000000 a3m-0.7.9/a3m/client/clientScripts/verify_sip_compliance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2478 2024-02-12 20:11:03.000000 a3m-0.7.9/a3m/client/clientScripts/verify_transfer_compliance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3709 2024-02-12 20:11:03.000000 a3m-0.7.9/a3m/client/job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8354 2024-02-12 20:11:03.000000 a3m-0.7.9/a3m/client/mcp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7672 2024-02-12 20:11:03.000000 a3m-0.7.9/a3m/client/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1811 2024-02-12 20:11:03.000000 a3m-0.7.9/a3m/common_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7351 2024-02-12 20:11:03.000000 a3m-0.7.9/a3m/countryCodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9571 2024-02-12 20:11:03.000000 a3m-0.7.9/a3m/databaseFunctions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8634 2024-02-12 20:11:03.000000 a3m-0.7.9/a3m/dicts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10094 2024-02-12 20:11:03.000000 a3m-0.7.9/a3m/executeOrRunSubProcess.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8130 2024-02-12 20:11:03.000000 a3m-0.7.9/a3m/fileOperations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 20:11:21.842666 a3m-0.7.9/a3m/fpr/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 20:11:03.000000 a3m-0.7.9/a3m/fpr/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 20:11:21.842666 a3m-0.7.9/a3m/fpr/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 20:11:03.000000 a3m-0.7.9/a3m/fpr/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)  2341782 2024-02-12 20:11:03.000000 a3m-0.7.9/a3m/fpr/migrations/initial-data.json
+-rw-r--r--   0 runner    (1001) docker     (127)    18206 2024-02-12 20:11:03.000000 a3m-0.7.9/a3m/fpr/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 20:11:21.846666 a3m-0.7.9/a3m/main/
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-02-12 20:11:03.000000 a3m-0.7.9/a3m/main/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-02-12 20:11:03.000000 a3m-0.7.9/a3m/main/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 20:11:21.846666 a3m-0.7.9/a3m/main/management/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 20:11:03.000000 a3m-0.7.9/a3m/main/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 20:11:21.846666 a3m-0.7.9/a3m/main/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)    63688 2024-02-12 20:11:03.000000 a3m-0.7.9/a3m/main/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-02-12 20:11:03.000000 a3m-0.7.9/a3m/main/migrations/0002_initial_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 20:11:03.000000 a3m-0.7.9/a3m/main/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5999 2024-02-12 20:11:03.000000 a3m-0.7.9/a3m/main/migrations/initial-data.json
+-rw-r--r--   0 runner    (1001) docker     (127)    47453 2024-02-12 20:11:03.000000 a3m-0.7.9/a3m/main/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-02-12 20:11:03.000000 a3m-0.7.9/a3m/namespaces.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 20:11:21.850666 a3m-0.7.9/a3m/server/
+-rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-02-12 20:11:03.000000 a3m-0.7.9/a3m/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6652 2024-02-12 20:11:03.000000 a3m-0.7.9/a3m/server/db.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 20:11:21.850666 a3m-0.7.9/a3m/server/jobs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-02-12 20:11:03.000000 a3m-0.7.9/a3m/server/jobs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2851 2024-02-12 20:11:03.000000 a3m-0.7.9/a3m/server/jobs/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3888 2024-02-12 20:11:03.000000 a3m-0.7.9/a3m/server/jobs/chain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6815 2024-02-12 20:11:03.000000 a3m-0.7.9/a3m/server/jobs/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-02-12 20:11:03.000000 a3m-0.7.9/a3m/server/jobs/decisions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3937 2024-02-12 20:11:03.000000 a3m-0.7.9/a3m/server/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16191 2024-02-12 20:11:03.000000 a3m-0.7.9/a3m/server/packages.py
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-02-12 20:11:03.000000 a3m-0.7.9/a3m/server/processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10885 2024-02-12 20:11:03.000000 a3m-0.7.9/a3m/server/queues.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 20:11:21.850666 a3m-0.7.9/a3m/server/rpc/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-02-12 20:11:03.000000 a3m-0.7.9/a3m/server/rpc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3146 2024-02-12 20:11:03.000000 a3m-0.7.9/a3m/server/rpc/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7392 2024-02-12 20:11:03.000000 a3m-0.7.9/a3m/server/runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)      969 2024-02-12 20:11:03.000000 a3m-0.7.9/a3m/server/shared_dirs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 20:11:21.850666 a3m-0.7.9/a3m/server/tasks/
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-02-12 20:11:03.000000 a3m-0.7.9/a3m/server/tasks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 20:11:21.850666 a3m-0.7.9/a3m/server/tasks/backends/
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2024-02-12 20:11:03.000000 a3m-0.7.9/a3m/server/tasks/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-02-12 20:11:03.000000 a3m-0.7.9/a3m/server/tasks/backends/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5559 2024-02-12 20:11:03.000000 a3m-0.7.9/a3m/server/tasks/backends/pool_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3583 2024-02-12 20:11:03.000000 a3m-0.7.9/a3m/server/tasks/task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3359 2024-02-12 20:11:03.000000 a3m-0.7.9/a3m/server/transfer_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2121 2024-02-12 20:11:03.000000 a3m-0.7.9/a3m/server/translation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6167 2024-02-12 20:11:03.000000 a3m-0.7.9/a3m/server/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 20:11:21.854666 a3m-0.7.9/a3m/settings/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 20:11:03.000000 a3m-0.7.9/a3m/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9645 2024-02-12 20:11:03.000000 a3m-0.7.9/a3m/settings/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-02-12 20:11:03.000000 a3m-0.7.9/a3m/settings/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 20:11:21.854666 a3m-0.7.9/a3m.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    43994 2024-02-12 20:11:21.000000 a3m-0.7.9/a3m.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5531 2024-02-12 20:11:21.000000 a3m-0.7.9/a3m.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-12 20:11:21.000000 a3m-0.7.9/a3m.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-02-12 20:11:21.000000 a3m-0.7.9/a3m.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      557 2024-02-12 20:11:21.000000 a3m-0.7.9/a3m.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-02-12 20:11:21.000000 a3m-0.7.9/a3m.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5084 2024-02-12 20:11:03.000000 a3m-0.7.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-12 20:11:21.854666 a3m-0.7.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 20:11:21.854666 a3m-0.7.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3142 2024-02-12 20:11:03.000000 a3m-0.7.9/tests/test_registry.py
```

### Comparing `a3m-0.7.8/LICENSE` & `a3m-0.7.9/LICENSE`

 * *Files identical despite different names*

### Comparing `a3m-0.7.8/PKG-INFO` & `a3m-0.7.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: a3m
-Version: 0.7.8
+Version: 0.7.9
 Summary: Lightweight Archivematica
 Author-email: "Artefactual Systems Inc." <info@artefactual.com>
 Maintainer-email: "Artefactual Systems Inc." <info@artefactual.com>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
```

### Comparing `a3m-0.7.8/README.rst` & `a3m-0.7.9/README.rst`

 * *Files identical despite different names*

### Comparing `a3m-0.7.8/a3m/api/transferservice/v1beta1/request_response_pb2.py` & `a3m-0.7.9/a3m/api/transferservice/v1beta1/request_response_pb2.py`

 * *Files identical despite different names*

### Comparing `a3m-0.7.8/a3m/api/transferservice/v1beta1/request_response_pb2.pyi` & `a3m-0.7.9/a3m/api/transferservice/v1beta1/request_response_pb2.pyi`

 * *Files identical despite different names*

### Comparing `a3m-0.7.8/a3m/api/transferservice/v1beta1/service_pb2.py` & `a3m-0.7.9/a3m/api/transferservice/v1beta1/service_pb2.py`

 * *Files identical despite different names*

### Comparing `a3m-0.7.8/a3m/api/transferservice/v1beta1/service_pb2_grpc.py` & `a3m-0.7.9/a3m/api/transferservice/v1beta1/service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `a3m-0.7.8/a3m/appconfig.py` & `a3m-0.7.9/a3m/appconfig.py`

 * *Files identical despite different names*

### Comparing `a3m-0.7.8/a3m/archivematicaFunctions.py` & `a3m-0.7.9/a3m/archivematicaFunctions.py`

 * *Files identical despite different names*

### Comparing `a3m-0.7.8/a3m/assets/workflow-schema-v1.json` & `a3m-0.7.9/a3m/assets/workflow-schema-v1.json`

 * *Files identical despite different names*

### Comparing `a3m-0.7.8/a3m/assets/workflow.json` & `a3m-0.7.9/a3m/assets/workflow.json`

 * *Files identical despite different names*

### Comparing `a3m-0.7.8/a3m/cli/__init__.py` & `a3m-0.7.9/a3m/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `a3m-0.7.8/a3m/cli/client/__main__.py` & `a3m-0.7.9/a3m/cli/client/__main__.py`

 * *Files identical despite different names*

### Comparing `a3m-0.7.8/a3m/cli/client/wrapper.py` & `a3m-0.7.9/a3m/cli/client/wrapper.py`

 * *Files identical despite different names*

### Comparing `a3m-0.7.8/a3m/cli/common.py` & `a3m-0.7.9/a3m/cli/common.py`

 * *Files identical despite different names*

### Comparing `a3m-0.7.8/a3m/cli/server/__main__.py` & `a3m-0.7.9/a3m/cli/server/__main__.py`

 * *Files identical despite different names*

### Comparing `a3m-0.7.8/a3m/client/assets/README/README.html` & `a3m-0.7.9/a3m/client/assets/README/README.html`

 * *Files identical despite different names*

### Comparing `a3m-0.7.8/a3m/client/assets/catalog/catalog.xml` & `a3m-0.7.9/a3m/client/assets/catalog/catalog.xml`

 * *Files identical despite different names*

### Comparing `a3m-0.7.8/a3m/client/assets/mets/mets.xsd` & `a3m-0.7.9/a3m/client/assets/mets/mets.xsd`

 * *Files identical despite different names*

### Comparing `a3m-0.7.8/a3m/client/assets/mets/xlink.xsd` & `a3m-0.7.9/a3m/client/assets/mets/xlink.xsd`

 * *Files identical despite different names*

### Comparing `a3m-0.7.8/a3m/client/assets/mods/mods.xsd` & `a3m-0.7.9/a3m/client/assets/mods/mods.xsd`

 * *Files identical despite different names*

### Comparing `a3m-0.7.8/a3m/client/assets/mods/xml.xsd` & `a3m-0.7.9/a3m/client/assets/mods/xml.xsd`

 * *Files identical despite different names*

### Comparing `a3m-0.7.8/a3m/client/assets/premis/premis-v2-2.xsd` & `a3m-0.7.9/a3m/client/assets/premis/premis-v2-2.xsd`

 * *Files identical despite different names*

### Comparing `a3m-0.7.8/a3m/client/assets/premis/premis.xsd` & `a3m-0.7.9/a3m/client/assets/premis/premis.xsd`

 * *Files identical despite different names*

### Comparing `a3m-0.7.8/a3m/client/clientScripts/a3m_download_transfer.py` & `a3m-0.7.9/a3m/client/clientScripts/a3m_download_transfer.py`

 * *Files identical despite different names*

### Comparing `a3m-0.7.8/a3m/client/clientScripts/a3m_store_aip.py` & `a3m-0.7.9/a3m/client/clientScripts/a3m_store_aip.py`

 * *Files identical despite different names*

### Comparing `a3m-0.7.8/a3m/client/clientScripts/archivematicaCreateMETSMetadataCSV.py` & `a3m-0.7.9/a3m/client/clientScripts/archivematicaCreateMETSMetadataCSV.py`

 * *Files identical despite different names*

### Comparing `a3m-0.7.8/a3m/client/clientScripts/archivematicaCreateMETSRights.py` & `a3m-0.7.9/a3m/client/clientScripts/archivematicaCreateMETSRights.py`

 * *Files identical despite different names*

### Comparing `a3m-0.7.8/a3m/client/clientScripts/assign_file_uuids.py` & `a3m-0.7.9/a3m/client/clientScripts/assign_file_uuids.py`

 * *Files identical despite different names*

### Comparing `a3m-0.7.8/a3m/client/clientScripts/assign_uuids_to_directories.py` & `a3m-0.7.9/a3m/client/clientScripts/assign_uuids_to_directories.py`

 * *Files identical despite different names*

### Comparing `a3m-0.7.8/a3m/client/clientScripts/bag_with_empty_directories.py` & `a3m-0.7.9/a3m/client/clientScripts/bag_with_empty_directories.py`

 * *Files identical despite different names*

### Comparing `a3m-0.7.8/a3m/client/clientScripts/change_names.py` & `a3m-0.7.9/a3m/client/clientScripts/change_names.py`

 * *Files identical despite different names*

### Comparing `a3m-0.7.8/a3m/client/clientScripts/change_object_names.py` & `a3m-0.7.9/a3m/client/clientScripts/change_object_names.py`

 * *Files identical despite different names*

### Comparing `a3m-0.7.8/a3m/client/clientScripts/characterize_file.py` & `a3m-0.7.9/a3m/client/clientScripts/characterize_file.py`

 * *Files identical despite different names*

### Comparing `a3m-0.7.8/a3m/client/clientScripts/check_for_service_directory.py` & `a3m-0.7.9/a3m/client/clientScripts/check_for_service_directory.py`

 * *Files identical despite different names*

### Comparing `a3m-0.7.8/a3m/client/clientScripts/check_for_submission_documentation.py` & `a3m-0.7.9/a3m/client/clientScripts/check_for_submission_documentation.py`

 * *Files identical despite different names*

### Comparing `a3m-0.7.8/a3m/client/clientScripts/check_transfer_directory_for_objects.py` & `a3m-0.7.9/a3m/client/clientScripts/check_transfer_directory_for_objects.py`

 * *Files identical despite different names*

### Comparing `a3m-0.7.8/a3m/client/clientScripts/compress_aip.py` & `a3m-0.7.9/a3m/client/clientScripts/compress_aip.py`

 * *Files identical despite different names*

### Comparing `a3m-0.7.8/a3m/client/clientScripts/copy_submission_docs.py` & `a3m-0.7.9/a3m/client/clientScripts/copy_submission_docs.py`

 * *Files identical despite different names*

### Comparing `a3m-0.7.8/a3m/client/clientScripts/copy_transfer_submission_documentation.py` & `a3m-0.7.9/a3m/client/clientScripts/copy_transfer_submission_documentation.py`

 * *Files identical despite different names*

### Comparing `a3m-0.7.8/a3m/client/clientScripts/copy_transfers_metadata_and_logs.py` & `a3m-0.7.9/a3m/client/clientScripts/copy_transfers_metadata_and_logs.py`

 * *Files identical despite different names*

### Comparing `a3m-0.7.8/a3m/client/clientScripts/create_mets_v2.py` & `a3m-0.7.9/a3m/client/clientScripts/create_mets_v2.py`

 * *Files identical despite different names*

### Comparing `a3m-0.7.8/a3m/client/clientScripts/create_sip_from_transfer_objects.py` & `a3m-0.7.9/a3m/client/clientScripts/create_sip_from_transfer_objects.py`

 * *Files identical despite different names*

### Comparing `a3m-0.7.8/a3m/client/clientScripts/create_transfer_metadata.py` & `a3m-0.7.9/a3m/client/clientScripts/create_transfer_metadata.py`

 * *Files identical despite different names*

### Comparing `a3m-0.7.8/a3m/client/clientScripts/examine_contents.py` & `a3m-0.7.9/a3m/client/clientScripts/examine_contents.py`

 * *Files identical despite different names*

### Comparing `a3m-0.7.8/a3m/client/clientScripts/extract_contents.py` & `a3m-0.7.9/a3m/client/clientScripts/extract_contents.py`

 * *Files identical despite different names*

### Comparing `a3m-0.7.8/a3m/client/clientScripts/failed_sip_cleanup.py` & `a3m-0.7.9/a3m/client/clientScripts/failed_sip_cleanup.py`

 * *Files identical despite different names*

### Comparing `a3m-0.7.8/a3m/client/clientScripts/has_packages.py` & `a3m-0.7.9/a3m/client/clientScripts/has_packages.py`

 * *Files identical despite different names*

### Comparing `a3m-0.7.8/a3m/client/clientScripts/identify_file_format.py` & `a3m-0.7.9/a3m/client/clientScripts/identify_file_format.py`

 * *Files identical despite different names*

### Comparing `a3m-0.7.8/a3m/client/clientScripts/json_metadata_to_csv.py` & `a3m-0.7.9/a3m/client/clientScripts/json_metadata_to_csv.py`

 * *Files identical despite different names*

### Comparing `a3m-0.7.8/a3m/client/clientScripts/load_dublin_core.py` & `a3m-0.7.9/a3m/client/clientScripts/load_dublin_core.py`

 * *Files identical despite different names*

### Comparing `a3m-0.7.8/a3m/client/clientScripts/load_labels_from_csv.py` & `a3m-0.7.9/a3m/client/clientScripts/load_labels_from_csv.py`

 * *Files identical despite different names*

### Comparing `a3m-0.7.8/a3m/client/clientScripts/load_premis_events_from_xml.py` & `a3m-0.7.9/a3m/client/clientScripts/load_premis_events_from_xml.py`

 * *Files identical despite different names*

### Comparing `a3m-0.7.8/a3m/client/clientScripts/manual_normalization_check_for_manual_normalization_directory.py` & `a3m-0.7.9/a3m/client/clientScripts/manual_normalization_check_for_manual_normalization_directory.py`

 * *Files identical despite different names*

### Comparing `a3m-0.7.8/a3m/client/clientScripts/manual_normalization_create_metadata_and_restructure.py` & `a3m-0.7.9/a3m/client/clientScripts/manual_normalization_create_metadata_and_restructure.py`

 * *Files identical despite different names*

### Comparing `a3m-0.7.8/a3m/client/clientScripts/manual_normalization_identify_files_included.py` & `a3m-0.7.9/a3m/client/clientScripts/manual_normalization_identify_files_included.py`

 * *Files identical despite different names*

### Comparing `a3m-0.7.8/a3m/client/clientScripts/manual_normalization_remove_mn_directories.py` & `a3m-0.7.9/a3m/client/clientScripts/manual_normalization_remove_mn_directories.py`

 * *Files identical despite different names*

### Comparing `a3m-0.7.8/a3m/client/clientScripts/move_or_merge.py` & `a3m-0.7.9/a3m/client/clientScripts/move_or_merge.py`

 * *Files identical despite different names*

### Comparing `a3m-0.7.8/a3m/client/clientScripts/move_sip.py` & `a3m-0.7.9/a3m/client/clientScripts/move_sip.py`

 * *Files identical despite different names*

### Comparing `a3m-0.7.8/a3m/client/clientScripts/move_transfer.py` & `a3m-0.7.9/a3m/client/clientScripts/move_transfer.py`

 * *Files identical despite different names*

### Comparing `a3m-0.7.8/a3m/client/clientScripts/normalize.py` & `a3m-0.7.9/a3m/client/clientScripts/normalize.py`

 * *Files identical despite different names*

### Comparing `a3m-0.7.8/a3m/client/clientScripts/policy_check.py` & `a3m-0.7.9/a3m/client/clientScripts/policy_check.py`

 * *Files identical despite different names*

### Comparing `a3m-0.7.8/a3m/client/clientScripts/remove_directories.py` & `a3m-0.7.9/a3m/client/clientScripts/remove_directories.py`

 * *Files identical despite different names*

### Comparing `a3m-0.7.8/a3m/client/clientScripts/remove_files_without_premis_metadata.py` & `a3m-0.7.9/a3m/client/clientScripts/remove_files_without_premis_metadata.py`

 * *Files identical despite different names*

### Comparing `a3m-0.7.8/a3m/client/clientScripts/remove_hidden_files_and_directories.py` & `a3m-0.7.9/a3m/client/clientScripts/remove_hidden_files_and_directories.py`

 * *Files identical despite different names*

### Comparing `a3m-0.7.8/a3m/client/clientScripts/remove_unneeded_files.py` & `a3m-0.7.9/a3m/client/clientScripts/remove_unneeded_files.py`

 * *Files identical despite different names*

### Comparing `a3m-0.7.8/a3m/client/clientScripts/restructure_for_compliance.py` & `a3m-0.7.9/a3m/client/clientScripts/restructure_for_compliance.py`

 * *Files identical despite different names*

### Comparing `a3m-0.7.8/a3m/client/clientScripts/rights_from_csv.py` & `a3m-0.7.9/a3m/client/clientScripts/rights_from_csv.py`

 * *Files identical despite different names*

### Comparing `a3m-0.7.8/a3m/client/clientScripts/save_dublin_core.py` & `a3m-0.7.9/a3m/client/clientScripts/save_dublin_core.py`

 * *Files identical despite different names*

### Comparing `a3m-0.7.8/a3m/client/clientScripts/store_file_modification_dates.py` & `a3m-0.7.9/a3m/client/clientScripts/store_file_modification_dates.py`

 * *Files identical despite different names*

### Comparing `a3m-0.7.8/a3m/client/clientScripts/transcribe_file.py` & `a3m-0.7.9/a3m/client/clientScripts/transcribe_file.py`

 * *Files identical despite different names*

### Comparing `a3m-0.7.8/a3m/client/clientScripts/update_size_and_checksum.py` & `a3m-0.7.9/a3m/client/clientScripts/update_size_and_checksum.py`

 * *Files identical despite different names*

### Comparing `a3m-0.7.8/a3m/client/clientScripts/validate_file.py` & `a3m-0.7.9/a3m/client/clientScripts/validate_file.py`

 * *Files identical despite different names*

### Comparing `a3m-0.7.8/a3m/client/clientScripts/verify_aip.py` & `a3m-0.7.9/a3m/client/clientScripts/verify_aip.py`

 * *Files identical despite different names*

### Comparing `a3m-0.7.8/a3m/client/clientScripts/verify_checksum.py` & `a3m-0.7.9/a3m/client/clientScripts/verify_checksum.py`

 * *Files identical despite different names*

### Comparing `a3m-0.7.8/a3m/client/clientScripts/verify_mets.py` & `a3m-0.7.9/a3m/client/clientScripts/verify_mets.py`

 * *Files identical despite different names*

### Comparing `a3m-0.7.8/a3m/client/clientScripts/verify_sip_compliance.py` & `a3m-0.7.9/a3m/client/clientScripts/verify_sip_compliance.py`

 * *Files identical despite different names*

### Comparing `a3m-0.7.8/a3m/client/clientScripts/verify_transfer_compliance.py` & `a3m-0.7.9/a3m/client/clientScripts/verify_transfer_compliance.py`

 * *Files identical despite different names*

### Comparing `a3m-0.7.8/a3m/client/job.py` & `a3m-0.7.9/a3m/client/job.py`

 * *Files identical despite different names*

### Comparing `a3m-0.7.8/a3m/client/mcp.py` & `a3m-0.7.9/a3m/client/mcp.py`

 * *Files identical despite different names*

### Comparing `a3m-0.7.8/a3m/client/metrics.py` & `a3m-0.7.9/a3m/client/metrics.py`

 * *Files identical despite different names*

### Comparing `a3m-0.7.8/a3m/common_metrics.py` & `a3m-0.7.9/a3m/common_metrics.py`

 * *Files identical despite different names*

### Comparing `a3m-0.7.8/a3m/countryCodes.py` & `a3m-0.7.9/a3m/countryCodes.py`

 * *Files identical despite different names*

### Comparing `a3m-0.7.8/a3m/databaseFunctions.py` & `a3m-0.7.9/a3m/databaseFunctions.py`

 * *Files identical despite different names*

### Comparing `a3m-0.7.8/a3m/dicts.py` & `a3m-0.7.9/a3m/dicts.py`

 * *Files identical despite different names*

### Comparing `a3m-0.7.8/a3m/executeOrRunSubProcess.py` & `a3m-0.7.9/a3m/executeOrRunSubProcess.py`

 * *Files identical despite different names*

### Comparing `a3m-0.7.8/a3m/fileOperations.py` & `a3m-0.7.9/a3m/fileOperations.py`

 * *Files identical despite different names*

### Comparing `a3m-0.7.8/a3m/fpr/migrations/initial-data.json` & `a3m-0.7.9/a3m/fpr/migrations/initial-data.json`

 * *Files identical despite different names*

### Comparing `a3m-0.7.8/a3m/fpr/registry.py` & `a3m-0.7.9/a3m/fpr/registry.py`

 * *Files identical despite different names*

### Comparing `a3m-0.7.8/a3m/main/migrations/0001_initial.py` & `a3m-0.7.9/a3m/main/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `a3m-0.7.8/a3m/main/migrations/initial-data.json` & `a3m-0.7.9/a3m/main/migrations/initial-data.json`

 * *Files identical despite different names*

### Comparing `a3m-0.7.8/a3m/main/models.py` & `a3m-0.7.9/a3m/main/models.py`

 * *Files identical despite different names*

### Comparing `a3m-0.7.8/a3m/namespaces.py` & `a3m-0.7.9/a3m/namespaces.py`

 * *Files identical despite different names*

### Comparing `a3m-0.7.8/a3m/server/__init__.py` & `a3m-0.7.9/a3m/server/__init__.py`

 * *Files identical despite different names*

### Comparing `a3m-0.7.8/a3m/server/db.py` & `a3m-0.7.9/a3m/server/db.py`

 * *Files identical despite different names*

### Comparing `a3m-0.7.8/a3m/server/jobs/__init__.py` & `a3m-0.7.9/a3m/server/jobs/__init__.py`

 * *Files identical despite different names*

### Comparing `a3m-0.7.8/a3m/server/jobs/base.py` & `a3m-0.7.9/a3m/server/jobs/base.py`

 * *Files identical despite different names*

### Comparing `a3m-0.7.8/a3m/server/jobs/chain.py` & `a3m-0.7.9/a3m/server/jobs/chain.py`

 * *Files identical despite different names*

### Comparing `a3m-0.7.8/a3m/server/jobs/client.py` & `a3m-0.7.9/a3m/server/jobs/client.py`

 * *Files identical despite different names*

### Comparing `a3m-0.7.8/a3m/server/jobs/decisions.py` & `a3m-0.7.9/a3m/server/jobs/decisions.py`

 * *Files identical despite different names*

### Comparing `a3m-0.7.8/a3m/server/metrics.py` & `a3m-0.7.9/a3m/server/metrics.py`

 * *Files identical despite different names*

### Comparing `a3m-0.7.8/a3m/server/packages.py` & `a3m-0.7.9/a3m/server/packages.py`

 * *Files identical despite different names*

### Comparing `a3m-0.7.8/a3m/server/processing.py` & `a3m-0.7.9/a3m/server/processing.py`

 * *Files identical despite different names*

### Comparing `a3m-0.7.8/a3m/server/queues.py` & `a3m-0.7.9/a3m/server/queues.py`

 * *Files identical despite different names*

### Comparing `a3m-0.7.8/a3m/server/rpc/client.py` & `a3m-0.7.9/a3m/server/rpc/client.py`

 * *Files identical despite different names*

### Comparing `a3m-0.7.8/a3m/server/runner.py` & `a3m-0.7.9/a3m/server/runner.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,15 +85,23 @@
         self.queue = PackageQueue(
             self.queue_executor,
             self.queue_shutdown_event,
             max_concurrent_packages=max_concurrent_packages,
             debug=debug,
         )
         self.grpc_executor = grpc_executor
-        self.grpc_server = grpc.server(grpc_executor)
+        self.grpc_server = grpc.server(
+            grpc_executor,
+            options=[
+                # Adjusted server tolerance to more frequent keepalive pings,
+                # mitigating ENHANCE_YOUR_CALM errors by allowing shorter
+                # intervals between pings.
+                ("grpc.http2.min_ping_interval_without_data_ms", 100),
+            ],
+        )
         self.grpc_port = self.grpc_server.add_insecure_port(bind_address)
 
         self._mount_services()
 
     def _mount_services(self):
         transfer_service = TransferService(
             self.workflow, self.queue, self.queue_executor
```

### Comparing `a3m-0.7.8/a3m/server/shared_dirs.py` & `a3m-0.7.9/a3m/server/shared_dirs.py`

 * *Files identical despite different names*

### Comparing `a3m-0.7.8/a3m/server/tasks/backends/__init__.py` & `a3m-0.7.9/a3m/server/tasks/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `a3m-0.7.8/a3m/server/tasks/backends/base.py` & `a3m-0.7.9/a3m/server/tasks/backends/base.py`

 * *Files identical despite different names*

### Comparing `a3m-0.7.8/a3m/server/tasks/backends/pool_backend.py` & `a3m-0.7.9/a3m/server/tasks/backends/pool_backend.py`

 * *Files identical despite different names*

### Comparing `a3m-0.7.8/a3m/server/tasks/task.py` & `a3m-0.7.9/a3m/server/tasks/task.py`

 * *Files identical despite different names*

### Comparing `a3m-0.7.8/a3m/server/transfer_service.py` & `a3m-0.7.9/a3m/server/transfer_service.py`

 * *Files identical despite different names*

### Comparing `a3m-0.7.8/a3m/server/translation.py` & `a3m-0.7.9/a3m/server/translation.py`

 * *Files identical despite different names*

### Comparing `a3m-0.7.8/a3m/server/workflow.py` & `a3m-0.7.9/a3m/server/workflow.py`

 * *Files identical despite different names*

### Comparing `a3m-0.7.8/a3m/settings/common.py` & `a3m-0.7.9/a3m/settings/common.py`

 * *Files identical despite different names*

### Comparing `a3m-0.7.8/a3m/settings/test.py` & `a3m-0.7.9/a3m/settings/test.py`

 * *Files identical despite different names*

### Comparing `a3m-0.7.8/a3m.egg-info/PKG-INFO` & `a3m-0.7.9/a3m.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: a3m
-Version: 0.7.8
+Version: 0.7.9
 Summary: Lightweight Archivematica
 Author-email: "Artefactual Systems Inc." <info@artefactual.com>
 Maintainer-email: "Artefactual Systems Inc." <info@artefactual.com>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
```

### Comparing `a3m-0.7.8/a3m.egg-info/SOURCES.txt` & `a3m-0.7.9/a3m.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `a3m-0.7.8/a3m.egg-info/requires.txt` & `a3m-0.7.9/a3m.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `a3m-0.7.8/pyproject.toml` & `a3m-0.7.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `a3m-0.7.8/tests/test_registry.py` & `a3m-0.7.9/tests/test_registry.py`

 * *Files identical despite different names*

