# Comparing `tmp/wrangle-0.7.3.tar.gz` & `tmp/wrangle-0.7.4.tar.gz`

## Comparing `wrangle-0.7.3.tar` & `wrangle-0.7.4.tar`

### file list

```diff
@@ -1,95 +1,95 @@
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 wrangle-0.7.3/wrangle/__init__.py
--rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 wrangle-0.7.3/wrangle/array/__init__.py
--rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 wrangle-0.7.3/wrangle/array/array_detect_task.py
--rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 wrangle-0.7.3/wrangle/array/array_random_shuffle.py
--rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 wrangle-0.7.3/wrangle/array/array_random_weighted.py
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 wrangle-0.7.3/wrangle/array/array_reshape_conv1d.py
--rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 wrangle-0.7.3/wrangle/array/array_reshape_lstm.py
--rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 wrangle-0.7.3/wrangle/array/array_split.py
--rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 wrangle-0.7.3/wrangle/array/array_to_generator.py
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 wrangle-0.7.3/wrangle/array/array_to_kfold.py
--rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 wrangle-0.7.3/wrangle/array/array_to_multilabel.py
--rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 wrangle-0.7.3/wrangle/col/__init__.py
--rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 wrangle-0.7.3/wrangle/col/col_check_allsame.py
--rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 wrangle-0.7.3/wrangle/col/col_corr_category.py
--rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 wrangle-0.7.3/wrangle/col/col_corr_ols.py
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 wrangle-0.7.3/wrangle/col/col_drop_outliers.py
--rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 wrangle-0.7.3/wrangle/col/col_fill_nan.py
--rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 wrangle-0.7.3/wrangle/col/col_groupby_cdf.py
--rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 wrangle-0.7.3/wrangle/col/col_groupby_pdf.py
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 wrangle-0.7.3/wrangle/col/col_groupby_stats.py
--rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 wrangle-0.7.3/wrangle/col/col_impute_nan.py
--rw-r--r--   0        0        0      990 2020-02-02 00:00:00.000000 wrangle-0.7.3/wrangle/col/col_move_place.py
--rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 wrangle-0.7.3/wrangle/col/col_resample_equal.py
--rw-r--r--   0        0        0     1282 2020-02-02 00:00:00.000000 wrangle-0.7.3/wrangle/col/col_resample_interval.py
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 wrangle-0.7.3/wrangle/col/col_rescale_max.py
--rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 wrangle-0.7.3/wrangle/col/col_to_biclass.py
--rw-r--r--   0        0        0     1995 2020-02-02 00:00:00.000000 wrangle-0.7.3/wrangle/col/col_to_binary.py
--rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 wrangle-0.7.3/wrangle/col/col_to_buckets.py
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 wrangle-0.7.3/wrangle/col/col_to_cols.py
--rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 wrangle-0.7.3/wrangle/col/col_to_multilabel.py
--rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 wrangle-0.7.3/wrangle/col/col_to_split.py
--rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 wrangle-0.7.3/wrangle/df/__init__.py
--rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 wrangle-0.7.3/wrangle/df/df_add_scorecol.py
--rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 wrangle-0.7.3/wrangle/df/df_clean_colnames.py
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 wrangle-0.7.3/wrangle/df/df_corr_any.py
--rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 wrangle-0.7.3/wrangle/df/df_corr_extratrees.py
--rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 wrangle-0.7.3/wrangle/df/df_corr_ols.py
--rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 wrangle-0.7.3/wrangle/df/df_corr_pearson.py
--rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 wrangle-0.7.3/wrangle/df/df_corr_randomforest.py
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 wrangle-0.7.3/wrangle/df/df_count_uniques.py
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 wrangle-0.7.3/wrangle/df/df_drop_col.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 wrangle-0.7.3/wrangle/df/df_drop_duplicates.py
--rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 wrangle-0.7.3/wrangle/df/df_drop_nancols.py
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 wrangle-0.7.3/wrangle/df/df_drop_nanrows.py
--rw-r--r--   0        0        0     1185 2020-02-02 00:00:00.000000 wrangle-0.7.3/wrangle/df/df_drop_weak.py
--rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 wrangle-0.7.3/wrangle/df/df_fill_empty.py
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 wrangle-0.7.3/wrangle/df/df_find_nan.py
--rw-r--r--   0        0        0     1463 2020-02-02 00:00:00.000000 wrangle-0.7.3/wrangle/df/df_groupby_params.py
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 wrangle-0.7.3/wrangle/df/df_impute_nan.py
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 wrangle-0.7.3/wrangle/df/df_merge.py
--rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 wrangle-0.7.3/wrangle/df/df_parallelize_process.py
--rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 wrangle-0.7.3/wrangle/df/df_print_values.py
--rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 wrangle-0.7.3/wrangle/df/df_rename_col.py
--rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 wrangle-0.7.3/wrangle/df/df_rename_cols.py
--rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 wrangle-0.7.3/wrangle/df/df_resample_id.py
--rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 wrangle-0.7.3/wrangle/df/df_resample_stratified.py
--rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 wrangle-0.7.3/wrangle/df/df_rescale_log.py
--rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 wrangle-0.7.3/wrangle/df/df_rescale_meanzero.py
--rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 wrangle-0.7.3/wrangle/df/df_rescale_sqrt.py
--rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 wrangle-0.7.3/wrangle/df/df_restructure_values.py
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 wrangle-0.7.3/wrangle/df/df_to_binary.py
--rw-r--r--   0        0        0     1283 2020-02-02 00:00:00.000000 wrangle-0.7.3/wrangle/df/df_to_dfs.py
--rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 wrangle-0.7.3/wrangle/df/df_to_groupby.py
--rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 wrangle-0.7.3/wrangle/df/df_to_lower.py
--rw-r--r--   0        0        0     1173 2020-02-02 00:00:00.000000 wrangle-0.7.3/wrangle/df/df_to_multiclass.py
--rw-r--r--   0        0        0     1352 2020-02-02 00:00:00.000000 wrangle-0.7.3/wrangle/df/df_to_multilabel.py
--rw-r--r--   0        0        0     1195 2020-02-02 00:00:00.000000 wrangle-0.7.3/wrangle/df/df_to_numeric.py
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 wrangle-0.7.3/wrangle/df/df_to_xy.py
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 wrangle-0.7.3/wrangle/dic/__init__.py
--rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 wrangle-0.7.3/wrangle/dic/dic_corr_perc.py
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 wrangle-0.7.3/wrangle/dic/dic_count_complexity.py
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 wrangle-0.7.3/wrangle/dic/dic_resample_values.py
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 wrangle-0.7.3/wrangle/utils/__init__.py
--rw-r--r--   0        0        0     2361 2020-02-02 00:00:00.000000 wrangle-0.7.3/wrangle/utils/category_labeling.py
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 wrangle-0.7.3/wrangle/utils/connection_check.py
--rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 wrangle-0.7.3/wrangle/utils/create_datetime_col.py
--rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 wrangle-0.7.3/wrangle/utils/create_synth_data.py
--rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 wrangle-0.7.3/wrangle/utils/create_synth_model.py
--rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 wrangle-0.7.3/wrangle/utils/create_time_sequence.py
--rw-r--r--   0        0        0     2589 2020-02-02 00:00:00.000000 wrangle-0.7.3/wrangle/utils/datetime_handler.py
--rw-r--r--   0        0        0     1564 2020-02-02 00:00:00.000000 wrangle-0.7.3/wrangle/utils/groupby_func.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 wrangle-0.7.3/wrangle/utils/int_to_string.py
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 wrangle-0.7.3/wrangle/utils/is_number.py
--rw-r--r--   0        0        0     1171 2020-02-02 00:00:00.000000 wrangle-0.7.3/wrangle/utils/multi_input_support.py
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 wrangle-0.7.3/wrangle/utils/nan_dropper.py
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 wrangle-0.7.3/wrangle/utils/network_check.py
--rw-r--r--   0        0        0     1178 2020-02-02 00:00:00.000000 wrangle-0.7.3/wrangle/utils/read_large_csv.py
--rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 wrangle-0.7.3/wrangle/utils/transform_data.py
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 wrangle-0.7.3/wrangle/utils/value_starts_with.py
--rw-r--r--   0        0        0     3193 2020-02-02 00:00:00.000000 wrangle-0.7.3/wrangle/utils/wrangler_utils.py
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 wrangle-0.7.3/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 wrangle-0.7.3/LICENSE
--rw-r--r--   0        0        0     3186 2020-02-02 00:00:00.000000 wrangle-0.7.3/README.md
--rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 wrangle-0.7.3/pyproject.toml
--rw-r--r--   0        0        0     4207 2020-02-02 00:00:00.000000 wrangle-0.7.3/PKG-INFO
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 wrangle-0.7.4/wrangle/__init__.py
+-rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 wrangle-0.7.4/wrangle/array/__init__.py
+-rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 wrangle-0.7.4/wrangle/array/array_detect_task.py
+-rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 wrangle-0.7.4/wrangle/array/array_random_shuffle.py
+-rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 wrangle-0.7.4/wrangle/array/array_random_weighted.py
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 wrangle-0.7.4/wrangle/array/array_reshape_conv1d.py
+-rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 wrangle-0.7.4/wrangle/array/array_reshape_lstm.py
+-rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 wrangle-0.7.4/wrangle/array/array_split.py
+-rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 wrangle-0.7.4/wrangle/array/array_to_generator.py
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 wrangle-0.7.4/wrangle/array/array_to_kfold.py
+-rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 wrangle-0.7.4/wrangle/array/array_to_multilabel.py
+-rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 wrangle-0.7.4/wrangle/col/__init__.py
+-rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 wrangle-0.7.4/wrangle/col/col_check_allsame.py
+-rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 wrangle-0.7.4/wrangle/col/col_corr_category.py
+-rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 wrangle-0.7.4/wrangle/col/col_corr_ols.py
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 wrangle-0.7.4/wrangle/col/col_drop_outliers.py
+-rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 wrangle-0.7.4/wrangle/col/col_fill_nan.py
+-rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 wrangle-0.7.4/wrangle/col/col_groupby_cdf.py
+-rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 wrangle-0.7.4/wrangle/col/col_groupby_pdf.py
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 wrangle-0.7.4/wrangle/col/col_groupby_stats.py
+-rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 wrangle-0.7.4/wrangle/col/col_impute_nan.py
+-rw-r--r--   0        0        0      990 2020-02-02 00:00:00.000000 wrangle-0.7.4/wrangle/col/col_move_place.py
+-rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 wrangle-0.7.4/wrangle/col/col_resample_equal.py
+-rw-r--r--   0        0        0     1282 2020-02-02 00:00:00.000000 wrangle-0.7.4/wrangle/col/col_resample_interval.py
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 wrangle-0.7.4/wrangle/col/col_rescale_max.py
+-rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 wrangle-0.7.4/wrangle/col/col_to_biclass.py
+-rw-r--r--   0        0        0     1995 2020-02-02 00:00:00.000000 wrangle-0.7.4/wrangle/col/col_to_binary.py
+-rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 wrangle-0.7.4/wrangle/col/col_to_buckets.py
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 wrangle-0.7.4/wrangle/col/col_to_cols.py
+-rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 wrangle-0.7.4/wrangle/col/col_to_multilabel.py
+-rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 wrangle-0.7.4/wrangle/col/col_to_split.py
+-rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 wrangle-0.7.4/wrangle/df/__init__.py
+-rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 wrangle-0.7.4/wrangle/df/df_add_scorecol.py
+-rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 wrangle-0.7.4/wrangle/df/df_clean_colnames.py
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 wrangle-0.7.4/wrangle/df/df_corr_any.py
+-rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 wrangle-0.7.4/wrangle/df/df_corr_extratrees.py
+-rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 wrangle-0.7.4/wrangle/df/df_corr_ols.py
+-rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 wrangle-0.7.4/wrangle/df/df_corr_pearson.py
+-rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 wrangle-0.7.4/wrangle/df/df_corr_randomforest.py
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 wrangle-0.7.4/wrangle/df/df_count_uniques.py
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 wrangle-0.7.4/wrangle/df/df_drop_col.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 wrangle-0.7.4/wrangle/df/df_drop_duplicates.py
+-rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 wrangle-0.7.4/wrangle/df/df_drop_nancols.py
+-rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 wrangle-0.7.4/wrangle/df/df_drop_nanrows.py
+-rw-r--r--   0        0        0     1185 2020-02-02 00:00:00.000000 wrangle-0.7.4/wrangle/df/df_drop_weak.py
+-rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 wrangle-0.7.4/wrangle/df/df_fill_empty.py
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 wrangle-0.7.4/wrangle/df/df_find_nan.py
+-rw-r--r--   0        0        0     1463 2020-02-02 00:00:00.000000 wrangle-0.7.4/wrangle/df/df_groupby_params.py
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 wrangle-0.7.4/wrangle/df/df_impute_nan.py
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 wrangle-0.7.4/wrangle/df/df_merge.py
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 wrangle-0.7.4/wrangle/df/df_parallelize_process.py
+-rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 wrangle-0.7.4/wrangle/df/df_print_values.py
+-rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 wrangle-0.7.4/wrangle/df/df_rename_col.py
+-rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 wrangle-0.7.4/wrangle/df/df_rename_cols.py
+-rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 wrangle-0.7.4/wrangle/df/df_resample_id.py
+-rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 wrangle-0.7.4/wrangle/df/df_resample_stratified.py
+-rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 wrangle-0.7.4/wrangle/df/df_rescale_log.py
+-rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 wrangle-0.7.4/wrangle/df/df_rescale_meanzero.py
+-rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 wrangle-0.7.4/wrangle/df/df_rescale_sqrt.py
+-rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 wrangle-0.7.4/wrangle/df/df_restructure_values.py
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 wrangle-0.7.4/wrangle/df/df_to_binary.py
+-rw-r--r--   0        0        0     1283 2020-02-02 00:00:00.000000 wrangle-0.7.4/wrangle/df/df_to_dfs.py
+-rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 wrangle-0.7.4/wrangle/df/df_to_groupby.py
+-rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 wrangle-0.7.4/wrangle/df/df_to_lower.py
+-rw-r--r--   0        0        0     1173 2020-02-02 00:00:00.000000 wrangle-0.7.4/wrangle/df/df_to_multiclass.py
+-rw-r--r--   0        0        0     1352 2020-02-02 00:00:00.000000 wrangle-0.7.4/wrangle/df/df_to_multilabel.py
+-rw-r--r--   0        0        0     1195 2020-02-02 00:00:00.000000 wrangle-0.7.4/wrangle/df/df_to_numeric.py
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 wrangle-0.7.4/wrangle/df/df_to_xy.py
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 wrangle-0.7.4/wrangle/dic/__init__.py
+-rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 wrangle-0.7.4/wrangle/dic/dic_corr_perc.py
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 wrangle-0.7.4/wrangle/dic/dic_count_complexity.py
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 wrangle-0.7.4/wrangle/dic/dic_resample_values.py
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 wrangle-0.7.4/wrangle/utils/__init__.py
+-rw-r--r--   0        0        0     2361 2020-02-02 00:00:00.000000 wrangle-0.7.4/wrangle/utils/category_labeling.py
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 wrangle-0.7.4/wrangle/utils/connection_check.py
+-rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 wrangle-0.7.4/wrangle/utils/create_datetime_col.py
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 wrangle-0.7.4/wrangle/utils/create_synth_data.py
+-rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 wrangle-0.7.4/wrangle/utils/create_synth_model.py
+-rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 wrangle-0.7.4/wrangle/utils/create_time_sequence.py
+-rw-r--r--   0        0        0     2589 2020-02-02 00:00:00.000000 wrangle-0.7.4/wrangle/utils/datetime_handler.py
+-rw-r--r--   0        0        0     1564 2020-02-02 00:00:00.000000 wrangle-0.7.4/wrangle/utils/groupby_func.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 wrangle-0.7.4/wrangle/utils/int_to_string.py
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 wrangle-0.7.4/wrangle/utils/is_number.py
+-rw-r--r--   0        0        0     1171 2020-02-02 00:00:00.000000 wrangle-0.7.4/wrangle/utils/multi_input_support.py
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 wrangle-0.7.4/wrangle/utils/nan_dropper.py
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 wrangle-0.7.4/wrangle/utils/network_check.py
+-rw-r--r--   0        0        0     1178 2020-02-02 00:00:00.000000 wrangle-0.7.4/wrangle/utils/read_large_csv.py
+-rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 wrangle-0.7.4/wrangle/utils/transform_data.py
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 wrangle-0.7.4/wrangle/utils/value_starts_with.py
+-rw-r--r--   0        0        0     3193 2020-02-02 00:00:00.000000 wrangle-0.7.4/wrangle/utils/wrangler_utils.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 wrangle-0.7.4/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 wrangle-0.7.4/LICENSE
+-rw-r--r--   0        0        0     3186 2020-02-02 00:00:00.000000 wrangle-0.7.4/README.md
+-rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 wrangle-0.7.4/pyproject.toml
+-rw-r--r--   0        0        0     4207 2020-02-02 00:00:00.000000 wrangle-0.7.4/PKG-INFO
```

### Comparing `wrangle-0.7.3/wrangle/array/array_detect_task.py` & `wrangle-0.7.4/wrangle/array/array_detect_task.py`

 * *Files identical despite different names*

### Comparing `wrangle-0.7.3/wrangle/array/array_random_shuffle.py` & `wrangle-0.7.4/wrangle/array/array_random_shuffle.py`

 * *Files identical despite different names*

### Comparing `wrangle-0.7.3/wrangle/array/array_random_weighted.py` & `wrangle-0.7.4/wrangle/array/array_random_weighted.py`

 * *Files identical despite different names*

### Comparing `wrangle-0.7.3/wrangle/array/array_reshape_lstm.py` & `wrangle-0.7.4/wrangle/array/array_reshape_lstm.py`

 * *Files identical despite different names*

### Comparing `wrangle-0.7.3/wrangle/array/array_to_generator.py` & `wrangle-0.7.4/wrangle/array/array_to_generator.py`

 * *Files identical despite different names*

### Comparing `wrangle-0.7.3/wrangle/col/__init__.py` & `wrangle-0.7.4/wrangle/col/__init__.py`

 * *Files identical despite different names*

### Comparing `wrangle-0.7.3/wrangle/col/col_corr_category.py` & `wrangle-0.7.4/wrangle/col/col_corr_category.py`

 * *Files identical despite different names*

### Comparing `wrangle-0.7.3/wrangle/col/col_corr_ols.py` & `wrangle-0.7.4/wrangle/col/col_corr_ols.py`

 * *Files identical despite different names*

### Comparing `wrangle-0.7.3/wrangle/col/col_drop_outliers.py` & `wrangle-0.7.4/wrangle/col/col_drop_outliers.py`

 * *Files identical despite different names*

### Comparing `wrangle-0.7.3/wrangle/col/col_fill_nan.py` & `wrangle-0.7.4/wrangle/col/col_fill_nan.py`

 * *Files identical despite different names*

### Comparing `wrangle-0.7.3/wrangle/col/col_groupby_cdf.py` & `wrangle-0.7.4/wrangle/col/col_groupby_cdf.py`

 * *Files identical despite different names*

### Comparing `wrangle-0.7.3/wrangle/col/col_groupby_pdf.py` & `wrangle-0.7.4/wrangle/col/col_groupby_pdf.py`

 * *Files identical despite different names*

### Comparing `wrangle-0.7.3/wrangle/col/col_groupby_stats.py` & `wrangle-0.7.4/wrangle/col/col_groupby_stats.py`

 * *Files identical despite different names*

### Comparing `wrangle-0.7.3/wrangle/col/col_impute_nan.py` & `wrangle-0.7.4/wrangle/col/col_impute_nan.py`

 * *Files identical despite different names*

### Comparing `wrangle-0.7.3/wrangle/col/col_move_place.py` & `wrangle-0.7.4/wrangle/col/col_move_place.py`

 * *Files identical despite different names*

### Comparing `wrangle-0.7.3/wrangle/col/col_resample_interval.py` & `wrangle-0.7.4/wrangle/col/col_resample_interval.py`

 * *Files identical despite different names*

### Comparing `wrangle-0.7.3/wrangle/col/col_rescale_max.py` & `wrangle-0.7.4/wrangle/col/col_rescale_max.py`

 * *Files identical despite different names*

### Comparing `wrangle-0.7.3/wrangle/col/col_to_biclass.py` & `wrangle-0.7.4/wrangle/col/col_to_biclass.py`

 * *Files identical despite different names*

### Comparing `wrangle-0.7.3/wrangle/col/col_to_binary.py` & `wrangle-0.7.4/wrangle/col/col_to_binary.py`

 * *Files identical despite different names*

### Comparing `wrangle-0.7.3/wrangle/col/col_to_buckets.py` & `wrangle-0.7.4/wrangle/col/col_to_buckets.py`

 * *Files identical despite different names*

### Comparing `wrangle-0.7.3/wrangle/col/col_to_cols.py` & `wrangle-0.7.4/wrangle/col/col_to_cols.py`

 * *Files identical despite different names*

### Comparing `wrangle-0.7.3/wrangle/col/col_to_multilabel.py` & `wrangle-0.7.4/wrangle/col/col_to_multilabel.py`

 * *Files identical despite different names*

### Comparing `wrangle-0.7.3/wrangle/col/col_to_split.py` & `wrangle-0.7.4/wrangle/col/col_to_split.py`

 * *Files identical despite different names*

### Comparing `wrangle-0.7.3/wrangle/df/__init__.py` & `wrangle-0.7.4/wrangle/df/__init__.py`

 * *Files identical despite different names*

### Comparing `wrangle-0.7.3/wrangle/df/df_add_scorecol.py` & `wrangle-0.7.4/wrangle/df/df_add_scorecol.py`

 * *Files identical despite different names*

### Comparing `wrangle-0.7.3/wrangle/df/df_clean_colnames.py` & `wrangle-0.7.4/wrangle/df/df_clean_colnames.py`

 * *Files identical despite different names*

### Comparing `wrangle-0.7.3/wrangle/df/df_corr_extratrees.py` & `wrangle-0.7.4/wrangle/df/df_corr_extratrees.py`

 * *Files identical despite different names*

### Comparing `wrangle-0.7.3/wrangle/df/df_corr_ols.py` & `wrangle-0.7.4/wrangle/df/df_corr_ols.py`

 * *Files identical despite different names*

### Comparing `wrangle-0.7.3/wrangle/df/df_corr_pearson.py` & `wrangle-0.7.4/wrangle/df/df_corr_pearson.py`

 * *Files identical despite different names*

### Comparing `wrangle-0.7.3/wrangle/df/df_corr_randomforest.py` & `wrangle-0.7.4/wrangle/df/df_corr_randomforest.py`

 * *Files identical despite different names*

### Comparing `wrangle-0.7.3/wrangle/df/df_drop_nancols.py` & `wrangle-0.7.4/wrangle/df/df_drop_nancols.py`

 * *Files identical despite different names*

### Comparing `wrangle-0.7.3/wrangle/df/df_drop_nanrows.py` & `wrangle-0.7.4/wrangle/df/df_drop_nanrows.py`

 * *Files identical despite different names*

### Comparing `wrangle-0.7.3/wrangle/df/df_drop_weak.py` & `wrangle-0.7.4/wrangle/df/df_drop_weak.py`

 * *Files identical despite different names*

### Comparing `wrangle-0.7.3/wrangle/df/df_fill_empty.py` & `wrangle-0.7.4/wrangle/df/df_fill_empty.py`

 * *Files identical despite different names*

### Comparing `wrangle-0.7.3/wrangle/df/df_find_nan.py` & `wrangle-0.7.4/wrangle/df/df_find_nan.py`

 * *Files identical despite different names*

### Comparing `wrangle-0.7.3/wrangle/df/df_groupby_params.py` & `wrangle-0.7.4/wrangle/df/df_groupby_params.py`

 * *Files identical despite different names*

### Comparing `wrangle-0.7.3/wrangle/df/df_impute_nan.py` & `wrangle-0.7.4/wrangle/df/df_impute_nan.py`

 * *Files identical despite different names*

### Comparing `wrangle-0.7.3/wrangle/df/df_parallelize_process.py` & `wrangle-0.7.4/wrangle/df/df_parallelize_process.py`

 * *Files identical despite different names*

### Comparing `wrangle-0.7.3/wrangle/df/df_rename_col.py` & `wrangle-0.7.4/wrangle/df/df_rename_col.py`

 * *Files identical despite different names*

### Comparing `wrangle-0.7.3/wrangle/df/df_rename_cols.py` & `wrangle-0.7.4/wrangle/df/df_rename_cols.py`

 * *Files identical despite different names*

### Comparing `wrangle-0.7.3/wrangle/df/df_resample_id.py` & `wrangle-0.7.4/wrangle/df/df_resample_id.py`

 * *Files identical despite different names*

### Comparing `wrangle-0.7.3/wrangle/df/df_resample_stratified.py` & `wrangle-0.7.4/wrangle/df/df_resample_stratified.py`

 * *Files identical despite different names*

### Comparing `wrangle-0.7.3/wrangle/df/df_rescale_log.py` & `wrangle-0.7.4/wrangle/df/df_rescale_log.py`

 * *Files identical despite different names*

### Comparing `wrangle-0.7.3/wrangle/df/df_rescale_meanzero.py` & `wrangle-0.7.4/wrangle/df/df_rescale_meanzero.py`

 * *Files identical despite different names*

### Comparing `wrangle-0.7.3/wrangle/df/df_rescale_sqrt.py` & `wrangle-0.7.4/wrangle/df/df_rescale_sqrt.py`

 * *Files identical despite different names*

### Comparing `wrangle-0.7.3/wrangle/df/df_restructure_values.py` & `wrangle-0.7.4/wrangle/df/df_restructure_values.py`

 * *Files identical despite different names*

### Comparing `wrangle-0.7.3/wrangle/df/df_to_dfs.py` & `wrangle-0.7.4/wrangle/df/df_to_dfs.py`

 * *Files identical despite different names*

### Comparing `wrangle-0.7.3/wrangle/df/df_to_lower.py` & `wrangle-0.7.4/wrangle/df/df_to_lower.py`

 * *Files identical despite different names*

### Comparing `wrangle-0.7.3/wrangle/df/df_to_multiclass.py` & `wrangle-0.7.4/wrangle/df/df_to_multiclass.py`

 * *Files identical despite different names*

### Comparing `wrangle-0.7.3/wrangle/df/df_to_multilabel.py` & `wrangle-0.7.4/wrangle/df/df_to_multilabel.py`

 * *Files identical despite different names*

### Comparing `wrangle-0.7.3/wrangle/df/df_to_numeric.py` & `wrangle-0.7.4/wrangle/df/df_to_numeric.py`

 * *Files identical despite different names*

### Comparing `wrangle-0.7.3/wrangle/dic/dic_corr_perc.py` & `wrangle-0.7.4/wrangle/dic/dic_corr_perc.py`

 * *Files identical despite different names*

### Comparing `wrangle-0.7.3/wrangle/utils/category_labeling.py` & `wrangle-0.7.4/wrangle/utils/category_labeling.py`

 * *Files identical despite different names*

### Comparing `wrangle-0.7.3/wrangle/utils/create_datetime_col.py` & `wrangle-0.7.4/wrangle/utils/create_datetime_col.py`

 * *Files identical despite different names*

### Comparing `wrangle-0.7.3/wrangle/utils/create_synth_data.py` & `wrangle-0.7.4/wrangle/utils/create_synth_data.py`

 * *Files identical despite different names*

### Comparing `wrangle-0.7.3/wrangle/utils/create_synth_model.py` & `wrangle-0.7.4/wrangle/utils/create_synth_model.py`

 * *Files identical despite different names*

### Comparing `wrangle-0.7.3/wrangle/utils/create_time_sequence.py` & `wrangle-0.7.4/wrangle/utils/create_time_sequence.py`

 * *Files identical despite different names*

### Comparing `wrangle-0.7.3/wrangle/utils/datetime_handler.py` & `wrangle-0.7.4/wrangle/utils/datetime_handler.py`

 * *Files identical despite different names*

### Comparing `wrangle-0.7.3/wrangle/utils/groupby_func.py` & `wrangle-0.7.4/wrangle/utils/groupby_func.py`

 * *Files identical despite different names*

### Comparing `wrangle-0.7.3/wrangle/utils/multi_input_support.py` & `wrangle-0.7.4/wrangle/utils/multi_input_support.py`

 * *Files identical despite different names*

### Comparing `wrangle-0.7.3/wrangle/utils/nan_dropper.py` & `wrangle-0.7.4/wrangle/utils/nan_dropper.py`

 * *Files identical despite different names*

### Comparing `wrangle-0.7.3/wrangle/utils/read_large_csv.py` & `wrangle-0.7.4/wrangle/utils/read_large_csv.py`

 * *Files identical despite different names*

### Comparing `wrangle-0.7.3/wrangle/utils/transform_data.py` & `wrangle-0.7.4/wrangle/utils/transform_data.py`

 * *Files identical despite different names*

### Comparing `wrangle-0.7.3/wrangle/utils/value_starts_with.py` & `wrangle-0.7.4/wrangle/utils/value_starts_with.py`

 * *Files identical despite different names*

### Comparing `wrangle-0.7.3/wrangle/utils/wrangler_utils.py` & `wrangle-0.7.4/wrangle/utils/wrangler_utils.py`

 * *Files identical despite different names*

### Comparing `wrangle-0.7.3/LICENSE` & `wrangle-0.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `wrangle-0.7.3/README.md` & `wrangle-0.7.4/README.md`

 * *Files identical despite different names*

### Comparing `wrangle-0.7.3/pyproject.toml` & `wrangle-0.7.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `wrangle-0.7.3/PKG-INFO` & `wrangle-0.7.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: wrangle
-Version: 0.7.3
+Version: 0.7.4
 Summary: Wrangle - Data Preparation for Deep Learning
 Project-URL: Download, https://github.com/autonomio/wrangle/
 Project-URL: Homepage, http://autonom.io
 Author-email: Mikko Kotila <mailme@mikkokotila.com>
 Maintainer-email: Mikko Kotila <mailme@mikkokotila.com>
 License-Expression: MIT
 License-File: LICENSE
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.3 Name: wrangle Version: 0.7.3 Summary: Wrangle - Data
+Metadata-Version: 2.3 Name: wrangle Version: 0.7.4 Summary: Wrangle - Data
 Preparation for Deep Learning Project-URL: Download, https://github.com/
 autonomio/wrangle/ Project-URL: Homepage, http://autonom.io Author-email: Mikko
 Kotila
 mikkokotila.com> Maintainer-email: Mikko Kotila
 mikkokotila.com> License-Expression: MIT License-File: LICENSE Classifier:
 Intended Audience :: Science/Research Classifier: License :: OSI Approved ::
 MIT License Classifier: Operating System :: MacOS Classifier: Operating System
```

