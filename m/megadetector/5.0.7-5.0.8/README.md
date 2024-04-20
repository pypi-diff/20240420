# Comparing `tmp/megadetector-5.0.7.tar.gz` & `tmp/megadetector-5.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "megadetector-5.0.7.tar", last modified: Fri Feb  2 00:50:45 2024, max compression
+gzip compressed data, was "megadetector-5.0.8.tar", last modified: Fri Apr 19 23:55:36 2024, max compression
```

## Comparing `megadetector-5.0.7.tar` & `megadetector-5.0.8.tar`

### file list

```diff
@@ -1,247 +1,250 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-02-02 00:50:45.496962 megadetector-5.0.7/
--rw-rw-r--   0 user      (1000) user      (1000)     1100 2023-05-22 23:49:44.000000 megadetector-5.0.7/LICENSE
--rw-r--r--   0 user      (1000) user      (1000)     7503 2024-02-02 00:50:45.496962 megadetector-5.0.7/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)     4941 2023-12-06 01:46:06.000000 megadetector-5.0.7/README-package.md
--rw-rw-r--   0 user      (1000) user      (1000)    19276 2023-12-07 22:17:50.000000 megadetector-5.0.7/README.md
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-02-02 00:50:45.480962 megadetector-5.0.7/api/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-02-02 00:50:45.480962 megadetector-5.0.7/api/batch_processing/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-02-02 00:50:45.484962 megadetector-5.0.7/api/batch_processing/api_core/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-02-02 00:50:45.484962 megadetector-5.0.7/api/batch_processing/api_core/batch_service/
--rw-rw-r--   0 user      (1000) user      (1000)    17347 2023-05-21 20:45:21.000000 megadetector-5.0.7/api/batch_processing/api_core/batch_service/score.py
--rw-rw-r--   0 user      (1000) user      (1000)    11668 2023-05-21 18:12:32.000000 megadetector-5.0.7/api/batch_processing/api_core/server.py
--rw-rw-r--   0 user      (1000) user      (1000)     3318 2023-05-20 21:19:48.000000 megadetector-5.0.7/api/batch_processing/api_core/server_api_config.py
--rw-rw-r--   0 user      (1000) user      (1000)     1860 2023-05-20 21:19:48.000000 megadetector-5.0.7/api/batch_processing/api_core/server_app_config.py
--rw-rw-r--   0 user      (1000) user      (1000)    10324 2023-05-21 18:12:32.000000 megadetector-5.0.7/api/batch_processing/api_core/server_batch_job_manager.py
--rw-rw-r--   0 user      (1000) user      (1000)     6240 2023-05-20 21:19:48.000000 megadetector-5.0.7/api/batch_processing/api_core/server_job_status_table.py
--rw-rw-r--   0 user      (1000) user      (1000)    17003 2023-05-21 18:12:32.000000 megadetector-5.0.7/api/batch_processing/api_core/server_orchestration.py
--rw-rw-r--   0 user      (1000) user      (1000)     3314 2023-05-21 18:12:32.000000 megadetector-5.0.7/api/batch_processing/api_core/server_utils.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-02-02 00:50:45.484962 megadetector-5.0.7/api/batch_processing/api_core_support/
--rw-rw-r--   0 user      (1000) user      (1000)     2275 2023-05-20 21:19:48.000000 megadetector-5.0.7/api/batch_processing/api_core_support/aggregate_results_manually.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-02-02 00:50:45.484962 megadetector-5.0.7/api/batch_processing/api_support/
--rw-rw-r--   0 user      (1000) user      (1000)     5383 2023-05-20 21:19:48.000000 megadetector-5.0.7/api/batch_processing/api_support/summarize_daily_activity.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-02-02 00:50:45.484962 megadetector-5.0.7/api/batch_processing/data_preparation/
--rw-rw-r--   0 user      (1000) user      (1000)    88618 2024-02-02 00:27:22.000000 megadetector-5.0.7/api/batch_processing/data_preparation/manage_local_batch.py
--rw-rw-r--   0 user      (1000) user      (1000)     9668 2024-01-28 18:41:58.000000 megadetector-5.0.7/api/batch_processing/data_preparation/manage_video_batch.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-02-02 00:50:45.480962 megadetector-5.0.7/api/batch_processing/integration/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-02-02 00:50:45.484962 megadetector-5.0.7/api/batch_processing/integration/digiKam/
--rw-rw-r--   0 user      (1000) user      (1000)      203 2023-05-20 21:19:48.000000 megadetector-5.0.7/api/batch_processing/integration/digiKam/setup.py
--rw-rw-r--   0 user      (1000) user      (1000)    17775 2023-05-20 21:19:48.000000 megadetector-5.0.7/api/batch_processing/integration/digiKam/xmp_integration.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-02-02 00:50:45.480962 megadetector-5.0.7/api/batch_processing/integration/eMammal/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-02-02 00:50:45.484962 megadetector-5.0.7/api/batch_processing/integration/eMammal/test_scripts/
--rw-rw-r--   0 user      (1000) user      (1000)       73 2023-05-20 21:19:48.000000 megadetector-5.0.7/api/batch_processing/integration/eMammal/test_scripts/config_template.py
--rw-rw-r--   0 user      (1000) user      (1000)     3608 2023-05-20 21:19:48.000000 megadetector-5.0.7/api/batch_processing/integration/eMammal/test_scripts/push_annotations_to_emammal.py
--rw-rw-r--   0 user      (1000) user      (1000)     1369 2023-05-20 21:19:48.000000 megadetector-5.0.7/api/batch_processing/integration/eMammal/test_scripts/select_images_for_testing.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-02-02 00:50:45.484962 megadetector-5.0.7/api/batch_processing/postprocessing/
--rw-rw-r--   0 user      (1000) user      (1000)     1530 2023-12-06 01:51:04.000000 megadetector-5.0.7/api/batch_processing/postprocessing/add_max_conf.py
--rw-rw-r--   0 user      (1000) user      (1000)     4877 2023-10-17 20:51:54.000000 megadetector-5.0.7/api/batch_processing/postprocessing/categorize_detections_by_size.py
--rw-rw-r--   0 user      (1000) user      (1000)     8233 2023-10-10 14:50:39.000000 megadetector-5.0.7/api/batch_processing/postprocessing/combine_api_outputs.py
--rw-rw-r--   0 user      (1000) user      (1000)    34652 2023-12-11 21:56:42.000000 megadetector-5.0.7/api/batch_processing/postprocessing/compare_batch_results.py
--rw-rw-r--   0 user      (1000) user      (1000)    12947 2023-10-10 14:50:39.000000 megadetector-5.0.7/api/batch_processing/postprocessing/convert_output_format.py
--rw-rw-r--   0 user      (1000) user      (1000)     6997 2023-12-28 01:45:41.000000 megadetector-5.0.7/api/batch_processing/postprocessing/load_api_results.py
--rw-rw-r--   0 user      (1000) user      (1000)    10139 2023-11-08 23:56:54.000000 megadetector-5.0.7/api/batch_processing/postprocessing/md_to_coco.py
--rw-rw-r--   0 user      (1000) user      (1000)     7075 2023-11-19 19:25:22.000000 megadetector-5.0.7/api/batch_processing/postprocessing/md_to_labelme.py
--rw-rw-r--   0 user      (1000) user      (1000)    15930 2023-09-22 20:29:38.000000 megadetector-5.0.7/api/batch_processing/postprocessing/merge_detections.py
--rw-rw-r--   0 user      (1000) user      (1000)    73653 2024-01-15 22:00:35.000000 megadetector-5.0.7/api/batch_processing/postprocessing/postprocess_batch_results.py
--rw-rw-r--   0 user      (1000) user      (1000)    25040 2023-12-03 17:33:08.000000 megadetector-5.0.7/api/batch_processing/postprocessing/render_detection_confusion_matrix.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-02-02 00:50:45.484962 megadetector-5.0.7/api/batch_processing/postprocessing/repeat_detection_elimination/
--rw-rw-r--   0 user      (1000) user      (1000)     9053 2024-01-28 18:41:58.000000 megadetector-5.0.7/api/batch_processing/postprocessing/repeat_detection_elimination/find_repeat_detections.py
--rw-rw-r--   0 user      (1000) user      (1000)     2189 2023-12-28 01:45:41.000000 megadetector-5.0.7/api/batch_processing/postprocessing/repeat_detection_elimination/remove_repeat_detections.py
--rw-rw-r--   0 user      (1000) user      (1000)    62882 2024-01-28 18:41:58.000000 megadetector-5.0.7/api/batch_processing/postprocessing/repeat_detection_elimination/repeat_detections_core.py
--rw-rw-r--   0 user      (1000) user      (1000)    28720 2023-10-02 01:42:03.000000 megadetector-5.0.7/api/batch_processing/postprocessing/separate_detections_into_folders.py
--rw-rw-r--   0 user      (1000) user      (1000)    26368 2024-02-02 00:27:22.000000 megadetector-5.0.7/api/batch_processing/postprocessing/subset_json_detector_output.py
--rw-rw-r--   0 user      (1000) user      (1000)     5476 2023-12-06 01:57:03.000000 megadetector-5.0.7/api/batch_processing/postprocessing/top_folders_to_bottom.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-02-02 00:50:45.480962 megadetector-5.0.7/api/synchronous/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-02-02 00:50:45.480962 megadetector-5.0.7/api/synchronous/api_core/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-02-02 00:50:45.484962 megadetector-5.0.7/api/synchronous/api_core/animal_detection_api/
--rw-rw-r--   0 user      (1000) user      (1000)     4934 2023-05-21 20:45:21.000000 megadetector-5.0.7/api/synchronous/api_core/animal_detection_api/api_backend.py
--rw-rw-r--   0 user      (1000) user      (1000)    10690 2023-05-21 20:45:21.000000 megadetector-5.0.7/api/synchronous/api_core/animal_detection_api/api_frontend.py
--rw-rw-r--   0 user      (1000) user      (1000)     1017 2023-05-20 21:19:48.000000 megadetector-5.0.7/api/synchronous/api_core/animal_detection_api/config.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-02-02 00:50:45.480962 megadetector-5.0.7/api/synchronous/api_core/animal_detection_api/data_management/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-02-02 00:50:45.484962 megadetector-5.0.7/api/synchronous/api_core/animal_detection_api/data_management/annotations/
--rw-r--r--   0 user      (1000) user      (1000)     1566 2023-10-10 14:44:28.000000 megadetector-5.0.7/api/synchronous/api_core/animal_detection_api/data_management/annotations/annotation_constants.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-02-02 00:50:45.484962 megadetector-5.0.7/api/synchronous/api_core/animal_detection_api/detection/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-02-02 00:50:45.484962 megadetector-5.0.7/api/synchronous/api_core/animal_detection_api/detection/detector_training/
--rw-rw-r--   0 user      (1000) user      (1000)     1091 2023-07-13 00:36:13.000000 megadetector-5.0.7/api/synchronous/api_core/animal_detection_api/detection/detector_training/copy_checkpoints.py
--rw-rw-r--   0 user      (1000) user      (1000)     4936 2023-05-20 21:19:48.000000 megadetector-5.0.7/api/synchronous/api_core/animal_detection_api/detection/detector_training/model_main_tf2.py
--rw-rw-r--   0 user      (1000) user      (1000)    22089 2023-09-22 21:33:40.000000 megadetector-5.0.7/api/synchronous/api_core/animal_detection_api/detection/process_video.py
--rw-rw-r--   0 user      (1000) user      (1000)    11505 2023-09-24 22:24:49.000000 megadetector-5.0.7/api/synchronous/api_core/animal_detection_api/detection/pytorch_detector.py
--rw-rw-r--   0 user      (1000) user      (1000)    23821 2023-09-24 22:27:02.000000 megadetector-5.0.7/api/synchronous/api_core/animal_detection_api/detection/run_detector.py
--rw-rw-r--   0 user      (1000) user      (1000)    41849 2023-11-08 23:08:09.000000 megadetector-5.0.7/api/synchronous/api_core/animal_detection_api/detection/run_detector_batch.py
--rw-rw-r--   0 user      (1000) user      (1000)    22118 2023-09-22 20:29:38.000000 megadetector-5.0.7/api/synchronous/api_core/animal_detection_api/detection/run_inference_with_yolov5_val.py
--rw-rw-r--   0 user      (1000) user      (1000)    28785 2023-09-02 21:43:14.000000 megadetector-5.0.7/api/synchronous/api_core/animal_detection_api/detection/run_tiled_inference.py
--rw-rw-r--   0 user      (1000) user      (1000)     6760 2023-09-22 20:29:38.000000 megadetector-5.0.7/api/synchronous/api_core/animal_detection_api/detection/tf_detector.py
--rw-rw-r--   0 user      (1000) user      (1000)    18317 2023-09-30 15:19:08.000000 megadetector-5.0.7/api/synchronous/api_core/animal_detection_api/detection/video_utils.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-02-02 00:50:45.488962 megadetector-5.0.7/api/synchronous/api_core/animal_detection_api/md_utils/
--rw-r--r--   0 user      (1000) user      (1000)     6243 2023-10-10 14:44:28.000000 megadetector-5.0.7/api/synchronous/api_core/animal_detection_api/md_utils/azure_utils.py
--rw-r--r--   0 user      (1000) user      (1000)     7600 2023-10-10 14:44:28.000000 megadetector-5.0.7/api/synchronous/api_core/animal_detection_api/md_utils/ct_utils.py
--rw-r--r--   0 user      (1000) user      (1000)     9598 2023-10-10 14:44:28.000000 megadetector-5.0.7/api/synchronous/api_core/animal_detection_api/md_utils/directory_listing.py
--rw-r--r--   0 user      (1000) user      (1000)     2005 2023-10-10 14:44:28.000000 megadetector-5.0.7/api/synchronous/api_core/animal_detection_api/md_utils/matlab_porting_tools.py
--rw-r--r--   0 user      (1000) user      (1000)    12397 2023-10-10 14:44:28.000000 megadetector-5.0.7/api/synchronous/api_core/animal_detection_api/md_utils/path_utils.py
--rw-r--r--   0 user      (1000) user      (1000)     3049 2023-10-10 14:44:28.000000 megadetector-5.0.7/api/synchronous/api_core/animal_detection_api/md_utils/process_utils.py
--rw-r--r--   0 user      (1000) user      (1000)    16955 2023-10-10 14:44:28.000000 megadetector-5.0.7/api/synchronous/api_core/animal_detection_api/md_utils/sas_blob_utils.py
--rw-r--r--   0 user      (1000) user      (1000)     1277 2023-10-10 14:44:28.000000 megadetector-5.0.7/api/synchronous/api_core/animal_detection_api/md_utils/string_utils.py
--rw-r--r--   0 user      (1000) user      (1000)     4598 2023-10-10 14:44:28.000000 megadetector-5.0.7/api/synchronous/api_core/animal_detection_api/md_utils/url_utils.py
--rw-r--r--   0 user      (1000) user      (1000)     7573 2023-10-10 14:44:28.000000 megadetector-5.0.7/api/synchronous/api_core/animal_detection_api/md_utils/write_html_image_list.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-02-02 00:50:45.488962 megadetector-5.0.7/api/synchronous/api_core/animal_detection_api/md_visualization/
--rw-r--r--   0 user      (1000) user      (1000)    31680 2023-10-10 14:44:28.000000 megadetector-5.0.7/api/synchronous/api_core/animal_detection_api/md_visualization/visualization_utils.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-02-02 00:50:45.488962 megadetector-5.0.7/api/synchronous/api_core/tests/
--rw-rw-r--   0 user      (1000) user      (1000)     3386 2023-05-20 21:19:48.000000 megadetector-5.0.7/api/synchronous/api_core/tests/load_test.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-02-02 00:50:45.488962 megadetector-5.0.7/classification/
--rw-rw-r--   0 user      (1000) user      (1000)     3488 2023-10-10 14:50:39.000000 megadetector-5.0.7/classification/aggregate_classifier_probs.py
--rw-rw-r--   0 user      (1000) user      (1000)     8463 2023-07-13 00:36:13.000000 megadetector-5.0.7/classification/analyze_failed_images.py
--rw-rw-r--   0 user      (1000) user      (1000)     6400 2023-07-13 00:36:13.000000 megadetector-5.0.7/classification/cache_batchapi_outputs.py
--rw-rw-r--   0 user      (1000) user      (1000)    25578 2023-07-13 00:36:13.000000 megadetector-5.0.7/classification/create_classification_dataset.py
--rw-rw-r--   0 user      (1000) user      (1000)    20510 2023-07-13 00:36:13.000000 megadetector-5.0.7/classification/crop_detections.py
--rw-rw-r--   0 user      (1000) user      (1000)     6088 2023-07-13 00:36:13.000000 megadetector-5.0.7/classification/csv_to_json.py
--rw-rw-r--   0 user      (1000) user      (1000)    37158 2023-07-13 00:36:13.000000 megadetector-5.0.7/classification/detect_and_crop.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-02-02 00:50:45.488962 megadetector-5.0.7/classification/efficientnet/
--rw-rw-r--   0 user      (1000) user      (1000)      182 2023-05-20 21:19:48.000000 megadetector-5.0.7/classification/efficientnet/__init__.py
--rwxrwxr-x   0 user      (1000) user      (1000)    17040 2023-05-20 21:19:48.000000 megadetector-5.0.7/classification/efficientnet/model.py
--rwxrwxr-x   0 user      (1000) user      (1000)    24846 2023-07-05 16:59:21.000000 megadetector-5.0.7/classification/efficientnet/utils.py
--rw-rw-r--   0 user      (1000) user      (1000)    19378 2023-07-13 00:36:13.000000 megadetector-5.0.7/classification/evaluate_model.py
--rw-rw-r--   0 user      (1000) user      (1000)     5111 2023-07-13 00:36:13.000000 megadetector-5.0.7/classification/identify_mislabeled_candidates.py
--rw-rw-r--   0 user      (1000) user      (1000)     1670 2023-07-13 00:36:13.000000 megadetector-5.0.7/classification/json_to_azcopy_list.py
--rw-rw-r--   0 user      (1000) user      (1000)    26618 2023-07-13 00:36:13.000000 megadetector-5.0.7/classification/json_validator.py
--rw-rw-r--   0 user      (1000) user      (1000)    10738 2023-07-13 00:36:13.000000 megadetector-5.0.7/classification/map_classification_categories.py
--rw-rw-r--   0 user      (1000) user      (1000)    20123 2023-09-22 20:28:52.000000 megadetector-5.0.7/classification/merge_classification_detection_output.py
--rw-rw-r--   0 user      (1000) user      (1000)     5952 2023-12-06 01:57:03.000000 megadetector-5.0.7/classification/prepare_classification_script.py
--rw-rw-r--   0 user      (1000) user      (1000)     7440 2023-07-13 00:36:13.000000 megadetector-5.0.7/classification/prepare_classification_script_mc.py
--rw-rw-r--   0 user      (1000) user      (1000)     9363 2023-07-13 00:36:13.000000 megadetector-5.0.7/classification/run_classifier.py
--rw-rw-r--   0 user      (1000) user      (1000)     3466 2023-07-13 00:36:13.000000 megadetector-5.0.7/classification/save_mislabeled.py
--rw-rw-r--   0 user      (1000) user      (1000)    32329 2023-07-13 00:36:13.000000 megadetector-5.0.7/classification/train_classifier.py
--rw-rw-r--   0 user      (1000) user      (1000)    28096 2023-07-13 00:36:13.000000 megadetector-5.0.7/classification/train_classifier_tf.py
--rw-rw-r--   0 user      (1000) user      (1000)    11355 2023-07-13 00:36:13.000000 megadetector-5.0.7/classification/train_utils.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-02-02 00:50:45.488962 megadetector-5.0.7/data_management/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-02-02 00:50:45.488962 megadetector-5.0.7/data_management/annotations/
--rw-rw-r--   0 user      (1000) user      (1000)     1566 2023-06-27 22:04:42.000000 megadetector-5.0.7/data_management/annotations/annotation_constants.py
--rw-rw-r--   0 user      (1000) user      (1000)     2416 2023-10-10 14:50:39.000000 megadetector-5.0.7/data_management/cct_json_to_filename_json.py
--rw-rw-r--   0 user      (1000) user      (1000)    12570 2023-06-27 22:00:52.000000 megadetector-5.0.7/data_management/cct_json_utils.py
--rw-rw-r--   0 user      (1000) user      (1000)     3859 2023-10-10 14:50:39.000000 megadetector-5.0.7/data_management/cct_to_csv.py
--rw-rw-r--   0 user      (1000) user      (1000)     4485 2023-08-19 17:11:37.000000 megadetector-5.0.7/data_management/cct_to_md.py
--rw-rw-r--   0 user      (1000) user      (1000)     8336 2023-05-22 23:05:38.000000 megadetector-5.0.7/data_management/cct_to_wi.py
--rw-rw-r--   0 user      (1000) user      (1000)    25880 2023-11-22 04:40:15.000000 megadetector-5.0.7/data_management/coco_to_yolo.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-02-02 00:50:45.488962 megadetector-5.0.7/data_management/databases/
--rw-rw-r--   0 user      (1000) user      (1000)      619 2023-06-27 21:58:14.000000 megadetector-5.0.7/data_management/databases/add_width_and_height_to_db.py
--rw-rw-r--   0 user      (1000) user      (1000)     6888 2023-10-10 14:50:39.000000 megadetector-5.0.7/data_management/databases/combine_coco_camera_traps_files.py
--rw-rw-r--   0 user      (1000) user      (1000)    14535 2024-01-28 21:41:10.000000 megadetector-5.0.7/data_management/databases/integrity_check_json_db.py
--rw-rw-r--   0 user      (1000) user      (1000)     6138 2023-10-10 14:50:39.000000 megadetector-5.0.7/data_management/databases/remove_corrupted_images_from_db.py
--rw-rw-r--   0 user      (1000) user      (1000)     2749 2023-10-10 14:50:39.000000 megadetector-5.0.7/data_management/databases/subset_json_db.py
--rw-rw-r--   0 user      (1000) user      (1000)     4283 2023-12-06 01:57:03.000000 megadetector-5.0.7/data_management/generate_crops_from_cct.py
--rw-rw-r--   0 user      (1000) user      (1000)     4220 2023-11-09 00:29:08.000000 megadetector-5.0.7/data_management/get_image_sizes.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-02-02 00:50:45.492962 megadetector-5.0.7/data_management/importers/
--rw-rw-r--   0 user      (1000) user      (1000)     1172 2023-09-21 01:58:08.000000 megadetector-5.0.7/data_management/importers/add_nacti_sizes.py
--rw-rw-r--   0 user      (1000) user      (1000)     2459 2023-11-05 20:26:38.000000 megadetector-5.0.7/data_management/importers/add_timestamps_to_icct.py
--rw-rw-r--   0 user      (1000) user      (1000)     4899 2023-12-06 01:47:11.000000 megadetector-5.0.7/data_management/importers/animl_results_to_md_results.py
--rw-rw-r--   0 user      (1000) user      (1000)    12910 2023-11-09 00:05:19.000000 megadetector-5.0.7/data_management/importers/auckland_doc_test_to_json.py
--rw-rw-r--   0 user      (1000) user      (1000)     5952 2023-11-08 23:59:23.000000 megadetector-5.0.7/data_management/importers/auckland_doc_to_json.py
--rw-rw-r--   0 user      (1000) user      (1000)     5307 2023-11-09 00:06:34.000000 megadetector-5.0.7/data_management/importers/awc_to_json.py
--rw-rw-r--   0 user      (1000) user      (1000)     7909 2023-11-09 00:06:34.000000 megadetector-5.0.7/data_management/importers/bellevue_to_json.py
--rw-rw-r--   0 user      (1000) user      (1000)    28621 2023-09-22 23:29:41.000000 megadetector-5.0.7/data_management/importers/cacophony-thermal-importer.py
--rw-rw-r--   0 user      (1000) user      (1000)     7827 2023-11-09 00:03:29.000000 megadetector-5.0.7/data_management/importers/carrizo_shrubfree_2018.py
--rw-rw-r--   0 user      (1000) user      (1000)     8830 2023-11-09 00:05:19.000000 megadetector-5.0.7/data_management/importers/carrizo_trail_cam_2017.py
--rw-rw-r--   0 user      (1000) user      (1000)     1351 2023-11-09 00:07:28.000000 megadetector-5.0.7/data_management/importers/cct_field_adjustments.py
--rw-rw-r--   0 user      (1000) user      (1000)    29483 2023-11-09 00:05:19.000000 megadetector-5.0.7/data_management/importers/channel_islands_to_cct.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-02-02 00:50:45.492962 megadetector-5.0.7/data_management/importers/eMammal/
--rw-rw-r--   0 user      (1000) user      (1000)     6080 2023-05-20 21:19:48.000000 megadetector-5.0.7/data_management/importers/eMammal/copy_and_unzip_emammal.py
--rw-rw-r--   0 user      (1000) user      (1000)     6838 2023-05-20 21:19:48.000000 megadetector-5.0.7/data_management/importers/eMammal/eMammal_helpers.py
--rw-rw-r--   0 user      (1000) user      (1000)     6987 2023-07-05 17:01:56.000000 megadetector-5.0.7/data_management/importers/eMammal/make_eMammal_json.py
--rw-rw-r--   0 user      (1000) user      (1000)     8248 2023-11-09 00:05:19.000000 megadetector-5.0.7/data_management/importers/ena24_to_json.py
--rw-rw-r--   0 user      (1000) user      (1000)    10526 2023-09-21 01:58:08.000000 megadetector-5.0.7/data_management/importers/filenames_to_json.py
--rw-rw-r--   0 user      (1000) user      (1000)     8701 2023-11-09 00:05:19.000000 megadetector-5.0.7/data_management/importers/helena_to_cct.py
--rw-rw-r--   0 user      (1000) user      (1000)    54058 2023-11-09 00:05:19.000000 megadetector-5.0.7/data_management/importers/idaho-camera-traps.py
--rw-rw-r--   0 user      (1000) user      (1000)     8166 2023-11-09 00:05:19.000000 megadetector-5.0.7/data_management/importers/idfg_iwildcam_lila_prep.py
--rw-rw-r--   0 user      (1000) user      (1000)     3730 2023-11-09 00:06:34.000000 megadetector-5.0.7/data_management/importers/jb_csv_to_json.py
--rw-rw-r--   0 user      (1000) user      (1000)     6718 2023-09-21 01:58:08.000000 megadetector-5.0.7/data_management/importers/mcgill_to_json.py
--rw-rw-r--   0 user      (1000) user      (1000)    14840 2023-11-09 00:01:34.000000 megadetector-5.0.7/data_management/importers/missouri_to_json.py
--rw-rw-r--   0 user      (1000) user      (1000)     2045 2023-09-21 01:58:08.000000 megadetector-5.0.7/data_management/importers/nacti_fieldname_adjustments.py
--rw-rw-r--   0 user      (1000) user      (1000)     5145 2023-12-06 01:45:31.000000 megadetector-5.0.7/data_management/importers/noaa_seals_2019.py
--rw-rw-r--   0 user      (1000) user      (1000)    10718 2023-11-09 00:06:34.000000 megadetector-5.0.7/data_management/importers/pc_to_json.py
--rw-rw-r--   0 user      (1000) user      (1000)     3787 2023-09-21 01:58:08.000000 megadetector-5.0.7/data_management/importers/plot_wni_giraffes.py
--rw-rw-r--   0 user      (1000) user      (1000)    12774 2023-11-08 23:59:39.000000 megadetector-5.0.7/data_management/importers/prepare-noaa-fish-data-for-lila.py
--rw-rw-r--   0 user      (1000) user      (1000)     3754 2023-11-09 00:06:34.000000 megadetector-5.0.7/data_management/importers/prepare_zsl_imerit.py
--rw-rw-r--   0 user      (1000) user      (1000)     9834 2023-11-09 00:07:41.000000 megadetector-5.0.7/data_management/importers/rspb_to_json.py
--rw-rw-r--   0 user      (1000) user      (1000)    10639 2023-11-09 00:05:19.000000 megadetector-5.0.7/data_management/importers/save_the_elephants_survey_A.py
--rw-rw-r--   0 user      (1000) user      (1000)    11167 2023-11-09 00:05:19.000000 megadetector-5.0.7/data_management/importers/save_the_elephants_survey_B.py
--rw-rw-r--   0 user      (1000) user      (1000)    23591 2023-11-09 00:06:52.000000 megadetector-5.0.7/data_management/importers/snapshot_safari_importer.py
--rw-rw-r--   0 user      (1000) user      (1000)    22996 2023-07-13 19:18:01.000000 megadetector-5.0.7/data_management/importers/snapshot_safari_importer_reprise.py
--rw-rw-r--   0 user      (1000) user      (1000)    33854 2023-11-09 00:07:01.000000 megadetector-5.0.7/data_management/importers/snapshot_serengeti_lila.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-02-02 00:50:45.492962 megadetector-5.0.7/data_management/importers/snapshotserengeti/
--rw-rw-r--   0 user      (1000) user      (1000)     4126 2023-05-20 21:19:48.000000 megadetector-5.0.7/data_management/importers/snapshotserengeti/make_full_SS_json.py
--rw-rw-r--   0 user      (1000) user      (1000)     4316 2023-05-20 21:19:48.000000 megadetector-5.0.7/data_management/importers/snapshotserengeti/make_per_season_SS_json.py
--rw-rw-r--   0 user      (1000) user      (1000)     2088 2023-09-21 01:58:08.000000 megadetector-5.0.7/data_management/importers/sulross_get_exif.py
--rw-rw-r--   0 user      (1000) user      (1000)    15902 2023-11-09 00:06:34.000000 megadetector-5.0.7/data_management/importers/timelapse_csv_set_to_json.py
--rw-rw-r--   0 user      (1000) user      (1000)    14869 2023-11-09 00:05:19.000000 megadetector-5.0.7/data_management/importers/ubc_to_json.py
--rw-rw-r--   0 user      (1000) user      (1000)    16177 2023-11-09 00:05:19.000000 megadetector-5.0.7/data_management/importers/umn_to_json.py
--rw-rw-r--   0 user      (1000) user      (1000)     7671 2023-11-08 23:58:56.000000 megadetector-5.0.7/data_management/importers/wellington_to_json.py
--rw-rw-r--   0 user      (1000) user      (1000)    13656 2023-11-09 00:00:11.000000 megadetector-5.0.7/data_management/importers/wi_to_json.py
--rw-rw-r--   0 user      (1000) user      (1000)     5594 2023-12-06 01:45:18.000000 megadetector-5.0.7/data_management/importers/zamba_results_to_md_results.py
--rw-rw-r--   0 user      (1000) user      (1000)    14204 2023-11-22 00:08:13.000000 megadetector-5.0.7/data_management/labelme_to_coco.py
--rw-rw-r--   0 user      (1000) user      (1000)     8480 2023-12-06 01:57:03.000000 megadetector-5.0.7/data_management/labelme_to_yolo.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-02-02 00:50:45.492962 megadetector-5.0.7/data_management/lila/
--rw-rw-r--   0 user      (1000) user      (1000)     2561 2023-11-08 23:58:29.000000 megadetector-5.0.7/data_management/lila/add_locations_to_island_camera_traps.py
--rw-rw-r--   0 user      (1000) user      (1000)     5017 2023-10-28 15:19:33.000000 megadetector-5.0.7/data_management/lila/add_locations_to_nacti.py
--rw-rw-r--   0 user      (1000) user      (1000)    16359 2024-02-01 03:02:05.000000 megadetector-5.0.7/data_management/lila/create_lila_blank_set.py
--rw-rw-r--   0 user      (1000) user      (1000)     4825 2023-12-31 18:59:10.000000 megadetector-5.0.7/data_management/lila/create_lila_test_set.py
--rw-rw-r--   0 user      (1000) user      (1000)     3916 2023-12-06 01:45:44.000000 megadetector-5.0.7/data_management/lila/create_links_to_md_results_files.py
--rw-rw-r--   0 user      (1000) user      (1000)     5283 2023-12-31 18:59:10.000000 megadetector-5.0.7/data_management/lila/download_lila_subset.py
--rw-rw-r--   0 user      (1000) user      (1000)    17351 2024-01-09 23:45:10.000000 megadetector-5.0.7/data_management/lila/generate_lila_per_image_labels.py
--rw-rw-r--   0 user      (1000) user      (1000)     5490 2023-12-31 18:59:10.000000 megadetector-5.0.7/data_management/lila/get_lila_annotation_counts.py
--rw-rw-r--   0 user      (1000) user      (1000)     3625 2023-06-26 23:52:53.000000 megadetector-5.0.7/data_management/lila/get_lila_image_counts.py
--rw-rw-r--   0 user      (1000) user      (1000)     8785 2023-12-31 18:59:10.000000 megadetector-5.0.7/data_management/lila/lila_common.py
--rw-rw-r--   0 user      (1000) user      (1000)     3966 2023-12-31 18:59:10.000000 megadetector-5.0.7/data_management/lila/test_lila_metadata_urls.py
--rw-rw-r--   0 user      (1000) user      (1000)    29920 2023-11-05 20:26:38.000000 megadetector-5.0.7/data_management/ocr_tools.py
--rw-rw-r--   0 user      (1000) user      (1000)    19036 2023-09-22 20:29:38.000000 megadetector-5.0.7/data_management/read_exif.py
--rw-rw-r--   0 user      (1000) user      (1000)     1555 2023-07-13 00:36:13.000000 megadetector-5.0.7/data_management/remove_exif.py
--rw-rw-r--   0 user      (1000) user      (1000)     7398 2024-01-28 21:56:47.000000 megadetector-5.0.7/data_management/resize_coco_dataset.py
--rw-rw-r--   0 user      (1000) user      (1000)    16313 2024-01-28 18:41:58.000000 megadetector-5.0.7/data_management/yolo_output_to_md_output.py
--rw-rw-r--   0 user      (1000) user      (1000)     8078 2023-12-03 16:04:00.000000 megadetector-5.0.7/data_management/yolo_to_coco.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-02-02 00:50:45.492962 megadetector-5.0.7/detection/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-02-02 00:50:45.496962 megadetector-5.0.7/detection/detector_training/
--rw-rw-r--   0 user      (1000) user      (1000)     1091 2023-07-13 00:36:13.000000 megadetector-5.0.7/detection/detector_training/copy_checkpoints.py
--rw-rw-r--   0 user      (1000) user      (1000)     4936 2023-05-20 21:19:48.000000 megadetector-5.0.7/detection/detector_training/model_main_tf2.py
--rw-rw-r--   0 user      (1000) user      (1000)    26825 2024-02-02 00:27:22.000000 megadetector-5.0.7/detection/process_video.py
--rw-rw-r--   0 user      (1000) user      (1000)    11992 2024-01-28 18:41:58.000000 megadetector-5.0.7/detection/pytorch_detector.py
--rw-rw-r--   0 user      (1000) user      (1000)    26036 2023-12-21 01:23:34.000000 megadetector-5.0.7/detection/run_detector.py
--rw-rw-r--   0 user      (1000) user      (1000)    46937 2024-01-28 18:41:58.000000 megadetector-5.0.7/detection/run_detector_batch.py
--rw-rw-r--   0 user      (1000) user      (1000)    33755 2024-02-02 00:27:22.000000 megadetector-5.0.7/detection/run_inference_with_yolov5_val.py
--rw-rw-r--   0 user      (1000) user      (1000)    33930 2024-02-02 00:27:22.000000 megadetector-5.0.7/detection/run_tiled_inference.py
--rw-rw-r--   0 user      (1000) user      (1000)     6760 2023-09-22 20:29:38.000000 megadetector-5.0.7/detection/tf_detector.py
--rw-rw-r--   0 user      (1000) user      (1000)    19425 2023-11-22 01:36:35.000000 megadetector-5.0.7/detection/video_utils.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-02-02 00:50:45.496962 megadetector-5.0.7/md_utils/
--rw-rw-r--   0 user      (1000) user      (1000)     6243 2023-05-22 23:02:57.000000 megadetector-5.0.7/md_utils/azure_utils.py
--rw-rw-r--   0 user      (1000) user      (1000)    12908 2023-12-10 19:18:44.000000 megadetector-5.0.7/md_utils/ct_utils.py
--rw-rw-r--   0 user      (1000) user      (1000)     9615 2023-10-10 14:50:39.000000 megadetector-5.0.7/md_utils/directory_listing.py
--rw-rw-r--   0 user      (1000) user      (1000)    33316 2024-02-02 00:27:22.000000 megadetector-5.0.7/md_utils/md_tests.py
--rw-rw-r--   0 user      (1000) user      (1000)    16573 2024-01-28 18:41:58.000000 megadetector-5.0.7/md_utils/path_utils.py
--rw-rw-r--   0 user      (1000) user      (1000)     4316 2024-01-28 18:41:58.000000 megadetector-5.0.7/md_utils/process_utils.py
--rw-rw-r--   0 user      (1000) user      (1000)    16955 2023-07-05 17:03:19.000000 megadetector-5.0.7/md_utils/sas_blob_utils.py
--rw-rw-r--   0 user      (1000) user      (1000)     9241 2023-11-22 03:22:33.000000 megadetector-5.0.7/md_utils/split_locations_into_train_val.py
--rw-rw-r--   0 user      (1000) user      (1000)     1600 2024-02-02 00:27:22.000000 megadetector-5.0.7/md_utils/string_utils.py
--rw-rw-r--   0 user      (1000) user      (1000)     4593 2023-12-06 01:59:00.000000 megadetector-5.0.7/md_utils/url_utils.py
--rw-rw-r--   0 user      (1000) user      (1000)     7036 2023-12-02 19:45:09.000000 megadetector-5.0.7/md_utils/write_html_image_list.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-02-02 00:50:45.496962 megadetector-5.0.7/md_visualization/
--rw-rw-r--   0 user      (1000) user      (1000)    10712 2023-10-25 02:02:08.000000 megadetector-5.0.7/md_visualization/plot_utils.py
--rw-rw-r--   0 user      (1000) user      (1000)    10391 2023-07-05 17:03:56.000000 megadetector-5.0.7/md_visualization/render_images_with_thumbnails.py
--rw-rw-r--   0 user      (1000) user      (1000)    35297 2024-01-28 18:41:58.000000 megadetector-5.0.7/md_visualization/visualization_utils.py
--rw-rw-r--   0 user      (1000) user      (1000)    18931 2023-12-06 01:44:58.000000 megadetector-5.0.7/md_visualization/visualize_db.py
--rw-rw-r--   0 user      (1000) user      (1000)    15814 2024-01-13 01:05:31.000000 megadetector-5.0.7/md_visualization/visualize_detector_output.py
--rw-rw-r--   0 user      (1000) user      (1000)     6188 2023-07-13 00:36:13.000000 megadetector-5.0.7/md_visualization/visualize_megadb.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-02-02 00:50:45.496962 megadetector-5.0.7/megadetector.egg-info/
--rw-r--r--   0 user      (1000) user      (1000)     7503 2024-02-02 00:50:45.000000 megadetector-5.0.7/megadetector.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)    10157 2024-02-02 00:50:45.000000 megadetector-5.0.7/megadetector.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2024-02-02 00:50:45.000000 megadetector-5.0.7/megadetector.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)      238 2024-02-02 00:50:45.000000 megadetector-5.0.7/megadetector.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)      101 2024-02-02 00:50:45.000000 megadetector-5.0.7/megadetector.egg-info/top_level.txt
--rw-rw-r--   0 user      (1000) user      (1000)     1688 2024-02-02 00:49:41.000000 megadetector-5.0.7/pyproject.toml
--rw-rw-r--   0 user      (1000) user      (1000)       38 2024-02-02 00:50:45.496962 megadetector-5.0.7/setup.cfg
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-02-02 00:50:45.496962 megadetector-5.0.7/taxonomy_mapping/
--rw-rw-r--   0 user      (1000) user      (1000)    16517 2023-12-06 01:57:03.000000 megadetector-5.0.7/taxonomy_mapping/map_lila_taxonomy_to_wi_taxonomy.py
--rw-rw-r--   0 user      (1000) user      (1000)     4324 2024-01-09 23:45:10.000000 megadetector-5.0.7/taxonomy_mapping/map_new_lila_datasets.py
--rw-rw-r--   0 user      (1000) user      (1000)     4357 2024-01-09 23:45:10.000000 megadetector-5.0.7/taxonomy_mapping/prepare_lila_taxonomy_release.py
--rw-rw-r--   0 user      (1000) user      (1000)    20144 2023-12-31 18:59:10.000000 megadetector-5.0.7/taxonomy_mapping/preview_lila_taxonomy.py
--rw-rw-r--   0 user      (1000) user      (1000)     1992 2023-06-26 19:00:42.000000 megadetector-5.0.7/taxonomy_mapping/retrieve_sample_image.py
--rw-rw-r--   0 user      (1000) user      (1000)     6874 2023-07-05 17:04:26.000000 megadetector-5.0.7/taxonomy_mapping/simple_image_download.py
--rw-rw-r--   0 user      (1000) user      (1000)    28303 2023-12-31 18:59:10.000000 megadetector-5.0.7/taxonomy_mapping/species_lookup.py
--rw-rw-r--   0 user      (1000) user      (1000)     4874 2023-12-31 18:59:10.000000 megadetector-5.0.7/taxonomy_mapping/taxonomy_csv_checker.py
--rw-rw-r--   0 user      (1000) user      (1000)    12361 2023-07-13 00:36:13.000000 megadetector-5.0.7/taxonomy_mapping/taxonomy_graph.py
--rw-rw-r--   0 user      (1000) user      (1000)     2314 2023-06-26 17:52:32.000000 megadetector-5.0.7/taxonomy_mapping/validate_lila_category_mappings.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-19 23:55:36.236348 megadetector-5.0.8/
+-rw-rw-r--   0 user      (1000) user      (1000)     1100 2023-05-22 23:49:44.000000 megadetector-5.0.8/LICENSE
+-rw-r--r--   0 user      (1000) user      (1000)     7373 2024-04-19 23:55:36.236348 megadetector-5.0.8/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)     4811 2024-04-19 23:54:16.000000 megadetector-5.0.8/README-package.md
+-rw-rw-r--   0 user      (1000) user      (1000)    20819 2024-04-19 23:54:16.000000 megadetector-5.0.8/README.md
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-19 23:55:36.220348 megadetector-5.0.8/api/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-19 23:55:36.220348 megadetector-5.0.8/api/batch_processing/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-19 23:55:36.220348 megadetector-5.0.8/api/batch_processing/api_core/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-19 23:55:36.220348 megadetector-5.0.8/api/batch_processing/api_core/batch_service/
+-rw-rw-r--   0 user      (1000) user      (1000)    17347 2023-05-21 20:45:21.000000 megadetector-5.0.8/api/batch_processing/api_core/batch_service/score.py
+-rw-rw-r--   0 user      (1000) user      (1000)    11668 2023-05-21 18:12:32.000000 megadetector-5.0.8/api/batch_processing/api_core/server.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3318 2023-05-20 21:19:48.000000 megadetector-5.0.8/api/batch_processing/api_core/server_api_config.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1860 2023-05-20 21:19:48.000000 megadetector-5.0.8/api/batch_processing/api_core/server_app_config.py
+-rw-rw-r--   0 user      (1000) user      (1000)    10324 2023-05-21 18:12:32.000000 megadetector-5.0.8/api/batch_processing/api_core/server_batch_job_manager.py
+-rw-rw-r--   0 user      (1000) user      (1000)     6240 2023-05-20 21:19:48.000000 megadetector-5.0.8/api/batch_processing/api_core/server_job_status_table.py
+-rw-rw-r--   0 user      (1000) user      (1000)    17003 2023-05-21 18:12:32.000000 megadetector-5.0.8/api/batch_processing/api_core/server_orchestration.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3314 2023-05-21 18:12:32.000000 megadetector-5.0.8/api/batch_processing/api_core/server_utils.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-19 23:55:36.220348 megadetector-5.0.8/api/batch_processing/api_core_support/
+-rw-rw-r--   0 user      (1000) user      (1000)     2275 2023-05-20 21:19:48.000000 megadetector-5.0.8/api/batch_processing/api_core_support/aggregate_results_manually.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-19 23:55:36.220348 megadetector-5.0.8/api/batch_processing/api_support/
+-rw-rw-r--   0 user      (1000) user      (1000)     5383 2023-05-20 21:19:48.000000 megadetector-5.0.8/api/batch_processing/api_support/summarize_daily_activity.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-19 23:55:36.220348 megadetector-5.0.8/api/batch_processing/data_preparation/
+-rw-rw-r--   0 user      (1000) user      (1000)    89186 2024-03-31 18:21:07.000000 megadetector-5.0.8/api/batch_processing/data_preparation/manage_local_batch.py
+-rw-rw-r--   0 user      (1000) user      (1000)     9668 2024-01-28 18:41:58.000000 megadetector-5.0.8/api/batch_processing/data_preparation/manage_video_batch.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-19 23:55:36.220348 megadetector-5.0.8/api/batch_processing/integration/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-19 23:55:36.224348 megadetector-5.0.8/api/batch_processing/integration/digiKam/
+-rw-rw-r--   0 user      (1000) user      (1000)      203 2023-05-20 21:19:48.000000 megadetector-5.0.8/api/batch_processing/integration/digiKam/setup.py
+-rw-rw-r--   0 user      (1000) user      (1000)    17775 2023-05-20 21:19:48.000000 megadetector-5.0.8/api/batch_processing/integration/digiKam/xmp_integration.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-19 23:55:36.220348 megadetector-5.0.8/api/batch_processing/integration/eMammal/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-19 23:55:36.224348 megadetector-5.0.8/api/batch_processing/integration/eMammal/test_scripts/
+-rw-rw-r--   0 user      (1000) user      (1000)       73 2023-05-20 21:19:48.000000 megadetector-5.0.8/api/batch_processing/integration/eMammal/test_scripts/config_template.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3608 2023-05-20 21:19:48.000000 megadetector-5.0.8/api/batch_processing/integration/eMammal/test_scripts/push_annotations_to_emammal.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1369 2023-05-20 21:19:48.000000 megadetector-5.0.8/api/batch_processing/integration/eMammal/test_scripts/select_images_for_testing.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-19 23:55:36.224348 megadetector-5.0.8/api/batch_processing/postprocessing/
+-rw-rw-r--   0 user      (1000) user      (1000)     1530 2023-12-06 01:51:04.000000 megadetector-5.0.8/api/batch_processing/postprocessing/add_max_conf.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4877 2023-10-17 20:51:54.000000 megadetector-5.0.8/api/batch_processing/postprocessing/categorize_detections_by_size.py
+-rw-rw-r--   0 user      (1000) user      (1000)     8237 2024-03-18 22:03:38.000000 megadetector-5.0.8/api/batch_processing/postprocessing/combine_api_outputs.py
+-rw-rw-r--   0 user      (1000) user      (1000)    34652 2024-02-25 01:09:49.000000 megadetector-5.0.8/api/batch_processing/postprocessing/compare_batch_results.py
+-rw-rw-r--   0 user      (1000) user      (1000)    13600 2024-04-09 13:56:32.000000 megadetector-5.0.8/api/batch_processing/postprocessing/convert_output_format.py
+-rw-rw-r--   0 user      (1000) user      (1000)     6895 2024-03-09 00:34:45.000000 megadetector-5.0.8/api/batch_processing/postprocessing/load_api_results.py
+-rw-rw-r--   0 user      (1000) user      (1000)    10139 2023-11-08 23:56:54.000000 megadetector-5.0.8/api/batch_processing/postprocessing/md_to_coco.py
+-rw-rw-r--   0 user      (1000) user      (1000)     9779 2024-03-31 18:21:07.000000 megadetector-5.0.8/api/batch_processing/postprocessing/md_to_labelme.py
+-rw-rw-r--   0 user      (1000) user      (1000)    17192 2024-03-18 22:03:38.000000 megadetector-5.0.8/api/batch_processing/postprocessing/merge_detections.py
+-rw-rw-r--   0 user      (1000) user      (1000)    74165 2024-03-19 20:27:38.000000 megadetector-5.0.8/api/batch_processing/postprocessing/postprocess_batch_results.py
+-rw-rw-r--   0 user      (1000) user      (1000)     6042 2024-04-19 23:54:16.000000 megadetector-5.0.8/api/batch_processing/postprocessing/remap_detection_categories.py
+-rw-rw-r--   0 user      (1000) user      (1000)    25047 2024-02-25 02:14:50.000000 megadetector-5.0.8/api/batch_processing/postprocessing/render_detection_confusion_matrix.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-19 23:55:36.224348 megadetector-5.0.8/api/batch_processing/postprocessing/repeat_detection_elimination/
+-rw-rw-r--   0 user      (1000) user      (1000)     9053 2024-01-28 18:41:58.000000 megadetector-5.0.8/api/batch_processing/postprocessing/repeat_detection_elimination/find_repeat_detections.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2189 2023-12-28 01:45:41.000000 megadetector-5.0.8/api/batch_processing/postprocessing/repeat_detection_elimination/remove_repeat_detections.py
+-rw-rw-r--   0 user      (1000) user      (1000)    62880 2024-03-31 18:21:07.000000 megadetector-5.0.8/api/batch_processing/postprocessing/repeat_detection_elimination/repeat_detections_core.py
+-rw-rw-r--   0 user      (1000) user      (1000)    28720 2023-10-02 01:42:03.000000 megadetector-5.0.8/api/batch_processing/postprocessing/separate_detections_into_folders.py
+-rw-rw-r--   0 user      (1000) user      (1000)    26368 2024-02-02 00:27:22.000000 megadetector-5.0.8/api/batch_processing/postprocessing/subset_json_detector_output.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5476 2023-12-06 01:57:03.000000 megadetector-5.0.8/api/batch_processing/postprocessing/top_folders_to_bottom.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-19 23:55:36.220348 megadetector-5.0.8/api/synchronous/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-19 23:55:36.220348 megadetector-5.0.8/api/synchronous/api_core/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-19 23:55:36.224348 megadetector-5.0.8/api/synchronous/api_core/animal_detection_api/
+-rw-rw-r--   0 user      (1000) user      (1000)     4934 2023-05-21 20:45:21.000000 megadetector-5.0.8/api/synchronous/api_core/animal_detection_api/api_backend.py
+-rw-rw-r--   0 user      (1000) user      (1000)    10690 2023-05-21 20:45:21.000000 megadetector-5.0.8/api/synchronous/api_core/animal_detection_api/api_frontend.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1017 2023-05-20 21:19:48.000000 megadetector-5.0.8/api/synchronous/api_core/animal_detection_api/config.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-19 23:55:36.220348 megadetector-5.0.8/api/synchronous/api_core/animal_detection_api/data_management/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-19 23:55:36.224348 megadetector-5.0.8/api/synchronous/api_core/animal_detection_api/data_management/annotations/
+-rw-r--r--   0 user      (1000) user      (1000)     1566 2023-10-10 14:44:28.000000 megadetector-5.0.8/api/synchronous/api_core/animal_detection_api/data_management/annotations/annotation_constants.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-19 23:55:36.224348 megadetector-5.0.8/api/synchronous/api_core/animal_detection_api/detection/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-19 23:55:36.224348 megadetector-5.0.8/api/synchronous/api_core/animal_detection_api/detection/detector_training/
+-rw-rw-r--   0 user      (1000) user      (1000)     1091 2023-07-13 00:36:13.000000 megadetector-5.0.8/api/synchronous/api_core/animal_detection_api/detection/detector_training/copy_checkpoints.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4936 2023-05-20 21:19:48.000000 megadetector-5.0.8/api/synchronous/api_core/animal_detection_api/detection/detector_training/model_main_tf2.py
+-rw-rw-r--   0 user      (1000) user      (1000)    22089 2023-09-22 21:33:40.000000 megadetector-5.0.8/api/synchronous/api_core/animal_detection_api/detection/process_video.py
+-rw-rw-r--   0 user      (1000) user      (1000)    11505 2023-09-24 22:24:49.000000 megadetector-5.0.8/api/synchronous/api_core/animal_detection_api/detection/pytorch_detector.py
+-rw-rw-r--   0 user      (1000) user      (1000)    23821 2023-09-24 22:27:02.000000 megadetector-5.0.8/api/synchronous/api_core/animal_detection_api/detection/run_detector.py
+-rw-rw-r--   0 user      (1000) user      (1000)    41849 2023-11-08 23:08:09.000000 megadetector-5.0.8/api/synchronous/api_core/animal_detection_api/detection/run_detector_batch.py
+-rw-rw-r--   0 user      (1000) user      (1000)    22118 2023-09-22 20:29:38.000000 megadetector-5.0.8/api/synchronous/api_core/animal_detection_api/detection/run_inference_with_yolov5_val.py
+-rw-rw-r--   0 user      (1000) user      (1000)    28785 2023-09-02 21:43:14.000000 megadetector-5.0.8/api/synchronous/api_core/animal_detection_api/detection/run_tiled_inference.py
+-rw-rw-r--   0 user      (1000) user      (1000)     6760 2023-09-22 20:29:38.000000 megadetector-5.0.8/api/synchronous/api_core/animal_detection_api/detection/tf_detector.py
+-rw-rw-r--   0 user      (1000) user      (1000)    18317 2023-09-30 15:19:08.000000 megadetector-5.0.8/api/synchronous/api_core/animal_detection_api/detection/video_utils.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-19 23:55:36.224348 megadetector-5.0.8/api/synchronous/api_core/animal_detection_api/md_utils/
+-rw-r--r--   0 user      (1000) user      (1000)     6243 2023-10-10 14:44:28.000000 megadetector-5.0.8/api/synchronous/api_core/animal_detection_api/md_utils/azure_utils.py
+-rw-r--r--   0 user      (1000) user      (1000)     7600 2023-10-10 14:44:28.000000 megadetector-5.0.8/api/synchronous/api_core/animal_detection_api/md_utils/ct_utils.py
+-rw-r--r--   0 user      (1000) user      (1000)     9598 2023-10-10 14:44:28.000000 megadetector-5.0.8/api/synchronous/api_core/animal_detection_api/md_utils/directory_listing.py
+-rw-r--r--   0 user      (1000) user      (1000)     2005 2023-10-10 14:44:28.000000 megadetector-5.0.8/api/synchronous/api_core/animal_detection_api/md_utils/matlab_porting_tools.py
+-rw-r--r--   0 user      (1000) user      (1000)    12397 2023-10-10 14:44:28.000000 megadetector-5.0.8/api/synchronous/api_core/animal_detection_api/md_utils/path_utils.py
+-rw-r--r--   0 user      (1000) user      (1000)     3049 2023-10-10 14:44:28.000000 megadetector-5.0.8/api/synchronous/api_core/animal_detection_api/md_utils/process_utils.py
+-rw-r--r--   0 user      (1000) user      (1000)    16955 2023-10-10 14:44:28.000000 megadetector-5.0.8/api/synchronous/api_core/animal_detection_api/md_utils/sas_blob_utils.py
+-rw-r--r--   0 user      (1000) user      (1000)     1277 2023-10-10 14:44:28.000000 megadetector-5.0.8/api/synchronous/api_core/animal_detection_api/md_utils/string_utils.py
+-rw-r--r--   0 user      (1000) user      (1000)     4598 2023-10-10 14:44:28.000000 megadetector-5.0.8/api/synchronous/api_core/animal_detection_api/md_utils/url_utils.py
+-rw-r--r--   0 user      (1000) user      (1000)     7573 2023-10-10 14:44:28.000000 megadetector-5.0.8/api/synchronous/api_core/animal_detection_api/md_utils/write_html_image_list.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-19 23:55:36.224348 megadetector-5.0.8/api/synchronous/api_core/animal_detection_api/md_visualization/
+-rw-r--r--   0 user      (1000) user      (1000)    31680 2023-10-10 14:44:28.000000 megadetector-5.0.8/api/synchronous/api_core/animal_detection_api/md_visualization/visualization_utils.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-19 23:55:36.224348 megadetector-5.0.8/api/synchronous/api_core/tests/
+-rw-rw-r--   0 user      (1000) user      (1000)     3386 2023-05-20 21:19:48.000000 megadetector-5.0.8/api/synchronous/api_core/tests/load_test.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-19 23:55:36.228348 megadetector-5.0.8/classification/
+-rw-rw-r--   0 user      (1000) user      (1000)     3488 2023-10-10 14:50:39.000000 megadetector-5.0.8/classification/aggregate_classifier_probs.py
+-rw-rw-r--   0 user      (1000) user      (1000)     8463 2023-07-13 00:36:13.000000 megadetector-5.0.8/classification/analyze_failed_images.py
+-rw-rw-r--   0 user      (1000) user      (1000)     6400 2023-07-13 00:36:13.000000 megadetector-5.0.8/classification/cache_batchapi_outputs.py
+-rw-rw-r--   0 user      (1000) user      (1000)    25578 2023-07-13 00:36:13.000000 megadetector-5.0.8/classification/create_classification_dataset.py
+-rw-rw-r--   0 user      (1000) user      (1000)    20510 2023-07-13 00:36:13.000000 megadetector-5.0.8/classification/crop_detections.py
+-rw-rw-r--   0 user      (1000) user      (1000)     6088 2023-07-13 00:36:13.000000 megadetector-5.0.8/classification/csv_to_json.py
+-rw-rw-r--   0 user      (1000) user      (1000)    37158 2023-07-13 00:36:13.000000 megadetector-5.0.8/classification/detect_and_crop.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-19 23:55:36.228348 megadetector-5.0.8/classification/efficientnet/
+-rw-rw-r--   0 user      (1000) user      (1000)      182 2023-05-20 21:19:48.000000 megadetector-5.0.8/classification/efficientnet/__init__.py
+-rwxrwxr-x   0 user      (1000) user      (1000)    17040 2023-05-20 21:19:48.000000 megadetector-5.0.8/classification/efficientnet/model.py
+-rwxrwxr-x   0 user      (1000) user      (1000)    24846 2023-07-05 16:59:21.000000 megadetector-5.0.8/classification/efficientnet/utils.py
+-rw-rw-r--   0 user      (1000) user      (1000)    19378 2023-07-13 00:36:13.000000 megadetector-5.0.8/classification/evaluate_model.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5111 2023-07-13 00:36:13.000000 megadetector-5.0.8/classification/identify_mislabeled_candidates.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1670 2023-07-13 00:36:13.000000 megadetector-5.0.8/classification/json_to_azcopy_list.py
+-rw-rw-r--   0 user      (1000) user      (1000)    26618 2023-07-13 00:36:13.000000 megadetector-5.0.8/classification/json_validator.py
+-rw-rw-r--   0 user      (1000) user      (1000)    10738 2023-07-13 00:36:13.000000 megadetector-5.0.8/classification/map_classification_categories.py
+-rw-rw-r--   0 user      (1000) user      (1000)    20123 2023-09-22 20:28:52.000000 megadetector-5.0.8/classification/merge_classification_detection_output.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5952 2023-12-06 01:57:03.000000 megadetector-5.0.8/classification/prepare_classification_script.py
+-rw-rw-r--   0 user      (1000) user      (1000)     7440 2023-07-13 00:36:13.000000 megadetector-5.0.8/classification/prepare_classification_script_mc.py
+-rw-rw-r--   0 user      (1000) user      (1000)     9363 2023-07-13 00:36:13.000000 megadetector-5.0.8/classification/run_classifier.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3466 2023-07-13 00:36:13.000000 megadetector-5.0.8/classification/save_mislabeled.py
+-rw-rw-r--   0 user      (1000) user      (1000)    32329 2023-07-13 00:36:13.000000 megadetector-5.0.8/classification/train_classifier.py
+-rw-rw-r--   0 user      (1000) user      (1000)    28096 2023-07-13 00:36:13.000000 megadetector-5.0.8/classification/train_classifier_tf.py
+-rw-rw-r--   0 user      (1000) user      (1000)    11355 2023-07-13 00:36:13.000000 megadetector-5.0.8/classification/train_utils.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-19 23:55:36.228348 megadetector-5.0.8/data_management/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-19 23:55:36.228348 megadetector-5.0.8/data_management/annotations/
+-rw-rw-r--   0 user      (1000) user      (1000)     1566 2023-06-27 22:04:42.000000 megadetector-5.0.8/data_management/annotations/annotation_constants.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2416 2023-10-10 14:50:39.000000 megadetector-5.0.8/data_management/cct_json_to_filename_json.py
+-rw-rw-r--   0 user      (1000) user      (1000)    12767 2024-03-09 00:34:45.000000 megadetector-5.0.8/data_management/cct_json_utils.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3859 2023-10-10 14:50:39.000000 megadetector-5.0.8/data_management/cct_to_csv.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4485 2023-08-19 17:11:37.000000 megadetector-5.0.8/data_management/cct_to_md.py
+-rw-rw-r--   0 user      (1000) user      (1000)     8336 2023-05-22 23:05:38.000000 megadetector-5.0.8/data_management/cct_to_wi.py
+-rw-rw-r--   0 user      (1000) user      (1000)     8077 2024-04-19 23:54:16.000000 megadetector-5.0.8/data_management/coco_to_labelme.py
+-rw-rw-r--   0 user      (1000) user      (1000)    26042 2024-02-05 18:22:23.000000 megadetector-5.0.8/data_management/coco_to_yolo.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-19 23:55:36.228348 megadetector-5.0.8/data_management/databases/
+-rw-rw-r--   0 user      (1000) user      (1000)      619 2023-06-27 21:58:14.000000 megadetector-5.0.8/data_management/databases/add_width_and_height_to_db.py
+-rw-rw-r--   0 user      (1000) user      (1000)     6888 2023-10-10 14:50:39.000000 megadetector-5.0.8/data_management/databases/combine_coco_camera_traps_files.py
+-rw-rw-r--   0 user      (1000) user      (1000)    14887 2024-04-19 23:54:16.000000 megadetector-5.0.8/data_management/databases/integrity_check_json_db.py
+-rw-rw-r--   0 user      (1000) user      (1000)     6138 2023-10-10 14:50:39.000000 megadetector-5.0.8/data_management/databases/remove_corrupted_images_from_db.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2749 2024-03-18 22:03:38.000000 megadetector-5.0.8/data_management/databases/subset_json_db.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4283 2023-12-06 01:57:03.000000 megadetector-5.0.8/data_management/generate_crops_from_cct.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4961 2024-04-19 23:54:16.000000 megadetector-5.0.8/data_management/get_image_sizes.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-19 23:55:36.232348 megadetector-5.0.8/data_management/importers/
+-rw-rw-r--   0 user      (1000) user      (1000)     1172 2023-09-21 01:58:08.000000 megadetector-5.0.8/data_management/importers/add_nacti_sizes.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2459 2023-11-05 20:26:38.000000 megadetector-5.0.8/data_management/importers/add_timestamps_to_icct.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4884 2024-03-18 22:03:38.000000 megadetector-5.0.8/data_management/importers/animl_results_to_md_results.py
+-rw-rw-r--   0 user      (1000) user      (1000)    12910 2023-11-09 00:05:19.000000 megadetector-5.0.8/data_management/importers/auckland_doc_test_to_json.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5952 2023-11-08 23:59:23.000000 megadetector-5.0.8/data_management/importers/auckland_doc_to_json.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5307 2023-11-09 00:06:34.000000 megadetector-5.0.8/data_management/importers/awc_to_json.py
+-rw-rw-r--   0 user      (1000) user      (1000)     7909 2023-11-09 00:06:34.000000 megadetector-5.0.8/data_management/importers/bellevue_to_json.py
+-rw-rw-r--   0 user      (1000) user      (1000)    28621 2023-09-22 23:29:41.000000 megadetector-5.0.8/data_management/importers/cacophony-thermal-importer.py
+-rw-rw-r--   0 user      (1000) user      (1000)     7827 2023-11-09 00:03:29.000000 megadetector-5.0.8/data_management/importers/carrizo_shrubfree_2018.py
+-rw-rw-r--   0 user      (1000) user      (1000)     8830 2023-11-09 00:05:19.000000 megadetector-5.0.8/data_management/importers/carrizo_trail_cam_2017.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1351 2023-11-09 00:07:28.000000 megadetector-5.0.8/data_management/importers/cct_field_adjustments.py
+-rw-rw-r--   0 user      (1000) user      (1000)    29483 2023-11-09 00:05:19.000000 megadetector-5.0.8/data_management/importers/channel_islands_to_cct.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-19 23:55:36.232348 megadetector-5.0.8/data_management/importers/eMammal/
+-rw-rw-r--   0 user      (1000) user      (1000)     6080 2023-05-20 21:19:48.000000 megadetector-5.0.8/data_management/importers/eMammal/copy_and_unzip_emammal.py
+-rw-rw-r--   0 user      (1000) user      (1000)     6838 2023-05-20 21:19:48.000000 megadetector-5.0.8/data_management/importers/eMammal/eMammal_helpers.py
+-rw-rw-r--   0 user      (1000) user      (1000)     6987 2023-07-05 17:01:56.000000 megadetector-5.0.8/data_management/importers/eMammal/make_eMammal_json.py
+-rw-rw-r--   0 user      (1000) user      (1000)     8248 2023-11-09 00:05:19.000000 megadetector-5.0.8/data_management/importers/ena24_to_json.py
+-rw-rw-r--   0 user      (1000) user      (1000)    10526 2023-09-21 01:58:08.000000 megadetector-5.0.8/data_management/importers/filenames_to_json.py
+-rw-rw-r--   0 user      (1000) user      (1000)     8701 2023-11-09 00:05:19.000000 megadetector-5.0.8/data_management/importers/helena_to_cct.py
+-rw-rw-r--   0 user      (1000) user      (1000)    54058 2023-11-09 00:05:19.000000 megadetector-5.0.8/data_management/importers/idaho-camera-traps.py
+-rw-rw-r--   0 user      (1000) user      (1000)     8166 2023-11-09 00:05:19.000000 megadetector-5.0.8/data_management/importers/idfg_iwildcam_lila_prep.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3730 2023-11-09 00:06:34.000000 megadetector-5.0.8/data_management/importers/jb_csv_to_json.py
+-rw-rw-r--   0 user      (1000) user      (1000)     6718 2023-09-21 01:58:08.000000 megadetector-5.0.8/data_management/importers/mcgill_to_json.py
+-rw-rw-r--   0 user      (1000) user      (1000)    14840 2023-11-09 00:01:34.000000 megadetector-5.0.8/data_management/importers/missouri_to_json.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2045 2023-09-21 01:58:08.000000 megadetector-5.0.8/data_management/importers/nacti_fieldname_adjustments.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5147 2024-02-03 20:07:26.000000 megadetector-5.0.8/data_management/importers/noaa_seals_2019.py
+-rw-rw-r--   0 user      (1000) user      (1000)    10718 2023-11-09 00:06:34.000000 megadetector-5.0.8/data_management/importers/pc_to_json.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3787 2023-09-21 01:58:08.000000 megadetector-5.0.8/data_management/importers/plot_wni_giraffes.py
+-rw-rw-r--   0 user      (1000) user      (1000)    12774 2023-11-08 23:59:39.000000 megadetector-5.0.8/data_management/importers/prepare-noaa-fish-data-for-lila.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3754 2023-11-09 00:06:34.000000 megadetector-5.0.8/data_management/importers/prepare_zsl_imerit.py
+-rw-rw-r--   0 user      (1000) user      (1000)     9834 2023-11-09 00:07:41.000000 megadetector-5.0.8/data_management/importers/rspb_to_json.py
+-rw-rw-r--   0 user      (1000) user      (1000)    10639 2023-11-09 00:05:19.000000 megadetector-5.0.8/data_management/importers/save_the_elephants_survey_A.py
+-rw-rw-r--   0 user      (1000) user      (1000)    11167 2023-11-09 00:05:19.000000 megadetector-5.0.8/data_management/importers/save_the_elephants_survey_B.py
+-rw-rw-r--   0 user      (1000) user      (1000)    23591 2023-11-09 00:06:52.000000 megadetector-5.0.8/data_management/importers/snapshot_safari_importer.py
+-rw-rw-r--   0 user      (1000) user      (1000)    22996 2023-07-13 19:18:01.000000 megadetector-5.0.8/data_management/importers/snapshot_safari_importer_reprise.py
+-rw-rw-r--   0 user      (1000) user      (1000)    33854 2023-11-09 00:07:01.000000 megadetector-5.0.8/data_management/importers/snapshot_serengeti_lila.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-19 23:55:36.232348 megadetector-5.0.8/data_management/importers/snapshotserengeti/
+-rw-rw-r--   0 user      (1000) user      (1000)     4126 2023-05-20 21:19:48.000000 megadetector-5.0.8/data_management/importers/snapshotserengeti/make_full_SS_json.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4316 2023-05-20 21:19:48.000000 megadetector-5.0.8/data_management/importers/snapshotserengeti/make_per_season_SS_json.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2088 2023-09-21 01:58:08.000000 megadetector-5.0.8/data_management/importers/sulross_get_exif.py
+-rw-rw-r--   0 user      (1000) user      (1000)    15902 2023-11-09 00:06:34.000000 megadetector-5.0.8/data_management/importers/timelapse_csv_set_to_json.py
+-rw-rw-r--   0 user      (1000) user      (1000)    14869 2023-11-09 00:05:19.000000 megadetector-5.0.8/data_management/importers/ubc_to_json.py
+-rw-rw-r--   0 user      (1000) user      (1000)    16177 2023-11-09 00:05:19.000000 megadetector-5.0.8/data_management/importers/umn_to_json.py
+-rw-rw-r--   0 user      (1000) user      (1000)     7671 2023-11-08 23:58:56.000000 megadetector-5.0.8/data_management/importers/wellington_to_json.py
+-rw-rw-r--   0 user      (1000) user      (1000)    13656 2023-11-09 00:00:11.000000 megadetector-5.0.8/data_management/importers/wi_to_json.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5594 2023-12-06 01:45:18.000000 megadetector-5.0.8/data_management/importers/zamba_results_to_md_results.py
+-rw-rw-r--   0 user      (1000) user      (1000)    18344 2024-04-19 23:54:16.000000 megadetector-5.0.8/data_management/labelme_to_coco.py
+-rw-rw-r--   0 user      (1000) user      (1000)    10041 2024-04-19 23:54:16.000000 megadetector-5.0.8/data_management/labelme_to_yolo.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-19 23:55:36.232348 megadetector-5.0.8/data_management/lila/
+-rw-rw-r--   0 user      (1000) user      (1000)     2561 2023-11-08 23:58:29.000000 megadetector-5.0.8/data_management/lila/add_locations_to_island_camera_traps.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5017 2023-10-28 15:19:33.000000 megadetector-5.0.8/data_management/lila/add_locations_to_nacti.py
+-rw-rw-r--   0 user      (1000) user      (1000)    19764 2024-02-04 15:39:49.000000 megadetector-5.0.8/data_management/lila/create_lila_blank_set.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4825 2023-12-31 18:59:10.000000 megadetector-5.0.8/data_management/lila/create_lila_test_set.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3916 2023-12-06 01:45:44.000000 megadetector-5.0.8/data_management/lila/create_links_to_md_results_files.py
+-rw-rw-r--   0 user      (1000) user      (1000)     7531 2024-04-09 13:56:32.000000 megadetector-5.0.8/data_management/lila/download_lila_subset.py
+-rw-rw-r--   0 user      (1000) user      (1000)    17352 2024-02-25 01:09:49.000000 megadetector-5.0.8/data_management/lila/generate_lila_per_image_labels.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5490 2023-12-31 18:59:10.000000 megadetector-5.0.8/data_management/lila/get_lila_annotation_counts.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3625 2023-06-26 23:52:53.000000 megadetector-5.0.8/data_management/lila/get_lila_image_counts.py
+-rw-rw-r--   0 user      (1000) user      (1000)     7691 2024-02-04 15:39:49.000000 megadetector-5.0.8/data_management/lila/lila_common.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3966 2023-12-31 18:59:10.000000 megadetector-5.0.8/data_management/lila/test_lila_metadata_urls.py
+-rw-rw-r--   0 user      (1000) user      (1000)    29920 2023-11-05 20:26:38.000000 megadetector-5.0.8/data_management/ocr_tools.py
+-rw-rw-r--   0 user      (1000) user      (1000)    21446 2024-04-19 23:54:16.000000 megadetector-5.0.8/data_management/read_exif.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3002 2024-04-19 23:54:16.000000 megadetector-5.0.8/data_management/remap_coco_categories.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1555 2023-07-13 00:36:13.000000 megadetector-5.0.8/data_management/remove_exif.py
+-rw-rw-r--   0 user      (1000) user      (1000)     6100 2024-04-19 23:54:16.000000 megadetector-5.0.8/data_management/resize_coco_dataset.py
+-rw-rw-r--   0 user      (1000) user      (1000)     7704 2024-03-09 00:34:45.000000 megadetector-5.0.8/data_management/wi_download_csv_to_coco.py
+-rw-rw-r--   0 user      (1000) user      (1000)    16313 2024-01-28 18:41:58.000000 megadetector-5.0.8/data_management/yolo_output_to_md_output.py
+-rw-rw-r--   0 user      (1000) user      (1000)    15196 2024-04-19 23:54:16.000000 megadetector-5.0.8/data_management/yolo_to_coco.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-19 23:55:36.232348 megadetector-5.0.8/detection/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-19 23:55:36.232348 megadetector-5.0.8/detection/detector_training/
+-rw-rw-r--   0 user      (1000) user      (1000)     1091 2023-07-13 00:36:13.000000 megadetector-5.0.8/detection/detector_training/copy_checkpoints.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4936 2023-05-20 21:19:48.000000 megadetector-5.0.8/detection/detector_training/model_main_tf2.py
+-rw-rw-r--   0 user      (1000) user      (1000)    26825 2024-02-02 00:27:22.000000 megadetector-5.0.8/detection/process_video.py
+-rw-rw-r--   0 user      (1000) user      (1000)    11992 2024-01-28 18:41:58.000000 megadetector-5.0.8/detection/pytorch_detector.py
+-rw-rw-r--   0 user      (1000) user      (1000)    26036 2023-12-21 01:23:34.000000 megadetector-5.0.8/detection/run_detector.py
+-rw-rw-r--   0 user      (1000) user      (1000)    47426 2024-03-31 18:21:07.000000 megadetector-5.0.8/detection/run_detector_batch.py
+-rw-rw-r--   0 user      (1000) user      (1000)    33975 2024-03-31 18:21:07.000000 megadetector-5.0.8/detection/run_inference_with_yolov5_val.py
+-rw-rw-r--   0 user      (1000) user      (1000)    33931 2024-02-25 01:09:49.000000 megadetector-5.0.8/detection/run_tiled_inference.py
+-rw-rw-r--   0 user      (1000) user      (1000)     6769 2024-03-31 18:21:07.000000 megadetector-5.0.8/detection/tf_detector.py
+-rw-rw-r--   0 user      (1000) user      (1000)    19501 2024-04-09 14:11:23.000000 megadetector-5.0.8/detection/video_utils.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-19 23:55:36.236348 megadetector-5.0.8/md_utils/
+-rw-rw-r--   0 user      (1000) user      (1000)     6243 2023-05-22 23:02:57.000000 megadetector-5.0.8/md_utils/azure_utils.py
+-rw-rw-r--   0 user      (1000) user      (1000)    13311 2024-04-13 19:10:46.000000 megadetector-5.0.8/md_utils/ct_utils.py
+-rw-rw-r--   0 user      (1000) user      (1000)     9615 2023-10-10 14:50:39.000000 megadetector-5.0.8/md_utils/directory_listing.py
+-rw-rw-r--   0 user      (1000) user      (1000)    33520 2024-03-19 20:27:38.000000 megadetector-5.0.8/md_utils/md_tests.py
+-rw-rw-r--   0 user      (1000) user      (1000)    23176 2024-04-19 23:54:16.000000 megadetector-5.0.8/md_utils/path_utils.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4316 2024-01-28 18:41:58.000000 megadetector-5.0.8/md_utils/process_utils.py
+-rw-rw-r--   0 user      (1000) user      (1000)    16955 2023-07-05 17:03:19.000000 megadetector-5.0.8/md_utils/sas_blob_utils.py
+-rw-rw-r--   0 user      (1000) user      (1000)     9241 2023-11-22 03:22:33.000000 megadetector-5.0.8/md_utils/split_locations_into_train_val.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1600 2024-02-02 00:27:22.000000 megadetector-5.0.8/md_utils/string_utils.py
+-rw-rw-r--   0 user      (1000) user      (1000)     6824 2024-03-31 18:21:07.000000 megadetector-5.0.8/md_utils/url_utils.py
+-rw-rw-r--   0 user      (1000) user      (1000)     7532 2024-03-19 20:27:38.000000 megadetector-5.0.8/md_utils/write_html_image_list.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-19 23:55:36.236348 megadetector-5.0.8/md_visualization/
+-rw-rw-r--   0 user      (1000) user      (1000)    10712 2023-10-25 02:02:08.000000 megadetector-5.0.8/md_visualization/plot_utils.py
+-rw-rw-r--   0 user      (1000) user      (1000)    10391 2023-07-05 17:03:56.000000 megadetector-5.0.8/md_visualization/render_images_with_thumbnails.py
+-rw-rw-r--   0 user      (1000) user      (1000)    46496 2024-03-31 18:21:07.000000 megadetector-5.0.8/md_visualization/visualization_utils.py
+-rw-rw-r--   0 user      (1000) user      (1000)    19616 2024-04-19 23:54:16.000000 megadetector-5.0.8/md_visualization/visualize_db.py
+-rw-rw-r--   0 user      (1000) user      (1000)    15814 2024-01-13 01:05:31.000000 megadetector-5.0.8/md_visualization/visualize_detector_output.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-19 23:55:36.236348 megadetector-5.0.8/megadetector.egg-info/
+-rw-r--r--   0 user      (1000) user      (1000)     7373 2024-04-19 23:55:36.000000 megadetector-5.0.8/megadetector.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)    10305 2024-04-19 23:55:36.000000 megadetector-5.0.8/megadetector.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2024-04-19 23:55:36.000000 megadetector-5.0.8/megadetector.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)      238 2024-04-19 23:55:36.000000 megadetector-5.0.8/megadetector.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)      101 2024-04-19 23:55:36.000000 megadetector-5.0.8/megadetector.egg-info/top_level.txt
+-rw-rw-r--   0 user      (1000) user      (1000)     1688 2024-04-19 23:55:26.000000 megadetector-5.0.8/pyproject.toml
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2024-04-19 23:55:36.236348 megadetector-5.0.8/setup.cfg
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-19 23:55:36.236348 megadetector-5.0.8/taxonomy_mapping/
+-rw-rw-r--   0 user      (1000) user      (1000)    16517 2023-12-06 01:57:03.000000 megadetector-5.0.8/taxonomy_mapping/map_lila_taxonomy_to_wi_taxonomy.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4324 2024-01-09 23:45:10.000000 megadetector-5.0.8/taxonomy_mapping/map_new_lila_datasets.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4357 2024-01-09 23:45:10.000000 megadetector-5.0.8/taxonomy_mapping/prepare_lila_taxonomy_release.py
+-rw-rw-r--   0 user      (1000) user      (1000)    20144 2023-12-31 18:59:10.000000 megadetector-5.0.8/taxonomy_mapping/preview_lila_taxonomy.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1992 2023-06-26 19:00:42.000000 megadetector-5.0.8/taxonomy_mapping/retrieve_sample_image.py
+-rw-rw-r--   0 user      (1000) user      (1000)     6874 2023-07-05 17:04:26.000000 megadetector-5.0.8/taxonomy_mapping/simple_image_download.py
+-rw-rw-r--   0 user      (1000) user      (1000)    28303 2023-12-31 18:59:10.000000 megadetector-5.0.8/taxonomy_mapping/species_lookup.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4874 2023-12-31 18:59:10.000000 megadetector-5.0.8/taxonomy_mapping/taxonomy_csv_checker.py
+-rw-rw-r--   0 user      (1000) user      (1000)    12361 2023-07-13 00:36:13.000000 megadetector-5.0.8/taxonomy_mapping/taxonomy_graph.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2314 2023-06-26 17:52:32.000000 megadetector-5.0.8/taxonomy_mapping/validate_lila_category_mappings.py
```

### Comparing `megadetector-5.0.7/LICENSE` & `megadetector-5.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `megadetector-5.0.7/PKG-INFO` & `megadetector-5.0.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: megadetector
-Version: 5.0.7
+Version: 5.0.8
 Summary: MegaDetector is an AI model that helps conservation folks spend less time doing boring things with camera trap images.
 Author-email: Your friendly neighborhood MegaDetector team <cameratraps@lila.science>
 Maintainer-email: Your friendly neighborhood MegaDetector team <cameratraps@lila.science>
 License:     MIT License
         
             Permission is hereby granted, free of charge, to any person obtaining a copy
             of this software and associated documentation files (the "Software"), to deal
@@ -56,15 +56,15 @@
 If you want to learn more about what MegaDetector is all about, head over to the [MegaDetector repo](https://github.com/agentmorris/MegaDetector).
 
 
 ## Reasons you probably aren't looking for this package
 
 ### If you are an ecologist...
 
-If you are an ecologist looking to use MegaDetector to help you get through your camera trap images, you probably don't want this package.  We recommend starting with our "[Getting started with MegaDetector](https://github.com/agentmorris/MegaDetector/blob/main/collaborations.md)" page, then digging in to the [MegaDetector User Guide](https://github.com/agentmorris/MegaDetector/blob/main/megadetector.md), which will walk you through the process of using MegaDetector.  That journey will <i>not</i> involve this package.
+If you are an ecologist looking to use MegaDetector to help you get through your camera trap images, you probably don't want this package.  We recommend starting with our "[Getting started with MegaDetector](https://github.com/agentmorris/MegaDetector/blob/main/collaborations.md)" page, then digging in to the [MegaDetector User Guide](https://github.com/agentmorris/MegaDetector/blob/main/megadetector.md), which will walk you through the process of using MegaDetector.  That journey will <i>not</i> involve this Python package.
 
 ### If you are a computer-vision-y type...
 
 If you are a computer-vision-y person looking to run or fine-tune MegaDetector programmatically, you still probably don't want this package.  MegaDetector is just a fine-tuned version of [YOLOv5](https://github.com/ultralytics/yolov5), and the [ultralytics](https://github.com/ultralytics/ultralytics/) package (from the developers of YOLOv5) has a zillion bells and whistles for both inference and fine-tuning that this package doesn't.
 
 ## Reasons you might want to use this package
 
@@ -91,23 +91,21 @@
 
 # This is the image at the bottom of this page, it has one animal in it
 image_url = 'https://github.com/agentmorris/MegaDetector/raw/main/images/orinoquia-thumb-web.jpg'
 temporary_filename = url_utils.download_url(image_url)
 
 image = vis_utils.load_image(temporary_filename)
 
-# This will automatically download MDv5a to the system temp folder;
-# you can also specify a filename explicitly, or set the $MDV5A
-# environment variable to point to the model file.
+# This will automatically download MDv5a; you can also specify a filename.
 model = run_detector.load_detector('MDV5A')
 
 result = model.generate_detections_one_image(image)
 
 detections_above_threshold = [d for d in result['detections'] if d['conf'] > 0.2]
-print('Found {} detection above threshold'.format(len(detections_above_threshold)))
+print('Found {} detections above threshold'.format(len(detections_above_threshold)))
 ```
 
 #### Run MegaDetector on a folder of images
 
 ```
 from detection.run_detector_batch import load_and_run_detector_batch,write_results_to_file
 from md_utils import path_utils
@@ -116,22 +114,22 @@
 # Pick a folder to run MD on recursively, and an output file
 image_folder = os.path.expanduser('~/megadetector_test_images')
 output_file = os.path.expanduser('~/megadetector_output_test.json')
 
 # Recursively find images
 image_file_names = path_utils.find_images(image_folder,recursive=True)
 
-# This will automatically download MDv5a to the system temp folder;
-# you can also specify a filename explicitly, or set the $MDV5A
-# environment variable to point to the model file.
+# This will automatically download MDv5a; you can also specify a filename.
 results = load_and_run_detector_batch('MDV5A', image_file_names)
 
-# Write results as relative filenames, this is what Timelapse
-# and other downstream tools expect.
-write_results_to_file(results,output_file,relative_path_base=image_folder)
+# Write results to a format that Timelapse and other downstream tools like.
+write_results_to_file(results,
+                      output_file,
+                      relative_path_base=image_folder,
+                      detector_file=detector_filename)
 ```
 
 ## Contact
 
 Contact <a href="cameratraps@lila.science">cameratraps@lila.science</a> with questions.
 
 ## Gratuitous animal picture
```

### Comparing `megadetector-5.0.7/README-package.md` & `megadetector-5.0.8/README-package.md`

 * *Files 16% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 If you want to learn more about what MegaDetector is all about, head over to the [MegaDetector repo](https://github.com/agentmorris/MegaDetector).
 
 
 ## Reasons you probably aren't looking for this package
 
 ### If you are an ecologist...
 
-If you are an ecologist looking to use MegaDetector to help you get through your camera trap images, you probably don't want this package.  We recommend starting with our "[Getting started with MegaDetector](https://github.com/agentmorris/MegaDetector/blob/main/collaborations.md)" page, then digging in to the [MegaDetector User Guide](https://github.com/agentmorris/MegaDetector/blob/main/megadetector.md), which will walk you through the process of using MegaDetector.  That journey will <i>not</i> involve this package.
+If you are an ecologist looking to use MegaDetector to help you get through your camera trap images, you probably don't want this package.  We recommend starting with our "[Getting started with MegaDetector](https://github.com/agentmorris/MegaDetector/blob/main/collaborations.md)" page, then digging in to the [MegaDetector User Guide](https://github.com/agentmorris/MegaDetector/blob/main/megadetector.md), which will walk you through the process of using MegaDetector.  That journey will <i>not</i> involve this Python package.
 
 ### If you are a computer-vision-y type...
 
 If you are a computer-vision-y person looking to run or fine-tune MegaDetector programmatically, you still probably don't want this package.  MegaDetector is just a fine-tuned version of [YOLOv5](https://github.com/ultralytics/yolov5), and the [ultralytics](https://github.com/ultralytics/ultralytics/) package (from the developers of YOLOv5) has a zillion bells and whistles for both inference and fine-tuning that this package doesn't.
 
 ## Reasons you might want to use this package
 
@@ -40,23 +40,21 @@
 
 # This is the image at the bottom of this page, it has one animal in it
 image_url = 'https://github.com/agentmorris/MegaDetector/raw/main/images/orinoquia-thumb-web.jpg'
 temporary_filename = url_utils.download_url(image_url)
 
 image = vis_utils.load_image(temporary_filename)
 
-# This will automatically download MDv5a to the system temp folder;
-# you can also specify a filename explicitly, or set the $MDV5A
-# environment variable to point to the model file.
+# This will automatically download MDv5a; you can also specify a filename.
 model = run_detector.load_detector('MDV5A')
 
 result = model.generate_detections_one_image(image)
 
 detections_above_threshold = [d for d in result['detections'] if d['conf'] > 0.2]
-print('Found {} detection above threshold'.format(len(detections_above_threshold)))
+print('Found {} detections above threshold'.format(len(detections_above_threshold)))
 ```
 
 #### Run MegaDetector on a folder of images
 
 ```
 from detection.run_detector_batch import load_and_run_detector_batch,write_results_to_file
 from md_utils import path_utils
@@ -65,22 +63,22 @@
 # Pick a folder to run MD on recursively, and an output file
 image_folder = os.path.expanduser('~/megadetector_test_images')
 output_file = os.path.expanduser('~/megadetector_output_test.json')
 
 # Recursively find images
 image_file_names = path_utils.find_images(image_folder,recursive=True)
 
-# This will automatically download MDv5a to the system temp folder;
-# you can also specify a filename explicitly, or set the $MDV5A
-# environment variable to point to the model file.
+# This will automatically download MDv5a; you can also specify a filename.
 results = load_and_run_detector_batch('MDV5A', image_file_names)
 
-# Write results as relative filenames, this is what Timelapse
-# and other downstream tools expect.
-write_results_to_file(results,output_file,relative_path_base=image_folder)
+# Write results to a format that Timelapse and other downstream tools like.
+write_results_to_file(results,
+                      output_file,
+                      relative_path_base=image_folder,
+                      detector_file=detector_filename)
 ```
 
 ## Contact
 
 Contact <a href="cameratraps@lila.science">cameratraps@lila.science</a> with questions.
 
 ## Gratuitous animal picture
```

### Comparing `megadetector-5.0.7/README.md` & `megadetector-5.0.8/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -2,1204 +2,1301 @@
 00000010: 2e2e 2e68 656c 7069 6e67 2063 6f6e 7365  ...helping conse
 00000020: 7276 6174 696f 6e20 6269 6f6c 6f67 6973  rvation biologis
 00000030: 7473 2073 7065 6e64 206c 6573 7320 7469  ts spend less ti
 00000040: 6d65 2064 6f69 6e67 2062 6f72 696e 6720  me doing boring 
 00000050: 7468 696e 6773 2077 6974 6820 6361 6d65  things with came
 00000060: 7261 2074 7261 7020 696d 6167 6573 2e0a  ra trap images..
 00000070: 0a23 2320 5461 626c 6520 6f66 2063 6f6e  .## Table of con
-00000080: 7465 6e74 730a 0a31 2e20 5b52 6570 6f20  tents..1. [Repo 
-00000090: 6f76 6572 7669 6577 5d28 2372 6570 6f2d  overview](#repo-
-000000a0: 6f76 6572 7669 6577 290a 322e 205b 5768  overview).2. [Wh
-000000b0: 6174 2773 204d 6567 6144 6574 6563 746f  at's MegaDetecto
-000000c0: 7220 616c 6c20 6162 6f75 743f 5d28 2377  r all about?](#w
-000000d0: 6861 7473 2d6d 6567 6164 6574 6563 746f  hats-megadetecto
-000000e0: 722d 616c 6c2d 6162 6f75 7429 0a33 2e20  r-all-about).3. 
-000000f0: 5b48 6f77 2064 6f20 4920 6765 7420 7374  [How do I get st
-00000100: 6172 7465 6420 7769 7468 204d 6567 6144  arted with MegaD
-00000110: 6574 6563 746f 723f 5d28 2368 6f77 2d64  etector?](#how-d
-00000120: 6f2d 692d 6765 742d 7374 6172 7465 642d  o-i-get-started-
-00000130: 7769 7468 2d6d 6567 6164 6574 6563 746f  with-megadetecto
-00000140: 7229 0a34 2e20 5b57 686f 2069 7320 7573  r).4. [Who is us
-00000150: 696e 6720 4d65 6761 4465 7465 6374 6f72  ing MegaDetector
-00000160: 3f5d 2823 7768 6f2d 6973 2d75 7369 6e67  ?](#who-is-using
-00000170: 2d6d 6567 6164 6574 6563 746f 7229 0a35  -megadetector).5
-00000180: 2e20 5b52 6570 6f20 636f 6e74 656e 7473  . [Repo contents
-00000190: 5d28 2372 6570 6f2d 636f 6e74 656e 7473  ](#repo-contents
-000001a0: 290a 362e 205b 436f 6e74 6163 745d 2823  ).6. [Contact](#
-000001b0: 636f 6e74 6163 7429 0a37 2e20 5b47 7261  contact).7. [Gra
-000001c0: 7475 6974 6f75 7320 6361 6d65 7261 2074  tuitous camera t
-000001d0: 7261 7020 7069 6374 7572 655d 2823 6772  rap picture](#gr
-000001e0: 6174 7569 746f 7573 2d63 616d 6572 612d  atuitous-camera-
-000001f0: 7472 6170 2d70 6963 7475 7265 290a 0a0a  trap-picture)...
-00000200: 2323 2052 6570 6f20 6f76 6572 7669 6577  ## Repo overview
-00000210: 0a0a 5468 6973 2072 6570 6f20 636f 6e74  ..This repo cont
-00000220: 6169 6e73 2074 6865 2074 6f6f 6c73 2066  ains the tools f
-00000230: 6f72 2074 7261 696e 696e 6720 616e 6420  or training and 
-00000240: 7275 6e6e 696e 6720 5b4d 6567 6144 6574  running [MegaDet
-00000250: 6563 746f 725d 286d 6567 6164 6574 6563  ector](megadetec
-00000260: 746f 722e 6d64 292c 2061 6e20 6f62 6a65  tor.md), an obje
-00000270: 6374 2064 6574 6563 7469 6f6e 206d 6f64  ct detection mod
-00000280: 656c 2074 6861 7420 646f 6573 2061 2070  el that does a p
-00000290: 7265 7474 7920 676f 6f64 206a 6f62 2066  retty good job f
-000002a0: 696e 6469 6e67 2061 6e69 6d61 6c73 2c20  inding animals, 
-000002b0: 7065 6f70 6c65 2c20 616e 6420 7665 6869  people, and vehi
-000002c0: 636c 6573 2028 616e 6420 7468 6572 6566  cles (and theref
-000002d0: 6f72 6520 6973 2070 7265 7474 7920 676f  ore is pretty go
-000002e0: 6f64 2061 7420 6669 6e64 696e 6720 656d  od at finding em
-000002f0: 7074 7920 696d 6167 6573 2920 696e 2063  pty images) in c
-00000300: 616d 6572 6120 7472 6170 2069 6d61 6765  amera trap image
-00000310: 7320 696e 2061 2076 6172 6965 7479 206f  s in a variety o
-00000320: 6620 7465 7272 6573 7472 6961 6c20 6563  f terrestrial ec
-00000330: 6f73 7973 7465 6d73 2e0a 0a54 6865 2063  osystems...The c
-00000340: 6f72 6520 6675 6e63 7469 6f6e 616c 6974  ore functionalit
-00000350: 7920 7072 6f76 6964 6564 2069 733a 0a0a  y provided is:..
-00000360: 2d20 5472 6169 6e69 6e67 2061 6e64 2072  - Training and r
-00000370: 756e 6e69 6e67 205b 4d65 6761 4465 7465  unning [MegaDete
-00000380: 6374 6f72 5d28 6d65 6761 6465 7465 6374  ctor](megadetect
-00000390: 6f72 2e6d 6429 2e0a 2d20 5472 6169 6e69  or.md)..- Traini
-000003a0: 6e67 2061 6e64 2072 756e 6e69 6e67 2073  ng and running s
-000003b0: 6f6d 6520 5b73 7065 6369 6573 2063 6c61  ome [species cla
-000003c0: 7373 6966 6965 7273 5d28 636c 6173 7369  ssifiers](classi
-000003d0: 6669 6361 7469 6f6e 2920 7468 6174 2061  fication) that a
-000003e0: 7265 2075 7365 6420 696e 2063 6f6e 6a75  re used in conju
-000003f0: 6e63 7469 6f6e 2077 6974 6820 4d65 6761  nction with Mega
-00000400: 4465 7465 6374 6f72 2e0a 2d20 546f 6f6c  Detector..- Tool
-00000410: 7320 746f 205b 636f 6e76 6572 745d 2864  s to [convert](d
-00000420: 6174 615f 6d61 6e61 6765 6d65 6e74 2920  ata_management) 
-00000430: 6672 6571 7565 6e74 6c79 2d75 7365 6420  frequently-used 
-00000440: 6361 6d65 7261 2074 7261 7020 6d65 7461  camera trap meta
-00000450: 6461 7461 2066 6f72 6d61 7473 2069 6e74  data formats int
-00000460: 6f20 6120 636f 6d6d 6f6e 2066 6f72 6d61  o a common forma
-00000470: 742e 0a2d 2041 205b 6261 7463 6820 7072  t..- A [batch pr
-00000480: 6f63 6573 7369 6e67 2041 5049 5d28 6874  ocessing API](ht
-00000490: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-000004a0: 2f61 6765 6e74 6d6f 7272 6973 2f4d 6567  /agentmorris/Meg
-000004b0: 6144 6574 6563 746f 722f 7472 6565 2f6d  aDetector/tree/m
-000004c0: 6169 6e2f 6170 692f 6261 7463 685f 7072  ain/api/batch_pr
-000004d0: 6f63 6573 7369 6e67 2920 7468 6174 2072  ocessing) that r
-000004e0: 756e 7320 4d65 6761 4465 7465 6374 6f72  uns MegaDetector
-000004f0: 206f 6e20 6c61 7267 6520 696d 6167 6520   on large image 
-00000500: 636f 6c6c 6563 7469 6f6e 732c 2074 6f20  collections, to 
-00000510: 6163 6365 6c65 7261 7465 2070 6f70 756c  accelerate popul
-00000520: 6174 696f 6e20 7375 7276 6579 732e 0a2d  ation surveys..-
-00000530: 2041 205b 7265 616c 2d74 696d 6520 4150   A [real-time AP
-00000540: 495d 2868 7474 7073 3a2f 2f67 6974 6875  I](https://githu
-00000550: 622e 636f 6d2f 6167 656e 746d 6f72 7269  b.com/agentmorri
-00000560: 732f 4d65 6761 4465 7465 6374 6f72 2f74  s/MegaDetector/t
-00000570: 7265 652f 6d61 696e 2f61 7069 2f73 796e  ree/main/api/syn
-00000580: 6368 726f 6e6f 7573 2920 7468 6174 2072  chronous) that r
-00000590: 756e 7320 4d65 6761 4465 7465 6374 6f72  uns MegaDetector
-000005a0: 2028 616e 6420 736f 6d65 2073 7065 6369   (and some speci
-000005b0: 6573 2063 6c61 7373 6966 6965 7273 2920  es classifiers) 
-000005c0: 7379 6e63 6872 6f6e 6f75 736c 792c 2070  synchronously, p
-000005d0: 7269 6d61 7269 6c79 2074 6f20 7375 7070  rimarily to supp
-000005e0: 6f72 7420 6269 6f73 6563 7572 6974 7920  ort biosecurity 
-000005f0: 6170 706c 6963 6174 696f 6e73 2e0a 0a4d  applications...M
-00000600: 6567 6144 6574 6563 746f 7220 7761 7320  egaDetector was 
-00000610: 696e 6974 6961 6c6c 7920 6465 7665 6c6f  initially develo
-00000620: 7065 6420 6279 2074 6865 205b 4d69 6372  ped by the [Micr
-00000630: 6f73 6f66 7420 4149 2066 6f72 2045 6172  osoft AI for Ear
-00000640: 7468 2070 726f 6772 616d 5d28 6874 7470  th program](http
-00000650: 733a 2f2f 7777 772e 6d69 6372 6f73 6f66  s://www.microsof
-00000660: 742e 636f 6d2f 656e 2d75 732f 6169 2f61  t.com/en-us/ai/a
-00000670: 692d 666f 722d 6561 7274 6829 3b20 7468  i-for-earth); th
-00000680: 6973 2072 6570 6f20 7761 7320 666f 726b  is repo was fork
-00000690: 6564 2066 726f 6d20 7468 6520 6d69 6372  ed from the micr
-000006a0: 6f73 6f66 742f 6361 6d65 7261 7472 6170  osoft/cameratrap
-000006b0: 7320 7265 706f 2061 6e64 2069 7320 6d61  s repo and is ma
-000006c0: 696e 7461 696e 6564 2062 7920 7468 6520  intained by the 
-000006d0: 6f72 6967 696e 616c 204d 6567 6144 6574  original MegaDet
-000006e0: 6563 746f 7220 6465 7665 6c6f 7065 7273  ector developers
-000006f0: 2028 7768 6f20 6172 6520 6e6f 206c 6f6e   (who are no lon
-00000700: 6765 7220 6174 204d 6963 726f 736f 6674  ger at Microsoft
-00000710: 2c20 6275 7420 6172 6520 6162 736f 6c75  , but are absolu
-00000720: 7465 6c79 2066 616e 7461 7374 6963 616c  tely fantastical
-00000730: 6c79 2065 7465 726e 616c 6c79 2067 7261  ly eternally gra
-00000740: 7465 6675 6c20 746f 204d 6963 726f 736f  teful to Microso
-00000750: 6674 2066 6f72 2074 6865 2069 6e76 6573  ft for the inves
-00000760: 746d 656e 7420 616e 6420 636f 6d6d 6974  tment and commit
-00000770: 6d65 6e74 2074 6861 7420 6d61 6465 204d  ment that made M
-00000780: 6567 6144 6574 6563 746f 7220 6861 7070  egaDetector happ
-00000790: 656e 292e 0a0a 0a23 2320 5768 6174 2773  en)....## What's
-000007a0: 204d 6567 6144 6574 6563 746f 7220 616c   MegaDetector al
-000007b0: 6c20 6162 6f75 743f 0a0a 5b4d 6567 6144  l about?..[MegaD
-000007c0: 6574 6563 746f 725d 286d 6567 6164 6574  etector](megadet
-000007d0: 6563 746f 722e 6d64 2920 6973 2061 6e20  ector.md) is an 
-000007e0: 6f62 6a65 6374 2064 6574 6563 7469 6f6e  object detection
-000007f0: 206d 6f64 656c 2074 6861 7420 6964 656e   model that iden
-00000800: 7469 6669 6573 2061 6e69 6d61 6c73 2c20  tifies animals, 
-00000810: 7065 6f70 6c65 2c20 616e 6420 7665 6869  people, and vehi
-00000820: 636c 6573 2069 6e20 6361 6d65 7261 2074  cles in camera t
-00000830: 7261 7020 696d 6167 6573 2028 7768 6963  rap images (whic
-00000840: 6820 616c 736f 206d 616b 6573 2069 7420  h also makes it 
-00000850: 7573 6566 756c 2066 6f72 2065 6c69 6d69  useful for elimi
-00000860: 6e61 7469 6e67 2062 6c61 6e6b 2069 6d61  nating blank ima
-00000870: 6765 7329 2e20 2054 6869 7320 6d6f 6465  ges).  This mode
-00000880: 6c20 6973 2074 7261 696e 6564 206f 6e20  l is trained on 
-00000890: 7365 7665 7261 6c20 6875 6e64 7265 6420  several hundred 
-000008a0: 7468 6f75 7361 6e64 2062 6f75 6e64 696e  thousand boundin
-000008b0: 6720 626f 7865 7320 6672 6f6d 2061 2076  g boxes from a v
-000008c0: 6172 6965 7479 206f 6620 6563 6f73 7973  ariety of ecosys
-000008d0: 7465 6d73 2e20 204c 6f74 7320 6d6f 7265  tems.  Lots more
-000008e0: 2069 6e66 6f72 6d61 7469 6f6e 2026 6e64   information &nd
-000008f0: 6173 683b 2069 6e63 6c75 6469 6e67 2064  ash; including d
-00000900: 6f77 6e6c 6f61 6420 6c69 6e6b 7320 616e  ownload links an
-00000910: 6420 696e 7374 7275 6374 696f 6e73 2066  d instructions f
-00000920: 6f72 2072 756e 6e69 6e67 2074 6865 206d  or running the m
-00000930: 6f64 656c 2026 6e64 6173 683b 2069 7320  odel &ndash; is 
-00000940: 6176 6169 6c61 626c 6520 696e 2074 6865  available in the
-00000950: 205b 4d65 6761 4465 7465 6374 6f72 2055   [MegaDetector U
-00000960: 7365 7220 4775 6964 655d 286d 6567 6164  ser Guide](megad
-00000970: 6574 6563 746f 722e 6d64 292e 0a0a 5468  etector.md)...Th
-00000980: 6973 2072 6570 6f20 646f 6573 206e 6f74  is repo does not
-00000990: 2068 6f73 7420 7468 6520 6461 7461 2075   host the data u
-000009a0: 7365 6420 746f 2074 7261 696e 204d 6567  sed to train Meg
-000009b0: 6144 6574 6563 746f 722c 2062 7574 2077  aDetector, but w
-000009c0: 6520 776f 726b 2077 6974 6820 6f75 7220  e work with our 
-000009d0: 636f 6c6c 6162 6f72 6174 6f72 7320 746f  collaborators to
-000009e0: 206d 616b 6520 6461 7461 2061 6e64 2061   make data and a
-000009f0: 6e6e 6f74 6174 696f 6e73 2061 7661 696c  nnotations avail
-00000a00: 6162 6c65 2077 6865 6e65 7665 7220 706f  able whenever po
-00000a10: 7373 6962 6c65 206f 6e20 5b6c 696c 612e  ssible on [lila.
-00000a20: 7363 6965 6e63 655d 2868 7474 703a 2f2f  science](http://
-00000a30: 6c69 6c61 2e73 6369 656e 6365 292e 2020  lila.science).  
-00000a40: 5365 6520 7468 6520 5b4d 6567 6144 6574  See the [MegaDet
-00000a50: 6563 746f 7220 7472 6169 6e69 6e67 2064  ector training d
-00000a60: 6174 615d 286d 6567 6164 6574 6563 746f  ata](megadetecto
-00000a70: 722e 6d64 2363 616e 2d79 6f75 2d73 6861  r.md#can-you-sha
-00000a80: 7265 2d74 6865 2d74 7261 696e 696e 672d  re-the-training-
-00000a90: 6461 7461 2920 7365 6374 696f 6e20 746f  data) section to
-00000aa0: 206c 6561 726e 206d 6f72 6520 6162 6f75   learn more abou
-00000ab0: 7420 7468 6520 6461 7461 2075 7365 6420  t the data used 
-00000ac0: 746f 2074 7261 696e 204d 6567 6144 6574  to train MegaDet
-00000ad0: 6563 746f 722e 0a0a 4865 7265 2773 2061  ector...Here's a
-00000ae0: 2026 6c64 7175 6f3b 7465 6173 6572 2672   &ldquo;teaser&r
-00000af0: 6471 756f 3b20 696d 6167 6520 6f66 2077  dquo; image of w
-00000b00: 6861 7420 4d65 6761 4465 7465 6374 6f72  hat MegaDetector
-00000b10: 206f 7574 7075 7420 6c6f 6f6b 7320 6c69   output looks li
-00000b20: 6b65 3a0a 0a21 5b52 6564 2062 6f75 6e64  ke:..![Red bound
-00000b30: 696e 6720 626f 7820 6f6e 2066 6f78 5d28  ing box on fox](
-00000b40: 696d 6167 6573 2f64 6574 6563 746f 725f  images/detector_
-00000b50: 6578 616d 706c 652e 6a70 6729 3c62 722f  example.jpg)<br/
-00000b60: 3e49 6d61 6765 2063 7265 6469 7420 556e  >Image credit Un
-00000b70: 6976 6572 7369 7479 206f 6620 5761 7368  iversity of Wash
-00000b80: 696e 6774 6f6e 2e0a 0a0a 2323 2048 6f77  ington....## How
-00000b90: 2064 6f20 4920 6765 7420 7374 6172 7465   do I get starte
-00000ba0: 6420 7769 7468 204d 6567 6144 6574 6563  d with MegaDetec
-00000bb0: 746f 723f 0a0a 4966 2079 6f75 2772 6520  tor?..If you're 
-00000bc0: 6a75 7374 2063 6f6e 7369 6465 7269 6e67  just considering
-00000bd0: 2074 6865 2075 7365 206f 6620 4149 2069   the use of AI i
-00000be0: 6e20 796f 7572 2077 6f72 6b66 6c6f 772c  n your workflow,
-00000bf0: 2061 6e64 2079 6f75 2061 7265 6e27 7420   and you aren't 
-00000c00: 6576 656e 2073 7572 6520 7965 7420 7768  even sure yet wh
-00000c10: 6574 6865 7220 4d65 6761 4465 7465 6374  ether MegaDetect
-00000c20: 6f72 2077 6f75 6c64 2062 6520 7573 6566  or would be usef
-00000c30: 756c 2074 6f20 796f 752c 2077 6520 7265  ul to you, we re
-00000c40: 636f 6d6d 656e 6420 7265 6164 696e 6720  commend reading 
-00000c50: 7468 6520 225b 6765 7474 696e 6720 7374  the "[getting st
-00000c60: 6172 7465 6420 7769 7468 204d 6567 6144  arted with MegaD
-00000c70: 6574 6563 746f 725d 2863 6f6c 6c61 626f  etector](collabo
-00000c80: 7261 7469 6f6e 732e 6d64 2922 2070 6167  rations.md)" pag
-00000c90: 652e 0a0a 4966 2079 6f75 2772 6520 616c  e...If you're al
-00000ca0: 7265 6164 7920 6661 6d69 6c69 6172 2077  ready familiar w
-00000cb0: 6974 6820 4d65 6761 4465 7465 6374 6f72  ith MegaDetector
-00000cc0: 2061 6e64 2079 6f75 2772 6520 7265 6164   and you're read
-00000cd0: 7920 746f 2072 756e 2069 7420 6f6e 2079  y to run it on y
-00000ce0: 6f75 7220 6461 7461 2028 616e 6420 796f  our data (and yo
-00000cf0: 7520 6861 7665 2073 6f6d 6520 6661 6d69  u have some fami
-00000d00: 6c69 6172 6974 7920 7769 7468 2072 756e  liarity with run
-00000d10: 6e69 6e67 2050 7974 686f 6e20 636f 6465  ning Python code
-00000d20: 292c 2073 6565 2074 6865 205b 4d65 6761  ), see the [Mega
-00000d30: 4465 7465 6374 6f72 2055 7365 7220 4775  Detector User Gu
-00000d40: 6964 655d 286d 6567 6164 6574 6563 746f  ide](megadetecto
-00000d50: 722e 6d64 2920 666f 7220 696e 7374 7275  r.md) for instru
-00000d60: 6374 696f 6e73 206f 6e20 646f 776e 6c6f  ctions on downlo
-00000d70: 6164 696e 6720 616e 6420 7275 6e6e 696e  ading and runnin
-00000d80: 6720 4d65 6761 4465 7465 6374 6f72 2e0a  g MegaDetector..
-00000d90: 0a49 6620 796f 7527 7265 2061 2070 726f  .If you're a pro
-00000da0: 6772 616d 6d65 722d 7479 7065 206c 6f6f  grammer-type loo
-00000db0: 6b69 6e67 2074 6f20 7573 6520 746f 6f6c  king to use tool
-00000dc0: 7320 6672 6f6d 2074 6869 7320 7265 706f  s from this repo
-00000dd0: 2c20 7765 2067 656e 6572 616c 6c79 2072  , we generally r
-00000de0: 6563 6f6d 6d65 6e64 2063 6c6f 6e69 6e67  ecommend cloning
-00000df0: 2074 6865 2072 6570 6f2c 2062 7574 2074   the repo, but t
-00000e00: 6865 7265 2069 7320 616c 736f 2061 205b  here is also a [
-00000e10: 5079 7468 6f6e 2070 6163 6b61 6765 5d28  Python package](
-00000e20: 6874 7470 733a 2f2f 7079 7069 2e6f 7267  https://pypi.org
-00000e30: 2f70 726f 6a65 6374 2f6d 6567 6164 6574  /project/megadet
-00000e40: 6563 746f 722f 2920 7468 6174 2070 726f  ector/) that pro
-00000e50: 7669 6465 7320 6163 6365 7373 2074 6f20  vides access to 
-00000e60: 6576 6572 7974 6869 6e67 2069 6e20 7468  everything in th
-00000e70: 6973 2072 6570 6f20 2879 6573 2c20 796f  is repo (yes, yo
-00000e80: 7520 6775 6573 7365 6420 6974 2c20 2270  u guessed it, "p
-00000e90: 6970 2069 6e73 7461 6c6c 206d 6567 6164  ip install megad
-00000ea0: 6574 6563 746f 7222 292e 0a0a 4d65 6761  etector")...Mega
-00000eb0: 4465 7465 6374 6f72 2069 7320 6a75 7374  Detector is just
-00000ec0: 206f 6e65 206f 6620 6d61 6e79 2074 6f6f   one of many too
-00000ed0: 6c73 2074 6861 7420 6169 6d73 2074 6f20  ls that aims to 
-00000ee0: 6d61 6b65 2063 6f6e 7365 7276 6174 696f  make conservatio
-00000ef0: 6e20 6269 6f6c 6f67 6973 7473 206d 6f72  n biologists mor
-00000f00: 6520 6566 6669 6369 656e 7420 7769 7468  e efficient with
-00000f10: 2041 492e 2020 4966 2079 6f75 2077 616e   AI.  If you wan
-00000f20: 7420 746f 206c 6561 726e 2061 626f 7574  t to learn about
-00000f30: 206f 7468 6572 2077 6179 7320 746f 2075   other ways to u
-00000f40: 7365 2041 4920 746f 2061 6363 656c 6572  se AI to acceler
-00000f50: 6174 6520 6361 6d65 7261 2074 7261 7020  ate camera trap 
-00000f60: 776f 726b 666c 6f77 732c 2063 6865 636b  workflows, check
-00000f70: 206f 7574 206f 7572 206f 6620 7468 6520   out our of the 
-00000f80: 6669 656c 642c 2061 6666 6563 7469 6f6e  field, affection
-00000f90: 6174 656c 7920 7469 746c 6564 2026 6c64  ately titled &ld
-00000fa0: 7175 6f3b 5b45 7665 7279 7468 696e 6720  quo;[Everything 
-00000fb0: 4920 6b6e 6f77 2061 626f 7574 206d 6163  I know about mac
-00000fc0: 6869 6e65 206c 6561 726e 696e 6720 616e  hine learning an
-00000fd0: 6420 6361 6d65 7261 2074 7261 7073 5d28  d camera traps](
-00000fe0: 6874 7470 733a 2f2f 6167 656e 746d 6f72  https://agentmor
-00000ff0: 7269 732e 6769 7468 7562 2e69 6f2f 6361  ris.github.io/ca
-00001000: 6d65 7261 2d74 7261 702d 6d6c 2d73 7572  mera-trap-ml-sur
-00001010: 7665 792f 2926 7264 7175 6f3b 2e0a 0a0a  vey/)&rdquo;....
-00001020: 2323 2057 686f 2069 7320 7573 696e 6720  ## Who is using 
-00001030: 4d65 6761 4465 7465 6374 6f72 3f0a 0a57  MegaDetector?..W
-00001040: 6520 776f 726b 2077 6974 6820 6563 6f6c  e work with ecol
-00001050: 6f67 6973 7473 2061 6c6c 206f 7665 7220  ogists all over 
-00001060: 7468 6520 776f 726c 6420 746f 2068 656c  the world to hel
-00001070: 7020 7468 656d 2073 7065 6e64 206c 6573  p them spend les
-00001080: 7320 7469 6d65 2061 6e6e 6f74 6174 696e  s time annotatin
-00001090: 6720 696d 6167 6573 2061 6e64 206d 6f72  g images and mor
-000010a0: 6520 7469 6d65 2074 6869 6e6b 696e 6720  e time thinking 
-000010b0: 6162 6f75 7420 636f 6e73 6572 7661 7469  about conservati
-000010c0: 6f6e 2e20 2059 6f75 2063 616e 2072 6561  on.  You can rea
-000010d0: 6420 6120 6c69 7474 6c65 206d 6f72 6520  d a little more 
-000010e0: 6162 6f75 7420 686f 7720 7468 6973 2077  about how this w
-000010f0: 6f72 6b73 206f 6e20 6f75 7220 5b67 6574  orks on our [get
-00001100: 7469 6e67 2073 7461 7274 6564 2077 6974  ting started wit
-00001110: 6820 4d65 6761 4465 7465 6374 6f72 5d28  h MegaDetector](
-00001120: 636f 6c6c 6162 6f72 6174 696f 6e73 2e6d  collaborations.m
-00001130: 6429 2070 6167 652e 0a0a 4865 7265 2061  d) page...Here a
-00001140: 7265 2061 2066 6577 206f 6620 7468 6520  re a few of the 
-00001150: 6f72 6761 6e69 7a61 7469 6f6e 7320 7468  organizations th
-00001160: 6174 2068 6176 6520 7573 6564 204d 6567  at have used Meg
-00001170: 6144 6574 6563 746f 722e 2e2e 2077 6527  aDetector... we'
-00001180: 7265 206f 6e6c 7920 6c69 7374 696e 6720  re only listing 
-00001190: 6f72 6761 6e69 7a61 7469 6f6e 7320 7768  organizations wh
-000011a0: 6f20 2861 2920 7765 206b 6e6f 7720 6162  o (a) we know ab
-000011b0: 6f75 7420 616e 6420 2862 2920 6861 7665  out and (b) have
-000011c0: 2067 6976 656e 2075 7320 7065 726d 6973   given us permis
-000011d0: 7369 6f6e 2074 6f20 7265 6665 7220 746f  sion to refer to
-000011e0: 2074 6865 6d20 6865 7265 2028 6f72 2068   them here (or h
-000011f0: 6176 6520 706f 7374 6564 2070 7562 6c69  ave posted publi
-00001200: 636c 7920 6162 6f75 7420 7468 6569 7220  cly about their 
-00001210: 7573 6520 6f66 204d 6567 6144 6574 6563  use of MegaDetec
-00001220: 746f 7229 2c20 736f 2069 6620 796f 7527  tor), so if you'
-00001230: 7265 2075 7369 6e67 204d 6567 6144 6574  re using MegaDet
-00001240: 6563 746f 7220 6f72 206f 7468 6572 2074  ector or other t
-00001250: 6f6f 6c73 2066 726f 6d20 7468 6973 2072  ools from this r
-00001260: 6570 6f20 616e 6420 776f 756c 6420 6c69  epo and would li
-00001270: 6b65 2074 6f20 6265 2061 6464 6564 2074  ke to be added t
-00001280: 6f20 7468 6973 206c 6973 742c 203c 6120  o this list, <a 
-00001290: 6872 6566 3d22 6d61 696c 746f 3a63 616d  href="mailto:cam
-000012a0: 6572 6174 7261 7073 406c 696c 612e 7363  eratraps@lila.sc
-000012b0: 6965 6e63 6522 3e65 6d61 696c 2075 733c  ience">email us<
-000012c0: 2f61 3e21 0a0a 2a20 5b41 7269 7a6f 6e61  /a>!..* [Arizona
-000012d0: 2044 6570 6172 746d 656e 7420 6f66 2045   Department of E
-000012e0: 6e76 6972 6f6e 6d65 6e74 616c 2051 7561  nvironmental Qua
-000012f0: 6c69 7479 5d28 6874 7470 3a2f 2f61 7a64  lity](http://azd
-00001300: 6571 2e67 6f76 2f29 0a2a 205b 426c 6163  eq.gov/).* [Blac
-00001310: 6b62 6972 6420 456e 7669 726f 6e6d 656e  kbird Environmen
-00001320: 7461 6c5d 2868 7474 7073 3a2f 2f62 6c61  tal](https://bla
-00001330: 636b 6269 7264 656e 762e 636f 6d2f 290a  ckbirdenv.com/).
-00001340: 2a20 5b43 616d 656c 6f74 5d28 6874 7470  * [Camelot](http
-00001350: 733a 2f2f 6361 6d65 6c6f 7470 726f 6a65  s://camelotproje
-00001360: 6374 2e6f 7267 2f29 0a2a 205b 4361 6e61  ct.org/).* [Cana
-00001370: 6469 616e 2050 6172 6b73 2061 6e64 2057  dian Parks and W
-00001380: 696c 6465 726e 6573 7320 536f 6369 6574  ilderness Societ
-00001390: 7920 2843 5041 5753 2920 4e6f 7274 6865  y (CPAWS) Northe
-000013a0: 726e 2041 6c62 6572 7461 2043 6861 7074  rn Alberta Chapt
-000013b0: 6572 5d28 6874 7470 733a 2f2f 6370 6177  er](https://cpaw
-000013c0: 736e 6162 2e6f 7267 2f29 0a2a 205b 436f  snab.org/).* [Co
-000013d0: 6e73 6572 7661 7469 6f6e 2058 204c 6162  nservation X Lab
-000013e0: 735d 2868 7474 7073 3a2f 2f63 6f6e 7365  s](https://conse
-000013f0: 7276 6174 696f 6e78 6c61 6273 2e63 6f6d  rvationxlabs.com
-00001400: 2f29 0a2a 205b 437a 6563 6820 556e 6976  /).* [Czech Univ
-00001410: 6572 7369 7479 206f 6620 4c69 6665 2053  ersity of Life S
-00001420: 6369 656e 6365 7320 5072 6167 7565 5d28  ciences Prague](
-00001430: 6874 7470 733a 2f2f 7777 772e 637a 752e  https://www.czu.
-00001440: 637a 2f65 6e29 0a2a 205b 4475 6465 6b20  cz/en).* [Dudek 
-00001450: 4361 6d65 7261 2054 7261 7020 4149 2049  Camera Trap AI I
-00001460: 6d61 6765 2054 6f6f 6c6b 6974 2028 4149  mage Toolkit (AI
-00001470: 5429 5d28 6874 7470 733a 2f2f 6475 6465  T)](https://dude
-00001480: 6b2e 636f 6d2f 7365 7276 6963 6573 2f77  k.com/services/w
-00001490: 696c 646c 6966 652d 6361 6d65 7261 2d74  ildlife-camera-t
-000014a0: 7261 702d 6169 2d69 6d61 6765 2d70 726f  rap-ai-image-pro
-000014b0: 6365 7373 696e 672d 616e 642d 6d61 6e61  cessing-and-mana
-000014c0: 6765 6d65 6e74 2f29 0a2a 205b 4563 6f4c  gement/).* [EcoL
-000014d0: 6f67 6963 2043 6f6e 7375 6c74 616e 7473  ogic Consultants
-000014e0: 204c 7464 2e5d 2868 7474 7073 3a2f 2f77   Ltd.](https://w
-000014f0: 7777 2e63 6f6e 7375 6c74 2d65 636f 6c6f  ww.consult-ecolo
-00001500: 6769 632e 636f 6d2f 290a 2a20 5b45 7374  gic.com/).* [Est
-00001510: 6163 69c3 b36e 2042 696f 6cc3 b367 6963  aci..n Biol..gic
-00001520: 6120 6465 2044 6fc3 b161 6e61 5d28 6874  a de Do..ana](ht
-00001530: 7470 3a2f 2f77 7777 2e65 6264 2e63 7369  tp://www.ebd.csi
-00001540: 632e 6573 2f69 6e69 6369 6f29 0a2a 205b  c.es/inicio).* [
-00001550: 4964 6168 6f20 4465 7061 7274 6d65 6e74  Idaho Department
-00001560: 206f 6620 4669 7368 2061 6e64 2047 616d   of Fish and Gam
-00001570: 655d 2868 7474 7073 3a2f 2f69 6466 672e  e](https://idfg.
-00001580: 6964 6168 6f2e 676f 762f 290a 2a20 5b49  idaho.gov/).* [I
-00001590: 736c 616e 6420 436f 6e73 6572 7661 7469  sland Conservati
-000015a0: 6f6e 5d28 6874 7470 733a 2f2f 7777 772e  on](https://www.
-000015b0: 6973 6c61 6e64 636f 6e73 6572 7661 7469  islandconservati
-000015c0: 6f6e 2e6f 7267 2f29 0a2a 205b 4d79 616c  on.org/).* [Myal
-000015d0: 6c20 4c61 6b65 7320 4469 6e67 6f20 5072  l Lakes Dingo Pr
-000015e0: 6f6a 6563 745d 2868 7474 7073 3a2f 2f63  oject](https://c
-000015f0: 6172 6e69 766f 7265 636f 6578 6973 7465  arnivorecoexiste
-00001600: 6e63 652e 696e 666f 2f6d 7961 6c6c 2d6c  nce.info/myall-l
-00001610: 616b 6573 2d64 696e 676f 2d70 726f 6a65  akes-dingo-proje
-00001620: 6374 2f29 0a2a 205b 4e6f 7277 6567 6961  ct/).* [Norwegia
-00001630: 6e20 496e 7374 6974 7574 6520 666f 7220  n Institute for 
-00001640: 4e61 7475 7265 2052 6573 6561 7263 685d  Nature Research]
-00001650: 2868 7474 7073 3a2f 2f77 7777 2e6e 696e  (https://www.nin
-00001660: 612e 6e6f 2f65 6e67 6c69 7368 2f48 6f6d  a.no/english/Hom
-00001670: 6529 0a2a 205b 506f 696e 7420 4e6f 2050  e).* [Point No P
-00001680: 6f69 6e74 2054 7265 6174 7920 436f 756e  oint Treaty Coun
-00001690: 6369 6c5d 2868 7474 7073 3a2f 2f70 6e70  cil](https://pnp
-000016a0: 7463 2e6f 7267 2f29 0a2a 205b 5261 6d61  tc.org/).* [Rama
-000016b0: 7420 4861 6e61 6469 7620 4e61 7475 7265  t Hanadiv Nature
-000016c0: 2050 6172 6b5d 2868 7474 7073 3a2f 2f77   Park](https://w
-000016d0: 7777 2e72 616d 6174 2d68 616e 6164 6976  ww.ramat-hanadiv
-000016e0: 2e6f 7267 2e69 6c2f 656e 2f29 0a2a 205b  .org.il/en/).* [
-000016f0: 5350 4541 2028 506f 7274 7567 7565 7365  SPEA (Portuguese
-00001700: 2053 6f63 6965 7479 2066 6f72 2074 6865   Society for the
-00001710: 2053 7475 6479 206f 6620 4269 7264 7329   Study of Birds)
-00001720: 5d28 6874 7470 733a 2f2f 7370 6561 2e70  ](https://spea.p
-00001730: 742f 656e 2f29 0a2a 205b 536b 7920 4973  t/en/).* [Sky Is
-00001740: 6c61 6e64 2041 6c6c 6961 6e63 655d 2868  land Alliance](h
-00001750: 7474 7073 3a2f 2f73 6b79 6973 6c61 6e64  ttps://skyisland
-00001760: 616c 6c69 616e 6365 2e6f 7267 2f29 0a2a  alliance.org/).*
-00001770: 205b 5379 6e74 6865 7461 6963 5d28 6874   [Synthetaic](ht
-00001780: 7470 733a 2f2f 7777 772e 7379 6e74 6865  tps://www.synthe
-00001790: 7461 6963 2e63 6f6d 2f29 0a2a 205b 5461  taic.com/).* [Ta
-000017a0: 726f 6e67 6120 436f 6e73 6572 7661 7469  ronga Conservati
-000017b0: 6f6e 2053 6f63 6965 7479 5d28 6874 7470  on Society](http
-000017c0: 733a 2f2f 7461 726f 6e67 612e 6f72 672e  s://taronga.org.
-000017d0: 6175 2f29 0a2a 205b 5468 6520 4e61 7475  au/).* [The Natu
-000017e0: 7265 2043 6f6e 7365 7276 616e 6379 2069  re Conservancy i
-000017f0: 6e20 5779 6f6d 696e 675d 2868 7474 7073  n Wyoming](https
-00001800: 3a2f 2f77 7777 2e6e 6174 7572 652e 6f72  ://www.nature.or
-00001810: 672f 656e 2d75 732f 6162 6f75 742d 7573  g/en-us/about-us
-00001820: 2f77 6865 7265 2d77 652d 776f 726b 2f75  /where-we-work/u
-00001830: 6e69 7465 642d 7374 6174 6573 2f77 796f  nited-states/wyo
-00001840: 6d69 6e67 2f29 0a2a 205b 5472 6170 5461  ming/).* [TrapTa
-00001850: 6767 6572 5d28 6874 7470 733a 2f2f 7769  gger](https://wi
-00001860: 6c64 6579 6563 6f6e 7365 7276 6174 696f  ldeyeconservatio
-00001870: 6e2e 6f72 672f 7472 6170 2d74 6167 6765  n.org/trap-tagge
-00001880: 722d 6162 6f75 742f 290a 2a20 5b55 6e69  r-about/).* [Uni
-00001890: 7665 7273 6974 7920 6f66 2043 616c 6966  versity of Calif
-000018a0: 6f72 6e69 6120 4461 7669 7320 4e61 7475  ornia Davis Natu
-000018b0: 7261 6c20 5265 7365 7276 6573 5d28 6874  ral Reserves](ht
-000018c0: 7470 733a 2f2f 6e61 7475 7261 6c72 6573  tps://naturalres
-000018d0: 6572 7665 732e 7563 6461 7669 732e 6564  erves.ucdavis.ed
-000018e0: 752f 290a 2a20 5b55 7070 6572 2059 656c  u/).* [Upper Yel
-000018f0: 6c6f 7773 746f 6e65 2057 6174 6572 7368  lowstone Watersh
-00001900: 6564 2047 726f 7570 5d28 6874 7470 733a  ed Group](https:
-00001910: 2f2f 7777 772e 7570 7065 7279 656c 6c6f  //www.upperyello
-00001920: 7773 746f 6e65 2e6f 7267 2f29 0a2a 205b  wstone.org/).* [
-00001930: 5a61 6d62 6120 436c 6f75 645d 2868 7474  Zamba Cloud](htt
-00001940: 7073 3a2f 2f77 7777 2e7a 616d 6261 636c  ps://www.zambacl
-00001950: 6f75 642e 636f 6d2f 290a 2a20 5b50 6172  oud.com/).* [Par
-00001960: 6320 6e61 7469 6f6e 616c 2064 7520 4d6f  c national du Mo
-00001970: 6e74 2d54 7265 6d62 6c61 6e74 5d28 6874  nt-Tremblant](ht
-00001980: 7470 733a 2f2f 7777 772e 7365 7061 712e  tps://www.sepaq.
-00001990: 636f 6d2f 7071 2f6d 6f74 2f69 6e64 6578  com/pq/mot/index
-000019a0: 2e64 6f74 3f6c 616e 6775 6167 655f 6964  .dot?language_id
-000019b0: 3d31 290a 2a20 5b54 6865 204c 616e 6420  =1).* [The Land 
-000019c0: 4261 6e6b 696e 6720 4772 6f75 705d 2868  Banking Group](h
-000019d0: 7474 7073 3a2f 2f74 6865 6c61 6e64 6261  ttps://thelandba
-000019e0: 6e6b 696e 6767 726f 7570 2e63 6f6d 2f29  nkinggroup.com/)
-000019f0: 0a2a 205b 4e65 7720 5a65 616c 616e 6420  .* [New Zealand 
-00001a00: 4465 7061 7274 6d65 6e74 206f 6620 436f  Department of Co
-00001a10: 6e73 6572 7661 7469 6f6e 5d28 6874 7470  nservation](http
-00001a20: 733a 2f2f 7777 772e 646f 632e 676f 7674  s://www.doc.govt
-00001a30: 2e6e 7a29 0a0a 2a20 5b41 7070 6c69 6564  .nz)..* [Applied
-00001a40: 2043 6f6e 7365 7276 6174 696f 6e20 4d61   Conservation Ma
-00001a50: 6372 6f20 4563 6f6c 6f67 7920 4c61 625d  cro Ecology Lab]
-00001a60: 2868 7474 703a 2f2f 7777 772e 6163 6d65  (http://www.acme
-00001a70: 6c61 622e 6361 2f29 2c20 556e 6976 6572  lab.ca/), Univer
-00001a80: 7369 7479 206f 6620 5669 6374 6f72 6961  sity of Victoria
-00001a90: 0a2a 205b 4261 6e66 6620 4e61 7469 6f6e  .* [Banff Nation
-00001aa0: 616c 2050 6172 6b20 5265 736f 7572 6365  al Park Resource
-00001ab0: 2043 6f6e 7365 7276 6174 696f 6e5d 2868   Conservation](h
-00001ac0: 7474 7073 3a2f 2f77 7777 2e70 632e 6763  ttps://www.pc.gc
-00001ad0: 2e63 612f 656e 2f70 6e2d 6e70 2f61 622f  .ca/en/pn-np/ab/
-00001ae0: 6261 6e66 662f 6e61 7475 7265 2f63 6f6e  banff/nature/con
-00001af0: 7365 7276 6174 696f 6e29 2c20 5061 726b  servation), Park
-00001b00: 7320 4361 6e61 6461 0a2a 205b 426c 756d  s Canada.* [Blum
-00001b10: 7374 6569 6e20 4c61 625d 2868 7474 7073  stein Lab](https
-00001b20: 3a2f 2f62 6c75 6d73 7465 696e 6c61 622e  ://blumsteinlab.
-00001b30: 6565 622e 7563 6c61 2e65 6475 2f29 2c20  eeb.ucla.edu/), 
-00001b40: 5543 4c41 0a2a 205b 426f 7264 6572 6c61  UCLA.* [Borderla
-00001b50: 6e64 7320 5265 7365 6172 6368 2049 6e73  nds Research Ins
-00001b60: 7469 7475 7465 5d28 6874 7470 733a 2f2f  titute](https://
-00001b70: 6272 692e 7375 6c72 6f73 732e 6564 752f  bri.sulross.edu/
-00001b80: 292c 2053 756c 2052 6f73 7320 5374 6174  ), Sul Ross Stat
-00001b90: 6520 556e 6976 6572 7369 7479 0a2a 205b  e University.* [
-00001ba0: 4361 7069 746f 6c20 5265 6566 204e 6174  Capitol Reef Nat
-00001bb0: 696f 6e61 6c20 5061 726b 5d28 6874 7470  ional Park](http
-00001bc0: 733a 2f2f 7777 772e 6e70 732e 676f 762f  s://www.nps.gov/
-00001bd0: 6361 7265 2f69 6e64 6578 2e68 746d 2920  care/index.htm) 
-00001be0: 2f20 5574 6168 2056 616c 6c65 7920 556e  / Utah Valley Un
-00001bf0: 6976 6572 7369 7479 0a2a 205b 4365 6e74  iversity.* [Cent
-00001c00: 6572 2066 6f72 2042 696f 6469 7665 7273  er for Biodivers
-00001c10: 6974 7920 616e 6420 436f 6e73 6572 7661  ity and Conserva
-00001c20: 7469 6f6e 5d28 6874 7470 733a 2f2f 7777  tion](https://ww
-00001c30: 772e 616d 6e68 2e6f 7267 2f72 6573 6561  w.amnh.org/resea
-00001c40: 7263 682f 6365 6e74 6572 2d66 6f72 2d62  rch/center-for-b
-00001c50: 696f 6469 7665 7273 6974 792d 636f 6e73  iodiversity-cons
-00001c60: 6572 7661 7469 6f6e 292c 2041 6d65 7269  ervation), Ameri
-00001c70: 6361 6e20 4d75 7365 756d 206f 6620 4e61  can Museum of Na
-00001c80: 7475 7261 6c20 4869 7374 6f72 790a 2a20  tural History.* 
-00001c90: 5b43 656e 7472 6520 666f 7220 4563 6f73  [Centre for Ecos
-00001ca0: 7973 7465 6d20 5363 6965 6e63 655d 2868  ystem Science](h
-00001cb0: 7474 7073 3a2f 2f77 7777 2e75 6e73 772e  ttps://www.unsw.
-00001cc0: 6564 752e 6175 2f72 6573 6561 7263 682f  edu.au/research/
-00001cd0: 292c 2055 4e53 5720 5379 646e 6579 0a2a  ), UNSW Sydney.*
-00001ce0: 205b 4372 6f73 732d 4375 6c74 7572 616c   [Cross-Cultural
-00001cf0: 2045 636f 6c6f 6779 204c 6162 5d28 6874   Ecology Lab](ht
-00001d00: 7470 733a 2f2f 6372 6f73 7363 756c 7475  tps://crosscultu
-00001d10: 7261 6c65 636f 6c6f 6779 2e6e 6574 2f29  ralecology.net/)
-00001d20: 2c20 4d61 6371 7561 7269 6520 556e 6976  , Macquarie Univ
-00001d30: 6572 7369 7479 0a2a 205b 4443 2043 6174  ersity.* [DC Cat
-00001d40: 2043 6f75 6e74 5d28 6874 7470 733a 2f2f   Count](https://
-00001d50: 6875 622e 6463 6361 7463 6f75 6e74 2e6f  hub.dccatcount.o
-00001d60: 7267 2f29 2c20 6c65 6420 6279 2074 6865  rg/), led by the
-00001d70: 2048 756d 616e 6520 5265 7363 7565 2041   Humane Rescue A
-00001d80: 6c6c 6961 6e63 650a 2a20 5b44 6570 6172  lliance.* [Depar
-00001d90: 746d 656e 7420 6f66 2046 6973 6820 616e  tment of Fish an
-00001da0: 6420 5769 6c64 6c69 6665 2053 6369 656e  d Wildlife Scien
-00001db0: 6365 735d 2868 7474 7073 3a2f 2f77 7777  ces](https://www
-00001dc0: 2e75 6964 6168 6f2e 6564 752f 636e 722f  .uidaho.edu/cnr/
-00001dd0: 6465 7061 7274 6d65 6e74 732f 6669 7368  departments/fish
-00001de0: 2d61 6e64 2d77 696c 646c 6966 652d 7363  -and-wildlife-sc
-00001df0: 6965 6e63 6573 292c 2055 6e69 7665 7273  iences), Univers
-00001e00: 6974 7920 6f66 2049 6461 686f 0a2a 205b  ity of Idaho.* [
-00001e10: 4465 7061 7274 6d65 6e74 206f 6620 5769  Department of Wi
-00001e20: 6c64 6c69 6665 2045 636f 6c6f 6779 2061  ldlife Ecology a
-00001e30: 6e64 2043 6f6e 7365 7276 6174 696f 6e5d  nd Conservation]
-00001e40: 2868 7474 7073 3a2f 2f77 6563 2e69 6661  (https://wec.ifa
-00001e50: 732e 7566 6c2e 6564 752f 292c 2055 6e69  s.ufl.edu/), Uni
-00001e60: 7665 7273 6974 7920 6f66 2046 6c6f 7269  versity of Flori
-00001e70: 6461 0a2a 205b 4563 6f6c 6f67 7920 616e  da.* [Ecology an
-00001e80: 6420 436f 6e73 6572 7661 7469 6f6e 206f  d Conservation o
-00001e90: 6620 416d 617a 6f6e 6961 6e20 5665 7274  f Amazonian Vert
-00001ea0: 6562 7261 7465 7320 5265 7365 6172 6368  ebrates Research
-00001eb0: 2047 726f 7570 5d28 6874 7470 733a 2f2f   Group](https://
-00001ec0: 7777 772e 7265 7365 6172 6368 6761 7465  www.researchgate
-00001ed0: 2e6e 6574 2f6c 6162 2f46 6572 6e61 6e64  .net/lab/Fernand
-00001ee0: 612d 4d69 6368 616c 736b 692d 4c61 622d  a-Michalski-Lab-
-00001ef0: 3429 2c20 4665 6465 7261 6c20 556e 6976  4), Federal Univ
-00001f00: 6572 7369 7479 206f 6620 416d 6170 c3a1  ersity of Amap..
-00001f10: 0a2a 205b 476f 6c61 2046 6f72 6573 7420  .* [Gola Forest 
-00001f20: 5072 6f67 7261 6d6d 615d 2868 7474 7073  Programma](https
-00001f30: 3a2f 2f77 7777 2e72 7370 622e 6f72 672e  ://www.rspb.org.
-00001f40: 756b 2f6f 7572 2d77 6f72 6b2f 636f 6e73  uk/our-work/cons
-00001f50: 6572 7661 7469 6f6e 2f70 726f 6a65 6374  ervation/project
-00001f60: 732f 7363 6965 6e74 6966 6963 2d73 7570  s/scientific-sup
-00001f70: 706f 7274 2d66 6f72 2d74 6865 2d67 6f6c  port-for-the-gol
-00001f80: 612d 666f 7265 7374 2d70 726f 6772 616d  a-forest-program
-00001f90: 6d65 2f29 2c20 526f 7961 6c20 536f 6369  me/), Royal Soci
-00001fa0: 6574 7920 666f 7220 7468 6520 5072 6f74  ety for the Prot
-00001fb0: 6563 7469 6f6e 206f 6620 4269 7264 7320  ection of Birds 
-00001fc0: 2852 5350 4229 0a2a 205b 4772 6165 6d65  (RSPB).* [Graeme
-00001fd0: 2053 6861 6e6e 6f6e 2773 2052 6573 6561   Shannon's Resea
-00001fe0: 7263 6820 4772 6f75 705d 2868 7474 7073  rch Group](https
-00001ff0: 3a2f 2f77 696c 646c 6966 6572 6573 6561  ://wildliferesea
-00002000: 7263 682e 636f 2e75 6b2f 6772 6f75 702d  rch.co.uk/group-
-00002010: 3129 2c20 4261 6e67 6f72 2055 6e69 7665  1), Bangor Unive
-00002020: 7273 6974 7920 0a2a 205b 4861 6d61 6172  rsity .* [Hamaar
-00002030: 6167 5d28 6874 7470 733a 2f2f 6861 6d61  ag](https://hama
-00002040: 6172 6167 2e6f 7267 2e69 6c2f 292c 2054  arag.org.il/), T
-00002050: 6865 2053 7465 696e 6861 7264 7420 4d75  he Steinhardt Mu
-00002060: 7365 756d 206f 6620 4e61 7475 7261 6c20  seum of Natural 
-00002070: 4869 7374 6f72 792c 2054 656c 2041 7669  History, Tel Avi
-00002080: 7620 556e 6976 6572 7369 7479 0a2a 205b  v University.* [
-00002090: 496e 7374 6974 7574 2064 6573 2053 6369  Institut des Sci
-000020a0: 656e 6365 2064 6520 6c61 2046 6f72 c3aa  ence de la For..
-000020b0: 7420 5465 6d70 c3a9 72c3 a965 5d28 6874  t Temp..r..e](ht
-000020c0: 7470 733a 2f2f 6973 666f 7274 2e75 716f  tps://isfort.uqo
-000020d0: 2e63 612f 2920 2849 5346 4f52 5429 2c20  .ca/) (ISFORT), 
-000020e0: 556e 6976 6572 7369 74c3 a920 6475 2051  Universit.. du Q
-000020f0: 75c3 a962 6563 2065 6e20 4f75 7461 6f75  u..bec en Outaou
-00002100: 6169 730a 2a20 5b4c 6162 206f 6620 4472  ais.* [Lab of Dr
-00002110: 2e20 4269 6c61 6c20 4861 6269 625d 2868  . Bilal Habib](h
-00002120: 7474 7073 3a2f 2f62 686c 6162 2e69 6e2f  ttps://bhlab.in/
-00002130: 6162 6f75 7429 2c20 7468 6520 5769 6c64  about), the Wild
-00002140: 6c69 6665 2049 6e73 7469 7475 7465 206f  life Institute o
-00002150: 6620 496e 6469 610a 2a20 5b4d 616d 6d61  f India.* [Mamma
-00002160: 6c20 5370 6174 6961 6c20 4563 6f6c 6f67  l Spatial Ecolog
-00002170: 7920 616e 6420 436f 6e73 6572 7661 7469  y and Conservati
-00002180: 6f6e 204c 6162 5d28 6874 7470 733a 2f2f  on Lab](https://
-00002190: 6c61 6273 2e77 7375 2e65 6475 2f64 7468  labs.wsu.edu/dth
-000021a0: 6f72 6e74 6f6e 2f29 2c20 5761 7368 696e  ornton/), Washin
-000021b0: 6774 6f6e 2053 7461 7465 2055 6e69 7665  gton State Unive
-000021c0: 7273 6974 790a 2a20 5b4d 634c 6f75 6768  rsity.* [McLough
-000021d0: 6c69 6e20 4c61 6220 696e 2050 6f70 756c  lin Lab in Popul
-000021e0: 6174 696f 6e20 4563 6f6c 6f67 795d 2868  ation Ecology](h
-000021f0: 7474 703a 2f2f 6d63 6c6f 7567 686c 696e  ttp://mcloughlin
-00002200: 6c61 622e 6361 2f6c 6162 2f29 2c20 556e  lab.ca/lab/), Un
-00002210: 6976 6572 7369 7479 206f 6620 5361 736b  iversity of Sask
-00002220: 6174 6368 6577 616e 0a2a 205b 4e61 7469  atchewan.* [Nati
-00002230: 6f6e 616c 2057 696c 646c 6966 6520 5265  onal Wildlife Re
-00002240: 6675 6765 2053 7973 7465 6d2c 2053 6f75  fuge System, Sou
-00002250: 7468 7765 7374 2052 6567 696f 6e5d 2868  thwest Region](h
-00002260: 7474 7073 3a2f 2f77 7777 2e66 7773 2e67  ttps://www.fws.g
-00002270: 6f76 2f61 626f 7574 2f72 6567 696f 6e2f  ov/about/region/
-00002280: 736f 7574 6877 6573 7429 2c20 552e 532e  southwest), U.S.
-00002290: 2046 6973 6820 2620 5769 6c64 6c69 6665   Fish & Wildlife
-000022a0: 2053 6572 7669 6365 0a2a 205b 4e6f 7274   Service.* [Nort
-000022b0: 6865 726e 2047 7265 6174 2050 6c61 696e  hern Great Plain
-000022c0: 7320 5072 6f67 7261 6d5d 2868 7474 7073  s Program](https
-000022d0: 3a2f 2f6e 6174 696f 6e61 6c7a 6f6f 2e73  ://nationalzoo.s
-000022e0: 692e 6564 752f 6e65 7773 2f72 6573 746f  i.edu/news/resto
-000022f0: 7269 6e67 2d61 6d65 7269 6361 732d 7072  ring-americas-pr
-00002300: 6169 7269 6529 2c20 536d 6974 6873 6f6e  airie), Smithson
-00002310: 6961 6e0a 2a20 5b50 6f6c 6172 2045 636f  ian.* [Polar Eco
-00002320: 6c6f 6779 2047 726f 7570 5d28 6874 7470  logy Group](http
-00002330: 733a 2f2f 706f 6c61 7265 636f 6c6f 6779  s://polarecology
-00002340: 6772 6f75 702e 776f 7264 7072 6573 732e  group.wordpress.
-00002350: 636f 6d29 2c20 556e 6976 6572 7369 7479  com), University
-00002360: 206f 6620 4764 616e 736b 0a2a 205b 5175   of Gdansk.* [Qu
-00002370: 616e 7469 7461 7469 7665 2045 636f 6c6f  antitative Ecolo
-00002380: 6779 204c 6162 5d28 6874 7470 733a 2f2f  gy Lab](https://
-00002390: 6465 7074 732e 7761 7368 696e 6774 6f6e  depts.washington
-000023a0: 2e65 6475 2f73 6566 7371 656c 2f29 2c20  .edu/sefsqel/), 
-000023b0: 556e 6976 6572 7369 7479 206f 6620 5761  University of Wa
-000023c0: 7368 696e 6774 6f6e 0a2a 205b 5361 6e74  shington.* [Sant
-000023d0: 6120 4d6f 6e69 6361 204d 6f75 6e74 6169  a Monica Mountai
-000023e0: 6e73 2052 6563 7265 6174 696f 6e20 4172  ns Recreation Ar
-000023f0: 6561 5d28 6874 7470 733a 2f2f 7777 772e  ea](https://www.
-00002400: 6e70 732e 676f 762f 7361 6d6f 2f69 6e64  nps.gov/samo/ind
-00002410: 6578 2e68 746d 292c 204e 6174 696f 6e61  ex.htm), Nationa
-00002420: 6c20 5061 726b 2053 6572 7669 6365 0a2a  l Park Service.*
-00002430: 205b 5365 6174 746c 6520 5572 6261 6e20   [Seattle Urban 
-00002440: 4361 726e 6976 6f72 6520 5072 6f6a 6563  Carnivore Projec
-00002450: 745d 2868 7474 7073 3a2f 2f77 7777 2e7a  t](https://www.z
-00002460: 6f6f 2e6f 7267 2f73 6561 7474 6c65 6361  oo.org/seattleca
-00002470: 726e 6976 6f72 6573 292c 2057 6f6f 646c  rnivores), Woodl
-00002480: 616e 6420 5061 726b 205a 6f6f 0a2a 205b  and Park Zoo.* [
-00002490: 5365 7272 6120 646f 7320 c393 7267 c3a3  Serra dos ..rg..
-000024a0: 6f73 204e 6174 696f 6e61 6c20 5061 726b  os National Park
-000024b0: 5d28 6874 7470 733a 2f2f 7777 772e 6963  ](https://www.ic
-000024c0: 6d62 696f 2e67 6f76 2e62 722f 7061 726e  mbio.gov.br/parn
-000024d0: 6173 6572 7261 646f 736f 7267 616f 732f  aserradosorgaos/
-000024e0: 292c 2049 434d 4269 6f0a 2a20 5b53 6e61  ), ICMBio.* [Sna
-000024f0: 7073 686f 7420 5553 415d 2868 7474 7073  pshot USA](https
-00002500: 3a2f 2f65 6d61 6d6d 616c 2e73 692e 6564  ://emammal.si.ed
-00002510: 752f 736e 6170 7368 6f74 2d75 7361 292c  u/snapshot-usa),
-00002520: 2053 6d69 7468 736f 6e69 616e 0a2a 205b   Smithsonian.* [
-00002530: 5769 6c64 6c69 6665 2043 6f65 7869 7374  Wildlife Coexist
-00002540: 656e 6365 204c 6162 5d28 6874 7470 733a  ence Lab](https:
-00002550: 2f2f 7769 6c64 6c69 6665 2e66 6f72 6573  //wildlife.fores
-00002560: 7472 792e 7562 632e 6361 2f29 2c20 556e  try.ubc.ca/), Un
-00002570: 6976 6572 7369 7479 206f 6620 4272 6974  iversity of Brit
-00002580: 6973 6820 436f 6c75 6d62 6961 0a2a 205b  ish Columbia.* [
-00002590: 5769 6c64 6c69 6665 2052 6573 6561 7263  Wildlife Researc
-000025a0: 685d 2868 7474 7073 3a2f 2f77 7777 2e64  h](https://www.d
-000025b0: 6677 2e73 7461 7465 2e6f 722e 7573 2f77  fw.state.or.us/w
-000025c0: 696c 646c 6966 652f 7265 7365 6172 6368  ildlife/research
-000025d0: 2f69 6e64 6578 2e61 7370 292c 204f 7265  /index.asp), Ore
-000025e0: 676f 6e20 4465 7061 7274 6d65 6e74 206f  gon Department o
-000025f0: 6620 4669 7368 2061 6e64 2057 696c 646c  f Fish and Wildl
-00002600: 6966 650a 2a20 5b57 696c 646c 6966 6520  ife.* [Wildlife 
-00002610: 4469 7669 7369 6f6e 5d28 6874 7470 733a  Division](https:
-00002620: 2f2f 7777 772e 6d69 6368 6967 616e 2e67  //www.michigan.g
-00002630: 6f76 2f64 6e72 2f61 626f 7574 2f63 6f6e  ov/dnr/about/con
-00002640: 7461 6374 2f77 696c 646c 6966 6529 2c20  tact/wildlife), 
-00002650: 4d69 6368 6967 616e 2044 6570 6172 746d  Michigan Departm
-00002660: 656e 7420 6f66 204e 6174 7572 616c 2052  ent of Natural R
-00002670: 6573 6f75 7263 6573 0a0a 2a20 4465 7061  esources..* Depa
-00002680: 7274 6d65 6e74 206f 6620 4563 6f6c 6f67  rtment of Ecolog
-00002690: 792c 2054 5520 4265 726c 696e 0a2a 2047  y, TU Berlin.* G
-000026a0: 686f 7374 2043 6174 2041 6e61 6c79 7469  host Cat Analyti
-000026b0: 6373 0a2a 2050 726f 7465 6374 6564 2041  cs.* Protected A
-000026c0: 7265 6173 2055 6e69 742c 2043 616e 6164  reas Unit, Canad
-000026d0: 6961 6e20 5769 6c64 6c69 6665 2053 6572  ian Wildlife Ser
-000026e0: 7669 6365 0a0a 2a20 5b53 6368 6f6f 6c20  vice..* [School 
-000026f0: 6f66 204e 6174 7572 616c 2053 6369 656e  of Natural Scien
-00002700: 6365 735d 2868 7474 7073 3a2f 2f77 7777  ces](https://www
-00002710: 2e75 7461 732e 6564 752e 6175 2f6e 6174  .utas.edu.au/nat
-00002720: 7572 616c 2d73 6369 656e 6365 7329 2c20  ural-sciences), 
-00002730: 556e 6976 6572 7369 7479 206f 6620 5461  University of Ta
-00002740: 736d 616e 6961 2028 5b73 746f 7279 5d28  smania ([story](
-00002750: 6874 7470 733a 2f2f 7777 772e 7574 6173  https://www.utas
-00002760: 2e65 6475 2e61 752f 6162 6f75 742f 6e65  .edu.au/about/ne
-00002770: 7773 2d61 6e64 2d73 746f 7269 6573 2f61  ws-and-stories/a
-00002780: 7274 6963 6c65 732f 3230 3232 2f31 3230  rticles/2022/120
-00002790: 342d 696e 6e6f 7661 7469 7665 2d63 616d  4-innovative-cam
-000027a0: 6572 612d 6e65 7477 6f72 6b2d 6b65 6570  era-network-keep
-000027b0: 732d 636c 6f73 652d 6579 652d 6f6e 2d74  s-close-eye-on-t
-000027c0: 6173 7369 652d 7769 6c64 6c69 6665 2929  assie-wildlife))
-000027d0: 0a2a 205b 4b65 6e61 6920 4e61 7469 6f6e  .* [Kenai Nation
-000027e0: 616c 2057 696c 646c 6966 6520 5265 6675  al Wildlife Refu
-000027f0: 6765 5d28 6874 7470 733a 2f2f 7777 772e  ge](https://www.
-00002800: 6677 732e 676f 762f 7265 6675 6765 2f6b  fws.gov/refuge/k
-00002810: 656e 6169 292c 2055 2e53 2e20 4669 7368  enai), U.S. Fish
-00002820: 2026 2057 696c 646c 6966 6520 5365 7276   & Wildlife Serv
-00002830: 6963 6520 285b 7374 6f72 795d 2868 7474  ice ([story](htt
-00002840: 7073 3a2f 2f77 7777 2e70 656e 696e 7375  ps://www.peninsu
-00002850: 6c61 636c 6172 696f 6e2e 636f 6d2f 7370  laclarion.com/sp
-00002860: 6f72 7473 2f72 6566 7567 652d 6e6f 7465  orts/refuge-note
-00002870: 626f 6f6b 2d6e 6577 2d74 6563 686e 6f6c  book-new-technol
-00002880: 6f67 792d 696e 6372 6561 7365 732d 6566  ogy-increases-ef
-00002890: 6669 6369 656e 6379 2d6f 662d 7265 6675  ficiency-of-refu
-000028a0: 6765 2d63 616d 6572 6173 2f29 290a 0a2a  ge-cameras/))..*
-000028b0: 205b 4175 7374 7261 6c69 616e 2057 696c   [Australian Wil
-000028c0: 646c 6966 6520 436f 6e73 6572 7661 6e63  dlife Conservanc
-000028d0: 795d 2868 7474 7073 3a2f 2f77 7777 2e61  y](https://www.a
-000028e0: 7573 7472 616c 6961 6e77 696c 646c 6966  ustralianwildlif
-000028f0: 652e 6f72 672f 2920 2862 6c6f 6720 706f  e.org/) (blog po
-00002900: 7374 7320 5b31 5d28 6874 7470 733a 2f2f  sts [1](https://
-00002910: 7777 772e 6175 7374 7261 6c69 616e 7769  www.australianwi
-00002920: 6c64 6c69 6665 2e6f 7267 2f63 7574 7469  ldlife.org/cutti
-00002930: 6e67 2d65 6467 652d 7465 6368 6e6f 6c6f  ng-edge-technolo
-00002940: 6779 2d64 656c 6976 6572 696e 672d 6566  gy-delivering-ef
-00002950: 6669 6369 656e 6379 2d67 6169 6e73 2d69  ficiency-gains-i
-00002960: 6e2d 636f 6e73 6572 7661 7469 6f6e 2f29  n-conservation/)
-00002970: 2c20 5b32 5d28 6874 7470 733a 2f2f 7777  , [2](https://ww
-00002980: 772e 6175 7374 7261 6c69 616e 7769 6c64  w.australianwild
-00002990: 6c69 6665 2e6f 7267 2f65 6666 6963 6965  life.org/efficie
-000029a0: 6e63 792d 6761 696e 732d 6174 2d74 6865  ncy-gains-at-the
-000029b0: 2d63 7574 7469 6e67 2d65 6467 652d 6f66  -cutting-edge-of
-000029c0: 2d74 6563 686e 6f6c 6f67 792f 2929 0a2a  -technology/)).*
-000029d0: 205b 4261 7661 7269 616e 2046 6f72 6573   [Bavarian Fores
-000029e0: 7420 4e61 7469 6f6e 616c 2050 6172 6b5d  t National Park]
-000029f0: 2868 7474 7073 3a2f 2f77 7777 2e6e 6174  (https://www.nat
-00002a00: 696f 6e61 6c70 6172 6b2d 6261 7965 7269  ionalpark-bayeri
-00002a10: 7363 6865 722d 7761 6c64 2e62 6179 6572  scher-wald.bayer
-00002a20: 6e2e 6465 2f65 6e67 6c69 7368 2f69 6e64  n.de/english/ind
-00002a30: 6578 2e68 746d 2920 285b 7374 6f72 795d  ex.htm) ([story]
-00002a40: 2868 7474 7073 3a2f 2f63 7573 746f 6d65  (https://custome
-00002a50: 7273 2e6d 6963 726f 736f 6674 2e63 6f6d  rs.microsoft.com
-00002a60: 2f65 6e2d 6175 2f73 746f 7279 2f31 3636  /en-au/story/166
-00002a70: 3735 3339 3533 3932 3731 3234 3737 3937  7539539271247797
-00002a80: 2d6e 6174 696f 6e61 6c70 6172 6b62 6179  -nationalparkbay
-00002a90: 6572 6973 6368 6572 7761 6c64 2d61 7a75  erischerwald-azu
-00002aa0: 7265 2d65 6e29 290a 2a20 5b46 656c 6964  re-en)).* [Felid
-00002ab0: 6165 2043 6f6e 7365 7276 6174 696f 6e20  ae Conservation 
-00002ac0: 4675 6e64 5d28 6874 7470 733a 2f2f 6665  Fund](https://fe
-00002ad0: 6c69 6461 6566 756e 642e 6f72 672f 2920  lidaefund.org/) 
-00002ae0: 285b 5769 6c64 6550 6f64 2070 6c61 7466  ([WildePod platf
-00002af0: 6f72 6d5d 2868 7474 7073 3a2f 2f77 696c  orm](https://wil
-00002b00: 6465 706f 642e 6f72 672f 2929 2028 5b62  depod.org/)) ([b
-00002b10: 6c6f 6720 706f 7374 5d28 6874 7470 733a  log post](https:
-00002b20: 2f2f 6162 6861 796b 6173 6879 6170 2e63  //abhaykashyap.c
-00002b30: 6f6d 2f62 6c6f 672f 6169 2d70 6f77 6572  om/blog/ai-power
-00002b40: 6564 2d63 616d 6572 612d 7472 6170 2d69  ed-camera-trap-i
-00002b50: 6d61 6765 2d61 6e6e 6f74 6174 696f 6e2d  mage-annotation-
-00002b60: 7379 7374 656d 2f29 290a 2a20 5b41 6c62  system/)).* [Alb
-00002b70: 6572 7461 2042 696f 6469 7665 7273 6974  erta Biodiversit
-00002b80: 7920 4d6f 6e69 746f 7269 6e67 2049 6e73  y Monitoring Ins
-00002b90: 7469 7475 7465 2028 4142 4d49 295d 2868  titute (ABMI)](h
-00002ba0: 7474 7073 3a2f 2f77 7777 2e61 626d 692e  ttps://www.abmi.
-00002bb0: 6361 2f68 6f6d 652e 6874 6d6c 2920 285b  ca/home.html) ([
-00002bc0: 5769 6c64 5472 6178 2070 6c61 7466 6f72  WildTrax platfor
-00002bd0: 6d5d 2868 7474 7073 3a2f 2f77 7777 2e77  m](https://www.w
-00002be0: 696c 6474 7261 782e 6361 2f29 2920 2862  ildtrax.ca/)) (b
-00002bf0: 6c6f 6720 706f 7374 7320 5b31 5d28 6874  log posts [1](ht
-00002c00: 7470 733a 2f2f 7769 6c64 6361 6d73 2e63  tps://wildcams.c
-00002c10: 612f 626c 6f67 2f74 6865 2d61 626d 692d  a/blog/the-abmi-
-00002c20: 7669 7369 7473 2d74 6865 2d7a 6f6f 2f29  visits-the-zoo/)
-00002c30: 2c5b 325d 2868 7474 703a 2f2f 626c 6f67  ,[2](http://blog
-00002c40: 2e61 626d 692e 6361 2f32 3032 332f 3036  .abmi.ca/2023/06
-00002c50: 2f31 342f 6d61 6b69 6e67 2d77 696c 6474  /14/making-wildt
-00002c60: 7261 782d 6974 732d 6e6f 742d 612d 6b69  rax-its-not-a-ki
-00002c70: 6e64 2d6f 662d 6d61 6769 632d 6265 6869  nd-of-magic-behi
-00002c80: 6e64 2d74 6865 2d73 6372 6565 6e2f 2929  nd-the-screen/))
-00002c90: 0a2a 205b 5368 616e 2053 6875 6920 436f  .* [Shan Shui Co
-00002ca0: 6e73 6572 7661 7469 6f6e 2043 656e 7465  nservation Cente
-00002cb0: 725d 2868 7474 703a 2f2f 656e 2e73 6861  r](http://en.sha
-00002cc0: 6e73 6875 692e 6f72 672f 2920 285b 626c  nshui.org/) ([bl
-00002cd0: 6f67 2070 6f73 745d 2868 7474 7073 3a2f  og post](https:/
-00002ce0: 2f6d 702e 7765 6978 696e 2e71 712e 636f  /mp.weixin.qq.co
-00002cf0: 6d2f 732f 694f 4951 4633 636b 6a30 2d72  m/s/iOIQF3ckj0-r
-00002d00: 4547 3479 4a67 6572 5977 3f66 6263 6c69  EG4yJgerYw?fbcli
-00002d10: 643d 4977 4152 3061 6c77 6957 6265 3375  d=IwAR0alwiWbe3u
-00002d20: 6449 6346 7671 7177 6d37 7935 7167 7239  dIcFvqqwm7y5qgr9
-00002d30: 685a 706a 7238 3731 465a 4961 2d45 7247  hZpjr871FZIa-ErG
-00002d40: 5575 6b5a 3779 4a33 5a68 6743 6576 7329  UukZ7yJ3ZhgCevs)
-00002d50: 2920 285b 7472 616e 736c 6174 6564 2062  ) ([translated b
-00002d60: 6c6f 6720 706f 7374 5d28 6874 7470 733a  log post](https:
-00002d70: 2f2f 6d70 2d77 6569 7869 6e2d 7171 2d63  //mp-weixin-qq-c
-00002d80: 6f6d 2e74 7261 6e73 6c61 7465 2e67 6f6f  om.translate.goo
-00002d90: 672f 732f 694f 4951 4633 636b 6a30 2d72  g/s/iOIQF3ckj0-r
-00002da0: 4547 3479 4a67 6572 5977 3f66 6263 6c69  EG4yJgerYw?fbcli
-00002db0: 643d 4977 4152 3061 6c77 6957 6265 3375  d=IwAR0alwiWbe3u
-00002dc0: 6449 6346 7671 7177 6d37 7935 7167 7239  dIcFvqqwm7y5qgr9
-00002dd0: 685a 706a 7238 3731 465a 4961 2d45 7247  hZpjr871FZIa-ErG
-00002de0: 5575 6b5a 3779 4a33 5a68 6743 6576 7326  UukZ7yJ3ZhgCevs&
-00002df0: 5f78 5f74 725f 736c 3d61 7574 6f26 5f78  _x_tr_sl=auto&_x
-00002e00: 5f74 725f 746c 3d65 6e26 5f78 5f74 725f  _tr_tl=en&_x_tr_
-00002e10: 686c 3d65 6e26 5f78 5f74 725f 7074 6f3d  hl=en&_x_tr_pto=
-00002e20: 7761 7070 2929 2028 5b57 6562 2064 656d  wapp)) ([Web dem
-00002e30: 6f5d 2868 7474 7073 3a2f 2f63 616d 6572  o](https://camer
-00002e40: 6174 7261 702d 6169 2e68 696e 6174 7572  atrap-ai.hinatur
-00002e50: 652e 636e 2f68 6f6d 6529 290a 2a20 5b49  e.cn/home)).* [I
-00002e60: 7276 696e 6520 5261 6e63 6820 436f 6e73  rvine Ranch Cons
-00002e70: 6572 7661 6e63 795d 2868 7474 703a 2f2f  ervancy](http://
-00002e80: 7777 772e 6972 636f 6e73 6572 7661 6e63  www.irconservanc
-00002e90: 792e 6f72 672f 2920 285b 7374 6f72 795d  y.org/) ([story]
-00002ea0: 2868 7474 7073 3a2f 2f77 7777 2e6f 6372  (https://www.ocr
-00002eb0: 6567 6973 7465 722e 636f 6d2f 3230 3232  egister.com/2022
-00002ec0: 2f30 332f 3330 2f61 692d 736f 6674 7761  /03/30/ai-softwa
-00002ed0: 7265 2d69 732d 6865 6c70 696e 672d 7265  re-is-helping-re
-00002ee0: 7365 6172 6368 6572 732d 666f 6375 732d  searchers-focus-
-00002ef0: 6f6e 2d6c 6561 726e 696e 672d 6162 6f75  on-learning-abou
-00002f00: 742d 6f63 732d 7769 6c64 2d61 6e69 6d61  t-ocs-wild-anima
-00002f10: 6c73 2f29 290a 2a20 5b57 696c 646c 6966  ls/)).* [Wildlif
-00002f20: 6520 5072 6f74 6563 7469 6f6e 2053 6f6c  e Protection Sol
-00002f30: 7574 696f 6e73 5d28 6874 7470 733a 2f2f  utions](https://
-00002f40: 7769 6c64 6c69 6665 7072 6f74 6563 7469  wildlifeprotecti
-00002f50: 6f6e 736f 6c75 7469 6f6e 732e 6f72 672f  onsolutions.org/
-00002f60: 2920 285b 7374 6f72 795d 2868 7474 7073  ) ([story](https
-00002f70: 3a2f 2f63 7573 746f 6d65 7273 2e6d 6963  ://customers.mic
-00002f80: 726f 736f 6674 2e63 6f6d 2f65 6e2d 7573  rosoft.com/en-us
-00002f90: 2f73 746f 7279 2f31 3338 3431 3834 3531  /story/138418451
-00002fa0: 3739 3239 3334 3330 3833 2d77 696c 646c  7929343083-wildl
-00002fb0: 6966 652d 7072 6f74 6563 7469 6f6e 2d73  ife-protection-s
-00002fc0: 6f6c 7574 696f 6e73 2d6e 6f6e 7072 6f66  olutions-nonprof
-00002fd0: 6974 2d61 692d 666f 722d 6561 7274 6829  it-ai-for-earth)
-00002fe0: 2c20 5b73 746f 7279 5d28 6874 7470 733a  , [story](https:
-00002ff0: 2f2f 7777 772e 656e 7465 7270 7269 7365  //www.enterprise
-00003000: 6169 2e6e 6577 732f 3230 3233 2f30 322f  ai.news/2023/02/
-00003010: 3230 2f61 692d 6865 6c70 732d 7769 6c64  20/ai-helps-wild
-00003020: 6c69 6665 2d70 726f 7465 6374 696f 6e2d  life-protection-
-00003030: 736f 6c75 7469 6f6e 732d 7361 6665 6775  solutions-safegu
-00003040: 6172 642d 656e 6461 6e67 6572 6564 2d73  ard-endangered-s
-00003050: 7065 6369 6573 2f29 290a 2a20 5b51 3432  pecies/)).* [Q42
-00003060: 5d28 6874 7470 733a 2f2f 7777 772e 7134  ](https://www.q4
-00003070: 322e 6e6c 2f65 6e29 2028 5b62 6c6f 6720  2.nl/en) ([blog 
-00003080: 706f 7374 5d28 6874 7470 733a 2f2f 656e  post](https://en
-00003090: 6769 6e65 6572 696e 672e 7134 322e 6e6c  gineering.q42.nl
-000030a0: 2f61 692d 6265 6172 2d72 6570 656c 6c65  /ai-bear-repelle
-000030b0: 722f 2929 0a2a 205b 4167 6f75 7469 5d28  r/)).* [Agouti](
-000030c0: 6874 7470 733a 2f2f 6167 6f75 7469 2e65  https://agouti.e
-000030d0: 752f 2920 285b 7265 706f 7274 5d28 6874  u/) ([report](ht
-000030e0: 7470 733a 2f2f 6566 7361 2e6f 6e6c 696e  tps://efsa.onlin
-000030f0: 656c 6962 7261 7279 2e77 696c 6579 2e63  elibrary.wiley.c
-00003100: 6f6d 2f64 6f69 2f70 6466 2f31 302e 3239  om/doi/pdf/10.29
-00003110: 3033 2f73 702e 6566 7361 2e32 3032 332e  03/sp.efsa.2023.
-00003120: 454e 2d38 3231 3729 290a 2a20 5b54 7261  EN-8217)).* [Tra
-00003130: 7070 6572 5d28 6874 7470 733a 2f2f 7472  pper](https://tr
-00003140: 6170 7065 722d 7072 6f6a 6563 742e 7265  apper-project.re
-00003150: 6164 7468 6564 6f63 732e 696f 2f65 6e2f  adthedocs.io/en/
-00003160: 6c61 7465 7374 2f6f 7665 7276 6965 772e  latest/overview.
-00003170: 6874 6d6c 2920 285b 7475 746f 7269 616c  html) ([tutorial
-00003180: 5d28 6874 7470 733a 2f2f 7472 6170 7065  ](https://trappe
-00003190: 722d 7072 6f6a 6563 742e 7265 6164 7468  r-project.readth
-000031a0: 6564 6f63 732e 696f 2f65 6e2f 6c61 7465  edocs.io/en/late
-000031b0: 7374 2f74 7574 6f72 6961 6c2e 6874 6d6c  st/tutorial.html
-000031c0: 2929 0a0a 2a20 5b52 6f61 6420 4563 6f6c  ))..* [Road Ecol
-000031d0: 6f67 7920 4365 6e74 6572 5d28 6874 7470  ogy Center](http
-000031e0: 733a 2f2f 726f 6164 6563 6f6c 6f67 792e  s://roadecology.
-000031f0: 7563 6461 7669 732e 6564 752f 292c 2055  ucdavis.edu/), U
-00003200: 6e69 7665 7273 6974 7920 6f66 2043 616c  niversity of Cal
-00003210: 6966 6f72 6e69 612c 2044 6176 6973 2028  ifornia, Davis (
-00003220: 5b57 696c 646c 6966 6520 4f62 7365 7276  [Wildlife Observ
-00003230: 6572 204e 6574 776f 726b 2070 6c61 7466  er Network platf
-00003240: 6f72 6d5d 2868 7474 7073 3a2f 2f77 696c  orm](https://wil
-00003250: 646c 6966 656f 6273 6572 7665 722e 6e65  dlifeobserver.ne
-00003260: 742f 2929 0a2a 205b 5468 6520 4e61 7475  t/)).* [The Natu
-00003270: 7265 2043 6f6e 7365 7276 616e 6379 2069  re Conservancy i
-00003280: 6e20 4361 6c69 666f 726e 6961 5d28 6874  n California](ht
-00003290: 7470 733a 2f2f 7777 772e 6e61 7475 7265  tps://www.nature
-000032a0: 2e6f 7267 2f65 6e2d 7573 2f61 626f 7574  .org/en-us/about
-000032b0: 2d75 732f 7768 6572 652d 7765 2d77 6f72  -us/where-we-wor
-000032c0: 6b2f 756e 6974 6564 2d73 7461 7465 732f  k/united-states/
-000032d0: 6361 6c69 666f 726e 6961 2f29 2028 5b41  california/) ([A
-000032e0: 6e69 6d6c 2070 6c61 7466 6f72 6d5d 2868  niml platform](h
-000032f0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00003300: 6d2f 746e 632d 6361 2d67 656f 2f61 6e69  m/tnc-ca-geo/ani
-00003310: 6d6c 2d66 726f 6e74 656e 6429 290a 2a20  ml-frontend)).* 
-00003320: 5b53 616e 2044 6965 676f 205a 6f6f 2057  [San Diego Zoo W
-00003330: 696c 646c 6966 6520 416c 6c69 616e 6365  ildlife Alliance
-00003340: 5d28 6874 7470 733a 2f2f 7363 6965 6e63  ](https://scienc
-00003350: 652e 7361 6e64 6965 676f 7a6f 6f2e 6f72  e.sandiegozoo.or
-00003360: 672f 2920 2028 5b41 6e69 6d6c 2052 2070  g/)  ([Animl R p
-00003370: 6163 6b61 6765 5d28 6874 7470 733a 2f2f  ackage](https://
-00003380: 6769 7468 7562 2e63 6f6d 2f63 6f6e 7365  github.com/conse
-00003390: 7276 6174 696f 6e74 6563 686c 6162 2f61  rvationtechlab/a
-000033a0: 6e69 6d6c 2929 0a0a 416c 736f 2073 6565  niml))..Also see
-000033b0: 3a0a 0a2a 2054 6865 205b 6c69 7374 206f  :..* The [list o
-000033c0: 6620 4d44 2d72 656c 6174 6564 2047 5549  f MD-related GUI
-000033d0: 732c 2070 6c61 7466 6f72 6d73 2c20 616e  s, platforms, an
-000033e0: 6420 4769 7448 7562 2072 6570 6f73 5d28  d GitHub repos](
-000033f0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00003400: 6f6d 2f61 6765 6e74 6d6f 7272 6973 2f4d  om/agentmorris/M
-00003410: 6567 6144 6574 6563 746f 722f 626c 6f62  egaDetector/blob
-00003420: 2f6d 6169 6e2f 6d65 6761 6465 7465 6374  /main/megadetect
-00003430: 6f72 2e6d 6423 6973 2d74 6865 7265 2d61  or.md#is-there-a
-00003440: 2d67 7569 2920 7769 7468 696e 2074 6865  -gui) within the
-00003450: 204d 6567 6144 6574 6563 746f 7220 5573   MegaDetector Us
-00003460: 6572 2047 7569 6465 0a0a 2a20 5b50 6574  er Guide..* [Pet
-00003470: 6572 2773 206d 6170 206f 6620 4563 6f41  er's map of EcoA
-00003480: 7373 6973 7420 7573 6572 735d 2868 7474  ssist users](htt
-00003490: 7073 3a2f 2f61 6464 6178 6461 7461 7363  ps://addaxdatasc
-000034a0: 6965 6e63 652e 636f 6d2f 6563 6f61 7373  ience.com/ecoass
-000034b0: 6973 7429 2028 7768 6f20 6172 6520 616c  ist) (who are al
-000034c0: 736f 204d 6567 6144 6574 6563 746f 7220  so MegaDetector 
-000034d0: 7573 6572 7321 290a 0a2a 2054 6865 206c  users!)..* The l
-000034e0: 6973 7420 6f66 2070 6170 6572 7320 7461  ist of papers ta
-000034f0: 6767 6564 2022 4d65 6761 4465 7465 6374  gged "MegaDetect
-00003500: 6f72 2220 6f6e 206f 7572 205b 6c69 7374  or" on our [list
-00003510: 206f 6620 7061 7065 7273 2061 626f 7574   of papers about
-00003520: 204d 4c20 616e 6420 6361 6d65 7261 2074   ML and camera t
-00003530: 7261 7073 5d28 6874 7470 733a 2f2f 6167  raps](https://ag
-00003540: 656e 746d 6f72 7269 732e 6769 7468 7562  entmorris.github
-00003550: 2e69 6f2f 6361 6d65 7261 2d74 7261 702d  .io/camera-trap-
-00003560: 6d6c 2d73 7572 7665 792f 2363 616d 6572  ml-survey/#camer
-00003570: 612d 7472 6170 2d6d 6c2d 7061 7065 7273  a-trap-ml-papers
-00003580: 290a 0a23 2320 5265 706f 2063 6f6e 7465  )..## Repo conte
-00003590: 6e74 730a 0a54 6869 7320 7265 706f 2069  nts..This repo i
-000035a0: 7320 6f72 6761 6e69 7a65 6420 696e 746f  s organized into
-000035b0: 2074 6865 2066 6f6c 6c6f 7769 6e67 2066   the following f
-000035c0: 6f6c 6465 7273 2e2e 2e0a 0a0a 2323 2320  olders......### 
-000035d0: 6170 690a 0a43 6f64 6520 666f 7220 686f  api..Code for ho
-000035e0: 7374 696e 6720 6f75 7220 6d6f 6465 6c73  sting our models
-000035f0: 2061 7320 616e 2041 5049 2c20 6569 7468   as an API, eith
-00003600: 6572 2066 6f72 2073 796e 6368 726f 6e6f  er for synchrono
-00003610: 7573 206f 7065 7261 7469 6f6e 2028 692e  us operation (i.
-00003620: 652e 2c20 666f 7220 7265 616c 2d74 696d  e., for real-tim
-00003630: 6520 696e 6665 7265 6e63 6529 206f 7220  e inference) or 
-00003640: 6173 2061 2062 6174 6368 2070 726f 6365  as a batch proce
-00003650: 7373 2028 666f 7220 6c61 7267 6520 6269  ss (for large bi
-00003660: 6f64 6976 6572 7369 7479 2073 7572 7665  odiversity surve
-00003670: 7973 292e 2020 436f 6d6d 6f6e 206f 7065  ys).  Common ope
-00003680: 7261 7469 6f6e 7320 6f6e 6520 6d69 6768  rations one migh
-00003690: 7420 646f 2061 6674 6572 2072 756e 6e69  t do after runni
-000036a0: 6e67 204d 6567 6144 6574 6563 746f 7220  ng MegaDetector 
-000036b0: 266e 6461 7368 3b20 652e 672e 205b 6765  &ndash; e.g. [ge
-000036c0: 6e65 7261 7469 6e67 2070 7265 7669 6577  nerating preview
-000036d0: 2070 6167 6573 2074 6f20 7375 6d6d 6172   pages to summar
-000036e0: 697a 6520 796f 7572 2072 6573 756c 7473  ize your results
-000036f0: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-00003700: 2e63 6f6d 2f61 6765 6e74 6d6f 7272 6973  .com/agentmorris
-00003710: 2f4d 6567 6144 6574 6563 746f 722f 626c  /MegaDetector/bl
-00003720: 6f62 2f6d 6169 6e2f 6170 692f 6261 7463  ob/main/api/batc
-00003730: 685f 7072 6f63 6573 7369 6e67 2f70 6f73  h_processing/pos
-00003740: 7470 726f 6365 7373 696e 672f 706f 7374  tprocessing/post
-00003750: 7072 6f63 6573 735f 6261 7463 685f 7265  process_batch_re
-00003760: 7375 6c74 732e 7079 292c 205b 7365 7061  sults.py), [sepa
-00003770: 7261 7469 6e67 2069 6d61 6765 7320 696e  rating images in
-00003780: 746f 2064 6966 6665 7265 6e74 2066 6f6c  to different fol
-00003790: 6465 7273 2062 6173 6564 206f 6e20 4149  ders based on AI
-000037a0: 2072 6573 756c 7473 5d28 6874 7470 733a   results](https:
-000037b0: 2f2f 6769 7468 7562 2e63 6f6d 2f61 6765  //github.com/age
-000037c0: 6e74 6d6f 7272 6973 2f4d 6567 6144 6574  ntmorris/MegaDet
-000037d0: 6563 746f 722f 626c 6f62 2f6d 6169 6e2f  ector/blob/main/
-000037e0: 6170 692f 6261 7463 685f 7072 6f63 6573  api/batch_proces
-000037f0: 7369 6e67 2f70 6f73 7470 726f 6365 7373  sing/postprocess
-00003800: 696e 672f 7365 7061 7261 7465 5f64 6574  ing/separate_det
-00003810: 6563 7469 6f6e 735f 696e 746f 5f66 6f6c  ections_into_fol
-00003820: 6465 7273 2e70 7929 2c20 6f72 205b 636f  ders.py), or [co
-00003830: 6e76 6572 7469 6e67 2072 6573 756c 7473  nverting results
-00003840: 2074 6f20 6120 6469 6666 6572 656e 7420   to a different 
-00003850: 666f 726d 6174 5d28 6874 7470 733a 2f2f  format](https://
-00003860: 6769 7468 7562 2e63 6f6d 2f61 6765 6e74  github.com/agent
-00003870: 6d6f 7272 6973 2f4d 6567 6144 6574 6563  morris/MegaDetec
-00003880: 746f 722f 626c 6f62 2f6d 6169 6e2f 6170  tor/blob/main/ap
-00003890: 692f 6261 7463 685f 7072 6f63 6573 7369  i/batch_processi
-000038a0: 6e67 2f70 6f73 7470 726f 6365 7373 696e  ng/postprocessin
-000038b0: 672f 636f 6e76 6572 745f 6f75 7470 7574  g/convert_output
-000038c0: 5f66 6f72 6d61 742e 7079 2920 266e 6461  _format.py) &nda
-000038d0: 7368 3b20 616c 736f 206c 6976 6520 696e  sh; also live in
-000038e0: 2074 6869 7320 666f 6c64 6572 2c20 7769   this folder, wi
-000038f0: 7468 696e 2074 6865 205b 6170 692f 6261  thin the [api/ba
-00003900: 7463 685f 7072 6f63 6573 7369 6e67 2f70  tch_processing/p
-00003910: 6f73 7470 726f 6365 7373 696e 675d 2868  ostprocessing](h
-00003920: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00003930: 6d2f 6167 656e 746d 6f72 7269 732f 4d65  m/agentmorris/Me
-00003940: 6761 4465 7465 6374 6f72 2f74 7265 652f  gaDetector/tree/
-00003950: 6d61 696e 2f61 7069 2f62 6174 6368 5f70  main/api/batch_p
-00003960: 726f 6365 7373 696e 672f 706f 7374 7072  rocessing/postpr
-00003970: 6f63 6573 7369 6e67 2920 666f 6c64 6572  ocessing) folder
-00003980: 2e0a 0a0a 2323 2320 6172 6368 6976 650a  ....### archive.
-00003990: 0a4f 6c64 2063 6f64 6520 7468 6174 2077  .Old code that w
-000039a0: 6520 6469 646e 2774 203c 693e 7175 6974  e didn't <i>quit
-000039b0: 653c 2f69 3e20 7761 6e74 2074 6f20 6465  e</i> want to de
-000039c0: 6c65 7465 2c20 6275 7420 6973 2062 6173  lete, but is bas
-000039d0: 6963 616c 6c79 206f 6273 6f6c 6574 652e  ically obsolete.
-000039e0: 0a0a 0a23 2323 2063 6c61 7373 6966 6963  ...### classific
-000039f0: 6174 696f 6e0a 0a45 7870 6572 696d 656e  ation..Experimen
-00003a00: 7461 6c20 636f 6465 2066 6f72 2074 7261  tal code for tra
-00003a10: 696e 696e 6720 7370 6563 6965 7320 636c  ining species cl
-00003a20: 6173 7369 6669 6572 7320 6f6e 206e 6577  assifiers on new
-00003a30: 2064 6174 6120 7365 7473 2c20 6765 6e65   data sets, gene
-00003a40: 7261 6c6c 7920 7472 6169 6e65 6420 6f6e  rally trained on
-00003a50: 204d 6567 6144 6574 6563 746f 7220 6372   MegaDetector cr
-00003a60: 6f70 732e 2020 4375 7272 656e 746c 7920  ops.  Currently 
-00003a70: 7468 6520 6d61 696e 2070 6970 656c 696e  the main pipelin
-00003a80: 6520 6465 7363 7269 6265 6420 696e 2074  e described in t
-00003a90: 6869 7320 666f 6c64 6572 2072 656c 6965  his folder relie
-00003aa0: 7320 6f6e 2061 206c 6172 6765 2064 6174  s on a large dat
-00003ab0: 6162 6173 6520 6f66 206c 6162 656c 6564  abase of labeled
-00003ac0: 2069 6d61 6765 7320 7468 6174 2069 7320   images that is 
-00003ad0: 6e6f 7420 7075 626c 6963 6c79 2061 7661  not publicly ava
-00003ae0: 696c 6162 6c65 3b20 7468 6572 6566 6f72  ilable; therefor
-00003af0: 652c 2074 6869 7320 666f 6c64 6572 2069  e, this folder i
-00003b00: 7320 6e6f 7420 7965 7420 7365 7420 7570  s not yet set up
-00003b10: 2074 6f20 6661 6369 6c69 7461 7465 2074   to facilitate t
-00003b20: 7261 696e 696e 6720 6f66 2079 6f75 7220  raining of your 
-00003b30: 6f77 6e20 636c 6173 7369 6669 6572 732e  own classifiers.
-00003b40: 2020 486f 7765 7665 722c 2069 7420 6973    However, it is
-00003b50: 2075 7365 6675 6c20 666f 7220 3c69 3e75   useful for <i>u
-00003b60: 7365 7273 3c2f 693e 206f 6620 7468 6520  sers</i> of the 
-00003b70: 636c 6173 7369 6669 6572 7320 7468 6174  classifiers that
-00003b80: 2077 6520 7472 6169 6e2c 2061 6e64 2063   we train, and c
-00003b90: 6f6e 7461 696e 7320 736f 6d65 2075 7365  ontains some use
-00003ba0: 6675 6c20 7374 6172 7469 6e67 2070 6f69  ful starting poi
-00003bb0: 6e74 7320 6966 2079 6f75 2061 7265 2067  nts if you are g
-00003bc0: 6f69 6e67 2074 6f20 7461 6b65 2061 2022  oing to take a "
-00003bd0: 4449 5922 2061 7070 726f 6163 6820 746f  DIY" approach to
-00003be0: 2074 7261 696e 696e 6720 636c 6173 7369   training classi
-00003bf0: 6669 6572 7320 6f6e 2063 726f 7070 6564  fiers on cropped
-00003c00: 2069 6d61 6765 732e 2020 0a0a 416c 6c20   images.  ..All 
-00003c10: 7468 6174 2073 6169 642c 2068 6572 6527  that said, here'
-00003c20: 7320 616e 6f74 6865 7220 2274 6561 7365  s another "tease
-00003c30: 7220 696d 6167 6522 206f 6620 7768 6174  r image" of what
-00003c40: 2079 6f75 2067 6574 2061 7420 7468 6520   you get at the 
-00003c50: 656e 6420 6f66 2074 7261 696e 696e 6720  end of training 
-00003c60: 616e 6420 7275 6e6e 696e 6720 6120 636c  and running a cl
-00003c70: 6173 7369 6669 6572 3a0a 0a3c 696d 6720  assifier:..<img 
-00003c80: 7372 633d 2269 6d61 6765 732f 7761 7274  src="images/wart
-00003c90: 686f 675f 636c 6173 7369 6669 6361 7469  hog_classificati
-00003ca0: 6f6e 732e 6a70 6722 2077 6964 7468 3d22  ons.jpg" width="
-00003cb0: 3730 3022 3e3c 6272 2f3e 496d 6167 6520  700"><br/>Image 
-00003cc0: 6372 6564 6974 2055 6e69 7665 7273 6974  credit Universit
-00003cd0: 7920 6f66 204d 696e 6e65 736f 7461 2c20  y of Minnesota, 
-00003ce0: 6672 6f6d 2074 6865 2053 6e61 7073 686f  from the Snapsho
-00003cf0: 7420 5361 6661 7269 2070 726f 6772 616d  t Safari program
-00003d00: 2e0a 0a0a 2323 2320 6461 7461 5f6d 616e  ....### data_man
-00003d10: 6167 656d 656e 740a 0a43 6f64 6520 666f  agement..Code fo
-00003d20: 723a 0a0a 2a20 436f 6e76 6572 7469 6e67  r:..* Converting
-00003d30: 2066 7265 7175 656e 746c 792d 7573 6564   frequently-used
-00003d40: 206d 6574 6164 6174 6120 666f 726d 6174   metadata format
-00003d50: 7320 746f 205b 434f 434f 2043 616d 6572  s to [COCO Camer
-00003d60: 6120 5472 6170 735d 2868 7474 7073 3a2f  a Traps](https:/
-00003d70: 2f67 6974 6875 622e 636f 6d2f 6167 656e  /github.com/agen
-00003d80: 746d 6f72 7269 732f 4d65 6761 4465 7465  tmorris/MegaDete
-00003d90: 6374 6f72 2f62 6c6f 622f 6d61 696e 2f64  ctor/blob/main/d
-00003da0: 6174 615f 6d61 6e61 6765 6d65 6e74 2f52  ata_management/R
-00003db0: 4541 444d 452e 6d64 2363 6f63 6f2d 6361  EADME.md#coco-ca
-00003dc0: 6d65 7261 7472 6170 732d 666f 726d 6174  meratraps-format
-00003dd0: 2920 666f 726d 6174 0a2a 2043 6f6e 7665  ) format.* Conve
-00003de0: 7274 696e 6720 7468 6520 6f75 7470 7574  rting the output
-00003df0: 206f 6620 4149 206d 6f64 656c 7320 2865   of AI models (e
-00003e00: 7370 6563 6961 6c6c 7920 5b59 4f4c 4f76  specially [YOLOv
-00003e10: 355d 2868 7474 7073 3a2f 2f67 6974 6875  5](https://githu
-00003e20: 622e 636f 6d2f 6167 656e 746d 6f72 7269  b.com/agentmorri
-00003e30: 732f 4d65 6761 4465 7465 6374 6f72 2f62  s/MegaDetector/b
-00003e40: 6c6f 622f 6d61 696e 2f61 7069 2f62 6174  lob/main/api/bat
-00003e50: 6368 5f70 726f 6365 7373 696e 672f 706f  ch_processing/po
-00003e60: 7374 7072 6f63 6573 7369 6e67 2f63 6f6e  stprocessing/con
-00003e70: 7665 7274 5f6f 7574 7075 745f 666f 726d  vert_output_form
-00003e80: 6174 2e70 7929 2920 746f 2074 6865 2066  at.py)) to the f
-00003e90: 6f72 6d61 7420 7573 6564 2066 6f72 2041  ormat used for A
-00003ea0: 4920 7265 7375 6c74 7320 7468 726f 7567  I results throug
-00003eb0: 686f 7574 2074 6869 7320 7265 706f 0a2a  hout this repo.*
-00003ec0: 2043 7265 6174 696e 672c 2076 6973 7561   Creating, visua
-00003ed0: 6c69 7a69 6e67 2c20 616e 6420 2065 6469  lizing, and  edi
-00003ee0: 7469 6e67 2043 4f43 4f20 4361 6d65 7261  ting COCO Camera
-00003ef0: 2054 7261 7073 202e 6a73 6f6e 2064 6174   Traps .json dat
-00003f00: 6162 6173 6573 0a0a 0a23 2323 2064 6574  abases...### det
-00003f10: 6563 7469 6f6e 0a0a 436f 6465 2066 6f72  ection..Code for
-00003f20: 2074 7261 696e 696e 672c 2072 756e 6e69   training, runni
-00003f30: 6e67 2c20 616e 6420 6576 616c 7561 7469  ng, and evaluati
-00003f40: 6e67 204d 6567 6144 6574 6563 746f 722e  ng MegaDetector.
-00003f50: 0a0a 0a23 2323 2065 6e76 730a 0a45 6e76  ...### envs..Env
-00003f60: 6972 6f6e 6d65 6e74 2066 696c 6573 2e2e  ironment files..
-00003f70: 2e20 7370 6563 6966 6963 616c 6c79 202e  . specifically .
-00003f80: 796d 6c20 6669 6c65 7320 666f 7220 6d61  yml files for ma
-00003f90: 6d62 612f 636f 6e64 6120 656e 7669 726f  mba/conda enviro
-00003fa0: 6e6d 656e 7473 2028 7468 6573 6520 6172  nments (these ar
-00003fb0: 6520 7768 6174 2077 6520 7265 636f 6d6d  e what we recomm
-00003fc0: 656e 6420 696e 206f 7572 205b 4d65 6761  end in our [Mega
-00003fd0: 4465 7465 6374 6f72 2055 7365 7220 4775  Detector User Gu
-00003fe0: 6964 655d 286d 6567 6164 6574 6563 746f  ide](megadetecto
-00003ff0: 722e 6d64 2929 2c20 616e 6420 6120 7265  r.md)), and a re
-00004000: 7175 6972 656d 656e 7473 2e74 7874 2066  quirements.txt f
-00004010: 6f72 2074 6865 2070 6970 2d69 6e63 6c69  or the pip-incli
-00004020: 6e65 642e 0a0a 0a23 2323 2069 6d61 6765  ned....### image
-00004030: 730a 0a4d 6564 6961 2075 7365 6420 696e  s..Media used in
-00004040: 2064 6f63 756d 656e 7461 7469 6f6e 2e0a   documentation..
-00004050: 0a0a 2323 2320 6d64 5f75 7469 6c73 0a0a  ..### md_utils..
-00004060: 536d 616c 6c20 7574 696c 6974 7920 6675  Small utility fu
-00004070: 6e63 7469 6f6e 7320 666f 7220 7374 7269  nctions for stri
-00004080: 6e67 206d 616e 6970 756c 6174 696f 6e2c  ng manipulation,
-00004090: 2066 696c 656e 616d 6520 6d61 6e69 7075   filename manipu
-000040a0: 6c61 7469 6f6e 2c20 646f 776e 6c6f 6164  lation, download
-000040b0: 696e 6720 6669 6c65 7320 6672 6f6d 2055  ing files from U
-000040c0: 524c 732c 2065 7463 2e20 204d 6f73 746c  RLs, etc.  Mostl
-000040d0: 7920 6164 6170 7465 6420 6672 6f6d 2074  y adapted from t
-000040e0: 6865 205b 6169 3465 7574 696c 735d 2868  he [ai4eutils](h
-000040f0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00004100: 6d2f 6d69 6372 6f73 6f66 742f 6169 3465  m/microsoft/ai4e
-00004110: 7574 696c 7329 2072 6570 6f2e 0a0a 0a23  utils) repo....#
-00004120: 2323 206d 645f 7669 7375 616c 697a 6174  ## md_visualizat
-00004130: 696f 6e0a 0a53 6861 7265 6420 746f 6f6c  ion..Shared tool
-00004140: 7320 666f 7220 7669 7375 616c 697a 696e  s for visualizin
-00004150: 6720 696d 6167 6573 2077 6974 6820 6772  g images with gr
-00004160: 6f75 6e64 2074 7275 7468 2061 6e64 2f6f  ound truth and/o
-00004170: 7220 7072 6564 6963 7465 6420 616e 6e6f  r predicted anno
-00004180: 7461 7469 6f6e 732e 0a0a 0a23 2323 2073  tations....### s
-00004190: 616e 6462 6f78 0a0a 5261 6e64 6f6d 2074  andbox..Random t
-000041a0: 6869 6e67 7320 7468 6174 2064 6f6e 2774  hings that don't
-000041b0: 2066 6974 2069 6e20 616e 7920 6f74 6865   fit in any othe
-000041c0: 7220 6469 7265 6374 6f72 792c 2062 7574  r directory, but
-000041d0: 2061 7265 6e27 7420 7175 6974 6520 6465   aren't quite de
-000041e0: 7072 6563 6174 6564 2e20 204d 6f73 746c  precated.  Mostl
-000041f0: 7920 706f 7374 7072 6f63 6573 7369 6e67  y postprocessing
-00004200: 2073 6372 6970 7473 2074 6861 7420 7765   scripts that we
-00004210: 7265 2062 7569 6c74 2066 6f72 2061 2073  re built for a s
-00004220: 696e 676c 6520 7573 6520 6361 7365 2062  ingle use case b
-00004230: 7574 2063 6f75 6c64 2070 6f74 656e 7469  ut could potenti
-00004240: 616c 6c79 2062 6520 7573 6566 756c 2069  ally be useful i
-00004250: 6e20 7468 6520 6675 7475 7265 2e0a 0a0a  n the future....
-00004260: 2323 2320 7461 786f 6e6f 6d79 5f6d 6170  ### taxonomy_map
-00004270: 7069 6e67 0a0a 436f 6465 2074 6f20 6661  ping..Code to fa
-00004280: 6369 6c69 7461 7465 206d 6170 7069 6e67  cilitate mapping
-00004290: 2064 6174 612d 7365 742d 7370 6563 6966   data-set-specif
-000042a0: 6963 2063 6174 6567 6f72 7920 6e61 6d65  ic category name
-000042b0: 7320 2865 2e67 2e20 226c 696f 6e22 2c20  s (e.g. "lion", 
-000042c0: 7768 6963 6820 6d65 616e 7320 7665 7279  which means very
-000042d0: 2064 6966 6665 7265 6e74 2074 6869 6e67   different thing
-000042e0: 7320 696e 2049 6461 686f 2076 732e 2053  s in Idaho vs. S
-000042f0: 6f75 7468 2041 6672 6963 6129 2074 6f20  outh Africa) to 
-00004300: 6120 7374 616e 6461 7264 2074 6178 6f6e  a standard taxon
-00004310: 6f6d 792e 0a0a 0a23 2323 2074 6573 745f  omy....### test_
-00004320: 696d 6167 6573 0a0a 4120 6861 6e64 6675  images..A handfu
-00004330: 6c20 6f66 2069 6d61 6765 7320 6672 6f6d  l of images from
-00004340: 205b 4c49 4c41 5d28 6874 7470 733a 2f2f   [LILA](https://
-00004350: 6c69 6c61 2e73 6369 656e 6365 2920 7468  lila.science) th
-00004360: 6174 2066 6163 696c 6974 6174 6520 7465  at facilitate te
-00004370: 7374 696e 6720 616e 6420 6465 6275 6767  sting and debugg
-00004380: 696e 672e 0a0a 0a23 2320 436f 6e74 6163  ing....## Contac
-00004390: 740a 0a46 6f72 2071 7565 7374 696f 6e73  t..For questions
-000043a0: 2061 626f 7574 2074 6869 7320 7265 706f   about this repo
-000043b0: 2c20 636f 6e74 6163 7420 5b63 616d 6572  , contact [camer
-000043c0: 6174 7261 7073 406c 696c 612e 7363 6965  atraps@lila.scie
-000043d0: 6e63 655d 286d 6169 6c74 6f3a 6361 6d65  nce](mailto:came
-000043e0: 7261 7472 6170 7340 6c69 6c61 2e73 6369  ratraps@lila.sci
-000043f0: 656e 6365 292e 0a0a 596f 7520 6361 6e20  ence)...You can 
-00004400: 616c 736f 2063 6861 7420 7769 7468 2075  also chat with u
-00004410: 7320 616e 6420 7468 6520 6272 6f61 6465  s and the broade
-00004420: 7220 6361 6d65 7261 2074 7261 7020 4149  r camera trap AI
-00004430: 2063 6f6d 6d75 6e69 7479 206f 6e20 7468   community on th
-00004440: 6520 5b41 4920 666f 7220 436f 6e73 6572  e [AI for Conser
-00004450: 7661 7469 6f6e 2066 6f72 756d 2061 7420  vation forum at 
-00004460: 5749 4c44 4c41 4253 5d28 6874 7470 733a  WILDLABS](https:
-00004470: 2f2f 7769 6c64 6c61 6273 2e6e 6574 2f67  //wildlabs.net/g
-00004480: 726f 7570 732f 6169 2d63 6f6e 7365 7276  roups/ai-conserv
-00004490: 6174 696f 6e29 206f 7220 7468 6520 5b41  ation) or the [A
-000044a0: 4920 666f 7220 436f 6e73 6572 7661 7469  I for Conservati
-000044b0: 6f6e 2053 6c61 636b 2067 726f 7570 5d28  on Slack group](
-000044c0: 6874 7470 733a 2f2f 6169 666f 7263 6f6e  https://aiforcon
-000044d0: 7365 7276 6174 696f 6e2e 736c 6163 6b2e  servation.slack.
-000044e0: 636f 6d29 2e0a 0a0a 2323 2047 7261 7475  com)....## Gratu
-000044f0: 6974 6f75 7320 6361 6d65 7261 2074 7261  itous camera tra
-00004500: 7020 7069 6374 7572 650a 0a21 5b42 6972  p picture..![Bir
-00004510: 6420 666c 7969 6e67 2061 626f 7665 2077  d flying above w
-00004520: 6174 6572 5d28 696d 6167 6573 2f6e 6163  ater](images/nac
-00004530: 7469 2e6a 7067 293c 6272 2f3e 496d 6167  ti.jpg)<br/>Imag
-00004540: 6520 6372 6564 6974 2055 5344 412c 2066  e credit USDA, f
-00004550: 726f 6d20 7468 6520 5b4e 4143 5449 5d28  rom the [NACTI](
-00004560: 6874 7470 3a2f 2f6c 696c 612e 7363 6965  http://lila.scie
-00004570: 6e63 652f 6461 7461 7365 7473 2f6e 6163  nce/datasets/nac
-00004580: 7469 2920 6461 7461 2073 6574 2e0a 0a59  ti) data set...Y
-00004590: 6f75 2077 696c 6c20 6669 6e64 206c 6f74  ou will find lot
-000045a0: 7320 6d6f 7265 2067 7261 7475 6974 6f75  s more gratuitou
-000045b0: 7320 6361 6d65 7261 2074 7261 7020 7069  s camera trap pi
-000045c0: 6374 7572 6573 2073 7072 696e 6b6c 6564  ctures sprinkled
-000045d0: 2061 626f 7574 2074 6869 7320 7265 706f   about this repo
-000045e0: 2e20 2049 7427 7320 6c69 6b65 2061 2073  .  It's like a s
-000045f0: 6361 7665 6e67 6572 2068 756e 742e 0a0a  cavenger hunt...
-00004600: 0a23 2320 4c69 6365 6e73 650a 0a54 6869  .## License..Thi
-00004610: 7320 7265 706f 7369 746f 7279 2069 7320  s repository is 
-00004620: 6c69 6365 6e73 6564 2077 6974 6820 7468  licensed with th
-00004630: 6520 5b4d 4954 206c 6963 656e 7365 5d28  e [MIT license](
-00004640: 6874 7470 733a 2f2f 6f70 656e 736f 7572  https://opensour
-00004650: 6365 2e6f 7267 2f6c 6963 656e 7365 2f6d  ce.org/license/m
-00004660: 6974 2f29 2e0a 0a43 6f64 6520 7772 6974  it/)...Code writ
-00004670: 7465 6e20 6f6e 206f 7220 6265 666f 7265  ten on or before
-00004680: 2041 7072 696c 2032 382c 2032 3032 3320   April 28, 2023 
-00004690: 6973 205b 636f 7079 7269 6768 7420 4d69  is [copyright Mi
-000046a0: 6372 6f73 6f66 745d 2868 7474 7073 3a2f  crosoft](https:/
-000046b0: 2f67 6974 6875 622e 636f 6d2f 4d69 6372  /github.com/Micr
-000046c0: 6f73 6f66 742f 646f 746e 6574 2f62 6c6f  osoft/dotnet/blo
-000046d0: 622f 6d61 696e 2f4c 4943 454e 5345 292e  b/main/LICENSE).
-000046e0: 0a0a 0a23 2320 436f 6e74 7269 6275 7469  ...## Contributi
-000046f0: 6e67 0a0a 5468 6973 2070 726f 6a65 6374  ng..This project
-00004700: 2077 656c 636f 6d65 7320 636f 6e74 7269   welcomes contri
-00004710: 6275 7469 6f6e 732c 2061 7320 7075 6c6c  butions, as pull
-00004720: 2072 6571 7565 7374 732c 2069 7373 7565   requests, issue
-00004730: 732c 206f 7220 7375 6767 6573 7469 6f6e  s, or suggestion
-00004740: 7320 6279 205b 656d 6169 6c5d 286d 6169  s by [email](mai
-00004750: 6c74 6f3a 6361 6d65 7261 7472 6170 7340  lto:cameratraps@
-00004760: 6c69 6c61 2e73 6369 656e 6365 292e 2020  lila.science).  
-00004770: 5765 2068 6176 6520 6120 5b6c 6973 745d  We have a [list]
-00004780: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-00004790: 636f 6d2f 6167 656e 746d 6f72 7269 732f  com/agentmorris/
-000047a0: 4d65 6761 4465 7465 6374 6f72 2f69 7373  MegaDetector/iss
-000047b0: 7565 732f 3834 2920 6f66 2069 7373 7565  ues/84) of issue
-000047c0: 7320 7468 6174 2077 6527 7265 2068 6f70  s that we're hop
-000047d0: 696e 6720 746f 2061 6464 7265 7373 2c20  ing to address, 
-000047e0: 6d61 6e79 206f 6620 7768 6963 6820 776f  many of which wo
-000047f0: 756c 6420 6265 2067 6f6f 6420 7374 6172  uld be good star
-00004800: 7469 6e67 2070 6f69 6e74 7320 666f 7220  ting points for 
-00004810: 6e65 7720 636f 6e74 7269 6275 746f 7273  new contributors
-00004820: 2e20 2057 6520 616c 736f 2064 6570 656e  .  We also depen
-00004830: 6420 6f6e 206f 7468 6572 206f 7065 6e2d  d on other open-
-00004840: 736f 7572 6365 2074 6f6f 6c73 2074 6861  source tools tha
-00004850: 7420 6865 6c70 2075 7365 7273 2072 756e  t help users run
-00004860: 204d 6567 6144 6574 6563 746f 7220 2865   MegaDetector (e
-00004870: 2e67 2e20 5b45 636f 4173 7369 7374 5d28  .g. [EcoAssist](
-00004880: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00004890: 6f6d 2f50 6574 6572 7661 6e4c 756e 7465  om/PetervanLunte
-000048a0: 7265 6e2f 4563 6f41 7373 6973 7429 2061  ren/EcoAssist) a
-000048b0: 6e64 205b 4361 6d54 7261 7020 4465 7465  nd [CamTrap Dete
-000048c0: 6374 6f72 5d28 6874 7470 733a 2f2f 6769  ctor](https://gi
-000048d0: 7468 7562 2e63 6f6d 2f62 656e 6365 7661  thub.com/benceva
-000048e0: 6e73 2f63 616d 7472 6170 2d64 6574 6563  ns/camtrap-detec
-000048f0: 746f 7229 2920 616e 6420 776f 726b 2077  tor)) and work w
-00004900: 6974 6820 4d65 6761 4465 7465 6374 6f72  ith MegaDetector
-00004910: 2072 6573 756c 7473 2028 652e 672e 205b   results (e.g. [
-00004920: 5469 6d65 6c61 7073 655d 2868 7474 7073  Timelapse](https
-00004930: 3a2f 2f67 6974 6875 622e 636f 6d2f 7361  ://github.com/sa
-00004940: 756c 6772 6565 6e62 6572 672f 5469 6d65  ulgreenberg/Time
-00004950: 6c61 7073 6529 293b 2069 6620 796f 7520  lapse)); if you 
-00004960: 6172 6520 6c6f 6f6b 696e 6720 746f 2067  are looking to g
-00004970: 6574 2069 6e76 6f6c 7665 6420 696e 2047  et involved in G
-00004980: 5549 2064 6576 656c 6f70 6d65 6e74 2c20  UI development, 
-00004990: 7265 6163 6820 6f75 7420 746f 2074 6865  reach out to the
-000049a0: 2064 6576 656c 6f70 6572 7320 6f66 2074   developers of t
-000049b0: 686f 7365 2074 6f6f 6c73 2061 7320 7765  hose tools as we
-000049c0: 6c6c 210a 0a49 6620 796f 7520 6172 6520  ll!..If you are 
-000049d0: 696e 7465 7265 7374 696e 6720 696e 2067  interesting in g
-000049e0: 6574 7469 6e67 2069 6e76 6f6c 7665 6420  etting involved 
-000049f0: 696e 2074 6865 2063 6f6e 7365 7276 6174  in the conservat
-00004a00: 696f 6e20 7465 6368 6e6f 6c6f 6779 2073  ion technology s
-00004a10: 7061 6365 2c20 616e 6420 4d65 6761 4465  pace, and MegaDe
-00004a20: 7465 6374 6f72 206a 7573 7420 6861 7070  tector just happ
-00004a30: 656e 7320 746f 2062 6520 7468 6520 6669  ens to be the fi
-00004a40: 7273 7420 7061 6765 2079 6f75 206c 616e  rst page you lan
-00004a50: 6465 6420 6f6e 2c20 616e 6420 6e6f 6e65  ded on, and none
-00004a60: 206f 6620 6f75 7220 6f70 656e 2069 7373   of our open iss
-00004a70: 7565 7320 6172 6520 6765 7474 696e 6720  ues are getting 
-00004a80: 796f 7520 6669 7265 6420 7570 2c20 646f  you fired up, do
-00004a90: 6e27 7420 6672 6574 2120 2048 6561 6420  n't fret!  Head 
-00004aa0: 6f76 6572 2074 6f20 7468 6520 5b57 494c  over to the [WIL
-00004ab0: 444c 4142 5320 6469 7363 7573 7369 6f6e  DLABS discussion
-00004ac0: 2066 6f72 756d 735d 2868 7474 7073 3a2f   forums](https:/
-00004ad0: 2f77 696c 646c 6162 732e 6e65 742f 6469  /wildlabs.net/di
-00004ae0: 7363 7573 7369 6f6e 7329 2061 6e64 206c  scussions) and l
-00004af0: 6574 2074 6865 2063 6f6d 6d75 6e69 7479  et the community
-00004b00: 206b 6e6f 7720 796f 7527 7265 2061 2064   know you're a d
-00004b10: 6576 656c 6f70 6572 206c 6f6f 6b69 6e67  eveloper looking
-00004b20: 2074 6f20 6765 7420 696e 766f 6c76 6564   to get involved
-00004b30: 2e20 2053 6f6d 656f 6e65 206e 6565 6473  .  Someone needs
-00004b40: 2079 6f75 7220 6865 6c70 210a             your help!.
+00000080: 7465 6e74 730a 0a31 2e20 5b57 6861 7427  tents..1. [What'
+00000090: 7320 4d65 6761 4465 7465 6374 6f72 2061  s MegaDetector a
+000000a0: 6c6c 2061 626f 7574 3f5d 2823 7768 6174  ll about?](#what
+000000b0: 732d 6d65 6761 6465 7465 6374 6f72 2d61  s-megadetector-a
+000000c0: 6c6c 2d61 626f 7574 290a 332e 205b 486f  ll-about).3. [Ho
+000000d0: 7720 646f 2049 2067 6574 2073 7461 7274  w do I get start
+000000e0: 6564 2077 6974 6820 4d65 6761 4465 7465  ed with MegaDete
+000000f0: 6374 6f72 3f5d 2823 686f 772d 646f 2d69  ctor?](#how-do-i
+00000100: 2d67 6574 2d73 7461 7274 6564 2d77 6974  -get-started-wit
+00000110: 682d 6d65 6761 6465 7465 6374 6f72 290a  h-megadetector).
+00000120: 342e 205b 5768 6f20 6973 2075 7369 6e67  4. [Who is using
+00000130: 204d 6567 6144 6574 6563 746f 723f 5d28   MegaDetector?](
+00000140: 2377 686f 2d69 732d 7573 696e 672d 6d65  #who-is-using-me
+00000150: 6761 6465 7465 6374 6f72 290a 352e 205b  gadetector).5. [
+00000160: 5265 706f 2063 6f6e 7465 6e74 735d 2823  Repo contents](#
+00000170: 7265 706f 2d63 6f6e 7465 6e74 7329 0a36  repo-contents).6
+00000180: 2e20 5b43 6f6e 7461 6374 5d28 2363 6f6e  . [Contact](#con
+00000190: 7461 6374 290a 372e 205b 4772 6174 7569  tact).7. [Gratui
+000001a0: 746f 7573 2063 616d 6572 6120 7472 6170  tous camera trap
+000001b0: 2070 6963 7475 7265 5d28 2367 7261 7475   picture](#gratu
+000001c0: 6974 6f75 732d 6361 6d65 7261 2d74 7261  itous-camera-tra
+000001d0: 702d 7069 6374 7572 6529 0a0a 2323 2057  p-picture)..## W
+000001e0: 6861 7427 7320 4d65 6761 4465 7465 6374  hat's MegaDetect
+000001f0: 6f72 2061 6c6c 2061 626f 7574 3f0a 0a5b  or all about?..[
+00000200: 4d65 6761 4465 7465 6374 6f72 5d28 6d65  MegaDetector](me
+00000210: 6761 6465 7465 6374 6f72 2e6d 6429 2069  gadetector.md) i
+00000220: 7320 616e 2041 4920 6d6f 6465 6c20 7468  s an AI model th
+00000230: 6174 2069 6465 6e74 6966 6965 7320 616e  at identifies an
+00000240: 696d 616c 732c 2070 656f 706c 652c 2061  imals, people, a
+00000250: 6e64 2076 6568 6963 6c65 7320 696e 2063  nd vehicles in c
+00000260: 616d 6572 6120 7472 6170 2069 6d61 6765  amera trap image
+00000270: 7320 2877 6869 6368 2061 6c73 6f20 6d61  s (which also ma
+00000280: 6b65 7320 6974 2075 7365 6675 6c20 666f  kes it useful fo
+00000290: 7220 656c 696d 696e 6174 696e 6720 626c  r eliminating bl
+000002a0: 616e 6b20 696d 6167 6573 292e 2020 5468  ank images).  Th
+000002b0: 6973 206d 6f64 656c 2069 7320 7472 6169  is model is trai
+000002c0: 6e65 6420 6f6e 2073 6576 6572 616c 206d  ned on several m
+000002d0: 696c 6c69 6f6e 2069 6d61 6765 7320 6672  illion images fr
+000002e0: 6f6d 2061 2076 6172 6965 7479 206f 6620  om a variety of 
+000002f0: 6563 6f73 7973 7465 6d73 2e0a 0a48 6572  ecosystems...Her
+00000300: 6527 7320 6120 266c 6471 756f 3b74 6561  e's a &ldquo;tea
+00000310: 7365 7226 7264 7175 6f3b 2069 6d61 6765  ser&rdquo; image
+00000320: 206f 6620 7768 6174 204d 6567 6144 6574   of what MegaDet
+00000330: 6563 746f 7220 6f75 7470 7574 206c 6f6f  ector output loo
+00000340: 6b73 206c 696b 653a 0a0a 215b 5265 6420  ks like:..![Red 
+00000350: 626f 756e 6469 6e67 2062 6f78 206f 6e20  bounding box on 
+00000360: 666f 785d 2869 6d61 6765 732f 6465 7465  fox](images/dete
+00000370: 6374 6f72 5f65 7861 6d70 6c65 2e6a 7067  ctor_example.jpg
+00000380: 293c 6272 2f3e 496d 6167 6520 6372 6564  )<br/>Image cred
+00000390: 6974 2055 6e69 7665 7273 6974 7920 6f66  it University of
+000003a0: 2057 6173 6869 6e67 746f 6e2e 0a0a 0a23   Washington....#
+000003b0: 2320 486f 7720 646f 2049 2067 6574 2073  # How do I get s
+000003c0: 7461 7274 6564 2077 6974 6820 4d65 6761  tarted with Mega
+000003d0: 4465 7465 6374 6f72 3f0a 0a2a 2049 6620  Detector?..* If 
+000003e0: 796f 7520 6172 6520 6c6f 6f6b 696e 6720  you are looking 
+000003f0: 666f 7220 6120 636f 6e76 656e 6965 6e74  for a convenient
+00000400: 2074 6f6f 6c20 746f 2072 756e 204d 6567   tool to run Meg
+00000410: 6144 6574 6563 746f 722c 2079 6f75 2064  aDetector, you d
+00000420: 6f6e 2774 206e 6565 6420 616e 7974 6869  on't need anythi
+00000430: 6e67 2066 726f 6d20 7468 6973 2072 6570  ng from this rep
+00000440: 6f73 6974 6f72 793a 2063 6865 636b 206f  ository: check o
+00000450: 7574 205b 4563 6f41 7373 6973 745d 2868  ut [EcoAssist](h
+00000460: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00000470: 6d2f 5065 7465 7276 616e 4c75 6e74 6572  m/PetervanLunter
+00000480: 656e 2f45 636f 4173 7369 7374 3f74 6162  en/EcoAssist?tab
+00000490: 3d72 6561 646d 652d 6f76 2d66 696c 6529  =readme-ov-file)
+000004a0: 2e0a 2a20 4966 2079 6f75 2772 6520 6a75  ..* If you're ju
+000004b0: 7374 203c 693e 636f 6e73 6964 6572 696e  st <i>considerin
+000004c0: 673c 2f69 3e20 7468 6520 7573 6520 6f66  g</i> the use of
+000004d0: 2041 4920 696e 2079 6f75 7220 776f 726b   AI in your work
+000004e0: 666c 6f77 2c20 616e 6420 796f 7520 6172  flow, and you ar
+000004f0: 656e 2774 2065 7665 6e20 7375 7265 2079  en't even sure y
+00000500: 6574 2077 6865 7468 6572 204d 6567 6144  et whether MegaD
+00000510: 6574 6563 746f 7220 776f 756c 6420 6265  etector would be
+00000520: 2075 7365 6675 6c20 746f 2079 6f75 2c20   useful to you, 
+00000530: 7765 2072 6563 6f6d 6d65 6e64 2072 6561  we recommend rea
+00000540: 6469 6e67 2074 6865 2022 5b67 6574 7469  ding the "[getti
+00000550: 6e67 2073 7461 7274 6564 2077 6974 6820  ng started with 
+00000560: 4d65 6761 4465 7465 6374 6f72 5d28 636f  MegaDetector](co
+00000570: 6c6c 6162 6f72 6174 696f 6e73 2e6d 6429  llaborations.md)
+00000580: 2220 7061 6765 2e0a 2a20 4966 2079 6f75  " page..* If you
+00000590: 2772 6520 616c 7265 6164 7920 6661 6d69  're already fami
+000005a0: 6c69 6172 2077 6974 6820 4d65 6761 4465  liar with MegaDe
+000005b0: 7465 6374 6f72 2061 6e64 2079 6f75 2772  tector and you'r
+000005c0: 6520 7265 6164 7920 746f 2072 756e 2069  e ready to run i
+000005d0: 7420 6f6e 2079 6f75 7220 6461 7461 2c20  t on your data, 
+000005e0: 7365 6520 7468 6520 5b4d 6567 6144 6574  see the [MegaDet
+000005f0: 6563 746f 7220 5573 6572 2047 7569 6465  ector User Guide
+00000600: 5d28 6d65 6761 6465 7465 6374 6f72 2e6d  ](megadetector.m
+00000610: 6429 2066 6f72 2069 6e73 7472 7563 7469  d) for instructi
+00000620: 6f6e 7320 6f6e 2072 756e 6e69 6e67 204d  ons on running M
+00000630: 6567 6144 6574 6563 746f 722e 0a2a 2049  egaDetector..* I
+00000640: 6620 796f 7527 7265 2061 2070 726f 6772  f you're a progr
+00000650: 616d 6d65 722d 7479 7065 206c 6f6f 6b69  ammer-type looki
+00000660: 6e67 2074 6f20 7573 6520 746f 6f6c 7320  ng to use tools 
+00000670: 6672 6f6d 2074 6869 7320 7265 706f 2c20  from this repo, 
+00000680: 6368 6563 6b20 6f75 7420 7468 6520 5b50  check out the [P
+00000690: 7974 686f 6e20 7061 636b 6167 655d 2868  ython package](h
+000006a0: 7474 7073 3a2f 2f70 7970 692e 6f72 672f  ttps://pypi.org/
+000006b0: 7072 6f6a 6563 742f 6d65 6761 6465 7465  project/megadete
+000006c0: 6374 6f72 2f29 2074 6861 7420 7072 6f76  ctor/) that prov
+000006d0: 6964 6573 2061 6363 6573 7320 746f 2065  ides access to e
+000006e0: 7665 7279 7468 696e 6720 696e 2074 6869  verything in thi
+000006f0: 7320 7265 706f 2028 7965 732c 2079 6f75  s repo (yes, you
+00000700: 2067 7565 7373 6564 2069 742c 2022 7069   guessed it, "pi
+00000710: 7020 696e 7374 616c 6c20 6d65 6761 6465  p install megade
+00000720: 7465 6374 6f72 2229 2e0a 2a20 4966 2079  tector")..* If y
+00000730: 6f75 2068 6176 6520 616e 7920 7175 6573  ou have any ques
+00000740: 7469 6f6e 732c 206f 7220 796f 7520 7761  tions, or you wa
+00000750: 6e74 2074 6f20 7465 6c6c 2075 7320 7468  nt to tell us th
+00000760: 6174 204d 6567 6144 6574 6563 746f 7220  at MegaDetector 
+00000770: 7761 7320 616d 617a 696e 672f 7465 7272  was amazing/terr
+00000780: 6962 6c65 206f 6e20 796f 7572 2069 6d61  ible on your ima
+00000790: 6765 732c 203c 6120 6872 6566 3d22 6d61  ges, <a href="ma
+000007a0: 696c 746f 3a63 616d 6572 6174 7261 7073  ilto:cameratraps
+000007b0: 406c 696c 612e 7363 6965 6e63 6522 3e65  @lila.science">e
+000007c0: 6d61 696c 2075 733c 2f61 3e21 0a0a 4d65  mail us</a>!..Me
+000007d0: 6761 4465 7465 6374 6f72 2069 7320 6a75  gaDetector is ju
+000007e0: 7374 206f 6e65 206f 6620 6d61 6e79 2074  st one of many t
+000007f0: 6f6f 6c73 2074 6861 7420 6169 6d73 2074  ools that aims t
+00000800: 6f20 6d61 6b65 2063 6f6e 7365 7276 6174  o make conservat
+00000810: 696f 6e20 6269 6f6c 6f67 6973 7473 206d  ion biologists m
+00000820: 6f72 6520 6566 6669 6369 656e 7420 7769  ore efficient wi
+00000830: 7468 2041 492e 2020 4966 2079 6f75 2077  th AI.  If you w
+00000840: 616e 7420 746f 206c 6561 726e 2061 626f  ant to learn abo
+00000850: 7574 206f 7468 6572 2077 6179 7320 746f  ut other ways to
+00000860: 2075 7365 2041 4920 746f 2061 6363 656c   use AI to accel
+00000870: 6572 6174 6520 6361 6d65 7261 2074 7261  erate camera tra
+00000880: 7020 776f 726b 666c 6f77 732c 2063 6865  p workflows, che
+00000890: 636b 206f 7574 206f 7572 206f 6620 7468  ck out our of th
+000008a0: 6520 6669 656c 642c 2061 6666 6563 7469  e field, affecti
+000008b0: 6f6e 6174 656c 7920 7469 746c 6564 2026  onately titled &
+000008c0: 6c64 7175 6f3b 5b45 7665 7279 7468 696e  ldquo;[Everythin
+000008d0: 6720 4920 6b6e 6f77 2061 626f 7574 206d  g I know about m
+000008e0: 6163 6869 6e65 206c 6561 726e 696e 6720  achine learning 
+000008f0: 616e 6420 6361 6d65 7261 2074 7261 7073  and camera traps
+00000900: 5d28 6874 7470 733a 2f2f 6167 656e 746d  ](https://agentm
+00000910: 6f72 7269 732e 6769 7468 7562 2e69 6f2f  orris.github.io/
+00000920: 6361 6d65 7261 2d74 7261 702d 6d6c 2d73  camera-trap-ml-s
+00000930: 7572 7665 792f 2926 7264 7175 6f3b 2e0a  urvey/)&rdquo;..
+00000940: 0a0a 2323 2057 686f 2069 7320 7573 696e  ..## Who is usin
+00000950: 6720 4d65 6761 4465 7465 6374 6f72 3f0a  g MegaDetector?.
+00000960: 0a57 6520 776f 726b 2077 6974 6820 6563  .We work with ec
+00000970: 6f6c 6f67 6973 7473 2061 6c6c 206f 7665  ologists all ove
+00000980: 7220 7468 6520 776f 726c 6420 746f 2068  r the world to h
+00000990: 656c 7020 7468 656d 2073 7065 6e64 206c  elp them spend l
+000009a0: 6573 7320 7469 6d65 2061 6e6e 6f74 6174  ess time annotat
+000009b0: 696e 6720 696d 6167 6573 2061 6e64 206d  ing images and m
+000009c0: 6f72 6520 7469 6d65 2074 6869 6e6b 696e  ore time thinkin
+000009d0: 6720 6162 6f75 7420 636f 6e73 6572 7661  g about conserva
+000009e0: 7469 6f6e 2e20 2059 6f75 2063 616e 2072  tion.  You can r
+000009f0: 6561 6420 6120 6c69 7474 6c65 206d 6f72  ead a little mor
+00000a00: 6520 6162 6f75 7420 686f 7720 7468 6973  e about how this
+00000a10: 2077 6f72 6b73 206f 6e20 6f75 7220 5b67   works on our [g
+00000a20: 6574 7469 6e67 2073 7461 7274 6564 2077  etting started w
+00000a30: 6974 6820 4d65 6761 4465 7465 6374 6f72  ith MegaDetector
+00000a40: 5d28 636f 6c6c 6162 6f72 6174 696f 6e73  ](collaborations
+00000a50: 2e6d 6429 2070 6167 652e 0a0a 4865 7265  .md) page...Here
+00000a60: 2061 7265 2061 2066 6577 206f 6620 7468   are a few of th
+00000a70: 6520 6f72 6761 6e69 7a61 7469 6f6e 7320  e organizations 
+00000a80: 7468 6174 2068 6176 6520 7573 6564 204d  that have used M
+00000a90: 6567 6144 6574 6563 746f 722e 2e2e 2077  egaDetector... w
+00000aa0: 6527 7265 206f 6e6c 7920 6c69 7374 696e  e're only listin
+00000ab0: 6720 6f72 6761 6e69 7a61 7469 6f6e 7320  g organizations 
+00000ac0: 7768 6f20 2861 2920 7765 206b 6e6f 7720  who (a) we know 
+00000ad0: 6162 6f75 7420 616e 6420 2862 2920 6861  about and (b) ha
+00000ae0: 7665 2067 6976 656e 2075 7320 7065 726d  ve given us perm
+00000af0: 6973 7369 6f6e 2074 6f20 7265 6665 7220  ission to refer 
+00000b00: 746f 2074 6865 6d20 6865 7265 2028 6f72  to them here (or
+00000b10: 2068 6176 6520 706f 7374 6564 2070 7562   have posted pub
+00000b20: 6c69 636c 7920 6162 6f75 7420 7468 6569  licly about thei
+00000b30: 7220 7573 6520 6f66 204d 6567 6144 6574  r use of MegaDet
+00000b40: 6563 746f 7229 2c20 736f 2069 6620 796f  ector), so if yo
+00000b50: 7527 7265 2075 7369 6e67 204d 6567 6144  u're using MegaD
+00000b60: 6574 6563 746f 7220 6f72 206f 7468 6572  etector or other
+00000b70: 2074 6f6f 6c73 2066 726f 6d20 7468 6973   tools from this
+00000b80: 2072 6570 6f20 616e 6420 776f 756c 6420   repo and would 
+00000b90: 6c69 6b65 2074 6f20 6265 2061 6464 6564  like to be added
+00000ba0: 2074 6f20 7468 6973 206c 6973 742c 203c   to this list, <
+00000bb0: 6120 6872 6566 3d22 6d61 696c 746f 3a63  a href="mailto:c
+00000bc0: 616d 6572 6174 7261 7073 406c 696c 612e  ameratraps@lila.
+00000bd0: 7363 6965 6e63 6522 3e65 6d61 696c 2075  science">email u
+00000be0: 733c 2f61 3e21 0a0a 2a20 5b41 7269 7a6f  s</a>!..* [Arizo
+00000bf0: 6e61 2044 6570 6172 746d 656e 7420 6f66  na Department of
+00000c00: 2045 6e76 6972 6f6e 6d65 6e74 616c 2051   Environmental Q
+00000c10: 7561 6c69 7479 5d28 6874 7470 3a2f 2f61  uality](http://a
+00000c20: 7a64 6571 2e67 6f76 2f29 0a2a 205b 4269  zdeq.gov/).* [Bi
+00000c30: 6f6d 6574 7269 6f2e 6561 7274 685d 2868  ometrio.earth](h
+00000c40: 7474 7073 3a2f 2f62 696f 6d65 7472 696f  ttps://biometrio
+00000c50: 2e65 6172 7468 2f29 0a2a 205b 426c 6163  .earth/).* [Blac
+00000c60: 6b62 6972 6420 456e 7669 726f 6e6d 656e  kbird Environmen
+00000c70: 7461 6c5d 2868 7474 7073 3a2f 2f62 6c61  tal](https://bla
+00000c80: 636b 6269 7264 656e 762e 636f 6d2f 290a  ckbirdenv.com/).
+00000c90: 2a20 5b43 616d 656c 6f74 5d28 6874 7470  * [Camelot](http
+00000ca0: 733a 2f2f 6361 6d65 6c6f 7470 726f 6a65  s://camelotproje
+00000cb0: 6374 2e6f 7267 2f29 0a2a 205b 4361 6e61  ct.org/).* [Cana
+00000cc0: 6469 616e 2050 6172 6b73 2061 6e64 2057  dian Parks and W
+00000cd0: 696c 6465 726e 6573 7320 536f 6369 6574  ilderness Societ
+00000ce0: 7920 2843 5041 5753 2920 4e6f 7274 6865  y (CPAWS) Northe
+00000cf0: 726e 2041 6c62 6572 7461 2043 6861 7074  rn Alberta Chapt
+00000d00: 6572 5d28 6874 7470 733a 2f2f 6370 6177  er](https://cpaw
+00000d10: 736e 6162 2e6f 7267 2f29 0a2a 205b 436f  snab.org/).* [Co
+00000d20: 6e73 6572 7661 7469 6f6e 2058 204c 6162  nservation X Lab
+00000d30: 735d 2868 7474 7073 3a2f 2f63 6f6e 7365  s](https://conse
+00000d40: 7276 6174 696f 6e78 6c61 6273 2e63 6f6d  rvationxlabs.com
+00000d50: 2f29 0a2a 205b 437a 6563 6820 556e 6976  /).* [Czech Univ
+00000d60: 6572 7369 7479 206f 6620 4c69 6665 2053  ersity of Life S
+00000d70: 6369 656e 6365 7320 5072 6167 7565 5d28  ciences Prague](
+00000d80: 6874 7470 733a 2f2f 7777 772e 637a 752e  https://www.czu.
+00000d90: 637a 2f65 6e29 0a2a 205b 4475 6465 6b20  cz/en).* [Dudek 
+00000da0: 4361 6d65 7261 2054 7261 7020 4149 2049  Camera Trap AI I
+00000db0: 6d61 6765 2054 6f6f 6c6b 6974 2028 4149  mage Toolkit (AI
+00000dc0: 5429 5d28 6874 7470 733a 2f2f 6475 6465  T)](https://dude
+00000dd0: 6b2e 636f 6d2f 7365 7276 6963 6573 2f77  k.com/services/w
+00000de0: 696c 646c 6966 652d 6361 6d65 7261 2d74  ildlife-camera-t
+00000df0: 7261 702d 6169 2d69 6d61 6765 2d70 726f  rap-ai-image-pro
+00000e00: 6365 7373 696e 672d 616e 642d 6d61 6e61  cessing-and-mana
+00000e10: 6765 6d65 6e74 2f29 0a2a 205b 4563 6f4c  gement/).* [EcoL
+00000e20: 6f67 6963 2043 6f6e 7375 6c74 616e 7473  ogic Consultants
+00000e30: 204c 7464 2e5d 2868 7474 7073 3a2f 2f77   Ltd.](https://w
+00000e40: 7777 2e63 6f6e 7375 6c74 2d65 636f 6c6f  ww.consult-ecolo
+00000e50: 6769 632e 636f 6d2f 290a 2a20 5b45 7374  gic.com/).* [Est
+00000e60: 6163 69c3 b36e 2042 696f 6cc3 b367 6963  aci..n Biol..gic
+00000e70: 6120 6465 2044 6fc3 b161 6e61 5d28 6874  a de Do..ana](ht
+00000e80: 7470 3a2f 2f77 7777 2e65 6264 2e63 7369  tp://www.ebd.csi
+00000e90: 632e 6573 2f69 6e69 6369 6f29 0a2a 205b  c.es/inicio).* [
+00000ea0: 496e 6469 6765 6e6f 7573 2044 6573 6572  Indigenous Deser
+00000eb0: 7420 416c 6c69 616e 6365 5d28 6874 7470  t Alliance](http
+00000ec0: 733a 2f2f 7777 772e 696e 6469 6765 6e6f  s://www.indigeno
+00000ed0: 7573 6465 7365 7274 616c 6c69 616e 6365  usdesertalliance
+00000ee0: 2e63 6f6d 2f29 0a2a 205b 4d79 616c 6c20  .com/).* [Myall 
+00000ef0: 4c61 6b65 7320 4469 6e67 6f20 5072 6f6a  Lakes Dingo Proj
+00000f00: 6563 745d 2868 7474 7073 3a2f 2f63 6172  ect](https://car
+00000f10: 6e69 766f 7265 636f 6578 6973 7465 6e63  nivorecoexistenc
+00000f20: 652e 696e 666f 2f6d 7961 6c6c 2d6c 616b  e.info/myall-lak
+00000f30: 6573 2d64 696e 676f 2d70 726f 6a65 6374  es-dingo-project
+00000f40: 2f29 0a2a 205b 4e6f 7277 6567 6961 6e20  /).* [Norwegian 
+00000f50: 496e 7374 6974 7574 6520 666f 7220 4e61  Institute for Na
+00000f60: 7475 7265 2052 6573 6561 7263 685d 2868  ture Research](h
+00000f70: 7474 7073 3a2f 2f77 7777 2e6e 696e 612e  ttps://www.nina.
+00000f80: 6e6f 2f65 6e67 6c69 7368 2f48 6f6d 6529  no/english/Home)
+00000f90: 0a2a 205b 4f6b 616c 615d 2868 7474 7073  .* [Okala](https
+00000fa0: 3a2f 2f77 7777 2e6f 6b61 6c61 2e69 6f2f  ://www.okala.io/
+00000fb0: 290a 2a20 5b50 6f69 6e74 204e 6f20 506f  ).* [Point No Po
+00000fc0: 696e 7420 5472 6561 7479 2043 6f75 6e63  int Treaty Counc
+00000fd0: 696c 5d28 6874 7470 733a 2f2f 706e 7074  il](https://pnpt
+00000fe0: 632e 6f72 672f 290a 2a20 5b52 616d 6174  c.org/).* [Ramat
+00000ff0: 2048 616e 6164 6976 204e 6174 7572 6520   Hanadiv Nature 
+00001000: 5061 726b 5d28 6874 7470 733a 2f2f 7777  Park](https://ww
+00001010: 772e 7261 6d61 742d 6861 6e61 6469 762e  w.ramat-hanadiv.
+00001020: 6f72 672e 696c 2f65 6e2f 290a 2a20 5b53  org.il/en/).* [S
+00001030: 5045 4120 2850 6f72 7475 6775 6573 6520  PEA (Portuguese 
+00001040: 536f 6369 6574 7920 666f 7220 7468 6520  Society for the 
+00001050: 5374 7564 7920 6f66 2042 6972 6473 295d  Study of Birds)]
+00001060: 2868 7474 7073 3a2f 2f73 7065 612e 7074  (https://spea.pt
+00001070: 2f65 6e2f 290a 2a20 5b53 6b79 2049 736c  /en/).* [Sky Isl
+00001080: 616e 6420 416c 6c69 616e 6365 5d28 6874  and Alliance](ht
+00001090: 7470 733a 2f2f 736b 7969 736c 616e 6461  tps://skyislanda
+000010a0: 6c6c 6961 6e63 652e 6f72 672f 290a 2a20  lliance.org/).* 
+000010b0: 5b53 796e 7468 6574 6169 635d 2868 7474  [Synthetaic](htt
+000010c0: 7073 3a2f 2f77 7777 2e73 796e 7468 6574  ps://www.synthet
+000010d0: 6169 632e 636f 6d2f 290a 2a20 5b54 6172  aic.com/).* [Tar
+000010e0: 6f6e 6761 2043 6f6e 7365 7276 6174 696f  onga Conservatio
+000010f0: 6e20 536f 6369 6574 795d 2868 7474 7073  n Society](https
+00001100: 3a2f 2f74 6172 6f6e 6761 2e6f 7267 2e61  ://taronga.org.a
+00001110: 752f 290a 2a20 5b54 6865 204e 6174 7572  u/).* [The Natur
+00001120: 6520 436f 6e73 6572 7661 6e63 7920 696e  e Conservancy in
+00001130: 2057 796f 6d69 6e67 5d28 6874 7470 733a   Wyoming](https:
+00001140: 2f2f 7777 772e 6e61 7475 7265 2e6f 7267  //www.nature.org
+00001150: 2f65 6e2d 7573 2f61 626f 7574 2d75 732f  /en-us/about-us/
+00001160: 7768 6572 652d 7765 2d77 6f72 6b2f 756e  where-we-work/un
+00001170: 6974 6564 2d73 7461 7465 732f 7779 6f6d  ited-states/wyom
+00001180: 696e 672f 290a 2a20 5b54 7261 7054 6167  ing/).* [TrapTag
+00001190: 6765 725d 2868 7474 7073 3a2f 2f77 696c  ger](https://wil
+000011a0: 6465 7965 636f 6e73 6572 7661 7469 6f6e  deyeconservation
+000011b0: 2e6f 7267 2f74 7261 702d 7461 6767 6572  .org/trap-tagger
+000011c0: 2d61 626f 7574 2f29 0a2a 205b 556e 6976  -about/).* [Univ
+000011d0: 6572 7369 7479 206f 6620 4361 6c69 666f  ersity of Califo
+000011e0: 726e 6961 2044 6176 6973 204e 6174 7572  rnia Davis Natur
+000011f0: 616c 2052 6573 6572 7665 735d 2868 7474  al Reserves](htt
+00001200: 7073 3a2f 2f6e 6174 7572 616c 7265 7365  ps://naturalrese
+00001210: 7276 6573 2e75 6364 6176 6973 2e65 6475  rves.ucdavis.edu
+00001220: 2f29 0a2a 205b 5570 7065 7220 5965 6c6c  /).* [Upper Yell
+00001230: 6f77 7374 6f6e 6520 5761 7465 7273 6865  owstone Watershe
+00001240: 6420 4772 6f75 705d 2868 7474 7073 3a2f  d Group](https:/
+00001250: 2f77 7777 2e75 7070 6572 7965 6c6c 6f77  /www.upperyellow
+00001260: 7374 6f6e 652e 6f72 672f 290a 2a20 5b5a  stone.org/).* [Z
+00001270: 616d 6261 2043 6c6f 7564 5d28 6874 7470  amba Cloud](http
+00001280: 733a 2f2f 7777 772e 7a61 6d62 6163 6c6f  s://www.zambaclo
+00001290: 7564 2e63 6f6d 2f29 0a2a 205b 5061 7263  ud.com/).* [Parc
+000012a0: 206e 6174 696f 6e61 6c20 6475 204d 6f6e   national du Mon
+000012b0: 742d 5472 656d 626c 616e 745d 2868 7474  t-Tremblant](htt
+000012c0: 7073 3a2f 2f77 7777 2e73 6570 6171 2e63  ps://www.sepaq.c
+000012d0: 6f6d 2f70 712f 6d6f 742f 696e 6465 782e  om/pq/mot/index.
+000012e0: 646f 743f 6c61 6e67 7561 6765 5f69 643d  dot?language_id=
+000012f0: 3129 0a2a 205b 5468 6520 4c61 6e64 2042  1).* [The Land B
+00001300: 616e 6b69 6e67 2047 726f 7570 5d28 6874  anking Group](ht
+00001310: 7470 733a 2f2f 7468 656c 616e 6462 616e  tps://thelandban
+00001320: 6b69 6e67 6772 6f75 702e 636f 6d2f 290a  kinggroup.com/).
+00001330: 2a20 5b4e 6577 205a 6561 6c61 6e64 2044  * [New Zealand D
+00001340: 6570 6172 746d 656e 7420 6f66 2043 6f6e  epartment of Con
+00001350: 7365 7276 6174 696f 6e5d 2868 7474 7073  servation](https
+00001360: 3a2f 2f77 7777 2e64 6f63 2e67 6f76 742e  ://www.doc.govt.
+00001370: 6e7a 290a 0a2a 205b 4170 706c 6965 6420  nz)..* [Applied 
+00001380: 436f 6e73 6572 7661 7469 6f6e 204d 6163  Conservation Mac
+00001390: 726f 2045 636f 6c6f 6779 204c 6162 5d28  ro Ecology Lab](
+000013a0: 6874 7470 3a2f 2f77 7777 2e61 636d 656c  http://www.acmel
+000013b0: 6162 2e63 612f 292c 2055 6e69 7665 7273  ab.ca/), Univers
+000013c0: 6974 7920 6f66 2056 6963 746f 7269 610a  ity of Victoria.
+000013d0: 2a20 5b42 616e 6666 204e 6174 696f 6e61  * [Banff Nationa
+000013e0: 6c20 5061 726b 2052 6573 6f75 7263 6520  l Park Resource 
+000013f0: 436f 6e73 6572 7661 7469 6f6e 5d28 6874  Conservation](ht
+00001400: 7470 733a 2f2f 7777 772e 7063 2e67 632e  tps://www.pc.gc.
+00001410: 6361 2f65 6e2f 706e 2d6e 702f 6162 2f62  ca/en/pn-np/ab/b
+00001420: 616e 6666 2f6e 6174 7572 652f 636f 6e73  anff/nature/cons
+00001430: 6572 7661 7469 6f6e 292c 2050 6172 6b73  ervation), Parks
+00001440: 2043 616e 6164 610a 2a20 5b42 6c75 6d73   Canada.* [Blums
+00001450: 7465 696e 204c 6162 5d28 6874 7470 733a  tein Lab](https:
+00001460: 2f2f 626c 756d 7374 6569 6e6c 6162 2e65  //blumsteinlab.e
+00001470: 6562 2e75 636c 612e 6564 752f 292c 2055  eb.ucla.edu/), U
+00001480: 434c 410a 2a20 5b42 6f72 6465 726c 616e  CLA.* [Borderlan
+00001490: 6473 2052 6573 6561 7263 6820 496e 7374  ds Research Inst
+000014a0: 6974 7574 655d 2868 7474 7073 3a2f 2f62  itute](https://b
+000014b0: 7269 2e73 756c 726f 7373 2e65 6475 2f29  ri.sulross.edu/)
+000014c0: 2c20 5375 6c20 526f 7373 2053 7461 7465  , Sul Ross State
+000014d0: 2055 6e69 7665 7273 6974 790a 2a20 5b43   University.* [C
+000014e0: 6170 6974 6f6c 2052 6565 6620 4e61 7469  apitol Reef Nati
+000014f0: 6f6e 616c 2050 6172 6b5d 2868 7474 7073  onal Park](https
+00001500: 3a2f 2f77 7777 2e6e 7073 2e67 6f76 2f63  ://www.nps.gov/c
+00001510: 6172 652f 696e 6465 782e 6874 6d29 202f  are/index.htm) /
+00001520: 2055 7461 6820 5661 6c6c 6579 2055 6e69   Utah Valley Uni
+00001530: 7665 7273 6974 790a 2a20 5b43 656e 7465  versity.* [Cente
+00001540: 7220 666f 7220 4269 6f64 6976 6572 7369  r for Biodiversi
+00001550: 7479 2061 6e64 2043 6f6e 7365 7276 6174  ty and Conservat
+00001560: 696f 6e5d 2868 7474 7073 3a2f 2f77 7777  ion](https://www
+00001570: 2e61 6d6e 682e 6f72 672f 7265 7365 6172  .amnh.org/resear
+00001580: 6368 2f63 656e 7465 722d 666f 722d 6269  ch/center-for-bi
+00001590: 6f64 6976 6572 7369 7479 2d63 6f6e 7365  odiversity-conse
+000015a0: 7276 6174 696f 6e29 2c20 416d 6572 6963  rvation), Americ
+000015b0: 616e 204d 7573 6575 6d20 6f66 204e 6174  an Museum of Nat
+000015c0: 7572 616c 2048 6973 746f 7279 0a2a 205b  ural History.* [
+000015d0: 4365 6e74 7265 2066 6f72 2045 636f 7379  Centre for Ecosy
+000015e0: 7374 656d 2053 6369 656e 6365 5d28 6874  stem Science](ht
+000015f0: 7470 733a 2f2f 7777 772e 756e 7377 2e65  tps://www.unsw.e
+00001600: 6475 2e61 752f 7265 7365 6172 6368 2f29  du.au/research/)
+00001610: 2c20 554e 5357 2053 7964 6e65 790a 2a20  , UNSW Sydney.* 
+00001620: 5b43 726f 7373 2d43 756c 7475 7261 6c20  [Cross-Cultural 
+00001630: 4563 6f6c 6f67 7920 4c61 625d 2868 7474  Ecology Lab](htt
+00001640: 7073 3a2f 2f63 726f 7373 6375 6c74 7572  ps://crosscultur
+00001650: 616c 6563 6f6c 6f67 792e 6e65 742f 292c  alecology.net/),
+00001660: 204d 6163 7175 6172 6965 2055 6e69 7665   Macquarie Unive
+00001670: 7273 6974 790a 2a20 5b44 4320 4361 7420  rsity.* [DC Cat 
+00001680: 436f 756e 745d 2868 7474 7073 3a2f 2f68  Count](https://h
+00001690: 7562 2e64 6363 6174 636f 756e 742e 6f72  ub.dccatcount.or
+000016a0: 672f 292c 206c 6564 2062 7920 7468 6520  g/), led by the 
+000016b0: 4875 6d61 6e65 2052 6573 6375 6520 416c  Humane Rescue Al
+000016c0: 6c69 616e 6365 0a2a 205b 4465 7061 7274  liance.* [Depart
+000016d0: 6d65 6e74 206f 6620 4669 7368 2061 6e64  ment of Fish and
+000016e0: 2057 696c 646c 6966 6520 5363 6965 6e63   Wildlife Scienc
+000016f0: 6573 5d28 6874 7470 733a 2f2f 7777 772e  es](https://www.
+00001700: 7569 6461 686f 2e65 6475 2f63 6e72 2f64  uidaho.edu/cnr/d
+00001710: 6570 6172 746d 656e 7473 2f66 6973 682d  epartments/fish-
+00001720: 616e 642d 7769 6c64 6c69 6665 2d73 6369  and-wildlife-sci
+00001730: 656e 6365 7329 2c20 556e 6976 6572 7369  ences), Universi
+00001740: 7479 206f 6620 4964 6168 6f0a 2a20 5b44  ty of Idaho.* [D
+00001750: 6570 6172 746d 656e 7420 6f66 2053 6f63  epartment of Soc
+00001760: 6965 7479 2026 2043 6f6e 7365 7276 6174  iety & Conservat
+00001770: 696f 6e5d 2868 7474 7073 3a2f 2f77 7777  ion](https://www
+00001780: 2e75 6d74 2e65 6475 2f65 6e76 6972 6f6e  .umt.edu/environ
+00001790: 6d65 6e74 2f61 626f 7574 2f64 6570 6172  ment/about/depar
+000017a0: 746d 656e 7473 2f73 6f63 6f6e 2f29 2c20  tments/socon/), 
+000017b0: 572e 412e 2046 7261 6e6b 6520 436f 6c6c  W.A. Franke Coll
+000017c0: 6567 6520 6f66 2046 6f72 6573 7472 7920  ege of Forestry 
+000017d0: 2620 436f 6e73 6572 7661 7469 6f6e 2c20  & Conservation, 
+000017e0: 556e 6976 6572 7369 7479 206f 6620 4d6f  University of Mo
+000017f0: 6e74 616e 610a 2a20 5b44 6570 6172 746d  ntana.* [Departm
+00001800: 656e 7420 6f66 2057 696c 646c 6966 6520  ent of Wildlife 
+00001810: 4563 6f6c 6f67 7920 616e 6420 436f 6e73  Ecology and Cons
+00001820: 6572 7661 7469 6f6e 5d28 6874 7470 733a  ervation](https:
+00001830: 2f2f 7765 632e 6966 6173 2e75 666c 2e65  //wec.ifas.ufl.e
+00001840: 6475 2f29 2c20 556e 6976 6572 7369 7479  du/), University
+00001850: 206f 6620 466c 6f72 6964 610a 2a20 5b45   of Florida.* [E
+00001860: 636f 6c6f 6779 2061 6e64 2043 6f6e 7365  cology and Conse
+00001870: 7276 6174 696f 6e20 6f66 2041 6d61 7a6f  rvation of Amazo
+00001880: 6e69 616e 2056 6572 7465 6272 6174 6573  nian Vertebrates
+00001890: 2052 6573 6561 7263 6820 4772 6f75 705d   Research Group]
+000018a0: 2868 7474 7073 3a2f 2f77 7777 2e72 6573  (https://www.res
+000018b0: 6561 7263 6867 6174 652e 6e65 742f 6c61  earchgate.net/la
+000018c0: 622f 4665 726e 616e 6461 2d4d 6963 6861  b/Fernanda-Micha
+000018d0: 6c73 6b69 2d4c 6162 2d34 292c 2046 6564  lski-Lab-4), Fed
+000018e0: 6572 616c 2055 6e69 7665 7273 6974 7920  eral University 
+000018f0: 6f66 2041 6d61 70c3 a10a 2a20 5b47 6f6c  of Amap...* [Gol
+00001900: 6120 466f 7265 7374 2050 726f 6772 616d  a Forest Program
+00001910: 6d61 5d28 6874 7470 733a 2f2f 7777 772e  ma](https://www.
+00001920: 7273 7062 2e6f 7267 2e75 6b2f 6f75 722d  rspb.org.uk/our-
+00001930: 776f 726b 2f63 6f6e 7365 7276 6174 696f  work/conservatio
+00001940: 6e2f 7072 6f6a 6563 7473 2f73 6369 656e  n/projects/scien
+00001950: 7469 6669 632d 7375 7070 6f72 742d 666f  tific-support-fo
+00001960: 722d 7468 652d 676f 6c61 2d66 6f72 6573  r-the-gola-fores
+00001970: 742d 7072 6f67 7261 6d6d 652f 292c 2052  t-programme/), R
+00001980: 6f79 616c 2053 6f63 6965 7479 2066 6f72  oyal Society for
+00001990: 2074 6865 2050 726f 7465 6374 696f 6e20   the Protection 
+000019a0: 6f66 2042 6972 6473 2028 5253 5042 290a  of Birds (RSPB).
+000019b0: 2a20 5b47 7261 656d 6520 5368 616e 6e6f  * [Graeme Shanno
+000019c0: 6e27 7320 5265 7365 6172 6368 2047 726f  n's Research Gro
+000019d0: 7570 5d28 6874 7470 733a 2f2f 7769 6c64  up](https://wild
+000019e0: 6c69 6665 7265 7365 6172 6368 2e63 6f2e  liferesearch.co.
+000019f0: 756b 2f67 726f 7570 2d31 292c 2042 616e  uk/group-1), Ban
+00001a00: 676f 7220 556e 6976 6572 7369 7479 200a  gor University .
+00001a10: 2a20 5b47 7269 7a7a 6c79 2042 6561 7220  * [Grizzly Bear 
+00001a20: 5265 636f 7665 7279 2050 726f 6772 616d  Recovery Program
+00001a30: 5d28 6874 7470 733a 2f2f 7777 772e 6677  ](https://www.fw
+00001a40: 732e 676f 762f 6f66 6669 6365 2f67 7269  s.gov/office/gri
+00001a50: 7a7a 6c79 2d62 6561 722d 7265 636f 7665  zzly-bear-recove
+00001a60: 7279 2d70 726f 6772 616d 292c 2055 2e53  ry-program), U.S
+00001a70: 2e20 4669 7368 2026 2057 696c 646c 6966  . Fish & Wildlif
+00001a80: 6520 5365 7276 6963 650a 2a20 5b48 616d  e Service.* [Ham
+00001a90: 6161 7261 675d 2868 7474 7073 3a2f 2f68  aarag](https://h
+00001aa0: 616d 6161 7261 672e 6f72 672e 696c 2f29  amaarag.org.il/)
+00001ab0: 2c20 5468 6520 5374 6569 6e68 6172 6474  , The Steinhardt
+00001ac0: 204d 7573 6575 6d20 6f66 204e 6174 7572   Museum of Natur
+00001ad0: 616c 2048 6973 746f 7279 2c20 5465 6c20  al History, Tel 
+00001ae0: 4176 6976 2055 6e69 7665 7273 6974 790a  Aviv University.
+00001af0: 2a20 5b49 6e73 7469 7475 7420 6465 7320  * [Institut des 
+00001b00: 5363 6965 6e63 6520 6465 206c 6120 466f  Science de la Fo
+00001b10: 72c3 aa74 2054 656d 70c3 a972 c3a9 655d  r..t Temp..r..e]
+00001b20: 2868 7474 7073 3a2f 2f69 7366 6f72 742e  (https://isfort.
+00001b30: 7571 6f2e 6361 2f29 2028 4953 464f 5254  uqo.ca/) (ISFORT
+00001b40: 292c 2055 6e69 7665 7273 6974 c3a9 2064  ), Universit.. d
+00001b50: 7520 5175 c3a9 6265 6320 656e 204f 7574  u Qu..bec en Out
+00001b60: 616f 7561 6973 0a2a 205b 4c61 6220 6f66  aouais.* [Lab of
+00001b70: 2044 722e 2042 696c 616c 2048 6162 6962   Dr. Bilal Habib
+00001b80: 5d28 6874 7470 733a 2f2f 6268 6c61 622e  ](https://bhlab.
+00001b90: 696e 2f61 626f 7574 292c 2074 6865 2057  in/about), the W
+00001ba0: 696c 646c 6966 6520 496e 7374 6974 7574  ildlife Institut
+00001bb0: 6520 6f66 2049 6e64 6961 0a2a 205b 4d61  e of India.* [Ma
+00001bc0: 6d6d 616c 2053 7061 7469 616c 2045 636f  mmal Spatial Eco
+00001bd0: 6c6f 6779 2061 6e64 2043 6f6e 7365 7276  logy and Conserv
+00001be0: 6174 696f 6e20 4c61 625d 2868 7474 7073  ation Lab](https
+00001bf0: 3a2f 2f6c 6162 732e 7773 752e 6564 752f  ://labs.wsu.edu/
+00001c00: 6474 686f 726e 746f 6e2f 292c 2057 6173  dthornton/), Was
+00001c10: 6869 6e67 746f 6e20 5374 6174 6520 556e  hington State Un
+00001c20: 6976 6572 7369 7479 0a2a 205b 4d63 4c6f  iversity.* [McLo
+00001c30: 7567 686c 696e 204c 6162 2069 6e20 506f  ughlin Lab in Po
+00001c40: 7075 6c61 7469 6f6e 2045 636f 6c6f 6779  pulation Ecology
+00001c50: 5d28 6874 7470 3a2f 2f6d 636c 6f75 6768  ](http://mclough
+00001c60: 6c69 6e6c 6162 2e63 612f 6c61 622f 292c  linlab.ca/lab/),
+00001c70: 2055 6e69 7665 7273 6974 7920 6f66 2053   University of S
+00001c80: 6173 6b61 7463 6865 7761 6e0a 2a20 5b4e  askatchewan.* [N
+00001c90: 6174 696f 6e61 6c20 5769 6c64 6c69 6665  ational Wildlife
+00001ca0: 2052 6566 7567 6520 5379 7374 656d 2c20   Refuge System, 
+00001cb0: 536f 7574 6877 6573 7420 5265 6769 6f6e  Southwest Region
+00001cc0: 5d28 6874 7470 733a 2f2f 7777 772e 6677  ](https://www.fw
+00001cd0: 732e 676f 762f 6162 6f75 742f 7265 6769  s.gov/about/regi
+00001ce0: 6f6e 2f73 6f75 7468 7765 7374 292c 2055  on/southwest), U
+00001cf0: 2e53 2e20 4669 7368 2026 2057 696c 646c  .S. Fish & Wildl
+00001d00: 6966 6520 5365 7276 6963 650a 2a20 5b4e  ife Service.* [N
+00001d10: 6f72 7468 6572 6e20 4772 6561 7420 506c  orthern Great Pl
+00001d20: 6169 6e73 2050 726f 6772 616d 5d28 6874  ains Program](ht
+00001d30: 7470 733a 2f2f 6e61 7469 6f6e 616c 7a6f  tps://nationalzo
+00001d40: 6f2e 7369 2e65 6475 2f6e 6577 732f 7265  o.si.edu/news/re
+00001d50: 7374 6f72 696e 672d 616d 6572 6963 6173  storing-americas
+00001d60: 2d70 7261 6972 6965 292c 2053 6d69 7468  -prairie), Smith
+00001d70: 736f 6e69 616e 0a2a 205b 506f 6c61 7220  sonian.* [Polar 
+00001d80: 4563 6f6c 6f67 7920 4772 6f75 705d 2868  Ecology Group](h
+00001d90: 7474 7073 3a2f 2f70 6f6c 6172 6563 6f6c  ttps://polarecol
+00001da0: 6f67 7967 726f 7570 2e77 6f72 6470 7265  ogygroup.wordpre
+00001db0: 7373 2e63 6f6d 292c 2055 6e69 7665 7273  ss.com), Univers
+00001dc0: 6974 7920 6f66 2047 6461 6e73 6b0a 2a20  ity of Gdansk.* 
+00001dd0: 5b51 7561 6e74 6974 6174 6976 6520 4563  [Quantitative Ec
+00001de0: 6f6c 6f67 7920 4c61 625d 2868 7474 7073  ology Lab](https
+00001df0: 3a2f 2f64 6570 7473 2e77 6173 6869 6e67  ://depts.washing
+00001e00: 746f 6e2e 6564 752f 7365 6673 7165 6c2f  ton.edu/sefsqel/
+00001e10: 292c 2055 6e69 7665 7273 6974 7920 6f66  ), University of
+00001e20: 2057 6173 6869 6e67 746f 6e0a 2a20 5b53   Washington.* [S
+00001e30: 616e 7461 204d 6f6e 6963 6120 4d6f 756e  anta Monica Moun
+00001e40: 7461 696e 7320 5265 6372 6561 7469 6f6e  tains Recreation
+00001e50: 2041 7265 615d 2868 7474 7073 3a2f 2f77   Area](https://w
+00001e60: 7777 2e6e 7073 2e67 6f76 2f73 616d 6f2f  ww.nps.gov/samo/
+00001e70: 696e 6465 782e 6874 6d29 2c20 4e61 7469  index.htm), Nati
+00001e80: 6f6e 616c 2050 6172 6b20 5365 7276 6963  onal Park Servic
+00001e90: 650a 2a20 5b53 6561 7474 6c65 2055 7262  e.* [Seattle Urb
+00001ea0: 616e 2043 6172 6e69 766f 7265 2050 726f  an Carnivore Pro
+00001eb0: 6a65 6374 5d28 6874 7470 733a 2f2f 7777  ject](https://ww
+00001ec0: 772e 7a6f 6f2e 6f72 672f 7365 6174 746c  w.zoo.org/seattl
+00001ed0: 6563 6172 6e69 766f 7265 7329 2c20 576f  ecarnivores), Wo
+00001ee0: 6f64 6c61 6e64 2050 6172 6b20 5a6f 6f0a  odland Park Zoo.
+00001ef0: 2a20 5b53 6572 7261 2064 6f73 20c3 9372  * [Serra dos ..r
+00001f00: 67c3 a36f 7320 4e61 7469 6f6e 616c 2050  g..os National P
+00001f10: 6172 6b5d 2868 7474 7073 3a2f 2f77 7777  ark](https://www
+00001f20: 2e69 636d 6269 6f2e 676f 762e 6272 2f70  .icmbio.gov.br/p
+00001f30: 6172 6e61 7365 7272 6164 6f73 6f72 6761  arnaserradosorga
+00001f40: 6f73 2f29 2c20 4943 4d42 696f 0a2a 205b  os/), ICMBio.* [
+00001f50: 536e 6170 7368 6f74 2055 5341 5d28 6874  Snapshot USA](ht
+00001f60: 7470 733a 2f2f 656d 616d 6d61 6c2e 7369  tps://emammal.si
+00001f70: 2e65 6475 2f73 6e61 7073 686f 742d 7573  .edu/snapshot-us
+00001f80: 6129 2c20 536d 6974 6873 6f6e 6961 6e0a  a), Smithsonian.
+00001f90: 2a20 5b54 524f 5045 434f 4c4e 4554 2070  * [TROPECOLNET p
+00001fa0: 726f 6a65 6374 5d28 6874 7470 733a 2f2f  roject](https://
+00001fb0: 7777 772e 616e 6162 656e 6974 657a 6c6f  www.anabenitezlo
+00001fc0: 7065 7a2e 636f 6d2f 7265 7365 6172 6368  pez.com/research
+00001fd0: 2f67 6c6f 6261 6c2d 6368 616e 6765 2d62  /global-change-b
+00001fe0: 696f 6c6f 6779 2f74 726f 7065 636f 6c6e  iology/tropecoln
+00001ff0: 6574 2f29 2c20 4d75 7365 6f20 4e61 6369  et/), Museo Naci
+00002000: 6f6e 616c 2064 6520 4369 656e 6369 6173  onal de Ciencias
+00002010: 204e 6174 7572 616c 6573 0a2a 205b 5769   Naturales.* [Wi
+00002020: 6c64 6c69 6665 2043 6f65 7869 7374 656e  ldlife Coexisten
+00002030: 6365 204c 6162 5d28 6874 7470 733a 2f2f  ce Lab](https://
+00002040: 7769 6c64 6c69 6665 2e66 6f72 6573 7472  wildlife.forestr
+00002050: 792e 7562 632e 6361 2f29 2c20 556e 6976  y.ubc.ca/), Univ
+00002060: 6572 7369 7479 206f 6620 4272 6974 6973  ersity of Britis
+00002070: 6820 436f 6c75 6d62 6961 0a2a 205b 5769  h Columbia.* [Wi
+00002080: 6c64 6c69 6665 2052 6573 6561 7263 685d  ldlife Research]
+00002090: 2868 7474 7073 3a2f 2f77 7777 2e64 6677  (https://www.dfw
+000020a0: 2e73 7461 7465 2e6f 722e 7573 2f77 696c  .state.or.us/wil
+000020b0: 646c 6966 652f 7265 7365 6172 6368 2f69  dlife/research/i
+000020c0: 6e64 6578 2e61 7370 292c 204f 7265 676f  ndex.asp), Orego
+000020d0: 6e20 4465 7061 7274 6d65 6e74 206f 6620  n Department of 
+000020e0: 4669 7368 2061 6e64 2057 696c 646c 6966  Fish and Wildlif
+000020f0: 650a 2a20 5b57 696c 646c 6966 6520 4469  e.* [Wildlife Di
+00002100: 7669 7369 6f6e 5d28 6874 7470 733a 2f2f  vision](https://
+00002110: 7777 772e 6d69 6368 6967 616e 2e67 6f76  www.michigan.gov
+00002120: 2f64 6e72 2f61 626f 7574 2f63 6f6e 7461  /dnr/about/conta
+00002130: 6374 2f77 696c 646c 6966 6529 2c20 4d69  ct/wildlife), Mi
+00002140: 6368 6967 616e 2044 6570 6172 746d 656e  chigan Departmen
+00002150: 7420 6f66 204e 6174 7572 616c 2052 6573  t of Natural Res
+00002160: 6f75 7263 6573 0a0a 2a20 4465 7061 7274  ources..* Depart
+00002170: 6d65 6e74 206f 6620 4563 6f6c 6f67 792c  ment of Ecology,
+00002180: 2054 5520 4265 726c 696e 0a2a 2047 686f   TU Berlin.* Gho
+00002190: 7374 2043 6174 2041 6e61 6c79 7469 6373  st Cat Analytics
+000021a0: 0a2a 2050 726f 7465 6374 6564 2041 7265  .* Protected Are
+000021b0: 6173 2055 6e69 742c 2043 616e 6164 6961  as Unit, Canadia
+000021c0: 6e20 5769 6c64 6c69 6665 2053 6572 7669  n Wildlife Servi
+000021d0: 6365 0a0a 2a20 5b53 6368 6f6f 6c20 6f66  ce..* [School of
+000021e0: 204e 6174 7572 616c 2053 6369 656e 6365   Natural Science
+000021f0: 735d 2868 7474 7073 3a2f 2f77 7777 2e75  s](https://www.u
+00002200: 7461 732e 6564 752e 6175 2f6e 6174 7572  tas.edu.au/natur
+00002210: 616c 2d73 6369 656e 6365 7329 2c20 556e  al-sciences), Un
+00002220: 6976 6572 7369 7479 206f 6620 5461 736d  iversity of Tasm
+00002230: 616e 6961 2028 5b73 746f 7279 5d28 6874  ania ([story](ht
+00002240: 7470 733a 2f2f 7777 772e 7574 6173 2e65  tps://www.utas.e
+00002250: 6475 2e61 752f 6162 6f75 742f 6e65 7773  du.au/about/news
+00002260: 2d61 6e64 2d73 746f 7269 6573 2f61 7274  -and-stories/art
+00002270: 6963 6c65 732f 3230 3232 2f31 3230 342d  icles/2022/1204-
+00002280: 696e 6e6f 7661 7469 7665 2d63 616d 6572  innovative-camer
+00002290: 612d 6e65 7477 6f72 6b2d 6b65 6570 732d  a-network-keeps-
+000022a0: 636c 6f73 652d 6579 652d 6f6e 2d74 6173  close-eye-on-tas
+000022b0: 7369 652d 7769 6c64 6c69 6665 2929 0a2a  sie-wildlife)).*
+000022c0: 205b 4b65 6e61 6920 4e61 7469 6f6e 616c   [Kenai National
+000022d0: 2057 696c 646c 6966 6520 5265 6675 6765   Wildlife Refuge
+000022e0: 5d28 6874 7470 733a 2f2f 7777 772e 6677  ](https://www.fw
+000022f0: 732e 676f 762f 7265 6675 6765 2f6b 656e  s.gov/refuge/ken
+00002300: 6169 292c 2055 2e53 2e20 4669 7368 2026  ai), U.S. Fish &
+00002310: 2057 696c 646c 6966 6520 5365 7276 6963   Wildlife Servic
+00002320: 6520 285b 7374 6f72 795d 2868 7474 7073  e ([story](https
+00002330: 3a2f 2f77 7777 2e70 656e 696e 7375 6c61  ://www.peninsula
+00002340: 636c 6172 696f 6e2e 636f 6d2f 7370 6f72  clarion.com/spor
+00002350: 7473 2f72 6566 7567 652d 6e6f 7465 626f  ts/refuge-notebo
+00002360: 6f6b 2d6e 6577 2d74 6563 686e 6f6c 6f67  ok-new-technolog
+00002370: 792d 696e 6372 6561 7365 732d 6566 6669  y-increases-effi
+00002380: 6369 656e 6379 2d6f 662d 7265 6675 6765  ciency-of-refuge
+00002390: 2d63 616d 6572 6173 2f29 290a 0a2a 205b  -cameras/))..* [
+000023a0: 4964 6168 6f20 4465 7061 7274 6d65 6e74  Idaho Department
+000023b0: 206f 6620 4669 7368 2061 6e64 2047 616d   of Fish and Gam
+000023c0: 655d 2868 7474 7073 3a2f 2f69 6466 672e  e](https://idfg.
+000023d0: 6964 6168 6f2e 676f 762f 2920 285b 6661  idaho.gov/) ([fa
+000023e0: 6e63 7920 5042 5320 7669 6465 6f5d 2868  ncy PBS video](h
+000023f0: 7474 7073 3a2f 2f77 7777 2e79 6f75 7475  ttps://www.youtu
+00002400: 6265 2e63 6f6d 2f77 6174 6368 3f76 3d75  be.com/watch?v=u
+00002410: 4573 4c38 455a 4b70 6241 2674 3d32 3631  EsL8EZKpbA&t=261
+00002420: 7326 6162 5f63 6861 6e6e 656c 3d4f 7574  s&ab_channel=Out
+00002430: 646f 6f72 4964 6168 6f29 290a 2a20 5b41  doorIdaho)).* [A
+00002440: 7573 7472 616c 6961 6e20 5769 6c64 6c69  ustralian Wildli
+00002450: 6665 2043 6f6e 7365 7276 616e 6379 5d28  fe Conservancy](
+00002460: 6874 7470 733a 2f2f 7777 772e 6175 7374  https://www.aust
+00002470: 7261 6c69 616e 7769 6c64 6c69 6665 2e6f  ralianwildlife.o
+00002480: 7267 2f29 2028 626c 6f67 2070 6f73 7473  rg/) (blog posts
+00002490: 205b 315d 2868 7474 7073 3a2f 2f77 7777   [1](https://www
+000024a0: 2e61 7573 7472 616c 6961 6e77 696c 646c  .australianwildl
+000024b0: 6966 652e 6f72 672f 6375 7474 696e 672d  ife.org/cutting-
+000024c0: 6564 6765 2d74 6563 686e 6f6c 6f67 792d  edge-technology-
+000024d0: 6465 6c69 7665 7269 6e67 2d65 6666 6963  delivering-effic
+000024e0: 6965 6e63 792d 6761 696e 732d 696e 2d63  iency-gains-in-c
+000024f0: 6f6e 7365 7276 6174 696f 6e2f 292c 205b  onservation/), [
+00002500: 325d 2868 7474 7073 3a2f 2f77 7777 2e61  2](https://www.a
+00002510: 7573 7472 616c 6961 6e77 696c 646c 6966  ustralianwildlif
+00002520: 652e 6f72 672f 6566 6669 6369 656e 6379  e.org/efficiency
+00002530: 2d67 6169 6e73 2d61 742d 7468 652d 6375  -gains-at-the-cu
+00002540: 7474 696e 672d 6564 6765 2d6f 662d 7465  tting-edge-of-te
+00002550: 6368 6e6f 6c6f 6779 2f29 2c20 5b33 5d28  chnology/), [3](
+00002560: 6874 7470 733a 2f2f 7777 772e 6175 7374  https://www.aust
+00002570: 7261 6c69 616e 7769 6c64 6c69 6665 2e6f  ralianwildlife.o
+00002580: 7267 2f66 6564 6572 616c 2d67 7261 6e74  rg/federal-grant
+00002590: 2d74 6f2d 6675 6e64 2d61 692d 7375 7070  -to-fund-ai-supp
+000025a0: 6f72 7465 642d 7769 6c64 6c69 6665 2d72  orted-wildlife-r
+000025b0: 6563 6f67 6e69 7365 7273 2929 0a2a 205b  ecognisers)).* [
+000025c0: 4261 7661 7269 616e 2046 6f72 6573 7420  Bavarian Forest 
+000025d0: 4e61 7469 6f6e 616c 2050 6172 6b5d 2868  National Park](h
+000025e0: 7474 7073 3a2f 2f77 7777 2e6e 6174 696f  ttps://www.natio
+000025f0: 6e61 6c70 6172 6b2d 6261 7965 7269 7363  nalpark-bayerisc
+00002600: 6865 722d 7761 6c64 2e62 6179 6572 6e2e  her-wald.bayern.
+00002610: 6465 2f65 6e67 6c69 7368 2f69 6e64 6578  de/english/index
+00002620: 2e68 746d 2920 285b 7374 6f72 795d 2868  .htm) ([story](h
+00002630: 7474 7073 3a2f 2f63 7573 746f 6d65 7273  ttps://customers
+00002640: 2e6d 6963 726f 736f 6674 2e63 6f6d 2f65  .microsoft.com/e
+00002650: 6e2d 6175 2f73 746f 7279 2f31 3636 3735  n-au/story/16675
+00002660: 3339 3533 3932 3731 3234 3737 3937 2d6e  39539271247797-n
+00002670: 6174 696f 6e61 6c70 6172 6b62 6179 6572  ationalparkbayer
+00002680: 6973 6368 6572 7761 6c64 2d61 7a75 7265  ischerwald-azure
+00002690: 2d65 6e29 290a 2a20 5b45 6e76 6972 6f6e  -en)).* [Environ
+000026a0: 7320 4b69 6d62 6572 6c65 795d 2868 7474  s Kimberley](htt
+000026b0: 7073 3a2f 2f77 7777 2e65 6e76 6972 6f6e  ps://www.environ
+000026c0: 736b 696d 6265 726c 6579 2e6f 7267 2e61  skimberley.org.a
+000026d0: 7529 2028 5b62 6c6f 6720 706f 7374 5d28  u) ([blog post](
+000026e0: 6874 7470 733a 2f2f 7777 772e 656e 7669  https://www.envi
+000026f0: 726f 6e73 6b69 6d62 6572 6c65 792e 6f72  ronskimberley.or
+00002700: 672e 6175 2f61 695f 6d65 6761 6465 7465  g.au/ai_megadete
+00002710: 6374 6f72 2929 0a2a 205b 4665 6c69 6461  ctor)).* [Felida
+00002720: 6520 436f 6e73 6572 7661 7469 6f6e 2046  e Conservation F
+00002730: 756e 645d 2868 7474 7073 3a2f 2f66 656c  und](https://fel
+00002740: 6964 6165 6675 6e64 2e6f 7267 2f29 2028  idaefund.org/) (
+00002750: 5b57 696c 6465 506f 6420 706c 6174 666f  [WildePod platfo
+00002760: 726d 5d28 6874 7470 733a 2f2f 7769 6c64  rm](https://wild
+00002770: 6570 6f64 2e6f 7267 2f29 2920 285b 626c  epod.org/)) ([bl
+00002780: 6f67 2070 6f73 745d 2868 7474 7073 3a2f  og post](https:/
+00002790: 2f61 6268 6179 6b61 7368 7961 702e 636f  /abhaykashyap.co
+000027a0: 6d2f 626c 6f67 2f61 692d 706f 7765 7265  m/blog/ai-powere
+000027b0: 642d 6361 6d65 7261 2d74 7261 702d 696d  d-camera-trap-im
+000027c0: 6167 652d 616e 6e6f 7461 7469 6f6e 2d73  age-annotation-s
+000027d0: 7973 7465 6d2f 2929 0a2a 205b 4973 6c61  ystem/)).* [Isla
+000027e0: 6e64 2043 6f6e 7365 7276 6174 696f 6e5d  nd Conservation]
+000027f0: 2868 7474 7073 3a2f 2f77 7777 2e69 736c  (https://www.isl
+00002800: 616e 6463 6f6e 7365 7276 6174 696f 6e2e  andconservation.
+00002810: 6f72 672f 2920 2862 6c6f 6720 706f 7374  org/) (blog post
+00002820: 7320 5b31 5d28 6874 7470 733a 2f2f 7777  s [1](https://ww
+00002830: 772e 6973 6c61 6e64 636f 6e73 6572 7661  w.islandconserva
+00002840: 7469 6f6e 2e6f 7267 2f63 6f6e 7365 7276  tion.org/conserv
+00002850: 6174 696f 6e2d 6d61 6368 696e 652d 6c65  ation-machine-le
+00002860: 6172 6e69 6e67 2f29 2c5b 325d 2868 7474  arning/),[2](htt
+00002870: 7073 3a2f 2f6e 6577 732e 6c65 6e6f 766f  ps://news.lenovo
+00002880: 2e63 6f6d 2f69 736c 616e 642d 636f 6e73  .com/island-cons
+00002890: 6572 7661 7469 6f6e 2d6d 6163 6869 6e65  ervation-machine
+000028a0: 2d6c 6561 726e 696e 672d 736f 6c75 7469  -learning-soluti
+000028b0: 6f6e 732d 6e76 6964 6961 2d69 736c 616e  ons-nvidia-islan
+000028c0: 642d 6563 6f73 7973 7465 6d73 2f3f 7370  d-ecosystems/?sp
+000028d0: 7269 6e6b 6c72 6964 3d31 3238 3639 3835  rinklrid=1286985
+000028e0: 3738 3234 266c 696e 6b49 643d 3335 3639  7824&linkId=3569
+000028f0: 3531 3931 3929 2920 285b 7669 6465 6f5d  51919)) ([video]
+00002900: 2868 7474 7073 3a2f 2f77 7777 2e6c 656e  (https://www.len
+00002910: 6f76 6f2e 636f 6d2f 636f 6e74 656e 742f  ovo.com/content/
+00002920: 6461 6d2f 6c65 6e6f 766f 2f69 736f 2f63  dam/lenovo/iso/c
+00002930: 7573 746f 6d65 722d 7265 6665 7265 6e63  ustomer-referenc
+00002940: 6573 2d63 6f65 2f6f 6e65 2d6c 656e 6f76  es-coe/one-lenov
+00002950: 6f2d 6375 7374 6f6d 6572 2d73 746f 7269  o-customer-stori
+00002960: 6573 2f77 6668 2f76 6964 656f 732f 5746  es/wfh/videos/WF
+00002970: 482d 4f6e 652d 4c65 6e6f 766f 2d45 4e47  H-One-Lenovo-ENG
+00002980: 2d73 7562 7469 746c 6573 2e6d 7034 2929  -subtitles.mp4))
+00002990: 0a2a 205b 416c 6265 7274 6120 4269 6f64  .* [Alberta Biod
+000029a0: 6976 6572 7369 7479 204d 6f6e 6974 6f72  iversity Monitor
+000029b0: 696e 6720 496e 7374 6974 7574 6520 2841  ing Institute (A
+000029c0: 424d 4929 5d28 6874 7470 733a 2f2f 7777  BMI)](https://ww
+000029d0: 772e 6162 6d69 2e63 612f 686f 6d65 2e68  w.abmi.ca/home.h
+000029e0: 746d 6c29 2028 5b57 696c 6454 7261 7820  tml) ([WildTrax 
+000029f0: 706c 6174 666f 726d 5d28 6874 7470 733a  platform](https:
+00002a00: 2f2f 7777 772e 7769 6c64 7472 6178 2e63  //www.wildtrax.c
+00002a10: 612f 2929 2028 626c 6f67 2070 6f73 7473  a/)) (blog posts
+00002a20: 205b 315d 2868 7474 7073 3a2f 2f77 696c   [1](https://wil
+00002a30: 6463 616d 732e 6361 2f62 6c6f 672f 7468  dcams.ca/blog/th
+00002a40: 652d 6162 6d69 2d76 6973 6974 732d 7468  e-abmi-visits-th
+00002a50: 652d 7a6f 6f2f 292c 5b32 5d28 6874 7470  e-zoo/),[2](http
+00002a60: 3a2f 2f62 6c6f 672e 6162 6d69 2e63 612f  ://blog.abmi.ca/
+00002a70: 3230 3233 2f30 362f 3134 2f6d 616b 696e  2023/06/14/makin
+00002a80: 672d 7769 6c64 7472 6178 2d69 7473 2d6e  g-wildtrax-its-n
+00002a90: 6f74 2d61 2d6b 696e 642d 6f66 2d6d 6167  ot-a-kind-of-mag
+00002aa0: 6963 2d62 6568 696e 642d 7468 652d 7363  ic-behind-the-sc
+00002ab0: 7265 656e 2f29 290a 2a20 5b53 6861 6e20  reen/)).* [Shan 
+00002ac0: 5368 7569 2043 6f6e 7365 7276 6174 696f  Shui Conservatio
+00002ad0: 6e20 4365 6e74 6572 5d28 6874 7470 3a2f  n Center](http:/
+00002ae0: 2f65 6e2e 7368 616e 7368 7569 2e6f 7267  /en.shanshui.org
+00002af0: 2f29 2028 5b62 6c6f 6720 706f 7374 5d28  /) ([blog post](
+00002b00: 6874 7470 733a 2f2f 6d70 2e77 6569 7869  https://mp.weixi
+00002b10: 6e2e 7171 2e63 6f6d 2f73 2f69 4f49 5146  n.qq.com/s/iOIQF
+00002b20: 3363 6b6a 302d 7245 4734 794a 6765 7259  3ckj0-rEG4yJgerY
+00002b30: 773f 6662 636c 6964 3d49 7741 5230 616c  w?fbclid=IwAR0al
+00002b40: 7769 5762 6533 7564 4963 4676 7171 776d  wiWbe3udIcFvqqwm
+00002b50: 3779 3571 6772 3968 5a70 6a72 3837 3146  7y5qgr9hZpjr871F
+00002b60: 5a49 612d 4572 4755 756b 5a37 794a 335a  ZIa-ErGUukZ7yJ3Z
+00002b70: 6867 4365 7673 2929 2028 5b74 7261 6e73  hgCevs)) ([trans
+00002b80: 6c61 7465 6420 626c 6f67 2070 6f73 745d  lated blog post]
+00002b90: 2868 7474 7073 3a2f 2f6d 702d 7765 6978  (https://mp-weix
+00002ba0: 696e 2d71 712d 636f 6d2e 7472 616e 736c  in-qq-com.transl
+00002bb0: 6174 652e 676f 6f67 2f73 2f69 4f49 5146  ate.goog/s/iOIQF
+00002bc0: 3363 6b6a 302d 7245 4734 794a 6765 7259  3ckj0-rEG4yJgerY
+00002bd0: 773f 6662 636c 6964 3d49 7741 5230 616c  w?fbclid=IwAR0al
+00002be0: 7769 5762 6533 7564 4963 4676 7171 776d  wiWbe3udIcFvqqwm
+00002bf0: 3779 3571 6772 3968 5a70 6a72 3837 3146  7y5qgr9hZpjr871F
+00002c00: 5a49 612d 4572 4755 756b 5a37 794a 335a  ZIa-ErGUukZ7yJ3Z
+00002c10: 6867 4365 7673 265f 785f 7472 5f73 6c3d  hgCevs&_x_tr_sl=
+00002c20: 6175 746f 265f 785f 7472 5f74 6c3d 656e  auto&_x_tr_tl=en
+00002c30: 265f 785f 7472 5f68 6c3d 656e 265f 785f  &_x_tr_hl=en&_x_
+00002c40: 7472 5f70 746f 3d77 6170 7029 2920 285b  tr_pto=wapp)) ([
+00002c50: 5765 6220 6465 6d6f 5d28 6874 7470 733a  Web demo](https:
+00002c60: 2f2f 6361 6d65 7261 7472 6170 2d61 692e  //cameratrap-ai.
+00002c70: 6869 6e61 7475 7265 2e63 6e2f 686f 6d65  hinature.cn/home
+00002c80: 2929 0a2a 205b 4972 7669 6e65 2052 616e  )).* [Irvine Ran
+00002c90: 6368 2043 6f6e 7365 7276 616e 6379 5d28  ch Conservancy](
+00002ca0: 6874 7470 3a2f 2f77 7777 2e69 7263 6f6e  http://www.ircon
+00002cb0: 7365 7276 616e 6379 2e6f 7267 2f29 2028  servancy.org/) (
+00002cc0: 5b73 746f 7279 5d28 6874 7470 733a 2f2f  [story](https://
+00002cd0: 7777 772e 6f63 7265 6769 7374 6572 2e63  www.ocregister.c
+00002ce0: 6f6d 2f32 3032 322f 3033 2f33 302f 6169  om/2022/03/30/ai
+00002cf0: 2d73 6f66 7477 6172 652d 6973 2d68 656c  -software-is-hel
+00002d00: 7069 6e67 2d72 6573 6561 7263 6865 7273  ping-researchers
+00002d10: 2d66 6f63 7573 2d6f 6e2d 6c65 6172 6e69  -focus-on-learni
+00002d20: 6e67 2d61 626f 7574 2d6f 6373 2d77 696c  ng-about-ocs-wil
+00002d30: 642d 616e 696d 616c 732f 2929 0a2a 205b  d-animals/)).* [
+00002d40: 5769 6c64 6c69 6665 2050 726f 7465 6374  Wildlife Protect
+00002d50: 696f 6e20 536f 6c75 7469 6f6e 735d 2868  ion Solutions](h
+00002d60: 7474 7073 3a2f 2f77 696c 646c 6966 6570  ttps://wildlifep
+00002d70: 726f 7465 6374 696f 6e73 6f6c 7574 696f  rotectionsolutio
+00002d80: 6e73 2e6f 7267 2f29 2028 5b73 746f 7279  ns.org/) ([story
+00002d90: 5d28 6874 7470 733a 2f2f 6375 7374 6f6d  ](https://custom
+00002da0: 6572 732e 6d69 6372 6f73 6f66 742e 636f  ers.microsoft.co
+00002db0: 6d2f 656e 2d75 732f 7374 6f72 792f 3133  m/en-us/story/13
+00002dc0: 3834 3138 3435 3137 3932 3933 3433 3038  8418451792934308
+00002dd0: 332d 7769 6c64 6c69 6665 2d70 726f 7465  3-wildlife-prote
+00002de0: 6374 696f 6e2d 736f 6c75 7469 6f6e 732d  ction-solutions-
+00002df0: 6e6f 6e70 726f 6669 742d 6169 2d66 6f72  nonprofit-ai-for
+00002e00: 2d65 6172 7468 292c 205b 7374 6f72 795d  -earth), [story]
+00002e10: 2868 7474 7073 3a2f 2f77 7777 2e65 6e74  (https://www.ent
+00002e20: 6572 7072 6973 6561 692e 6e65 7773 2f32  erpriseai.news/2
+00002e30: 3032 332f 3032 2f32 302f 6169 2d68 656c  023/02/20/ai-hel
+00002e40: 7073 2d77 696c 646c 6966 652d 7072 6f74  ps-wildlife-prot
+00002e50: 6563 7469 6f6e 2d73 6f6c 7574 696f 6e73  ection-solutions
+00002e60: 2d73 6166 6567 7561 7264 2d65 6e64 616e  -safeguard-endan
+00002e70: 6765 7265 642d 7370 6563 6965 732f 2929  gered-species/))
+00002e80: 0a2a 205b 5134 325d 2868 7474 7073 3a2f  .* [Q42](https:/
+00002e90: 2f77 7777 2e71 3432 2e6e 6c2f 656e 2920  /www.q42.nl/en) 
+00002ea0: 285b 626c 6f67 2070 6f73 745d 2868 7474  ([blog post](htt
+00002eb0: 7073 3a2f 2f65 6e67 696e 6565 7269 6e67  ps://engineering
+00002ec0: 2e71 3432 2e6e 6c2f 6169 2d62 6561 722d  .q42.nl/ai-bear-
+00002ed0: 7265 7065 6c6c 6572 2f29 290a 2a20 5b41  repeller/)).* [A
+00002ee0: 676f 7574 695d 2868 7474 7073 3a2f 2f61  gouti](https://a
+00002ef0: 676f 7574 692e 6575 2f29 2028 5b72 6570  gouti.eu/) ([rep
+00002f00: 6f72 745d 2868 7474 7073 3a2f 2f65 6673  ort](https://efs
+00002f10: 612e 6f6e 6c69 6e65 6c69 6272 6172 792e  a.onlinelibrary.
+00002f20: 7769 6c65 792e 636f 6d2f 646f 692f 7064  wiley.com/doi/pd
+00002f30: 662f 3130 2e32 3930 332f 7370 2e65 6673  f/10.2903/sp.efs
+00002f40: 612e 3230 3233 2e45 4e2d 3832 3137 2929  a.2023.EN-8217))
+00002f50: 0a2a 205b 5472 6170 7065 725d 2868 7474  .* [Trapper](htt
+00002f60: 7073 3a2f 2f74 7261 7070 6572 2d70 726f  ps://trapper-pro
+00002f70: 6a65 6374 2e72 6561 6474 6865 646f 6373  ject.readthedocs
+00002f80: 2e69 6f2f 656e 2f6c 6174 6573 742f 6f76  .io/en/latest/ov
+00002f90: 6572 7669 6577 2e68 746d 6c29 2028 5b74  erview.html) ([t
+00002fa0: 7574 6f72 6961 6c5d 2868 7474 7073 3a2f  utorial](https:/
+00002fb0: 2f74 7261 7070 6572 2d70 726f 6a65 6374  /trapper-project
+00002fc0: 2e72 6561 6474 6865 646f 6373 2e69 6f2f  .readthedocs.io/
+00002fd0: 656e 2f6c 6174 6573 742f 7475 746f 7269  en/latest/tutori
+00002fe0: 616c 2e68 746d 6c29 290a 0a2a 205b 526f  al.html))..* [Ro
+00002ff0: 6164 2045 636f 6c6f 6779 2043 656e 7465  ad Ecology Cente
+00003000: 725d 2868 7474 7073 3a2f 2f72 6f61 6465  r](https://roade
+00003010: 636f 6c6f 6779 2e75 6364 6176 6973 2e65  cology.ucdavis.e
+00003020: 6475 2f29 2c20 556e 6976 6572 7369 7479  du/), University
+00003030: 206f 6620 4361 6c69 666f 726e 6961 2c20   of California, 
+00003040: 4461 7669 7320 285b 5769 6c64 6c69 6665  Davis ([Wildlife
+00003050: 204f 6273 6572 7665 7220 4e65 7477 6f72   Observer Networ
+00003060: 6b20 706c 6174 666f 726d 5d28 6874 7470  k platform](http
+00003070: 733a 2f2f 7769 6c64 6c69 6665 6f62 7365  s://wildlifeobse
+00003080: 7276 6572 2e6e 6574 2f29 290a 2a20 5b54  rver.net/)).* [T
+00003090: 6865 204e 6174 7572 6520 436f 6e73 6572  he Nature Conser
+000030a0: 7661 6e63 7920 696e 2043 616c 6966 6f72  vancy in Califor
+000030b0: 6e69 615d 2868 7474 7073 3a2f 2f77 7777  nia](https://www
+000030c0: 2e6e 6174 7572 652e 6f72 672f 656e 2d75  .nature.org/en-u
+000030d0: 732f 6162 6f75 742d 7573 2f77 6865 7265  s/about-us/where
+000030e0: 2d77 652d 776f 726b 2f75 6e69 7465 642d  -we-work/united-
+000030f0: 7374 6174 6573 2f63 616c 6966 6f72 6e69  states/californi
+00003100: 612f 2920 285b 416e 696d 6c20 706c 6174  a/) ([Animl plat
+00003110: 666f 726d 5d28 6874 7470 733a 2f2f 6769  form](https://gi
+00003120: 7468 7562 2e63 6f6d 2f74 6e63 2d63 612d  thub.com/tnc-ca-
+00003130: 6765 6f2f 616e 696d 6c2d 6672 6f6e 7465  geo/animl-fronte
+00003140: 6e64 2929 2028 5b73 746f 7279 5d28 6874  nd)) ([story](ht
+00003150: 7470 733a 2f2f 7777 772e 7669 7369 6f6e  tps://www.vision
+00003160: 2d73 7973 7465 6d73 2e63 6f6d 2f6e 6f6e  -systems.com/non
+00003170: 2d66 6163 746f 7279 2f65 6e76 6972 6f6e  -factory/environ
+00003180: 6d65 6e74 2d61 6772 6963 756c 7475 7265  ment-agriculture
+00003190: 2f61 7274 6963 6c65 2f31 3433 3034 3433  /article/1430443
+000031a0: 332f 7468 652d 6e61 7475 7265 2d63 6f6e  3/the-nature-con
+000031b0: 7365 7276 616e 6379 2d62 7269 6e67 732d  servancy-brings-
+000031c0: 6361 6d65 7261 732d 6169 2d74 6f2d 696e  cameras-ai-to-in
+000031d0: 7661 7369 7665 2d73 7065 6369 6573 2d70  vasive-species-p
+000031e0: 7265 7665 6e74 696f 6e29 290a 2a20 5b53  revention)).* [S
+000031f0: 616e 2044 6965 676f 205a 6f6f 2057 696c  an Diego Zoo Wil
+00003200: 646c 6966 6520 416c 6c69 616e 6365 5d28  dlife Alliance](
+00003210: 6874 7470 733a 2f2f 7363 6965 6e63 652e  https://science.
+00003220: 7361 6e64 6965 676f 7a6f 6f2e 6f72 672f  sandiegozoo.org/
+00003230: 2920 2028 5b41 6e69 6d6c 2052 2070 6163  )  ([Animl R pac
+00003240: 6b61 6765 5d28 6874 7470 733a 2f2f 6769  kage](https://gi
+00003250: 7468 7562 2e63 6f6d 2f63 6f6e 7365 7276  thub.com/conserv
+00003260: 6174 696f 6e74 6563 686c 6162 2f61 6e69  ationtechlab/ani
+00003270: 6d6c 2929 0a2a 205b 5465 7272 4fc3 af6b  ml)).* [TerrO..k
+00003280: 6f5d 2868 7474 7073 3a2f 2f77 7777 2e74  o](https://www.t
+00003290: 6572 726f 696b 6f2e 6672 2f29 2028 5b4f  erroiko.fr/) ([O
+000032a0: 4341 5049 2070 6c61 7466 6f72 6d5d 2868  CAPI platform](h
+000032b0: 7474 7073 3a2f 2f77 7777 2e74 6572 726f  ttps://www.terro
+000032c0: 696b 6f2e 6672 2f6f 6361 7069 2929 0a0a  iko.fr/ocapi))..
+000032d0: 416c 736f 2073 6565 3a0a 0a2a 2054 6865  Also see:..* The
+000032e0: 205b 6c69 7374 206f 6620 4d44 2d72 656c   [list of MD-rel
+000032f0: 6174 6564 2047 5549 732c 2070 6c61 7466  ated GUIs, platf
+00003300: 6f72 6d73 2c20 616e 6420 4769 7448 7562  orms, and GitHub
+00003310: 2072 6570 6f73 5d28 6874 7470 733a 2f2f   repos](https://
+00003320: 6769 7468 7562 2e63 6f6d 2f61 6765 6e74  github.com/agent
+00003330: 6d6f 7272 6973 2f4d 6567 6144 6574 6563  morris/MegaDetec
+00003340: 746f 722f 626c 6f62 2f6d 6169 6e2f 6d65  tor/blob/main/me
+00003350: 6761 6465 7465 6374 6f72 2e6d 6423 6973  gadetector.md#is
+00003360: 2d74 6865 7265 2d61 2d67 7569 2920 7769  -there-a-gui) wi
+00003370: 7468 696e 2074 6865 204d 6567 6144 6574  thin the MegaDet
+00003380: 6563 746f 7220 5573 6572 2047 7569 6465  ector User Guide
+00003390: 0a0a 2a20 5b50 6574 6572 2773 206d 6170  ..* [Peter's map
+000033a0: 206f 6620 4563 6f41 7373 6973 7420 7573   of EcoAssist us
+000033b0: 6572 735d 2868 7474 7073 3a2f 2f61 6464  ers](https://add
+000033c0: 6178 6461 7461 7363 6965 6e63 652e 636f  axdatascience.co
+000033d0: 6d2f 6563 6f61 7373 6973 7429 2028 7768  m/ecoassist) (wh
+000033e0: 6f20 6172 6520 616c 736f 204d 6567 6144  o are also MegaD
+000033f0: 6574 6563 746f 7220 7573 6572 7321 290a  etector users!).
+00003400: 0a2a 2054 6865 206c 6973 7420 6f66 2070  .* The list of p
+00003410: 6170 6572 7320 7461 6767 6564 2022 4d65  apers tagged "Me
+00003420: 6761 4465 7465 6374 6f72 2220 6f6e 206f  gaDetector" on o
+00003430: 7572 205b 6c69 7374 206f 6620 7061 7065  ur [list of pape
+00003440: 7273 2061 626f 7574 204d 4c20 616e 6420  rs about ML and 
+00003450: 6361 6d65 7261 2074 7261 7073 5d28 6874  camera traps](ht
+00003460: 7470 733a 2f2f 6167 656e 746d 6f72 7269  tps://agentmorri
+00003470: 732e 6769 7468 7562 2e69 6f2f 6361 6d65  s.github.io/came
+00003480: 7261 2d74 7261 702d 6d6c 2d73 7572 7665  ra-trap-ml-surve
+00003490: 792f 2363 616d 6572 612d 7472 6170 2d6d  y/#camera-trap-m
+000034a0: 6c2d 7061 7065 7273 290a 0a0a 2323 2052  l-papers)...## R
+000034b0: 6570 6f20 636f 6e74 656e 7473 0a0a 5468  epo contents..Th
+000034c0: 6973 2072 6570 6f20 6973 206f 7267 616e  is repo is organ
+000034d0: 697a 6564 2069 6e74 6f20 7468 6520 666f  ized into the fo
+000034e0: 6c6c 6f77 696e 6720 666f 6c64 6572 732e  llowing folders.
+000034f0: 2e2e 0a0a 5468 6973 2072 6570 6f20 636f  ....This repo co
+00003500: 6e74 6169 6e73 2074 6865 2074 6f6f 6c73  ntains the tools
+00003510: 2066 6f72 2074 7261 696e 696e 6720 616e   for training an
+00003520: 6420 7275 6e6e 696e 6720 5b4d 6567 6144  d running [MegaD
+00003530: 6574 6563 746f 725d 286d 6567 6164 6574  etector](megadet
+00003540: 6563 746f 722e 6d64 292c 2061 6e20 6f62  ector.md), an ob
+00003550: 6a65 6374 2064 6574 6563 7469 6f6e 206d  ject detection m
+00003560: 6f64 656c 2074 6861 7420 646f 6573 2061  odel that does a
+00003570: 2070 7265 7474 7920 676f 6f64 206a 6f62   pretty good job
+00003580: 2066 696e 6469 6e67 2061 6e69 6d61 6c73   finding animals
+00003590: 2c20 7065 6f70 6c65 2c20 616e 6420 7665  , people, and ve
+000035a0: 6869 636c 6573 2028 616e 6420 7468 6572  hicles (and ther
+000035b0: 6566 6f72 6520 6973 2070 7265 7474 7920  efore is pretty 
+000035c0: 676f 6f64 2061 7420 6669 6e64 696e 6720  good at finding 
+000035d0: 656d 7074 7920 696d 6167 6573 2920 696e  empty images) in
+000035e0: 2063 616d 6572 6120 7472 6170 2069 6d61   camera trap ima
+000035f0: 6765 7320 696e 2061 2076 6172 6965 7479  ges in a variety
+00003600: 206f 6620 7465 7272 6573 7472 6961 6c20   of terrestrial 
+00003610: 6563 6f73 7973 7465 6d73 2e0a 0a54 6865  ecosystems...The
+00003620: 2063 6f72 6520 6675 6e63 7469 6f6e 616c   core functional
+00003630: 6974 7920 7072 6f76 6964 6564 2069 733a  ity provided is:
+00003640: 0a0a 2d20 5472 6169 6e69 6e67 2061 6e64  ..- Training and
+00003650: 2072 756e 6e69 6e67 205b 4d65 6761 4465   running [MegaDe
+00003660: 7465 6374 6f72 5d28 6d65 6761 6465 7465  tector](megadete
+00003670: 6374 6f72 2e6d 6429 2e0a 2d20 5472 6169  ctor.md)..- Trai
+00003680: 6e69 6e67 2061 6e64 2072 756e 6e69 6e67  ning and running
+00003690: 2073 6f6d 6520 5b73 7065 6369 6573 2063   some [species c
+000036a0: 6c61 7373 6966 6965 7273 5d28 636c 6173  lassifiers](clas
+000036b0: 7369 6669 6361 7469 6f6e 2920 7468 6174  sification) that
+000036c0: 2061 7265 2075 7365 6420 696e 2063 6f6e   are used in con
+000036d0: 6a75 6e63 7469 6f6e 2077 6974 6820 4d65  junction with Me
+000036e0: 6761 4465 7465 6374 6f72 2e0a 2d20 546f  gaDetector..- To
+000036f0: 6f6c 7320 746f 205b 636f 6e76 6572 745d  ols to [convert]
+00003700: 2864 6174 615f 6d61 6e61 6765 6d65 6e74  (data_management
+00003710: 2920 6672 6571 7565 6e74 6c79 2d75 7365  ) frequently-use
+00003720: 6420 6361 6d65 7261 2074 7261 7020 6d65  d camera trap me
+00003730: 7461 6461 7461 2066 6f72 6d61 7473 2069  tadata formats i
+00003740: 6e74 6f20 6120 636f 6d6d 6f6e 2066 6f72  nto a common for
+00003750: 6d61 742e 0a2d 2041 205b 6261 7463 6820  mat..- A [batch 
+00003760: 7072 6f63 6573 7369 6e67 2041 5049 5d28  processing API](
+00003770: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00003780: 6f6d 2f61 6765 6e74 6d6f 7272 6973 2f4d  om/agentmorris/M
+00003790: 6567 6144 6574 6563 746f 722f 7472 6565  egaDetector/tree
+000037a0: 2f6d 6169 6e2f 6170 692f 6261 7463 685f  /main/api/batch_
+000037b0: 7072 6f63 6573 7369 6e67 2920 7468 6174  processing) that
+000037c0: 2072 756e 7320 4d65 6761 4465 7465 6374   runs MegaDetect
+000037d0: 6f72 206f 6e20 6c61 7267 6520 696d 6167  or on large imag
+000037e0: 6520 636f 6c6c 6563 7469 6f6e 732c 2074  e collections, t
+000037f0: 6f20 6163 6365 6c65 7261 7465 2070 6f70  o accelerate pop
+00003800: 756c 6174 696f 6e20 7375 7276 6579 732e  ulation surveys.
+00003810: 0a2d 2041 205b 7265 616c 2d74 696d 6520  .- A [real-time 
+00003820: 4150 495d 2868 7474 7073 3a2f 2f67 6974  API](https://git
+00003830: 6875 622e 636f 6d2f 6167 656e 746d 6f72  hub.com/agentmor
+00003840: 7269 732f 4d65 6761 4465 7465 6374 6f72  ris/MegaDetector
+00003850: 2f74 7265 652f 6d61 696e 2f61 7069 2f73  /tree/main/api/s
+00003860: 796e 6368 726f 6e6f 7573 2920 7468 6174  ynchronous) that
+00003870: 2072 756e 7320 4d65 6761 4465 7465 6374   runs MegaDetect
+00003880: 6f72 2028 616e 6420 736f 6d65 2073 7065  or (and some spe
+00003890: 6369 6573 2063 6c61 7373 6966 6965 7273  cies classifiers
+000038a0: 2920 7379 6e63 6872 6f6e 6f75 736c 792c  ) synchronously,
+000038b0: 2070 7269 6d61 7269 6c79 2074 6f20 7375   primarily to su
+000038c0: 7070 6f72 7420 6269 6f73 6563 7572 6974  pport biosecurit
+000038d0: 7920 6170 706c 6963 6174 696f 6e73 2e0a  y applications..
+000038e0: 0a54 6869 7320 7265 706f 2064 6f65 7320  .This repo does 
+000038f0: 6e6f 7420 686f 7374 2074 6865 2064 6174  not host the dat
+00003900: 6120 7573 6564 2074 6f20 7472 6169 6e20  a used to train 
+00003910: 4d65 6761 4465 7465 6374 6f72 2c20 6275  MegaDetector, bu
+00003920: 7420 7765 2077 6f72 6b20 7769 7468 206f  t we work with o
+00003930: 7572 2063 6f6c 6c61 626f 7261 746f 7273  ur collaborators
+00003940: 2074 6f20 6d61 6b65 2064 6174 6120 616e   to make data an
+00003950: 6420 616e 6e6f 7461 7469 6f6e 7320 6176  d annotations av
+00003960: 6169 6c61 626c 6520 7768 656e 6576 6572  ailable whenever
+00003970: 2070 6f73 7369 626c 6520 6f6e 205b 6c69   possible on [li
+00003980: 6c61 2e73 6369 656e 6365 5d28 6874 7470  la.science](http
+00003990: 3a2f 2f6c 696c 612e 7363 6965 6e63 6529  ://lila.science)
+000039a0: 2e20 2053 6565 2074 6865 205b 4d65 6761  .  See the [Mega
+000039b0: 4465 7465 6374 6f72 2074 7261 696e 696e  Detector trainin
+000039c0: 6720 6461 7461 5d28 6d65 6761 6465 7465  g data](megadete
+000039d0: 6374 6f72 2e6d 6423 6361 6e2d 796f 752d  ctor.md#can-you-
+000039e0: 7368 6172 652d 7468 652d 7472 6169 6e69  share-the-traini
+000039f0: 6e67 2d64 6174 6129 2073 6563 7469 6f6e  ng-data) section
+00003a00: 2074 6f20 6c65 6172 6e20 6d6f 7265 2061   to learn more a
+00003a10: 626f 7574 2074 6865 2064 6174 6120 7573  bout the data us
+00003a20: 6564 2074 6f20 7472 6169 6e20 4d65 6761  ed to train Mega
+00003a30: 4465 7465 6374 6f72 2e0a 0a4d 6567 6144  Detector...MegaD
+00003a40: 6574 6563 746f 7220 7761 7320 696e 6974  etector was init
+00003a50: 6961 6c6c 7920 6465 7665 6c6f 7065 6420  ially developed 
+00003a60: 6279 2074 6865 205b 4d69 6372 6f73 6f66  by the [Microsof
+00003a70: 7420 4149 2066 6f72 2045 6172 7468 2070  t AI for Earth p
+00003a80: 726f 6772 616d 5d28 6874 7470 733a 2f2f  rogram](https://
+00003a90: 7777 772e 6d69 6372 6f73 6f66 742e 636f  www.microsoft.co
+00003aa0: 6d2f 656e 2d75 732f 6169 2f61 692d 666f  m/en-us/ai/ai-fo
+00003ab0: 722d 6561 7274 6829 3b20 7468 6973 2072  r-earth); this r
+00003ac0: 6570 6f20 7761 7320 666f 726b 6564 2066  epo was forked f
+00003ad0: 726f 6d20 7468 6520 6d69 6372 6f73 6f66  rom the microsof
+00003ae0: 742f 6361 6d65 7261 7472 6170 7320 7265  t/cameratraps re
+00003af0: 706f 2061 6e64 2069 7320 6d61 696e 7461  po and is mainta
+00003b00: 696e 6564 2062 7920 7468 6520 6f72 6967  ined by the orig
+00003b10: 696e 616c 204d 6567 6144 6574 6563 746f  inal MegaDetecto
+00003b20: 7220 6465 7665 6c6f 7065 7273 2028 7768  r developers (wh
+00003b30: 6f20 6172 6520 6e6f 206c 6f6e 6765 7220  o are no longer 
+00003b40: 6174 204d 6963 726f 736f 6674 2c20 6275  at Microsoft, bu
+00003b50: 7420 6172 6520 6162 736f 6c75 7465 6c79  t are absolutely
+00003b60: 2066 616e 7461 7374 6963 616c 6c79 2065   fantastically e
+00003b70: 7465 726e 616c 6c79 2067 7261 7465 6675  ternally gratefu
+00003b80: 6c20 746f 204d 6963 726f 736f 6674 2066  l to Microsoft f
+00003b90: 6f72 2074 6865 2069 6e76 6573 746d 656e  or the investmen
+00003ba0: 7420 616e 6420 636f 6d6d 6974 6d65 6e74  t and commitment
+00003bb0: 2074 6861 7420 6d61 6465 204d 6567 6144   that made MegaD
+00003bc0: 6574 6563 746f 7220 6861 7070 656e 292e  etector happen).
+00003bd0: 0a0a 0a23 2323 2061 7069 0a0a 436f 6465  ...### api..Code
+00003be0: 2066 6f72 2068 6f73 7469 6e67 206f 7572   for hosting our
+00003bf0: 206d 6f64 656c 7320 6173 2061 6e20 4150   models as an AP
+00003c00: 492c 2065 6974 6865 7220 666f 7220 7379  I, either for sy
+00003c10: 6e63 6872 6f6e 6f75 7320 6f70 6572 6174  nchronous operat
+00003c20: 696f 6e20 2869 2e65 2e2c 2066 6f72 2072  ion (i.e., for r
+00003c30: 6561 6c2d 7469 6d65 2069 6e66 6572 656e  eal-time inferen
+00003c40: 6365 2920 6f72 2061 7320 6120 6261 7463  ce) or as a batc
+00003c50: 6820 7072 6f63 6573 7320 2866 6f72 206c  h process (for l
+00003c60: 6172 6765 2062 696f 6469 7665 7273 6974  arge biodiversit
+00003c70: 7920 7375 7276 6579 7329 2e20 2043 6f6d  y surveys).  Com
+00003c80: 6d6f 6e20 6f70 6572 6174 696f 6e73 206f  mon operations o
+00003c90: 6e65 206d 6967 6874 2064 6f20 6166 7465  ne might do afte
+00003ca0: 7220 7275 6e6e 696e 6720 4d65 6761 4465  r running MegaDe
+00003cb0: 7465 6374 6f72 2026 6e64 6173 683b 2065  tector &ndash; e
+00003cc0: 2e67 2e20 5b67 656e 6572 6174 696e 6720  .g. [generating 
+00003cd0: 7072 6576 6965 7720 7061 6765 7320 746f  preview pages to
+00003ce0: 2073 756d 6d61 7269 7a65 2079 6f75 7220   summarize your 
+00003cf0: 7265 7375 6c74 735d 2868 7474 7073 3a2f  results](https:/
+00003d00: 2f67 6974 6875 622e 636f 6d2f 6167 656e  /github.com/agen
+00003d10: 746d 6f72 7269 732f 4d65 6761 4465 7465  tmorris/MegaDete
+00003d20: 6374 6f72 2f62 6c6f 622f 6d61 696e 2f61  ctor/blob/main/a
+00003d30: 7069 2f62 6174 6368 5f70 726f 6365 7373  pi/batch_process
+00003d40: 696e 672f 706f 7374 7072 6f63 6573 7369  ing/postprocessi
+00003d50: 6e67 2f70 6f73 7470 726f 6365 7373 5f62  ng/postprocess_b
+00003d60: 6174 6368 5f72 6573 756c 7473 2e70 7929  atch_results.py)
+00003d70: 2c20 5b73 6570 6172 6174 696e 6720 696d  , [separating im
+00003d80: 6167 6573 2069 6e74 6f20 6469 6666 6572  ages into differ
+00003d90: 656e 7420 666f 6c64 6572 7320 6261 7365  ent folders base
+00003da0: 6420 6f6e 2041 4920 7265 7375 6c74 735d  d on AI results]
+00003db0: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+00003dc0: 636f 6d2f 6167 656e 746d 6f72 7269 732f  com/agentmorris/
+00003dd0: 4d65 6761 4465 7465 6374 6f72 2f62 6c6f  MegaDetector/blo
+00003de0: 622f 6d61 696e 2f61 7069 2f62 6174 6368  b/main/api/batch
+00003df0: 5f70 726f 6365 7373 696e 672f 706f 7374  _processing/post
+00003e00: 7072 6f63 6573 7369 6e67 2f73 6570 6172  processing/separ
+00003e10: 6174 655f 6465 7465 6374 696f 6e73 5f69  ate_detections_i
+00003e20: 6e74 6f5f 666f 6c64 6572 732e 7079 292c  nto_folders.py),
+00003e30: 206f 7220 5b63 6f6e 7665 7274 696e 6720   or [converting 
+00003e40: 7265 7375 6c74 7320 746f 2061 2064 6966  results to a dif
+00003e50: 6665 7265 6e74 2066 6f72 6d61 745d 2868  ferent format](h
+00003e60: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00003e70: 6d2f 6167 656e 746d 6f72 7269 732f 4d65  m/agentmorris/Me
+00003e80: 6761 4465 7465 6374 6f72 2f62 6c6f 622f  gaDetector/blob/
+00003e90: 6d61 696e 2f61 7069 2f62 6174 6368 5f70  main/api/batch_p
+00003ea0: 726f 6365 7373 696e 672f 706f 7374 7072  rocessing/postpr
+00003eb0: 6f63 6573 7369 6e67 2f63 6f6e 7665 7274  ocessing/convert
+00003ec0: 5f6f 7574 7075 745f 666f 726d 6174 2e70  _output_format.p
+00003ed0: 7929 2026 6e64 6173 683b 2061 6c73 6f20  y) &ndash; also 
+00003ee0: 6c69 7665 2069 6e20 7468 6973 2066 6f6c  live in this fol
+00003ef0: 6465 722c 2077 6974 6869 6e20 7468 6520  der, within the 
+00003f00: 5b61 7069 2f62 6174 6368 5f70 726f 6365  [api/batch_proce
+00003f10: 7373 696e 672f 706f 7374 7072 6f63 6573  ssing/postproces
+00003f20: 7369 6e67 5d28 6874 7470 733a 2f2f 6769  sing](https://gi
+00003f30: 7468 7562 2e63 6f6d 2f61 6765 6e74 6d6f  thub.com/agentmo
+00003f40: 7272 6973 2f4d 6567 6144 6574 6563 746f  rris/MegaDetecto
+00003f50: 722f 7472 6565 2f6d 6169 6e2f 6170 692f  r/tree/main/api/
+00003f60: 6261 7463 685f 7072 6f63 6573 7369 6e67  batch_processing
+00003f70: 2f70 6f73 7470 726f 6365 7373 696e 6729  /postprocessing)
+00003f80: 2066 6f6c 6465 722e 0a0a 0a23 2323 2061   folder....### a
+00003f90: 7263 6869 7665 0a0a 4f6c 6420 636f 6465  rchive..Old code
+00003fa0: 2074 6861 7420 7765 2064 6964 6e27 7420   that we didn't 
+00003fb0: 3c69 3e71 7569 7465 3c2f 693e 2077 616e  <i>quite</i> wan
+00003fc0: 7420 746f 2064 656c 6574 652c 2062 7574  t to delete, but
+00003fd0: 2069 7320 6261 7369 6361 6c6c 7920 6f62   is basically ob
+00003fe0: 736f 6c65 7465 2e0a 0a0a 2323 2320 636c  solete....### cl
+00003ff0: 6173 7369 6669 6361 7469 6f6e 0a0a 4578  assification..Ex
+00004000: 7065 7269 6d65 6e74 616c 2063 6f64 6520  perimental code 
+00004010: 666f 7220 7472 6169 6e69 6e67 2073 7065  for training spe
+00004020: 6369 6573 2063 6c61 7373 6966 6965 7273  cies classifiers
+00004030: 206f 6e20 6e65 7720 6461 7461 2073 6574   on new data set
+00004040: 732c 2067 656e 6572 616c 6c79 2074 7261  s, generally tra
+00004050: 696e 6564 206f 6e20 4d65 6761 4465 7465  ined on MegaDete
+00004060: 6374 6f72 2063 726f 7073 2e20 2043 7572  ctor crops.  Cur
+00004070: 7265 6e74 6c79 2074 6865 206d 6169 6e20  rently the main 
+00004080: 7069 7065 6c69 6e65 2064 6573 6372 6962  pipeline describ
+00004090: 6564 2069 6e20 7468 6973 2066 6f6c 6465  ed in this folde
+000040a0: 7220 7265 6c69 6573 206f 6e20 6120 6c61  r relies on a la
+000040b0: 7267 6520 6461 7461 6261 7365 206f 6620  rge database of 
+000040c0: 6c61 6265 6c65 6420 696d 6167 6573 2074  labeled images t
+000040d0: 6861 7420 6973 206e 6f74 2070 7562 6c69  hat is not publi
+000040e0: 636c 7920 6176 6169 6c61 626c 653b 2074  cly available; t
+000040f0: 6865 7265 666f 7265 2c20 7468 6973 2066  herefore, this f
+00004100: 6f6c 6465 7220 6973 206e 6f74 2079 6574  older is not yet
+00004110: 2073 6574 2075 7020 746f 2066 6163 696c   set up to facil
+00004120: 6974 6174 6520 7472 6169 6e69 6e67 206f  itate training o
+00004130: 6620 796f 7572 206f 776e 2063 6c61 7373  f your own class
+00004140: 6966 6965 7273 2e20 2048 6f77 6576 6572  ifiers.  However
+00004150: 2c20 6974 2069 7320 7573 6566 756c 2066  , it is useful f
+00004160: 6f72 203c 693e 7573 6572 733c 2f69 3e20  or <i>users</i> 
+00004170: 6f66 2074 6865 2063 6c61 7373 6966 6965  of the classifie
+00004180: 7273 2074 6861 7420 7765 2074 7261 696e  rs that we train
+00004190: 2c20 616e 6420 636f 6e74 6169 6e73 2073  , and contains s
+000041a0: 6f6d 6520 7573 6566 756c 2073 7461 7274  ome useful start
+000041b0: 696e 6720 706f 696e 7473 2069 6620 796f  ing points if yo
+000041c0: 7520 6172 6520 676f 696e 6720 746f 2074  u are going to t
+000041d0: 616b 6520 6120 2244 4959 2220 6170 7072  ake a "DIY" appr
+000041e0: 6f61 6368 2074 6f20 7472 6169 6e69 6e67  oach to training
+000041f0: 2063 6c61 7373 6966 6965 7273 206f 6e20   classifiers on 
+00004200: 6372 6f70 7065 6420 696d 6167 6573 2e20  cropped images. 
+00004210: 200a 0a41 6c6c 2074 6861 7420 7361 6964   ..All that said
+00004220: 2c20 6865 7265 2773 2061 6e6f 7468 6572  , here's another
+00004230: 2022 7465 6173 6572 2069 6d61 6765 2220   "teaser image" 
+00004240: 6f66 2077 6861 7420 796f 7520 6765 7420  of what you get 
+00004250: 6174 2074 6865 2065 6e64 206f 6620 7472  at the end of tr
+00004260: 6169 6e69 6e67 2061 6e64 2072 756e 6e69  aining and runni
+00004270: 6e67 2061 2063 6c61 7373 6966 6965 723a  ng a classifier:
+00004280: 0a0a 3c69 6d67 2073 7263 3d22 696d 6167  ..<img src="imag
+00004290: 6573 2f77 6172 7468 6f67 5f63 6c61 7373  es/warthog_class
+000042a0: 6966 6963 6174 696f 6e73 2e6a 7067 2220  ifications.jpg" 
+000042b0: 7769 6474 683d 2237 3030 223e 3c62 722f  width="700"><br/
+000042c0: 3e49 6d61 6765 2063 7265 6469 7420 556e  >Image credit Un
+000042d0: 6976 6572 7369 7479 206f 6620 4d69 6e6e  iversity of Minn
+000042e0: 6573 6f74 612c 2066 726f 6d20 7468 6520  esota, from the 
+000042f0: 536e 6170 7368 6f74 2053 6166 6172 6920  Snapshot Safari 
+00004300: 7072 6f67 7261 6d2e 0a0a 0a23 2323 2064  program....### d
+00004310: 6174 615f 6d61 6e61 6765 6d65 6e74 0a0a  ata_management..
+00004320: 436f 6465 2066 6f72 3a0a 0a2a 2043 6f6e  Code for:..* Con
+00004330: 7665 7274 696e 6720 6672 6571 7565 6e74  verting frequent
+00004340: 6c79 2d75 7365 6420 6d65 7461 6461 7461  ly-used metadata
+00004350: 2066 6f72 6d61 7473 2074 6f20 5b43 4f43   formats to [COC
+00004360: 4f20 4361 6d65 7261 2054 7261 7073 5d28  O Camera Traps](
+00004370: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00004380: 6f6d 2f61 6765 6e74 6d6f 7272 6973 2f4d  om/agentmorris/M
+00004390: 6567 6144 6574 6563 746f 722f 626c 6f62  egaDetector/blob
+000043a0: 2f6d 6169 6e2f 6461 7461 5f6d 616e 6167  /main/data_manag
+000043b0: 656d 656e 742f 5245 4144 4d45 2e6d 6423  ement/README.md#
+000043c0: 636f 636f 2d63 616d 6572 6174 7261 7073  coco-cameratraps
+000043d0: 2d66 6f72 6d61 7429 2066 6f72 6d61 740a  -format) format.
+000043e0: 2a20 436f 6e76 6572 7469 6e67 2074 6865  * Converting the
+000043f0: 206f 7574 7075 7420 6f66 2041 4920 6d6f   output of AI mo
+00004400: 6465 6c73 2028 6573 7065 6369 616c 6c79  dels (especially
+00004410: 205b 594f 4c4f 7635 5d28 6874 7470 733a   [YOLOv5](https:
+00004420: 2f2f 6769 7468 7562 2e63 6f6d 2f61 6765  //github.com/age
+00004430: 6e74 6d6f 7272 6973 2f4d 6567 6144 6574  ntmorris/MegaDet
+00004440: 6563 746f 722f 626c 6f62 2f6d 6169 6e2f  ector/blob/main/
+00004450: 6170 692f 6261 7463 685f 7072 6f63 6573  api/batch_proces
+00004460: 7369 6e67 2f70 6f73 7470 726f 6365 7373  sing/postprocess
+00004470: 696e 672f 636f 6e76 6572 745f 6f75 7470  ing/convert_outp
+00004480: 7574 5f66 6f72 6d61 742e 7079 2929 2074  ut_format.py)) t
+00004490: 6f20 7468 6520 666f 726d 6174 2075 7365  o the format use
+000044a0: 6420 666f 7220 4149 2072 6573 756c 7473  d for AI results
+000044b0: 2074 6872 6f75 6768 6f75 7420 7468 6973   throughout this
+000044c0: 2072 6570 6f0a 2a20 4372 6561 7469 6e67   repo.* Creating
+000044d0: 2c20 7669 7375 616c 697a 696e 672c 2061  , visualizing, a
+000044e0: 6e64 2020 6564 6974 696e 6720 434f 434f  nd  editing COCO
+000044f0: 2043 616d 6572 6120 5472 6170 7320 2e6a   Camera Traps .j
+00004500: 736f 6e20 6461 7461 6261 7365 730a 0a0a  son databases...
+00004510: 2323 2320 6465 7465 6374 696f 6e0a 0a43  ### detection..C
+00004520: 6f64 6520 666f 7220 7472 6169 6e69 6e67  ode for training
+00004530: 2c20 7275 6e6e 696e 672c 2061 6e64 2065  , running, and e
+00004540: 7661 6c75 6174 696e 6720 4d65 6761 4465  valuating MegaDe
+00004550: 7465 6374 6f72 2e0a 0a0a 2323 2320 656e  tector....### en
+00004560: 7673 0a0a 456e 7669 726f 6e6d 656e 7420  vs..Environment 
+00004570: 6669 6c65 732e 2e2e 2073 7065 6369 6669  files... specifi
+00004580: 6361 6c6c 7920 2e79 6d6c 2066 696c 6573  cally .yml files
+00004590: 2066 6f72 206d 616d 6261 2f63 6f6e 6461   for mamba/conda
+000045a0: 2065 6e76 6972 6f6e 6d65 6e74 7320 2874   environments (t
+000045b0: 6865 7365 2061 7265 2077 6861 7420 7765  hese are what we
+000045c0: 2072 6563 6f6d 6d65 6e64 2069 6e20 6f75   recommend in ou
+000045d0: 7220 5b4d 6567 6144 6574 6563 746f 7220  r [MegaDetector 
+000045e0: 5573 6572 2047 7569 6465 5d28 6d65 6761  User Guide](mega
+000045f0: 6465 7465 6374 6f72 2e6d 6429 292c 2061  detector.md)), a
+00004600: 6e64 2061 2072 6571 7569 7265 6d65 6e74  nd a requirement
+00004610: 732e 7478 7420 666f 7220 7468 6520 7069  s.txt for the pi
+00004620: 702d 696e 636c 696e 6564 2e0a 0a0a 2323  p-inclined....##
+00004630: 2320 696d 6167 6573 0a0a 4d65 6469 6120  # images..Media 
+00004640: 7573 6564 2069 6e20 646f 6375 6d65 6e74  used in document
+00004650: 6174 696f 6e2e 0a0a 0a23 2323 206d 645f  ation....### md_
+00004660: 7574 696c 730a 0a53 6d61 6c6c 2075 7469  utils..Small uti
+00004670: 6c69 7479 2066 756e 6374 696f 6e73 2066  lity functions f
+00004680: 6f72 2073 7472 696e 6720 6d61 6e69 7075  or string manipu
+00004690: 6c61 7469 6f6e 2c20 6669 6c65 6e61 6d65  lation, filename
+000046a0: 206d 616e 6970 756c 6174 696f 6e2c 2064   manipulation, d
+000046b0: 6f77 6e6c 6f61 6469 6e67 2066 696c 6573  ownloading files
+000046c0: 2066 726f 6d20 5552 4c73 2c20 6574 632e   from URLs, etc.
+000046d0: 2020 4d6f 7374 6c79 2061 6461 7074 6564    Mostly adapted
+000046e0: 2066 726f 6d20 7468 6520 5b61 6934 6575   from the [ai4eu
+000046f0: 7469 6c73 5d28 6874 7470 733a 2f2f 6769  tils](https://gi
+00004700: 7468 7562 2e63 6f6d 2f6d 6963 726f 736f  thub.com/microso
+00004710: 6674 2f61 6934 6575 7469 6c73 2920 7265  ft/ai4eutils) re
+00004720: 706f 2e0a 0a0a 2323 2320 6d64 5f76 6973  po....### md_vis
+00004730: 7561 6c69 7a61 7469 6f6e 0a0a 5368 6172  ualization..Shar
+00004740: 6564 2074 6f6f 6c73 2066 6f72 2076 6973  ed tools for vis
+00004750: 7561 6c69 7a69 6e67 2069 6d61 6765 7320  ualizing images 
+00004760: 7769 7468 2067 726f 756e 6420 7472 7574  with ground trut
+00004770: 6820 616e 642f 6f72 2070 7265 6469 6374  h and/or predict
+00004780: 6564 2061 6e6e 6f74 6174 696f 6e73 2e0a  ed annotations..
+00004790: 0a0a 2323 2320 7361 6e64 626f 780a 0a52  ..### sandbox..R
+000047a0: 616e 646f 6d20 7468 696e 6773 2074 6861  andom things tha
+000047b0: 7420 646f 6e27 7420 6669 7420 696e 2061  t don't fit in a
+000047c0: 6e79 206f 7468 6572 2064 6972 6563 746f  ny other directo
+000047d0: 7279 2c20 6275 7420 6172 656e 2774 2071  ry, but aren't q
+000047e0: 7569 7465 2064 6570 7265 6361 7465 642e  uite deprecated.
+000047f0: 2020 4d6f 7374 6c79 2070 6f73 7470 726f    Mostly postpro
+00004800: 6365 7373 696e 6720 7363 7269 7074 7320  cessing scripts 
+00004810: 7468 6174 2077 6572 6520 6275 696c 7420  that were built 
+00004820: 666f 7220 6120 7369 6e67 6c65 2075 7365  for a single use
+00004830: 2063 6173 6520 6275 7420 636f 756c 6420   case but could 
+00004840: 706f 7465 6e74 6961 6c6c 7920 6265 2075  potentially be u
+00004850: 7365 6675 6c20 696e 2074 6865 2066 7574  seful in the fut
+00004860: 7572 652e 0a0a 0a23 2323 2074 6178 6f6e  ure....### taxon
+00004870: 6f6d 795f 6d61 7070 696e 670a 0a43 6f64  omy_mapping..Cod
+00004880: 6520 746f 2066 6163 696c 6974 6174 6520  e to facilitate 
+00004890: 6d61 7070 696e 6720 6461 7461 2d73 6574  mapping data-set
+000048a0: 2d73 7065 6369 6669 6320 6361 7465 676f  -specific catego
+000048b0: 7279 206e 616d 6573 2028 652e 672e 2022  ry names (e.g. "
+000048c0: 6c69 6f6e 222c 2077 6869 6368 206d 6561  lion", which mea
+000048d0: 6e73 2076 6572 7920 6469 6666 6572 656e  ns very differen
+000048e0: 7420 7468 696e 6773 2069 6e20 4964 6168  t things in Idah
+000048f0: 6f20 7673 2e20 536f 7574 6820 4166 7269  o vs. South Afri
+00004900: 6361 2920 746f 2061 2073 7461 6e64 6172  ca) to a standar
+00004910: 6420 7461 786f 6e6f 6d79 2e0a 0a0a 2323  d taxonomy....##
+00004920: 2320 7465 7374 5f69 6d61 6765 730a 0a41  # test_images..A
+00004930: 2068 616e 6466 756c 206f 6620 696d 6167   handful of imag
+00004940: 6573 2066 726f 6d20 5b4c 494c 415d 2868  es from [LILA](h
+00004950: 7474 7073 3a2f 2f6c 696c 612e 7363 6965  ttps://lila.scie
+00004960: 6e63 6529 2074 6861 7420 6661 6369 6c69  nce) that facili
+00004970: 7461 7465 2074 6573 7469 6e67 2061 6e64  tate testing and
+00004980: 2064 6562 7567 6769 6e67 2e0a 0a0a 2323   debugging....##
+00004990: 2043 6f6e 7461 6374 0a0a 466f 7220 7175   Contact..For qu
+000049a0: 6573 7469 6f6e 7320 6162 6f75 7420 7468  estions about th
+000049b0: 6973 2072 6570 6f2c 2063 6f6e 7461 6374  is repo, contact
+000049c0: 205b 6361 6d65 7261 7472 6170 7340 6c69   [cameratraps@li
+000049d0: 6c61 2e73 6369 656e 6365 5d28 6d61 696c  la.science](mail
+000049e0: 746f 3a63 616d 6572 6174 7261 7073 406c  to:cameratraps@l
+000049f0: 696c 612e 7363 6965 6e63 6529 2e0a 0a59  ila.science)...Y
+00004a00: 6f75 2063 616e 2061 6c73 6f20 6368 6174  ou can also chat
+00004a10: 2077 6974 6820 7573 2061 6e64 2074 6865   with us and the
+00004a20: 2062 726f 6164 6572 2063 616d 6572 6120   broader camera 
+00004a30: 7472 6170 2041 4920 636f 6d6d 756e 6974  trap AI communit
+00004a40: 7920 6f6e 2074 6865 205b 4149 2066 6f72  y on the [AI for
+00004a50: 2043 6f6e 7365 7276 6174 696f 6e20 666f   Conservation fo
+00004a60: 7275 6d20 6174 2057 494c 444c 4142 535d  rum at WILDLABS]
+00004a70: 2868 7474 7073 3a2f 2f77 696c 646c 6162  (https://wildlab
+00004a80: 732e 6e65 742f 6772 6f75 7073 2f61 692d  s.net/groups/ai-
+00004a90: 636f 6e73 6572 7661 7469 6f6e 2920 6f72  conservation) or
+00004aa0: 2074 6865 205b 4149 2066 6f72 2043 6f6e   the [AI for Con
+00004ab0: 7365 7276 6174 696f 6e20 536c 6163 6b20  servation Slack 
+00004ac0: 6772 6f75 705d 2868 7474 7073 3a2f 2f61  group](https://a
+00004ad0: 6966 6f72 636f 6e73 6572 7661 7469 6f6e  iforconservation
+00004ae0: 2e73 6c61 636b 2e63 6f6d 292e 0a0a 0a23  .slack.com)....#
+00004af0: 2320 4772 6174 7569 746f 7573 2063 616d  # Gratuitous cam
+00004b00: 6572 6120 7472 6170 2070 6963 7475 7265  era trap picture
+00004b10: 0a0a 215b 4269 7264 2066 6c79 696e 6720  ..![Bird flying 
+00004b20: 6162 6f76 6520 7761 7465 725d 2869 6d61  above water](ima
+00004b30: 6765 732f 6e61 6374 692e 6a70 6729 3c62  ges/nacti.jpg)<b
+00004b40: 722f 3e49 6d61 6765 2063 7265 6469 7420  r/>Image credit 
+00004b50: 5553 4441 2c20 6672 6f6d 2074 6865 205b  USDA, from the [
+00004b60: 4e41 4354 495d 2868 7474 703a 2f2f 6c69  NACTI](http://li
+00004b70: 6c61 2e73 6369 656e 6365 2f64 6174 6173  la.science/datas
+00004b80: 6574 732f 6e61 6374 6929 2064 6174 6120  ets/nacti) data 
+00004b90: 7365 742e 0a0a 596f 7520 7769 6c6c 2066  set...You will f
+00004ba0: 696e 6420 6c6f 7473 206d 6f72 6520 6772  ind lots more gr
+00004bb0: 6174 7569 746f 7573 2063 616d 6572 6120  atuitous camera 
+00004bc0: 7472 6170 2070 6963 7475 7265 7320 7370  trap pictures sp
+00004bd0: 7269 6e6b 6c65 6420 6162 6f75 7420 7468  rinkled about th
+00004be0: 6973 2072 6570 6f2e 2020 4974 2773 206c  is repo.  It's l
+00004bf0: 696b 6520 6120 7363 6176 656e 6765 7220  ike a scavenger 
+00004c00: 6875 6e74 2e0a 0a0a 2323 204c 6963 656e  hunt....## Licen
+00004c10: 7365 0a0a 5468 6973 2072 6570 6f73 6974  se..This reposit
+00004c20: 6f72 7920 6973 206c 6963 656e 7365 6420  ory is licensed 
+00004c30: 7769 7468 2074 6865 205b 4d49 5420 6c69  with the [MIT li
+00004c40: 6365 6e73 655d 2868 7474 7073 3a2f 2f6f  cense](https://o
+00004c50: 7065 6e73 6f75 7263 652e 6f72 672f 6c69  pensource.org/li
+00004c60: 6365 6e73 652f 6d69 742f 292e 0a0a 436f  cense/mit/)...Co
+00004c70: 6465 2077 7269 7474 656e 206f 6e20 6f72  de written on or
+00004c80: 2062 6566 6f72 6520 4170 7269 6c20 3238   before April 28
+00004c90: 2c20 3230 3233 2069 7320 5b63 6f70 7972  , 2023 is [copyr
+00004ca0: 6967 6874 204d 6963 726f 736f 6674 5d28  ight Microsoft](
+00004cb0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00004cc0: 6f6d 2f4d 6963 726f 736f 6674 2f64 6f74  om/Microsoft/dot
+00004cd0: 6e65 742f 626c 6f62 2f6d 6169 6e2f 4c49  net/blob/main/LI
+00004ce0: 4345 4e53 4529 2e0a 0a0a 2323 2043 6f6e  CENSE)....## Con
+00004cf0: 7472 6962 7574 696e 670a 0a54 6869 7320  tributing..This 
+00004d00: 7072 6f6a 6563 7420 7765 6c63 6f6d 6573  project welcomes
+00004d10: 2063 6f6e 7472 6962 7574 696f 6e73 2c20   contributions, 
+00004d20: 6173 2070 756c 6c20 7265 7175 6573 7473  as pull requests
+00004d30: 2c20 6973 7375 6573 2c20 6f72 2073 7567  , issues, or sug
+00004d40: 6765 7374 696f 6e73 2062 7920 5b65 6d61  gestions by [ema
+00004d50: 696c 5d28 6d61 696c 746f 3a63 616d 6572  il](mailto:camer
+00004d60: 6174 7261 7073 406c 696c 612e 7363 6965  atraps@lila.scie
+00004d70: 6e63 6529 2e20 2057 6520 6861 7665 2061  nce).  We have a
+00004d80: 205b 6c69 7374 5d28 6874 7470 733a 2f2f   [list](https://
+00004d90: 6769 7468 7562 2e63 6f6d 2f61 6765 6e74  github.com/agent
+00004da0: 6d6f 7272 6973 2f4d 6567 6144 6574 6563  morris/MegaDetec
+00004db0: 746f 722f 6973 7375 6573 2f38 3429 206f  tor/issues/84) o
+00004dc0: 6620 6973 7375 6573 2074 6861 7420 7765  f issues that we
+00004dd0: 2772 6520 686f 7069 6e67 2074 6f20 6164  're hoping to ad
+00004de0: 6472 6573 732c 206d 616e 7920 6f66 2077  dress, many of w
+00004df0: 6869 6368 2077 6f75 6c64 2062 6520 676f  hich would be go
+00004e00: 6f64 2073 7461 7274 696e 6720 706f 696e  od starting poin
+00004e10: 7473 2066 6f72 206e 6577 2063 6f6e 7472  ts for new contr
+00004e20: 6962 7574 6f72 732e 2020 5765 2061 6c73  ibutors.  We als
+00004e30: 6f20 6465 7065 6e64 206f 6e20 6f74 6865  o depend on othe
+00004e40: 7220 6f70 656e 2d73 6f75 7263 6520 746f  r open-source to
+00004e50: 6f6c 7320 7468 6174 2068 656c 7020 7573  ols that help us
+00004e60: 6572 7320 7275 6e20 4d65 6761 4465 7465  ers run MegaDete
+00004e70: 6374 6f72 2028 652e 672e 205b 4563 6f41  ctor (e.g. [EcoA
+00004e80: 7373 6973 745d 2868 7474 7073 3a2f 2f67  ssist](https://g
+00004e90: 6974 6875 622e 636f 6d2f 5065 7465 7276  ithub.com/Peterv
+00004ea0: 616e 4c75 6e74 6572 656e 2f45 636f 4173  anLunteren/EcoAs
+00004eb0: 7369 7374 2920 616e 6420 5b43 616d 5472  sist) and [CamTr
+00004ec0: 6170 2044 6574 6563 746f 725d 2868 7474  ap Detector](htt
+00004ed0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00004ee0: 6265 6e63 6576 616e 732f 6361 6d74 7261  bencevans/camtra
+00004ef0: 702d 6465 7465 6374 6f72 2929 2061 6e64  p-detector)) and
+00004f00: 2077 6f72 6b20 7769 7468 204d 6567 6144   work with MegaD
+00004f10: 6574 6563 746f 7220 7265 7375 6c74 7320  etector results 
+00004f20: 2865 2e67 2e20 5b54 696d 656c 6170 7365  (e.g. [Timelapse
+00004f30: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+00004f40: 2e63 6f6d 2f73 6175 6c67 7265 656e 6265  .com/saulgreenbe
+00004f50: 7267 2f54 696d 656c 6170 7365 2929 3b20  rg/Timelapse)); 
+00004f60: 6966 2079 6f75 2061 7265 206c 6f6f 6b69  if you are looki
+00004f70: 6e67 2074 6f20 6765 7420 696e 766f 6c76  ng to get involv
+00004f80: 6564 2069 6e20 4755 4920 6465 7665 6c6f  ed in GUI develo
+00004f90: 706d 656e 742c 2072 6561 6368 206f 7574  pment, reach out
+00004fa0: 2074 6f20 7468 6520 6465 7665 6c6f 7065   to the develope
+00004fb0: 7273 206f 6620 7468 6f73 6520 746f 6f6c  rs of those tool
+00004fc0: 7320 6173 2077 656c 6c21 0a0a 4966 2079  s as well!..If y
+00004fd0: 6f75 2061 7265 2069 6e74 6572 6573 7469  ou are interesti
+00004fe0: 6e67 2069 6e20 6765 7474 696e 6720 696e  ng in getting in
+00004ff0: 766f 6c76 6564 2069 6e20 7468 6520 636f  volved in the co
+00005000: 6e73 6572 7661 7469 6f6e 2074 6563 686e  nservation techn
+00005010: 6f6c 6f67 7920 7370 6163 652c 2061 6e64  ology space, and
+00005020: 204d 6567 6144 6574 6563 746f 7220 6a75   MegaDetector ju
+00005030: 7374 2068 6170 7065 6e73 2074 6f20 6265  st happens to be
+00005040: 2074 6865 2066 6972 7374 2070 6167 6520   the first page 
+00005050: 796f 7520 6c61 6e64 6564 206f 6e2c 2061  you landed on, a
+00005060: 6e64 206e 6f6e 6520 6f66 206f 7572 206f  nd none of our o
+00005070: 7065 6e20 6973 7375 6573 2061 7265 2067  pen issues are g
+00005080: 6574 7469 6e67 2079 6f75 2066 6972 6564  etting you fired
+00005090: 2075 702c 2064 6f6e 2774 2066 7265 7421   up, don't fret!
+000050a0: 2020 4865 6164 206f 7665 7220 746f 2074    Head over to t
+000050b0: 6865 205b 5749 4c44 4c41 4253 2064 6973  he [WILDLABS dis
+000050c0: 6375 7373 696f 6e20 666f 7275 6d73 5d28  cussion forums](
+000050d0: 6874 7470 733a 2f2f 7769 6c64 6c61 6273  https://wildlabs
+000050e0: 2e6e 6574 2f64 6973 6375 7373 696f 6e73  .net/discussions
+000050f0: 2920 616e 6420 6c65 7420 7468 6520 636f  ) and let the co
+00005100: 6d6d 756e 6974 7920 6b6e 6f77 2079 6f75  mmunity know you
+00005110: 2772 6520 6120 6465 7665 6c6f 7065 7220  're a developer 
+00005120: 6c6f 6f6b 696e 6720 746f 2067 6574 2069  looking to get i
+00005130: 6e76 6f6c 7665 642e 2020 536f 6d65 6f6e  nvolved.  Someon
+00005140: 6520 6e65 6564 7320 796f 7572 2068 656c  e needs your hel
+00005150: 7021 0a                                  p!.
```

### Comparing `megadetector-5.0.7/api/batch_processing/api_core/batch_service/score.py` & `megadetector-5.0.8/api/batch_processing/api_core/batch_service/score.py`

 * *Files identical despite different names*

### Comparing `megadetector-5.0.7/api/batch_processing/api_core/server.py` & `megadetector-5.0.8/api/batch_processing/api_core/server.py`

 * *Files identical despite different names*

### Comparing `megadetector-5.0.7/api/batch_processing/api_core/server_api_config.py` & `megadetector-5.0.8/api/batch_processing/api_core/server_api_config.py`

 * *Files identical despite different names*

### Comparing `megadetector-5.0.7/api/batch_processing/api_core/server_app_config.py` & `megadetector-5.0.8/api/batch_processing/api_core/server_app_config.py`

 * *Files identical despite different names*

### Comparing `megadetector-5.0.7/api/batch_processing/api_core/server_batch_job_manager.py` & `megadetector-5.0.8/api/batch_processing/api_core/server_batch_job_manager.py`

 * *Files identical despite different names*

### Comparing `megadetector-5.0.7/api/batch_processing/api_core/server_job_status_table.py` & `megadetector-5.0.8/api/batch_processing/api_core/server_job_status_table.py`

 * *Files identical despite different names*

### Comparing `megadetector-5.0.7/api/batch_processing/api_core/server_orchestration.py` & `megadetector-5.0.8/api/batch_processing/api_core/server_orchestration.py`

 * *Files identical despite different names*

### Comparing `megadetector-5.0.7/api/batch_processing/api_core/server_utils.py` & `megadetector-5.0.8/api/batch_processing/api_core/server_utils.py`

 * *Files identical despite different names*

### Comparing `megadetector-5.0.7/api/batch_processing/api_core_support/aggregate_results_manually.py` & `megadetector-5.0.8/api/batch_processing/api_core_support/aggregate_results_manually.py`

 * *Files identical despite different names*

### Comparing `megadetector-5.0.7/api/batch_processing/api_support/summarize_daily_activity.py` & `megadetector-5.0.8/api/batch_processing/api_support/summarize_daily_activity.py`

 * *Files identical despite different names*

### Comparing `megadetector-5.0.7/api/batch_processing/data_preparation/manage_local_batch.py` & `megadetector-5.0.8/api/batch_processing/data_preparation/manage_local_batch.py`

 * *Files 0% similar despite different names*

```diff
@@ -82,14 +82,16 @@
 from detection.run_detector import estimate_md_images_per_second
 
 from api.batch_processing.postprocessing.postprocess_batch_results import (
     PostProcessingOptions, process_batch_results)
 from detection.run_detector import get_detector_version_from_filename
 from md_utils.ct_utils import image_file_to_camera_folder
 
+## Inference options
+
 # To specify a non-default confidence threshold for including detections in the .json file
 json_threshold = None
 
 # Turn warnings into errors if more than this many images are missing
 max_tolerable_failed_images = 100
 
 # Should we supply the --image_queue_option to run_detector_batch.py?  I only set this 
@@ -105,14 +107,19 @@
 
 # Specify a target image size when running MD... strongly recommended to leave this at "None"
 #
 # When using augmented inference, if you leave this at "None", run_inference_with_yolov5_val.py
 # will use its default size, which is 1280 * 1.3, which is almost always what you want.
 image_size = None
 
+# Should we include image size, timestamp, and/or EXIF data in MD output?
+include_image_size = False
+include_image_timestamp = False
+include_exif_data = False
+
 # Only relevant when running on CPU
 ncores = 1
 
 # OS-specific script line continuation character (modified later if we're running on Windows)
 slcc = '\\'
 
 # OS-specific script comment character (modified later if we're running on Windows)
@@ -183,15 +190,15 @@
 
 # Should we apply YOLOv5's test-time augmentation?
 augment = False
 
 
 ## Constants related to tiled inference
 
-use_tiled_inference = True
+use_tiled_inference = False
 
 # Should we delete tiles after each job?  Only set this to False for debugging;
 # large jobs will take up a lot of space if you keep tiles around after each task.
 remove_tiles = True
 tile_size = (1280,1280)
 tile_overlap = 0.2
 
@@ -230,15 +237,15 @@
 # checkpointing.  Don't worry, this will be assert()'d in the next cell.
 checkpoint_frequency = 10000
 
 # Estimate inference speed for the current GPU
 approx_images_per_second = estimate_md_images_per_second(model_file) 
     
 # Rough estimate for the inference time cost of augmentation    
-if augment:
+if augment and (approx_images_per_second is not None):
     approx_images_per_second = approx_images_per_second * 0.7
     
 base_task_name = organization_name_short + '-' + job_date + job_description_string + '-' + \
     get_detector_version_from_filename(model_file)
 base_output_folder_name = os.path.join(postprocessing_base,organization_name_short)
 os.makedirs(base_output_folder_name,exist_ok=True)
 
@@ -264,14 +271,18 @@
     assert checkpoint_frequency is None, \
         'Checkpointing is not supported when using tiled inference'
         
 filename_base = os.path.join(base_output_folder_name, base_task_name)
 combined_api_output_folder = os.path.join(filename_base, 'combined_api_outputs')
 postprocessing_output_folder = os.path.join(filename_base, 'preview')
 
+combined_api_output_file = os.path.join(
+    combined_api_output_folder,
+    '{}_detections.json'.format(base_task_name))
+
 os.makedirs(filename_base, exist_ok=True)
 os.makedirs(combined_api_output_folder, exist_ok=True)
 os.makedirs(postprocessing_output_folder, exist_ok=True)
 
 if input_path.endswith('/'):
     input_path = input_path[0:-1]
 
@@ -490,15 +501,22 @@
         
         confidence_threshold_string = ''
         if json_threshold is not None:
             confidence_threshold_string = '--threshold {}'.format(json_threshold)
         
         overwrite_handling_string = '--overwrite_handling {}'.format(overwrite_handling)        
         cmd = f'{cuda_string} python run_detector_batch.py "{model_file}" "{chunk_file}" "{output_fn}" {checkpoint_frequency_string} {checkpoint_path_string} {use_image_queue_string} {ncores_string} {quiet_string} {image_size_string} {confidence_threshold_string} {overwrite_handling_string}'
-                
+        
+        if include_image_size:
+            cmd += ' --include_image_size'
+        if include_image_timestamp:
+            cmd += ' --include_image_timestamp'
+        if include_exif_data:
+            cmd += ' --include_exif_data'
+        
     cmd_file = os.path.join(filename_base,'run_chunk_{}_gpu_{}{}'.format(str(i_task).zfill(3),
                             str(gpu_number).zfill(2),script_extension))
     
     with open(cmd_file,'w') as f:
         f.write(cmd + '\n')
     
     st = os.stat(cmd_file)
@@ -743,18 +761,14 @@
     assert '\\' not in im['file']
     assert im['file'].startswith(input_path)
     if input_path.endswith(':'):
         im['file'] = im['file'].replace(input_path,'',1)
     else:
         im['file'] = im['file'].replace(input_path + '/','',1)
     
-combined_api_output_file = os.path.join(
-    combined_api_output_folder,
-    '{}_detections.json'.format(base_task_name))
-
 with open(combined_api_output_file,'w') as f:
     json.dump(combined_results,f,indent=1)
 
 print('Wrote results to {}'.format(combined_api_output_file))
 
 
 #%% Post-processing (pre-RDE)
@@ -789,15 +803,15 @@
 os.makedirs(output_base, exist_ok=True)
 print('Processing to {}'.format(output_base))
 
 options.api_output_file = combined_api_output_file
 options.output_dir = output_base
 ppresults = process_batch_results(options)
 html_output_file = ppresults.output_html_file
-path_utils.open_file(html_output_file,attempt_to_open_in_wsl_host=True)
+path_utils.open_file(html_output_file,attempt_to_open_in_wsl_host=True,browser_name='chrome')
 # import clipboard; clipboard.copy(html_output_file)
 
 
 #%% Repeat detection elimination, phase 1
 
 # Deliberately leaving these imports here, rather than at the top, because this
 # cell is not typically executed
@@ -819,15 +833,15 @@
 # This will cause a very light gray box to get drawn around all the detections
 # we're *not* considering as suspicious.
 options.bRenderOtherDetections = True
 options.otherDetectionsThreshold = options.confidenceMin
 
 options.bRenderDetectionTiles = True
 options.maxOutputImageWidth = 2000
-options.detectionTilesMaxCrops = 300
+options.detectionTilesMaxCrops = 250
 
 # options.lineThickness = 5
 # options.boxExpansion = 8
 
 # To invoke custom collapsing of folders for a particular manufacturer's naming scheme
 options.customDirNameFunction = relative_path_to_location
 
@@ -926,15 +940,15 @@
 print('Processing post-RDE to {}'.format(output_base))
 
 options.api_output_file = filtered_output_filename
 options.output_dir = output_base
 ppresults = process_batch_results(options)
 html_output_file = ppresults.output_html_file
 
-path_utils.open_file(html_output_file,attempt_to_open_in_wsl_host=True)
+path_utils.open_file(html_output_file,attempt_to_open_in_wsl_host=True,browser_name='chrome')
 # import clipboard; clipboard.copy(html_output_file)
 
 
 #%% Run MegaClassifier (actually, write out a script that runs MegaClassifier)
 
 # Variables that will indicate which classifiers we ran
 final_output_path_mc = None
@@ -1999,15 +2013,15 @@
     base_task_name + '_{:.3f}'.format(options.confidence_threshold))
 os.makedirs(output_base, exist_ok=True)
 print('Processing {} to {}'.format(base_task_name, output_base))
 
 options.api_output_file = sequence_smoothed_classification_file
 options.output_dir = output_base
 ppresults = process_batch_results(options)
-path_utils.open_file(ppresults.output_html_file,attempt_to_open_in_wsl_host=True)
+path_utils.open_file(ppresults.output_html_file,attempt_to_open_in_wsl_host=True,browser_name='chrome')
 # import clipboard; clipboard.copy(ppresults.output_html_file)
 
 #% Zip .json files
 
 from md_utils.path_utils import parallel_zip_files
 
 json_files = os.listdir(combined_api_output_folder)
@@ -2067,15 +2081,15 @@
                                                'person':detection_thresholds[j],
                                                'vehicle':detection_thresholds[j]}
     options.pairwise_options.append(pairwise_options)
 
 results = compare_batch_results(options)
 
 from md_utils.path_utils import open_file
-open_file(results.html_output_file,attempt_to_open_in_wsl_host=True)
+open_file(results.html_output_file,attempt_to_open_in_wsl_host=True,browser_name='chrome')
 
 
 #%% Merge in high-confidence detections from another results file
 
 from api.batch_processing.postprocessing.merge_detections import MergeDetectionsOptions,merge_detections
 
 source_files = ['']
@@ -2121,15 +2135,15 @@
 print('Processing post-RDE, post-size-separation to {}'.format(output_base_large_boxes))
 
 options.api_output_file = size_separated_file
 options.output_dir = output_base_large_boxes
 
 ppresults = process_batch_results(options)
 html_output_file = ppresults.output_html_file
-path_utils.open_file(html_output_file,attempt_to_open_in_wsl_host=True)
+path_utils.open_file(html_output_file,attempt_to_open_in_wsl_host=True,browser_name='chrome')
 
 
 #%% .json splitting
 
 data = None
 
 from api.batch_processing.postprocessing.subset_json_detector_output import (
@@ -2276,15 +2290,15 @@
 
 import os
 import nbformat as nbf
 
 if os.name == 'nt':
     git_base = r'c:\git'
 else:
-    git_base = os.path.expanduer('~/git')
+    git_base = os.path.expanduser('~/git')
     
 input_py_file = git_base + '/MegaDetector/api/batch_processing/data_preparation/manage_local_batch.py'
 assert os.path.isfile(input_py_file)
 output_ipynb_file = input_py_file.replace('.py','.ipynb')
 
 nb_header = '# Managing a local MegaDetector batch'
```

### Comparing `megadetector-5.0.7/api/batch_processing/data_preparation/manage_video_batch.py` & `megadetector-5.0.8/api/batch_processing/data_preparation/manage_video_batch.py`

 * *Files identical despite different names*

### Comparing `megadetector-5.0.7/api/batch_processing/integration/digiKam/xmp_integration.py` & `megadetector-5.0.8/api/batch_processing/integration/digiKam/xmp_integration.py`

 * *Files identical despite different names*

### Comparing `megadetector-5.0.7/api/batch_processing/integration/eMammal/test_scripts/push_annotations_to_emammal.py` & `megadetector-5.0.8/api/batch_processing/integration/eMammal/test_scripts/push_annotations_to_emammal.py`

 * *Files identical despite different names*

### Comparing `megadetector-5.0.7/api/batch_processing/integration/eMammal/test_scripts/select_images_for_testing.py` & `megadetector-5.0.8/api/batch_processing/integration/eMammal/test_scripts/select_images_for_testing.py`

 * *Files identical despite different names*

### Comparing `megadetector-5.0.7/api/batch_processing/postprocessing/add_max_conf.py` & `megadetector-5.0.8/api/batch_processing/postprocessing/add_max_conf.py`

 * *Files identical despite different names*

### Comparing `megadetector-5.0.7/api/batch_processing/postprocessing/categorize_detections_by_size.py` & `megadetector-5.0.8/api/batch_processing/postprocessing/categorize_detections_by_size.py`

 * *Files identical despite different names*

### Comparing `megadetector-5.0.7/api/batch_processing/postprocessing/combine_api_outputs.py` & `megadetector-5.0.8/api/batch_processing/postprocessing/combine_api_outputs.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
     Merges list of JSON API detection files *input_files* into a single
     dictionary, optionally writing the result to *output_file*.
 
     Args:
         input_files: list of str, paths to JSON detection files
         output_file: optional str, path to write merged JSON
         require_uniqueness: bool, whether to require that the images in
-            each input_dict be unique
+            each list of images be unique
     """
     
     def print_if_verbose(s):
         if verbose:
             print(s)
             
     input_dicts = []
@@ -80,15 +80,15 @@
     Merges the list of API detection dictionaries *input_dicts*.  See header
     comment for details on merge rules.
 
     Args:
         input_dicts: list of dicts, each dict is the JSON of the detections
             output file from the Batch Processing API
         require_uniqueness: bool, whether to require that the images in
-            each input_dict be unique
+            each input dict be unique
 
     Returns: dict, represents the merged JSON
     """
     
     # Map image filenames to detections, we'll convert to a list later
     images = {}
     info: Dict[str, str] = {}
```

### Comparing `megadetector-5.0.7/api/batch_processing/postprocessing/compare_batch_results.py` & `megadetector-5.0.8/api/batch_processing/postprocessing/compare_batch_results.py`

 * *Files 0% similar despite different names*

```diff
@@ -287,15 +287,15 @@
     
     ##%% Make sure they represent the same set of images
     
     filenames_a = [im['file'] for im in images_a]
     filenames_b_set = set([im['file'] for im in images_b])
     
     if len(images_a) != len(images_b):
-        s = 'set A has {} iamges, set B has {}'.format(len(images_a),len(images_b))
+        s = 'set A has {} images, set B has {}'.format(len(images_a),len(images_b))
         if options.error_on_non_matching_lists:
             raise ValueError(s)
         else:
             print('Warning: ' + s)
     else:
         if options.error_on_non_matching_lists:
             for fn in filenames_a:
```

### Comparing `megadetector-5.0.7/api/batch_processing/postprocessing/convert_output_format.py` & `megadetector-5.0.8/api/batch_processing/postprocessing/convert_output_format.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 ########
 #
 # convert_output_format.py
 #
 # Converts between file formats output by our batch processing API.  Currently
 # supports json <--> csv conversion, but this should be the landing place for any
-# conversion - including between future .json versions - that we support in the 
-# future.
+# conversion - including between hypothetical alternative .json versions - that we support 
+# in the future.
 #
 ########
 
 #%% Constants and imports
 
 import argparse
 import json
@@ -26,26 +26,33 @@
 
 CONF_DIGITS = 3
 
 
 #%% Conversion functions
 
 def convert_json_to_csv(input_path,output_path=None,min_confidence=None,
-                        omit_bounding_boxes=False,output_encoding=None):
+                        omit_bounding_boxes=False,output_encoding=None,
+                        overwrite=True):
     """
     Convert .json to .csv
     
+    If output_path is None, will convert x.json to x.csv.
+    
     TODO: this function should obviously be using Pandas or some other sensible structured
     representation of tabular data.  Even a list of dicts.  This implementation is quite
     brittle and depends on adding fields to every row in exactly the right order.
     """
     
     if output_path is None:
         output_path = os.path.splitext(input_path)[0]+'.csv'
         
+    if os.path.isfile(output_path) and (not overwrite):
+        print('File {} exists, skipping json --> csv conversion'.format(output_path))
+        return
+    
     print('Loading json results from {}...'.format(input_path))
     json_output = json.load(open(input_path))
 
     rows = []
     
     fixed_columns = ['image_path', 'max_confidence', 'detections']
     
@@ -69,15 +76,15 @@
             category_name = classification_category_id_to_name[category_id].\
                 replace(' ','_').replace(',','')
             classification_category_column_names.append('max_classification_conf_' + category_name)
             classification_category_id_to_column_number[category_id] = i_category
 
         n_classification_categories = len(classification_category_ids)
     
-    # There are several fields for which we add columns, other random bespoke fields
+    # There are several .json fields for which we add .csv columns; other random bespoke fields
     # will be ignored.
     optional_fields = ['width','height','datetime','exif_metadata']
     optional_fields_present = set()
     
     # Iterate once over the data to check for optional fields
     print('Looking for optional fields...')
     
@@ -100,15 +107,15 @@
     for im in tqdm(json_output['images']):
         
         image_id = im['file']
         
         if 'failure' in im and im['failure'] is not None:
             row = [image_id, 'failure', im['failure']]
             rows.append(row)
-            print('Skipping failed image {} ({})'.format(im['file'],im['failure']))
+            # print('Skipping failed image {} ({})'.format(im['file'],im['failure']))
             continue
 
         max_conf = ct_utils.get_max_conf(im)
         detections = []
         max_detection_category_probabilities = [None] * n_non_empty_detection_categories
         max_classification_category_probabilities = [0] * n_classification_categories
               
@@ -189,20 +196,29 @@
         if n_classification_categories > 0:
             header.extend(classification_category_column_names)
         for field_name in optional_fields_present:
             header.append(field_name)
         writer.writerow(header)
         writer.writerows(rows)
 
+# ...def convert_json_to_csv(...)
+
     
-def convert_csv_to_json(input_path,output_path=None):
+def convert_csv_to_json(input_path,output_path=None,overwrite=True):
+    """
+    Convert .csv to .json.  If output_path is None, will convert x.csv to x.json.
+    """
     
     if output_path is None:
         output_path = os.path.splitext(input_path)[0]+'.json'
         
+    if os.path.isfile(output_path) and (not overwrite):
+        print('File {} exists, skipping csv --> json conversion'.format(output_path))
+        return
+            
     # Format spec:
     #
     # https://github.com/agentmorris/MegaDetector/tree/master/api/batch_processing
     
     print('Loading csv results...')
     df = load_api_results_csv(input_path)
 
@@ -255,14 +271,16 @@
     json_out = {}
     json_out['info'] = info
     json_out['detection_categories'] = detection_categories
     json_out['classification_categories'] = classification_categories
     json_out['images'] = images
     
     json.dump(json_out,open(output_path,'w'),indent=1)
+    
+# ...def convert_csv_to_json(...)
 
 
 #%% Interactive driver
 
 if False:    
 
     #%%
```

### Comparing `megadetector-5.0.7/api/batch_processing/postprocessing/load_api_results.py` & `megadetector-5.0.8/api/batch_processing/postprocessing/load_api_results.py`

 * *Files 5% similar despite different names*

```diff
@@ -60,19 +60,17 @@
 
     # Fields in the output json other than 'images'
     other_fields = {}
     for k, v in detection_results.items():
         if k != 'images':
             other_fields[k] = v
 
-    # Normalize paths to simplify comparisons later
     if normalize_paths:
         for image in detection_results['images']:
-            image['file'] = os.path.normpath(image['file'])
-            # image['file'] = image['file'].replace('\\','/')
+            image['file'] = os.path.normpath(image['file'])            
 
     if force_forward_slashes:
         for image in detection_results['images']:
             image['file'] = image['file'].replace('\\','/')
             
     # Replace some path tokens to match local paths to original blob structure
     if filename_replacements is not None:
```

### Comparing `megadetector-5.0.7/api/batch_processing/postprocessing/md_to_coco.py` & `megadetector-5.0.8/api/batch_processing/postprocessing/md_to_coco.py`

 * *Files identical despite different names*

### Comparing `megadetector-5.0.7/api/batch_processing/postprocessing/md_to_labelme.py` & `megadetector-5.0.8/api/batch_processing/postprocessing/md_to_labelme.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,44 +16,55 @@
 #%% Imports and constants
 
 import os
 import json
 
 from tqdm import tqdm
 
+from multiprocessing.pool import Pool
+from multiprocessing.pool import ThreadPool
+from functools import partial
+
 from md_visualization.visualization_utils import open_image
 from md_utils.ct_utils import truncate_float
 
 output_precision = 3
 default_confidence_threshold = 0.15
 
 
 #%% Functions
 
-def get_labelme_dict_for_image(im,image_base_name,category_id_to_name,info=None,confidence_threshold=None):
+def get_labelme_dict_for_image(im,image_base_name,category_id_to_name,
+                               info=None,confidence_threshold=None):
     """
     For the given image struct in MD results format, reformat the detections into
     labelme format.  Returns a dict.
+    
+    'height' and 'width' are required in [im].
+    
+    image_base_name is written directly to the 'imagePath' field in the output; it should generally be
+    os.path.basename(your_image_file).
     """
     
     if confidence_threshold is None:        
         confidence_threshold = -1.0
-        
+     
     output_dict = {}
     if info is not None:
         output_dict['detector_info'] = info
     output_dict['version'] = '5.3.0a0'
     output_dict['flags'] = {}
     output_dict['shapes'] = []
     output_dict['imagePath'] = image_base_name
     output_dict['imageHeight'] = im['height']
     output_dict['imageWidth'] = im['width']
     output_dict['imageData'] = None
     output_dict['detections'] = im['detections']
     
+    # det = im['detections'][1]
     for det in im['detections']:
         
         if det['conf'] < confidence_threshold:
             continue
         
         shape = {}
         shape['conf'] = det['conf']
@@ -75,77 +86,133 @@
     # ...for each detection
     
     return output_dict
 
 # ...def get_labelme_dict_for_image()
 
 
+def _write_output_for_image(im,image_base,extension_prefix,info,
+                            confidence_threshold,category_id_to_name,overwrite,
+                            verbose=False):
+    
+    if 'failure' in im and im['failure'] is not None:
+        assert 'detections' not in im or im['detections'] is None
+        if verbose:
+            print('Skipping labelme file generation for failed image {}'.format(
+                im['file']))
+        return
+        
+    im_full_path = os.path.join(image_base,im['file'])
+    json_path = os.path.splitext(im_full_path)[0] + extension_prefix + '.json'
+    
+    if (not overwrite) and (os.path.isfile(json_path)):
+        if verbose:
+            print('Skipping existing file {}'.format(json_path))
+        return
+
+    output_dict = get_labelme_dict_for_image(im,
+                                             image_base_name=os.path.basename(im_full_path),
+                                             category_id_to_name=category_id_to_name,
+                                             info=info,
+                                             confidence_threshold=confidence_threshold)
+            
+    with open(json_path,'w') as f:
+        json.dump(output_dict,f,indent=1)
+    
+# ...def write_output_for_image(...)
+
+
+
 def md_to_labelme(results_file,image_base,confidence_threshold=None,
-                  overwrite=False):
+                  overwrite=False,extension_prefix='',n_workers=1,
+                  use_threads=False,bypass_image_size_read=False,
+                  verbose=False):
     """
     For all the images in [results_file], write a .json file in labelme format alongside the
     corresponding relative path within image_base.
+    
+    If non-empty, "extension_prefix" will be inserted before the .json extension.
     """
     
-    # Load MD results
-    with open(results_file,'r') as f:
-        md_results = json.load(f)
-        
-    # Read image sizes
-    #
-    # TODO: parallelize this loop
-    #
-    # im = md_results['images'][0]
-    for im in tqdm(md_results['images']):
-        
-        # Make sure this file exists
-        im_full_path = os.path.join(image_base,im['file'])
-        assert os.path.isfile(im_full_path), 'Image file {} does not exist'.format(im_full_path)
-        
-        # Load w/h information if necessary
-        if 'height' not in im or 'width' not in im:
-            
-            try:
-                pil_im = open_image(im_full_path)
-                im['width'] = pil_im.width
-                im['height'] = pil_im.height
-            except Exception:
-                print('Warning: cannot open image {}, treating as a failure during inference'.format(
-                    im_full_path))
-                if 'failure' not in im:
-                    im['failure'] = 'Failure image access'        
-
-        # ...if we need to read w/h information
+    if extension_prefix is None:
+        extension_prefix = ''
         
-    # ...for each image
-    
-    # Write output
-    for im in tqdm(md_results['images']):
+    # Load MD results if necessary
+    if isinstance(results_file,dict):
+        md_results = results_file
+    else:
+        print('Loading MD results...')
+        with open(results_file,'r') as f:
+            md_results = json.load(f)
         
-        if 'failure' in im and im['failure'] is not None:
-            assert 'detections' not in im
-            print('Warning: skipping labelme file generation for failed image {}'.format(
-                im['file']))
-            continue
-            
-        im_full_path = os.path.join(image_base,im['file'])
-        json_path = os.path.splitext(im_full_path)[0] + '.json'
+    # Read image sizes if necessary            
+    if bypass_image_size_read:     
         
-        if (not overwrite) and (os.path.isfile(json_path)):
-            print('Skipping existing file {}'.format(json_path))
-            continue
+        print('Bypassing image size read')
+        
+    else:
+    
+        # TODO: parallelize this loop
     
-        output_dict = get_labelme_dict_for_image(im,
-                                                 image_base_name=os.path.basename(im_full_path),
-                                                 category_id_to_name=md_results['detection_categories'],
-                                                 info=md_results['info'],
-                                                 confidence_threshold=confidence_threshold)
+        print('Reading image sizes...')
+                
+        # im = md_results['images'][0]
+        for im in tqdm(md_results['images']):
+            
+            # Make sure this file exists
+            im_full_path = os.path.join(image_base,im['file'])
+            assert os.path.isfile(im_full_path), 'Image file {} does not exist'.format(im_full_path)
+            
+            json_path = os.path.splitext(im_full_path)[0] + extension_prefix + '.json'
+            
+            # Don't even bother reading sizes for files we're not going to generate
+            if (not overwrite) and (os.path.isfile(json_path)):
+                continue
+            
+            # Load w/h information if necessary
+            if 'height' not in im or 'width' not in im:
                 
-        with open(json_path,'w') as f:
-            json.dump(output_dict,f,indent=1)
+                try:
+                    pil_im = open_image(im_full_path)
+                    im['width'] = pil_im.width
+                    im['height'] = pil_im.height
+                except Exception:
+                    print('Warning: cannot open image {}, treating as a failure during inference'.format(
+                        im_full_path))
+                    if 'failure' not in im:
+                        im['failure'] = 'Failure image access'        
+    
+            # ...if we need to read w/h information
+            
+        # ...for each image
+        
+    # ...if we're not bypassing image size read        
+    
+    print('\nGenerating labelme files...')
+        
+    # Write output
+    if n_workers <= 1:
+        for im in tqdm(md_results['images']):    
+            _write_output_for_image(im,image_base,extension_prefix,md_results['info'],confidence_threshold,
+                                   md_results['detection_categories'],overwrite,verbose)
+    else:
+        if use_threads:
+            print('Starting parallel thread pool with {} workers'.format(n_workers))
+            pool = ThreadPool(n_workers)
+        else:
+            print('Starting parallel process pool with {} workers'.format(n_workers))
+            pool = Pool(n_workers)
+        _ = list(tqdm(pool.imap(
+                partial(_write_output_for_image,
+                        image_base=image_base,extension_prefix=extension_prefix,
+                        info=md_results['info'],confidence_threshold=confidence_threshold,
+                        category_id_to_name=md_results['detection_categories'],
+                        overwrite=overwrite,verbose=verbose),
+                 md_results['images']),
+                 total=len(md_results['images'])))
             
     # ...for each image
     
 # ...def md_to_labelme()
 
 
 #%% Interactive driver
```

### Comparing `megadetector-5.0.7/api/batch_processing/postprocessing/merge_detections.py` & `megadetector-5.0.8/api/batch_processing/postprocessing/merge_detections.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 ########
 #
 # merge_detections.py
 #
 # Merge high-confidence detections from one or more results files into another 
-# file.   Typically used to combine results from MDv5b and/or MDv4 into a "primary"
+# file.  Typically used to combine results from MDv5b and/or MDv4 into a "primary"
 # results file from MDv5a.
 #
+# Detection categories must be the same in both files; if you want to first remap
+# one file's category mapping to be the same as another's, see remap_detection_categories.
+#
 # If you want to literally merge two .json files, see combine_api_outputs.py.
 #
 ########
 
 #%% Constants and imports
 
 import argparse
@@ -26,43 +29,64 @@
 
 class MergeDetectionsOptions:
     
     def __init__(self):
         
         self.max_detection_size = 1.01
         self.min_detection_size = 0
-        self.source_confidence_thresholds = [0.2]
+        self.source_confidence_thresholds = [0.05]
         
         # Don't bother merging into target images if there is a similar detection
         # above this threshold (or if there is *any* detection above this threshold,
         # and merge_empty_only is True)
         self.target_confidence_threshold = 0.2
         
         # If you want to merge only certain categories, specify one
-        # (but not both) of these.
+        # (but not both) of these.  These are category IDs, not names.
         self.categories_to_include = None
         self.categories_to_exclude = None
 
         # Only merge detections into images that have *no* detections in the 
         # target results file.
         self.merge_empty_only = False
         
         self.iou_threshold = 0.65
+        
+        self.overwrite = False
 
 
 #%% Main function
 
 def merge_detections(source_files,target_file,output_file,options=None):
+    """
+    Merge high-confidence detections from one or more results files into another 
+    file.   Typically used to combine results from MDv5b and/or MDv4 into a "primary"
+    results file from MDv5a.
+    
+    [source_files] (a list of files or a single filename) specifies the set of 
+    results files that will be merged into [target_file].  The difference between a 
+    "source file" and the "target file" is that if no merging is necessary, either because
+    two boxes are nearly identical or because merge_only_empty is True and the target
+    file already has above-threshold detection for an image+category, the output file gets
+    the results of the "target" file.  I.e., the "target" file wins all ties.
+    
+    The results are written to [output_file].
+
+    """
     
     if isinstance(source_files,str):
         source_files = [source_files]    
         
     if options is None:
         options = MergeDetectionsOptions()    
         
+    if (not options.overwrite) and (os.path.isfile(output_file)):
+        print('File {} exists, bypassing merge'.format(output_file))
+        return
+    
     assert not ((options.categories_to_exclude is not None) and \
                 (options.categories_to_include is not None)), \
                 'categories_to_include and categories_to_exclude are mutually exclusive'
     
     if options.categories_to_exclude is not None:
         options.categories_to_exclude = [int(c) for c in options.categories_to_exclude]
         
@@ -129,15 +153,16 @@
             source_detector_name = source_data['info']['detector']
         else:
             source_detector_name = os.path.basename(source_file)
         
         output_data['info']['detections_transferred_from'].append(os.path.basename(source_file))
         output_data['info']['detector'] = output_data['info']['detector'] + ' + ' + source_detector_name
         
-        assert source_data['detection_categories'] == output_data['detection_categories']
+        assert source_data['detection_categories'] == output_data['detection_categories'], \
+            'Cannot merge files with different detection category maps'
         
         source_confidence_threshold = options.source_confidence_thresholds[i_source_file]
         
         # source_im = source_data['images'][0]
         for source_im in tqdm(source_data['images']):
             
             image_filename = source_im['file']            
@@ -242,15 +267,15 @@
             # ...if we have any detections to transfer
             
         # ...for each image
         
     # ...for each source file        
     
     with open(output_file,'w') as f:
-        json.dump(output_data,f,indent=2)
+        json.dump(output_data,f,indent=1)
     
     print('Saved merged results to {}'.format(output_file))
 
 
 #%% Command-line driver
 
 def main():
```

### Comparing `megadetector-5.0.7/api/batch_processing/postprocessing/postprocess_batch_results.py` & `megadetector-5.0.8/api/batch_processing/postprocessing/postprocess_batch_results.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,14 @@
 import copy
 import errno
 import io
 import os
 import sys
 import time
 import uuid
-import urllib
 import warnings
 import random
 
 from typing import Any, Dict, Iterable, Optional, Tuple
 from enum import IntEnum
 from multiprocessing.pool import ThreadPool
 from multiprocessing.pool import Pool
@@ -49,15 +48,14 @@
 import md_visualization.plot_utils as plot_utils
 
 from md_utils.write_html_image_list import write_html_image_list
 from md_utils import path_utils
 from data_management.cct_json_utils import (CameraTrapJsonUtils, IndexedJsonDb)
 from api.batch_processing.postprocessing.load_api_results import load_api_results
 from md_utils.ct_utils import args_to_object
-from md_utils.ct_utils import invert_dictionary
 
 from detection.run_detector import get_typical_confidence_threshold_from_results
 
 warnings.filterwarnings('ignore', '(Possibly )?corrupt EXIF data', UserWarning)
 
 
 #%% Options
@@ -480,15 +478,22 @@
         'title': display_name,
         'textStyle':\
          'font-family:verdana,arial,calibri;font-size:80%;text-align:left;margin-top:20;margin-bottom:5'
     }
     
     # Optionally add links back to the original images
     if options.link_images_to_originals and (image_full_path is not None):
-        info['linkTarget'] = urllib.parse.quote(image_full_path)
+                
+        # Handling special characters in links has been pushed down into
+        # write_html_image_list
+        #
+        # link_target = image_full_path.replace('\\','/')
+        # link_target  = urllib.parse.quote(link_target)
+        link_target = image_full_path
+        info['linkTarget'] = link_target 
         
     return info
 
 # ...render_bounding_boxes
 
 
 def prepare_html_subpages(images_html, output_dir, options=None):
@@ -844,15 +849,15 @@
 
 
     ##%% Load ground truth if available
 
     ground_truth_indexed_db = None
 
     if (options.ground_truth_json_file is not None):
-        assert (options.confidence_threshold is None) or (isinstance(confidence_threshold,float)), \
+        assert (options.confidence_threshold is None) or (isinstance(options.confidence_threshold,float)), \
             'Variable confidence thresholds are not supported when supplying ground truth'
             
     if (options.ground_truth_json_file is not None) and (len(options.ground_truth_json_file) > 0):
 
         if options.separate_detections_by_category:
             print("Warning: I don't know how to separate categories yet when doing " + \
                   "a P/R analysis, disabling category separation")
@@ -872,15 +877,15 @@
 
 
     ##%% Load detection (and possibly classification) results
 
     # If the caller hasn't supplied results, load them
     if options.api_detection_results is None:
         detections_df, other_fields = load_api_results(
-            options.api_output_file, normalize_paths=True,
+            options.api_output_file, force_forward_slashes=True,
             filename_replacements=options.api_output_filename_replacements)
         ppresults.api_detection_results = detections_df
         ppresults.api_other_fields = other_fields        
 
     else:
         print('Bypassing detection results loading...')
         assert options.api_other_fields is not None
@@ -1083,15 +1088,15 @@
 
         precision_at_confidence_threshold = tp / (tp + fp)
         recall_at_confidence_threshold = tp / (tp + fn)
         f1 = 2.0 * (precision_at_confidence_threshold * recall_at_confidence_threshold) / \
             (precision_at_confidence_threshold + recall_at_confidence_threshold)
 
         print('At a confidence threshold of {:.1%}, precision={:.1%}, recall={:.1%}, f1={:.1%}'.format(
-                str(options.confidence_threshold), precision_at_confidence_threshold,
+                options.confidence_threshold, precision_at_confidence_threshold,
                 recall_at_confidence_threshold, f1))
 
         ##%% Collect classification results, if they exist
 
         classifier_accuracies = []
 
         # Mapping of classnames to idx for the confusion matrix.
@@ -1285,15 +1290,16 @@
                         classification_categories=classification_categories,
                         options=options), 
                 files_to_render), total=len(files_to_render)))
         else:
             for file_info in tqdm(files_to_render):
                 rendering_results.append(render_image_with_gt(
                     file_info,ground_truth_indexed_db,
-                    detection_categories,classification_categories))
+                    detection_categories,classification_categories,
+                    options=options))
         elapsed = time.time() - start_time
 
         # Map all the rendering results in the list rendering_results into the
         # dictionary images_html, which maps category names to lists of results
         image_rendered_count = 0
         for rendering_result in rendering_results:
             if rendering_result is None:
@@ -1315,53 +1321,59 @@
            &nbsp;&nbsp;&nbsp;&nbsp;<a href="tpi.html">with one or more incorrect top-1 prediction (TPI)</a> ({})<br/>
            &nbsp;&nbsp;&nbsp;&nbsp;<a href="tp.html">without classification evaluation</a><sup>*</sup> ({})<br/>""".format(
             image_counts['tpc'],
             image_counts['tpi'],
             image_counts['tp']
         )
 
+        confidence_threshold_string = ''
+        if isinstance(options.confidence_threshold,float):
+            confidence_threshold_string = '{:.2%}'.format(options.confidence_threshold)
+        else:
+            confidence_threshold_string = str(options.confidence_threshold)
+        
         index_page = """<html>
         {}
         <body>
         <h2>Evaluation</h2>
 
         <h3>Job metadata</h3>
         
         <div class="contentdiv">
         <p>Job name: {}<br/>
         <p>Model version: {}</p>
         </div>
         
         <h3>Sample images</h3>
         <div class="contentdiv">
-        <p>A sample of {} images, annotated with detections above {:.1%} confidence.</p>
+        <p>A sample of {} images, annotated with detections above confidence {}.</p>
         <a href="tp.html">True positives (TP)</a> ({}) ({:0.1%})<br/>
         CLASSIFICATION_PLACEHOLDER_1
         <a href="tn.html">True negatives (TN)</a> ({}) ({:0.1%})<br/>
         <a href="fp.html">False positives (FP)</a> ({}) ({:0.1%})<br/>
         <a href="fn.html">False negatives (FN)</a> ({}) ({:0.1%})<br/>
         CLASSIFICATION_PLACEHOLDER_2
         </div>
         """.format(
             style_header,job_name_string,model_version_string,
-            image_count, str(options.confidence_threshold),
+            image_count, confidence_threshold_string,
             all_tp_count, all_tp_count/total_count,
             image_counts['tn'], image_counts['tn']/total_count,
             image_counts['fp'], image_counts['fp']/total_count,
             image_counts['fn'], image_counts['fn']/total_count
         )
 
         index_page += """
             <h3>Detection results</h3>
             <div class="contentdiv">
-            <p>At a confidence threshold of {:0.1%}, precision={:0.1%}, recall={:0.1%}</p>
+            <p>At a confidence threshold of {}, precision={:0.1%}, recall={:0.1%}</p>
             <p><strong>Precision/recall summary for all {} images</strong></p><img src="{}"><br/>
             </div>
             """.format(
-                str(options.confidence_threshold), precision_at_confidence_threshold, recall_at_confidence_threshold,
+                confidence_threshold_string, precision_at_confidence_threshold, recall_at_confidence_threshold,
                 len(detections_df), pr_figure_relative_filename
            )
 
         if len(classifier_accuracies) > 0:
             index_page = index_page.replace('CLASSIFICATION_PLACEHOLDER_1',classification_detection_results)
             index_page = index_page.replace('CLASSIFICATION_PLACEHOLDER_2',"""<p><sup>*</sup>We do not evaluate the classification result of images
                 if the classification information is missing, if the image contains
@@ -1585,15 +1597,15 @@
         almost_detection_string = ''
         if options.include_almost_detections:
             almost_detection_string = ' (&ldquo;almost detection&rdquo; threshold at {:.1%})'.format(
                 options.almost_detection_confidence_threshold)
 
         confidence_threshold_string = ''
         if isinstance(options.confidence_threshold,float):
-            confidence_threshold_string = '{:.1%}'.format(options.confidence_threshold)
+            confidence_threshold_string = '{:.2%}'.format(options.confidence_threshold)
         else:
             confidence_threshold_string = str(options.confidence_threshold)
             
         index_page = """<html>\n{}\n<body>\n
         <h2>Visualization of results for {}</h2>\n
         <p>A sample of {} images (of {} total)FAILURE_PLACEHOLDER, annotated with detections above confidence {}{}.</p>\n
```

### Comparing `megadetector-5.0.7/api/batch_processing/postprocessing/render_detection_confusion_matrix.py` & `megadetector-5.0.8/api/batch_processing/postprocessing/render_detection_confusion_matrix.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,21 +52,21 @@
     force_render_images = render_image_constants['force_render_images']
     results_category_id_to_name = render_image_constants['results_category_id_to_name']
     rendering_confidence_thresholds = render_image_constants['rendering_confidence_thresholds']
     target_image_size = render_image_constants['target_image_size']
     
     assert im['file'] in filename_to_ground_truth_im
     
-    input_file = os.path.join(image_folder,im['file'])
-    assert os.path.isfile(input_file)
-                          
     output_file = image_to_output_file(im,preview_images_folder)
     if os.path.isfile(output_file) and not force_render_images:
         return output_file
     
+    input_file = os.path.join(image_folder,im['file'])
+    assert os.path.isfile(input_file)
+                          
     detections_to_render = []
     
     for det in im['detections']:
         category_name = results_category_id_to_name[det['category']]
         detection_threshold = rendering_confidence_thresholds['default']
         if category_name in rendering_confidence_thresholds:
             detection_threshold = rendering_confidence_thresholds[category_name]
@@ -78,16 +78,20 @@
                                           label_font_size=20,target_size=target_image_size)
     
     return output_file
 
 
 #%% Main function
 
-def render_detection_confusion_matrix(ground_truth_file,results_file,image_folder,preview_folder,
-                                      force_render_images=False, confidence_thresholds=None,
+def render_detection_confusion_matrix(ground_truth_file,
+                                      results_file,
+                                      image_folder,
+                                      preview_folder,
+                                      force_render_images=False, 
+                                      confidence_thresholds=None,
                                       rendering_confidence_thresholds=None,
                                       target_image_size=(1280,-1),
                                       parallelize_rendering=True,
                                       parallelize_rendering_n_cores=None,
                                       parallelize_rendering_with_threads=False,
                                       job_name='unknown',
                                       model_file=None,
@@ -219,15 +223,15 @@
     
     
     #%% Map images to predicted categories, and vice-versa
     
     filename_to_predicted_categories = defaultdict(set)
     predicted_category_name_to_filenames = defaultdict(set)
     
-    # im = md_results['images'][0]
+    # im = md_formatted_results['images'][0]
     for im in tqdm(md_formatted_results['images']):
         
         assert im['file'] in filename_to_ground_truth_im
         
         # det = im['detections'][0]
         for det in im['detections']:
             category_name = results_category_id_to_name[det['category']]
@@ -243,17 +247,14 @@
     # ...for each image
     
     
     #%% Create TP/TN/FP/FN lists
     
     category_name_to_image_lists = {}
     
-    # These may not be identical; currently the ground truth contains an "unknown" category
-    # results_category_names = sorted(list(results_category_id_to_name.values()))
-    
     sub_page_tokens = ['fn','tn','fp','tp']
     
     for category_name in ground_truth_category_names:
         
         category_name_to_image_lists[category_name] = {}
         for sub_page_token in sub_page_tokens:
             category_name_to_image_lists[category_name][sub_page_token] = []
@@ -292,15 +293,15 @@
                 else:
                     if category_name in predicted_categories_this_image:
                         assignment = 'fp'
                     else:
                         assignment = 'tn'        
                             
             category_name_to_image_lists[category_name][assignment].append(filename)
-            
+                        
     # ...for each filename
     
     
     #%% Create confusion matrix
     
     gt_category_name_to_category_index = {}
     
@@ -329,16 +330,16 @@
         if len(results_im['detections']) == 0:
             predicted_category_name = empty_category_name
         # Otherwise look for above-threshold detections
         else:            
             results_category_name_to_confidence = defaultdict(int)
             for det in results_im['detections']:
                 category_name = results_category_id_to_name[det['category']]
-                detection_threshold = rendering_confidence_thresholds['default']
-                if category_name in rendering_confidence_thresholds:
+                detection_threshold = confidence_thresholds['default']
+                if category_name in confidence_thresholds:
                     detection_threshold = confidence_thresholds[category_name]
                 if det['conf'] > detection_threshold:
                     results_category_name_to_confidence[category_name] = max(
                         results_category_name_to_confidence[category_name],det['conf'])
                 # If there were no detections above threshold
                 if len(results_category_name_to_confidence) == 0:
                     predicted_category_name = empty_category_name
@@ -350,14 +351,16 @@
         predicted_category_index = gt_category_name_to_category_index[predicted_category_name]
         
         true_predicted_token = ground_truth_category_name + '_' + predicted_category_name
         true_predicted_to_file_list[true_predicted_token].append(filename)
         
         confusion_matrix[ground_truth_category_index,predicted_category_index] += 1
     
+    # ...for each file
+    
     plt.ioff()    
     
     fig_h = 3 + 0.3 * n_categories
     fig_w = fig_h
     fig = plt.figure(figsize=(fig_w, fig_h),tight_layout=True)
         
     plot_utils.plot_confusion_matrix(
```

### Comparing `megadetector-5.0.7/api/batch_processing/postprocessing/repeat_detection_elimination/find_repeat_detections.py` & `megadetector-5.0.8/api/batch_processing/postprocessing/repeat_detection_elimination/find_repeat_detections.py`

 * *Files identical despite different names*

### Comparing `megadetector-5.0.7/api/batch_processing/postprocessing/repeat_detection_elimination/remove_repeat_detections.py` & `megadetector-5.0.8/api/batch_processing/postprocessing/repeat_detection_elimination/remove_repeat_detections.py`

 * *Files identical despite different names*

### Comparing `megadetector-5.0.7/api/batch_processing/postprocessing/repeat_detection_elimination/repeat_detections_core.py` & `megadetector-5.0.8/api/batch_processing/postprocessing/repeat_detection_elimination/repeat_detections_core.py`

 * *Files 0% similar despite different names*

```diff
@@ -177,27 +177,27 @@
     # one the user is evaluating) in a light gray
     bRenderOtherDetections = False
     otherDetectionsThreshold = 0.2    
     otherDetectionsLineWidth = 1
     
     # Optionally show a grid that includes a sample image for the detection, plus
     # the top N additional detections
-    bRenderDetectionTiles = False
+    bRenderDetectionTiles = True
     
     # If this is None, we'll render at the width of the original image
     detectionTilesPrimaryImageWidth = None
     
     # Can be a width in pixels, or a number from 0 to 1 representing a fraction
     # of the primary image width.
     #
     # If you want to render the grid at exactly 1 pixel wide, I guess you're out
     # of luck.
     detectionTilesCroppedGridWidth = 0.6
     detectionTilesPrimaryImageLocation='right'
-    detectionTilesMaxCrops = None
+    detectionTilesMaxCrops = 250
     
     # If bRenderOtherDetections is True, what color should we use to render the
     # (hopefully pretty subtle) non-target detections?
     # 
     # In theory I'd like these "other detection" rectangles to be partially 
     # transparent, but this is not straightforward, and the alpha is ignored
     # here.  But maybe if I leave it here and wish hard enough, someday it
```

### Comparing `megadetector-5.0.7/api/batch_processing/postprocessing/separate_detections_into_folders.py` & `megadetector-5.0.8/api/batch_processing/postprocessing/separate_detections_into_folders.py`

 * *Files identical despite different names*

### Comparing `megadetector-5.0.7/api/batch_processing/postprocessing/subset_json_detector_output.py` & `megadetector-5.0.8/api/batch_processing/postprocessing/subset_json_detector_output.py`

 * *Files identical despite different names*

### Comparing `megadetector-5.0.7/api/batch_processing/postprocessing/top_folders_to_bottom.py` & `megadetector-5.0.8/api/batch_processing/postprocessing/top_folders_to_bottom.py`

 * *Files identical despite different names*

### Comparing `megadetector-5.0.7/api/synchronous/api_core/animal_detection_api/api_backend.py` & `megadetector-5.0.8/api/synchronous/api_core/animal_detection_api/api_backend.py`

 * *Files identical despite different names*

### Comparing `megadetector-5.0.7/api/synchronous/api_core/animal_detection_api/api_frontend.py` & `megadetector-5.0.8/api/synchronous/api_core/animal_detection_api/api_frontend.py`

 * *Files identical despite different names*

### Comparing `megadetector-5.0.7/api/synchronous/api_core/animal_detection_api/config.py` & `megadetector-5.0.8/api/synchronous/api_core/animal_detection_api/config.py`

 * *Files identical despite different names*

### Comparing `megadetector-5.0.7/api/synchronous/api_core/animal_detection_api/data_management/annotations/annotation_constants.py` & `megadetector-5.0.8/api/synchronous/api_core/animal_detection_api/data_management/annotations/annotation_constants.py`

 * *Files identical despite different names*

### Comparing `megadetector-5.0.7/api/synchronous/api_core/animal_detection_api/detection/detector_training/copy_checkpoints.py` & `megadetector-5.0.8/api/synchronous/api_core/animal_detection_api/detection/detector_training/copy_checkpoints.py`

 * *Files identical despite different names*

### Comparing `megadetector-5.0.7/api/synchronous/api_core/animal_detection_api/detection/detector_training/model_main_tf2.py` & `megadetector-5.0.8/api/synchronous/api_core/animal_detection_api/detection/detector_training/model_main_tf2.py`

 * *Files identical despite different names*

### Comparing `megadetector-5.0.7/api/synchronous/api_core/animal_detection_api/detection/process_video.py` & `megadetector-5.0.8/api/synchronous/api_core/animal_detection_api/detection/process_video.py`

 * *Files identical despite different names*

### Comparing `megadetector-5.0.7/api/synchronous/api_core/animal_detection_api/detection/pytorch_detector.py` & `megadetector-5.0.8/api/synchronous/api_core/animal_detection_api/detection/pytorch_detector.py`

 * *Files identical despite different names*

### Comparing `megadetector-5.0.7/api/synchronous/api_core/animal_detection_api/detection/run_detector.py` & `megadetector-5.0.8/api/synchronous/api_core/animal_detection_api/detection/run_detector.py`

 * *Files identical despite different names*

### Comparing `megadetector-5.0.7/api/synchronous/api_core/animal_detection_api/detection/run_detector_batch.py` & `megadetector-5.0.8/api/synchronous/api_core/animal_detection_api/detection/run_detector_batch.py`

 * *Files identical despite different names*

### Comparing `megadetector-5.0.7/api/synchronous/api_core/animal_detection_api/detection/run_inference_with_yolov5_val.py` & `megadetector-5.0.8/api/synchronous/api_core/animal_detection_api/detection/run_inference_with_yolov5_val.py`

 * *Files identical despite different names*

### Comparing `megadetector-5.0.7/api/synchronous/api_core/animal_detection_api/detection/run_tiled_inference.py` & `megadetector-5.0.8/api/synchronous/api_core/animal_detection_api/detection/run_tiled_inference.py`

 * *Files identical despite different names*

### Comparing `megadetector-5.0.7/api/synchronous/api_core/animal_detection_api/detection/tf_detector.py` & `megadetector-5.0.8/api/synchronous/api_core/animal_detection_api/detection/tf_detector.py`

 * *Files identical despite different names*

### Comparing `megadetector-5.0.7/api/synchronous/api_core/animal_detection_api/detection/video_utils.py` & `megadetector-5.0.8/api/synchronous/api_core/animal_detection_api/detection/video_utils.py`

 * *Files identical despite different names*

### Comparing `megadetector-5.0.7/api/synchronous/api_core/animal_detection_api/md_utils/azure_utils.py` & `megadetector-5.0.8/api/synchronous/api_core/animal_detection_api/md_utils/azure_utils.py`

 * *Files identical despite different names*

### Comparing `megadetector-5.0.7/api/synchronous/api_core/animal_detection_api/md_utils/ct_utils.py` & `megadetector-5.0.8/api/synchronous/api_core/animal_detection_api/md_utils/ct_utils.py`

 * *Files identical despite different names*

### Comparing `megadetector-5.0.7/api/synchronous/api_core/animal_detection_api/md_utils/directory_listing.py` & `megadetector-5.0.8/api/synchronous/api_core/animal_detection_api/md_utils/directory_listing.py`

 * *Files identical despite different names*

### Comparing `megadetector-5.0.7/api/synchronous/api_core/animal_detection_api/md_utils/matlab_porting_tools.py` & `megadetector-5.0.8/api/synchronous/api_core/animal_detection_api/md_utils/matlab_porting_tools.py`

 * *Files identical despite different names*

### Comparing `megadetector-5.0.7/api/synchronous/api_core/animal_detection_api/md_utils/path_utils.py` & `megadetector-5.0.8/api/synchronous/api_core/animal_detection_api/md_utils/path_utils.py`

 * *Files identical despite different names*

### Comparing `megadetector-5.0.7/api/synchronous/api_core/animal_detection_api/md_utils/process_utils.py` & `megadetector-5.0.8/api/synchronous/api_core/animal_detection_api/md_utils/process_utils.py`

 * *Files identical despite different names*

### Comparing `megadetector-5.0.7/api/synchronous/api_core/animal_detection_api/md_utils/sas_blob_utils.py` & `megadetector-5.0.8/api/synchronous/api_core/animal_detection_api/md_utils/sas_blob_utils.py`

 * *Files identical despite different names*

### Comparing `megadetector-5.0.7/api/synchronous/api_core/animal_detection_api/md_utils/string_utils.py` & `megadetector-5.0.8/api/synchronous/api_core/animal_detection_api/md_utils/string_utils.py`

 * *Files identical despite different names*

### Comparing `megadetector-5.0.7/api/synchronous/api_core/animal_detection_api/md_utils/url_utils.py` & `megadetector-5.0.8/api/synchronous/api_core/animal_detection_api/md_utils/url_utils.py`

 * *Files identical despite different names*

### Comparing `megadetector-5.0.7/api/synchronous/api_core/animal_detection_api/md_utils/write_html_image_list.py` & `megadetector-5.0.8/api/synchronous/api_core/animal_detection_api/md_utils/write_html_image_list.py`

 * *Files identical despite different names*

### Comparing `megadetector-5.0.7/api/synchronous/api_core/animal_detection_api/md_visualization/visualization_utils.py` & `megadetector-5.0.8/api/synchronous/api_core/animal_detection_api/md_visualization/visualization_utils.py`

 * *Files identical despite different names*

### Comparing `megadetector-5.0.7/api/synchronous/api_core/tests/load_test.py` & `megadetector-5.0.8/api/synchronous/api_core/tests/load_test.py`

 * *Files identical despite different names*

### Comparing `megadetector-5.0.7/classification/aggregate_classifier_probs.py` & `megadetector-5.0.8/classification/aggregate_classifier_probs.py`

 * *Files identical despite different names*

### Comparing `megadetector-5.0.7/classification/analyze_failed_images.py` & `megadetector-5.0.8/classification/analyze_failed_images.py`

 * *Files identical despite different names*

### Comparing `megadetector-5.0.7/classification/cache_batchapi_outputs.py` & `megadetector-5.0.8/classification/cache_batchapi_outputs.py`

 * *Files identical despite different names*

### Comparing `megadetector-5.0.7/classification/create_classification_dataset.py` & `megadetector-5.0.8/classification/create_classification_dataset.py`

 * *Files identical despite different names*

### Comparing `megadetector-5.0.7/classification/crop_detections.py` & `megadetector-5.0.8/classification/crop_detections.py`

 * *Files identical despite different names*

### Comparing `megadetector-5.0.7/classification/csv_to_json.py` & `megadetector-5.0.8/classification/csv_to_json.py`

 * *Files identical despite different names*

### Comparing `megadetector-5.0.7/classification/detect_and_crop.py` & `megadetector-5.0.8/classification/detect_and_crop.py`

 * *Files identical despite different names*

### Comparing `megadetector-5.0.7/classification/efficientnet/model.py` & `megadetector-5.0.8/classification/efficientnet/model.py`

 * *Files identical despite different names*

### Comparing `megadetector-5.0.7/classification/efficientnet/utils.py` & `megadetector-5.0.8/classification/efficientnet/utils.py`

 * *Files identical despite different names*

### Comparing `megadetector-5.0.7/classification/evaluate_model.py` & `megadetector-5.0.8/classification/evaluate_model.py`

 * *Files identical despite different names*

### Comparing `megadetector-5.0.7/classification/identify_mislabeled_candidates.py` & `megadetector-5.0.8/classification/identify_mislabeled_candidates.py`

 * *Files identical despite different names*

### Comparing `megadetector-5.0.7/classification/json_to_azcopy_list.py` & `megadetector-5.0.8/classification/json_to_azcopy_list.py`

 * *Files identical despite different names*

### Comparing `megadetector-5.0.7/classification/json_validator.py` & `megadetector-5.0.8/classification/json_validator.py`

 * *Files identical despite different names*

### Comparing `megadetector-5.0.7/classification/map_classification_categories.py` & `megadetector-5.0.8/classification/map_classification_categories.py`

 * *Files identical despite different names*

### Comparing `megadetector-5.0.7/classification/merge_classification_detection_output.py` & `megadetector-5.0.8/classification/merge_classification_detection_output.py`

 * *Files identical despite different names*

### Comparing `megadetector-5.0.7/classification/prepare_classification_script.py` & `megadetector-5.0.8/classification/prepare_classification_script.py`

 * *Files identical despite different names*

### Comparing `megadetector-5.0.7/classification/prepare_classification_script_mc.py` & `megadetector-5.0.8/classification/prepare_classification_script_mc.py`

 * *Files identical despite different names*

### Comparing `megadetector-5.0.7/classification/run_classifier.py` & `megadetector-5.0.8/classification/run_classifier.py`

 * *Files identical despite different names*

### Comparing `megadetector-5.0.7/classification/save_mislabeled.py` & `megadetector-5.0.8/classification/save_mislabeled.py`

 * *Files identical despite different names*

### Comparing `megadetector-5.0.7/classification/train_classifier.py` & `megadetector-5.0.8/classification/train_classifier.py`

 * *Files identical despite different names*

### Comparing `megadetector-5.0.7/classification/train_classifier_tf.py` & `megadetector-5.0.8/classification/train_classifier_tf.py`

 * *Files identical despite different names*

### Comparing `megadetector-5.0.7/classification/train_utils.py` & `megadetector-5.0.8/classification/train_utils.py`

 * *Files identical despite different names*

### Comparing `megadetector-5.0.7/data_management/annotations/annotation_constants.py` & `megadetector-5.0.8/data_management/annotations/annotation_constants.py`

 * *Files identical despite different names*

### Comparing `megadetector-5.0.7/data_management/cct_json_to_filename_json.py` & `megadetector-5.0.8/data_management/cct_json_to_filename_json.py`

 * *Files identical despite different names*

### Comparing `megadetector-5.0.7/data_management/cct_json_utils.py` & `megadetector-5.0.8/data_management/cct_json_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -138,15 +138,16 @@
     Handles boilerplate dictionary creation that we do almost every time we load
     a .json database.
     """
 
     def __init__(self, json_filename: Union[str, JSONObject],
                  b_normalize_paths: bool = False,
                  filename_replacements: Optional[Mapping[str, str]] = None,
-                 b_convert_classes_to_lower: bool = True):
+                 b_convert_classes_to_lower: bool = True,
+                 b_force_forward_slashes: bool = True):
         """
         json_filename can also be an existing json db
         """
         
         if isinstance(json_filename, str):
             with open(json_filename) as f:
                 self.db = json.load(f)
@@ -158,19 +159,23 @@
             'this is a COCO camera traps file?')
         
         if b_convert_classes_to_lower:
             # Convert classnames to lowercase to simplify comparisons later
             for c in self.db['categories']:
                 c['name'] = c['name'].lower()
 
+        # Normalize paths to simplify comparisons later
         if b_normalize_paths:
-            # Normalize paths to simplify comparisons later
             for im in self.db['images']:
                 im['file_name'] = os.path.normpath(im['file_name'])
 
+        if b_force_forward_slashes:
+            for im in self.db['images']:
+                im['file_name'] = im['file_name'].replace('\\','/')
+
         if filename_replacements is not None:
             for s in filename_replacements:
                 # Make custom replacements in filenames, typically used to
                 # accommodate changes in root paths after DB construction
                 r = filename_replacements[s]
                 for im in self.db['images']:
                     im['file_name'] = im['file_name'].replace(s, r)
```

### Comparing `megadetector-5.0.7/data_management/cct_to_csv.py` & `megadetector-5.0.8/data_management/cct_to_csv.py`

 * *Files identical despite different names*

### Comparing `megadetector-5.0.7/data_management/cct_to_md.py` & `megadetector-5.0.8/data_management/cct_to_md.py`

 * *Files identical despite different names*

### Comparing `megadetector-5.0.7/data_management/cct_to_wi.py` & `megadetector-5.0.8/data_management/cct_to_wi.py`

 * *Files identical despite different names*

### Comparing `megadetector-5.0.7/data_management/coco_to_yolo.py` & `megadetector-5.0.8/data_management/coco_to_yolo.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,14 +52,18 @@
     # Read class names
     if isinstance(class_list,str):
         with open(class_list,'r') as f:
             class_lines = f.readlines()
         class_lines = [s.strip() for s in class_lines]    
         class_list = [s for s in class_lines if len(s) > 0]
 
+    if not (yolo_dataset_file.endswith('.yml') or yolo_dataset_file.endswith('.yaml')):
+        print('Warning: writing dataset file to a non-yml/yaml extension:\n{}'.format(
+            yolo_dataset_file))
+        
     # Write dataset.yaml
     with open(yolo_dataset_file,'w') as f:
         
         f.write('# Train/val sets\n')
         f.write('path: {}\n'.format(dataset_base_dir))
         if train_folder_relative is not None:
             f.write('train: {}\n'.format(train_folder_relative))
@@ -185,15 +189,14 @@
     # Note: this allows unused categories in the output data set.  This is OK for
     # some training pipelines, not for others.
     next_category_id = 0
     coco_id_to_yolo_id = {}    
     coco_id_to_name = {}
     yolo_id_to_name = {}
     coco_category_ids_to_exclude = set()
-    category_exclusion_warnings_printed = set()
     
     for category in data['categories']:
         coco_id_to_name[category['id']] = category['name']
         if (category_names_to_include is not None) and \
             (category['name'] not in category_names_to_include):
             coco_category_ids_to_exclude.add(category['id'])
             continue
@@ -461,17 +464,17 @@
             bboxes = output_info['bboxes']        
             
             # Only write an annotation file if there are bounding boxes.  Images with 
             # no .txt files are treated as hard negatives, at least by YOLOv5:
             #
             # https://github.com/ultralytics/yolov5/issues/3218
             #
-            # I think this is also true for images with empty annotation files, but 
-            # I'm using the convention suggested on that issue, i.e. hard negatives 
-            # are expressed as images without .txt files.
+            # I think this is also true for images with empty .txt files, but 
+            # I'm using the convention suggested on that issue, i.e. hard 
+            # negatives are expressed as images without .txt files.
             if len(bboxes) > 0:
                 
                 with open(dest_txt,'w') as f:
                     
                     # bbox = bboxes[0]
                     for bbox in bboxes:
                         assert len(bbox) == 5
```

### Comparing `megadetector-5.0.7/data_management/databases/add_width_and_height_to_db.py` & `megadetector-5.0.8/data_management/databases/add_width_and_height_to_db.py`

 * *Files identical despite different names*

### Comparing `megadetector-5.0.7/data_management/databases/combine_coco_camera_traps_files.py` & `megadetector-5.0.8/data_management/databases/combine_coco_camera_traps_files.py`

 * *Files identical despite different names*

### Comparing `megadetector-5.0.7/data_management/databases/integrity_check_json_db.py` & `megadetector-5.0.8/data_management/databases/integrity_check_json_db.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,31 +20,33 @@
 import argparse
 import json
 import os
 import sys
 
 from multiprocessing.pool import ThreadPool
 from operator import itemgetter
-from PIL import Image
 from tqdm import tqdm
 
+from md_visualization.visualization_utils import open_image
 from md_utils import ct_utils
 
 
 #%% Classes and environment
 
 class IntegrityCheckOptions:
     
     baseDir = ''
     bCheckImageSizes = False
     bCheckImageExistence = False
     bFindUnusedImages = False
     bRequireLocation = True
     iMaxNumImages = -1
     nThreads = 10
+    verbose = True
+    
     
 # This is used in a medium-hacky way to share modified options across threads
 defaultOptions = IntegrityCheckOptions()
 
 
 #%% Functions
 
@@ -61,15 +63,17 @@
         return False
     
     if options.bCheckImageSizes:
         if not ('height' in image and 'width' in image):
             print('Missing image size in {}'.format(filePath))
             return False
 
-        width, height = Image.open(filePath).size
+        # width, height = Image.open(filePath).size
+        pil_im = open_image(filePath)
+        width,height = pil_im.size
         if (not (width == image['width'] and height == image['height'])):
             print('Size mismatch for image {}: {} (reported {},{}, actual {},{})'.format(
                     image['id'], filePath, image['width'], image['height'], width, height))
             return False
         
     return True
 
@@ -82,16 +86,17 @@
     """
     
     if options is None:       
         options = IntegrityCheckOptions()
     
     if options.bCheckImageSizes:        
         options.bCheckImageExistence = True
-        
-    print(options.__dict__)
+     
+    if options.verbose:
+        print(options.__dict__)
     
     if options.baseDir is None:
         options.baseDir = ''
         
     baseDir = options.baseDir
     
     
@@ -101,16 +106,17 @@
         
         data = jsonFile
         
     elif isinstance(jsonFile,str):
         
         assert os.path.isfile(jsonFile), '.json file {} does not exist'.format(jsonFile)
     
-        print('Reading .json {} with base dir [{}]...'.format(
-                jsonFile,baseDir))
+        if options.verbose:
+            print('Reading .json {} with base dir [{}]...'.format(
+                    jsonFile,baseDir))
         
         with open(jsonFile,'r') as f:
             data = json.load(f) 
             
     else:
         
         raise ValueError('Illegal value for jsonFile')
@@ -129,15 +135,16 @@
     
     imageIdToImage = {}
     annIdToAnn = {}
     catIdToCat = {}
     catNameToCat = {}
     imageLocationSet = set()
     
-    print('Checking categories...')
+    if options.verbose:
+        print('Checking categories...')
     
     for cat in tqdm(categories):
         
         # Confirm that required fields are present
         assert 'name' in cat
         assert 'id' in cat
         
@@ -153,19 +160,21 @@
         cat['_count'] = 0
         
         assert catName not in catNameToCat, 'Category name {} is used more than once'.format(catName)
         catNameToCat[catName] = cat        
         
     # ...for each category
         
-    print('\nChecking images...')
+    if options.verbose:
+        print('\nChecking images...')
     
     if options.iMaxNumImages > 0 and len(images) > options.iMaxNumImages:
         
-        print('Trimming image list to {}'.format(options.iMaxNumImages))
+        if options.verbose:
+            print('Trimming image list to {}'.format(options.iMaxNumImages))
         images = images[0:options.iMaxNumImages]
         
     imagePathsInJson = set()
     
     sequences = set()
     
     # image = images[0]
@@ -213,15 +222,16 @@
         assert not ('sequence_id' in image or 'sequence' in image), 'Illegal sequence identifier'
         
     unusedFiles = []
                 
     # Are we checking for unused images?
     if (len(baseDir) > 0) and options.bFindUnusedImages:    
         
-        print('\nEnumerating images...')
+        if options.verbose:
+            print('\nEnumerating images...')
         
         # Recursively enumerate images
         imagePaths = []
         for root, dirs, files in os.walk(baseDir):
             for file in files:
                 if file.lower().endswith(('.jpeg', '.jpg', '.png')):
                     relDir = os.path.relpath(root, baseDir)
@@ -240,16 +250,17 @@
     validationErrors = []
     
     # Are we checking file existence and/or image size?
     if options.bCheckImageSizes or options.bCheckImageExistence:
         
         if len(baseDir) == 0:
             print('Warning: checking image sizes without a base directory, assuming "."')
-            
-        print('Checking image existence and/or image sizes...')
+         
+        if options.verbose:
+            print('Checking image existence and/or image sizes...')
         
         if options.nThreads is not None and options.nThreads > 1:
             pool = ThreadPool(options.nThreads)
             # results = pool.imap_unordered(lambda x: fetch_url(x,nImages), indexedUrlList)
             defaultOptions.baseDir = options.baseDir
             defaultOptions.bCheckImageSizes = options.bCheckImageSizes
             defaultOptions.bCheckImageExistence = options.bCheckImageExistence
@@ -261,17 +272,17 @@
                 
         for iImage,r in enumerate(results):
             if not r:            
                 validationErrors.append(os.path.join(options.baseDir,images[iImage]['file_name']))
                             
     # ...for each image
     
-    print('{} validation errors (of {})'.format(len(validationErrors),len(images)))
-                                                
-    print('Checking annotations...')
+    if options.verbose:
+        print('{} validation errors (of {})'.format(len(validationErrors),len(images)))
+        print('Checking annotations...')
     
     nBoxes = 0
     
     for ann in tqdm(annotations):
     
         # Confirm that required fields are present
         assert 'image_id' in ann
@@ -298,66 +309,64 @@
           'Image ID {} referred to by annotation {}, not available'.format(
             ann['image_id'],ann['id'])
     
         imageIdToImage[ann['image_id']]['_count'] += 1
         catIdToCat[ann['category_id']]['_count'] +=1 
         
     # ...for each annotation
-        
-        
-    ##%% Print statistics
     
-    # Find un-annotated images and multi-annotation images
-    nUnannotated = 0
-    nMultiAnnotated = 0
-    
-    for image in images:
-        if image['_count'] == 0:
-            nUnannotated += 1
-        elif image['_count'] > 1:
-            nMultiAnnotated += 1
-            
-    print('Found {} unannotated images, {} images with multiple annotations'.format(
-            nUnannotated,nMultiAnnotated))
-    
-    if (len(baseDir) > 0) and options.bFindUnusedImages:
-        print('Found {} unused image files'.format(len(unusedFiles)))
-        
-    nUnusedCategories = 0
-    
-    # Find unused categories
-    for cat in categories:
-        if cat['_count'] == 0:
-            print('Unused category: {}'.format(cat['name']))
-            nUnusedCategories += 1
+    sortedCategories = sorted(categories, key=itemgetter('_count'), reverse=True)
     
-    print('Found {} unused categories'.format(nUnusedCategories))
-            
-    sequenceString = 'no sequence info'
-    if len(sequences) > 0:
-        sequenceString = '{} sequences'.format(len(sequences))
-        
-    print('\nDB contains {} images, {} annotations, {} bboxes, {} categories, {}\n'.format(
-            len(images),len(annotations),nBoxes,len(categories),sequenceString))
-
-    if len(imageLocationSet) > 0:
-        print('DB contains images from {} locations\n'.format(len(imageLocationSet)))
-    
-    # Prints a list of categories sorted by count
-    #
-    # https://stackoverflow.com/questions/72899/how-do-i-sort-a-list-of-dictionaries-by-a-value-of-the-dictionary
     
-    sortedCategories = sorted(categories, key=itemgetter('_count'), reverse=True)
+    ##%% Print statistics
     
-    print('Categories and annotation (not image) counts:\n')
+    if options.verbose:
     
-    for cat in sortedCategories:
-        print('{:6} {}'.format(cat['_count'],cat['name']))
+        # Find un-annotated images and multi-annotation images
+        nUnannotated = 0
+        nMultiAnnotated = 0
+        
+        for image in images:
+            if image['_count'] == 0:
+                nUnannotated += 1
+            elif image['_count'] > 1:
+                nMultiAnnotated += 1
+                
+        print('Found {} unannotated images, {} images with multiple annotations'.format(
+                nUnannotated,nMultiAnnotated))
+        
+        if (len(baseDir) > 0) and options.bFindUnusedImages:
+            print('Found {} unused image files'.format(len(unusedFiles)))
+            
+        nUnusedCategories = 0
+        
+        # Find unused categories
+        for cat in categories:
+            if cat['_count'] == 0:
+                print('Unused category: {}'.format(cat['name']))
+                nUnusedCategories += 1
+        
+        print('Found {} unused categories'.format(nUnusedCategories))
+                
+        sequenceString = 'no sequence info'
+        if len(sequences) > 0:
+            sequenceString = '{} sequences'.format(len(sequences))
+            
+        print('\nDB contains {} images, {} annotations, {} bboxes, {} categories, {}\n'.format(
+                len(images),len(annotations),nBoxes,len(categories),sequenceString))
     
-    print('')
+        if len(imageLocationSet) > 0:
+            print('DB contains images from {} locations\n'.format(len(imageLocationSet)))
+                
+        print('Categories and annotation (not image) counts:\n')
+        
+        for cat in sortedCategories:
+            print('{:6} {}'.format(cat['_count'],cat['name']))
+        
+        print('')
     
     errorInfo = {}
     errorInfo['unusedFiles'] = unusedFiles
     errorInfo['validationErrors'] = validationErrors
     
     return sortedCategories, data, errorInfo
```

### Comparing `megadetector-5.0.7/data_management/databases/remove_corrupted_images_from_db.py` & `megadetector-5.0.8/data_management/databases/remove_corrupted_images_from_db.py`

 * *Files identical despite different names*

### Comparing `megadetector-5.0.7/data_management/databases/subset_json_db.py` & `megadetector-5.0.8/data_management/databases/subset_json_db.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,15 +61,15 @@
     output_data = data
     output_data['images'] = images
     output_data['annotations'] = annotations
     
     # Write the output file if requested
     if output_json is not None:
         print('Writing output .json...')
-        json.dump(output_data,open(output_json,'w'),indent=4)
+        json.dump(output_data,open(output_json,'w'),indent=1)
         
     return output_data
 
 
 #%% Interactive driver
 
 if False:
```

### Comparing `megadetector-5.0.7/data_management/generate_crops_from_cct.py` & `megadetector-5.0.8/data_management/generate_crops_from_cct.py`

 * *Files identical despite different names*

### Comparing `megadetector-5.0.7/data_management/get_image_sizes.py` & `megadetector-5.0.8/data_management/get_image_sizes.py`

 * *Files 26% similar despite different names*

```diff
@@ -11,27 +11,33 @@
 
 import argparse
 import json
 import os
 from PIL import Image
 import sys
 
+from md_utils.path_utils import find_images
+
 from multiprocessing.pool import ThreadPool
 from multiprocessing.pool import Pool
 from functools import partial
 from tqdm import tqdm
 
 image_base = ''
 default_n_threads = 1
 use_threads = False
 
 
 #%% Processing functions
 
-def process_image(image_path,image_prefix=None):
+def _get_image_size(image_path,image_prefix=None):
+    """
+    Support function to get the size of a single image.  Returns a (path,w,h) tuple.
+    w and h will be -1 if the image fails to load.
+    """
     
     if image_prefix is not None:
         full_path = os.path.join(image_prefix,image_path)
     else:
         full_path = image_path
     
     # Is this image on disk?
@@ -45,51 +51,64 @@
         h = pil_im.height
         return (image_path,w,h)
     except Exception as e:    
         print('Error reading image {}: {}'.format(full_path,str(e)))
         return (image_path,-1,-1)
     
     
-def process_images(filenames,image_prefix=None,n_threads=default_n_threads):
+def get_image_sizes(filenames,image_prefix=None,output_file=None,
+                    n_workers=default_n_threads,use_threads=True,
+                    recursive=True):
+    """
+    Get the width and height of all images in [filenames], which can be:
+        
+    * A .json-formatted file 
+    * A folder
+    * A list of files
+
+    ...returning a list of (path,w,h) tuples, and optionally writing the results to [output_file].
+    """        
+    
+    if output_file is not None:
+        assert os.path.isdir(os.path.dirname(output_file)), \
+            'Illegal output file {}, parent folder does not exist'.format(output_file)
+        
+    if isinstance(filenames,str) and os.path.isfile(filenames):
+        with open(filenames,'r') as f:        
+            filenames = json.load(f)
+        filenames = [s.strip() for s in filenames]
+    elif isinstance(filenames,str) and os.path.isdir(filenames):
+        filenames = find_images(filenames,recursive=recursive,
+                                return_relative_paths=False,convert_slashes=True)
+    else:
+        assert isinstance(filenames,list)        
     
-    if n_threads <= 1:
+    if n_workers <= 1:
         
         all_results = []
         for i_file,fn in tqdm(enumerate(filenames),total=len(filenames)):
-            all_results.append(process_image(fn,image_prefix=image_prefix))
+            all_results.append(_get_image_size(fn,image_prefix=image_prefix))
     
     else:
         
-        print('Creating a pool with {} threads'.format(n_threads))
+        print('Creating a pool with {} workers'.format(n_workers))
         if use_threads:
-            pool = ThreadPool(n_threads)        
+            pool = ThreadPool(n_workers)        
         else:
-            pool = Pool(n_threads)
+            pool = Pool(n_workers)
         # all_results = list(tqdm(pool.imap(process_image, filenames), total=len(filenames)))
         all_results = list(tqdm(pool.imap(
-            partial(process_image,image_prefix=image_prefix), filenames), total=len(filenames)))
-                
-    return all_results
-
-
-def process_list_file(input_file,output_file=None,image_prefix=None,n_threads=default_n_threads):
-    
-    assert os.path.isdir(os.path.dirname(output_file))
-    assert os.path.isfile(input_file)
-    
-    with open(input_file,'r') as f:        
-        filenames = json.load(f)
-    filenames = [s.strip() for s in filenames]
-    
-    all_results = process_images(filenames,image_prefix=image_prefix,n_threads=n_threads)
+            partial(_get_image_size,image_prefix=image_prefix), filenames), total=len(filenames)))
     
     if output_file is not None:
         with open(output_file,'w') as f:
             json.dump(all_results,f,indent=1)
-    
+            
+    return all_results
+
     
 #%% Interactive driver
 
 if False:
 
     pass    
 
@@ -112,16 +131,15 @@
     
     with open(relative_image_list_file,'w') as f:
         json.dump(relative_image_names,f,indent=1)
     
     
     #%%
     
-    # process_list_file(image_list_file,image_size_file,image_prefix=base_dir)
-    process_list_file(relative_image_list_file,image_size_file,image_prefix=base_dir,n_threads=4)
+    get_image_sizes(relative_image_list_file,image_size_file,image_prefix=base_dir,n_threads=4)
     
     
 #%% Command-line driver
     
 def main():
     
     parser = argparse.ArgumentParser()
@@ -132,13 +150,13 @@
                         
     if len(sys.argv[1:])==0:
         parser.print_help()
         parser.exit()
         
     args = parser.parse_args()
     
-    process_list_file(args.input_file,args.output_file,args.image_prefix,args.n_threads)
+    _ = get_image_sizes(args.input_file,args.output_file,args.image_prefix,args.n_threads)
     
 
 if __name__ == '__main__':
     
     main()
```

### Comparing `megadetector-5.0.7/data_management/importers/add_nacti_sizes.py` & `megadetector-5.0.8/data_management/importers/add_nacti_sizes.py`

 * *Files identical despite different names*

### Comparing `megadetector-5.0.7/data_management/importers/add_timestamps_to_icct.py` & `megadetector-5.0.8/data_management/importers/add_timestamps_to_icct.py`

 * *Files identical despite different names*

### Comparing `megadetector-5.0.7/data_management/importers/animl_results_to_md_results.py` & `megadetector-5.0.8/data_management/importers/animl_results_to_md_results.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,16 +35,14 @@
 def animl_results_to_md_results(input_file,output_file=None):
     """
     Converts the .csv file [input_file] to the MD-formatted .json file [output_file].
     
     If [output_file] is None, '.json' will be appended to the input file.
     """
     
-    #%%
-    
     if output_file is None:
         output_file = input_file + '.json'
 
     df = pd.read_csv(input_file)
     
     expected_columns = ('file','category','detection_conf',
                         'bbox1','bbox2','bbox3','bbox4','class','classification_conf')
@@ -107,15 +105,15 @@
     results['classification_categories'] = \
         {v: k for k, v in classification_category_name_to_id.items()}
     results['images'] = list(filename_to_results.values())
     
     with open(output_file,'w') as f:
         json.dump(results,f,indent=1)
         
-# ...zamba_results_to_md_results(...)
+# ...animl_results_to_md_results(...)
         
 
 #%% Interactive driver
 
 if False:
 
     pass
```

### Comparing `megadetector-5.0.7/data_management/importers/auckland_doc_test_to_json.py` & `megadetector-5.0.8/data_management/importers/auckland_doc_test_to_json.py`

 * *Files identical despite different names*

### Comparing `megadetector-5.0.7/data_management/importers/auckland_doc_to_json.py` & `megadetector-5.0.8/data_management/importers/auckland_doc_to_json.py`

 * *Files identical despite different names*

### Comparing `megadetector-5.0.7/data_management/importers/awc_to_json.py` & `megadetector-5.0.8/data_management/importers/awc_to_json.py`

 * *Files identical despite different names*

### Comparing `megadetector-5.0.7/data_management/importers/bellevue_to_json.py` & `megadetector-5.0.8/data_management/importers/bellevue_to_json.py`

 * *Files identical despite different names*

### Comparing `megadetector-5.0.7/data_management/importers/cacophony-thermal-importer.py` & `megadetector-5.0.8/data_management/importers/cacophony-thermal-importer.py`

 * *Files identical despite different names*

### Comparing `megadetector-5.0.7/data_management/importers/carrizo_shrubfree_2018.py` & `megadetector-5.0.8/data_management/importers/carrizo_shrubfree_2018.py`

 * *Files identical despite different names*

### Comparing `megadetector-5.0.7/data_management/importers/carrizo_trail_cam_2017.py` & `megadetector-5.0.8/data_management/importers/carrizo_trail_cam_2017.py`

 * *Files identical despite different names*

### Comparing `megadetector-5.0.7/data_management/importers/cct_field_adjustments.py` & `megadetector-5.0.8/data_management/importers/cct_field_adjustments.py`

 * *Files identical despite different names*

### Comparing `megadetector-5.0.7/data_management/importers/channel_islands_to_cct.py` & `megadetector-5.0.8/data_management/importers/channel_islands_to_cct.py`

 * *Files identical despite different names*

### Comparing `megadetector-5.0.7/data_management/importers/eMammal/copy_and_unzip_emammal.py` & `megadetector-5.0.8/data_management/importers/eMammal/copy_and_unzip_emammal.py`

 * *Files identical despite different names*

### Comparing `megadetector-5.0.7/data_management/importers/eMammal/eMammal_helpers.py` & `megadetector-5.0.8/data_management/importers/eMammal/eMammal_helpers.py`

 * *Files identical despite different names*

### Comparing `megadetector-5.0.7/data_management/importers/eMammal/make_eMammal_json.py` & `megadetector-5.0.8/data_management/importers/eMammal/make_eMammal_json.py`

 * *Files identical despite different names*

### Comparing `megadetector-5.0.7/data_management/importers/ena24_to_json.py` & `megadetector-5.0.8/data_management/importers/ena24_to_json.py`

 * *Files identical despite different names*

### Comparing `megadetector-5.0.7/data_management/importers/filenames_to_json.py` & `megadetector-5.0.8/data_management/importers/filenames_to_json.py`

 * *Files identical despite different names*

### Comparing `megadetector-5.0.7/data_management/importers/helena_to_cct.py` & `megadetector-5.0.8/data_management/importers/helena_to_cct.py`

 * *Files identical despite different names*

### Comparing `megadetector-5.0.7/data_management/importers/idaho-camera-traps.py` & `megadetector-5.0.8/data_management/importers/idaho-camera-traps.py`

 * *Files identical despite different names*

### Comparing `megadetector-5.0.7/data_management/importers/idfg_iwildcam_lila_prep.py` & `megadetector-5.0.8/data_management/importers/idfg_iwildcam_lila_prep.py`

 * *Files identical despite different names*

### Comparing `megadetector-5.0.7/data_management/importers/jb_csv_to_json.py` & `megadetector-5.0.8/data_management/importers/jb_csv_to_json.py`

 * *Files identical despite different names*

### Comparing `megadetector-5.0.7/data_management/importers/mcgill_to_json.py` & `megadetector-5.0.8/data_management/importers/mcgill_to_json.py`

 * *Files identical despite different names*

### Comparing `megadetector-5.0.7/data_management/importers/missouri_to_json.py` & `megadetector-5.0.8/data_management/importers/missouri_to_json.py`

 * *Files identical despite different names*

### Comparing `megadetector-5.0.7/data_management/importers/nacti_fieldname_adjustments.py` & `megadetector-5.0.8/data_management/importers/nacti_fieldname_adjustments.py`

 * *Files identical despite different names*

### Comparing `megadetector-5.0.7/data_management/importers/noaa_seals_2019.py` & `megadetector-5.0.8/data_management/importers/noaa_seals_2019.py`

 * *Files 1% similar despite different names*

```diff
@@ -161,15 +161,15 @@
     assert box_top > box_bottom; assert box_right > box_left    
     ymin = box_bottom; ymax = box_top; xmin = box_left; xmax = box_right
 
     visualization_utils.draw_bounding_box_on_image(img_ir,ymin,xmin,ymax,xmax,
                                                    use_normalized_coordinates=False,
                                                    thickness=3)
 
-visualization_utils.show_images_in_a_row([img_rgb,img_ir])
+# visualization_utils.show_images_in_a_row([img_rgb,img_ir])
 
 
 #%% Save images
 
 img_rgb.save(r'c:\temp\seals_rgb.png')
 img_ir.save(r'c:\temp\seals_ir.png')
```

### Comparing `megadetector-5.0.7/data_management/importers/pc_to_json.py` & `megadetector-5.0.8/data_management/importers/pc_to_json.py`

 * *Files identical despite different names*

### Comparing `megadetector-5.0.7/data_management/importers/plot_wni_giraffes.py` & `megadetector-5.0.8/data_management/importers/plot_wni_giraffes.py`

 * *Files identical despite different names*

### Comparing `megadetector-5.0.7/data_management/importers/prepare-noaa-fish-data-for-lila.py` & `megadetector-5.0.8/data_management/importers/prepare-noaa-fish-data-for-lila.py`

 * *Files identical despite different names*

### Comparing `megadetector-5.0.7/data_management/importers/prepare_zsl_imerit.py` & `megadetector-5.0.8/data_management/importers/prepare_zsl_imerit.py`

 * *Files identical despite different names*

### Comparing `megadetector-5.0.7/data_management/importers/rspb_to_json.py` & `megadetector-5.0.8/data_management/importers/rspb_to_json.py`

 * *Files identical despite different names*

### Comparing `megadetector-5.0.7/data_management/importers/save_the_elephants_survey_A.py` & `megadetector-5.0.8/data_management/importers/save_the_elephants_survey_A.py`

 * *Files identical despite different names*

### Comparing `megadetector-5.0.7/data_management/importers/save_the_elephants_survey_B.py` & `megadetector-5.0.8/data_management/importers/save_the_elephants_survey_B.py`

 * *Files identical despite different names*

### Comparing `megadetector-5.0.7/data_management/importers/snapshot_safari_importer.py` & `megadetector-5.0.8/data_management/importers/snapshot_safari_importer.py`

 * *Files identical despite different names*

### Comparing `megadetector-5.0.7/data_management/importers/snapshot_safari_importer_reprise.py` & `megadetector-5.0.8/data_management/importers/snapshot_safari_importer_reprise.py`

 * *Files identical despite different names*

### Comparing `megadetector-5.0.7/data_management/importers/snapshot_serengeti_lila.py` & `megadetector-5.0.8/data_management/importers/snapshot_serengeti_lila.py`

 * *Files identical despite different names*

### Comparing `megadetector-5.0.7/data_management/importers/snapshotserengeti/make_full_SS_json.py` & `megadetector-5.0.8/data_management/importers/snapshotserengeti/make_full_SS_json.py`

 * *Files identical despite different names*

### Comparing `megadetector-5.0.7/data_management/importers/snapshotserengeti/make_per_season_SS_json.py` & `megadetector-5.0.8/data_management/importers/snapshotserengeti/make_per_season_SS_json.py`

 * *Files identical despite different names*

### Comparing `megadetector-5.0.7/data_management/importers/sulross_get_exif.py` & `megadetector-5.0.8/data_management/importers/sulross_get_exif.py`

 * *Files identical despite different names*

### Comparing `megadetector-5.0.7/data_management/importers/timelapse_csv_set_to_json.py` & `megadetector-5.0.8/data_management/importers/timelapse_csv_set_to_json.py`

 * *Files identical despite different names*

### Comparing `megadetector-5.0.7/data_management/importers/ubc_to_json.py` & `megadetector-5.0.8/data_management/importers/ubc_to_json.py`

 * *Files identical despite different names*

### Comparing `megadetector-5.0.7/data_management/importers/umn_to_json.py` & `megadetector-5.0.8/data_management/importers/umn_to_json.py`

 * *Files identical despite different names*

### Comparing `megadetector-5.0.7/data_management/importers/wellington_to_json.py` & `megadetector-5.0.8/data_management/importers/wellington_to_json.py`

 * *Files identical despite different names*

### Comparing `megadetector-5.0.7/data_management/importers/wi_to_json.py` & `megadetector-5.0.8/data_management/importers/wi_to_json.py`

 * *Files identical despite different names*

### Comparing `megadetector-5.0.7/data_management/importers/zamba_results_to_md_results.py` & `megadetector-5.0.8/data_management/importers/zamba_results_to_md_results.py`

 * *Files identical despite different names*

### Comparing `megadetector-5.0.7/data_management/labelme_to_coco.py` & `megadetector-5.0.8/data_management/labelme_to_coco.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,47 +1,219 @@
 ########
 #
 # labelme_to_coco.py
 #
-# Converts a folder of labelme-formatted .json files to COCO.
+# Converts a folder of labelme-formatted .json files to COCO format.
 #
 ########
 
 #%% Constants and imports
 
 import json
 import os
 import uuid
 
 from md_utils import path_utils
 from md_visualization.visualization_utils import open_image
 
+from multiprocessing.pool import Pool, ThreadPool
+from functools import partial
+
 from tqdm import tqdm
 
 
-#%% Functions
+#%% Support functions
+
+def add_category(category_name,category_name_to_id,candidate_category_id=0):
+    """
+    Add the category [category_name] to the dict [category_name_to_id], by default
+    using the next available integer index.
+    """
+    
+    if category_name in category_name_to_id:
+        return category_name_to_id[category_name]
+    while candidate_category_id in category_name_to_id.values():
+        candidate_category_id += 1
+    category_name_to_id[category_name] = candidate_category_id
+    return candidate_category_id
+
+
+def _process_labelme_file(image_fn_relative,input_folder,use_folders_as_labels,
+                          no_json_handling,validate_image_sizes,
+                          category_name_to_id,allow_new_categories=True):
+    """
+    Internal function for processing each image; this support function facilitates parallelization.
+    """
+    
+    result = {}
+    result['im'] = None
+    result['annotations_this_image'] = None
+    result['status'] = None
+    
+    image_fn_abs = os.path.join(input_folder,image_fn_relative)
+    json_fn_abs = os.path.splitext(image_fn_abs)[0] + '.json'
+    
+    im = {}
+    im['id'] = image_fn_relative
+    im['file_name'] = image_fn_relative
+    
+    # If there's no .json file for this image...
+    if not os.path.isfile(json_fn_abs):
+        
+        # Either skip it...
+        if no_json_handling == 'skip':
+            print('Skipping image {} (no .json file)'.format(image_fn_relative))
+            result['status'] = 'skipped (no .json file)'
+            return result
+        
+        # ...or error
+        elif no_json_handling == 'error':
+            raise ValueError('Image file {} has no corresponding .json file'.format(
+                image_fn_relative))
+        
+        # ...or treat it as empty.
+        elif no_json_handling == 'empty':
+            try:
+                pil_im = open_image(image_fn_abs)
+            except Exception:
+                print('Warning: error opening image {}, skipping'.format(image_fn_abs))
+                result['status'] = 'image load error'
+                return result
+            im['width'] = pil_im.width
+            im['height'] = pil_im.height
+            
+            # Just in case we need to differentiate between "no .json file" and "a .json file with no annotations"
+            im['no_labelme_json'] = True
+            shapes = []
+        else:
+            raise ValueError('Unrecognized specifier {} for handling images with no .json files'.format(
+                no_json_handling))            
+    
+    # If we found a .json file for this image...
+    else:
+        
+        # Read the .json file
+        with open(json_fn_abs,'r') as f:
+            labelme_data = json.load(f)            
+        im['width'] = labelme_data['imageWidth']
+        im['height'] = labelme_data['imageHeight']
+        
+        if validate_image_sizes:
+            try:
+                pil_im = open_image(image_fn_abs)
+            except Exception:
+                print('Warning: error opening image {} for size validation, skipping'.format(image_fn_abs))
+                result['status'] = 'skipped (size validation error)'
+                return result
+            if not (im['width'] == pil_im.width and im['height'] == pil_im.height):
+                print('Warning: image size validation error for file {}'.format(image_fn_relative))
+                im['width'] = pil_im.width
+                im['height'] = pil_im.height
+                im['labelme_width'] = labelme_data['imageWidth']
+                im['labelme_height'] = labelme_data['imageHeight']
+
+        shapes = labelme_data['shapes']
+
+        if ('flags' in labelme_data) and (len(labelme_data['flags']) > 0):
+            im['flags'] = labelme_data['flags']
+
+    annotations_this_image = []
+    
+    if len(shapes) == 0:
+        
+        if allow_new_categories:
+            category_id = add_category('empty',category_name_to_id)
+        else:
+            assert 'empty' in category_name_to_id
+            category_id = category_name_to_id['empty']
+            
+        ann = {}
+        ann['id'] = str(uuid.uuid1())
+        ann['image_id'] = im['id']
+        ann['category_id'] = category_id
+        ann['sequence_level_annotation'] = False
+        annotations_this_image.append(ann)
+        
+    else:
+        
+        for shape in shapes:
+            
+            if shape['shape_type'] != 'rectangle':
+                print('Only rectangles are supported, skipping an annotation of type {} in {}'.format(
+                    shape['shape_type'],image_fn_relative))
+                continue
+            
+            if use_folders_as_labels:
+                category_name = os.path.basename(os.path.dirname(image_fn_abs))
+            else:
+                category_name = shape['label']                
+            
+            if allow_new_categories:
+                category_id = add_category(category_name,category_name_to_id)
+            else:
+                assert category_name in category_name_to_id
+                category_id = category_name_to_id[category_name]
+            
+            points = shape['points']
+            if len(points) != 2:
+                print('Warning: illegal rectangle with {} points for {}'.format(
+                    len(points),image_fn_relative))
+                continue
+            
+            p0 = points[0]
+            p1 = points[1]
+            x0 = min(p0[0],p1[0])
+            x1 = max(p0[0],p1[0])
+            y0 = min(p0[1],p1[1])
+            y1 = max(p0[1],p1[1])
+            
+            bbox = [x0,y0,abs(x1-x0),abs(y1-y0)]
+            ann = {}
+            ann['id'] = str(uuid.uuid1())
+            ann['image_id'] = im['id']
+            ann['category_id'] = category_id
+            ann['sequence_level_annotation'] = False
+            ann['bbox'] = bbox
+            annotations_this_image.append(ann)
+            
+        # ...for each shape
+        
+    result['im'] = im
+    result['annotations_this_image'] = annotations_this_image
+
+    return result
+    
+# ...def _process_labelme_file(...)
+
+
+#%% Main function
 
 def labelme_to_coco(input_folder,
                     output_file=None,
                     category_id_to_category_name=None,
                     empty_category_name='empty',
                     empty_category_id=None,
                     info_struct=None,
                     relative_paths_to_include=None,
                     relative_paths_to_exclude=None,
                     use_folders_as_labels=False,
                     recursive=True,
                     no_json_handling='skip',
                     validate_image_sizes=True,
-                    right_edge_quantization_threshold=None):
+                    max_workers=1, 
+                    use_threads=True):
     """
     Find all images in [input_folder] that have corresponding .json files, and convert
     to a COCO .json file.
     
-    Currently only supports bounding box annotations.
+    Currently only supports bounding box annotations and image-level flags (i.e., does not
+    support point or general polygon annotations).
+    
+    Labelme's image-level flags don't quite fit the COCO annotations format, so they are attached
+    to image objects, rather than annotation objects.
     
     If output_file is None, just returns the resulting dict, does not write to file.    
     
     if use_folders_as_labels is False (default), the output labels come from the labelme
     .json files.  If use_folders_as_labels is True, the lowest-level folder name containing
     each .json file will determine the output label.  E.g., if use_folders_as_labels is True,
     and the folder contains:
@@ -52,183 +224,120 @@
     file.  Empty images in the "lion" folder will still be given the label "empty" (or 
     [empty_category_name]).
     
     no_json_handling can be:
         
     * 'skip': ignore image files with no corresponding .json files
     * 'empty': treat image files with no corresponding .json files as empty
-    * 'error': throw an error when an image file has no corresponding .json file
-    
-    right_edge_quantization_threshold is an off-by-default hack to handle cases where 
-    boxes that really should be running off the right side of the image only extend like 99%
-    of the way there, due to what appears to be a slight bias inherent to MD.  If a box extends
-    within [right_edge_quantization_threshold] (a small number, from 0 to 1, but probably around 
-    0.02) of the right edge of the image, it will be extended to the far right edge.    
+    * 'error': throw an error when an image file has no corresponding .json file    
     """
     
+    if max_workers > 1:
+        assert category_id_to_category_name is not None, \
+            'When parallelizing labelme --> COCO conversion, you must supply a category mapping'
+            
     if category_id_to_category_name is None:
         category_name_to_id = {}
     else:
         category_name_to_id = {v: k for k, v in category_id_to_category_name.items()}
-        
     for category_name in category_name_to_id:
         try:
             category_name_to_id[category_name] = int(category_name_to_id[category_name])
         except ValueError:
             raise ValueError('Category IDs must be ints or string-formatted ints')
+    
+    # If the user supplied an explicit empty category ID, and the empty category
+    # name is already in category_name_to_id, make sure they match.
+    if empty_category_id is not None:
+        if empty_category_name in category_name_to_id:
+            assert category_name_to_id[empty_category_name] == empty_category_id, \
+                'Ambiguous empty category specification'
+        if empty_category_id in category_id_to_category_name:
+            assert category_id_to_category_name[empty_category_id] == empty_category_name, \
+                'Ambiguous empty category specification'
+    else:
+        if empty_category_name in category_name_to_id:
+            empty_category_id = category_name_to_id[empty_category_name]
 
+    del category_id_to_category_name
+            
     # Enumerate images
+    print('Enumerating images in {}'.format(input_folder))    
     image_filenames_relative = path_utils.find_images(input_folder,recursive=recursive,
-                                                      return_relative_paths=True)    
+                                                      return_relative_paths=True,
+                                                      convert_slashes=True)    
     
-    def add_category(category_name,candidate_category_id=0):
-        if category_name in category_name_to_id:
-            return category_name_to_id[category_name]
-        while candidate_category_id in category_name_to_id.values():
-            candidate_category_id += 1
-        category_name_to_id[category_name] = candidate_category_id
-        return candidate_category_id
+    # Remove any images we're supposed to skip
+    if (relative_paths_to_include is not None) or (relative_paths_to_exclude is not None):
+        image_filenames_relative_to_process = []
+        for image_fn_relative in image_filenames_relative:
+            if relative_paths_to_include is not None and image_fn_relative not in relative_paths_to_include:
+                continue
+            if relative_paths_to_exclude is not None and image_fn_relative in relative_paths_to_exclude:
+                continue
+            image_filenames_relative_to_process.append(image_fn_relative)
+        print('Processing {} of {} images'.format(
+            len(image_filenames_relative_to_process),
+            len(image_filenames_relative)))
+        image_filenames_relative = image_filenames_relative_to_process
     
+    # If the user supplied a category ID to use for empty images...
     if empty_category_id is not None:
         try:
             empty_category_id = int(empty_category_id)
         except ValueError:
             raise ValueError('Category IDs must be ints or string-formatted ints')
         
     if empty_category_id is None:
-        empty_category_id = add_category(empty_category_name)
-        
-    images = []
-    annotations = []
-    
-    n_edges_quantized = 0
-    
-    # image_fn_relative = image_filenames_relative[0]
-    for image_fn_relative in tqdm(image_filenames_relative):
-        
-        if relative_paths_to_include is not None and image_fn_relative not in relative_paths_to_include:
-            continue
-        if relative_paths_to_exclude is not None and image_fn_relative in relative_paths_to_exclude:
-            continue
-        
-        image_fn_abs = os.path.join(input_folder,image_fn_relative)
-        json_fn_abs = os.path.splitext(image_fn_abs)[0] + '.json'
-        
-        im = {}
-        im['id'] = image_fn_relative
-        im['file_name'] = image_fn_relative
+        empty_category_id = add_category(empty_category_name,category_name_to_id)
+            
+    if max_workers <= 1:
         
-        # If there's no .json file for this image...
-        if not os.path.isfile(json_fn_abs):
+        image_results = []
+        for image_fn_relative in tqdm(image_filenames_relative):
             
-            # Either skip it...
-            if no_json_handling == 'skip':
-                continue
+            result = _process_labelme_file(image_fn_relative,input_folder,use_folders_as_labels,
+                                      no_json_handling,validate_image_sizes,
+                                      category_name_to_id,allow_new_categories=True)        
+            image_results.append(result)
             
-            # ...or error
-            elif no_json_handling == 'error':
-                raise ValueError('Image file {} has no corresponding .json file'.format(
-                    image_fn_relative))
-            
-            # ...or treat it as empty.
-            elif no_json_handling == 'empty':
-                try:
-                    pil_im = open_image(image_fn_abs)
-                except Exception:
-                    print('Warning: error opening image {}, skipping'.format(image_fn_abs))
-                    continue
-                im['width'] = pil_im.width
-                im['height'] = pil_im.height
-                shapes = []
-            else:
-                raise ValueError('Unrecognized specifier {} for handling images with no .json files'.format(
-                    no_json_handling))            
+    else:                      
         
-        # If we found a .json file for this image...
+        n_workers = min(max_workers,len(image_filenames_relative))
+        assert category_name_to_id is not None
+        
+        if use_threads:
+            pool = ThreadPool(n_workers)
         else:
-            
-            # Read the .json file
-            with open(json_fn_abs,'r') as f:
-                labelme_data = json.load(f)            
-            im['width'] = labelme_data['imageWidth']
-            im['height'] = labelme_data['imageHeight']
-            
-            if validate_image_sizes:
-                try:
-                    pil_im = open_image(image_fn_abs)
-                except Exception:
-                    print('Warning: error opening image {}, skipping'.format(image_fn_abs))
-                    continue                
-                assert im['width'] == pil_im.width and im['height'] == pil_im.height, \
-                    'Image size validation error for file {}'.format(image_fn_relative)                
-                
-            shapes = labelme_data['shapes']
+            pool = Pool(n_workers)
         
-        if len(shapes) == 0:
-            
-            category_id = add_category('empty')
-            ann = {}
-            ann['id'] = str(uuid.uuid1())
-            ann['image_id'] = im['id']
-            ann['category_id'] = category_id
-            ann['sequence_level_annotation'] = False
-            annotations.append(ann)
-            
+        image_results = list(tqdm(pool.imap(
+            partial(_process_labelme_file,
+                input_folder=input_folder,
+                use_folders_as_labels=use_folders_as_labels,
+                no_json_handling=no_json_handling,
+                validate_image_sizes=validate_image_sizes,
+                category_name_to_id=category_name_to_id,
+                allow_new_categories=False
+                ),image_filenames_relative), total=len(image_filenames_relative)))
+        
+    images = []
+    annotations = []
+    
+    # Flatten the lists of images and annotations
+    for result in image_results:
+        im = result['im']
+        annotations_this_image = result['annotations_this_image']
+        
+        if im is None:
+            assert annotations_this_image is None
         else:
+            images.append(im)
+            annotations.extend(annotations_this_image)
             
-            for shape in shapes:
-                if shape['shape_type'] != 'rectangle':
-                    print('Only rectangles are supported, skipping an annotation of type {} in {}'.format(
-                        shape['shape_type'],image_fn_relative))
-                    continue
-                
-                if use_folders_as_labels:
-                    category_name = os.path.basename(os.path.dirname(image_fn_abs))
-                else:
-                    category_name = shape['label']                
-                
-                category_id = add_category(category_name)
-            
-                points = shape['points']
-                assert len(points) == 2, 'Illegal rectangle with {} points'.format(
-                    len(points))
-                
-                p0 = points[0]
-                p1 = points[1]
-                x0 = min(p0[0],p1[0])
-                x1 = max(p0[0],p1[0])
-                y0 = min(p0[1],p1[1])
-                y1 = max(p0[1],p1[1])
-                
-                if right_edge_quantization_threshold is not None:                    
-                    x1_rel = x1 / (im['width'] - 1)
-                    right_edge_distance = 1.0 - x1_rel
-                    if right_edge_distance < right_edge_quantization_threshold:
-                        n_edges_quantized += 1
-                        x1 = im['width'] - 1
-                        
-                bbox = [x0,y0,abs(x1-x0),abs(y1-y0)]
-                ann = {}
-                ann['id'] = str(uuid.uuid1())
-                ann['image_id'] = im['id']
-                ann['category_id'] = category_id
-                ann['sequence_level_annotation'] = False
-                ann['bbox'] = bbox
-                annotations.append(ann)
-                
-            # ...for each shape
-            
-        images.append(im)
-                  
-    # ..for each image                
-    
-    if n_edges_quantized > 0:
-        print('Quantized the right edge in {} of {} images'.format(
-            n_edges_quantized,len(image_filenames_relative)))
-        
     output_dict = {}
     output_dict['images'] = images
     output_dict['annotations'] = annotations
     
     if info_struct is None:
         info_struct = {}
     if 'description' not in info_struct:
```

### Comparing `megadetector-5.0.7/data_management/labelme_to_yolo.py` & `megadetector-5.0.8/data_management/labelme_to_yolo.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,58 +7,62 @@
 ########
 
 #%% Imports
 
 import os
 import json
 
+from multiprocessing.pool import Pool, ThreadPool
+from functools import partial
+
 from md_utils.path_utils import recursive_file_list
 from tqdm import tqdm
 
 
 #%% Main function
 
 def labelme_file_to_yolo_file(labelme_file,
                               category_name_to_category_id,
                               yolo_file=None,
                               required_token=None,
-                              right_edge_quantization_threshold=None,
                               overwrite_behavior='overwrite'):
     """
     Convert the single .json file labelme_file to yolo format, writing the results to the text
     file yolo_file (defaults to s/json/txt).
     
-    If required_token is not None and the labelme_file does not contain the key [required_token],
-    no-ops.
+    If required_token is not None and the dict in labelme_file does not contain the key [required_token],
+    this function no-ops (i.e., does not generate a YOLO file).    
     
-    right_edge_quantization_threshold is an off-by-default hack to handle cases where 
-    boxes that really should be running off the right side of the image only extend like 99%
-    of the way there, due to what appears to be a slight bias inherent to MD.  If a box extends
-    within [right_edge_quantization_threshold] (a small number, from 0 to 1, but probably around 
-    0.02) of the right edge of the image, it will be extended to the far right edge.    
+    overwrite_behavior should be 'skip' or 'overwrite' (default).
     """
     
+    result = {}
+    result['labelme_file'] = labelme_file
+    result['status'] = 'unknown'
+    
     assert os.path.isfile(labelme_file), 'Could not find labelme .json file {}'.format(labelme_file)
     assert labelme_file.endswith('.json'), 'Illegal labelme .json file {}'.format(labelme_file)
     
     if yolo_file is None:
         yolo_file = os.path.splitext(labelme_file)[0] + '.txt'
     
     if os.path.isfile(yolo_file):
         if overwrite_behavior == 'skip':
-            return
+            result['status'] = 'skip-exists'
+            return result
         else:
             assert overwrite_behavior == 'overwrite', \
                 'Unrecognized overwrite behavior {}'.format(overwrite_behavior)
                 
     with open(labelme_file,'r') as f:
         labelme_data = json.load(f)
         
     if required_token is not None and required_token not in labelme_data:
-        return
+        result['status'] = 'skip-no-required-token'
+        return result
     
     im_height = labelme_data['imageHeight']
     im_width = labelme_data['imageWidth']
     
     yolo_lines = []
     
     for shape in labelme_data['shapes']:
@@ -79,33 +83,30 @@
         minx_abs = min(p0[0],p1[0])
         maxx_abs = max(p0[0],p1[0])
         miny_abs = min(p0[1],p1[1])
         maxy_abs = max(p0[1],p1[1])
         
         if (minx_abs >= (im_width-1)) or (maxx_abs <= 0) or \
             (miny_abs >= (im_height-1)) or (maxy_abs <= 0):
-                print('Skipping invalid shape in {}'.format(labelme_file))
+                print('Skipping invalid shape in {}'.format(labelme_file))                
                 continue
             
-        # Clip to [0,1]
+        # Clip to [0,1]... it's not obvious that the YOLO format doesn't allow bounding
+        # boxes to extend outside the image, but YOLOv5 and YOLOv8 get sad about boxes
+        # that extend outside the image.
         maxx_abs = min(maxx_abs,im_width-1)
         maxy_abs = min(maxy_abs,im_height-1)
         minx_abs = max(minx_abs,0.0)
         miny_abs = max(miny_abs,0.0)
         
         minx_rel = minx_abs / (im_width-1)
         maxx_rel = maxx_abs / (im_width-1)
         miny_rel = miny_abs / (im_height-1)
         maxy_rel = maxy_abs / (im_height-1)
         
-        if (right_edge_quantization_threshold is not None):
-            right_edge_distance = 1.0 - maxx_rel
-            if right_edge_distance < right_edge_quantization_threshold:
-                maxx_rel = 1.0
-        
         assert maxx_rel >= minx_rel
         assert maxy_rel >= miny_rel
         
         xcenter_rel = (maxx_rel + minx_rel) / 2.0
         ycenter_rel = (maxy_rel + miny_rel) / 2.0
         w_rel = maxx_rel - minx_rel
         h_rel = maxy_rel - miny_rel
@@ -115,40 +116,53 @@
         yolo_lines.append(yolo_line)
         
     # ...for each shape
     
     with open(yolo_file,'w') as f:
         for s in yolo_lines:
             f.write(s + '\n')
-        
+    
+    result['status'] = 'converted'
+    return result
+
 
 def labelme_folder_to_yolo(labelme_folder,
                            category_name_to_category_id=None,
                            required_token=None,
-                           right_edge_quantization_threshold=None,
-                           overwrite_behavior='overwrite'):
+                           overwrite_behavior='overwrite',
+                           relative_filenames_to_convert=None,
+                           n_workers=1,
+                           use_threads=True):
     """
     Given a folder with images and labelme .json files, convert the .json files
     to YOLO .txt format.  If category_name_to_category_id is None, first reads
     all the labels in the folder to build a zero-indexed name --> ID mapping.
     
     If required_token is not None and a labelme_file does not contain the key [required_token],
-    it won't be converted.
+    it won't be converted.  Typically used to specify a field that indicates which files have
+    been reviewed.
     
-    right_edge_quantization_threshold is an off-by-default hack to handle cases where 
-    boxes that really should be running off the right side of the image only extend like 99%
-    of the way there, due to what appears to be a slight bias inherent to MD.  If a box extends
-    within [right_edge_quantization_threshold] (a small number, from 0 to 1, but probably around 
-    0.02) of the right edge of the image, it will be extended to the far right edge.    
+    If relative_filenames_to_convert is not None, this should be a list of .json (not image)
+    files that should get converted, relative to the base folder.
     
-    returns category_name_to_category_id, whether it was passed in or constructed.
+    overwrite_behavior should be 'skip' or 'overwrite' (default).
+    
+    returns a dict with:
+        'category_name_to_category_id', whether it was passed in or constructed
+        'image_results': a list of results for each image (converted, skipped, error)
+        
     """
     
-    labelme_files_relative = recursive_file_list(labelme_folder,return_relative_paths=True)
-    labelme_files_relative = [fn for fn in labelme_files_relative if fn.endswith('.json')]
+    if relative_filenames_to_convert is not None:
+        labelme_files_relative = relative_filenames_to_convert
+        assert all([fn.endswith('.json') for fn in labelme_files_relative]), \
+            'relative_filenames_to_convert contains non-json files'
+    else:
+        labelme_files_relative = recursive_file_list(labelme_folder,return_relative_paths=True)
+        labelme_files_relative = [fn for fn in labelme_files_relative if fn.endswith('.json')]
     
     if required_token is None:
         valid_labelme_files_relative = labelme_files_relative
     else:        
         valid_labelme_files_relative = []
         
         # fn_relative = labelme_files_relative[-1]
@@ -159,17 +173,17 @@
             with open(fn_abs,'r') as f:
                 labelme_data = json.load(f)
                 if required_token not in labelme_data:
                     continue
                 
             valid_labelme_files_relative.append(fn_relative)
     
-    print('{} of {} files are valid'.format(len(valid_labelme_files_relative),
-                                           len(labelme_files_relative)))
-    
+        print('{} of {} files are valid'.format(len(valid_labelme_files_relative),
+                                                len(labelme_files_relative)))
+        
     del labelme_files_relative
         
     if category_name_to_category_id is None:
         
         category_name_to_category_id = {}
         
         for fn_relative in valid_labelme_files_relative:
@@ -180,50 +194,79 @@
                 for shape in labelme_data['shapes']:
                     label = shape['label']
                     if label not in category_name_to_category_id:
                         category_name_to_category_id[label] = len(category_name_to_category_id)
         # ...for each file
         
     # ...if we need to build a category mapping
-            
-    for fn_relative in tqdm(valid_labelme_files_relative):
-        
-        fn_abs = os.path.join(labelme_folder,fn_relative)
-        labelme_file_to_yolo_file(fn_abs,
-                                  category_name_to_category_id,
-                                  yolo_file=None,
-                                  required_token=required_token,
-                                  right_edge_quantization_threshold=\
-                                      right_edge_quantization_threshold,
-                                  overwrite_behavior=overwrite_behavior)
     
-    # ...for each file
+    image_results = []
+    
+    n_workers = min(n_workers,len(valid_labelme_files_relative))
+    
+    if n_workers <= 1:
+        for fn_relative in tqdm(valid_labelme_files_relative):
+            
+            fn_abs = os.path.join(labelme_folder,fn_relative)
+            image_result = labelme_file_to_yolo_file(fn_abs,
+                                      category_name_to_category_id,
+                                      yolo_file=None,
+                                      required_token=required_token,
+                                      overwrite_behavior=overwrite_behavior)
+            image_results.append(image_result)
+        # ...for each file
+    else:
+        if use_threads:
+            pool = ThreadPool(n_workers)
+        else:
+            pool = Pool(n_workers)
+
+        valid_labelme_files_abs = [os.path.join(labelme_folder,fn_relative) for \
+                                   fn_relative in valid_labelme_files_relative]
+            
+        image_results = list(tqdm(pool.imap(
+            partial(labelme_file_to_yolo_file,
+                    category_name_to_category_id=category_name_to_category_id,
+                    yolo_file=None,
+                    required_token=required_token,
+                    overwrite_behavior=overwrite_behavior),
+                    valid_labelme_files_abs), 
+                    total=len(valid_labelme_files_abs)))
+
+    assert len(valid_labelme_files_relative) == len(image_results)
     
     print('Converted {} labelme .json files to YOLO'.format(
         len(valid_labelme_files_relative)))
     
-    return category_name_to_category_id
+    labelme_to_yolo_results = {}
+    labelme_to_yolo_results['category_name_to_category_id'] = category_name_to_category_id
+    labelme_to_yolo_results['image_results'] = image_results
     
-        
+    return labelme_to_yolo_results
+    
+# ...def labelme_folder_to_yolo(...)        
+
+
 #%% Interactive driver
 
 if False:
 
     pass
 
     #%%
 
-    import os
     labelme_file = os.path.expanduser('~/tmp/labels/x.json')
-    yolo_file = None
     required_token = 'saved_by_labelme'
-    right_edge_quantization_threshold = 0.015
     category_name_to_category_id = {'animal':0}
+    labelme_folder = os.path.expanduser('~/tmp/labels')
 
     #%%
     
-    labelme_folder = os.path.expanduser('~/tmp/labels')
-
-
+    category_name_to_category_id = \
+        labelme_folder_to_yolo(labelme_folder,
+                               category_name_to_category_id=category_name_to_category_id,
+                               required_token=required_token,
+                               overwrite_behavior='overwrite')
+    
 #%% Command-line driver
 
 # TODO
```

### Comparing `megadetector-5.0.7/data_management/lila/add_locations_to_island_camera_traps.py` & `megadetector-5.0.8/data_management/lila/add_locations_to_island_camera_traps.py`

 * *Files identical despite different names*

### Comparing `megadetector-5.0.7/data_management/lila/add_locations_to_nacti.py` & `megadetector-5.0.8/data_management/lila/add_locations_to_nacti.py`

 * *Files identical despite different names*

### Comparing `megadetector-5.0.7/data_management/lila/create_lila_blank_set.py` & `megadetector-5.0.8/data_management/lila/create_lila_blank_set.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 ########
 #
 # create_lila_blank_set.py
 #
 # Create a folder of blank images sampled from LILA.  We'll aim for diversity, so less-common
 # locations will be oversampled relative to more common locations.  We'll also run MegaDetector
-# to minimize the chance that incorrectly-labeled non-empty images sneak into our blank set.
+# (with manual review) to remove some incorrectly-labeled, not-actually-empty images from our 
+# blank set.
+#
+# We'll store location information for each image in a .json file, so we can split locations
+# into train/val in downstream tasks.
 #
 ########
 
 #%% Constants and imports
 
 import os
 import random
 import math
 import json
-import shutil
 
 import numpy as np
 from tqdm import tqdm
 from multiprocessing.pool import ThreadPool
 from urllib.parse import urlparse
 from collections import defaultdict
 
-from data_management.lila.lila_common import \
-    read_lila_all_images_file, azure_url_to_gcp_http_url
+from data_management.lila.lila_common import read_lila_all_images_file
 from md_utils.url_utils import download_url
 from md_visualization import visualization_utils as vis_utils
 from md_utils.path_utils import recursive_file_list
 
 # We'll write images, metadata downloads, and temporary files here
 lila_local_base = os.path.expanduser('~/lila')
 
@@ -41,14 +43,22 @@
 
 confirmed_blanks_base = os.path.join(project_base,'confirmed_blanks')
 os.makedirs(confirmed_blanks_base,exist_ok=True)
 
 md_possible_non_blanks_folder = os.path.join(project_base,'candidate_non_blanks')
 os.makedirs(md_possible_non_blanks_folder,exist_ok=True)
 
+location_to_blank_image_urls_cache_file = os.path.join(project_base,
+                                                       'location_to_blank_image_urls.json')
+
+md_results_file = os.path.join(project_base,'lila_blanks_md_results.json')
+
+all_fn_relative_to_location_file = os.path.join(project_base,'all_fn_relative_to_location.json')
+confirmed_fn_relative_to_location_file = os.path.join(project_base,'confirmed_fn_relative_to_location.json')
+
 preferred_image_download_source = 'gcp'
 
 # Number of concurrent download threads
 n_download_threads = 20
 
 n_blanks = 100000
 
@@ -167,17 +177,14 @@
         (s in blank_original_labels) or \
         (s in nonblank_original_labels) or \
         (s in other_labels_without_common_names)
 
 
 #%% Map locations to blank images
 
-location_to_blank_image_urls_cache_file = os.path.join(project_base,
-                                                       'location_to_blank_image_urls.json')
-
 force_map_locations = False
 
 # Load from .json if available
 if (not force_map_locations) and (os.path.isfile(location_to_blank_image_urls_cache_file)):
     
     with open(location_to_blank_image_urls_cache_file,'r') as f:
         location_to_blank_image_urls = json.load(f)
@@ -271,15 +278,15 @@
 print('Choose {} blanks from {} locations'.format(n_blanks,len(location_ids)))
 print('Fully sampled {} locations'.format(len(fully_sampled_locations)))
 print('Max samples per location: {}'.format(max_blanks_per_location))
     
 
 #%% Download those image files (prep)
 
-container_to_url_base = { 
+container_to_url_base = {
                          'lilablobssc.blob.core.windows.net':'/',
                          'storage.googleapis.com':'/public-datasets-lila/'
                          }
 
 def download_relative_filename(url, output_base, verbose=False, url_base=None, overwrite=False):
     """
     Download a URL to output_base, preserving relative path
@@ -314,14 +321,29 @@
             url,str(e)))     
         result['status'] = 'error: {}'.format(str(e))
         return result
     
     result['status'] = 'success'
     return result
 
+def azure_url_to_gcp_http_url(url,error_if_not_azure_url=True):
+    """
+    Most URLs point to Azure by default, but most files are available on both Azure and GCP.
+    This function converts an Azure URL to the corresponding GCP http:// url.
+    """
+    
+    lila_azure_storage_account = 'https://lilablobssc.blob.core.windows.net'
+    gcp_bucket_api_url = 'https://storage.googleapis.com/public-datasets-lila'
+    error_if_not_azure_url = False
+    
+    if error_if_not_azure_url:
+        assert url.startswith(lila_azure_storage_account)
+    gcp_url = url.replace(lila_azure_storage_account,gcp_bucket_api_url,1)
+    return gcp_url
+
 # Convert Azure URLs to GCP URLs if necessary
 if preferred_image_download_source != 'azure':
     assert preferred_image_download_source == 'gcp'
     blank_urls = [azure_url_to_gcp_http_url(url) for url in blank_urls]    
 
 
 #%% Download those image files (execution)
@@ -354,16 +376,14 @@
         error_urls.append(r['url'])
 
 print('Errors on {} of {} downloads'.format(len(error_urls),len(results)))
 
 
 #%% Run MegaDetector on the folder
 
-md_results_file = os.path.join(project_base,'lila_blanks_md_results.json')
-
 cmd = 'python run_detector_batch.py MDV5A "{}" "{}"'.format(
     candidate_blanks_base,md_results_file)
 cmd += ' --recursive --output_relative_filenames'
 
 import clipboard; clipboard.copy(cmd); print(cmd)
 
 
@@ -415,14 +435,15 @@
     # shutil.copyfile(source_file_abs,target_file_abs)
     vis_utils.draw_bounding_boxes_on_file(input_file=source_file_abs,
                                           output_file=target_file_abs, 
                                           detections=images_to_review_to_detections[source_file_relative], 
                                           confidence_threshold=min_threshold,
                                           target_size=(1280,-1))
 
+# This is a temporary file I just used during debugging
 with open(os.path.join(project_base,'output_file_to_source_file.json'),'w') as f:
     json.dump(output_file_to_source_file,f,indent=1)
     
     
 #%% Manual review
 
 # Delete images that are *not* empty
@@ -438,37 +459,99 @@
 
 # output_file = next(iter(output_file_to_source_file.keys()))
 for output_file in tqdm(output_file_to_source_file.keys()):
     if output_file not in remaining_images:
         source_file_relative = output_file_to_source_file[output_file]
         removed_blank_images_relative.append(source_file_relative)
         
+removed_blank_images_relative_set = set(removed_blank_images_relative)
 assert len(removed_blank_images_relative) + len(remaining_images) == len(output_file_to_source_file)
 
 
-#%% Copy all the confirmed blanks to the confirmed folder
+#%% Copy only the confirmed blanks to the confirmed folder
+
+from md_utils.path_utils import is_image_file
 
 all_candidate_blanks = recursive_file_list(candidate_blanks_base,return_relative_paths=True)
 print('Found {} candidate blanks'.format(len(all_candidate_blanks)))
 
+skipped_images_relative = []
+skipped_non_images = []
+
 for source_fn_relative in tqdm(all_candidate_blanks):
+    
+    # Skip anything we removed from the "candidate non-blanks" folder; these weren't really
+    # blank.
+    if source_fn_relative in removed_blank_images_relative_set:
+        skipped_images_relative.append(source_fn_relative)
+        continue
+    
+    if not is_image_file(source_fn_relative):
+        # Not a typo; "skipped images" really means "skipped files"
+        skipped_images_relative.append(source_fn_relative)
+        skipped_non_images.append(source_fn_relative)
+    
+    
     source_fn_abs = os.path.join(candidate_blanks_base,source_fn_relative)
     assert os.path.isfile(source_fn_abs)
     target_fn_abs = os.path.join(confirmed_blanks_base,source_fn_relative)
     os.makedirs(os.path.dirname(target_fn_abs),exist_ok=True)
-    shutil.copyfile(source_fn_abs,target_fn_abs)
+    # shutil.copyfile(source_fn_abs,target_fn_abs)
 
+print('Skipped {} files ({} non-image files)'.format(len(skipped_images_relative),
+                                                     len(skipped_non_images)))
 
-#%% Record location information for each file
 
-fn_relative_to_location = {}
-for location in location_to_blank_image_urls:
+#%% Validate the folder of confirmed blanks
+
+from md_utils.path_utils import find_images
+# all_confirmed_blanks = recursive_file_list(confirmed_blanks_base,return_relative_paths=True)
+all_confirmed_blanks = find_images(confirmed_blanks_base,return_relative_paths=True,recursive=True)
+assert len(all_confirmed_blanks) < len(all_candidate_blanks)
+print('Found {} confirmed blanks'.format(len(all_confirmed_blanks)))
+
+
+#%% Manually review a few of the images we skipped
+
+# ...to make sure they're non-blank
+i_image = random.randint(0, len(skipped_images_relative))
+fn_relative = skipped_images_relative[i_image]
+fn_abs = os.path.join(candidate_blanks_base,fn_relative)
+assert os.path.isfile(fn_abs)
+import clipboard
+clipboard.copy('feh --scale-down "{}"'.format(fn_abs))
+
+
+#%% Record location information for each confirmed file
+
+# Map every URL's path to the corresponding location
+#
+# This is *all empty URLs*, not just the ones we downloaded
+all_fn_relative_to_location = {}
+
+# location = next(iter(location_to_blank_image_urls.keys()))
+for location in tqdm(location_to_blank_image_urls):
     urls_this_location = location_to_blank_image_urls[location]
+    
+    # url = urls_this_location[0]
     for url in urls_this_location:
-        fn_relative = url.split('//')[1]
-        fn_relative_to_location[fn_relative] = location
-        
-all_confirmed_blanks = recursive_file_list(confirmed_blanks_base,return_relative_paths=True)
-print('Found {} confirmed blanks'.format(len(all_confirmed_blanks)))
+        # Turn:
+        # 
+        # https://lilablobssc.blob.core.windows.net/caltech-unzipped/cct_images/5968c0f9-23d2-11e8-a6a3-ec086b02610b.jpg'
+        #
+        # ...into:
+        #
+        # caltech-unzipped/cct_images/5968c0f9-23d2-11e8-a6a3-ec086b02610b.jpg'   
+        p = urlparse(url)
+        fn_relative = str(p.path)[1:]
+        all_fn_relative_to_location[fn_relative] = location
+
+# Build a much smaller mapping of just the confirmed blanks
+confirmed_fn_relative_to_location = {}        
+for i_fn,fn_relative in tqdm(enumerate(all_confirmed_blanks),total=len(all_confirmed_blanks)):
+    confirmed_fn_relative_to_location[fn_relative] = all_fn_relative_to_location[fn_relative]
 
-for fn_relative in all_confirmed_blanks:
-    assert fn_relative in fn_relative_to_location
+with open(all_fn_relative_to_location_file,'w') as f:
+    json.dump(all_fn_relative_to_location,f,indent=1)
+    
+with open(confirmed_fn_relative_to_location_file,'w') as f:
+    json.dump(confirmed_fn_relative_to_location,f,indent=1)
```

### Comparing `megadetector-5.0.7/data_management/lila/create_lila_test_set.py` & `megadetector-5.0.8/data_management/lila/create_lila_test_set.py`

 * *Files identical despite different names*

### Comparing `megadetector-5.0.7/data_management/lila/create_links_to_md_results_files.py` & `megadetector-5.0.8/data_management/lila/create_links_to_md_results_files.py`

 * *Files identical despite different names*

### Comparing `megadetector-5.0.7/data_management/lila/generate_lila_per_image_labels.py` & `megadetector-5.0.8/data_management/lila/generate_lila_per_image_labels.py`

 * *Files 0% similar despite different names*

```diff
@@ -334,15 +334,15 @@
             print('Warning: {} of {} images are un-annotated\n'.\
                   format(len(unannotated_images),len(images)))
         
     # ...for each dataset
 
 # ...with open()
 
-print('Processed {} datsets'.format(len(metadata_table)))
+print('Processed {} datasets'.format(len(metadata_table)))
 
 
 #%% Read the .csv back
 
 df = pd.read_csv(output_file)
 print('Read {} lines from {}'.format(len(df),output_file))
```

### Comparing `megadetector-5.0.7/data_management/lila/get_lila_annotation_counts.py` & `megadetector-5.0.8/data_management/lila/get_lila_annotation_counts.py`

 * *Files identical despite different names*

### Comparing `megadetector-5.0.7/data_management/lila/get_lila_image_counts.py` & `megadetector-5.0.8/data_management/lila/get_lila_image_counts.py`

 * *Files identical despite different names*

### Comparing `megadetector-5.0.7/data_management/lila/lila_common.py` & `megadetector-5.0.8/data_management/lila/lila_common.py`

 * *Files 9% similar despite different names*

```diff
@@ -27,17 +27,21 @@
 wildlife_insights_page_size = 30000
 wildlife_insights_taxonomy_url = 'https://api.wildlifeinsights.org/api/v1/taxonomy/taxonomies-all?fields=class,order,family,genus,species,authority,taxonomyType,uniqueIdentifier,commonNameEnglish&page[size]={}'.format(
     wildlife_insights_page_size)
 wildlife_insights_taxonomy_local_json_filename = 'wi_taxonomy.json'
 wildlife_insights_taxonomy_local_csv_filename = \
     wildlife_insights_taxonomy_local_json_filename.replace('.json','.csv')
 
-lila_azure_storage_account = 'https://lilablobssc.blob.core.windows.net'
-gcp_bucket_api_url = 'https://storage.googleapis.com/public-datasets-lila'
-gcp_bucket_gs_url = 'gs://public-datasets-lila'
+# Filenames are consistent across clouds relative to these URLs
+lila_base_urls = {
+    'azure':'https://lilablobssc.blob.core.windows.net/',
+    'gcp':'https://storage.googleapis.com/public-datasets-lila/',
+    'aws':'http://us-west-2.opendata.source.coop.s3.amazonaws.com/agentmorris/lila-wildlife/'
+}
+
 
 
 #%% Common functions
 
 def read_wildlife_insights_taxonomy_mapping(metadata_dir):
     """
     Reads the WI taxonomy mapping file, downloading the .json data (and writing to .csv) if necessary.
@@ -194,36 +198,14 @@
         else:
             print('{} already unzipped'.format(unzipped_json_filename))
         json_filename = unzipped_json_filename
     
     return json_filename
 
 
-def azure_url_to_gcp_http_url(url,error_if_not_azure_url=True):
-    """
-    Most URLs point to Azure by default, but most files are available on both Azure and GCP.
-    This function converts an Azure URL to the corresponding GCP http:// url.
-    """
-    
-    if error_if_not_azure_url:
-        assert url.startswith(lila_azure_storage_account)
-    gcp_url = url.replace(lila_azure_storage_account,gcp_bucket_api_url,1)
-    return gcp_url
-
-
-def azure_url_to_gcp_gs_url(url,error_if_not_azure_url=True):
-    """
-    Most URLs point to Azure by default, but most files are available on both Azure and GCP.
-    This function converts an Azure URL to the corresponding GCP gs:// url.
-    """
-    
-    return azure_url_to_gcp_http_url(url,error_if_not_azure_url).\
-        replace(gcp_bucket_api_url,gcp_bucket_gs_url,1)
-
-
 #%% Interactive test driver
 
 if False:
     
     pass
 
     #%% Verify that all base URLs exist
@@ -248,20 +230,8 @@
         
         ds_info = dataset_metadata[ds_name]
         urls_to_test.append(ds_info['metadata_url'])
         if ds_info['bbox_url'] != None:
             urls_to_test.append(ds_info['bbox_url'])
             
     status_codes = url_utils.test_urls(urls_to_test)    
-    
-    
-    #%% Verify that the GCP versions of all metadata files exist
-    
-    gcp_urls = []
-    
-    # url = urls_to_test[0]
-    for url in urls_to_test:
-        assert url.startswith(lila_azure_storage_account)
-        gcp_url = url.replace(lila_azure_storage_account,gcp_bucket_api_url,1)
-        gcp_urls.append(gcp_url)
-        
-    status_codes = url_utils.test_urls(gcp_urls)
+
```

### Comparing `megadetector-5.0.7/data_management/lila/test_lila_metadata_urls.py` & `megadetector-5.0.8/data_management/lila/test_lila_metadata_urls.py`

 * *Files identical despite different names*

### Comparing `megadetector-5.0.7/data_management/ocr_tools.py` & `megadetector-5.0.8/data_management/ocr_tools.py`

 * *Files identical despite different names*

### Comparing `megadetector-5.0.7/data_management/read_exif.py` & `megadetector-5.0.8/data_management/read_exif.py`

 * *Files 14% similar despite different names*

```diff
@@ -44,38 +44,48 @@
     # Number of concurrent workers
     n_workers = 1
     
     # Should we use threads (vs. processes) for parallelization?
     #
     # Not relevant if n_workers is 1.
     use_threads = True
-    
+        
+    # "File" and "ExifTool" are tag types used by ExifTool to report data that 
+    # doesn't come from EXIF, rather from the file (e.g. file size).
     tag_types_to_ignore = set(['File','ExifTool'])
     
+    # Include/exclude specific tags (mutually incompatible)
+    tags_to_include = None
+    tags_to_exclude = None
+    
+    # A useful set of tags one might want to limit queries for
+    # options.tags_to_include = ['DateTime','Model','Make','ExifImageWidth','ExifImageHeight','DateTime','DateTimeOriginal','Orientation']
+    
     exiftool_command_name = 'exiftool'
     
     # How should we handle byte-formatted EXIF tags?
     #
     # 'convert_to_string': convert to a Python string
     # 'delete': don't include at all
     # 'raw': include as a byte string
     byte_handling = 'convert_to_string' # 'convert_to_string','delete','raw'
     
     # Should we use exiftool or pil?
     processing_library = 'pil' # 'exiftool','pil'
-
+    
+    
 
 #%% Functions
 
-def enumerate_files(input_folder):
+def enumerate_files(input_folder,recursive=True):
     """
     Enumerates all image files in input_folder, returning relative paths
     """
     
-    image_files = find_images(input_folder,recursive=True)
+    image_files = find_images(input_folder,recursive=recursive)
     image_files = [os.path.relpath(s,input_folder) for s in image_files]
     image_files = [s.replace('\\','/') for s in image_files]
     print('Enumerated {} files'.format(len(image_files)))
     return image_files
 
 
 def get_exif_ifd(exif):
@@ -95,15 +105,15 @@
         for key, value in info.items()
     }
 
 
 def read_pil_exif(im,options=None):
     """
     Read all the EXIF data we know how to read from [im] (path or PIL Image), whether it's 
-    in the PIL default EXIF data or not.
+    in the PIL default EXIF data or not.  Returns a dict.
     """
     
     if options is None:
         options = ReadExifOptions()
         
     image_name = '[image]'
     if isinstance(im,str):
@@ -188,14 +198,40 @@
         dt = datetime.strptime(s, '%Y:%m:%d %H:%M:%S')
     except Exception:
         if verbose:
             print('Warning: could not parse datetime {}'.format(str(s)))
     return dt
 
 
+def _filter_tags(tags,options):
+    """
+    Internal function used to include/exclude specific tags from the exif_tags
+    dict.
+    """
+    
+    if options is None:
+        return tags
+    if options.tags_to_include is None and options.tags_to_exclude is None:
+        return tags
+    if options.tags_to_include is not None:
+        assert options.tags_to_exclude is None, "tags_to_include and tags_to_exclude are incompatible"
+        tags_to_return = {}
+        for tag_name in tags.keys():
+            if tag_name in options.tags_to_include:
+                tags_to_return[tag_name] = tags[tag_name]
+        return tags_to_return
+    if options.tags_to_exclude is not None:
+        assert options.tags_to_include is None, "tags_to_include and tags_to_exclude are incompatible"
+        tags_to_return = {}
+        for tag_name in tags.keys():
+            if tag_name not in options.tags_to_exclude:
+                tags_to_return[tag_name] = tags[tag_name]
+        return tags_to_return
+
+
 def read_exif_tags_for_image(file_path,options=None):
     """
     Get relevant fields from EXIF data for an image
     
     Returns a dict with fields 'status' (str) and 'tags'
     
     The exact format of 'tags' depends on options.processing_library
@@ -223,16 +259,16 @@
             result['error'] = str(e)
         
         if result['status'] == 'unknown':
             if exif_tags is None:            
                 result['status'] = 'empty_read'
             else:
                 result['status'] = 'success'
-                result['tags'] = exif_tags
-                
+                result['tags'] = _filter_tags(exif_tags,options)
+                            
         return result
         
     elif options.processing_library == 'exiftool':
         
         # -G means "Print group name for each tag", e.g. print:
         #
         # [File]          Bits Per Sample                 : 8
@@ -279,17 +315,20 @@
             field_type = field_type[1:-1]
             
             if field_type in options.tag_types_to_ignore:
                 if options.verbose:
                     print('Ignoring tag with type {}'.format(field_type))
                 continue        
             
-            field_tag = field_name_type_tokens[1].strip()
-            
-            tag = [field_type,field_tag,field_value]
+            field_name = field_name_type_tokens[1].strip()
+            if options.tags_to_exclude is not None and field_name in options.tags_to_exclude:
+                continue
+            if options.tags_to_include is not None and field_name not in options.tags_to_include:
+                continue
+            tag = [field_type,field_name,field_value]
             
             exif_tags.append(tag)
             
         # ...for each output line
             
         result['status'] = 'success'
         result['tags'] = exif_tags
@@ -346,28 +385,30 @@
         im['exif_tags'] = None
     
     return im
 
 # ...populate_exif_data()
 
 
-def create_image_objects(image_files):
+def create_image_objects(image_files,recursive=True):
     """
     Create empty image objects for every image in [image_files], which can be a 
     list of relative paths (which will get stored without processing, so the base 
     path doesn't matter here), or a folder name.
     
     Returns a list of dicts with field 'file_name' (a relative path).
+    
+    "recursive" is ignored if "image_files" is a list.
     """
     
     # Enumerate *relative* paths
     if isinstance(image_files,str):    
         print('Enumerating image files in {}'.format(image_files))
         assert os.path.isdir(image_files), 'Invalid image folder {}'.format(image_files)
-        image_files = enumerate_files(image_files)
+        image_files = enumerate_files(image_files,recursive=recursive)
         
     images = []
     for fn in image_files:
         im = {}
         im['file_name'] = fn
         images.append(im)
     
@@ -495,15 +536,15 @@
     
     # https://stackoverflow.com/questions/11210104/check-if-a-program-exists-from-a-python-script
 
     from shutil import which
     return which(name) is not None
 
 
-def read_exif_from_folder(input_folder,output_file=None,options=None,filenames=None):
+def read_exif_from_folder(input_folder,output_file=None,options=None,filenames=None,recursive=True):
     """
     Read EXIF data for all images in input_folder.
     
     If filenames is not None, it should be a list of relative filenames; only those files will 
     be processed.
     
     input_folder can be None or '', in which case filenames should be a list of absolute paths.
@@ -512,14 +553,20 @@
     
     returns a dictionary mapping relative filenames to EXIF data.
     """
     
     if options is None:
         options = ReadExifOptions()
     
+    # Validate options
+    if options.tags_to_include is not None:
+        assert options.tags_to_exclude is None, "tags_to_include and tags_to_exclude are incompatible"
+    if options.tags_to_exclude is not None:
+        assert options.tags_to_include is None, "tags_to_include and tags_to_exclude are incompatible"    
+    
     if input_folder is None:
         input_folder = ''
     if len(input_folder) > 0:
         assert os.path.isdir(input_folder), \
             '{} is not a valid folder'.format(input_folder)
 
     assert (len(input_folder) > 0) or (filenames is not None), \
@@ -538,15 +585,15 @@
             print('Could not write to file {}'.format(output_file))
             raise
         
     if options.processing_library == 'exif':
         assert is_executable(options.exiftool_command_name), 'exiftool not available'
 
     if filenames is None:
-        images = create_image_objects(input_folder)
+        images = create_image_objects(input_folder,recursive=recursive)
     else:
         assert isinstance(filenames,list)
         images = create_image_objects(filenames)
         
     results = populate_exif_for_images(input_folder,images,options)
     
     if output_file is not None:
@@ -563,22 +610,24 @@
     
 #%% Interactive driver
 
 if False:
     
     #%%
     
-    input_folder = os.path.expanduser('~/data/KRU-test')
-    output_file = os.path.expanduser('~/data/test-exif.json')
+    input_folder = r'C:\temp\md-name-testing'
+    output_file = None # r'C:\temp\md-name-testing\exif.json'
     options = ReadExifOptions()
     options.verbose = False
     options.n_workers = 10
     options.use_threads = False
     options.processing_library = 'pil'
     # options.processing_library = 'exiftool'
+    options.tags_to_include = ['DateTime','Model','Make','ExifImageWidth','ExifImageHeight','DateTime','DateTimeOriginal','Orientation']
+    # options.tags_to_exclude = ['MakerNote']
     
     results = read_exif_from_folder(input_folder,output_file,options)
 
     #%%
     
     with open(output_file,'r') as f:
         d = json.load(f)
```

### Comparing `megadetector-5.0.7/data_management/remove_exif.py` & `megadetector-5.0.8/data_management/remove_exif.py`

 * *Files identical despite different names*

### Comparing `megadetector-5.0.7/data_management/resize_coco_dataset.py` & `megadetector-5.0.8/data_management/resize_coco_dataset.py`

 * *Files 25% similar despite different names*

```diff
@@ -22,38 +22,31 @@
 
 
 #%% Functions
 
 def resize_coco_dataset(input_folder,input_filename,
                         output_folder,output_filename,
                         target_size=(-1,-1),
-                        correct_size_image_handling='copy',
-                        right_edge_quantization_threshold=None):
+                        correct_size_image_handling='copy'):
     """
     Given a COCO-formatted dataset (images in input_folder, data in input_filename), resize 
     all the images to a target size (in output_folder) and scale bounding boxes accordingly
     (in output_filename).
     
     target_size should be a tuple/list of ints, length 2.  If either dimension is -1, aspect ratio
     will be preserved.  If both dimensions are -1, this means "keep the original size".  If 
     both dimensions are -1 and correct_size_image_handling is copy, this function is basically 
-    a no-op, although you might still use it for right_edge_quantization_threshold.
+    a no-op.
     
     correct_size_image_handling can be 'copy' (in which case the original image is just copied 
     to the output folder) or 'rewrite' (in which case the image is opened via PIL and re-written,
     attempting to preserve the same quality).  The only reason to do this is the case where 
     you're superstitious about biases coming from images in a training set being written
     by different image encoders.
    
-    right_edge_quantization_threshold is an off-by-default hack to adjust large datasets where 
-    boxes that really should be running off the right side of the image only extend like 99%
-    of the way there, due to what appears to be a slight bias inherent to MD.  If a box extends
-    within [right_edge_quantization_threshold] (a small number, from 0 to 1, but probably around 
-    0.02) of the right edge of the image, it will be extended to the far right edge.
-    
     Returns the COCO database with resized images.
     """
     
     # Read input data
     with open(input_filename,'r') as f:
         d = json.load(f)
     
@@ -122,23 +115,14 @@
                     height_scale = output_h/input_h
                     bbox = \
                            [bbox[0] * width_scale,
                             bbox[1] * height_scale,
                             bbox[2] * width_scale,
                             bbox[3] * height_scale]
                 
-                # Do we need to quantize this box?
-                if right_edge_quantization_threshold is not None and \
-                    right_edge_quantization_threshold > 0:
-                    bbox_right_edge_abs = bbox[0] + bbox[2]
-                    bbox_right_edge_norm = bbox_right_edge_abs / output_w
-                    bbox_right_edge_distance = (1.0 - bbox_right_edge_norm)
-                    if bbox_right_edge_distance < right_edge_quantization_threshold:
-                        bbox[2] = output_w - bbox[0]
-                
                 ann['bbox'] = bbox
             
             # ...if this annotation has a box
     
         # ...for each annotation
     
     # ...for each image
@@ -165,21 +149,18 @@
     target_size = (1600,-1)
     
     output_filename = insert_before_extension(input_filename,'resized-test')
     output_folder = input_folder + '-resized-test'
     
     correct_size_image_handling = 'rewrite'
     
-    right_edge_quantization_threshold = 0.015
-    
     resize_coco_dataset(input_folder,input_filename,
                         output_folder,output_filename,
                         target_size=target_size,
-                        correct_size_image_handling=correct_size_image_handling,
-                        right_edge_quantization_threshold=right_edge_quantization_threshold)
+                        correct_size_image_handling=correct_size_image_handling)
     
     
     #%% Preview
     
     from md_visualization import visualize_db
     options = visualize_db.DbVizOptions()
     options.parallelize_rendering = True
```

### Comparing `megadetector-5.0.7/data_management/yolo_output_to_md_output.py` & `megadetector-5.0.8/data_management/yolo_output_to_md_output.py`

 * *Files identical despite different names*

### Comparing `megadetector-5.0.7/detection/detector_training/copy_checkpoints.py` & `megadetector-5.0.8/detection/detector_training/copy_checkpoints.py`

 * *Files identical despite different names*

### Comparing `megadetector-5.0.7/detection/detector_training/model_main_tf2.py` & `megadetector-5.0.8/detection/detector_training/model_main_tf2.py`

 * *Files identical despite different names*

### Comparing `megadetector-5.0.7/detection/process_video.py` & `megadetector-5.0.8/detection/process_video.py`

 * *Files identical despite different names*

### Comparing `megadetector-5.0.7/detection/pytorch_detector.py` & `megadetector-5.0.8/detection/pytorch_detector.py`

 * *Files identical despite different names*

### Comparing `megadetector-5.0.7/detection/run_detector.py` & `megadetector-5.0.8/detection/run_detector.py`

 * *Files identical despite different names*

### Comparing `megadetector-5.0.7/detection/run_detector_batch.py` & `megadetector-5.0.8/detection/run_detector_batch.py`

 * *Files 1% similar despite different names*

```diff
@@ -241,15 +241,16 @@
 
 #%% Image processing functions
 
 def process_images(im_files, detector, confidence_threshold, use_image_queue=False, 
                    quiet=False, image_size=None, checkpoint_queue=None, include_image_size=False,
                    include_image_timestamp=False, include_exif_data=False):
     """
-    Runs MegaDetector over a list of image files.
+    Runs MegaDetector over a list of image files.  As of 3/2024, this entry point is used when the
+    image queue is enabled, but not in the standard inference path (which loops over process_image()).
 
     Args
     - im_files: list of str, paths to image files
     - detector: loaded model or str (path to .pb/.pt model file)
     - confidence_threshold: float, only detections above this threshold are returned
 
     Returns
@@ -265,15 +266,15 @@
 
     if use_image_queue:
         run_detector_with_image_queue(im_files, detector, confidence_threshold, 
                                       quiet=quiet, image_size=image_size,
                                       include_image_size=include_image_size, 
                                       include_image_timestamp=include_image_timestamp,
                                       include_exif_data=include_exif_data)
-    else:
+    else:            
         results = []
         for im_file in im_files:
             result = process_image(im_file, detector, confidence_threshold,
                                          quiet=quiet, image_size=image_size, 
                                          include_image_size=include_image_size, 
                                          include_image_timestamp=include_image_timestamp,
                                          include_exif_data=include_exif_data)
@@ -658,15 +659,15 @@
 
     except Exception:
         return None        
 
 
 def write_results_to_file(results, output_file, relative_path_base=None, 
                           detector_file=None, info=None, include_max_conf=False,
-                          custom_metadata=None):
+                          custom_metadata=None, force_forward_slashes=True):
     """
     Writes list of detection results to JSON output file. Format matches:
 
     https://github.com/agentmorris/MegaDetector/tree/master/api/batch_processing#batch-processing-api-output-format
 
     Args
     - results: list of dict, each dict represents detections on one image
@@ -688,14 +689,22 @@
         results_relative = []
         for r in results:
             r_relative = copy.copy(r)
             r_relative['file'] = os.path.relpath(r_relative['file'], start=relative_path_base)
             results_relative.append(r_relative)
         results = results_relative
 
+    if force_forward_slashes:
+        results_converted = []
+        for r in results:
+            r_converted = copy.copy(r)
+            r_converted['file'] = r_converted['file'].replace('\\','/')
+            results_converted.append(r_converted)
+        results = results_converted
+            
     # The typical case: we need to build the 'info' struct
     if info is None:
         
         info = { 
             'detection_completion_time': datetime.utcnow().strftime('%Y-%m-%d %H:%M:%S'),
             'format_version': '1.3' 
         }
```

### Comparing `megadetector-5.0.7/detection/run_inference_with_yolov5_val.py` & `megadetector-5.0.8/detection/run_inference_with_yolov5_val.py`

 * *Files 1% similar despite different names*

```diff
@@ -101,14 +101,16 @@
     overwrite_handling = 'skip'
     
     preview_yolo_command_only = False
     
     treat_copy_failures_as_warnings = False
     
     save_yolo_debug_output = False
+    
+    recursive = True
             
     
 #%% Main function
 
 def run_inference_with_yolo_val(options):
 
     ##%% Input and path handling
@@ -199,15 +201,15 @@
     os.makedirs(symlink_folder_inner,exist_ok=True)
     os.makedirs(yolo_results_folder,exist_ok=True)
     
 
     ##%% Enumerate images
     
     if os.path.isdir(options.input_folder):
-        image_files_absolute = path_utils.find_images(options.input_folder,recursive=True)
+        image_files_absolute = path_utils.find_images(options.input_folder,recursive=options.recursive)
     else:
         assert os.path.isfile(options.input_folder)
         with open(options.input_folder,'r') as f:            
             image_files_absolute = json.load(f)
             assert isinstance(image_files_absolute,list)
             for fn in image_files_absolute:
                 assert os.path.isfile(fn), 'Could not find image file {}'.format(fn)
@@ -377,15 +379,15 @@
         with open(os.path.join(yolo_results_folder,'image_id_to_error.json'),'w') as f:
             json.dump(image_id_to_error,f,indent=1)
                 
         
     # YOLO console output contains lots of ANSI escape codes, remove them for easier parsing
     yolo_console_output = [string_utils.remove_ansi_codes(s) for s in yolo_console_output]
     
-    # Find errors that occrred during the initial corruption check; these will not be included in the
+    # Find errors that occurred during the initial corruption check; these will not be included in the
     # output.  Errors that occur during inference will be handled separately.
     yolo_read_failures = []
     
     for line in yolo_console_output:
         # Lines look like:
         #
         # For ultralytics val:
@@ -514,15 +516,15 @@
         help='confidence threshold for including detections in the output file (default {})'.format(
             options.conf_thres))
     parser.add_argument(
         '--batch_size', default=options.batch_size, type=int,
         help='inference batch size (default {})'.format(options.batch_size))
     parser.add_argument(
         '--half_precision_enabled', default=None, type=int,
-        help='use half-precision-inference (1 or 0) (default is the underlying model\'s default, probably half for YOLOv8 and full for YOLOv8')
+        help='use half-precision-inference (1 or 0) (default is the underlying model\'s default, probably full for YOLOv8 and half for YOLOv5')
     parser.add_argument(
         '--device_string', default=options.device_string, type=str,
         help='CUDA device specifier, typically "0" or "1" for CUDA devices, "mps" for M1/M2 devices, or "cpu" (default {})'.format(options.device_string))
     parser.add_argument(
         '--overwrite_handling', default=options.overwrite_handling, type=str,
         help='action to take if the output file exists (skip, error, overwrite) (default {})'.format(
             options.overwrite_handling))
@@ -550,14 +552,18 @@
         '--no_remove_yolo_results_folder', action='store_true',
         help='don\'t remove the temporary folder full of YOLO intermediate files')
     parser.add_argument(
         '--save_yolo_debug_output', action='store_true',
         help='write yolo console output to a text file in the results folder, along with additional debug files')
     
     parser.add_argument(
+        '--nonrecursive', action='store_true',
+        help='Disable recursive folder processing')
+    
+    parser.add_argument(
         '--preview_yolo_command_only', action='store_true',
         help='don\'t run inference, just preview the YOLO inference command (still creates symlinks)')
     
     if options.augment:
         default_augment_enabled = 1
     else:
         default_augment_enabled = 0
@@ -588,14 +594,15 @@
             augment_enabled_string,args.image_size))
         
     args_to_object(args, options)
     
     if args.yolo_dataset_file is not None:
         options.yolo_category_id_to_name = args.yolo_dataset_file
         
+    options.recursive = (not options.nonrecursive)
     options.remove_symlink_folder = (not options.no_remove_symlink_folder)
     options.remove_yolo_results_folder = (not options.no_remove_yolo_results_folder)
     options.use_symlinks = (not options.no_use_symlinks)
     options.augment = (options.augment_enabled > 0)        
             
     print(options.__dict__)
```

### Comparing `megadetector-5.0.7/detection/run_tiled_inference.py` & `megadetector-5.0.8/detection/run_tiled_inference.py`

 * *Files 0% similar despite different names*

```diff
@@ -819,20 +819,20 @@
         type=float,
         default=default_patch_overlap,
         help=('Overlap between tiles [0,1] (defaults to {})'.format(default_patch_overlap)))
     parser.add_argument(
         '--overwrite_handling',
         type=str,
         default='skip',
-        help=('behavior when the targt file exists (skip/overwrite/error) (default skip)'))
+        help=('Behavior when the target file exists (skip/overwrite/error) (default skip)'))
     parser.add_argument(
         '--image_list',
         type=str,
         default=None,
-        help=('a .json list of relative filenames (or absolute paths contained within image_folder) to include'))
+        help=('A .json list of relative filenames (or absolute paths contained within image_folder) to include'))
         
     if len(sys.argv[1:]) == 0:
         parser.print_help()
         parser.exit()
 
     args = parser.parse_args()
```

### Comparing `megadetector-5.0.7/detection/tf_detector.py` & `megadetector-5.0.8/detection/tf_detector.py`

 * *Files 0% similar despite different names*

```diff
@@ -118,15 +118,16 @@
 
         Args:
             image: the PIL Image object
             image_id: a path to identify the image; will be in the "file" field of the output object
             detection_threshold: confidence above which to include the detection proposal
 
         Returns:
-        A dict with the following fields, see the 'images' key in https://github.com/agentmorris/MegaDetector/tree/master/api/batch_processing#batch-processing-api-output-format
+        A dict with the following fields, see the 'images' key in:
+        https://github.com/agentmorris/MegaDetector/tree/master/api/batch_processing#batch-processing-api-output-format
             - 'file' (always present)
             - 'max_detection_conf'
             - 'detections', which is a list of detection objects containing keys 'category', 'conf' and 'bbox'
             - 'failure'
         """
         
         assert image_size is None, 'Image sizing not supported for TF detectors'
```

### Comparing `megadetector-5.0.7/detection/video_utils.py` & `megadetector-5.0.8/detection/video_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -306,15 +306,15 @@
         fs_by_video = [x[1] for x in results]
         
     return frame_filenames_by_video,fs_by_video,input_files_full_paths
   
 
 class FrameToVideoOptions:
     
-    # zero-indexed
+    # One-indexed, i.e. "1" means "use the confidence value from the highest-confidence frame"
     nth_highest_confidence = 1
     
     # 'error' or 'skip_with_warning'
     non_video_behavior = 'error'
     
     
 def frame_results_to_video_results(input_file,output_file,options:FrameToVideoOptions = None):
```

### Comparing `megadetector-5.0.7/md_utils/azure_utils.py` & `megadetector-5.0.8/md_utils/azure_utils.py`

 * *Files identical despite different names*

### Comparing `megadetector-5.0.7/md_utils/ct_utils.py` & `megadetector-5.0.8/md_utils/ct_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,17 +35,21 @@
     """
 
     return [truncate_float(x, precision=precision) for x in xs]
 
 
 def truncate_float(x, precision=3):
     """
-    Truncates a floating-point value to a specific number of significant digits.
+    Truncates the fractional portion of a floating-point value to a specific number of 
+    floating-point digits.
     
-    For example: truncate_float(0.0003214884) --> 0.000321
+    For example: 
+        
+        truncate_float(0.0003214884) --> 0.000321
+        truncate_float(1.0003214884) --> 1.000321
     
     This function is primarily used to achieve a certain float representation
     before exporting to JSON.
 
     Args:
     x         (float) Scalar to truncate
     precision (int)   The number of significant digits to preserve, should be
@@ -54,21 +58,26 @@
 
     assert precision > 0
 
     if np.isclose(x, 0):
         
         return 0
     
+    elif (x > 1):
+        
+        fractional_component = x - 1.0
+        return 1 + truncate_float(fractional_component)
+    
     else:
         
         # Determine the factor, which shifts the decimal point of x
         # just behind the last significant digit.
         factor = math.pow(10, precision - 1 - math.floor(math.log10(abs(x))))
         
-        # Shift decimal point by multiplicatipon with factor, flooring, and
+        # Shift decimal point by multiplication with factor, flooring, and
         # division by factor.
         return math.floor(x * factor)/factor
 
 
 def args_to_object(args: argparse.Namespace, obj: object) -> None:
     """
     Copies all fields from a Namespace (typically the output from parse_args) to an
@@ -170,14 +179,15 @@
 
 
 def convert_xywh_to_xyxy(api_bbox):
     """
     Converts an xywh bounding box to an xyxy bounding box.
 
     Note that this is also different from the TensorFlow Object Detection API coords format.
+    
     Args:
         api_bbox: bbox output by the batch processing API [x_min, y_min, width_of_box, height_of_box]
 
     Returns:
         bbox with coordinates represented as [x_min, y_min, x_max, y_max]
     """
 
@@ -348,14 +358,23 @@
             i_chunk = i_item % n
             chunks[i_chunk].append(item)
         return chunks
     else:
         raise ValueError('Invalid chunk strategy: {}'.format(chunk_strategy))
 
 
+def sort_dictionary_by_key(d,reverse=False):
+    """
+    Sorts the dictionary [d] by key.
+    """
+    
+    d = dict(sorted(d.items(),reverse=reverse))
+    return d
+    
+
 def sort_dictionary_by_value(d,sort_values=None,reverse=False):
     """
     Sorts the dictionary [d] by value.  If sort_values is None, uses d.values(),
     otherwise uses the dictionary sort_values as the sorting criterion.
     """
     
     if sort_values is None:
```

### Comparing `megadetector-5.0.7/md_utils/directory_listing.py` & `megadetector-5.0.8/md_utils/directory_listing.py`

 * *Files identical despite different names*

### Comparing `megadetector-5.0.7/md_utils/md_tests.py` & `megadetector-5.0.8/md_utils/md_tests.py`

 * *Files 0% similar despite different names*

```diff
@@ -82,19 +82,22 @@
         pt_string = 'pt1.10.1'
     except Exception:
         pass
     
     return 'md-test-results-{}-{}.json'.format(hw_string,pt_string)
     
     
-def download_test_data(options):
+def download_test_data(options=None):
     """
     Download the test zipfile if necessary, unzip if necessary.
     """
-    
+
+    if options is None:
+        options = MDTestOptions()
+        
     if options.scratch_dir is None:        
         tempdir_base = tempfile.gettempdir()
         scratch_dir = os.path.join(tempdir_base,'md-tests')
     else:
         scratch_dir = options.scratch_dir
     
     os.makedirs(scratch_dir,exist_ok=True)    
@@ -156,14 +159,16 @@
     # Populate the test options with test data information
     options.scratch_dir = scratch_dir
     options.all_test_files = test_files
     options.test_images = [fn for fn in test_files if os.path.splitext(fn.lower())[1] in ('.jpg','.jpeg','.png')]
     options.test_videos = [fn for fn in test_files if os.path.splitext(fn.lower())[1] in ('.mp4','.avi')]    
     options.test_videos = [fn for fn in options.test_videos if 'rendered' not in fn]
         
+    print('Finished unzipping and enumerating test data')
+    
 # ...def download_test_data(...)
 
 
 def is_gpu_available(verbose=True):
     """
     Check whether a GPU (including M1/M2 MPS) is available.
     """
@@ -836,14 +841,18 @@
             options.max_coord_error))
 
     parser.add_argument(
         '--cli_working_dir',
         type=str,
         default=None,
         help='Working directory for CLI tests')
+
+    # token used for linting
+    #
+    # no_arguments_required
         
     args = parser.parse_args()
         
     options.disable_gpu = args.disable_gpu
     options.cpu_execution_is_error = args.cpu_execution_is_error
     options.skip_video_tests = args.skip_video_tests
     options.skip_python_tests = args.skip_python_tests
```

### Comparing `megadetector-5.0.7/md_utils/path_utils.py` & `megadetector-5.0.8/md_utils/path_utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,19 +8,25 @@
 ########
 
 #%% Imports and constants
 
 import glob
 import ntpath
 import os
+import sys
+import platform
 import posixpath
 import string
 import json
+import shutil
 import unicodedata
 import zipfile
+import webbrowser
+import subprocess
+import re
 
 from zipfile import ZipFile
 from datetime import datetime
 from typing import Container, Iterable, List, Optional, Tuple, Sequence
 from multiprocessing.pool import Pool, ThreadPool
 from functools import partial
 from tqdm import tqdm
@@ -39,14 +45,16 @@
                         return_relative_paths=False, sort_files=True,
                         recursive=True):
     r"""
     Enumerate files (not directories) in [base_dir], optionally converting
     \ to /
     """
     
+    assert os.path.isdir(base_dir), '{} is not a folder'.format(base_dir)
+    
     all_files = []
 
     if recursive:
         for root, _, filenames in os.walk(base_dir):
             for filename in filenames:
                 full_path = os.path.join(root, filename)
                 all_files.append(full_path)
@@ -215,31 +223,14 @@
         if not os.readlink(link_new) == link_exists:
             os.remove(link_new)
             os.symlink(link_exists,link_new)
     else:
         os.symlink(link_exists,link_new)
         
 
-def get_file_sizes(base_dir, convert_slashes=True):
-    """
-    Get sizes recursively for all files in base_dir, returning a dict mapping
-    relative filenames to size.
-    """
-    
-    relative_filenames = recursive_file_list(base_dir, convert_slashes=convert_slashes, 
-                                             return_relative_paths=True)
-    
-    fn_to_size = {}
-    for fn_relative in tqdm(relative_filenames):
-        fn_abs = os.path.join(base_dir,fn_relative)
-        fn_to_size[fn_relative] = os.path.getsize(fn_abs)
-                   
-    return fn_to_size
-        
-
 #%% Image-related path functions
 
 def is_image_file(s: str, img_extensions: Container[str] = IMG_EXTENSIONS
                   ) -> bool:
     """
     Checks a file's extension against a hard-coded set of image file
     extensions.
@@ -263,18 +254,20 @@
 
 def find_images(dirname: str, recursive: bool = False, 
                 return_relative_paths: bool = False, 
                 convert_slashes: bool = False) -> List[str]:
     """
     Finds all files in a directory that look like image file names. Returns
     absolute paths unless return_relative_paths is set.  Uses the OS-native
-    path separator unless convert_slahes is set, in which case will always
+    path separator unless convert_slashes is set, in which case will always
     use '/'.
     """
     
+    assert os.path.isdir(dirname), '{} is not a folder'.format(dirname)
+    
     if recursive:
         strings = glob.glob(os.path.join(dirname, '**', '*.*'), recursive=True)
     else:
         strings = glob.glob(os.path.join(dirname, '*.*'))
     
     image_files = find_image_strings(strings)
     
@@ -338,16 +331,14 @@
     for c in separator_chars:
         s = s.replace(c, '~')
     return s
 
 
 #%% Platform-independent way to open files in their associated application
 
-import sys,subprocess,platform,re
-
 def environment_is_wsl():
     """
     Returns True if we're running in WSL
     """
     
     if sys.platform not in ('linux','posix'):
         return False
@@ -369,21 +360,43 @@
     
     result = subprocess.run(['wslpath', '-w', filename], text=True, capture_output=True)
     if result.returncode != 0:
         print('Could not convert path {} from WSL to Windows'.format(filename))
         return None
     return result.stdout.strip()
     
-
-def open_file(filename,attempt_to_open_in_wsl_host=False):
-    """
-    Opens [filename] in the native OS file handler.  If attempt_to_open_in_wsl_host
-    is True, and we're in WSL, attempts to open [filename] in Windows.
+    
+def open_file(filename, attempt_to_open_in_wsl_host=False, browser_name=None):
     """
+    Opens [filename] in the default OS file handler for this file type.
+    
+    If attempt_to_open_in_wsl_host is True, and we're in WSL, attempts to open
+    [filename] in the Windows host environment.
     
+    If browser_name is not None, uses the webbrowser module to open the filename
+    in the specified browser; see https://docs.python.org/3/library/webbrowser.html
+    for supported browsers.  Falls back to the default file handler if webbrowser.open()
+    fails.  In this case, attempt_to_open_in_wsl_host is ignored unless webbrowser.open() fails.
+    
+    If browser_name is 'default', use the system default.  This is different from the 
+    parameter to webbrowser.get(), where None implies the system default.
+    """
+    
+    if browser_name is not None:
+        if browser_name == 'chrome':
+            browser_name = 'google-chrome'
+        elif browser_name == 'default':
+            browser_name = None
+        try:
+            result = webbrowser.get(using=browser_name).open(filename)
+        except Exception:
+            result = False
+        if result:
+            return
+        
     if sys.platform == 'win32':
         
         os.startfile(filename)
 
     elif sys.platform == 'darwin':
       
         opener = 'open'
@@ -433,14 +446,115 @@
         file_list = json.load(f)
     assert isinstance(file_list, list)
     for s in file_list:
         assert isinstance(s, str)
     return file_list
 
 
+def _copy_file(input_output_tuple,overwrite=True,verbose=False):
+    assert len(input_output_tuple) == 2
+    source_fn = input_output_tuple[0]
+    target_fn = input_output_tuple[1]
+    if (not overwrite) and (os.path.isfile(target_fn)):
+        if verbose:
+            print('Skipping existing file {}'.format(target_fn))
+        return
+    os.makedirs(os.path.dirname(target_fn),exist_ok=True)
+    shutil.copyfile(source_fn,target_fn)
+    
+
+def parallel_copy_files(input_file_to_output_file, max_workers=16, 
+                        use_threads=True, overwrite=False, verbose=False):
+    """
+    Copy files from source to target according to the dict input_file_to_output_file.
+    """
+
+    n_workers = min(max_workers,len(input_file_to_output_file))
+    
+    # Package the dictionary as a set of 2-tuples
+    input_output_tuples = []
+    for input_fn in input_file_to_output_file:
+        input_output_tuples.append((input_fn,input_file_to_output_file[input_fn]))
+
+    if use_threads:
+        pool = ThreadPool(n_workers)
+    else:
+        pool = Pool(n_workers)
+
+    with tqdm(total=len(input_output_tuples)) as pbar:
+        for i,_ in enumerate(pool.imap_unordered(partial(_copy_file,overwrite=overwrite,verbose=verbose),
+                                                 input_output_tuples)):
+            pbar.update()
+
+# ...def parallel_copy_files(...)
+
+
+def get_file_sizes(base_dir, convert_slashes=True):
+    """
+    Get sizes recursively for all files in base_dir, returning a dict mapping
+    relative filenames to size.
+    
+    TODO: merge the functionality here with parallel_get_file_sizes, which uses slightly
+    different semantics.
+    """
+    
+    relative_filenames = recursive_file_list(base_dir, convert_slashes=convert_slashes, 
+                                             return_relative_paths=True)
+    
+    fn_to_size = {}
+    for fn_relative in tqdm(relative_filenames):
+        fn_abs = os.path.join(base_dir,fn_relative)
+        fn_to_size[fn_relative] = os.path.getsize(fn_abs)
+                   
+    return fn_to_size
+        
+
+def _get_file_size(filename,verbose=False):
+    """
+    Internal function for safely getting the size of a file.  Returns a (filename,size)
+    tuple, where size is None if there is an error.
+    """
+    
+    try:
+        size = os.path.getsize(filename)
+    except Exception as e:
+        if verbose:
+            print('Error reading file size for {}: {}'.format(filename,str(e)))
+        size = None
+    return (filename,size)
+
+    
+def parallel_get_file_sizes(filenames, max_workers=16, 
+                        use_threads=True, verbose=False,
+                        recursive=True):
+    """
+    Return a dictionary mapping every file in [filenames] to the corresponding file size,
+    or None for errors.  If [filenames] is a folder, will enumerate the folder (optionally recursively).
+    """
+
+    n_workers = min(max_workers,len(filenames))
+    
+    if isinstance(filenames,str) and os.path.isdir(filenames):
+        filenames = recursive_file_list(filenames,recursive=recursive,return_relative_paths=False)
+    
+    if use_threads:
+        pool = ThreadPool(n_workers)
+    else:
+        pool = Pool(n_workers)
+
+    resize_results = list(tqdm(pool.imap(
+        partial(_get_file_size,verbose=verbose),filenames), total=len(filenames)))
+    
+    to_return = {}
+    for r in resize_results:
+        to_return[r[0]] = r[1]
+
+    return to_return
+
+
 #%% Zip functions
 
 def zip_file(input_fn, output_fn=None, overwrite=False, verbose=False, compresslevel=9):
     """
     Zip a single file, by default writing to a new file called [input_fn].zip
     """
     
@@ -450,91 +564,151 @@
         output_fn = input_fn + '.zip'
         
     if (not overwrite) and (os.path.isfile(output_fn)):
         print('Skipping existing file {}'.format(output_fn))
         return
     
     if verbose:
-        print('Zipping {} to {}'.format(input_fn,output_fn))
+        print('Zipping {} to {} with level {}'.format(input_fn,output_fn,compresslevel))
     
     with ZipFile(output_fn,'w',zipfile.ZIP_DEFLATED) as zipf:
         zipf.write(input_fn,arcname=basename,compresslevel=compresslevel,
                    compress_type=zipfile.ZIP_DEFLATED)
 
     return output_fn
 
 
+def zip_files_into_single_zipfile(input_files, output_fn, arc_name_base,
+                                  overwrite=False, verbose=False, compresslevel=9):
+    """
+    Zip all the files in [input_files] into [output_fn].  Archive names are relative to 
+    arc_name_base.
+    """
+    
+    if not overwrite:
+        if os.path.isfile(output_fn):
+            print('Zip file {} exists, skipping'.format(output_fn))
+            return            
+        
+    if verbose:
+        print('Zipping {} files to {} (compression level {})'.format(
+            len(input_files),output_fn,compresslevel))
+        
+    with ZipFile(output_fn,'w',zipfile.ZIP_DEFLATED) as zipf:
+        for input_fn_abs in tqdm(input_files,disable=(not verbose)):
+            input_fn_relative = os.path.relpath(input_fn_abs,arc_name_base)
+            zipf.write(input_fn_abs,
+                       arcname=input_fn_relative,
+                       compresslevel=compresslevel,
+                       compress_type=zipfile.ZIP_DEFLATED)
+
+    return output_fn
+    
+    
 def zip_folder(input_folder, output_fn=None, overwrite=False, verbose=False, compresslevel=9):
     """
-    Recursively zip everything in [input_folder], storing outputs as relative paths.
+    Recursively zip everything in [input_folder] into a single zipfile, storing outputs as relative 
+    paths.
     
     Defaults to writing to [input_folder].zip
     """
     
     if output_fn is None:
         output_fn = input_folder + '.zip'
         
     if not overwrite:
-        assert not os.path.isfile(output_fn), 'Zip file {} exists'.format(output_fn)
+        if os.path.isfile(output_fn):
+            print('Zip file {} exists, skipping'.format(output_fn))
+            return            
         
     if verbose:
-        print('Zipping {} to {}'.format(input_folder,output_fn))
+        print('Zipping {} to {} (compression level {})'.format(
+            input_folder,output_fn,compresslevel))
     
     relative_filenames = recursive_file_list(input_folder,return_relative_paths=True)
     
     with ZipFile(output_fn,'w',zipfile.ZIP_DEFLATED) as zipf:
         for input_fn_relative in tqdm(relative_filenames,disable=(not verbose)):
             input_fn_abs = os.path.join(input_folder,input_fn_relative)            
             zipf.write(input_fn_abs,
                        arcname=input_fn_relative,
                        compresslevel=compresslevel,
                        compress_type=zipfile.ZIP_DEFLATED)
 
     return output_fn
 
         
-def parallel_zip_files(input_files, max_workers=16, use_threads=True):
+def parallel_zip_files(input_files, max_workers=16, use_threads=True, compresslevel=9, 
+                       overwrite=False, verbose=False):
     """
     Zip one or more files to separate output files in parallel, leaving the 
     original files in place.  Each file is zipped to [filename].zip.
     """
 
     n_workers = min(max_workers,len(input_files))
 
     if use_threads:
         pool = ThreadPool(n_workers)
     else:
         pool = Pool(n_workers)
 
     with tqdm(total=len(input_files)) as pbar:
-        for i,_ in enumerate(pool.imap_unordered(zip_file,input_files)):
+        for i,_ in enumerate(pool.imap_unordered(partial(zip_file,
+          output_fn=None,overwrite=overwrite,verbose=verbose,compresslevel=compresslevel),
+          input_files)):
             pbar.update()
 
 
 def parallel_zip_folders(input_folders, max_workers=16, use_threads=True,
-                         compresslevel=9, overwrite=False):
+                         compresslevel=9, overwrite=False, verbose=False):
     """
     Zip one or more folders to separate output files in parallel, leaving the 
     original folders in place.  Each folder is zipped to [folder_name].zip.
     """
 
     n_workers = min(max_workers,len(input_folders))
 
     if use_threads:
         pool = ThreadPool(n_workers)
     else:
         pool = Pool(n_workers)
     
     with tqdm(total=len(input_folders)) as pbar:
         for i,_ in enumerate(pool.imap_unordered(
-                partial(zip_folder,overwrite=overwrite,compresslevel=compresslevel),
+                partial(zip_folder,overwrite=overwrite,
+                        compresslevel=compresslevel,verbose=verbose),
                 input_folders)):
             pbar.update()
 
 
+def zip_each_file_in_folder(folder_name,recursive=False,max_workers=16,use_threads=True,
+                            compresslevel=9,overwrite=False,required_token=None,verbose=False,
+                            exclude_zip=True):
+    """
+    Zip each file in [folder_name] to its own zipfile (filename.zip), optionally recursing.  To zip a whole
+    folder into a single zipfile, use zip_folder().
+    
+    If required_token is not None, include only files that contain that token.
+    """
+    
+    assert os.path.isdir(folder_name), '{} is not a folder'.format(folder_name)
+    
+    input_files = recursive_file_list(folder_name,recursive=recursive,return_relative_paths=False)
+    
+    if required_token is not None:
+        input_files = [fn for fn in input_files if required_token in fn]
+    
+    if exclude_zip:
+        input_files = [fn for fn in input_files if (not fn.endswith('.zip'))]
+                                                    
+    parallel_zip_files(input_files=input_files,max_workers=max_workers,
+                       use_threads=use_threads,compresslevel=compresslevel,
+                       overwrite=overwrite,verbose=verbose)
+
+
 def unzip_file(input_file, output_folder=None):
     """
     Unzip a zipfile to the specified output folder, defaulting to the same location as
     the input file    
     """
     
     if output_folder is None:
```

### Comparing `megadetector-5.0.7/md_utils/process_utils.py` & `megadetector-5.0.8/md_utils/process_utils.py`

 * *Files identical despite different names*

### Comparing `megadetector-5.0.7/md_utils/sas_blob_utils.py` & `megadetector-5.0.8/md_utils/sas_blob_utils.py`

 * *Files identical despite different names*

### Comparing `megadetector-5.0.7/md_utils/split_locations_into_train_val.py` & `megadetector-5.0.8/md_utils/split_locations_into_train_val.py`

 * *Files identical despite different names*

### Comparing `megadetector-5.0.7/md_utils/string_utils.py` & `megadetector-5.0.8/md_utils/string_utils.py`

 * *Files identical despite different names*

### Comparing `megadetector-5.0.7/md_utils/write_html_image_list.py` & `megadetector-5.0.8/md_utils/write_html_image_list.py`

 * *Files 6% similar despite different names*

```diff
@@ -38,14 +38,15 @@
         fHtml
         headerHtml
         trailerHtml
         defaultTextStyle
         defaultImageStyle
         maxFiguresPerHtmlFile
         urlEncodeFilenames (default True, e.g. '#' will be replaced by '%23')
+        urlEncodeLinkTargets (default True, e.g. '#' will be replaced by '%23')
         
     """
     
     # returns an options struct
     if options is None:
         options = {}
         
@@ -64,15 +65,18 @@
 
     if 'defaultImageStyle' not in options or options['defaultImageStyle'] is None:
         options['defaultImageStyle'] = \
         "margin:0px;margin-top:5px;margin-bottom:5px;"
     
     if 'urlEncodeFilenames' not in options or options['urlEncodeFilenames'] is None:
         options['urlEncodeFilenames'] = True
-        
+    
+    if 'urlEncodeLinkTargets' not in options or options['urlEncodeLinkTargets'] is None:
+        options['urlEncodeLinkTargets'] = True
+    
     # Possibly split the html output for figures into multiple files; Chrome gets sad with
     # thousands of images in a single tab.        
     if 'maxFiguresPerHtmlFile' not in options or options['maxFiguresPerHtmlFile'] is None:
         options['maxFiguresPerHtmlFile'] = math.inf    
     
     if filename is None:
         return options
@@ -172,23 +176,28 @@
         filename = image['filename']
         linkTarget = image['linkTarget']
         
         # Remove unicode characters
         title = title.encode('ascii','ignore').decode('ascii')
         filename = filename.encode('ascii','ignore').decode('ascii')
         
-        if options['urlEncodeFilenames']:
-            filename = filename.replace('\\','/')
+        filename = filename.replace('\\','/')
+        if options['urlEncodeFilenames']:            
             filename = urllib.parse.quote(filename)
         
         if len(title) > 0:       
             fHtml.write(
                     '<p style="{}">{}</p>\n'\
                     .format(textStyle,title))            
 
+        linkTarget = linkTarget.replace('\\','/')
+        if options['urlEncodeLinkTargets']:
+            # These are typically absolute paths, so we only want to mess with certain characters
+            linkTarget = urllib.parse.quote(linkTarget,safe=':/')
+            
         if len(linkTarget) > 0:
             fHtml.write('<a href="{}">'.format(linkTarget))
             # imageStyle.append(';border:0px;')
         
         fHtml.write('<img src="{}" style="{}">\n'.format(filename,imageStyle))
         
         if len(linkTarget) > 0:
```

### Comparing `megadetector-5.0.7/md_visualization/plot_utils.py` & `megadetector-5.0.8/md_visualization/plot_utils.py`

 * *Files identical despite different names*

### Comparing `megadetector-5.0.7/md_visualization/render_images_with_thumbnails.py` & `megadetector-5.0.8/md_visualization/render_images_with_thumbnails.py`

 * *Files identical despite different names*

### Comparing `megadetector-5.0.7/md_visualization/visualization_utils.py` & `megadetector-5.0.8/md_visualization/visualization_utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,39 +4,49 @@
 # 
 # Core rendering functions shared across visualization scripts
 #
 ########
 
 #%% Constants and imports
 
-from io import BytesIO
-from typing import Union
 import time
-
-import matplotlib.pyplot as plt
 import numpy as np
 import requests
+import os
+
+from io import BytesIO
+from typing import Union
 from PIL import Image, ImageFile, ImageFont, ImageDraw
+from multiprocessing.pool import ThreadPool
+from multiprocessing.pool import Pool
+from tqdm import tqdm
+from functools import partial
+
+from md_utils.path_utils import find_images
 
 from data_management.annotations import annotation_constants
 from data_management.annotations.annotation_constants import (
-    detector_bbox_category_id_to_name)  # here id is int
+    detector_bbox_category_id_to_name)
 
 ImageFile.LOAD_TRUNCATED_IMAGES = True
 
-IMAGE_ROTATIONS = {
+# Maps EXIF standard rotation identifiers to degrees.  The value "1" indicates no
+# rotation; this will be ignored.  The values 2, 4, 5, and 7 are mirrored rotations,
+# which are not supported (we'll assert() on this when we apply rotations).
+EXIF_IMAGE_NO_ROTATION = 1
+EXIF_IMAGE_ROTATIONS = {
     3: 180,
     6: 270,
     8: 90
 }
 
 TEXTALIGN_LEFT = 0
 TEXTALIGN_RIGHT = 1
 
-# convert category ID from int to str
+# Convert category ID from int to str
 DEFAULT_DETECTOR_LABEL_MAP = {
     str(k): v for k, v in detector_bbox_category_id_to_name.items()
 }
 
 # Retry on blob storage read failures
 n_retries = 10
 retry_sleep_time = 0.01
@@ -44,23 +54,23 @@
 
 DEFAULT_BOX_THICKNESS = 4
 DEFAULT_LABEL_FONT_SIZE = 16
 
 
 #%% Functions
 
-def open_image(input_file: Union[str, BytesIO]) -> Image:
+def open_image(input_file: Union[str, BytesIO], ignore_exif_rotation=False) -> Image:
     """
     Opens an image in binary format using PIL.Image and converts to RGB mode.
     
     Supports local files or URLs.
 
     This operation is lazy; image will not be actually loaded until the first
     operation that needs to load it (for example, resizing), so file opening
-    errors can show up later.
+    errors can show up later.  load_image() is the non-lazy version of this function.
 
     Args:
         input_file: str or BytesIO, either a path to an image file (anything
             that PIL can open), or an image as a stream of bytes
 
     Returns:
         A PIL image object in RGB mode
@@ -97,148 +107,197 @@
     if image.mode not in ('RGBA', 'RGB', 'L', 'I;16'):
         raise AttributeError(
             f'Image {input_file} uses unsupported mode {image.mode}')
     if image.mode == 'RGBA' or image.mode == 'L':
         # PIL.Image.convert() returns a converted copy of this image
         image = image.convert(mode='RGB')
 
-    # Alter orientation as needed according to EXIF tag 0x112 (274) for Orientation
-    #
-    # https://gist.github.com/dangtrinhnt/a577ece4cbe5364aad28
-    # https://www.media.mit.edu/pia/Research/deepview/exif.html
-    #
-    try:
-        exif = image._getexif()
-        orientation: int = exif.get(274, None)  # 274 is the key for the Orientation field
-        if orientation is not None and orientation in IMAGE_ROTATIONS:
-            image = image.rotate(IMAGE_ROTATIONS[orientation], expand=True)  # returns a rotated copy
-    except Exception:
-        pass
+    if not ignore_exif_rotation:
+        # Alter orientation as needed according to EXIF tag 0x112 (274) for Orientation
+        #
+        # https://gist.github.com/dangtrinhnt/a577ece4cbe5364aad28
+        # https://www.media.mit.edu/pia/Research/deepview/exif.html
+        #
+        try:
+            exif = image._getexif()
+            orientation: int = exif.get(274, None)  
+            if (orientation is not None) and (orientation != EXIF_IMAGE_NO_ROTATION):
+                assert orientation in EXIF_IMAGE_ROTATIONS, \
+                    'Mirrored rotations are not supported'
+                image = image.rotate(EXIF_IMAGE_ROTATIONS[orientation], expand=True)  
+        except Exception:
+            pass
 
     return image
 
+# ...def open_image(...)
+
 
-def exif_preserving_save(pil_image,output_file):
+def exif_preserving_save(pil_image,output_file,quality='keep',default_quality=85,verbose=False):
     """
     Save [pil_image] to [output_file], making a moderate attempt to preserve EXIF
     data and JPEG quality.  Neither is guaranteed.
     
     Also see:
     
     https://discuss.dizzycoding.com/determining-jpg-quality-in-python-pil/
      
     ...for more ways to preserve jpeg quality if quality='keep' doesn't do the trick.
+
+    The "quality" parameter should be "keep" (default), or an integer from 0 to 100. 
+    This is only used if PIL thinks the the source image is a JPEG.  If you load a JPEG
+    and resize it in memory, for example, it's no longer a JPEG.
+    
+    'default_quality' is used when quality == 'keep' and we are saving a non-JPEG source.
+    'keep' is only supported for JPEG sources.
     """
     
     # Read EXIF metadata
     exif = pil_image.info['exif'] if ('exif' in pil_image.info) else None
     
-    # Write output with EXIF metadata if available, and quality='keep' if this is a JPEG
-    # image.  Unfortunately, neither parameter likes "None", so we get a slightly
-    # icky cascade of if's here.
-    if exif is not None:
-        if pil_image.format == "JPEG":
-            pil_image.save(output_file, exif=exif, quality='keep')
+    # Quality preservation is only supported for JPEG sources.
+    if pil_image.format != "JPEG":
+        if quality == 'keep':
+            if verbose:
+                print('Warning: quality "keep" passed when saving a non-JPEG source (during save to {})'.format(
+                    output_file))
+            quality = default_quality            
+    
+    # Some output formats don't support the quality parameter, so we try once with, 
+    # and once without.  This is a horrible cascade of if's, but it's a consequence of
+    # the fact that "None" is not supported for either "exif" or "quality".
+        
+    try:
+        
+        if exif is not None:
+            pil_image.save(output_file, exif=exif, quality=quality)
         else:
-            pil_image.save(output_file, exif=exif)
-    else:
-        if pil_image.format == "JPEG":            
-            pil_image.save(output_file, quality='keep')
+            pil_image.save(output_file, quality=quality)
+                
+    except Exception:
+        
+        if verbose:
+            print('Warning: failed to write {}, trying again without quality parameter'.format(output_file))
+        if exif is not None:
+            pil_image.save(output_file, exif=exif)            
         else:
             pil_image.save(output_file)
             
-            
-def load_image(input_file: Union[str, BytesIO]) -> Image:
+# ...def exif_preserving_save(...)
+
+
+def load_image(input_file: Union[str, BytesIO], ignore_exif_rotation=False) -> Image:
     """
     Loads the image at input_file as a PIL Image into memory.
 
     Image.open() used in open_image() is lazy and errors will occur downstream
     if not explicitly loaded.
 
     Args:
         input_file: str or BytesIO, either a path to an image file (anything
             that PIL can open), or an image as a stream of bytes
 
     Returns: PIL.Image.Image, in RGB mode
     """
     
-    image = open_image(input_file)
+    image = open_image(input_file, ignore_exif_rotation=ignore_exif_rotation)
     image.load()
     return image
 
 
-def resize_image(image, target_width, target_height=-1, output_file=None):
+def resize_image(image, target_width, target_height=-1, output_file=None,
+                 no_enlarge_width=False, verbose=False, quality='keep'):
     """
     Resizes a PIL image object to the specified width and height; does not resize
     in place. If either width or height are -1, resizes with aspect ratio preservation.
-    If both are -1, returns the original image (does not copy in this case).
     
     None is equivalent to -1 for target_width and target_height.
     
     [image] can be a PIL image or a filename.
+    
+    If target_width and target_height are both -1, does not modify the image, but 
+    will write to output_file if supplied.
+    
+    If no_enlarge_width is True, and the target width is larger than the original
+    image width, does not modify the image, but will write to output_file if supplied.
+    
+    'quality' is passed to exif_preserving_save, see docs there.
     """
 
+    image_fn = 'in_memory'
     if isinstance(image,str):
+        image_fn = image
         image = load_image(image)
         
     if target_width is None:
         target_width = -1
     
     if target_height is None:
         target_height = -1
+    
+    resize_required = True
         
-    # Null operation
+    # No resize was requested, this is always a no-op
     if target_width == -1 and target_height == -1:
-        return image
-
+        
+        resize_required = False
+    
+    # Does either dimension need to scale according to the other?
     elif target_width == -1 or target_height == -1:
 
         # Aspect ratio as width over height
         # ar = w / h
         aspect_ratio = image.size[0] / image.size[1]
 
         if target_width != -1:
             # h = w / ar
             target_height = int(target_width / aspect_ratio)
         else:
             # w = ar * h
             target_width = int(aspect_ratio * target_height)
-
-    # This parameter changed between Pillow versions 9 and 10, and for a bit, I'd like to
-    # support both.
+    
+    # If we're not enlarging images and this would be an enlarge operation
+    if (no_enlarge_width) and (target_width > image.size[0]):
+        
+        if verbose:
+            print('Bypassing image enlarge for {} --> {}'.format(
+                image_fn,str(output_file)))
+        resize_required = False
+        
+    # If the target size is the same as the original size
+    if (target_width == image.size[0]) and (target_height == image.size[1]):
+        
+        resize_required = False    
+    
+    if not resize_required:
+        
+        if output_file is not None:
+            if verbose:
+                print('No resize required for resize {} --> {}'.format(
+                    image_fn,str(output_file)))
+            exif_preserving_save(image,output_file,quality=quality,verbose=verbose)
+        return image
+    
+    assert target_width > 0 and target_height > 0, \
+        'Invalid image resize target {},{}'.format(target_width,target_height)
+        
+    # The antialiasing parameter changed between Pillow versions 9 and 10, and for a bit, 
+    # I'd like to support both.
     try:
         resized_image = image.resize((target_width, target_height), Image.ANTIALIAS)
     except:
         resized_image = image.resize((target_width, target_height), Image.Resampling.LANCZOS)
         
     if output_file is not None:
-        exif_preserving_save(resized_image,output_file)
+        exif_preserving_save(resized_image,output_file,quality=quality,verbose=verbose)
         
     return resized_image
 
+# ...def resize_image(...)
 
-def show_images_in_a_row(images):
-
-    num = len(images)
-    assert num > 0
-
-    if isinstance(images[0], str):
-        images = [Image.open(img) for img in images]
-
-    fig, axarr = plt.subplots(1, num, squeeze=False)  # number of rows, number of columns
-    fig.set_size_inches((num * 5, 25))  # each image is 2 inches wide
-    for i, img in enumerate(images):
-        axarr[0, i].set_axis_off()
-        axarr[0, i].imshow(img)
-    return fig
-
-
-# The following three functions are modified versions of those at:
-#
-# https://github.com/tensorflow/models/blob/master/research/object_detection/utils/visualization_utils.py
 
 DEFAULT_COLORS = [
     'AliceBlue', 'Red', 'RoyalBlue', 'Gold', 'Chartreuse', 'Aqua', 'Azure',
     'Beige', 'Bisque', 'BlanchedAlmond', 'BlueViolet', 'BurlyWood', 'CadetBlue',
     'AntiqueWhite', 'Chocolate', 'Coral', 'CornflowerBlue', 'Cornsilk', 'Crimson',
     'Cyan', 'DarkCyan', 'DarkGoldenRod', 'DarkGrey', 'DarkKhaki', 'DarkOrange',
     'DarkOrchid', 'DarkSalmon', 'DarkSeaGreen', 'DarkTurquoise', 'DarkViolet',
@@ -369,15 +428,16 @@
                 }
             ]
 
         image: PIL.Image object
 
         label_map: optional, mapping the numerical label to a string name. The type of the numerical label
             (default string) needs to be consistent with the keys in label_map; no casting is carried out.
-            If this is None, no labels are shown.
+            If this is None, no labels are shown (not even numbers and confidence values).  If you want
+            category numbers and confidence values without class labels, use {}.
 
         classification_label_map: optional, mapping of the string class labels to the actual class names.
             The type of the numerical label (default string) needs to be consistent with the keys in
             label_map; no casting is carried out.  If this is None, no classification labels are shown.
 
         confidence_threshold: optional, threshold above which boxes are rendered.  Can also be a dictionary
         mapping category IDs to thresholds.
@@ -487,14 +547,16 @@
     display_boxes = np.array(display_boxes)
 
     draw_bounding_boxes_on_image(image, display_boxes, classes,
                                  display_strs=display_strs, thickness=thickness, 
                                  expansion=expansion, colormap=colormap, textalign=textalign,
                                  label_font_size=label_font_size)
 
+# ...render_detection_bounding_boxes(...)
+
 
 def draw_bounding_boxes_on_image(image,
                                  boxes,
                                  classes,
                                  thickness=DEFAULT_BOX_THICKNESS,
                                  expansion=0,
                                  display_strs=None,
@@ -533,14 +595,16 @@
                                        classes[i],
                                        thickness=thickness, expansion=expansion,
                                        display_str_list=display_str_list,
                                        colormap=colormap,
                                        textalign=textalign,
                                        label_font_size=label_font_size)
 
+# ...draw_bounding_boxes_on_image(...)
+
 
 def draw_bounding_box_on_image(image,
                                ymin,
                                xmin,
                                ymax,
                                xmax,
                                clss=None,
@@ -563,27 +627,33 @@
     are displayed below the bounding box.
 
     Args:
     image: a PIL.Image object.
     ymin: ymin of bounding box - upper left.
     xmin: xmin of bounding box.
     ymax: ymax of bounding box.
-    xmax: xmax of bounding box.
-    clss: str, the class of the object in this bounding box - will be cast to an int.
+    xmax: xmax of bounding box.    
+    clss: str, the class of the object in this bounding box; should be either an integer
+        or a string-formatted integer.
     thickness: line thickness. Default value is 4.
     expansion: number of pixels to expand bounding boxes on each side.  Default is 0.
     display_str_list: list of strings to display in box
         (each to be shown on its own line).
         use_normalized_coordinates: If True (default), treat coordinates
         ymin, xmin, ymax, xmax as relative to the image.  Otherwise treat
         coordinates as absolute.
-    label_font_size: font size to attempt to load arial.ttf with
+    label_font_size: font size 
+    
+    Adapted from:
+        
+    https://github.com/tensorflow/models/blob/master/research/object_detection/utils/visualization_utils.py
     """
     
     if clss is None:
+        # Default to the MegaDetector animal class ID (1)
         color = colormap[1]
     else:
         color = colormap[int(clss) % len(colormap)]
 
     draw = ImageDraw.Draw(image)
     im_width, im_height = image.size
     if use_normalized_coordinates:
@@ -681,14 +751,16 @@
             (text_left + margin, text_bottom - text_height - margin),
             display_str,
             fill='black',
             font=font)
 
         text_bottom -= (text_height + 2 * margin)
 
+# ...def draw_bounding_box_on_image(...)
+
 
 def render_iMerit_boxes(boxes, classes, image,
                         label_map=annotation_constants.annotation_bbox_category_id_to_name):
     """
     Renders bounding boxes and their category labels on a PIL image.
 
     Args:
@@ -754,14 +826,16 @@
         display_boxes.append([y_min, x_min, y_max, x_max])
         display_strs.append([b['category']])
         classes.append(annotation_constants.detector_bbox_category_name_to_id[b['category']])
 
     display_boxes = np.array(display_boxes)
     draw_bounding_boxes_on_image(image, display_boxes, classes, display_strs=display_strs)
 
+# ...def render_iMerit_boxes(...)
+
 
 def render_db_bounding_boxes(boxes, classes, image, original_size=None,
                              label_map=None, thickness=DEFAULT_BOX_THICKNESS, expansion=0):
     """
     Render bounding boxes (with class labels) on [image].  This is a wrapper for
     draw_bounding_boxes_on_image, allowing the caller to operate on a resized image
     by providing the original size of the image; bboxes will be scaled accordingly.
@@ -798,81 +872,90 @@
         # need to be a string here because PIL needs to iterate through chars
         display_strs.append([str(clss)])  
 
     display_boxes = np.array(display_boxes)
     draw_bounding_boxes_on_image(image, display_boxes, classes, display_strs=display_strs,
                                  thickness=thickness, expansion=expansion)
 
+# ...def render_db_bounding_boxes(...)
+
 
 def draw_bounding_boxes_on_file(input_file, output_file, detections, confidence_threshold=0.0,
                                 detector_label_map=DEFAULT_DETECTOR_LABEL_MAP,
                                 thickness=DEFAULT_BOX_THICKNESS, expansion=0,
                                 colormap=DEFAULT_COLORS,
                                 label_font_size=DEFAULT_LABEL_FONT_SIZE,
-                                custom_strings=None,target_size=None):
+                                custom_strings=None,target_size=None,
+                                ignore_exif_rotation=False):
     """
     Render detection bounding boxes on an image loaded from file, writing the results to a
     new image file.
     
     "detections" is in the API results format:
         
     [{"category": "2","conf": 0.996,"bbox": [0.0,0.2762,0.1234,0.2458]}]
     
     ...where the bbox is:
         
     [x_min, y_min, width_of_box, height_of_box]
     
     Normalized, with the origin at the upper-left.
     
-    detector_label_map is a dict mapping category IDs to strings.
+    detector_label_map is a dict mapping category IDs to strings.  If this is None, 
+    no confidence values or identifiers are shown  If this is {}, just category indices and 
+    confidence values are shown.
     
     custom_strings: optional set of strings to append to detection labels, should have the
     same length as [detections].  Appended before classification labels, if classification
     data is provided.
     
     target_size: tuple of (target_width,target_height).  Either or both can be -1,
     see resize_image for documentation.  If None or (-1,-1), uses the original image size.
     """
     
-    image = open_image(input_file)
+    image = open_image(input_file, ignore_exif_rotation=ignore_exif_rotation)
     
     if target_size is not None:
         image = resize_image(image,target_size[0],target_size[1])
         
     render_detection_bounding_boxes(
             detections, image, label_map=detector_label_map,
             confidence_threshold=confidence_threshold,
             thickness=thickness,expansion=expansion,colormap=colormap,
             custom_strings=custom_strings,label_font_size=label_font_size)
 
     image.save(output_file)
 
 
 def draw_db_boxes_on_file(input_file, output_file, boxes, classes=None, 
-                          label_map=None, thickness=DEFAULT_BOX_THICKNESS, expansion=0):
+                          label_map=None, thickness=DEFAULT_BOX_THICKNESS, expansion=0,
+                          ignore_exif_rotation=False):
     """
     Render COCO bounding boxes (in absolute coordinates) on an image loaded from file, writing the
     results to a new image file.
 
     classes is a list of integer category IDs.
     
     detector_label_map is a dict mapping category IDs to strings.
     """
     
-    image = open_image(input_file)
+    image = open_image(input_file, ignore_exif_rotation=ignore_exif_rotation)
 
     if classes is None:
         classes = [0] * len(boxes)
         
     render_db_bounding_boxes(boxes, classes, image, original_size=None,
                                  label_map=label_map, thickness=thickness, expansion=expansion)
 
     image.save(output_file)
     
 
+# ...def draw_bounding_boxes_on_file(...)
+
+
 def gray_scale_fraction(image,crop_size=(0.1,0.1)):
     """
     Returns the fraction of the pixels in [image] that appear to be grayscale (R==G==B), 
     useful for approximating whether this is a night-time image when flash information is not
     available in EXIF data (or for video frames, where this information is often not available
     in structured metadata at all).
     
@@ -934,7 +1017,215 @@
         n_pixels = w*h
         n_gray_pixels = 0
         for i in range(w):
             for j in range(h):
                 r, g, b = image.getpixel((i,j))
                 if r == g and r == b and g == b:
                     n_gray_pixels += 1            
+
+
+# ...def gray_scale_fraction(...)
+
+
+def _resize_relative_image(fn_relative,
+                          input_folder,output_folder,
+                          target_width,target_height,no_enlarge_width,verbose,quality):
+    """
+    Internal function for resizing an image from one folder to another,
+    maintaining relative path.
+    """
+    
+    input_fn_abs = os.path.join(input_folder,fn_relative)
+    output_fn_abs = os.path.join(output_folder,fn_relative)
+    os.makedirs(os.path.dirname(output_fn_abs),exist_ok=True)
+    try:
+        _ = resize_image(input_fn_abs, 
+                         output_file=output_fn_abs, 
+                         target_width=target_width, target_height=target_height, 
+                         no_enlarge_width=no_enlarge_width, verbose=verbose, quality=quality)
+        status = 'success'
+        error = None
+    except Exception as e:
+        if verbose:
+            print('Error resizing {}: {}'.format(fn_relative,str(e)))
+        status = 'error'
+        error = str(e)
+        
+    return {'fn_relative':fn_relative,'status':status,'error':error}
+
+# ...def _resize_relative_image(...)
+
+
+def _resize_absolute_image(input_output_files,
+                          target_width,target_height,no_enlarge_width,verbose,quality):
+    
+    """
+    Internal wrappter for resize_image used in the context of a batch resize operation.
+    """
+    
+    input_fn_abs = input_output_files[0]
+    output_fn_abs = input_output_files[1]
+    os.makedirs(os.path.dirname(output_fn_abs),exist_ok=True)
+    try:
+        _ = resize_image(input_fn_abs, 
+                         output_file=output_fn_abs, 
+                         target_width=target_width, target_height=target_height, 
+                         no_enlarge_width=no_enlarge_width, verbose=verbose, quality=quality)
+        status = 'success'
+        error = None
+    except Exception as e:
+        if verbose:
+            print('Error resizing {}: {}'.format(input_fn_abs,str(e)))
+        status = 'error'
+        error = str(e)
+        
+    return {'input_fn':input_fn_abs,'output_fn':output_fn_abs,status:'status',
+            'error':error}
+
+# ..._resize_absolute_image(...)
+
+
+def resize_images(input_file_to_output_file,
+                  target_width=-1, target_height=-1,
+                  no_enlarge_width=False, verbose=False, quality='keep',
+                  pool_type='process', n_workers=10):
+    """
+    Resize all images the dictionary [input_file_to_output_file].
+    
+    Defaults to parallelizing across processes.
+    
+    See resize_image() for parameter information.
+    
+    TODO: This is a little more redundant with resize_image_folder than I would like;
+    refactor resize_image_folder to call resize_images.  Not doing that yet because
+    at the time I'm writing this comment, a lot of code depends on resize_image_folder 
+    and I don't want to rock the boat yet.
+    """
+
+    
+    assert pool_type in ('process','thread'), 'Illegal pool type {}'.format(pool_type)
+    
+    input_output_file_pairs = []
+    
+    # Reformat input files as (input,output) tuples
+    for input_fn in input_file_to_output_file:
+        input_output_file_pairs.append((input_fn,input_file_to_output_file[input_fn]))
+    
+    if n_workers == 1:    
+        
+        results = []
+        for i_o_file_pair in tqdm(input_output_file_pairs):
+            results.append(_resize_absolute_image(i_o_file_pair,
+                            target_width=target_width,
+                            target_height=target_height,
+                            no_enlarge_width=no_enlarge_width,
+                            verbose=verbose,
+                            quality=quality))
+
+    else:
+        
+        if pool_type == 'thread':
+            pool = ThreadPool(n_workers); poolstring = 'threads'                
+        else:
+            assert pool_type == 'process'
+            pool = Pool(n_workers); poolstring = 'processes'
+        
+        if verbose:
+            print('Starting resizing pool with {} {}'.format(n_workers,poolstring))
+        
+        p = partial(_resize_absolute_image,
+                target_width=target_width,
+                target_height=target_height,
+                no_enlarge_width=no_enlarge_width,
+                verbose=verbose,
+                quality=quality)
+        
+        results = list(tqdm(pool.imap(p, input_output_file_pairs),total=len(input_output_file_pairs)))
+
+    return results
+
+# ...def resize_images(...)
+
+
+def resize_image_folder(input_folder, output_folder=None,
+                        target_width=-1, target_height=-1,
+                        no_enlarge_width=False, verbose=False, quality='keep',
+                        pool_type='process', n_workers=10, recursive=True,
+                        image_files_relative=None):
+    """
+    Resize all images in a folder (defaults to recursive)
+    
+    Defaults to in-place resizing (output_folder is optional).
+    
+    Defaults to parallelizing across processes.
+    
+    See resize_image() for parameter information.
+    """
+
+    assert os.path.isdir(input_folder), '{} is not a folder'.format(input_folder)
+    
+    if output_folder is None:
+        output_folder = input_folder
+    else:
+        os.makedirs(output_folder,exist_ok=True)
+        
+    assert pool_type in ('process','thread'), 'Illegal pool type {}'.format(pool_type)
+    
+    if image_files_relative is None:
+        image_files_relative = find_images(input_folder,recursive=recursive,return_relative_paths=True)
+        if verbose:
+            print('Found {} images'.format(len(image_files_relative)))
+    
+    if n_workers == 1:    
+        
+        results = []
+        for fn_relative in tqdm(image_files_relative):
+            results.append(_resize_relative_image(fn_relative,
+                                  input_folder=input_folder,
+                                  output_folder=output_folder,
+                                  target_width=target_width,
+                                  target_height=target_height,
+                                  no_enlarge_width=no_enlarge_width,
+                                  verbose=verbose,
+                                  quality=quality))
+
+    else:
+        
+        if pool_type == 'thread':
+            pool = ThreadPool(n_workers); poolstring = 'threads'                
+        else:
+            assert pool_type == 'process'
+            pool = Pool(n_workers); poolstring = 'processes'
+        
+        if verbose:
+            print('Starting resizing pool with {} {}'.format(n_workers,poolstring))
+        
+        p = partial(_resize_relative_image,
+                input_folder=input_folder,
+                output_folder=output_folder,
+                target_width=target_width,
+                target_height=target_height,
+                no_enlarge_width=no_enlarge_width,
+                verbose=verbose,
+                quality=quality)
+        
+        results = list(tqdm(pool.imap(p, image_files_relative),total=len(image_files_relative)))
+
+    return results
+
+# ...def resize_image_folder(...)
+
+
+#%% Test drivers
+
+if False:
+    
+    #%% Recursive resize test
+    
+    from md_visualization.visualization_utils import resize_image_folder # noqa
+    
+    input_folder = r"C:\temp\resize-test\in"
+    output_folder = r"C:\temp\resize-test\out"
+    
+    resize_results = resize_image_folder(input_folder,output_folder,
+                         target_width=1280,verbose=True,quality=85,no_enlarge_width=True,
+                         pool_type='process',n_workers=10)
```

### Comparing `megadetector-5.0.7/md_visualization/visualize_db.py` & `megadetector-5.0.8/md_visualization/visualize_db.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,39 +12,42 @@
 import argparse
 import inspect
 import json
 import math
 import os
 import sys
 import time
+
+import pandas as pd
+import numpy as np
+
+import humanfriendly
+
 from itertools import compress
 from multiprocessing.pool import ThreadPool
 from multiprocessing.pool import Pool
-
-import pandas as pd
 from tqdm import tqdm
-import humanfriendly
 
 from md_utils.write_html_image_list import write_html_image_list
+from data_management.cct_json_utils import IndexedJsonDb
 
 import md_visualization.visualization_utils as vis_utils
-from data_management.cct_json_utils import IndexedJsonDb
 
 
 #%% Settings
 
 class DbVizOptions:
     
     # Set to None to visualize all images
     num_to_visualize = None
     
     # Target size for rendering; set either dimension to -1 to preserve aspect ratio
     #
     # If viz_size is None or (-1,-1), the original image size is used.
-    viz_size = (675, -1)
+    viz_size = (800, -1)
     
     # The most relevant option one might want to set here is:
     #
     # htmlOptions['maxFiguresPerHtmlFile']
     #
     # ...which can be used to paginate previews to a number of images that will load well
     # in a browser (5000 is a reasonable limit).
@@ -86,14 +89,19 @@
     # flip this with a warning, since I intend to support it in the future.
     parallelize_rendering_with_threads = True
     parallelize_rendering = False
     
     # Should we show absolute (vs. relative) paths for each image?
     show_full_paths = False
     
+    # Set to False to skip existing images
+    force_rendering = True
+    
+    verbose = False
+    
 
 #%% Helper functions
 
 # Translate the file name in an image entry in the json database to a path, possibly doing
 # some manipulation of path separators
 def image_filename_to_path(image_file_name, image_base_dir, pathsep_replacement=''):
     
@@ -268,15 +276,15 @@
                 elif annotationLevelForImage != annLevel:
                     annotationLevelForImage = 'mixed'
                     
             categoryID = anno['category_id']
             categoryName = label_map[categoryID]
             if options.add_search_links:
                 categoryName = categoryName.replace('"','')
-                categoryName = '<a href="https://www.bing.com/images/search?q={}">{}</a>'.format(
+                categoryName = '<a href="https://www.google.com/search?tbm=isch&q={}">{}</a>'.format(
                     categoryName,categoryName)
             imageCategories.add(categoryName)
             
             if 'bbox' in anno:
                 bbox = anno['bbox']        
                 if isinstance(bbox,float):
                     assert math.isnan(bbox), "I shouldn't see a bbox that's neither a box nor NaN"
@@ -313,22 +321,30 @@
         if options.show_full_paths:
             filename_text = img_path
         else:
             filename_text = img_relative_path
         if options.include_filename_links:
             filename_text = '<a href="{}">{}</a>'.format(img_path,filename_text)
             
+        flagString = ''
+        
+        def isnan(x):
+            return (isinstance(x,float) and np.isnan(x))
+        
+        if ('flags' in img) and (not isnan(img['flags'])):
+            flagString = ', flags: {}'.format(str(img['flags']))
+            
         # We're adding html for an image before we render it, so it's possible this image will
         # fail to render.  For applications where this script is being used to debua a database
         # (the common case?), this is useful behavior, for other applications, this is annoying.
         image_dict = \
         {
             'filename': '{}/{}'.format('rendered_images', file_name),
-            'title': '{}<br/>{}, num boxes: {}, {}class labels: {}{}'.format(
-                filename_text, img_id, len(bboxes), frameString, imageClasses, labelLevelString),
+            'title': '{}<br/>{}, num boxes: {}, {}class labels: {}{}{}'.format(
+                filename_text, img_id, len(bboxes), frameString, imageClasses, labelLevelString, flagString),
             'textStyle': 'font-family:verdana,arial,calibri;font-size:80%;' + \
                 'text-align:left;margin-top:20;margin-bottom:5'
         }
         if options.include_image_links:
             image_dict['linkTarget'] = img_path
             
         images_html.append(image_dict)
@@ -337,39 +353,46 @@
 
     def render_image_info(rendering_info):
         
         img_path = rendering_info['img_path']
         bboxes = rendering_info['bboxes']
         bboxClasses = rendering_info['boxClasses']
         output_file_name = rendering_info['output_file_name']
+        output_full_path = os.path.join(output_dir, 'rendered_images', output_file_name)
         
+        if (os.path.isfile(output_full_path)) and (not options.force_rendering):
+            if options.verbose:
+                print('Skipping existing image {}'.format(output_full_path))
+            return True
+            
         if not img_path.startswith('http'):
             if not os.path.exists(img_path):
                 print('Image {} cannot be found'.format(img_path))
                 return False
             
         try:
             original_image = vis_utils.open_image(img_path)
             original_size = original_image.size
             if (options.viz_size is None) or (options.viz_size[0] == -1 and options.viz_size[1] == -1):
                 image = original_image
             else:
                 image = vis_utils.resize_image(original_image, options.viz_size[0],
                                                options.viz_size[1])
         except Exception as e:
-            print('Image {} failed to open. Error: {}'.format(img_path, e))
+            print('Image {} failed to open, error: {}'.format(img_path, e))
             return False
             
         vis_utils.render_db_bounding_boxes(boxes=bboxes, classes=bboxClasses,
                                            image=image, original_size=original_size,
                                            label_map=label_map,
                                            thickness=options.box_thickness,
                                            expansion=options.box_expansion)
         
-        image.save(os.path.join(output_dir, 'rendered_images', output_file_name))
+        image.save(output_full_path)
+                
         return True
     
     # ...def render_image_info
     
     print('Rendering images')
     start_time = time.time()
```

### Comparing `megadetector-5.0.7/md_visualization/visualize_detector_output.py` & `megadetector-5.0.8/md_visualization/visualize_detector_output.py`

 * *Files identical despite different names*

### Comparing `megadetector-5.0.7/megadetector.egg-info/PKG-INFO` & `megadetector-5.0.8/megadetector.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: megadetector
-Version: 5.0.7
+Version: 5.0.8
 Summary: MegaDetector is an AI model that helps conservation folks spend less time doing boring things with camera trap images.
 Author-email: Your friendly neighborhood MegaDetector team <cameratraps@lila.science>
 Maintainer-email: Your friendly neighborhood MegaDetector team <cameratraps@lila.science>
 License:     MIT License
         
             Permission is hereby granted, free of charge, to any person obtaining a copy
             of this software and associated documentation files (the "Software"), to deal
@@ -56,15 +56,15 @@
 If you want to learn more about what MegaDetector is all about, head over to the [MegaDetector repo](https://github.com/agentmorris/MegaDetector).
 
 
 ## Reasons you probably aren't looking for this package
 
 ### If you are an ecologist...
 
-If you are an ecologist looking to use MegaDetector to help you get through your camera trap images, you probably don't want this package.  We recommend starting with our "[Getting started with MegaDetector](https://github.com/agentmorris/MegaDetector/blob/main/collaborations.md)" page, then digging in to the [MegaDetector User Guide](https://github.com/agentmorris/MegaDetector/blob/main/megadetector.md), which will walk you through the process of using MegaDetector.  That journey will <i>not</i> involve this package.
+If you are an ecologist looking to use MegaDetector to help you get through your camera trap images, you probably don't want this package.  We recommend starting with our "[Getting started with MegaDetector](https://github.com/agentmorris/MegaDetector/blob/main/collaborations.md)" page, then digging in to the [MegaDetector User Guide](https://github.com/agentmorris/MegaDetector/blob/main/megadetector.md), which will walk you through the process of using MegaDetector.  That journey will <i>not</i> involve this Python package.
 
 ### If you are a computer-vision-y type...
 
 If you are a computer-vision-y person looking to run or fine-tune MegaDetector programmatically, you still probably don't want this package.  MegaDetector is just a fine-tuned version of [YOLOv5](https://github.com/ultralytics/yolov5), and the [ultralytics](https://github.com/ultralytics/ultralytics/) package (from the developers of YOLOv5) has a zillion bells and whistles for both inference and fine-tuning that this package doesn't.
 
 ## Reasons you might want to use this package
 
@@ -91,23 +91,21 @@
 
 # This is the image at the bottom of this page, it has one animal in it
 image_url = 'https://github.com/agentmorris/MegaDetector/raw/main/images/orinoquia-thumb-web.jpg'
 temporary_filename = url_utils.download_url(image_url)
 
 image = vis_utils.load_image(temporary_filename)
 
-# This will automatically download MDv5a to the system temp folder;
-# you can also specify a filename explicitly, or set the $MDV5A
-# environment variable to point to the model file.
+# This will automatically download MDv5a; you can also specify a filename.
 model = run_detector.load_detector('MDV5A')
 
 result = model.generate_detections_one_image(image)
 
 detections_above_threshold = [d for d in result['detections'] if d['conf'] > 0.2]
-print('Found {} detection above threshold'.format(len(detections_above_threshold)))
+print('Found {} detections above threshold'.format(len(detections_above_threshold)))
 ```
 
 #### Run MegaDetector on a folder of images
 
 ```
 from detection.run_detector_batch import load_and_run_detector_batch,write_results_to_file
 from md_utils import path_utils
@@ -116,22 +114,22 @@
 # Pick a folder to run MD on recursively, and an output file
 image_folder = os.path.expanduser('~/megadetector_test_images')
 output_file = os.path.expanduser('~/megadetector_output_test.json')
 
 # Recursively find images
 image_file_names = path_utils.find_images(image_folder,recursive=True)
 
-# This will automatically download MDv5a to the system temp folder;
-# you can also specify a filename explicitly, or set the $MDV5A
-# environment variable to point to the model file.
+# This will automatically download MDv5a; you can also specify a filename.
 results = load_and_run_detector_batch('MDV5A', image_file_names)
 
-# Write results as relative filenames, this is what Timelapse
-# and other downstream tools expect.
-write_results_to_file(results,output_file,relative_path_base=image_folder)
+# Write results to a format that Timelapse and other downstream tools like.
+write_results_to_file(results,
+                      output_file,
+                      relative_path_base=image_folder,
+                      detector_file=detector_filename)
 ```
 
 ## Contact
 
 Contact <a href="cameratraps@lila.science">cameratraps@lila.science</a> with questions.
 
 ## Gratuitous animal picture
```

### Comparing `megadetector-5.0.7/megadetector.egg-info/SOURCES.txt` & `megadetector-5.0.8/megadetector.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 api/batch_processing/postprocessing/compare_batch_results.py
 api/batch_processing/postprocessing/convert_output_format.py
 api/batch_processing/postprocessing/load_api_results.py
 api/batch_processing/postprocessing/md_to_coco.py
 api/batch_processing/postprocessing/md_to_labelme.py
 api/batch_processing/postprocessing/merge_detections.py
 api/batch_processing/postprocessing/postprocess_batch_results.py
+api/batch_processing/postprocessing/remap_detection_categories.py
 api/batch_processing/postprocessing/render_detection_confusion_matrix.py
 api/batch_processing/postprocessing/separate_detections_into_folders.py
 api/batch_processing/postprocessing/subset_json_detector_output.py
 api/batch_processing/postprocessing/top_folders_to_bottom.py
 api/batch_processing/postprocessing/repeat_detection_elimination/find_repeat_detections.py
 api/batch_processing/postprocessing/repeat_detection_elimination/remove_repeat_detections.py
 api/batch_processing/postprocessing/repeat_detection_elimination/repeat_detections_core.py
@@ -86,23 +87,26 @@
 classification/efficientnet/model.py
 classification/efficientnet/utils.py
 data_management/cct_json_to_filename_json.py
 data_management/cct_json_utils.py
 data_management/cct_to_csv.py
 data_management/cct_to_md.py
 data_management/cct_to_wi.py
+data_management/coco_to_labelme.py
 data_management/coco_to_yolo.py
 data_management/generate_crops_from_cct.py
 data_management/get_image_sizes.py
 data_management/labelme_to_coco.py
 data_management/labelme_to_yolo.py
 data_management/ocr_tools.py
 data_management/read_exif.py
+data_management/remap_coco_categories.py
 data_management/remove_exif.py
 data_management/resize_coco_dataset.py
+data_management/wi_download_csv_to_coco.py
 data_management/yolo_output_to_md_output.py
 data_management/yolo_to_coco.py
 data_management/annotations/annotation_constants.py
 data_management/databases/add_width_and_height_to_db.py
 data_management/databases/combine_coco_camera_traps_files.py
 data_management/databases/integrity_check_json_db.py
 data_management/databases/remove_corrupted_images_from_db.py
@@ -184,15 +188,14 @@
 md_utils/url_utils.py
 md_utils/write_html_image_list.py
 md_visualization/plot_utils.py
 md_visualization/render_images_with_thumbnails.py
 md_visualization/visualization_utils.py
 md_visualization/visualize_db.py
 md_visualization/visualize_detector_output.py
-md_visualization/visualize_megadb.py
 megadetector.egg-info/PKG-INFO
 megadetector.egg-info/SOURCES.txt
 megadetector.egg-info/dependency_links.txt
 megadetector.egg-info/requires.txt
 megadetector.egg-info/top_level.txt
 taxonomy_mapping/map_lila_taxonomy_to_wi_taxonomy.py
 taxonomy_mapping/map_new_lila_datasets.py
```

### Comparing `megadetector-5.0.7/pyproject.toml` & `megadetector-5.0.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = [
   "setuptools>61"
 ]
 
 [project]
 name = "megadetector"
-version = "5.0.7"
+version = "5.0.8"
 description = "MegaDetector is an AI model that helps conservation folks spend less time doing boring things with camera trap images."
 readme = "README-package.md"
 # As of 2023.10.10, PyTorch isn't installable on Python 3.12
 requires-python = ">=3.9,<3.12"
 license = {file = "LICENSE"}
 keywords = ["camera traps", "conservation", "wildlife", "ai"]
 authors = [
```

### Comparing `megadetector-5.0.7/taxonomy_mapping/map_lila_taxonomy_to_wi_taxonomy.py` & `megadetector-5.0.8/taxonomy_mapping/map_lila_taxonomy_to_wi_taxonomy.py`

 * *Files identical despite different names*

### Comparing `megadetector-5.0.7/taxonomy_mapping/map_new_lila_datasets.py` & `megadetector-5.0.8/taxonomy_mapping/map_new_lila_datasets.py`

 * *Files identical despite different names*

### Comparing `megadetector-5.0.7/taxonomy_mapping/prepare_lila_taxonomy_release.py` & `megadetector-5.0.8/taxonomy_mapping/prepare_lila_taxonomy_release.py`

 * *Files identical despite different names*

### Comparing `megadetector-5.0.7/taxonomy_mapping/preview_lila_taxonomy.py` & `megadetector-5.0.8/taxonomy_mapping/preview_lila_taxonomy.py`

 * *Files identical despite different names*

### Comparing `megadetector-5.0.7/taxonomy_mapping/retrieve_sample_image.py` & `megadetector-5.0.8/taxonomy_mapping/retrieve_sample_image.py`

 * *Files identical despite different names*

### Comparing `megadetector-5.0.7/taxonomy_mapping/simple_image_download.py` & `megadetector-5.0.8/taxonomy_mapping/simple_image_download.py`

 * *Files identical despite different names*

### Comparing `megadetector-5.0.7/taxonomy_mapping/species_lookup.py` & `megadetector-5.0.8/taxonomy_mapping/species_lookup.py`

 * *Files identical despite different names*

### Comparing `megadetector-5.0.7/taxonomy_mapping/taxonomy_csv_checker.py` & `megadetector-5.0.8/taxonomy_mapping/taxonomy_csv_checker.py`

 * *Files identical despite different names*

### Comparing `megadetector-5.0.7/taxonomy_mapping/taxonomy_graph.py` & `megadetector-5.0.8/taxonomy_mapping/taxonomy_graph.py`

 * *Files identical despite different names*

### Comparing `megadetector-5.0.7/taxonomy_mapping/validate_lila_category_mappings.py` & `megadetector-5.0.8/taxonomy_mapping/validate_lila_category_mappings.py`

 * *Files identical despite different names*

