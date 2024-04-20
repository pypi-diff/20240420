# Comparing `tmp/stanza-1.8.1.tar.gz` & `tmp/stanza-1.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stanza-1.8.1.tar", last modified: Fri Mar  1 06:44:43 2024, max compression
+gzip compressed data, was "stanza-1.8.2.tar", last modified: Sat Apr 20 16:32:24 2024, max compression
```

## Comparing `stanza-1.8.1.tar` & `stanza-1.8.2.tar`

### file list

```diff
@@ -1,527 +1,535 @@
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-03-01 06:44:43.230464 stanza-1.8.1/
--rw-rw-r--   0 john      (1000) john      (1000)      603 2022-07-26 21:49:07.000000 stanza-1.8.1/LICENSE
--rw-r--r--   0 john      (1000) john      (1000)    13192 2024-03-01 06:44:43.230464 stanza-1.8.1/PKG-INFO
--rw-rw-r--   0 john      (1000) john      (1000)    11336 2024-01-19 08:13:21.000000 stanza-1.8.1/README.md
--rw-rw-r--   0 john      (1000) john      (1000)       38 2024-03-01 06:44:43.230464 stanza-1.8.1/setup.cfg
--rw-rw-r--   0 john      (1000) john      (1000)     4774 2024-01-19 08:13:21.000000 stanza-1.8.1/setup.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-03-01 06:44:43.052464 stanza-1.8.1/stanza/
--rw-rw-r--   0 john      (1000) john      (1000)     1021 2023-06-22 00:27:12.000000 stanza-1.8.1/stanza/__init__.py
--rw-rw-r--   0 john      (1000) john      (1000)      105 2024-03-01 06:43:51.000000 stanza-1.8.1/stanza/_version.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-03-01 06:44:43.054464 stanza-1.8.1/stanza/models/
--rw-rw-r--   0 john      (1000) john      (1000)        0 2022-07-26 21:49:07.000000 stanza-1.8.1/stanza/models/__init__.py
--rw-rw-r--   0 john      (1000) john      (1000)       83 2022-07-26 21:49:07.000000 stanza-1.8.1/stanza/models/_training_logging.py
--rw-rw-r--   0 john      (1000) john      (1000)    16184 2024-01-19 08:13:21.000000 stanza-1.8.1/stanza/models/charlm.py
--rw-rw-r--   0 john      (1000) john      (1000)    35200 2024-02-26 08:15:40.000000 stanza-1.8.1/stanza/models/classifier.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-03-01 06:44:43.055464 stanza-1.8.1/stanza/models/classifiers/
--rw-rw-r--   0 john      (1000) john      (1000)        0 2022-07-26 21:49:07.000000 stanza-1.8.1/stanza/models/classifiers/__init__.py
--rw-rw-r--   0 john      (1000) john      (1000)     1938 2023-09-18 14:41:48.000000 stanza-1.8.1/stanza/models/classifiers/base_classifier.py
--rw-rw-r--   0 john      (1000) john      (1000)    26763 2024-02-26 08:15:40.000000 stanza-1.8.1/stanza/models/classifiers/cnn_classifier.py
--rw-rw-r--   0 john      (1000) john      (1000)     4056 2024-02-26 08:15:40.000000 stanza-1.8.1/stanza/models/classifiers/constituency_classifier.py
--rw-rw-r--   0 john      (1000) john      (1000)     6069 2024-02-26 08:15:40.000000 stanza-1.8.1/stanza/models/classifiers/data.py
--rw-rw-r--   0 john      (1000) john      (1000)     2166 2023-09-18 14:41:48.000000 stanza-1.8.1/stanza/models/classifiers/iterate_test.py
--rw-rw-r--   0 john      (1000) john      (1000)    13703 2024-02-26 08:15:40.000000 stanza-1.8.1/stanza/models/classifiers/trainer.py
--rw-rw-r--   0 john      (1000) john      (1000)     1054 2023-09-18 14:41:48.000000 stanza-1.8.1/stanza/models/classifiers/utils.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-03-01 06:44:43.058464 stanza-1.8.1/stanza/models/common/
--rw-rw-r--   0 john      (1000) john      (1000)        0 2022-07-26 21:49:07.000000 stanza-1.8.1/stanza/models/common/__init__.py
--rw-rw-r--   0 john      (1000) john      (1000)     4481 2024-02-26 08:15:40.000000 stanza-1.8.1/stanza/models/common/beam.py
--rw-rw-r--   0 john      (1000) john      (1000)    21559 2024-02-26 08:15:40.000000 stanza-1.8.1/stanza/models/common/bert_embedding.py
--rw-rw-r--   0 john      (1000) john      (1000)     3582 2022-07-26 21:49:07.000000 stanza-1.8.1/stanza/models/common/biaffine.py
--rw-rw-r--   0 john      (1000) john      (1000)     2075 2024-01-19 08:13:21.000000 stanza-1.8.1/stanza/models/common/build_short_name_to_treebank.py
--rw-rw-r--   0 john      (1000) john      (1000)    15704 2024-02-26 08:15:40.000000 stanza-1.8.1/stanza/models/common/char_model.py
--rw-rw-r--   0 john      (1000) john      (1000)    11900 2024-01-19 08:13:21.000000 stanza-1.8.1/stanza/models/common/chuliu_edmonds.py
--rw-rw-r--   0 john      (1000) john      (1000)    14459 2024-02-26 08:15:40.000000 stanza-1.8.1/stanza/models/common/constant.py
--rw-rw-r--   0 john      (1000) john      (1000)     1856 2023-09-18 14:41:48.000000 stanza-1.8.1/stanza/models/common/convert_pretrain.py
--rw-rw-r--   0 john      (1000) john      (1000)     1171 2023-06-22 00:27:12.000000 stanza-1.8.1/stanza/models/common/count_ner_coverage.py
--rw-rw-r--   0 john      (1000) john      (1000)     1535 2023-06-22 00:27:12.000000 stanza-1.8.1/stanza/models/common/count_pretrain_coverage.py
--rw-rw-r--   0 john      (1000) john      (1000)     5915 2024-01-19 08:13:21.000000 stanza-1.8.1/stanza/models/common/crf.py
--rw-rw-r--   0 john      (1000) john      (1000)     6111 2024-01-19 08:13:21.000000 stanza-1.8.1/stanza/models/common/data.py
--rw-rw-r--   0 john      (1000) john      (1000)    66593 2024-02-26 08:15:40.000000 stanza-1.8.1/stanza/models/common/doc.py
--rw-rw-r--   0 john      (1000) john      (1000)     2858 2022-07-26 21:49:07.000000 stanza-1.8.1/stanza/models/common/dropout.py
--rw-rw-r--   0 john      (1000) john      (1000)      452 2024-01-19 08:13:21.000000 stanza-1.8.1/stanza/models/common/exceptions.py
--rw-rw-r--   0 john      (1000) john      (1000)     3941 2024-01-19 08:13:21.000000 stanza-1.8.1/stanza/models/common/foundation_cache.py
--rw-rw-r--   0 john      (1000) john      (1000)     5180 2023-06-22 00:27:12.000000 stanza-1.8.1/stanza/models/common/hlstm.py
--rw-rw-r--   0 john      (1000) john      (1000)     2638 2023-09-18 14:41:48.000000 stanza-1.8.1/stanza/models/common/large_margin_loss.py
--rw-rw-r--   0 john      (1000) john      (1000)     4716 2023-09-18 14:41:48.000000 stanza-1.8.1/stanza/models/common/loss.py
--rw-rw-r--   0 john      (1000) john      (1000)     1265 2023-09-18 14:41:48.000000 stanza-1.8.1/stanza/models/common/maxout_linear.py
--rw-rw-r--   0 john      (1000) john      (1000)     4855 2022-07-26 21:49:07.000000 stanza-1.8.1/stanza/models/common/packed_lstm.py
--rw-rw-r--   0 john      (1000) john      (1000)     3608 2024-02-26 08:15:40.000000 stanza-1.8.1/stanza/models/common/peft_config.py
--rw-rw-r--   0 john      (1000) john      (1000)    11012 2024-02-26 08:15:40.000000 stanza-1.8.1/stanza/models/common/pretrain.py
--rw-rw-r--   0 john      (1000) john      (1000)      221 2022-07-26 21:49:07.000000 stanza-1.8.1/stanza/models/common/seq2seq_constant.py
--rw-rw-r--   0 john      (1000) john      (1000)    13578 2024-01-19 08:13:21.000000 stanza-1.8.1/stanza/models/common/seq2seq_model.py
--rw-rw-r--   0 john      (1000) john      (1000)     8483 2023-06-22 00:27:12.000000 stanza-1.8.1/stanza/models/common/seq2seq_modules.py
--rw-rw-r--   0 john      (1000) john      (1000)     3334 2023-09-07 05:52:02.000000 stanza-1.8.1/stanza/models/common/seq2seq_utils.py
--rw-rw-r--   0 john      (1000) john      (1000)    29850 2024-01-19 08:13:21.000000 stanza-1.8.1/stanza/models/common/short_name_to_treebank.py
--rw-rw-r--   0 john      (1000) john      (1000)     1147 2023-09-18 14:41:48.000000 stanza-1.8.1/stanza/models/common/stanza_object.py
--rw-rw-r--   0 john      (1000) john      (1000)      645 2022-07-26 21:49:07.000000 stanza-1.8.1/stanza/models/common/trainer.py
--rw-rw-r--   0 john      (1000) john      (1000)    30382 2024-02-26 08:15:40.000000 stanza-1.8.1/stanza/models/common/utils.py
--rw-rw-r--   0 john      (1000) john      (1000)     9703 2024-01-19 08:13:21.000000 stanza-1.8.1/stanza/models/common/vocab.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-03-01 06:44:43.061464 stanza-1.8.1/stanza/models/constituency/
--rw-rw-r--   0 john      (1000) john      (1000)        0 2023-06-22 00:27:12.000000 stanza-1.8.1/stanza/models/constituency/__init__.py
--rw-rw-r--   0 john      (1000) john      (1000)    18762 2024-02-26 08:15:40.000000 stanza-1.8.1/stanza/models/constituency/base_model.py
--rw-rw-r--   0 john      (1000) john      (1000)     2388 2024-02-26 08:15:40.000000 stanza-1.8.1/stanza/models/constituency/dynamic_oracle.py
--rw-rw-r--   0 john      (1000) john      (1000)    13793 2024-02-26 08:15:40.000000 stanza-1.8.1/stanza/models/constituency/ensemble.py
--rw-rw-r--   0 john      (1000) john      (1000)     1249 2023-09-07 05:52:02.000000 stanza-1.8.1/stanza/models/constituency/evaluate_treebanks.py
--rw-rw-r--   0 john      (1000) john      (1000)    20875 2024-02-26 08:15:40.000000 stanza-1.8.1/stanza/models/constituency/in_order_oracle.py
--rw-rw-r--   0 john      (1000) john      (1000)    31043 2023-09-18 14:41:48.000000 stanza-1.8.1/stanza/models/constituency/label_attention.py
--rw-rw-r--   0 john      (1000) john      (1000)    68137 2024-02-26 08:15:40.000000 stanza-1.8.1/stanza/models/constituency/lstm_model.py
--rw-rw-r--   0 john      (1000) john      (1000)     3605 2023-09-07 05:52:02.000000 stanza-1.8.1/stanza/models/constituency/lstm_tree_stack.py
--rw-rw-r--   0 john      (1000) john      (1000)    30651 2024-02-26 08:15:40.000000 stanza-1.8.1/stanza/models/constituency/parse_transitions.py
--rw-rw-r--   0 john      (1000) john      (1000)    19313 2023-09-18 14:41:48.000000 stanza-1.8.1/stanza/models/constituency/parse_tree.py
--rw-rw-r--   0 john      (1000) john      (1000)    11165 2023-09-07 05:52:02.000000 stanza-1.8.1/stanza/models/constituency/partitioned_transformer.py
--rw-rw-r--   0 john      (1000) john      (1000)     3049 2023-09-18 14:41:48.000000 stanza-1.8.1/stanza/models/constituency/positional_encoding.py
--rw-rw-r--   0 john      (1000) john      (1000)     6579 2024-03-01 06:43:51.000000 stanza-1.8.1/stanza/models/constituency/retagging.py
--rw-rw-r--   0 john      (1000) john      (1000)     2186 2023-09-18 14:41:48.000000 stanza-1.8.1/stanza/models/constituency/score_converted_dependencies.py
--rw-rw-r--   0 john      (1000) john      (1000)    25468 2024-02-26 08:15:40.000000 stanza-1.8.1/stanza/models/constituency/top_down_oracle.py
--rw-rw-r--   0 john      (1000) john      (1000)    61881 2024-02-26 08:15:40.000000 stanza-1.8.1/stanza/models/constituency/trainer.py
--rw-rw-r--   0 john      (1000) john      (1000)     7555 2023-09-18 14:41:48.000000 stanza-1.8.1/stanza/models/constituency/transformer_tree_stack.py
--rw-rw-r--   0 john      (1000) john      (1000)     6117 2024-02-26 08:15:40.000000 stanza-1.8.1/stanza/models/constituency/transition_sequence.py
--rw-rw-r--   0 john      (1000) john      (1000)     6123 2023-09-18 14:41:48.000000 stanza-1.8.1/stanza/models/constituency/tree_embedding.py
--rw-rw-r--   0 john      (1000) john      (1000)     9142 2024-01-19 08:13:21.000000 stanza-1.8.1/stanza/models/constituency/tree_reader.py
--rw-rw-r--   0 john      (1000) john      (1000)     2033 2023-09-18 14:41:48.000000 stanza-1.8.1/stanza/models/constituency/tree_stack.py
--rw-rw-r--   0 john      (1000) john      (1000)    11719 2024-02-26 08:15:40.000000 stanza-1.8.1/stanza/models/constituency/utils.py
--rw-rw-r--   0 john      (1000) john      (1000)    51374 2024-03-01 06:43:51.000000 stanza-1.8.1/stanza/models/constituency_parser.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-03-01 06:44:43.063464 stanza-1.8.1/stanza/models/coref/
--rw-rw-r--   0 john      (1000) john      (1000)        0 2024-01-19 08:13:21.000000 stanza-1.8.1/stanza/models/coref/__init__.py
--rw-rw-r--   0 john      (1000) john      (1000)     4072 2024-01-19 08:13:21.000000 stanza-1.8.1/stanza/models/coref/anaphoricity_scorer.py
--rw-rw-r--   0 john      (1000) john      (1000)     2623 2024-01-19 08:13:21.000000 stanza-1.8.1/stanza/models/coref/bert.py
--rw-rw-r--   0 john      (1000) john      (1000)     2863 2024-01-19 08:13:21.000000 stanza-1.8.1/stanza/models/coref/cluster_checker.py
--rw-rw-r--   0 john      (1000) john      (1000)     1352 2024-01-19 08:13:21.000000 stanza-1.8.1/stanza/models/coref/config.py
--rw-rw-r--   0 john      (1000) john      (1000)     2675 2024-01-19 08:13:21.000000 stanza-1.8.1/stanza/models/coref/conll.py
--rw-rw-r--   0 john      (1000) john      (1000)      687 2024-01-19 08:13:21.000000 stanza-1.8.1/stanza/models/coref/const.py
--rw-rw-r--   0 john      (1000) john      (1000)     1377 2024-01-19 08:13:21.000000 stanza-1.8.1/stanza/models/coref/coref_chain.py
--rw-rw-r--   0 john      (1000) john      (1000)     1465 2024-01-19 08:13:21.000000 stanza-1.8.1/stanza/models/coref/loss.py
--rw-rw-r--   0 john      (1000) john      (1000)    29455 2024-02-26 08:15:40.000000 stanza-1.8.1/stanza/models/coref/model.py
--rw-rw-r--   0 john      (1000) john      (1000)     3092 2024-01-19 08:13:21.000000 stanza-1.8.1/stanza/models/coref/pairwise_encoder.py
--rw-rw-r--   0 john      (1000) john      (1000)     2167 2024-01-19 08:13:21.000000 stanza-1.8.1/stanza/models/coref/predict.py
--rw-rw-r--   0 john      (1000) john      (1000)     2210 2024-01-19 08:13:21.000000 stanza-1.8.1/stanza/models/coref/rough_scorer.py
--rw-rw-r--   0 john      (1000) john      (1000)     6032 2024-01-20 04:09:40.000000 stanza-1.8.1/stanza/models/coref/span_predictor.py
--rw-rw-r--   0 john      (1000) john      (1000)      749 2024-01-19 08:13:21.000000 stanza-1.8.1/stanza/models/coref/tokenizer_customization.py
--rw-rw-r--   0 john      (1000) john      (1000)      993 2024-01-19 08:13:21.000000 stanza-1.8.1/stanza/models/coref/utils.py
--rw-rw-r--   0 john      (1000) john      (1000)     4040 2024-01-19 08:13:21.000000 stanza-1.8.1/stanza/models/coref/word_encoder.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-03-01 06:44:43.063464 stanza-1.8.1/stanza/models/depparse/
--rw-rw-r--   0 john      (1000) john      (1000)        0 2022-07-26 21:49:07.000000 stanza-1.8.1/stanza/models/depparse/__init__.py
--rw-rw-r--   0 john      (1000) john      (1000)     9717 2024-02-26 08:15:40.000000 stanza-1.8.1/stanza/models/depparse/data.py
--rw-rw-r--   0 john      (1000) john      (1000)    15517 2024-02-26 08:15:40.000000 stanza-1.8.1/stanza/models/depparse/model.py
--rw-rw-r--   0 john      (1000) john      (1000)     2431 2023-09-18 14:41:48.000000 stanza-1.8.1/stanza/models/depparse/scorer.py
--rw-rw-r--   0 john      (1000) john      (1000)    11923 2024-02-26 08:15:40.000000 stanza-1.8.1/stanza/models/depparse/trainer.py
--rw-rw-r--   0 john      (1000) john      (1000)     2297 2024-01-19 08:13:21.000000 stanza-1.8.1/stanza/models/identity_lemmatizer.py
--rw-rw-r--   0 john      (1000) john      (1000)    10266 2024-01-19 08:13:21.000000 stanza-1.8.1/stanza/models/lang_identifier.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-03-01 06:44:43.064464 stanza-1.8.1/stanza/models/langid/
--rw-rw-r--   0 john      (1000) john      (1000)        0 2023-06-22 00:27:12.000000 stanza-1.8.1/stanza/models/langid/__init__.py
--rw-rw-r--   0 john      (1000) john      (1000)     8627 2023-06-22 00:27:12.000000 stanza-1.8.1/stanza/models/langid/create_ud_data.py
--rw-rw-r--   0 john      (1000) john      (1000)     5206 2023-09-18 14:41:48.000000 stanza-1.8.1/stanza/models/langid/data.py
--rw-rw-r--   0 john      (1000) john      (1000)     4771 2024-01-19 08:13:21.000000 stanza-1.8.1/stanza/models/langid/model.py
--rw-rw-r--   0 john      (1000) john      (1000)     1778 2024-01-19 08:13:21.000000 stanza-1.8.1/stanza/models/langid/trainer.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-03-01 06:44:43.064464 stanza-1.8.1/stanza/models/lemma/
--rw-rw-r--   0 john      (1000) john      (1000)        0 2022-07-26 21:49:07.000000 stanza-1.8.1/stanza/models/lemma/__init__.py
--rw-rw-r--   0 john      (1000) john      (1000)     5957 2024-02-26 08:15:40.000000 stanza-1.8.1/stanza/models/lemma/data.py
--rw-rw-r--   0 john      (1000) john      (1000)      631 2022-07-26 21:49:07.000000 stanza-1.8.1/stanza/models/lemma/edit.py
--rw-rw-r--   0 john      (1000) john      (1000)      350 2023-09-07 05:52:02.000000 stanza-1.8.1/stanza/models/lemma/scorer.py
--rw-rw-r--   0 john      (1000) john      (1000)    10141 2024-02-26 08:15:40.000000 stanza-1.8.1/stanza/models/lemma/trainer.py
--rw-rw-r--   0 john      (1000) john      (1000)      649 2022-07-26 21:49:07.000000 stanza-1.8.1/stanza/models/lemma/vocab.py
--rw-rw-r--   0 john      (1000) john      (1000)    14123 2024-02-26 08:15:40.000000 stanza-1.8.1/stanza/models/lemmatizer.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-03-01 06:44:43.065464 stanza-1.8.1/stanza/models/mwt/
--rw-rw-r--   0 john      (1000) john      (1000)        0 2022-07-26 21:49:07.000000 stanza-1.8.1/stanza/models/mwt/__init__.py
--rw-rw-r--   0 john      (1000) john      (1000)     3545 2023-06-22 00:27:12.000000 stanza-1.8.1/stanza/models/mwt/data.py
--rw-rw-r--   0 john      (1000) john      (1000)      348 2023-09-07 05:52:02.000000 stanza-1.8.1/stanza/models/mwt/scorer.py
--rw-rw-r--   0 john      (1000) john      (1000)     5541 2024-01-19 08:13:21.000000 stanza-1.8.1/stanza/models/mwt/trainer.py
--rw-rw-r--   0 john      (1000) john      (1000)     3549 2024-01-19 08:13:21.000000 stanza-1.8.1/stanza/models/mwt/utils.py
--rw-rw-r--   0 john      (1000) john      (1000)      506 2022-07-26 21:49:07.000000 stanza-1.8.1/stanza/models/mwt/vocab.py
--rw-rw-r--   0 john      (1000) john      (1000)    12548 2024-01-19 08:13:21.000000 stanza-1.8.1/stanza/models/mwt_expander.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-03-01 06:44:43.065464 stanza-1.8.1/stanza/models/ner/
--rw-rw-r--   0 john      (1000) john      (1000)        0 2022-07-26 21:49:07.000000 stanza-1.8.1/stanza/models/ner/__init__.py
--rw-rw-r--   0 john      (1000) john      (1000)     9261 2024-01-19 08:13:21.000000 stanza-1.8.1/stanza/models/ner/data.py
--rw-rw-r--   0 john      (1000) john      (1000)    15449 2024-02-26 08:15:40.000000 stanza-1.8.1/stanza/models/ner/model.py
--rw-rw-r--   0 john      (1000) john      (1000)     6364 2024-01-19 08:13:21.000000 stanza-1.8.1/stanza/models/ner/scorer.py
--rw-rw-r--   0 john      (1000) john      (1000)    13018 2024-02-26 08:15:40.000000 stanza-1.8.1/stanza/models/ner/trainer.py
--rw-rw-r--   0 john      (1000) john      (1000)    11202 2024-01-19 08:13:21.000000 stanza-1.8.1/stanza/models/ner/utils.py
--rw-rw-r--   0 john      (1000) john      (1000)     2601 2024-01-19 08:13:21.000000 stanza-1.8.1/stanza/models/ner/vocab.py
--rw-rw-r--   0 john      (1000) john      (1000)    26061 2024-02-26 08:15:40.000000 stanza-1.8.1/stanza/models/ner_tagger.py
--rw-rw-r--   0 john      (1000) john      (1000)    21743 2024-02-26 08:15:40.000000 stanza-1.8.1/stanza/models/parser.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-03-01 06:44:43.066464 stanza-1.8.1/stanza/models/pos/
--rw-rw-r--   0 john      (1000) john      (1000)        0 2022-07-26 21:49:07.000000 stanza-1.8.1/stanza/models/pos/__init__.py
--rw-rw-r--   0 john      (1000) john      (1000)     5626 2023-06-22 00:27:12.000000 stanza-1.8.1/stanza/models/pos/build_xpos_vocab_factory.py
--rw-rw-r--   0 john      (1000) john      (1000)    14020 2024-02-26 08:15:40.000000 stanza-1.8.1/stanza/models/pos/data.py
--rw-rw-r--   0 john      (1000) john      (1000)    14043 2024-02-26 08:15:40.000000 stanza-1.8.1/stanza/models/pos/model.py
--rw-rw-r--   0 john      (1000) john      (1000)      670 2024-01-19 08:13:21.000000 stanza-1.8.1/stanza/models/pos/scorer.py
--rw-rw-r--   0 john      (1000) john      (1000)     6661 2024-03-01 06:43:51.000000 stanza-1.8.1/stanza/models/pos/trainer.py
--rw-rw-r--   0 john      (1000) john      (1000)     2691 2023-09-07 05:52:02.000000 stanza-1.8.1/stanza/models/pos/vocab.py
--rw-rw-r--   0 john      (1000) john      (1000)     9586 2023-09-07 05:52:02.000000 stanza-1.8.1/stanza/models/pos/xpos_vocab_factory.py
--rw-rw-r--   0 john      (1000) john      (1000)     1595 2023-06-22 00:27:12.000000 stanza-1.8.1/stanza/models/pos/xpos_vocab_utils.py
--rw-rw-r--   0 john      (1000) john      (1000)    21940 2024-02-25 01:10:00.000000 stanza-1.8.1/stanza/models/tagger.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-03-01 06:44:43.067464 stanza-1.8.1/stanza/models/tokenization/
--rw-rw-r--   0 john      (1000) john      (1000)        0 2022-07-26 21:49:07.000000 stanza-1.8.1/stanza/models/tokenization/__init__.py
--rw-rw-r--   0 john      (1000) john      (1000)    19164 2023-09-07 05:52:02.000000 stanza-1.8.1/stanza/models/tokenization/data.py
--rw-rw-r--   0 john      (1000) john      (1000)     3834 2024-01-19 08:10:20.000000 stanza-1.8.1/stanza/models/tokenization/model.py
--rw-rw-r--   0 john      (1000) john      (1000)     3788 2024-01-19 08:13:21.000000 stanza-1.8.1/stanza/models/tokenization/tokenize_files.py
--rw-rw-r--   0 john      (1000) john      (1000)     3783 2024-01-19 08:13:21.000000 stanza-1.8.1/stanza/models/tokenization/trainer.py
--rw-rw-r--   0 john      (1000) john      (1000)    26104 2024-02-26 08:15:40.000000 stanza-1.8.1/stanza/models/tokenization/utils.py
--rw-rw-r--   0 john      (1000) john      (1000)     1097 2023-06-22 00:27:12.000000 stanza-1.8.1/stanza/models/tokenization/vocab.py
--rw-rw-r--   0 john      (1000) john      (1000)    13799 2024-01-19 08:13:21.000000 stanza-1.8.1/stanza/models/tokenizer.py
--rw-rw-r--   0 john      (1000) john      (1000)     6609 2024-02-26 08:15:40.000000 stanza-1.8.1/stanza/models/wl_coref.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-03-01 06:44:43.069464 stanza-1.8.1/stanza/pipeline/
--rw-rw-r--   0 john      (1000) john      (1000)        0 2022-07-26 21:49:07.000000 stanza-1.8.1/stanza/pipeline/__init__.py
--rw-rw-r--   0 john      (1000) john      (1000)      258 2024-01-19 08:13:21.000000 stanza-1.8.1/stanza/pipeline/_constants.py
--rw-rw-r--   0 john      (1000) john      (1000)     2612 2023-09-18 14:41:48.000000 stanza-1.8.1/stanza/pipeline/constituency_processor.py
--rw-rw-r--   0 john      (1000) john      (1000)    24444 2024-02-25 01:10:00.000000 stanza-1.8.1/stanza/pipeline/core.py
--rw-rw-r--   0 john      (1000) john      (1000)     6319 2024-02-26 08:15:40.000000 stanza-1.8.1/stanza/pipeline/coref_processor.py
--rw-rw-r--   0 john      (1000) john      (1000)     3647 2024-01-19 08:13:21.000000 stanza-1.8.1/stanza/pipeline/depparse_processor.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-03-01 06:44:43.069464 stanza-1.8.1/stanza/pipeline/external/
--rw-rw-r--   0 john      (1000) john      (1000)        0 2022-07-26 21:49:07.000000 stanza-1.8.1/stanza/pipeline/external/__init__.py
--rw-rw-r--   0 john      (1000) john      (1000)     1256 2023-09-18 14:41:48.000000 stanza-1.8.1/stanza/pipeline/external/corenlp_converter_depparse.py
--rw-rw-r--   0 john      (1000) john      (1000)     2378 2023-06-22 00:27:12.000000 stanza-1.8.1/stanza/pipeline/external/jieba.py
--rw-rw-r--   0 john      (1000) john      (1000)     3247 2023-06-22 00:27:12.000000 stanza-1.8.1/stanza/pipeline/external/pythainlp.py
--rw-rw-r--   0 john      (1000) john      (1000)     2724 2023-06-22 00:27:12.000000 stanza-1.8.1/stanza/pipeline/external/spacy.py
--rw-rw-r--   0 john      (1000) john      (1000)     2917 2023-06-22 00:27:12.000000 stanza-1.8.1/stanza/pipeline/external/sudachipy.py
--rw-rw-r--   0 john      (1000) john      (1000)     4026 2024-02-26 08:15:40.000000 stanza-1.8.1/stanza/pipeline/langid_processor.py
--rw-rw-r--   0 john      (1000) john      (1000)     5342 2024-02-26 08:15:40.000000 stanza-1.8.1/stanza/pipeline/lemma_processor.py
--rw-rw-r--   0 john      (1000) john      (1000)     8277 2024-03-01 06:43:51.000000 stanza-1.8.1/stanza/pipeline/multilingual.py
--rw-rw-r--   0 john      (1000) john      (1000)     1928 2024-01-19 08:13:21.000000 stanza-1.8.1/stanza/pipeline/mwt_processor.py
--rw-rw-r--   0 john      (1000) john      (1000)     6524 2024-01-19 08:13:21.000000 stanza-1.8.1/stanza/pipeline/ner_processor.py
--rw-rw-r--   0 john      (1000) john      (1000)     3383 2024-02-06 08:15:00.000000 stanza-1.8.1/stanza/pipeline/pos_processor.py
--rw-rw-r--   0 john      (1000) john      (1000)    10947 2023-09-18 14:41:48.000000 stanza-1.8.1/stanza/pipeline/processor.py
--rw-rw-r--   0 john      (1000) john      (1000)      224 2022-07-26 21:49:07.000000 stanza-1.8.1/stanza/pipeline/registry.py
--rw-rw-r--   0 john      (1000) john      (1000)     3154 2024-01-19 08:13:21.000000 stanza-1.8.1/stanza/pipeline/sentiment_processor.py
--rw-rw-r--   0 john      (1000) john      (1000)     8192 2024-02-26 08:15:40.000000 stanza-1.8.1/stanza/pipeline/tokenize_processor.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-03-01 06:44:43.070464 stanza-1.8.1/stanza/protobuf/
--rw-rw-r--   0 john      (1000) john      (1000)    53693 2024-02-26 08:15:40.000000 stanza-1.8.1/stanza/protobuf/CoreNLP_pb2.py
--rw-rw-r--   0 john      (1000) john      (1000)     1701 2022-07-26 21:49:07.000000 stanza-1.8.1/stanza/protobuf/__init__.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-03-01 06:44:43.070464 stanza-1.8.1/stanza/resources/
--rw-rw-r--   0 john      (1000) john      (1000)        0 2022-07-26 21:49:07.000000 stanza-1.8.1/stanza/resources/__init__.py
--rw-rw-r--   0 john      (1000) john      (1000)    25972 2024-02-26 08:15:40.000000 stanza-1.8.1/stanza/resources/common.py
--rw-rw-r--   0 john      (1000) john      (1000)    26711 2024-02-26 08:15:40.000000 stanza-1.8.1/stanza/resources/default_packages.py
--rw-rw-r--   0 john      (1000) john      (1000)     5799 2023-06-22 00:27:12.000000 stanza-1.8.1/stanza/resources/installation.py
--rw-rw-r--   0 john      (1000) john      (1000)    27855 2024-02-26 08:15:40.000000 stanza-1.8.1/stanza/resources/prepare_resources.py
--rw-rw-r--   0 john      (1000) john      (1000)      818 2024-01-19 08:13:21.000000 stanza-1.8.1/stanza/resources/print_charlm_depparse.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-03-01 06:44:43.072464 stanza-1.8.1/stanza/server/
--rw-rw-r--   0 john      (1000) john      (1000)      624 2022-07-26 21:49:07.000000 stanza-1.8.1/stanza/server/__init__.py
--rw-rw-r--   0 john      (1000) john      (1000)     4648 2024-01-19 08:13:21.000000 stanza-1.8.1/stanza/server/annotator.py
--rw-rw-r--   0 john      (1000) john      (1000)    32750 2024-01-19 08:13:21.000000 stanza-1.8.1/stanza/server/client.py
--rw-rw-r--   0 john      (1000) john      (1000)     4097 2023-09-18 14:41:48.000000 stanza-1.8.1/stanza/server/dependency_converter.py
--rw-rw-r--   0 john      (1000) john      (1000)    12711 2024-02-26 08:15:40.000000 stanza-1.8.1/stanza/server/java_protobuf_requests.py
--rw-rw-r--   0 john      (1000) john      (1000)     2619 2022-07-26 21:49:07.000000 stanza-1.8.1/stanza/server/main.py
--rw-rw-r--   0 john      (1000) john      (1000)     2355 2024-01-19 08:13:21.000000 stanza-1.8.1/stanza/server/morphology.py
--rw-rw-r--   0 john      (1000) john      (1000)     3032 2024-01-19 08:13:21.000000 stanza-1.8.1/stanza/server/parser_eval.py
--rw-rw-r--   0 john      (1000) john      (1000)     7537 2024-01-19 08:13:21.000000 stanza-1.8.1/stanza/server/semgrex.py
--rw-rw-r--   0 john      (1000) john      (1000)    14856 2024-02-26 08:15:40.000000 stanza-1.8.1/stanza/server/ssurgeon.py
--rw-rw-r--   0 john      (1000) john      (1000)     1356 2023-06-22 00:27:12.000000 stanza-1.8.1/stanza/server/tokensregex.py
--rw-rw-r--   0 john      (1000) john      (1000)     3144 2023-06-22 00:27:12.000000 stanza-1.8.1/stanza/server/tsurgeon.py
--rw-rw-r--   0 john      (1000) john      (1000)     3317 2024-01-19 08:13:21.000000 stanza-1.8.1/stanza/server/ud_enhancer.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-03-01 06:44:43.072464 stanza-1.8.1/stanza/tests/
--rw-rw-r--   0 john      (1000) john      (1000)     4263 2024-01-19 08:13:21.000000 stanza-1.8.1/stanza/tests/__init__.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-03-01 06:44:43.072464 stanza-1.8.1/stanza/tests/classifiers/
--rw-rw-r--   0 john      (1000) john      (1000)        0 2023-09-07 05:52:02.000000 stanza-1.8.1/stanza/tests/classifiers/__init__.py
--rw-rw-r--   0 john      (1000) john      (1000)    10120 2024-02-26 08:15:40.000000 stanza-1.8.1/stanza/tests/classifiers/test_classifier.py
--rw-rw-r--   0 john      (1000) john      (1000)     7226 2023-09-18 14:41:48.000000 stanza-1.8.1/stanza/tests/classifiers/test_constituency_classifier.py
--rw-rw-r--   0 john      (1000) john      (1000)     4949 2023-09-18 14:41:48.000000 stanza-1.8.1/stanza/tests/classifiers/test_data.py
--rw-rw-r--   0 john      (1000) john      (1000)     3254 2023-09-18 14:41:48.000000 stanza-1.8.1/stanza/tests/classifiers/test_process_utils.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-03-01 06:44:43.074464 stanza-1.8.1/stanza/tests/common/
--rw-rw-r--   0 john      (1000) john      (1000)        0 2023-06-22 00:27:12.000000 stanza-1.8.1/stanza/tests/common/__init__.py
--rw-rw-r--   0 john      (1000) john      (1000)     7609 2024-01-19 08:13:21.000000 stanza-1.8.1/stanza/tests/common/test_char_model.py
--rw-rw-r--   0 john      (1000) john      (1000)     1049 2024-01-19 08:13:21.000000 stanza-1.8.1/stanza/tests/common/test_chuliu_edmonds.py
--rw-rw-r--   0 john      (1000) john      (1000)     1210 2023-06-22 00:27:12.000000 stanza-1.8.1/stanza/tests/common/test_common_data.py
--rw-rw-r--   0 john      (1000) john      (1000)     2897 2024-01-19 08:13:21.000000 stanza-1.8.1/stanza/tests/common/test_confusion.py
--rw-rw-r--   0 john      (1000) john      (1000)     2470 2023-09-07 05:52:02.000000 stanza-1.8.1/stanza/tests/common/test_constant.py
--rw-rw-r--   0 john      (1000) john      (1000)    23096 2024-02-26 08:15:40.000000 stanza-1.8.1/stanza/tests/common/test_data_conversion.py
--rw-rw-r--   0 john      (1000) john      (1000)     1924 2024-01-19 08:13:21.000000 stanza-1.8.1/stanza/tests/common/test_data_objects.py
--rw-rw-r--   0 john      (1000) john      (1000)     6373 2024-01-19 08:13:21.000000 stanza-1.8.1/stanza/tests/common/test_doc.py
--rw-rw-r--   0 john      (1000) john      (1000)      918 2023-09-07 05:52:02.000000 stanza-1.8.1/stanza/tests/common/test_dropout.py
--rw-rw-r--   0 john      (1000) john      (1000)     1059 2023-06-22 00:27:12.000000 stanza-1.8.1/stanza/tests/common/test_foundation_cache.py
--rw-rw-r--   0 john      (1000) john      (1000)     4435 2023-09-07 05:52:02.000000 stanza-1.8.1/stanza/tests/common/test_pretrain.py
--rw-rw-r--   0 john      (1000) john      (1000)      556 2023-09-07 05:52:02.000000 stanza-1.8.1/stanza/tests/common/test_short_name_to_treebank.py
--rw-rw-r--   0 john      (1000) john      (1000)     7017 2023-09-07 05:52:02.000000 stanza-1.8.1/stanza/tests/common/test_utils.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-03-01 06:44:43.076464 stanza-1.8.1/stanza/tests/constituency/
--rw-rw-r--   0 john      (1000) john      (1000)        0 2023-06-22 00:27:12.000000 stanza-1.8.1/stanza/tests/constituency/__init__.py
--rw-rw-r--   0 john      (1000) john      (1000)    11505 2023-06-22 00:27:12.000000 stanza-1.8.1/stanza/tests/constituency/test_convert_arboretum.py
--rw-rw-r--   0 john      (1000) john      (1000)    18280 2024-02-26 08:15:40.000000 stanza-1.8.1/stanza/tests/constituency/test_convert_it_vit.py
--rw-rw-r--   0 john      (1000) john      (1000)     1911 2023-06-22 00:27:12.000000 stanza-1.8.1/stanza/tests/constituency/test_convert_starlang.py
--rw-rw-r--   0 john      (1000) john      (1000)    20385 2023-09-18 14:41:48.000000 stanza-1.8.1/stanza/tests/constituency/test_in_order_oracle.py
--rw-rw-r--   0 john      (1000) john      (1000)    23578 2024-01-19 08:13:21.000000 stanza-1.8.1/stanza/tests/constituency/test_lstm_model.py
--rw-rw-r--   0 john      (1000) john      (1000)    17218 2023-09-18 14:41:48.000000 stanza-1.8.1/stanza/tests/constituency/test_parse_transitions.py
--rw-rw-r--   0 john      (1000) john      (1000)    12458 2023-09-18 14:41:48.000000 stanza-1.8.1/stanza/tests/constituency/test_parse_tree.py
--rw-rw-r--   0 john      (1000) john      (1000)     1159 2023-09-18 14:41:48.000000 stanza-1.8.1/stanza/tests/constituency/test_positional_encoding.py
--rw-rw-r--   0 john      (1000) john      (1000)     4434 2023-06-22 00:27:12.000000 stanza-1.8.1/stanza/tests/constituency/test_selftrain_vi_quad.py
--rw-rw-r--   0 john      (1000) john      (1000)    25364 2024-02-26 08:15:40.000000 stanza-1.8.1/stanza/tests/constituency/test_top_down_oracle.py
--rw-rw-r--   0 john      (1000) john      (1000)    30520 2024-02-26 08:15:40.000000 stanza-1.8.1/stanza/tests/constituency/test_trainer.py
--rw-rw-r--   0 john      (1000) john      (1000)     7040 2023-09-07 05:52:02.000000 stanza-1.8.1/stanza/tests/constituency/test_transformer_tree_stack.py
--rw-rw-r--   0 john      (1000) john      (1000)     7355 2023-09-18 14:41:48.000000 stanza-1.8.1/stanza/tests/constituency/test_transition_sequence.py
--rw-rw-r--   0 john      (1000) john      (1000)     3408 2023-06-22 00:27:12.000000 stanza-1.8.1/stanza/tests/constituency/test_tree_reader.py
--rw-rw-r--   0 john      (1000) john      (1000)     1222 2023-06-22 00:27:12.000000 stanza-1.8.1/stanza/tests/constituency/test_tree_stack.py
--rw-rw-r--   0 john      (1000) john      (1000)     2267 2024-01-19 08:13:21.000000 stanza-1.8.1/stanza/tests/constituency/test_utils.py
--rw-rw-r--   0 john      (1000) john      (1000)     4795 2023-09-18 14:41:48.000000 stanza-1.8.1/stanza/tests/constituency/test_vietnamese.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-03-01 06:44:43.076464 stanza-1.8.1/stanza/tests/datasets/
--rw-rw-r--   0 john      (1000) john      (1000)        0 2023-09-07 05:52:02.000000 stanza-1.8.1/stanza/tests/datasets/__init__.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-03-01 06:44:43.076464 stanza-1.8.1/stanza/tests/datasets/ner/
--rw-rw-r--   0 john      (1000) john      (1000)        0 2024-01-19 08:13:21.000000 stanza-1.8.1/stanza/tests/datasets/ner/__init__.py
--rw-rw-r--   0 john      (1000) john      (1000)     2056 2024-01-19 08:13:21.000000 stanza-1.8.1/stanza/tests/datasets/ner/test_prepare_ner_file.py
--rw-rw-r--   0 john      (1000) john      (1000)     1328 2024-01-19 08:13:21.000000 stanza-1.8.1/stanza/tests/datasets/ner/test_utils.py
--rw-rw-r--   0 john      (1000) john      (1000)     2525 2023-09-07 05:52:02.000000 stanza-1.8.1/stanza/tests/datasets/test_common.py
--rw-rw-r--   0 john      (1000) john      (1000)      903 2023-09-07 05:52:02.000000 stanza-1.8.1/stanza/tests/datasets/test_vietnamese_renormalization.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-03-01 06:44:43.077464 stanza-1.8.1/stanza/tests/depparse/
--rw-rw-r--   0 john      (1000) john      (1000)        0 2023-06-22 00:27:12.000000 stanza-1.8.1/stanza/tests/depparse/__init__.py
--rw-rw-r--   0 john      (1000) john      (1000)     2558 2023-06-22 00:27:12.000000 stanza-1.8.1/stanza/tests/depparse/test_depparse_data.py
--rw-rw-r--   0 john      (1000) john      (1000)     9715 2024-02-26 08:15:40.000000 stanza-1.8.1/stanza/tests/depparse/test_parser.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-03-01 06:44:43.077464 stanza-1.8.1/stanza/tests/langid/
--rw-rw-r--   0 john      (1000) john      (1000)        0 2023-06-22 00:27:12.000000 stanza-1.8.1/stanza/tests/langid/__init__.py
--rw-rw-r--   0 john      (1000) john      (1000)    45670 2023-09-18 14:41:48.000000 stanza-1.8.1/stanza/tests/langid/test_langid.py
--rw-rw-r--   0 john      (1000) john      (1000)     3817 2024-01-19 08:13:21.000000 stanza-1.8.1/stanza/tests/langid/test_multilingual.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-03-01 06:44:43.077464 stanza-1.8.1/stanza/tests/lemma/
--rw-rw-r--   0 john      (1000) john      (1000)        0 2023-06-22 00:27:12.000000 stanza-1.8.1/stanza/tests/lemma/__init__.py
--rw-rw-r--   0 john      (1000) john      (1000)     3831 2024-02-26 08:15:40.000000 stanza-1.8.1/stanza/tests/lemma/test_data.py
--rw-rw-r--   0 john      (1000) john      (1000)     6043 2024-01-19 08:13:21.000000 stanza-1.8.1/stanza/tests/lemma/test_lemma_trainer.py
--rw-rw-r--   0 john      (1000) john      (1000)     3113 2024-02-26 08:15:40.000000 stanza-1.8.1/stanza/tests/lemma/test_lowercase.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-03-01 06:44:43.078464 stanza-1.8.1/stanza/tests/mwt/
--rw-rw-r--   0 john      (1000) john      (1000)        0 2023-09-07 05:52:02.000000 stanza-1.8.1/stanza/tests/mwt/__init__.py
--rw-rw-r--   0 john      (1000) john      (1000)     2071 2024-01-19 08:13:21.000000 stanza-1.8.1/stanza/tests/mwt/test_utils.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-03-01 06:44:43.079464 stanza-1.8.1/stanza/tests/ner/
--rw-rw-r--   0 john      (1000) john      (1000)        0 2023-06-22 00:27:12.000000 stanza-1.8.1/stanza/tests/ner/__init__.py
--rw-rw-r--   0 john      (1000) john      (1000)     9455 2023-06-22 00:27:12.000000 stanza-1.8.1/stanza/tests/ner/test_bsf_2_beios.py
--rw-rw-r--   0 john      (1000) john      (1000)     2634 2023-06-22 00:27:12.000000 stanza-1.8.1/stanza/tests/ner/test_bsf_2_iob.py
--rw-rw-r--   0 john      (1000) john      (1000)     1402 2023-09-18 14:41:48.000000 stanza-1.8.1/stanza/tests/ner/test_combine_ner_datasets.py
--rw-rw-r--   0 john      (1000) john      (1000)     3364 2023-09-07 05:52:02.000000 stanza-1.8.1/stanza/tests/ner/test_convert_amt.py
--rw-rw-r--   0 john      (1000) john      (1000)    56852 2023-09-07 05:52:02.000000 stanza-1.8.1/stanza/tests/ner/test_convert_nkjp.py
--rw-rw-r--   0 john      (1000) john      (1000)     1501 2023-06-22 00:27:12.000000 stanza-1.8.1/stanza/tests/ner/test_convert_starlang_ner.py
--rw-rw-r--   0 john      (1000) john      (1000)     1167 2024-01-19 08:13:21.000000 stanza-1.8.1/stanza/tests/ner/test_models_ner_scorer.py
--rw-rw-r--   0 john      (1000) john      (1000)     2510 2024-01-19 08:13:21.000000 stanza-1.8.1/stanza/tests/ner/test_ner_tagger.py
--rw-rw-r--   0 john      (1000) john      (1000)     1756 2023-06-22 00:27:12.000000 stanza-1.8.1/stanza/tests/ner/test_ner_trainer.py
--rw-rw-r--   0 john      (1000) john      (1000)     8575 2024-02-26 08:15:40.000000 stanza-1.8.1/stanza/tests/ner/test_ner_training.py
--rw-rw-r--   0 john      (1000) john      (1000)     6643 2024-01-19 08:13:21.000000 stanza-1.8.1/stanza/tests/ner/test_ner_utils.py
--rw-rw-r--   0 john      (1000) john      (1000)     1725 2023-09-18 14:41:48.000000 stanza-1.8.1/stanza/tests/ner/test_pay_amt_annotators.py
--rw-rw-r--   0 john      (1000) john      (1000)     4426 2023-06-22 00:27:12.000000 stanza-1.8.1/stanza/tests/ner/test_split_wikiner.py
--rw-rw-r--   0 john      (1000) john      (1000)     2742 2023-06-22 00:27:12.000000 stanza-1.8.1/stanza/tests/ner/test_suc3.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-03-01 06:44:43.081464 stanza-1.8.1/stanza/tests/pipeline/
--rw-rw-r--   0 john      (1000) john      (1000)        0 2023-06-22 00:27:12.000000 stanza-1.8.1/stanza/tests/pipeline/__init__.py
--rw-rw-r--   0 john      (1000) john      (1000)     1478 2023-09-18 14:41:48.000000 stanza-1.8.1/stanza/tests/pipeline/pipeline_device_tests.py
--rw-rw-r--   0 john      (1000) john      (1000)      980 2024-01-19 08:13:21.000000 stanza-1.8.1/stanza/tests/pipeline/test_arabic_pipeline.py
--rw-rw-r--   0 john      (1000) john      (1000)    11565 2024-01-19 08:13:21.000000 stanza-1.8.1/stanza/tests/pipeline/test_core.py
--rw-rw-r--   0 john      (1000) john      (1000)     4922 2024-01-19 08:13:21.000000 stanza-1.8.1/stanza/tests/pipeline/test_decorators.py
--rw-rw-r--   0 john      (1000) john      (1000)     2747 2023-09-07 05:52:02.000000 stanza-1.8.1/stanza/tests/pipeline/test_depparse.py
--rw-rw-r--   0 john      (1000) john      (1000)    14936 2024-02-26 08:15:40.000000 stanza-1.8.1/stanza/tests/pipeline/test_english_pipeline.py
--rw-rw-r--   0 john      (1000) john      (1000)     7519 2024-02-26 08:15:40.000000 stanza-1.8.1/stanza/tests/pipeline/test_french_pipeline.py
--rw-rw-r--   0 john      (1000) john      (1000)     4680 2024-02-26 08:15:40.000000 stanza-1.8.1/stanza/tests/pipeline/test_lemmatizer.py
--rw-rw-r--   0 john      (1000) john      (1000)     2678 2023-09-18 14:41:48.000000 stanza-1.8.1/stanza/tests/pipeline/test_pipeline_constituency_processor.py
--rw-rw-r--   0 john      (1000) john      (1000)     1028 2023-09-07 05:52:02.000000 stanza-1.8.1/stanza/tests/pipeline/test_pipeline_depparse_processor.py
--rw-rw-r--   0 john      (1000) john      (1000)     3363 2023-06-22 00:27:12.000000 stanza-1.8.1/stanza/tests/pipeline/test_pipeline_mwt_expander.py
--rw-rw-r--   0 john      (1000) john      (1000)     4022 2024-01-19 08:13:21.000000 stanza-1.8.1/stanza/tests/pipeline/test_pipeline_ner_processor.py
--rw-rw-r--   0 john      (1000) john      (1000)     1777 2024-01-19 08:13:21.000000 stanza-1.8.1/stanza/tests/pipeline/test_pipeline_pos_processor.py
--rw-rw-r--   0 john      (1000) john      (1000)     1384 2023-06-22 00:27:12.000000 stanza-1.8.1/stanza/tests/pipeline/test_pipeline_sentiment_processor.py
--rw-rw-r--   0 john      (1000) john      (1000)     3100 2024-01-19 08:13:21.000000 stanza-1.8.1/stanza/tests/pipeline/test_requirements.py
--rw-rw-r--   0 john      (1000) john      (1000)    22906 2024-01-19 08:13:21.000000 stanza-1.8.1/stanza/tests/pipeline/test_tokenizer.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-03-01 06:44:43.081464 stanza-1.8.1/stanza/tests/pos/
--rw-rw-r--   0 john      (1000) john      (1000)        0 2023-06-22 00:27:12.000000 stanza-1.8.1/stanza/tests/pos/__init__.py
--rw-rw-r--   0 john      (1000) john      (1000)     5473 2024-01-19 08:13:21.000000 stanza-1.8.1/stanza/tests/pos/test_data.py
--rw-rw-r--   0 john      (1000) john      (1000)    13431 2024-02-26 08:15:40.000000 stanza-1.8.1/stanza/tests/pos/test_tagger.py
--rw-rw-r--   0 john      (1000) john      (1000)     6700 2024-01-19 08:13:21.000000 stanza-1.8.1/stanza/tests/pos/test_xpos_vocab_factory.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-03-01 06:44:43.082464 stanza-1.8.1/stanza/tests/resources/
--rw-rw-r--   0 john      (1000) john      (1000)        0 2023-06-22 00:27:12.000000 stanza-1.8.1/stanza/tests/resources/__init__.py
--rw-rw-r--   0 john      (1000) john      (1000)     1374 2024-01-19 08:13:21.000000 stanza-1.8.1/stanza/tests/resources/test_charlm_depparse.py
--rw-rw-r--   0 john      (1000) john      (1000)     5865 2024-01-19 08:13:21.000000 stanza-1.8.1/stanza/tests/resources/test_common.py
--rw-rw-r--   0 john      (1000) john      (1000)      811 2024-01-19 08:13:21.000000 stanza-1.8.1/stanza/tests/resources/test_default_packages.py
--rw-rw-r--   0 john      (1000) john      (1000)     1904 2023-06-22 00:27:12.000000 stanza-1.8.1/stanza/tests/resources/test_installation.py
--rw-rw-r--   0 john      (1000) john      (1000)     1008 2023-06-22 00:27:12.000000 stanza-1.8.1/stanza/tests/resources/test_prepare_resources.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-03-01 06:44:43.084464 stanza-1.8.1/stanza/tests/server/
--rw-rw-r--   0 john      (1000) john      (1000)        0 2023-06-22 00:27:12.000000 stanza-1.8.1/stanza/tests/server/__init__.py
--rw-rw-r--   0 john      (1000) john      (1000)    11609 2024-01-19 08:13:21.000000 stanza-1.8.1/stanza/tests/server/test_client.py
--rw-rw-r--   0 john      (1000) john      (1000)     3924 2024-02-26 08:15:40.000000 stanza-1.8.1/stanza/tests/server/test_java_protobuf_requests.py
--rw-rw-r--   0 john      (1000) john      (1000)      674 2024-01-19 08:13:21.000000 stanza-1.8.1/stanza/tests/server/test_morphology.py
--rw-rw-r--   0 john      (1000) john      (1000)     1864 2024-01-19 08:13:21.000000 stanza-1.8.1/stanza/tests/server/test_parser_eval.py
--rw-rw-r--   0 john      (1000) john      (1000)     4669 2023-06-22 00:27:12.000000 stanza-1.8.1/stanza/tests/server/test_protobuf.py
--rw-rw-r--   0 john      (1000) john      (1000)     6973 2024-01-19 08:13:21.000000 stanza-1.8.1/stanza/tests/server/test_semgrex.py
--rw-rw-r--   0 john      (1000) john      (1000)     5083 2023-06-22 00:27:12.000000 stanza-1.8.1/stanza/tests/server/test_server_misc.py
--rw-rw-r--   0 john      (1000) john      (1000)     1804 2023-06-22 00:27:12.000000 stanza-1.8.1/stanza/tests/server/test_server_pretokenized.py
--rw-rw-r--   0 john      (1000) john      (1000)    10460 2023-06-22 00:27:12.000000 stanza-1.8.1/stanza/tests/server/test_server_request.py
--rw-rw-r--   0 john      (1000) john      (1000)     9732 2023-06-22 00:27:12.000000 stanza-1.8.1/stanza/tests/server/test_server_start.py
--rw-rw-r--   0 john      (1000) john      (1000)    14199 2024-02-26 08:15:40.000000 stanza-1.8.1/stanza/tests/server/test_ssurgeon.py
--rw-rw-r--   0 john      (1000) john      (1000)     1334 2023-06-22 00:27:12.000000 stanza-1.8.1/stanza/tests/server/test_tokensregex.py
--rw-rw-r--   0 john      (1000) john      (1000)     3934 2023-06-22 00:27:12.000000 stanza-1.8.1/stanza/tests/server/test_tsurgeon.py
--rw-rw-r--   0 john      (1000) john      (1000)     1144 2023-06-22 00:27:12.000000 stanza-1.8.1/stanza/tests/server/test_ud_enhancer.py
--rw-rw-r--   0 john      (1000) john      (1000)     2477 2024-02-26 08:15:40.000000 stanza-1.8.1/stanza/tests/setup.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-03-01 06:44:43.085464 stanza-1.8.1/stanza/tests/tokenization/
--rw-rw-r--   0 john      (1000) john      (1000)        0 2023-06-22 00:27:12.000000 stanza-1.8.1/stanza/tests/tokenization/__init__.py
--rw-rw-r--   0 john      (1000) john      (1000)    23229 2023-09-18 14:41:48.000000 stanza-1.8.1/stanza/tests/tokenization/test_prepare_tokenizer_treebank.py
--rw-rw-r--   0 john      (1000) john      (1000)     1072 2024-01-19 08:13:21.000000 stanza-1.8.1/stanza/tests/tokenization/test_replace_long_tokens.py
--rw-rw-r--   0 john      (1000) john      (1000)     2954 2024-02-26 08:15:40.000000 stanza-1.8.1/stanza/tests/tokenization/test_spaces.py
--rw-rw-r--   0 john      (1000) john      (1000)     9481 2023-09-07 05:52:02.000000 stanza-1.8.1/stanza/tests/tokenization/test_tokenization_lst20.py
--rw-rw-r--   0 john      (1000) john      (1000)     5039 2023-09-07 05:52:02.000000 stanza-1.8.1/stanza/tests/tokenization/test_tokenization_orchid.py
--rw-rw-r--   0 john      (1000) john      (1000)     9844 2023-06-22 00:27:12.000000 stanza-1.8.1/stanza/tests/tokenization/test_tokenize_data.py
--rw-rw-r--   0 john      (1000) john      (1000)      748 2023-09-07 05:52:02.000000 stanza-1.8.1/stanza/tests/tokenization/test_tokenize_files.py
--rw-rw-r--   0 john      (1000) john      (1000)    11205 2024-02-26 08:15:40.000000 stanza-1.8.1/stanza/tests/tokenization/test_tokenize_utils.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-03-01 06:44:43.086464 stanza-1.8.1/stanza/utils/
--rw-rw-r--   0 john      (1000) john      (1000)        0 2022-07-26 21:49:07.000000 stanza-1.8.1/stanza/utils/__init__.py
--rw-rw-r--   0 john      (1000) john      (1000)      511 2022-07-26 21:49:07.000000 stanza-1.8.1/stanza/utils/avg_sent_len.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-03-01 06:44:43.086464 stanza-1.8.1/stanza/utils/charlm/
--rw-rw-r--   0 john      (1000) john      (1000)        0 2023-06-22 00:27:12.000000 stanza-1.8.1/stanza/utils/charlm/__init__.py
--rw-rw-r--   0 john      (1000) john      (1000)     3549 2023-06-22 00:27:12.000000 stanza-1.8.1/stanza/utils/charlm/conll17_to_text.py
--rw-rw-r--   0 john      (1000) john      (1000)     4272 2024-01-19 08:13:21.000000 stanza-1.8.1/stanza/utils/charlm/dump_oscar.py
--rw-rw-r--   0 john      (1000) john      (1000)     7456 2024-01-19 08:13:21.000000 stanza-1.8.1/stanza/utils/charlm/make_lm_data.py
--rw-rw-r--   0 john      (1000) john      (1000)     2742 2023-09-18 14:41:48.000000 stanza-1.8.1/stanza/utils/charlm/oscar_to_text.py
--rw-rw-r--   0 john      (1000) john      (1000)     7337 2024-03-01 03:19:48.000000 stanza-1.8.1/stanza/utils/confusion.py
--rw-rw-r--   0 john      (1000) john      (1000)     8947 2024-02-26 08:15:40.000000 stanza-1.8.1/stanza/utils/conll.py
--rwxrwxr-x   0 john      (1000) john      (1000)    40528 2023-09-07 05:52:02.000000 stanza-1.8.1/stanza/utils/conll18_ud_eval.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-03-01 06:44:43.086464 stanza-1.8.1/stanza/utils/constituency/
--rw-rw-r--   0 john      (1000) john      (1000)        0 2024-01-19 08:13:21.000000 stanza-1.8.1/stanza/utils/constituency/__init__.py
--rw-rw-r--   0 john      (1000) john      (1000)      365 2024-01-19 08:13:21.000000 stanza-1.8.1/stanza/utils/constituency/list_tensors.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-03-01 06:44:43.088464 stanza-1.8.1/stanza/utils/datasets/
--rw-rw-r--   0 john      (1000) john      (1000)        0 2022-07-26 21:49:07.000000 stanza-1.8.1/stanza/utils/datasets/__init__.py
--rw-rw-r--   0 john      (1000) john      (1000)     1079 2024-01-18 05:03:09.000000 stanza-1.8.1/stanza/utils/datasets/add_fake_dependencies.py
--rw-rw-r--   0 john      (1000) john      (1000)    10533 2024-02-26 08:15:40.000000 stanza-1.8.1/stanza/utils/datasets/common.py
--rw-rw-r--   0 john      (1000) john      (1000)     8641 2022-07-26 21:49:07.000000 stanza-1.8.1/stanza/utils/datasets/conllu_to_text.pl
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-03-01 06:44:43.171464 stanza-1.8.1/stanza/utils/datasets/constituency/
--rw-rw-r--   0 john      (1000) john      (1000)        0 2023-06-22 00:27:12.000000 stanza-1.8.1/stanza/utils/datasets/constituency/__init__.py
--rw-rw-r--   0 john      (1000) john      (1000)     5114 2024-02-26 08:15:40.000000 stanza-1.8.1/stanza/utils/datasets/constituency/build_silver_dataset.py
--rw-rw-r--   0 john      (1000) john      (1000)      479 2023-09-18 14:41:48.000000 stanza-1.8.1/stanza/utils/datasets/constituency/common_trees.py
--rw-rw-r--   0 john      (1000) john      (1000)     3686 2023-06-22 00:27:12.000000 stanza-1.8.1/stanza/utils/datasets/constituency/convert_alt.py
--rw-rw-r--   0 john      (1000) john      (1000)    16062 2023-06-22 00:27:12.000000 stanza-1.8.1/stanza/utils/datasets/constituency/convert_arboretum.py
--rw-rw-r--   0 john      (1000) john      (1000)     3237 2023-06-22 00:27:12.000000 stanza-1.8.1/stanza/utils/datasets/constituency/convert_cintil.py
--rw-rw-r--   0 john      (1000) john      (1000)     6441 2024-01-19 08:13:21.000000 stanza-1.8.1/stanza/utils/datasets/constituency/convert_ctb.py
--rw-rw-r--   0 john      (1000) john      (1000)    13171 2023-06-22 00:27:12.000000 stanza-1.8.1/stanza/utils/datasets/constituency/convert_it_turin.py
--rw-rw-r--   0 john      (1000) john      (1000)    34313 2024-02-26 08:15:40.000000 stanza-1.8.1/stanza/utils/datasets/constituency/convert_it_vit.py
--rw-rw-r--   0 john      (1000) john      (1000)     3478 2023-06-22 00:27:12.000000 stanza-1.8.1/stanza/utils/datasets/constituency/convert_starlang.py
--rw-rw-r--   0 john      (1000) john      (1000)      341 2023-09-18 14:41:48.000000 stanza-1.8.1/stanza/utils/datasets/constituency/count_common_words.py
--rw-rw-r--   0 john      (1000) john      (1000)     2010 2024-02-26 08:15:40.000000 stanza-1.8.1/stanza/utils/datasets/constituency/extract_silver_dataset.py
--rw-rw-r--   0 john      (1000) john      (1000)    23424 2024-02-25 01:10:00.000000 stanza-1.8.1/stanza/utils/datasets/constituency/prepare_con_dataset.py
--rw-rw-r--   0 john      (1000) john      (1000)     2472 2023-09-07 05:52:02.000000 stanza-1.8.1/stanza/utils/datasets/constituency/relabel_tags.py
--rw-rw-r--   0 john      (1000) john      (1000)    10324 2024-01-19 08:13:21.000000 stanza-1.8.1/stanza/utils/datasets/constituency/selftrain.py
--rw-rw-r--   0 john      (1000) john      (1000)     4277 2023-09-18 14:41:48.000000 stanza-1.8.1/stanza/utils/datasets/constituency/selftrain_it.py
--rw-rw-r--   0 john      (1000) john      (1000)     2558 2023-09-18 14:41:48.000000 stanza-1.8.1/stanza/utils/datasets/constituency/selftrain_single_file.py
--rw-rw-r--   0 john      (1000) john      (1000)     3007 2023-09-18 14:41:48.000000 stanza-1.8.1/stanza/utils/datasets/constituency/selftrain_vi_quad.py
--rw-rw-r--   0 john      (1000) john      (1000)     4782 2023-09-18 14:41:48.000000 stanza-1.8.1/stanza/utils/datasets/constituency/selftrain_wiki.py
--rw-rw-r--   0 john      (1000) john      (1000)     4980 2024-02-26 08:15:40.000000 stanza-1.8.1/stanza/utils/datasets/constituency/silver_variance.py
--rw-rw-r--   0 john      (1000) john      (1000)     3726 2024-02-26 08:15:40.000000 stanza-1.8.1/stanza/utils/datasets/constituency/tokenize_wiki.py
--rw-rw-r--   0 john      (1000) john      (1000)     1488 2023-09-18 14:41:48.000000 stanza-1.8.1/stanza/utils/datasets/constituency/treebank_to_labeled_brackets.py
--rw-rw-r--   0 john      (1000) john      (1000)      792 2023-06-22 00:27:12.000000 stanza-1.8.1/stanza/utils/datasets/constituency/utils.py
--rw-rw-r--   0 john      (1000) john      (1000)     9983 2024-01-19 08:13:21.000000 stanza-1.8.1/stanza/utils/datasets/constituency/vtb_convert.py
--rw-rw-r--   0 john      (1000) john      (1000)     5909 2023-09-18 14:41:48.000000 stanza-1.8.1/stanza/utils/datasets/constituency/vtb_split.py
--rw-rw-r--   0 john      (1000) john      (1000)     1567 2023-09-18 14:41:48.000000 stanza-1.8.1/stanza/utils/datasets/contract_mwt.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-03-01 06:44:43.171464 stanza-1.8.1/stanza/utils/datasets/coref/
--rw-rw-r--   0 john      (1000) john      (1000)        0 2024-01-19 08:13:21.000000 stanza-1.8.1/stanza/utils/datasets/coref/__init__.py
--rw-rw-r--   0 john      (1000) john      (1000)     9119 2024-01-19 08:13:21.000000 stanza-1.8.1/stanza/utils/datasets/coref/convert_ontonotes.py
--rw-rw-r--   0 john      (1000) john      (1000)     2956 2024-01-19 08:13:21.000000 stanza-1.8.1/stanza/utils/datasets/corenlp_segmenter_dataset.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-03-01 06:44:43.175464 stanza-1.8.1/stanza/utils/datasets/ner/
--rw-rw-r--   0 john      (1000) john      (1000)        0 2023-06-22 00:27:12.000000 stanza-1.8.1/stanza/utils/datasets/ner/__init__.py
--rw-rw-r--   0 john      (1000) john      (1000)     4114 2024-01-19 08:13:21.000000 stanza-1.8.1/stanza/utils/datasets/ner/build_en_combined.py
--rw-rw-r--   0 john      (1000) john      (1000)     1932 2023-06-22 00:27:12.000000 stanza-1.8.1/stanza/utils/datasets/ner/check_for_duplicates.py
--rw-rw-r--   0 john      (1000) john      (1000)      925 2024-01-19 08:13:21.000000 stanza-1.8.1/stanza/utils/datasets/ner/combine_ner_datasets.py
--rw-rw-r--   0 john      (1000) john      (1000)     1358 2024-01-19 08:13:21.000000 stanza-1.8.1/stanza/utils/datasets/ner/compare_entities.py
--rw-rw-r--   0 john      (1000) john      (1000)     2128 2023-06-22 00:27:12.000000 stanza-1.8.1/stanza/utils/datasets/ner/conll_to_iob.py
--rw-rw-r--   0 john      (1000) john      (1000)     9329 2023-09-07 05:52:02.000000 stanza-1.8.1/stanza/utils/datasets/ner/convert_amt.py
--rw-rw-r--   0 john      (1000) john      (1000)     4041 2024-01-19 08:13:21.000000 stanza-1.8.1/stanza/utils/datasets/ner/convert_ar_aqmar.py
--rw-rw-r--   0 john      (1000) john      (1000)     4380 2023-09-07 05:52:02.000000 stanza-1.8.1/stanza/utils/datasets/ner/convert_bn_daffodil.py
--rw-rw-r--   0 john      (1000) john      (1000)     9197 2023-06-22 00:27:12.000000 stanza-1.8.1/stanza/utils/datasets/ner/convert_bsf_to_beios.py
--rw-rw-r--   0 john      (1000) john      (1000)    17697 2023-06-22 00:27:12.000000 stanza-1.8.1/stanza/utils/datasets/ner/convert_bsnlp.py
--rw-rw-r--   0 john      (1000) john      (1000)     1536 2024-01-19 08:13:21.000000 stanza-1.8.1/stanza/utils/datasets/ner/convert_en_conll03.py
--rw-rw-r--   0 john      (1000) john      (1000)     4490 2023-06-22 00:27:12.000000 stanza-1.8.1/stanza/utils/datasets/ner/convert_fire_2013.py
--rw-rw-r--   0 john      (1000) john      (1000)     5651 2024-01-19 08:13:21.000000 stanza-1.8.1/stanza/utils/datasets/ner/convert_hy_armtdp.py
--rw-rw-r--   0 john      (1000) john      (1000)     5377 2023-06-22 00:27:12.000000 stanza-1.8.1/stanza/utils/datasets/ner/convert_ijc.py
--rw-rw-r--   0 john      (1000) john      (1000)     1385 2023-09-07 05:52:02.000000 stanza-1.8.1/stanza/utils/datasets/ner/convert_kk_kazNERD.py
--rw-rw-r--   0 john      (1000) john      (1000)     3061 2023-06-22 00:27:12.000000 stanza-1.8.1/stanza/utils/datasets/ner/convert_lst20.py
--rw-rw-r--   0 john      (1000) john      (1000)     1715 2023-06-22 00:27:12.000000 stanza-1.8.1/stanza/utils/datasets/ner/convert_mr_l3cube.py
--rw-rw-r--   0 john      (1000) john      (1000)     3685 2023-06-22 00:27:12.000000 stanza-1.8.1/stanza/utils/datasets/ner/convert_my_ucsy.py
--rw-rw-r--   0 john      (1000) john      (1000)    10216 2023-09-07 05:52:02.000000 stanza-1.8.1/stanza/utils/datasets/ner/convert_nkjp.py
--rw-rw-r--   0 john      (1000) john      (1000)     2366 2024-01-19 08:13:21.000000 stanza-1.8.1/stanza/utils/datasets/ner/convert_nner22.py
--rw-rw-r--   0 john      (1000) john      (1000)     1472 2023-06-22 00:27:12.000000 stanza-1.8.1/stanza/utils/datasets/ner/convert_nytk.py
--rw-rw-r--   0 john      (1000) john      (1000)     2727 2024-01-19 08:13:21.000000 stanza-1.8.1/stanza/utils/datasets/ner/convert_ontonotes.py
--rw-rw-r--   0 john      (1000) john      (1000)     2367 2023-06-22 00:27:12.000000 stanza-1.8.1/stanza/utils/datasets/ner/convert_rgai.py
--rw-rw-r--   0 john      (1000) john      (1000)     2853 2023-09-07 05:52:02.000000 stanza-1.8.1/stanza/utils/datasets/ner/convert_sindhi_siner.py
--rw-rw-r--   0 john      (1000) john      (1000)     1615 2023-06-22 00:27:12.000000 stanza-1.8.1/stanza/utils/datasets/ner/convert_starlang_ner.py
--rw-rw-r--   0 john      (1000) john      (1000)     1122 2024-01-19 08:13:21.000000 stanza-1.8.1/stanza/utils/datasets/ner/count_entities.py
--rw-rw-r--   0 john      (1000) john      (1000)     1960 2023-09-18 14:41:48.000000 stanza-1.8.1/stanza/utils/datasets/ner/json_to_bio.py
--rw-rw-r--   0 john      (1000) john      (1000)     3530 2024-01-19 08:13:21.000000 stanza-1.8.1/stanza/utils/datasets/ner/misc_to_date.py
--rw-rw-r--   0 john      (1000) john      (1000)     4232 2024-01-19 08:13:21.000000 stanza-1.8.1/stanza/utils/datasets/ner/ontonotes_multitag.py
--rw-rw-r--   0 john      (1000) john      (1000)    57993 2024-01-19 08:13:21.000000 stanza-1.8.1/stanza/utils/datasets/ner/prepare_ner_dataset.py
--rw-rw-r--   0 john      (1000) john      (1000)     2641 2023-09-07 05:52:02.000000 stanza-1.8.1/stanza/utils/datasets/ner/prepare_ner_file.py
--rw-rw-r--   0 john      (1000) john      (1000)     1436 2023-06-22 00:27:12.000000 stanza-1.8.1/stanza/utils/datasets/ner/preprocess_wikiner.py
--rw-rw-r--   0 john      (1000) john      (1000)     5853 2024-01-19 08:13:21.000000 stanza-1.8.1/stanza/utils/datasets/ner/simplify_en_worldwide.py
--rw-rw-r--   0 john      (1000) john      (1000)     3055 2024-01-19 08:13:21.000000 stanza-1.8.1/stanza/utils/datasets/ner/simplify_ontonotes_to_worldwide.py
--rw-rw-r--   0 john      (1000) john      (1000)     3366 2023-06-22 00:27:12.000000 stanza-1.8.1/stanza/utils/datasets/ner/split_wikiner.py
--rw-rw-r--   0 john      (1000) john      (1000)     2484 2023-06-22 00:27:12.000000 stanza-1.8.1/stanza/utils/datasets/ner/suc_conll_to_iob.py
--rw-rw-r--   0 john      (1000) john      (1000)     5308 2023-06-22 00:27:12.000000 stanza-1.8.1/stanza/utils/datasets/ner/suc_to_iob.py
--rw-rw-r--   0 john      (1000) john      (1000)    14275 2024-01-19 08:13:21.000000 stanza-1.8.1/stanza/utils/datasets/ner/utils.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-03-01 06:44:43.175464 stanza-1.8.1/stanza/utils/datasets/pos/
--rw-rw-r--   0 john      (1000) john      (1000)        0 2023-09-07 05:52:02.000000 stanza-1.8.1/stanza/utils/datasets/pos/__init__.py
--rw-rw-r--   0 john      (1000) john      (1000)     3724 2024-01-19 08:13:21.000000 stanza-1.8.1/stanza/utils/datasets/pos/convert_trees_to_pos.py
--rw-rw-r--   0 john      (1000) john      (1000)     6811 2024-02-26 08:15:40.000000 stanza-1.8.1/stanza/utils/datasets/prepare_depparse_treebank.py
--rw-rw-r--   0 john      (1000) john      (1000)     2007 2024-01-19 08:13:21.000000 stanza-1.8.1/stanza/utils/datasets/prepare_lemma_treebank.py
--rw-rw-r--   0 john      (1000) john      (1000)     2379 2024-01-19 08:13:21.000000 stanza-1.8.1/stanza/utils/datasets/prepare_mwt_treebank.py
--rw-rw-r--   0 john      (1000) john      (1000)      656 2024-01-19 08:13:21.000000 stanza-1.8.1/stanza/utils/datasets/prepare_pos_treebank.py
--rw-rw-r--   0 john      (1000) john      (1000)     5625 2024-02-26 08:15:40.000000 stanza-1.8.1/stanza/utils/datasets/prepare_tokenizer_data.py
--rwxrwxr-x   0 john      (1000) john      (1000)    50063 2024-02-26 08:15:40.000000 stanza-1.8.1/stanza/utils/datasets/prepare_tokenizer_treebank.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-03-01 06:44:43.176464 stanza-1.8.1/stanza/utils/datasets/pretrain/
--rw-rw-r--   0 john      (1000) john      (1000)        0 2023-09-18 14:41:48.000000 stanza-1.8.1/stanza/utils/datasets/pretrain/__init__.py
--rw-rw-r--   0 john      (1000) john      (1000)     1281 2023-09-18 14:41:48.000000 stanza-1.8.1/stanza/utils/datasets/pretrain/word_in_pretrain.py
--rw-rw-r--   0 john      (1000) john      (1000)     2569 2024-02-25 01:10:00.000000 stanza-1.8.1/stanza/utils/datasets/random_split_conllu.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-03-01 06:44:43.178464 stanza-1.8.1/stanza/utils/datasets/sentiment/
--rw-rw-r--   0 john      (1000) john      (1000)        0 2023-06-22 00:27:12.000000 stanza-1.8.1/stanza/utils/datasets/sentiment/__init__.py
--rw-rw-r--   0 john      (1000) john      (1000)     4902 2024-02-26 08:15:40.000000 stanza-1.8.1/stanza/utils/datasets/sentiment/add_constituency.py
--rw-rw-r--   0 john      (1000) john      (1000)     2486 2024-02-26 08:15:40.000000 stanza-1.8.1/stanza/utils/datasets/sentiment/convert_italian_poetry_classification.py
--rw-rw-r--   0 john      (1000) john      (1000)     3082 2023-09-18 14:41:48.000000 stanza-1.8.1/stanza/utils/datasets/sentiment/convert_italian_sentence_classification.py
--rw-rw-r--   0 john      (1000) john      (1000)    16102 2024-01-19 08:13:21.000000 stanza-1.8.1/stanza/utils/datasets/sentiment/prepare_sentiment_dataset.py
--rw-rw-r--   0 john      (1000) john      (1000)     2408 2023-09-07 05:52:02.000000 stanza-1.8.1/stanza/utils/datasets/sentiment/process_MELD.py
--rw-rw-r--   0 john      (1000) john      (1000)     2631 2023-09-07 05:52:02.000000 stanza-1.8.1/stanza/utils/datasets/sentiment/process_airline.py
--rw-rw-r--   0 john      (1000) john      (1000)     2880 2023-09-07 05:52:02.000000 stanza-1.8.1/stanza/utils/datasets/sentiment/process_arguana_xml.py
--rw-rw-r--   0 john      (1000) john      (1000)     2801 2024-01-19 08:13:21.000000 stanza-1.8.1/stanza/utils/datasets/sentiment/process_corona.py
--rw-rw-r--   0 john      (1000) john      (1000)     8958 2023-09-07 05:52:02.000000 stanza-1.8.1/stanza/utils/datasets/sentiment/process_es_tass2020.py
--rw-rw-r--   0 john      (1000) john      (1000)     3545 2023-09-07 05:52:02.000000 stanza-1.8.1/stanza/utils/datasets/sentiment/process_it_sentipolc16.py
--rw-rw-r--   0 john      (1000) john      (1000)     3170 2023-09-07 05:52:02.000000 stanza-1.8.1/stanza/utils/datasets/sentiment/process_ren_chinese.py
--rw-rw-r--   0 john      (1000) john      (1000)     2839 2023-06-22 00:27:12.000000 stanza-1.8.1/stanza/utils/datasets/sentiment/process_sb10k.py
--rw-rw-r--   0 john      (1000) john      (1000)     3854 2023-09-07 05:52:02.000000 stanza-1.8.1/stanza/utils/datasets/sentiment/process_scare.py
--rw-rw-r--   0 john      (1000) john      (1000)     2294 2023-09-07 05:52:02.000000 stanza-1.8.1/stanza/utils/datasets/sentiment/process_slsd.py
--rw-rw-r--   0 john      (1000) john      (1000)     3159 2023-09-07 05:52:02.000000 stanza-1.8.1/stanza/utils/datasets/sentiment/process_sst.py
--rw-rw-r--   0 john      (1000) john      (1000)     2551 2023-09-07 05:52:02.000000 stanza-1.8.1/stanza/utils/datasets/sentiment/process_usage_german.py
--rw-rw-r--   0 john      (1000) john      (1000)     5647 2024-01-19 08:13:21.000000 stanza-1.8.1/stanza/utils/datasets/sentiment/process_utils.py
--rw-rw-r--   0 john      (1000) john      (1000)     1976 2023-09-07 05:52:02.000000 stanza-1.8.1/stanza/utils/datasets/sentiment/process_vsfc_vietnamese.py
--rw-rw-r--   0 john      (1000) john      (1000)     1429 2023-06-22 00:27:12.000000 stanza-1.8.1/stanza/utils/datasets/thai_syllable_dict_generator.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-03-01 06:44:43.178464 stanza-1.8.1/stanza/utils/datasets/tokenization/
--rw-rw-r--   0 john      (1000) john      (1000)        0 2023-06-22 00:27:12.000000 stanza-1.8.1/stanza/utils/datasets/tokenization/__init__.py
--rw-rw-r--   0 john      (1000) john      (1000)     9650 2024-01-19 08:13:21.000000 stanza-1.8.1/stanza/utils/datasets/tokenization/convert_ml_cochin.py
--rw-rw-r--   0 john      (1000) john      (1000)     6431 2023-06-22 00:27:12.000000 stanza-1.8.1/stanza/utils/datasets/tokenization/convert_my_alt.py
--rw-rw-r--   0 john      (1000) john      (1000)     8336 2023-09-18 14:41:48.000000 stanza-1.8.1/stanza/utils/datasets/tokenization/convert_text_files.py
--rw-rw-r--   0 john      (1000) john      (1000)     5941 2023-09-07 05:52:02.000000 stanza-1.8.1/stanza/utils/datasets/tokenization/convert_th_best.py
--rw-rw-r--   0 john      (1000) john      (1000)     5273 2023-06-22 00:27:12.000000 stanza-1.8.1/stanza/utils/datasets/tokenization/convert_th_lst20.py
--rw-rw-r--   0 john      (1000) john      (1000)     5352 2023-06-22 00:27:12.000000 stanza-1.8.1/stanza/utils/datasets/tokenization/convert_th_orchid.py
--rw-rw-r--   0 john      (1000) john      (1000)     7383 2023-06-22 00:27:12.000000 stanza-1.8.1/stanza/utils/datasets/tokenization/convert_vi_vlsp.py
--rw-rw-r--   0 john      (1000) john      (1000)     7697 2023-06-22 00:27:12.000000 stanza-1.8.1/stanza/utils/datasets/tokenization/process_thai_tokenization.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-03-01 06:44:43.179464 stanza-1.8.1/stanza/utils/datasets/vietnamese/
--rw-rw-r--   0 john      (1000) john      (1000)        0 2023-09-07 05:52:02.000000 stanza-1.8.1/stanza/utils/datasets/vietnamese/__init__.py
--rw-rw-r--   0 john      (1000) john      (1000)     3768 2023-09-07 05:52:02.000000 stanza-1.8.1/stanza/utils/datasets/vietnamese/renormalize.py
--rw-rw-r--   0 john      (1000) john      (1000)     2023 2024-03-01 03:19:48.000000 stanza-1.8.1/stanza/utils/default_paths.py
--rw-rw-r--   0 john      (1000) john      (1000)     1253 2023-09-18 14:41:48.000000 stanza-1.8.1/stanza/utils/get_tqdm.py
--rw-rw-r--   0 john      (1000) john      (1000)     1263 2022-07-26 21:49:07.000000 stanza-1.8.1/stanza/utils/helper_func.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-03-01 06:44:43.179464 stanza-1.8.1/stanza/utils/languages/
--rw-rw-r--   0 john      (1000) john      (1000)        0 2024-01-19 08:13:21.000000 stanza-1.8.1/stanza/utils/languages/__init__.py
--rw-rw-r--   0 john      (1000) john      (1000)     6960 2024-01-19 08:13:21.000000 stanza-1.8.1/stanza/utils/languages/kazakh_transliteration.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-03-01 06:44:43.179464 stanza-1.8.1/stanza/utils/lemma/
--rw-rw-r--   0 john      (1000) john      (1000)        0 2024-01-19 08:13:21.000000 stanza-1.8.1/stanza/utils/lemma/__init__.py
--rw-rw-r--   0 john      (1000) john      (1000)      762 2024-01-19 08:13:21.000000 stanza-1.8.1/stanza/utils/lemma/count_ambiguous_lemmas.py
--rw-rw-r--   0 john      (1000) john      (1000)      329 2022-07-26 21:49:07.000000 stanza-1.8.1/stanza/utils/max_mwt_length.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-03-01 06:44:43.179464 stanza-1.8.1/stanza/utils/ner/
--rw-rw-r--   0 john      (1000) john      (1000)        0 2023-09-18 14:41:48.000000 stanza-1.8.1/stanza/utils/ner/__init__.py
--rw-rw-r--   0 john      (1000) john      (1000)     3445 2024-01-19 08:13:21.000000 stanza-1.8.1/stanza/utils/ner/flair_ner_tag_dataset.py
--rw-rw-r--   0 john      (1000) john      (1000)     2467 2023-09-18 14:41:48.000000 stanza-1.8.1/stanza/utils/ner/paying_annotators.py
--rw-rw-r--   0 john      (1000) john      (1000)     4383 2024-01-19 08:13:21.000000 stanza-1.8.1/stanza/utils/ner/spacy_ner_tag_dataset.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-03-01 06:44:43.180464 stanza-1.8.1/stanza/utils/pretrain/
--rw-rw-r--   0 john      (1000) john      (1000)        0 2024-01-19 08:13:21.000000 stanza-1.8.1/stanza/utils/pretrain/__init__.py
--rw-rw-r--   0 john      (1000) john      (1000)     1476 2024-01-19 08:13:21.000000 stanza-1.8.1/stanza/utils/pretrain/compare_pretrains.py
--rw-rw-r--   0 john      (1000) john      (1000)      451 2022-07-26 21:49:07.000000 stanza-1.8.1/stanza/utils/select_backoff.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-03-01 06:44:43.229464 stanza-1.8.1/stanza/utils/training/
--rw-rw-r--   0 john      (1000) john      (1000)        0 2022-07-26 21:49:07.000000 stanza-1.8.1/stanza/utils/training/__init__.py
--rw-rw-r--   0 john      (1000) john      (1000)    20182 2024-01-19 08:13:21.000000 stanza-1.8.1/stanza/utils/training/common.py
--rw-rw-r--   0 john      (1000) john      (1000)     3643 2024-01-19 08:13:21.000000 stanza-1.8.1/stanza/utils/training/compose_ete_results.py
--rw-rw-r--   0 john      (1000) john      (1000)     3416 2024-01-19 08:13:21.000000 stanza-1.8.1/stanza/utils/training/remove_constituency_optimizer.py
--rw-rw-r--   0 john      (1000) john      (1000)     3361 2024-01-19 08:13:21.000000 stanza-1.8.1/stanza/utils/training/run_charlm.py
--rw-rw-r--   0 john      (1000) john      (1000)     5288 2024-01-19 08:13:21.000000 stanza-1.8.1/stanza/utils/training/run_constituency.py
--rw-rw-r--   0 john      (1000) john      (1000)     5947 2024-01-19 08:13:21.000000 stanza-1.8.1/stanza/utils/training/run_depparse.py
--rw-rw-r--   0 john      (1000) john      (1000)     8200 2024-01-19 08:13:21.000000 stanza-1.8.1/stanza/utils/training/run_ete.py
--rw-rw-r--   0 john      (1000) john      (1000)     6775 2024-01-19 08:13:21.000000 stanza-1.8.1/stanza/utils/training/run_lemma.py
--rw-rw-r--   0 john      (1000) john      (1000)     4613 2024-01-19 08:13:21.000000 stanza-1.8.1/stanza/utils/training/run_mwt.py
--rw-rw-r--   0 john      (1000) john      (1000)     6865 2024-01-19 08:13:21.000000 stanza-1.8.1/stanza/utils/training/run_ner.py
--rw-rw-r--   0 john      (1000) john      (1000)     6293 2024-01-19 08:13:21.000000 stanza-1.8.1/stanza/utils/training/run_pos.py
--rw-rw-r--   0 john      (1000) john      (1000)     5035 2024-02-26 08:15:40.000000 stanza-1.8.1/stanza/utils/training/run_sentiment.py
--rw-rw-r--   0 john      (1000) john      (1000)     4729 2024-01-19 08:13:21.000000 stanza-1.8.1/stanza/utils/training/run_tokenizer.py
--rw-rw-r--   0 john      (1000) john      (1000)     9930 2023-09-18 14:41:48.000000 stanza-1.8.1/stanza/utils/training/separate_ner_pretrain.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-03-01 06:44:43.229464 stanza-1.8.1/stanza.egg-info/
--rw-r--r--   0 john      (1000) john      (1000)    13192 2024-03-01 06:44:43.000000 stanza-1.8.1/stanza.egg-info/PKG-INFO
--rw-rw-r--   0 john      (1000) john      (1000)    18900 2024-03-01 06:44:43.000000 stanza-1.8.1/stanza.egg-info/SOURCES.txt
--rw-rw-r--   0 john      (1000) john      (1000)        1 2024-03-01 06:44:43.000000 stanza-1.8.1/stanza.egg-info/dependency_links.txt
--rw-rw-r--   0 john      (1000) john      (1000)      185 2024-03-01 06:44:43.000000 stanza-1.8.1/stanza.egg-info/requires.txt
--rw-rw-r--   0 john      (1000) john      (1000)        7 2024-03-01 06:44:43.000000 stanza-1.8.1/stanza.egg-info/top_level.txt
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-20 16:32:24.104412 stanza-1.8.2/
+-rw-rw-r--   0 john      (1000) john      (1000)      603 2022-07-26 21:49:07.000000 stanza-1.8.2/LICENSE
+-rw-r--r--   0 john      (1000) john      (1000)    13192 2024-04-20 16:32:24.104412 stanza-1.8.2/PKG-INFO
+-rw-rw-r--   0 john      (1000) john      (1000)    11336 2024-01-19 08:13:21.000000 stanza-1.8.2/README.md
+-rw-rw-r--   0 john      (1000) john      (1000)       38 2024-04-20 16:32:24.104412 stanza-1.8.2/setup.cfg
+-rw-rw-r--   0 john      (1000) john      (1000)     4774 2024-01-19 08:13:21.000000 stanza-1.8.2/setup.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-20 16:32:24.052412 stanza-1.8.2/stanza/
+-rw-rw-r--   0 john      (1000) john      (1000)     1021 2023-06-22 00:27:12.000000 stanza-1.8.2/stanza/__init__.py
+-rw-rw-r--   0 john      (1000) john      (1000)      105 2024-04-20 16:29:51.000000 stanza-1.8.2/stanza/_version.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-20 16:32:24.054412 stanza-1.8.2/stanza/models/
+-rw-rw-r--   0 john      (1000) john      (1000)        0 2022-07-26 21:49:07.000000 stanza-1.8.2/stanza/models/__init__.py
+-rw-rw-r--   0 john      (1000) john      (1000)       83 2022-07-26 21:49:07.000000 stanza-1.8.2/stanza/models/_training_logging.py
+-rw-rw-r--   0 john      (1000) john      (1000)    16184 2024-01-19 08:13:21.000000 stanza-1.8.2/stanza/models/charlm.py
+-rw-rw-r--   0 john      (1000) john      (1000)    36241 2024-04-20 16:29:51.000000 stanza-1.8.2/stanza/models/classifier.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-20 16:32:24.055412 stanza-1.8.2/stanza/models/classifiers/
+-rw-rw-r--   0 john      (1000) john      (1000)        0 2022-07-26 21:49:07.000000 stanza-1.8.2/stanza/models/classifiers/__init__.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1938 2023-09-18 14:41:48.000000 stanza-1.8.2/stanza/models/classifiers/base_classifier.py
+-rw-rw-r--   0 john      (1000) john      (1000)    28105 2024-04-20 16:29:51.000000 stanza-1.8.2/stanza/models/classifiers/cnn_classifier.py
+-rw-rw-r--   0 john      (1000) john      (1000)     4056 2024-03-13 08:17:47.000000 stanza-1.8.2/stanza/models/classifiers/constituency_classifier.py
+-rw-rw-r--   0 john      (1000) john      (1000)     6069 2024-03-13 08:17:47.000000 stanza-1.8.2/stanza/models/classifiers/data.py
+-rw-rw-r--   0 john      (1000) john      (1000)     2166 2023-09-18 14:41:48.000000 stanza-1.8.2/stanza/models/classifiers/iterate_test.py
+-rw-rw-r--   0 john      (1000) john      (1000)    14179 2024-04-20 16:29:51.000000 stanza-1.8.2/stanza/models/classifiers/trainer.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1054 2023-09-18 14:41:48.000000 stanza-1.8.2/stanza/models/classifiers/utils.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-20 16:32:24.058412 stanza-1.8.2/stanza/models/common/
+-rw-rw-r--   0 john      (1000) john      (1000)        0 2022-07-26 21:49:07.000000 stanza-1.8.2/stanza/models/common/__init__.py
+-rw-rw-r--   0 john      (1000) john      (1000)     4481 2024-03-13 08:17:47.000000 stanza-1.8.2/stanza/models/common/beam.py
+-rw-rw-r--   0 john      (1000) john      (1000)    22151 2024-04-20 16:29:51.000000 stanza-1.8.2/stanza/models/common/bert_embedding.py
+-rw-rw-r--   0 john      (1000) john      (1000)     3582 2022-07-26 21:49:07.000000 stanza-1.8.2/stanza/models/common/biaffine.py
+-rw-rw-r--   0 john      (1000) john      (1000)     2075 2024-01-19 08:13:21.000000 stanza-1.8.2/stanza/models/common/build_short_name_to_treebank.py
+-rw-rw-r--   0 john      (1000) john      (1000)    15704 2024-03-13 08:17:47.000000 stanza-1.8.2/stanza/models/common/char_model.py
+-rw-rw-r--   0 john      (1000) john      (1000)    11900 2024-01-19 08:13:21.000000 stanza-1.8.2/stanza/models/common/chuliu_edmonds.py
+-rw-rw-r--   0 john      (1000) john      (1000)    14459 2024-03-13 08:17:47.000000 stanza-1.8.2/stanza/models/common/constant.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1856 2023-09-18 14:41:48.000000 stanza-1.8.2/stanza/models/common/convert_pretrain.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1171 2023-06-22 00:27:12.000000 stanza-1.8.2/stanza/models/common/count_ner_coverage.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1535 2023-06-22 00:27:12.000000 stanza-1.8.2/stanza/models/common/count_pretrain_coverage.py
+-rw-rw-r--   0 john      (1000) john      (1000)     5915 2024-01-19 08:13:21.000000 stanza-1.8.2/stanza/models/common/crf.py
+-rw-rw-r--   0 john      (1000) john      (1000)     6111 2024-01-19 08:13:21.000000 stanza-1.8.2/stanza/models/common/data.py
+-rw-rw-r--   0 john      (1000) john      (1000)    67239 2024-04-20 16:29:51.000000 stanza-1.8.2/stanza/models/common/doc.py
+-rw-rw-r--   0 john      (1000) john      (1000)     2858 2022-07-26 21:49:07.000000 stanza-1.8.2/stanza/models/common/dropout.py
+-rw-rw-r--   0 john      (1000) john      (1000)      452 2024-01-19 08:13:21.000000 stanza-1.8.2/stanza/models/common/exceptions.py
+-rw-rw-r--   0 john      (1000) john      (1000)     6715 2024-04-20 16:29:51.000000 stanza-1.8.2/stanza/models/common/foundation_cache.py
+-rw-rw-r--   0 john      (1000) john      (1000)     5180 2023-06-22 00:27:12.000000 stanza-1.8.2/stanza/models/common/hlstm.py
+-rw-rw-r--   0 john      (1000) john      (1000)     2638 2023-09-18 14:41:48.000000 stanza-1.8.2/stanza/models/common/large_margin_loss.py
+-rw-rw-r--   0 john      (1000) john      (1000)     4716 2023-09-18 14:41:48.000000 stanza-1.8.2/stanza/models/common/loss.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1265 2023-09-18 14:41:48.000000 stanza-1.8.2/stanza/models/common/maxout_linear.py
+-rw-rw-r--   0 john      (1000) john      (1000)     4855 2022-07-26 21:49:07.000000 stanza-1.8.2/stanza/models/common/packed_lstm.py
+-rw-rw-r--   0 john      (1000) john      (1000)     4715 2024-04-20 16:29:51.000000 stanza-1.8.2/stanza/models/common/peft_config.py
+-rw-rw-r--   0 john      (1000) john      (1000)    11012 2024-03-13 08:17:47.000000 stanza-1.8.2/stanza/models/common/pretrain.py
+-rw-rw-r--   0 john      (1000) john      (1000)     3456 2024-04-04 07:31:14.000000 stanza-1.8.2/stanza/models/common/relative_attn.py
+-rw-rw-r--   0 john      (1000) john      (1000)      221 2022-07-26 21:49:07.000000 stanza-1.8.2/stanza/models/common/seq2seq_constant.py
+-rw-rw-r--   0 john      (1000) john      (1000)    13578 2024-01-19 08:13:21.000000 stanza-1.8.2/stanza/models/common/seq2seq_model.py
+-rw-rw-r--   0 john      (1000) john      (1000)     8483 2023-06-22 00:27:12.000000 stanza-1.8.2/stanza/models/common/seq2seq_modules.py
+-rw-rw-r--   0 john      (1000) john      (1000)     3334 2023-09-07 05:52:02.000000 stanza-1.8.2/stanza/models/common/seq2seq_utils.py
+-rw-rw-r--   0 john      (1000) john      (1000)    29850 2024-01-19 08:13:21.000000 stanza-1.8.2/stanza/models/common/short_name_to_treebank.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1147 2023-09-18 14:41:48.000000 stanza-1.8.2/stanza/models/common/stanza_object.py
+-rw-rw-r--   0 john      (1000) john      (1000)      645 2022-07-26 21:49:07.000000 stanza-1.8.2/stanza/models/common/trainer.py
+-rw-rw-r--   0 john      (1000) john      (1000)    31007 2024-04-20 16:29:51.000000 stanza-1.8.2/stanza/models/common/utils.py
+-rw-rw-r--   0 john      (1000) john      (1000)     9703 2024-01-19 08:13:21.000000 stanza-1.8.2/stanza/models/common/vocab.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-20 16:32:24.061412 stanza-1.8.2/stanza/models/constituency/
+-rw-rw-r--   0 john      (1000) john      (1000)        0 2023-06-22 00:27:12.000000 stanza-1.8.2/stanza/models/constituency/__init__.py
+-rw-rw-r--   0 john      (1000) john      (1000)    22391 2024-04-20 16:29:51.000000 stanza-1.8.2/stanza/models/constituency/base_model.py
+-rw-rw-r--   0 john      (1000) john      (1000)     2388 2024-03-13 08:17:47.000000 stanza-1.8.2/stanza/models/constituency/dynamic_oracle.py
+-rw-rw-r--   0 john      (1000) john      (1000)    14113 2024-04-20 16:29:51.000000 stanza-1.8.2/stanza/models/constituency/ensemble.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1249 2023-09-07 05:52:02.000000 stanza-1.8.2/stanza/models/constituency/evaluate_treebanks.py
+-rw-rw-r--   0 john      (1000) john      (1000)    20875 2024-03-13 08:17:47.000000 stanza-1.8.2/stanza/models/constituency/in_order_oracle.py
+-rw-rw-r--   0 john      (1000) john      (1000)    31043 2023-09-18 14:41:48.000000 stanza-1.8.2/stanza/models/constituency/label_attention.py
+-rw-rw-r--   0 john      (1000) john      (1000)    67720 2024-04-20 16:29:51.000000 stanza-1.8.2/stanza/models/constituency/lstm_model.py
+-rw-rw-r--   0 john      (1000) john      (1000)     3605 2023-09-07 05:52:02.000000 stanza-1.8.2/stanza/models/constituency/lstm_tree_stack.py
+-rw-rw-r--   0 john      (1000) john      (1000)    23504 2024-04-20 16:29:51.000000 stanza-1.8.2/stanza/models/constituency/parse_transitions.py
+-rw-rw-r--   0 john      (1000) john      (1000)    20536 2024-04-20 16:29:51.000000 stanza-1.8.2/stanza/models/constituency/parse_tree.py
+-rw-rw-r--   0 john      (1000) john      (1000)    11165 2023-09-07 05:52:02.000000 stanza-1.8.2/stanza/models/constituency/partitioned_transformer.py
+-rw-rw-r--   0 john      (1000) john      (1000)     3049 2023-09-18 14:41:48.000000 stanza-1.8.2/stanza/models/constituency/positional_encoding.py
+-rw-rw-r--   0 john      (1000) john      (1000)     6647 2024-04-20 16:29:51.000000 stanza-1.8.2/stanza/models/constituency/retagging.py
+-rw-rw-r--   0 john      (1000) john      (1000)     2186 2023-09-18 14:41:48.000000 stanza-1.8.2/stanza/models/constituency/score_converted_dependencies.py
+-rw-rw-r--   0 john      (1000) john      (1000)     4247 2024-04-20 16:29:51.000000 stanza-1.8.2/stanza/models/constituency/state.py
+-rw-rw-r--   0 john      (1000) john      (1000)     4262 2024-04-20 16:29:51.000000 stanza-1.8.2/stanza/models/constituency/text_processing.py
+-rw-rw-r--   0 john      (1000) john      (1000)    25468 2024-03-13 08:17:47.000000 stanza-1.8.2/stanza/models/constituency/top_down_oracle.py
+-rw-rw-r--   0 john      (1000) john      (1000)    56604 2024-04-20 16:29:51.000000 stanza-1.8.2/stanza/models/constituency/trainer.py
+-rw-rw-r--   0 john      (1000) john      (1000)     7555 2023-09-18 14:41:48.000000 stanza-1.8.2/stanza/models/constituency/transformer_tree_stack.py
+-rw-rw-r--   0 john      (1000) john      (1000)     6117 2024-03-13 08:17:47.000000 stanza-1.8.2/stanza/models/constituency/transition_sequence.py
+-rw-rw-r--   0 john      (1000) john      (1000)     6165 2024-04-20 16:29:51.000000 stanza-1.8.2/stanza/models/constituency/tree_embedding.py
+-rw-rw-r--   0 john      (1000) john      (1000)     9212 2024-04-20 16:29:51.000000 stanza-1.8.2/stanza/models/constituency/tree_reader.py
+-rw-rw-r--   0 john      (1000) john      (1000)     2033 2023-09-18 14:41:48.000000 stanza-1.8.2/stanza/models/constituency/tree_stack.py
+-rw-rw-r--   0 john      (1000) john      (1000)    15742 2024-04-20 16:29:51.000000 stanza-1.8.2/stanza/models/constituency/utils.py
+-rw-rw-r--   0 john      (1000) john      (1000)    51443 2024-04-20 16:29:51.000000 stanza-1.8.2/stanza/models/constituency_parser.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-20 16:32:24.063412 stanza-1.8.2/stanza/models/coref/
+-rw-rw-r--   0 john      (1000) john      (1000)        0 2024-01-19 08:13:21.000000 stanza-1.8.2/stanza/models/coref/__init__.py
+-rw-rw-r--   0 john      (1000) john      (1000)     4072 2024-01-19 08:13:21.000000 stanza-1.8.2/stanza/models/coref/anaphoricity_scorer.py
+-rw-rw-r--   0 john      (1000) john      (1000)     2623 2024-01-19 08:13:21.000000 stanza-1.8.2/stanza/models/coref/bert.py
+-rw-rw-r--   0 john      (1000) john      (1000)     2863 2024-01-19 08:13:21.000000 stanza-1.8.2/stanza/models/coref/cluster_checker.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1352 2024-01-19 08:13:21.000000 stanza-1.8.2/stanza/models/coref/config.py
+-rw-rw-r--   0 john      (1000) john      (1000)     2675 2024-01-19 08:13:21.000000 stanza-1.8.2/stanza/models/coref/conll.py
+-rw-rw-r--   0 john      (1000) john      (1000)      687 2024-01-19 08:13:21.000000 stanza-1.8.2/stanza/models/coref/const.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1377 2024-01-19 08:13:21.000000 stanza-1.8.2/stanza/models/coref/coref_chain.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1465 2024-01-19 08:13:21.000000 stanza-1.8.2/stanza/models/coref/loss.py
+-rw-rw-r--   0 john      (1000) john      (1000)    29455 2024-03-13 08:17:47.000000 stanza-1.8.2/stanza/models/coref/model.py
+-rw-rw-r--   0 john      (1000) john      (1000)     3092 2024-01-19 08:13:21.000000 stanza-1.8.2/stanza/models/coref/pairwise_encoder.py
+-rw-rw-r--   0 john      (1000) john      (1000)     2167 2024-01-19 08:13:21.000000 stanza-1.8.2/stanza/models/coref/predict.py
+-rw-rw-r--   0 john      (1000) john      (1000)     2210 2024-01-19 08:13:21.000000 stanza-1.8.2/stanza/models/coref/rough_scorer.py
+-rw-rw-r--   0 john      (1000) john      (1000)     6032 2024-01-20 04:09:40.000000 stanza-1.8.2/stanza/models/coref/span_predictor.py
+-rw-rw-r--   0 john      (1000) john      (1000)      749 2024-01-19 08:13:21.000000 stanza-1.8.2/stanza/models/coref/tokenizer_customization.py
+-rw-rw-r--   0 john      (1000) john      (1000)      993 2024-01-19 08:13:21.000000 stanza-1.8.2/stanza/models/coref/utils.py
+-rw-rw-r--   0 john      (1000) john      (1000)     4040 2024-01-19 08:13:21.000000 stanza-1.8.2/stanza/models/coref/word_encoder.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-20 16:32:24.063412 stanza-1.8.2/stanza/models/depparse/
+-rw-rw-r--   0 john      (1000) john      (1000)        0 2022-07-26 21:49:07.000000 stanza-1.8.2/stanza/models/depparse/__init__.py
+-rw-rw-r--   0 john      (1000) john      (1000)     9717 2024-03-13 08:17:47.000000 stanza-1.8.2/stanza/models/depparse/data.py
+-rw-rw-r--   0 john      (1000) john      (1000)    15144 2024-04-20 16:29:51.000000 stanza-1.8.2/stanza/models/depparse/model.py
+-rw-rw-r--   0 john      (1000) john      (1000)     2431 2023-09-18 14:41:48.000000 stanza-1.8.2/stanza/models/depparse/scorer.py
+-rw-rw-r--   0 john      (1000) john      (1000)    12848 2024-04-20 16:29:51.000000 stanza-1.8.2/stanza/models/depparse/trainer.py
+-rw-rw-r--   0 john      (1000) john      (1000)     2297 2024-01-19 08:13:21.000000 stanza-1.8.2/stanza/models/identity_lemmatizer.py
+-rw-rw-r--   0 john      (1000) john      (1000)    10266 2024-01-19 08:13:21.000000 stanza-1.8.2/stanza/models/lang_identifier.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-20 16:32:24.064411 stanza-1.8.2/stanza/models/langid/
+-rw-rw-r--   0 john      (1000) john      (1000)        0 2023-06-22 00:27:12.000000 stanza-1.8.2/stanza/models/langid/__init__.py
+-rw-rw-r--   0 john      (1000) john      (1000)     8627 2023-06-22 00:27:12.000000 stanza-1.8.2/stanza/models/langid/create_ud_data.py
+-rw-rw-r--   0 john      (1000) john      (1000)     5206 2023-09-18 14:41:48.000000 stanza-1.8.2/stanza/models/langid/data.py
+-rw-rw-r--   0 john      (1000) john      (1000)     4771 2024-01-19 08:13:21.000000 stanza-1.8.2/stanza/models/langid/model.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1778 2024-01-19 08:13:21.000000 stanza-1.8.2/stanza/models/langid/trainer.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-20 16:32:24.065412 stanza-1.8.2/stanza/models/lemma/
+-rw-rw-r--   0 john      (1000) john      (1000)        0 2022-07-26 21:49:07.000000 stanza-1.8.2/stanza/models/lemma/__init__.py
+-rw-rw-r--   0 john      (1000) john      (1000)     5957 2024-03-13 08:17:47.000000 stanza-1.8.2/stanza/models/lemma/data.py
+-rw-rw-r--   0 john      (1000) john      (1000)      631 2022-07-26 21:49:07.000000 stanza-1.8.2/stanza/models/lemma/edit.py
+-rw-rw-r--   0 john      (1000) john      (1000)      350 2023-09-07 05:52:02.000000 stanza-1.8.2/stanza/models/lemma/scorer.py
+-rw-rw-r--   0 john      (1000) john      (1000)    10141 2024-03-13 08:17:47.000000 stanza-1.8.2/stanza/models/lemma/trainer.py
+-rw-rw-r--   0 john      (1000) john      (1000)      649 2022-07-26 21:49:07.000000 stanza-1.8.2/stanza/models/lemma/vocab.py
+-rw-rw-r--   0 john      (1000) john      (1000)    14123 2024-03-13 08:17:47.000000 stanza-1.8.2/stanza/models/lemmatizer.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-20 16:32:24.065412 stanza-1.8.2/stanza/models/mwt/
+-rw-rw-r--   0 john      (1000) john      (1000)        0 2022-07-26 21:49:07.000000 stanza-1.8.2/stanza/models/mwt/__init__.py
+-rw-rw-r--   0 john      (1000) john      (1000)     3591 2024-04-20 16:29:51.000000 stanza-1.8.2/stanza/models/mwt/data.py
+-rw-rw-r--   0 john      (1000) john      (1000)      348 2023-09-07 05:52:02.000000 stanza-1.8.2/stanza/models/mwt/scorer.py
+-rw-rw-r--   0 john      (1000) john      (1000)     6994 2024-04-20 16:29:51.000000 stanza-1.8.2/stanza/models/mwt/trainer.py
+-rw-rw-r--   0 john      (1000) john      (1000)     4006 2024-04-20 16:29:51.000000 stanza-1.8.2/stanza/models/mwt/utils.py
+-rw-rw-r--   0 john      (1000) john      (1000)      506 2022-07-26 21:49:07.000000 stanza-1.8.2/stanza/models/mwt/vocab.py
+-rw-rw-r--   0 john      (1000) john      (1000)    13334 2024-04-20 16:29:51.000000 stanza-1.8.2/stanza/models/mwt_expander.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-20 16:32:24.066412 stanza-1.8.2/stanza/models/ner/
+-rw-rw-r--   0 john      (1000) john      (1000)        0 2022-07-26 21:49:07.000000 stanza-1.8.2/stanza/models/ner/__init__.py
+-rw-rw-r--   0 john      (1000) john      (1000)     9831 2024-04-20 16:29:51.000000 stanza-1.8.2/stanza/models/ner/data.py
+-rw-rw-r--   0 john      (1000) john      (1000)    14623 2024-04-20 16:29:51.000000 stanza-1.8.2/stanza/models/ner/model.py
+-rw-rw-r--   0 john      (1000) john      (1000)     6364 2024-01-19 08:13:21.000000 stanza-1.8.2/stanza/models/ner/scorer.py
+-rw-rw-r--   0 john      (1000) john      (1000)    13276 2024-04-20 16:29:51.000000 stanza-1.8.2/stanza/models/ner/trainer.py
+-rw-rw-r--   0 john      (1000) john      (1000)    11202 2024-01-19 08:13:21.000000 stanza-1.8.2/stanza/models/ner/utils.py
+-rw-rw-r--   0 john      (1000) john      (1000)     2601 2024-01-19 08:13:21.000000 stanza-1.8.2/stanza/models/ner/vocab.py
+-rw-rw-r--   0 john      (1000) john      (1000)    26809 2024-04-20 16:29:51.000000 stanza-1.8.2/stanza/models/ner_tagger.py
+-rw-rw-r--   0 john      (1000) john      (1000)    22735 2024-04-20 16:29:51.000000 stanza-1.8.2/stanza/models/parser.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-20 16:32:24.067412 stanza-1.8.2/stanza/models/pos/
+-rw-rw-r--   0 john      (1000) john      (1000)        0 2022-07-26 21:49:07.000000 stanza-1.8.2/stanza/models/pos/__init__.py
+-rw-rw-r--   0 john      (1000) john      (1000)     5626 2023-06-22 00:27:12.000000 stanza-1.8.2/stanza/models/pos/build_xpos_vocab_factory.py
+-rw-rw-r--   0 john      (1000) john      (1000)    16153 2024-04-20 16:29:51.000000 stanza-1.8.2/stanza/models/pos/data.py
+-rw-rw-r--   0 john      (1000) john      (1000)    13840 2024-04-20 16:29:51.000000 stanza-1.8.2/stanza/models/pos/model.py
+-rw-rw-r--   0 john      (1000) john      (1000)      670 2024-01-19 08:13:21.000000 stanza-1.8.2/stanza/models/pos/scorer.py
+-rw-rw-r--   0 john      (1000) john      (1000)     8957 2024-04-20 16:29:51.000000 stanza-1.8.2/stanza/models/pos/trainer.py
+-rw-rw-r--   0 john      (1000) john      (1000)     2805 2024-04-20 16:29:51.000000 stanza-1.8.2/stanza/models/pos/vocab.py
+-rw-rw-r--   0 john      (1000) john      (1000)     9586 2023-09-07 05:52:02.000000 stanza-1.8.2/stanza/models/pos/xpos_vocab_factory.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1595 2023-06-22 00:27:12.000000 stanza-1.8.2/stanza/models/pos/xpos_vocab_utils.py
+-rw-rw-r--   0 john      (1000) john      (1000)    23515 2024-04-20 16:29:51.000000 stanza-1.8.2/stanza/models/tagger.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-20 16:32:24.067412 stanza-1.8.2/stanza/models/tokenization/
+-rw-rw-r--   0 john      (1000) john      (1000)        0 2022-07-26 21:49:07.000000 stanza-1.8.2/stanza/models/tokenization/__init__.py
+-rw-rw-r--   0 john      (1000) john      (1000)    19164 2023-09-07 05:52:02.000000 stanza-1.8.2/stanza/models/tokenization/data.py
+-rw-rw-r--   0 john      (1000) john      (1000)     3834 2024-03-13 21:46:28.000000 stanza-1.8.2/stanza/models/tokenization/model.py
+-rw-rw-r--   0 john      (1000) john      (1000)     3788 2024-01-19 08:13:21.000000 stanza-1.8.2/stanza/models/tokenization/tokenize_files.py
+-rw-rw-r--   0 john      (1000) john      (1000)     3783 2024-01-19 08:13:21.000000 stanza-1.8.2/stanza/models/tokenization/trainer.py
+-rw-rw-r--   0 john      (1000) john      (1000)    26104 2024-03-13 08:17:47.000000 stanza-1.8.2/stanza/models/tokenization/utils.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1097 2023-06-22 00:27:12.000000 stanza-1.8.2/stanza/models/tokenization/vocab.py
+-rw-rw-r--   0 john      (1000) john      (1000)    13799 2024-01-19 08:13:21.000000 stanza-1.8.2/stanza/models/tokenizer.py
+-rw-rw-r--   0 john      (1000) john      (1000)     6609 2024-03-13 08:17:47.000000 stanza-1.8.2/stanza/models/wl_coref.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-20 16:32:24.069412 stanza-1.8.2/stanza/pipeline/
+-rw-rw-r--   0 john      (1000) john      (1000)        0 2022-07-26 21:49:07.000000 stanza-1.8.2/stanza/pipeline/__init__.py
+-rw-rw-r--   0 john      (1000) john      (1000)      258 2024-01-19 08:13:21.000000 stanza-1.8.2/stanza/pipeline/_constants.py
+-rw-rw-r--   0 john      (1000) john      (1000)     2612 2023-09-18 14:41:48.000000 stanza-1.8.2/stanza/pipeline/constituency_processor.py
+-rw-rw-r--   0 john      (1000) john      (1000)    24709 2024-04-20 16:29:51.000000 stanza-1.8.2/stanza/pipeline/core.py
+-rw-rw-r--   0 john      (1000) john      (1000)     6319 2024-03-13 08:17:47.000000 stanza-1.8.2/stanza/pipeline/coref_processor.py
+-rw-rw-r--   0 john      (1000) john      (1000)     3647 2024-01-19 08:13:21.000000 stanza-1.8.2/stanza/pipeline/depparse_processor.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-20 16:32:24.070412 stanza-1.8.2/stanza/pipeline/external/
+-rw-rw-r--   0 john      (1000) john      (1000)        0 2022-07-26 21:49:07.000000 stanza-1.8.2/stanza/pipeline/external/__init__.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1256 2023-09-18 14:41:48.000000 stanza-1.8.2/stanza/pipeline/external/corenlp_converter_depparse.py
+-rw-rw-r--   0 john      (1000) john      (1000)     2378 2023-06-22 00:27:12.000000 stanza-1.8.2/stanza/pipeline/external/jieba.py
+-rw-rw-r--   0 john      (1000) john      (1000)     3247 2023-06-22 00:27:12.000000 stanza-1.8.2/stanza/pipeline/external/pythainlp.py
+-rw-rw-r--   0 john      (1000) john      (1000)     2724 2023-06-22 00:27:12.000000 stanza-1.8.2/stanza/pipeline/external/spacy.py
+-rw-rw-r--   0 john      (1000) john      (1000)     2917 2023-06-22 00:27:12.000000 stanza-1.8.2/stanza/pipeline/external/sudachipy.py
+-rw-rw-r--   0 john      (1000) john      (1000)     4026 2024-03-13 08:17:47.000000 stanza-1.8.2/stanza/pipeline/langid_processor.py
+-rw-rw-r--   0 john      (1000) john      (1000)     5342 2024-03-13 08:17:47.000000 stanza-1.8.2/stanza/pipeline/lemma_processor.py
+-rw-rw-r--   0 john      (1000) john      (1000)     8277 2024-03-13 08:17:47.000000 stanza-1.8.2/stanza/pipeline/multilingual.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1928 2024-03-11 03:04:42.000000 stanza-1.8.2/stanza/pipeline/mwt_processor.py
+-rw-rw-r--   0 john      (1000) john      (1000)     6524 2024-01-19 08:13:21.000000 stanza-1.8.2/stanza/pipeline/ner_processor.py
+-rw-rw-r--   0 john      (1000) john      (1000)     3577 2024-04-20 16:29:51.000000 stanza-1.8.2/stanza/pipeline/pos_processor.py
+-rw-rw-r--   0 john      (1000) john      (1000)    10947 2023-09-18 14:41:48.000000 stanza-1.8.2/stanza/pipeline/processor.py
+-rw-rw-r--   0 john      (1000) john      (1000)      224 2022-07-26 21:49:07.000000 stanza-1.8.2/stanza/pipeline/registry.py
+-rw-rw-r--   0 john      (1000) john      (1000)     3154 2024-01-19 08:13:21.000000 stanza-1.8.2/stanza/pipeline/sentiment_processor.py
+-rw-rw-r--   0 john      (1000) john      (1000)     8192 2024-03-13 08:17:47.000000 stanza-1.8.2/stanza/pipeline/tokenize_processor.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-20 16:32:24.070412 stanza-1.8.2/stanza/protobuf/
+-rw-rw-r--   0 john      (1000) john      (1000)    53693 2024-03-13 08:17:47.000000 stanza-1.8.2/stanza/protobuf/CoreNLP_pb2.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1701 2022-07-26 21:49:07.000000 stanza-1.8.2/stanza/protobuf/__init__.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-20 16:32:24.071412 stanza-1.8.2/stanza/resources/
+-rw-rw-r--   0 john      (1000) john      (1000)        0 2022-07-26 21:49:07.000000 stanza-1.8.2/stanza/resources/__init__.py
+-rw-rw-r--   0 john      (1000) john      (1000)    25972 2024-03-13 08:17:47.000000 stanza-1.8.2/stanza/resources/common.py
+-rw-rw-r--   0 john      (1000) john      (1000)    27986 2024-04-20 16:29:51.000000 stanza-1.8.2/stanza/resources/default_packages.py
+-rw-rw-r--   0 john      (1000) john      (1000)     5799 2023-06-22 00:27:12.000000 stanza-1.8.2/stanza/resources/installation.py
+-rw-rw-r--   0 john      (1000) john      (1000)    27855 2024-03-13 08:17:47.000000 stanza-1.8.2/stanza/resources/prepare_resources.py
+-rw-rw-r--   0 john      (1000) john      (1000)      818 2024-01-19 08:13:21.000000 stanza-1.8.2/stanza/resources/print_charlm_depparse.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-20 16:32:24.072412 stanza-1.8.2/stanza/server/
+-rw-rw-r--   0 john      (1000) john      (1000)      624 2022-07-26 21:49:07.000000 stanza-1.8.2/stanza/server/__init__.py
+-rw-rw-r--   0 john      (1000) john      (1000)     4648 2024-01-19 08:13:21.000000 stanza-1.8.2/stanza/server/annotator.py
+-rw-rw-r--   0 john      (1000) john      (1000)    32750 2024-01-19 08:13:21.000000 stanza-1.8.2/stanza/server/client.py
+-rw-rw-r--   0 john      (1000) john      (1000)     4097 2023-09-18 14:41:48.000000 stanza-1.8.2/stanza/server/dependency_converter.py
+-rw-rw-r--   0 john      (1000) john      (1000)    12885 2024-04-20 16:29:51.000000 stanza-1.8.2/stanza/server/java_protobuf_requests.py
+-rw-rw-r--   0 john      (1000) john      (1000)     2619 2022-07-26 21:49:07.000000 stanza-1.8.2/stanza/server/main.py
+-rw-rw-r--   0 john      (1000) john      (1000)     2355 2024-01-19 08:13:21.000000 stanza-1.8.2/stanza/server/morphology.py
+-rw-rw-r--   0 john      (1000) john      (1000)     3032 2024-01-19 08:13:21.000000 stanza-1.8.2/stanza/server/parser_eval.py
+-rw-rw-r--   0 john      (1000) john      (1000)     7625 2024-04-20 16:29:51.000000 stanza-1.8.2/stanza/server/semgrex.py
+-rw-rw-r--   0 john      (1000) john      (1000)    14675 2024-04-20 16:29:51.000000 stanza-1.8.2/stanza/server/ssurgeon.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1356 2023-06-22 00:27:12.000000 stanza-1.8.2/stanza/server/tokensregex.py
+-rw-rw-r--   0 john      (1000) john      (1000)     3144 2023-06-22 00:27:12.000000 stanza-1.8.2/stanza/server/tsurgeon.py
+-rw-rw-r--   0 john      (1000) john      (1000)     3317 2024-01-19 08:13:21.000000 stanza-1.8.2/stanza/server/ud_enhancer.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-20 16:32:24.072412 stanza-1.8.2/stanza/tests/
+-rw-rw-r--   0 john      (1000) john      (1000)     4263 2024-01-19 08:13:21.000000 stanza-1.8.2/stanza/tests/__init__.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-20 16:32:24.073412 stanza-1.8.2/stanza/tests/classifiers/
+-rw-rw-r--   0 john      (1000) john      (1000)        0 2023-09-07 05:52:02.000000 stanza-1.8.2/stanza/tests/classifiers/__init__.py
+-rw-rw-r--   0 john      (1000) john      (1000)    17077 2024-04-20 16:29:51.000000 stanza-1.8.2/stanza/tests/classifiers/test_classifier.py
+-rw-rw-r--   0 john      (1000) john      (1000)     7226 2023-09-18 14:41:48.000000 stanza-1.8.2/stanza/tests/classifiers/test_constituency_classifier.py
+-rw-rw-r--   0 john      (1000) john      (1000)     4949 2023-09-18 14:41:48.000000 stanza-1.8.2/stanza/tests/classifiers/test_data.py
+-rw-rw-r--   0 john      (1000) john      (1000)     3254 2023-09-18 14:41:48.000000 stanza-1.8.2/stanza/tests/classifiers/test_process_utils.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-20 16:32:24.074412 stanza-1.8.2/stanza/tests/common/
+-rw-rw-r--   0 john      (1000) john      (1000)        0 2023-06-22 00:27:12.000000 stanza-1.8.2/stanza/tests/common/__init__.py
+-rw-rw-r--   0 john      (1000) john      (1000)     7609 2024-01-19 08:13:21.000000 stanza-1.8.2/stanza/tests/common/test_char_model.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1049 2024-01-19 08:13:21.000000 stanza-1.8.2/stanza/tests/common/test_chuliu_edmonds.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1210 2023-06-22 00:27:12.000000 stanza-1.8.2/stanza/tests/common/test_common_data.py
+-rw-rw-r--   0 john      (1000) john      (1000)     2897 2024-01-19 08:13:21.000000 stanza-1.8.2/stanza/tests/common/test_confusion.py
+-rw-rw-r--   0 john      (1000) john      (1000)     2470 2023-09-07 05:52:02.000000 stanza-1.8.2/stanza/tests/common/test_constant.py
+-rw-rw-r--   0 john      (1000) john      (1000)    23096 2024-03-13 08:17:47.000000 stanza-1.8.2/stanza/tests/common/test_data_conversion.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1924 2024-01-19 08:13:21.000000 stanza-1.8.2/stanza/tests/common/test_data_objects.py
+-rw-rw-r--   0 john      (1000) john      (1000)     6373 2024-01-19 08:13:21.000000 stanza-1.8.2/stanza/tests/common/test_doc.py
+-rw-rw-r--   0 john      (1000) john      (1000)      918 2023-09-07 05:52:02.000000 stanza-1.8.2/stanza/tests/common/test_dropout.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1059 2023-06-22 00:27:12.000000 stanza-1.8.2/stanza/tests/common/test_foundation_cache.py
+-rw-rw-r--   0 john      (1000) john      (1000)     4435 2023-09-07 05:52:02.000000 stanza-1.8.2/stanza/tests/common/test_pretrain.py
+-rw-rw-r--   0 john      (1000) john      (1000)      556 2023-09-07 05:52:02.000000 stanza-1.8.2/stanza/tests/common/test_short_name_to_treebank.py
+-rw-rw-r--   0 john      (1000) john      (1000)     7017 2023-09-07 05:52:02.000000 stanza-1.8.2/stanza/tests/common/test_utils.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-20 16:32:24.076412 stanza-1.8.2/stanza/tests/constituency/
+-rw-rw-r--   0 john      (1000) john      (1000)        0 2023-06-22 00:27:12.000000 stanza-1.8.2/stanza/tests/constituency/__init__.py
+-rw-rw-r--   0 john      (1000) john      (1000)    11505 2023-06-22 00:27:12.000000 stanza-1.8.2/stanza/tests/constituency/test_convert_arboretum.py
+-rw-rw-r--   0 john      (1000) john      (1000)    18212 2024-04-20 16:29:51.000000 stanza-1.8.2/stanza/tests/constituency/test_convert_it_vit.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1911 2023-06-22 00:27:12.000000 stanza-1.8.2/stanza/tests/constituency/test_convert_starlang.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1707 2024-04-20 16:29:51.000000 stanza-1.8.2/stanza/tests/constituency/test_ensemble.py
+-rw-rw-r--   0 john      (1000) john      (1000)    20385 2023-09-18 14:41:48.000000 stanza-1.8.2/stanza/tests/constituency/test_in_order_oracle.py
+-rw-rw-r--   0 john      (1000) john      (1000)    23445 2024-04-20 16:29:51.000000 stanza-1.8.2/stanza/tests/constituency/test_lstm_model.py
+-rw-rw-r--   0 john      (1000) john      (1000)    17218 2023-09-18 14:41:48.000000 stanza-1.8.2/stanza/tests/constituency/test_parse_transitions.py
+-rw-rw-r--   0 john      (1000) john      (1000)    12458 2023-09-18 14:41:48.000000 stanza-1.8.2/stanza/tests/constituency/test_parse_tree.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1159 2023-09-18 14:41:48.000000 stanza-1.8.2/stanza/tests/constituency/test_positional_encoding.py
+-rw-rw-r--   0 john      (1000) john      (1000)     4434 2023-06-22 00:27:12.000000 stanza-1.8.2/stanza/tests/constituency/test_selftrain_vi_quad.py
+-rw-rw-r--   0 john      (1000) john      (1000)     4316 2024-04-20 16:29:51.000000 stanza-1.8.2/stanza/tests/constituency/test_text_processing.py
+-rw-rw-r--   0 john      (1000) john      (1000)    25364 2024-03-13 08:17:47.000000 stanza-1.8.2/stanza/tests/constituency/test_top_down_oracle.py
+-rw-rw-r--   0 john      (1000) john      (1000)    30616 2024-04-20 16:29:51.000000 stanza-1.8.2/stanza/tests/constituency/test_trainer.py
+-rw-rw-r--   0 john      (1000) john      (1000)     7040 2023-09-07 05:52:02.000000 stanza-1.8.2/stanza/tests/constituency/test_transformer_tree_stack.py
+-rw-rw-r--   0 john      (1000) john      (1000)     7336 2024-04-20 16:29:51.000000 stanza-1.8.2/stanza/tests/constituency/test_transition_sequence.py
+-rw-rw-r--   0 john      (1000) john      (1000)     3408 2023-06-22 00:27:12.000000 stanza-1.8.2/stanza/tests/constituency/test_tree_reader.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1222 2023-06-22 00:27:12.000000 stanza-1.8.2/stanza/tests/constituency/test_tree_stack.py
+-rw-rw-r--   0 john      (1000) john      (1000)     2246 2024-04-20 16:29:51.000000 stanza-1.8.2/stanza/tests/constituency/test_utils.py
+-rw-rw-r--   0 john      (1000) john      (1000)     4795 2023-09-18 14:41:48.000000 stanza-1.8.2/stanza/tests/constituency/test_vietnamese.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-20 16:32:24.077412 stanza-1.8.2/stanza/tests/datasets/
+-rw-rw-r--   0 john      (1000) john      (1000)        0 2023-09-07 05:52:02.000000 stanza-1.8.2/stanza/tests/datasets/__init__.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-20 16:32:24.077412 stanza-1.8.2/stanza/tests/datasets/ner/
+-rw-rw-r--   0 john      (1000) john      (1000)        0 2024-01-19 08:13:21.000000 stanza-1.8.2/stanza/tests/datasets/ner/__init__.py
+-rw-rw-r--   0 john      (1000) john      (1000)     2056 2024-01-19 08:13:21.000000 stanza-1.8.2/stanza/tests/datasets/ner/test_prepare_ner_file.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1328 2024-01-19 08:13:21.000000 stanza-1.8.2/stanza/tests/datasets/ner/test_utils.py
+-rw-rw-r--   0 john      (1000) john      (1000)     2525 2023-09-07 05:52:02.000000 stanza-1.8.2/stanza/tests/datasets/test_common.py
+-rw-rw-r--   0 john      (1000) john      (1000)      903 2023-09-07 05:52:02.000000 stanza-1.8.2/stanza/tests/datasets/test_vietnamese_renormalization.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-20 16:32:24.077412 stanza-1.8.2/stanza/tests/depparse/
+-rw-rw-r--   0 john      (1000) john      (1000)        0 2023-06-22 00:27:12.000000 stanza-1.8.2/stanza/tests/depparse/__init__.py
+-rw-rw-r--   0 john      (1000) john      (1000)     2558 2023-06-22 00:27:12.000000 stanza-1.8.2/stanza/tests/depparse/test_depparse_data.py
+-rw-rw-r--   0 john      (1000) john      (1000)     9674 2024-04-20 16:29:51.000000 stanza-1.8.2/stanza/tests/depparse/test_parser.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-20 16:32:24.077412 stanza-1.8.2/stanza/tests/langid/
+-rw-rw-r--   0 john      (1000) john      (1000)        0 2023-06-22 00:27:12.000000 stanza-1.8.2/stanza/tests/langid/__init__.py
+-rw-rw-r--   0 john      (1000) john      (1000)    45670 2023-09-18 14:41:48.000000 stanza-1.8.2/stanza/tests/langid/test_langid.py
+-rw-rw-r--   0 john      (1000) john      (1000)     3817 2024-01-19 08:13:21.000000 stanza-1.8.2/stanza/tests/langid/test_multilingual.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-20 16:32:24.078412 stanza-1.8.2/stanza/tests/lemma/
+-rw-rw-r--   0 john      (1000) john      (1000)        0 2023-06-22 00:27:12.000000 stanza-1.8.2/stanza/tests/lemma/__init__.py
+-rw-rw-r--   0 john      (1000) john      (1000)     3831 2024-03-13 08:17:47.000000 stanza-1.8.2/stanza/tests/lemma/test_data.py
+-rw-rw-r--   0 john      (1000) john      (1000)     6043 2024-01-19 08:13:21.000000 stanza-1.8.2/stanza/tests/lemma/test_lemma_trainer.py
+-rw-rw-r--   0 john      (1000) john      (1000)     3113 2024-03-13 08:17:47.000000 stanza-1.8.2/stanza/tests/lemma/test_lowercase.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-20 16:32:24.078412 stanza-1.8.2/stanza/tests/mwt/
+-rw-rw-r--   0 john      (1000) john      (1000)        0 2023-09-07 05:52:02.000000 stanza-1.8.2/stanza/tests/mwt/__init__.py
+-rw-rw-r--   0 john      (1000) john      (1000)     3634 2024-04-20 16:29:51.000000 stanza-1.8.2/stanza/tests/mwt/test_english_corner_cases.py
+-rw-rw-r--   0 john      (1000) john      (1000)     3327 2024-04-20 16:29:51.000000 stanza-1.8.2/stanza/tests/mwt/test_prepare_mwt.py
+-rw-rw-r--   0 john      (1000) john      (1000)     2071 2024-01-19 08:13:21.000000 stanza-1.8.2/stanza/tests/mwt/test_utils.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-20 16:32:24.080412 stanza-1.8.2/stanza/tests/ner/
+-rw-rw-r--   0 john      (1000) john      (1000)        0 2023-06-22 00:27:12.000000 stanza-1.8.2/stanza/tests/ner/__init__.py
+-rw-rw-r--   0 john      (1000) john      (1000)     9455 2023-06-22 00:27:12.000000 stanza-1.8.2/stanza/tests/ner/test_bsf_2_beios.py
+-rw-rw-r--   0 john      (1000) john      (1000)     2634 2023-06-22 00:27:12.000000 stanza-1.8.2/stanza/tests/ner/test_bsf_2_iob.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1402 2023-09-18 14:41:48.000000 stanza-1.8.2/stanza/tests/ner/test_combine_ner_datasets.py
+-rw-rw-r--   0 john      (1000) john      (1000)     3364 2023-09-07 05:52:02.000000 stanza-1.8.2/stanza/tests/ner/test_convert_amt.py
+-rw-rw-r--   0 john      (1000) john      (1000)    56852 2023-09-07 05:52:02.000000 stanza-1.8.2/stanza/tests/ner/test_convert_nkjp.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1501 2023-06-22 00:27:12.000000 stanza-1.8.2/stanza/tests/ner/test_convert_starlang_ner.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1167 2024-01-19 08:13:21.000000 stanza-1.8.2/stanza/tests/ner/test_models_ner_scorer.py
+-rw-rw-r--   0 john      (1000) john      (1000)     2510 2024-01-19 08:13:21.000000 stanza-1.8.2/stanza/tests/ner/test_ner_tagger.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1756 2023-06-22 00:27:12.000000 stanza-1.8.2/stanza/tests/ner/test_ner_trainer.py
+-rw-rw-r--   0 john      (1000) john      (1000)     8575 2024-03-13 08:17:47.000000 stanza-1.8.2/stanza/tests/ner/test_ner_training.py
+-rw-rw-r--   0 john      (1000) john      (1000)     6643 2024-01-19 08:13:21.000000 stanza-1.8.2/stanza/tests/ner/test_ner_utils.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1725 2023-09-18 14:41:48.000000 stanza-1.8.2/stanza/tests/ner/test_pay_amt_annotators.py
+-rw-rw-r--   0 john      (1000) john      (1000)     4426 2023-06-22 00:27:12.000000 stanza-1.8.2/stanza/tests/ner/test_split_wikiner.py
+-rw-rw-r--   0 john      (1000) john      (1000)     2742 2023-06-22 00:27:12.000000 stanza-1.8.2/stanza/tests/ner/test_suc3.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-20 16:32:24.082412 stanza-1.8.2/stanza/tests/pipeline/
+-rw-rw-r--   0 john      (1000) john      (1000)        0 2023-06-22 00:27:12.000000 stanza-1.8.2/stanza/tests/pipeline/__init__.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1478 2023-09-18 14:41:48.000000 stanza-1.8.2/stanza/tests/pipeline/pipeline_device_tests.py
+-rw-rw-r--   0 john      (1000) john      (1000)      980 2024-01-19 08:13:21.000000 stanza-1.8.2/stanza/tests/pipeline/test_arabic_pipeline.py
+-rw-rw-r--   0 john      (1000) john      (1000)    11565 2024-01-19 08:13:21.000000 stanza-1.8.2/stanza/tests/pipeline/test_core.py
+-rw-rw-r--   0 john      (1000) john      (1000)     4922 2024-01-19 08:13:21.000000 stanza-1.8.2/stanza/tests/pipeline/test_decorators.py
+-rw-rw-r--   0 john      (1000) john      (1000)     2747 2023-09-07 05:52:02.000000 stanza-1.8.2/stanza/tests/pipeline/test_depparse.py
+-rw-rw-r--   0 john      (1000) john      (1000)    14936 2024-03-13 08:17:47.000000 stanza-1.8.2/stanza/tests/pipeline/test_english_pipeline.py
+-rw-rw-r--   0 john      (1000) john      (1000)     7519 2024-03-13 08:17:47.000000 stanza-1.8.2/stanza/tests/pipeline/test_french_pipeline.py
+-rw-rw-r--   0 john      (1000) john      (1000)     4680 2024-03-13 08:17:47.000000 stanza-1.8.2/stanza/tests/pipeline/test_lemmatizer.py
+-rw-rw-r--   0 john      (1000) john      (1000)     2678 2023-09-18 14:41:48.000000 stanza-1.8.2/stanza/tests/pipeline/test_pipeline_constituency_processor.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1028 2023-09-07 05:52:02.000000 stanza-1.8.2/stanza/tests/pipeline/test_pipeline_depparse_processor.py
+-rw-rw-r--   0 john      (1000) john      (1000)     3385 2024-04-20 16:29:51.000000 stanza-1.8.2/stanza/tests/pipeline/test_pipeline_mwt_expander.py
+-rw-rw-r--   0 john      (1000) john      (1000)     4022 2024-01-19 08:13:21.000000 stanza-1.8.2/stanza/tests/pipeline/test_pipeline_ner_processor.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1777 2024-01-19 08:13:21.000000 stanza-1.8.2/stanza/tests/pipeline/test_pipeline_pos_processor.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1384 2023-06-22 00:27:12.000000 stanza-1.8.2/stanza/tests/pipeline/test_pipeline_sentiment_processor.py
+-rw-rw-r--   0 john      (1000) john      (1000)     3100 2024-01-19 08:13:21.000000 stanza-1.8.2/stanza/tests/pipeline/test_requirements.py
+-rw-rw-r--   0 john      (1000) john      (1000)    22906 2024-01-19 08:13:21.000000 stanza-1.8.2/stanza/tests/pipeline/test_tokenizer.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-20 16:32:24.082412 stanza-1.8.2/stanza/tests/pos/
+-rw-rw-r--   0 john      (1000) john      (1000)        0 2023-06-22 00:27:12.000000 stanza-1.8.2/stanza/tests/pos/__init__.py
+-rw-rw-r--   0 john      (1000) john      (1000)    11175 2024-04-20 16:29:51.000000 stanza-1.8.2/stanza/tests/pos/test_data.py
+-rw-rw-r--   0 john      (1000) john      (1000)    13460 2024-04-20 16:29:51.000000 stanza-1.8.2/stanza/tests/pos/test_tagger.py
+-rw-rw-r--   0 john      (1000) john      (1000)     6700 2024-01-19 08:13:21.000000 stanza-1.8.2/stanza/tests/pos/test_xpos_vocab_factory.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-20 16:32:24.083412 stanza-1.8.2/stanza/tests/resources/
+-rw-rw-r--   0 john      (1000) john      (1000)        0 2023-06-22 00:27:12.000000 stanza-1.8.2/stanza/tests/resources/__init__.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1374 2024-01-19 08:13:21.000000 stanza-1.8.2/stanza/tests/resources/test_charlm_depparse.py
+-rw-rw-r--   0 john      (1000) john      (1000)     5865 2024-01-19 08:13:21.000000 stanza-1.8.2/stanza/tests/resources/test_common.py
+-rw-rw-r--   0 john      (1000) john      (1000)      811 2024-01-19 08:13:21.000000 stanza-1.8.2/stanza/tests/resources/test_default_packages.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1904 2023-06-22 00:27:12.000000 stanza-1.8.2/stanza/tests/resources/test_installation.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1008 2023-06-22 00:27:12.000000 stanza-1.8.2/stanza/tests/resources/test_prepare_resources.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-20 16:32:24.084412 stanza-1.8.2/stanza/tests/server/
+-rw-rw-r--   0 john      (1000) john      (1000)        0 2023-06-22 00:27:12.000000 stanza-1.8.2/stanza/tests/server/__init__.py
+-rw-rw-r--   0 john      (1000) john      (1000)    11550 2024-04-20 16:29:51.000000 stanza-1.8.2/stanza/tests/server/test_client.py
+-rw-rw-r--   0 john      (1000) john      (1000)     3924 2024-03-13 08:17:47.000000 stanza-1.8.2/stanza/tests/server/test_java_protobuf_requests.py
+-rw-rw-r--   0 john      (1000) john      (1000)      674 2024-01-19 08:13:21.000000 stanza-1.8.2/stanza/tests/server/test_morphology.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1864 2024-01-19 08:13:21.000000 stanza-1.8.2/stanza/tests/server/test_parser_eval.py
+-rw-rw-r--   0 john      (1000) john      (1000)     4669 2023-06-22 00:27:12.000000 stanza-1.8.2/stanza/tests/server/test_protobuf.py
+-rw-rw-r--   0 john      (1000) john      (1000)     9062 2024-04-20 16:29:51.000000 stanza-1.8.2/stanza/tests/server/test_semgrex.py
+-rw-rw-r--   0 john      (1000) john      (1000)     5083 2023-06-22 00:27:12.000000 stanza-1.8.2/stanza/tests/server/test_server_misc.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1804 2023-06-22 00:27:12.000000 stanza-1.8.2/stanza/tests/server/test_server_pretokenized.py
+-rw-rw-r--   0 john      (1000) john      (1000)    10460 2023-06-22 00:27:12.000000 stanza-1.8.2/stanza/tests/server/test_server_request.py
+-rw-rw-r--   0 john      (1000) john      (1000)     9732 2023-06-22 00:27:12.000000 stanza-1.8.2/stanza/tests/server/test_server_start.py
+-rw-rw-r--   0 john      (1000) john      (1000)    16455 2024-04-20 16:29:51.000000 stanza-1.8.2/stanza/tests/server/test_ssurgeon.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1334 2023-06-22 00:27:12.000000 stanza-1.8.2/stanza/tests/server/test_tokensregex.py
+-rw-rw-r--   0 john      (1000) john      (1000)     3934 2023-06-22 00:27:12.000000 stanza-1.8.2/stanza/tests/server/test_tsurgeon.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1144 2023-06-22 00:27:12.000000 stanza-1.8.2/stanza/tests/server/test_ud_enhancer.py
+-rw-rw-r--   0 john      (1000) john      (1000)     2477 2024-03-13 08:17:47.000000 stanza-1.8.2/stanza/tests/setup.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-20 16:32:24.085412 stanza-1.8.2/stanza/tests/tokenization/
+-rw-rw-r--   0 john      (1000) john      (1000)        0 2023-06-22 00:27:12.000000 stanza-1.8.2/stanza/tests/tokenization/__init__.py
+-rw-rw-r--   0 john      (1000) john      (1000)    23229 2023-09-18 14:41:48.000000 stanza-1.8.2/stanza/tests/tokenization/test_prepare_tokenizer_treebank.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1072 2024-01-19 08:13:21.000000 stanza-1.8.2/stanza/tests/tokenization/test_replace_long_tokens.py
+-rw-rw-r--   0 john      (1000) john      (1000)     3046 2024-04-20 16:29:51.000000 stanza-1.8.2/stanza/tests/tokenization/test_spaces.py
+-rw-rw-r--   0 john      (1000) john      (1000)     9481 2023-09-07 05:52:02.000000 stanza-1.8.2/stanza/tests/tokenization/test_tokenization_lst20.py
+-rw-rw-r--   0 john      (1000) john      (1000)     5039 2023-09-07 05:52:02.000000 stanza-1.8.2/stanza/tests/tokenization/test_tokenization_orchid.py
+-rw-rw-r--   0 john      (1000) john      (1000)     9844 2023-06-22 00:27:12.000000 stanza-1.8.2/stanza/tests/tokenization/test_tokenize_data.py
+-rw-rw-r--   0 john      (1000) john      (1000)      748 2023-09-07 05:52:02.000000 stanza-1.8.2/stanza/tests/tokenization/test_tokenize_files.py
+-rw-rw-r--   0 john      (1000) john      (1000)    11205 2024-03-13 08:17:47.000000 stanza-1.8.2/stanza/tests/tokenization/test_tokenize_utils.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-20 16:32:24.086412 stanza-1.8.2/stanza/utils/
+-rw-rw-r--   0 john      (1000) john      (1000)        0 2022-07-26 21:49:07.000000 stanza-1.8.2/stanza/utils/__init__.py
+-rw-rw-r--   0 john      (1000) john      (1000)      511 2022-07-26 21:49:07.000000 stanza-1.8.2/stanza/utils/avg_sent_len.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-20 16:32:24.087411 stanza-1.8.2/stanza/utils/charlm/
+-rw-rw-r--   0 john      (1000) john      (1000)        0 2023-06-22 00:27:12.000000 stanza-1.8.2/stanza/utils/charlm/__init__.py
+-rw-rw-r--   0 john      (1000) john      (1000)     3549 2023-06-22 00:27:12.000000 stanza-1.8.2/stanza/utils/charlm/conll17_to_text.py
+-rw-rw-r--   0 john      (1000) john      (1000)     4272 2024-01-19 08:13:21.000000 stanza-1.8.2/stanza/utils/charlm/dump_oscar.py
+-rw-rw-r--   0 john      (1000) john      (1000)     7459 2024-04-20 16:29:51.000000 stanza-1.8.2/stanza/utils/charlm/make_lm_data.py
+-rw-rw-r--   0 john      (1000) john      (1000)     2742 2023-09-18 14:41:48.000000 stanza-1.8.2/stanza/utils/charlm/oscar_to_text.py
+-rw-rw-r--   0 john      (1000) john      (1000)     7337 2024-03-06 02:35:26.000000 stanza-1.8.2/stanza/utils/confusion.py
+-rw-rw-r--   0 john      (1000) john      (1000)     8947 2024-03-13 08:17:47.000000 stanza-1.8.2/stanza/utils/conll.py
+-rwxrwxr-x   0 john      (1000) john      (1000)    40528 2023-09-07 05:52:02.000000 stanza-1.8.2/stanza/utils/conll18_ud_eval.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-20 16:32:24.087411 stanza-1.8.2/stanza/utils/constituency/
+-rw-rw-r--   0 john      (1000) john      (1000)        0 2024-01-19 08:13:21.000000 stanza-1.8.2/stanza/utils/constituency/__init__.py
+-rw-rw-r--   0 john      (1000) john      (1000)      365 2024-01-19 08:13:21.000000 stanza-1.8.2/stanza/utils/constituency/list_tensors.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-20 16:32:24.089412 stanza-1.8.2/stanza/utils/datasets/
+-rw-rw-r--   0 john      (1000) john      (1000)        0 2022-07-26 21:49:07.000000 stanza-1.8.2/stanza/utils/datasets/__init__.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1079 2024-01-18 05:03:09.000000 stanza-1.8.2/stanza/utils/datasets/add_fake_dependencies.py
+-rw-rw-r--   0 john      (1000) john      (1000)    10533 2024-03-13 08:17:47.000000 stanza-1.8.2/stanza/utils/datasets/common.py
+-rw-rw-r--   0 john      (1000) john      (1000)     8641 2022-07-26 21:49:07.000000 stanza-1.8.2/stanza/utils/datasets/conllu_to_text.pl
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-20 16:32:24.092412 stanza-1.8.2/stanza/utils/datasets/constituency/
+-rw-rw-r--   0 john      (1000) john      (1000)        0 2023-06-22 00:27:12.000000 stanza-1.8.2/stanza/utils/datasets/constituency/__init__.py
+-rw-rw-r--   0 john      (1000) john      (1000)     6212 2024-04-20 16:29:51.000000 stanza-1.8.2/stanza/utils/datasets/constituency/build_silver_dataset.py
+-rw-rw-r--   0 john      (1000) john      (1000)      479 2023-09-18 14:41:48.000000 stanza-1.8.2/stanza/utils/datasets/constituency/common_trees.py
+-rw-rw-r--   0 john      (1000) john      (1000)     3686 2023-06-22 00:27:12.000000 stanza-1.8.2/stanza/utils/datasets/constituency/convert_alt.py
+-rw-rw-r--   0 john      (1000) john      (1000)    16062 2023-06-22 00:27:12.000000 stanza-1.8.2/stanza/utils/datasets/constituency/convert_arboretum.py
+-rw-rw-r--   0 john      (1000) john      (1000)     3237 2023-06-22 00:27:12.000000 stanza-1.8.2/stanza/utils/datasets/constituency/convert_cintil.py
+-rw-rw-r--   0 john      (1000) john      (1000)     6441 2024-01-19 08:13:21.000000 stanza-1.8.2/stanza/utils/datasets/constituency/convert_ctb.py
+-rw-rw-r--   0 john      (1000) john      (1000)    13171 2023-06-22 00:27:12.000000 stanza-1.8.2/stanza/utils/datasets/constituency/convert_it_turin.py
+-rw-rw-r--   0 john      (1000) john      (1000)    34313 2024-03-13 08:17:47.000000 stanza-1.8.2/stanza/utils/datasets/constituency/convert_it_vit.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1340 2024-04-20 16:29:51.000000 stanza-1.8.2/stanza/utils/datasets/constituency/convert_spmrl.py
+-rw-rw-r--   0 john      (1000) john      (1000)     3478 2023-06-22 00:27:12.000000 stanza-1.8.2/stanza/utils/datasets/constituency/convert_starlang.py
+-rw-rw-r--   0 john      (1000) john      (1000)      341 2023-09-18 14:41:48.000000 stanza-1.8.2/stanza/utils/datasets/constituency/count_common_words.py
+-rw-rw-r--   0 john      (1000) john      (1000)     2010 2024-03-13 08:17:47.000000 stanza-1.8.2/stanza/utils/datasets/constituency/extract_silver_dataset.py
+-rw-rw-r--   0 john      (1000) john      (1000)    24229 2024-04-20 16:29:51.000000 stanza-1.8.2/stanza/utils/datasets/constituency/prepare_con_dataset.py
+-rw-rw-r--   0 john      (1000) john      (1000)     2472 2024-04-08 00:21:14.000000 stanza-1.8.2/stanza/utils/datasets/constituency/relabel_tags.py
+-rw-rw-r--   0 john      (1000) john      (1000)    10324 2024-01-19 08:13:21.000000 stanza-1.8.2/stanza/utils/datasets/constituency/selftrain.py
+-rw-rw-r--   0 john      (1000) john      (1000)     4277 2023-09-18 14:41:48.000000 stanza-1.8.2/stanza/utils/datasets/constituency/selftrain_it.py
+-rw-rw-r--   0 john      (1000) john      (1000)     2558 2023-09-18 14:41:48.000000 stanza-1.8.2/stanza/utils/datasets/constituency/selftrain_single_file.py
+-rw-rw-r--   0 john      (1000) john      (1000)     3007 2023-09-18 14:41:48.000000 stanza-1.8.2/stanza/utils/datasets/constituency/selftrain_vi_quad.py
+-rw-rw-r--   0 john      (1000) john      (1000)     4782 2023-09-18 14:41:48.000000 stanza-1.8.2/stanza/utils/datasets/constituency/selftrain_wiki.py
+-rw-rw-r--   0 john      (1000) john      (1000)     4980 2024-04-19 18:11:08.000000 stanza-1.8.2/stanza/utils/datasets/constituency/silver_variance.py
+-rw-rw-r--   0 john      (1000) john      (1000)     3726 2024-03-13 08:17:47.000000 stanza-1.8.2/stanza/utils/datasets/constituency/tokenize_wiki.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1488 2023-09-18 14:41:48.000000 stanza-1.8.2/stanza/utils/datasets/constituency/treebank_to_labeled_brackets.py
+-rw-rw-r--   0 john      (1000) john      (1000)      792 2023-06-22 00:27:12.000000 stanza-1.8.2/stanza/utils/datasets/constituency/utils.py
+-rw-rw-r--   0 john      (1000) john      (1000)     9983 2024-01-19 08:13:21.000000 stanza-1.8.2/stanza/utils/datasets/constituency/vtb_convert.py
+-rw-rw-r--   0 john      (1000) john      (1000)     5909 2023-09-18 14:41:48.000000 stanza-1.8.2/stanza/utils/datasets/constituency/vtb_split.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1567 2023-09-18 14:41:48.000000 stanza-1.8.2/stanza/utils/datasets/contract_mwt.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-20 16:32:24.092412 stanza-1.8.2/stanza/utils/datasets/coref/
+-rw-rw-r--   0 john      (1000) john      (1000)        0 2024-01-19 08:13:21.000000 stanza-1.8.2/stanza/utils/datasets/coref/__init__.py
+-rw-rw-r--   0 john      (1000) john      (1000)     9119 2024-01-19 08:13:21.000000 stanza-1.8.2/stanza/utils/datasets/coref/convert_ontonotes.py
+-rw-rw-r--   0 john      (1000) john      (1000)     2956 2024-01-19 08:13:21.000000 stanza-1.8.2/stanza/utils/datasets/corenlp_segmenter_dataset.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-20 16:32:24.096412 stanza-1.8.2/stanza/utils/datasets/ner/
+-rw-rw-r--   0 john      (1000) john      (1000)        0 2023-06-22 00:27:12.000000 stanza-1.8.2/stanza/utils/datasets/ner/__init__.py
+-rw-rw-r--   0 john      (1000) john      (1000)     4114 2024-01-19 08:13:21.000000 stanza-1.8.2/stanza/utils/datasets/ner/build_en_combined.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1932 2023-06-22 00:27:12.000000 stanza-1.8.2/stanza/utils/datasets/ner/check_for_duplicates.py
+-rw-rw-r--   0 john      (1000) john      (1000)      925 2024-01-19 08:13:21.000000 stanza-1.8.2/stanza/utils/datasets/ner/combine_ner_datasets.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1358 2024-01-19 08:13:21.000000 stanza-1.8.2/stanza/utils/datasets/ner/compare_entities.py
+-rw-rw-r--   0 john      (1000) john      (1000)     2128 2023-06-22 00:27:12.000000 stanza-1.8.2/stanza/utils/datasets/ner/conll_to_iob.py
+-rw-rw-r--   0 john      (1000) john      (1000)     9329 2023-09-07 05:52:02.000000 stanza-1.8.2/stanza/utils/datasets/ner/convert_amt.py
+-rw-rw-r--   0 john      (1000) john      (1000)     4041 2024-01-19 08:13:21.000000 stanza-1.8.2/stanza/utils/datasets/ner/convert_ar_aqmar.py
+-rw-rw-r--   0 john      (1000) john      (1000)     4380 2023-09-07 05:52:02.000000 stanza-1.8.2/stanza/utils/datasets/ner/convert_bn_daffodil.py
+-rw-rw-r--   0 john      (1000) john      (1000)     9197 2023-06-22 00:27:12.000000 stanza-1.8.2/stanza/utils/datasets/ner/convert_bsf_to_beios.py
+-rw-rw-r--   0 john      (1000) john      (1000)    17697 2023-06-22 00:27:12.000000 stanza-1.8.2/stanza/utils/datasets/ner/convert_bsnlp.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1536 2024-01-19 08:13:21.000000 stanza-1.8.2/stanza/utils/datasets/ner/convert_en_conll03.py
+-rw-rw-r--   0 john      (1000) john      (1000)     4490 2023-06-22 00:27:12.000000 stanza-1.8.2/stanza/utils/datasets/ner/convert_fire_2013.py
+-rw-rw-r--   0 john      (1000) john      (1000)     5651 2024-01-19 08:13:21.000000 stanza-1.8.2/stanza/utils/datasets/ner/convert_hy_armtdp.py
+-rw-rw-r--   0 john      (1000) john      (1000)     5377 2023-06-22 00:27:12.000000 stanza-1.8.2/stanza/utils/datasets/ner/convert_ijc.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1385 2023-09-07 05:52:02.000000 stanza-1.8.2/stanza/utils/datasets/ner/convert_kk_kazNERD.py
+-rw-rw-r--   0 john      (1000) john      (1000)     3061 2023-06-22 00:27:12.000000 stanza-1.8.2/stanza/utils/datasets/ner/convert_lst20.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1715 2023-06-22 00:27:12.000000 stanza-1.8.2/stanza/utils/datasets/ner/convert_mr_l3cube.py
+-rw-rw-r--   0 john      (1000) john      (1000)     3685 2023-06-22 00:27:12.000000 stanza-1.8.2/stanza/utils/datasets/ner/convert_my_ucsy.py
+-rw-rw-r--   0 john      (1000) john      (1000)    10216 2023-09-07 05:52:02.000000 stanza-1.8.2/stanza/utils/datasets/ner/convert_nkjp.py
+-rw-rw-r--   0 john      (1000) john      (1000)     2366 2024-01-19 08:13:21.000000 stanza-1.8.2/stanza/utils/datasets/ner/convert_nner22.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1472 2023-06-22 00:27:12.000000 stanza-1.8.2/stanza/utils/datasets/ner/convert_nytk.py
+-rw-rw-r--   0 john      (1000) john      (1000)     2727 2024-01-19 08:13:21.000000 stanza-1.8.2/stanza/utils/datasets/ner/convert_ontonotes.py
+-rw-rw-r--   0 john      (1000) john      (1000)     2367 2023-06-22 00:27:12.000000 stanza-1.8.2/stanza/utils/datasets/ner/convert_rgai.py
+-rw-rw-r--   0 john      (1000) john      (1000)     2853 2023-09-07 05:52:02.000000 stanza-1.8.2/stanza/utils/datasets/ner/convert_sindhi_siner.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1615 2023-06-22 00:27:12.000000 stanza-1.8.2/stanza/utils/datasets/ner/convert_starlang_ner.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1122 2024-01-19 08:13:21.000000 stanza-1.8.2/stanza/utils/datasets/ner/count_entities.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1960 2023-09-18 14:41:48.000000 stanza-1.8.2/stanza/utils/datasets/ner/json_to_bio.py
+-rw-rw-r--   0 john      (1000) john      (1000)     3530 2024-01-19 08:13:21.000000 stanza-1.8.2/stanza/utils/datasets/ner/misc_to_date.py
+-rw-rw-r--   0 john      (1000) john      (1000)     4232 2024-01-19 08:13:21.000000 stanza-1.8.2/stanza/utils/datasets/ner/ontonotes_multitag.py
+-rw-rw-r--   0 john      (1000) john      (1000)    57993 2024-01-19 08:13:21.000000 stanza-1.8.2/stanza/utils/datasets/ner/prepare_ner_dataset.py
+-rw-rw-r--   0 john      (1000) john      (1000)     2641 2023-09-07 05:52:02.000000 stanza-1.8.2/stanza/utils/datasets/ner/prepare_ner_file.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1436 2023-06-22 00:27:12.000000 stanza-1.8.2/stanza/utils/datasets/ner/preprocess_wikiner.py
+-rw-rw-r--   0 john      (1000) john      (1000)     5853 2024-01-19 08:13:21.000000 stanza-1.8.2/stanza/utils/datasets/ner/simplify_en_worldwide.py
+-rw-rw-r--   0 john      (1000) john      (1000)     3055 2024-01-19 08:13:21.000000 stanza-1.8.2/stanza/utils/datasets/ner/simplify_ontonotes_to_worldwide.py
+-rw-rw-r--   0 john      (1000) john      (1000)     3366 2023-06-22 00:27:12.000000 stanza-1.8.2/stanza/utils/datasets/ner/split_wikiner.py
+-rw-rw-r--   0 john      (1000) john      (1000)     2484 2023-06-22 00:27:12.000000 stanza-1.8.2/stanza/utils/datasets/ner/suc_conll_to_iob.py
+-rw-rw-r--   0 john      (1000) john      (1000)     5308 2023-06-22 00:27:12.000000 stanza-1.8.2/stanza/utils/datasets/ner/suc_to_iob.py
+-rw-rw-r--   0 john      (1000) john      (1000)    14275 2024-01-19 08:13:21.000000 stanza-1.8.2/stanza/utils/datasets/ner/utils.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-20 16:32:24.096412 stanza-1.8.2/stanza/utils/datasets/pos/
+-rw-rw-r--   0 john      (1000) john      (1000)        0 2023-09-07 05:52:02.000000 stanza-1.8.2/stanza/utils/datasets/pos/__init__.py
+-rw-rw-r--   0 john      (1000) john      (1000)     3724 2024-01-19 08:13:21.000000 stanza-1.8.2/stanza/utils/datasets/pos/convert_trees_to_pos.py
+-rw-rw-r--   0 john      (1000) john      (1000)     6811 2024-03-13 08:17:47.000000 stanza-1.8.2/stanza/utils/datasets/prepare_depparse_treebank.py
+-rw-rw-r--   0 john      (1000) john      (1000)     2007 2024-01-19 08:13:21.000000 stanza-1.8.2/stanza/utils/datasets/prepare_lemma_treebank.py
+-rw-rw-r--   0 john      (1000) john      (1000)     3484 2024-04-20 16:29:51.000000 stanza-1.8.2/stanza/utils/datasets/prepare_mwt_treebank.py
+-rw-rw-r--   0 john      (1000) john      (1000)      656 2024-01-19 08:13:21.000000 stanza-1.8.2/stanza/utils/datasets/prepare_pos_treebank.py
+-rw-rw-r--   0 john      (1000) john      (1000)     5635 2024-04-20 16:29:51.000000 stanza-1.8.2/stanza/utils/datasets/prepare_tokenizer_data.py
+-rwxrwxr-x   0 john      (1000) john      (1000)    51524 2024-04-20 16:29:51.000000 stanza-1.8.2/stanza/utils/datasets/prepare_tokenizer_treebank.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-20 16:32:24.097411 stanza-1.8.2/stanza/utils/datasets/pretrain/
+-rw-rw-r--   0 john      (1000) john      (1000)        0 2023-09-18 14:41:48.000000 stanza-1.8.2/stanza/utils/datasets/pretrain/__init__.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1281 2023-09-18 14:41:48.000000 stanza-1.8.2/stanza/utils/datasets/pretrain/word_in_pretrain.py
+-rw-rw-r--   0 john      (1000) john      (1000)     2625 2024-04-20 16:29:51.000000 stanza-1.8.2/stanza/utils/datasets/random_split_conllu.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-20 16:32:24.099412 stanza-1.8.2/stanza/utils/datasets/sentiment/
+-rw-rw-r--   0 john      (1000) john      (1000)        0 2023-06-22 00:27:12.000000 stanza-1.8.2/stanza/utils/datasets/sentiment/__init__.py
+-rw-rw-r--   0 john      (1000) john      (1000)     4902 2024-03-13 08:17:47.000000 stanza-1.8.2/stanza/utils/datasets/sentiment/add_constituency.py
+-rw-rw-r--   0 john      (1000) john      (1000)     2486 2024-03-13 08:17:47.000000 stanza-1.8.2/stanza/utils/datasets/sentiment/convert_italian_poetry_classification.py
+-rw-rw-r--   0 john      (1000) john      (1000)     3082 2023-09-18 14:41:48.000000 stanza-1.8.2/stanza/utils/datasets/sentiment/convert_italian_sentence_classification.py
+-rw-rw-r--   0 john      (1000) john      (1000)    16102 2024-01-19 08:13:21.000000 stanza-1.8.2/stanza/utils/datasets/sentiment/prepare_sentiment_dataset.py
+-rw-rw-r--   0 john      (1000) john      (1000)     2408 2023-09-07 05:52:02.000000 stanza-1.8.2/stanza/utils/datasets/sentiment/process_MELD.py
+-rw-rw-r--   0 john      (1000) john      (1000)     2631 2023-09-07 05:52:02.000000 stanza-1.8.2/stanza/utils/datasets/sentiment/process_airline.py
+-rw-rw-r--   0 john      (1000) john      (1000)     2880 2023-09-07 05:52:02.000000 stanza-1.8.2/stanza/utils/datasets/sentiment/process_arguana_xml.py
+-rw-rw-r--   0 john      (1000) john      (1000)     2801 2024-01-19 08:13:21.000000 stanza-1.8.2/stanza/utils/datasets/sentiment/process_corona.py
+-rw-rw-r--   0 john      (1000) john      (1000)     8958 2023-09-07 05:52:02.000000 stanza-1.8.2/stanza/utils/datasets/sentiment/process_es_tass2020.py
+-rw-rw-r--   0 john      (1000) john      (1000)     3545 2023-09-07 05:52:02.000000 stanza-1.8.2/stanza/utils/datasets/sentiment/process_it_sentipolc16.py
+-rw-rw-r--   0 john      (1000) john      (1000)     3170 2023-09-07 05:52:02.000000 stanza-1.8.2/stanza/utils/datasets/sentiment/process_ren_chinese.py
+-rw-rw-r--   0 john      (1000) john      (1000)     2839 2023-06-22 00:27:12.000000 stanza-1.8.2/stanza/utils/datasets/sentiment/process_sb10k.py
+-rw-rw-r--   0 john      (1000) john      (1000)     3854 2023-09-07 05:52:02.000000 stanza-1.8.2/stanza/utils/datasets/sentiment/process_scare.py
+-rw-rw-r--   0 john      (1000) john      (1000)     2294 2023-09-07 05:52:02.000000 stanza-1.8.2/stanza/utils/datasets/sentiment/process_slsd.py
+-rw-rw-r--   0 john      (1000) john      (1000)     3159 2023-09-07 05:52:02.000000 stanza-1.8.2/stanza/utils/datasets/sentiment/process_sst.py
+-rw-rw-r--   0 john      (1000) john      (1000)     2551 2023-09-07 05:52:02.000000 stanza-1.8.2/stanza/utils/datasets/sentiment/process_usage_german.py
+-rw-rw-r--   0 john      (1000) john      (1000)     5647 2024-01-19 08:13:21.000000 stanza-1.8.2/stanza/utils/datasets/sentiment/process_utils.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1976 2023-09-07 05:52:02.000000 stanza-1.8.2/stanza/utils/datasets/sentiment/process_vsfc_vietnamese.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1429 2023-06-22 00:27:12.000000 stanza-1.8.2/stanza/utils/datasets/thai_syllable_dict_generator.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-20 16:32:24.100412 stanza-1.8.2/stanza/utils/datasets/tokenization/
+-rw-rw-r--   0 john      (1000) john      (1000)        0 2023-06-22 00:27:12.000000 stanza-1.8.2/stanza/utils/datasets/tokenization/__init__.py
+-rw-rw-r--   0 john      (1000) john      (1000)     9650 2024-01-19 08:13:21.000000 stanza-1.8.2/stanza/utils/datasets/tokenization/convert_ml_cochin.py
+-rw-rw-r--   0 john      (1000) john      (1000)     6431 2023-06-22 00:27:12.000000 stanza-1.8.2/stanza/utils/datasets/tokenization/convert_my_alt.py
+-rw-rw-r--   0 john      (1000) john      (1000)     8336 2023-09-18 14:41:48.000000 stanza-1.8.2/stanza/utils/datasets/tokenization/convert_text_files.py
+-rw-rw-r--   0 john      (1000) john      (1000)     5941 2023-09-07 05:52:02.000000 stanza-1.8.2/stanza/utils/datasets/tokenization/convert_th_best.py
+-rw-rw-r--   0 john      (1000) john      (1000)     5273 2023-06-22 00:27:12.000000 stanza-1.8.2/stanza/utils/datasets/tokenization/convert_th_lst20.py
+-rw-rw-r--   0 john      (1000) john      (1000)     5352 2023-06-22 00:27:12.000000 stanza-1.8.2/stanza/utils/datasets/tokenization/convert_th_orchid.py
+-rw-rw-r--   0 john      (1000) john      (1000)     7383 2023-06-22 00:27:12.000000 stanza-1.8.2/stanza/utils/datasets/tokenization/convert_vi_vlsp.py
+-rw-rw-r--   0 john      (1000) john      (1000)     7697 2023-06-22 00:27:12.000000 stanza-1.8.2/stanza/utils/datasets/tokenization/process_thai_tokenization.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-20 16:32:24.100412 stanza-1.8.2/stanza/utils/datasets/vietnamese/
+-rw-rw-r--   0 john      (1000) john      (1000)        0 2023-09-07 05:52:02.000000 stanza-1.8.2/stanza/utils/datasets/vietnamese/__init__.py
+-rw-rw-r--   0 john      (1000) john      (1000)     3768 2023-09-07 05:52:02.000000 stanza-1.8.2/stanza/utils/datasets/vietnamese/renormalize.py
+-rw-rw-r--   0 john      (1000) john      (1000)     2023 2024-03-06 02:35:26.000000 stanza-1.8.2/stanza/utils/default_paths.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1287 2024-04-20 16:29:51.000000 stanza-1.8.2/stanza/utils/get_tqdm.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1263 2022-07-26 21:49:07.000000 stanza-1.8.2/stanza/utils/helper_func.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-20 16:32:24.100412 stanza-1.8.2/stanza/utils/languages/
+-rw-rw-r--   0 john      (1000) john      (1000)        0 2024-01-19 08:13:21.000000 stanza-1.8.2/stanza/utils/languages/__init__.py
+-rw-rw-r--   0 john      (1000) john      (1000)     6960 2024-01-19 08:13:21.000000 stanza-1.8.2/stanza/utils/languages/kazakh_transliteration.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-20 16:32:24.100412 stanza-1.8.2/stanza/utils/lemma/
+-rw-rw-r--   0 john      (1000) john      (1000)        0 2024-01-19 08:13:21.000000 stanza-1.8.2/stanza/utils/lemma/__init__.py
+-rw-rw-r--   0 john      (1000) john      (1000)      762 2024-01-19 08:13:21.000000 stanza-1.8.2/stanza/utils/lemma/count_ambiguous_lemmas.py
+-rw-rw-r--   0 john      (1000) john      (1000)      329 2022-07-26 21:49:07.000000 stanza-1.8.2/stanza/utils/max_mwt_length.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-20 16:32:24.101412 stanza-1.8.2/stanza/utils/ner/
+-rw-rw-r--   0 john      (1000) john      (1000)        0 2023-09-18 14:41:48.000000 stanza-1.8.2/stanza/utils/ner/__init__.py
+-rw-rw-r--   0 john      (1000) john      (1000)     3445 2024-01-19 08:13:21.000000 stanza-1.8.2/stanza/utils/ner/flair_ner_tag_dataset.py
+-rw-rw-r--   0 john      (1000) john      (1000)     2467 2023-09-18 14:41:48.000000 stanza-1.8.2/stanza/utils/ner/paying_annotators.py
+-rw-rw-r--   0 john      (1000) john      (1000)     4383 2024-01-19 08:13:21.000000 stanza-1.8.2/stanza/utils/ner/spacy_ner_tag_dataset.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-20 16:32:24.101412 stanza-1.8.2/stanza/utils/pretrain/
+-rw-rw-r--   0 john      (1000) john      (1000)        0 2024-01-19 08:13:21.000000 stanza-1.8.2/stanza/utils/pretrain/__init__.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1476 2024-01-19 08:13:21.000000 stanza-1.8.2/stanza/utils/pretrain/compare_pretrains.py
+-rw-rw-r--   0 john      (1000) john      (1000)      451 2022-07-26 21:49:07.000000 stanza-1.8.2/stanza/utils/select_backoff.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-20 16:32:24.102412 stanza-1.8.2/stanza/utils/training/
+-rw-rw-r--   0 john      (1000) john      (1000)        0 2022-07-26 21:49:07.000000 stanza-1.8.2/stanza/utils/training/__init__.py
+-rw-rw-r--   0 john      (1000) john      (1000)    20182 2024-01-19 08:13:21.000000 stanza-1.8.2/stanza/utils/training/common.py
+-rw-rw-r--   0 john      (1000) john      (1000)     3643 2024-01-19 08:13:21.000000 stanza-1.8.2/stanza/utils/training/compose_ete_results.py
+-rw-rw-r--   0 john      (1000) john      (1000)     3416 2024-01-19 08:13:21.000000 stanza-1.8.2/stanza/utils/training/remove_constituency_optimizer.py
+-rw-rw-r--   0 john      (1000) john      (1000)     3361 2024-01-19 08:13:21.000000 stanza-1.8.2/stanza/utils/training/run_charlm.py
+-rw-rw-r--   0 john      (1000) john      (1000)     5288 2024-04-16 00:36:20.000000 stanza-1.8.2/stanza/utils/training/run_constituency.py
+-rw-rw-r--   0 john      (1000) john      (1000)     6221 2024-04-20 16:29:51.000000 stanza-1.8.2/stanza/utils/training/run_depparse.py
+-rw-rw-r--   0 john      (1000) john      (1000)     8200 2024-01-19 08:13:21.000000 stanza-1.8.2/stanza/utils/training/run_ete.py
+-rw-rw-r--   0 john      (1000) john      (1000)     6775 2024-01-19 08:13:21.000000 stanza-1.8.2/stanza/utils/training/run_lemma.py
+-rw-rw-r--   0 john      (1000) john      (1000)     4613 2024-01-19 08:13:21.000000 stanza-1.8.2/stanza/utils/training/run_mwt.py
+-rw-rw-r--   0 john      (1000) john      (1000)     6865 2024-01-19 08:13:21.000000 stanza-1.8.2/stanza/utils/training/run_ner.py
+-rw-rw-r--   0 john      (1000) john      (1000)     6293 2024-04-02 04:28:55.000000 stanza-1.8.2/stanza/utils/training/run_pos.py
+-rw-rw-r--   0 john      (1000) john      (1000)     5035 2024-03-13 08:17:47.000000 stanza-1.8.2/stanza/utils/training/run_sentiment.py
+-rw-rw-r--   0 john      (1000) john      (1000)     4729 2024-01-19 08:13:21.000000 stanza-1.8.2/stanza/utils/training/run_tokenizer.py
+-rw-rw-r--   0 john      (1000) john      (1000)     9930 2023-09-18 14:41:48.000000 stanza-1.8.2/stanza/utils/training/separate_ner_pretrain.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-20 16:32:24.102412 stanza-1.8.2/stanza.egg-info/
+-rw-r--r--   0 john      (1000) john      (1000)    13192 2024-04-20 16:32:24.000000 stanza-1.8.2/stanza.egg-info/PKG-INFO
+-rw-rw-r--   0 john      (1000) john      (1000)    19248 2024-04-20 16:32:24.000000 stanza-1.8.2/stanza.egg-info/SOURCES.txt
+-rw-rw-r--   0 john      (1000) john      (1000)        1 2024-04-20 16:32:24.000000 stanza-1.8.2/stanza.egg-info/dependency_links.txt
+-rw-rw-r--   0 john      (1000) john      (1000)      185 2024-04-20 16:32:24.000000 stanza-1.8.2/stanza.egg-info/requires.txt
+-rw-rw-r--   0 john      (1000) john      (1000)        7 2024-04-20 16:32:24.000000 stanza-1.8.2/stanza.egg-info/top_level.txt
```

### Comparing `stanza-1.8.1/LICENSE` & `stanza-1.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/PKG-INFO` & `stanza-1.8.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stanza
-Version: 1.8.1
+Version: 1.8.2
 Summary: A Python NLP Library for Many Human Languages, by the Stanford NLP Group
 Home-page: https://github.com/stanfordnlp/stanza
 Author: Stanford Natural Language Processing Group
 Author-email: jebolton@stanford.edu
 License: Apache License 2.0
 Keywords: natural-language-processing nlp natural-language-understanding stanford-nlp deep-learning
 Classifier: Development Status :: 4 - Beta
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: stanza Version: 1.8.1 Summary: A Python NLP Library
+Metadata-Version: 2.1 Name: stanza Version: 1.8.2 Summary: A Python NLP Library
 for Many Human Languages, by the Stanford NLP Group Home-page: https://
 github.com/stanfordnlp/stanza Author: Stanford Natural Language Processing
 Group Author-email: jebolton@stanford.edu License: Apache License 2.0 Keywords:
 natural-language-processing nlp natural-language-understanding stanford-nlp
 deep-learning Classifier: Development Status :: 4 - Beta Classifier: Intended
 Audience :: Developers Classifier: Intended Audience :: Education Classifier:
 Intended Audience :: Science/Research Classifier: Intended Audience ::
```

### Comparing `stanza-1.8.1/README.md` & `stanza-1.8.2/README.md`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/setup.py` & `stanza-1.8.2/setup.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/__init__.py` & `stanza-1.8.2/stanza/__init__.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/models/charlm.py` & `stanza-1.8.2/stanza/models/charlm.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/models/classifier.py` & `stanza-1.8.2/stanza/models/classifier.py`

 * *Files 2% similar despite different names*

```diff
@@ -228,14 +228,16 @@
     parser.add_argument('--elmo_projection', type=int, default=None, help='Project elmo to this many dimensions')
 
     parser.add_argument('--bert_model', type=str, default=None, help="Use an external bert model (requires the transformers package)")
     parser.add_argument('--no_bert_model', dest='bert_model', action="store_const", const=None, help="Don't use bert")
     parser.add_argument('--bert_finetune', default=False, action='store_true', help="Finetune the Bert model")
     parser.add_argument('--bert_learning_rate', default=0.01, type=float, help='Scale the learning rate for transformer finetuning by this much')
     parser.add_argument('--bert_weight_decay', default=0.0001, type=float, help='Scale the weight decay for transformer finetuning by this much')
+    parser.add_argument('--bert_hidden_layers', type=int, default=4, help="How many layers of hidden state to use from the transformer")
+    parser.add_argument('--bert_hidden_layers_original', action='store_const', const=None, dest='bert_hidden_layers', help='Use layers 2,3,4 of the Bert embedding')
 
     parser.add_argument('--bilstm', dest='bilstm', action='store_true', default=True, help="Use a bilstm after the inputs, before the convs.  Using bilstm is about as accurate and significantly faster (because of dim reduction) than going straight to the filters")
     parser.add_argument('--no_bilstm', dest='bilstm', action='store_false', help="Don't use a bilstm after the inputs, before the convs.")
     # somewhere between 200-300 seems to be the sweet spot for a couple datasets:
     # dev set macro f1 scores on 3 class problems
     # note that these were only run once each
     # more trials might narrow down which ones works best
@@ -501,14 +503,22 @@
         import wandb
         wandb_name = args.wandb_name if args.wandb_name else "%s_classifier" % args.shorthand
         wandb.init(name=wandb_name, config=args)
         wandb.run.define_metric('accuracy', summary='max')
         wandb.run.define_metric('macro_f1', summary='max')
         wandb.run.define_metric('epoch_loss', summary='min')
 
+    for opt_name, opt in optimizer.items():
+        current_lr = opt.param_groups[0]['lr']
+        logger.info("optimizer %s learning rate: %s", opt_name, current_lr)
+
+    # if this is a brand new training run, and we're saving all intermediate models, save the start model as well
+    if args.save_intermediate_models and trainer.epochs_trained == 0:
+        intermediate_file = intermediate_name(model_file, trainer.epochs_trained, args.dev_eval_scoring, 0.0)
+        trainer.save(intermediate_file, save_optimizer=False)
     for trainer.epochs_trained in range(trainer.epochs_trained, args.max_epochs):
         running_loss = 0.0
         epoch_loss = 0.0
         shuffled_batches = data.shuffle_dataset(train_set_by_len, args.batch_size, args.batch_single_item)
 
         model.train()
         logger.info("Starting epoch %d", trainer.epochs_trained)
@@ -519,21 +529,23 @@
             # logger.debug("Batch size %d max len %d" % (len(batch), max(len(x.text) for x in batch)))
             trainer.global_step += 1
             logger.debug("Starting batch: %d step %d", batch_num, trainer.global_step)
 
             batch_labels = torch.stack([label_tensors[x.sentiment] for x in batch])
 
             # zero the parameter gradients
-            optimizer.zero_grad()
+            for opt in optimizer.values():
+                opt.zero_grad()
 
             outputs = model(batch)
             outputs = process_outputs(outputs)
             batch_loss = loss_function(outputs, batch_labels)
             batch_loss.backward()
-            optimizer.step()
+            for opt in optimizer.values():
+                opt.step()
 
             # print statistics
             running_loss += batch_loss.item()
             if (batch_num + 1) % args.tick == 0: # print every so many batches
                 train_loss = running_loss / args.tick
                 logger.info('[%d, %5d] Average loss: %.3f', trainer.epochs_trained + 1, batch_num + 1, train_loss)
                 if args.wandb:
@@ -586,16 +598,18 @@
     checkpoint_file = None
     if args.train:
         train_set = data.read_dataset(args.train_file, args.wordvec_type, args.min_train_len)
         logger.info("Using training set: %s" % args.train_file)
         logger.info("Training set has %d labels" % len(data.dataset_labels(train_set)))
         tlogger.setLevel(logging.DEBUG)
 
+        tlogger.info("Saving checkpoints: %s", args.checkpoint)
         if args.checkpoint:
             checkpoint_file = utils.checkpoint_name(args.save_dir, save_name, args.checkpoint_save_name)
+            tlogger.info("Checkpoint filename: %s", checkpoint_file)
     elif not args.load_name:
         if save_name:
             args.load_name = save_name
         else:
             raise ValueError("No model provided and not asked to train a model.  This makes no sense")
     else:
         train_set = None
```

### Comparing `stanza-1.8.1/stanza/models/classifiers/base_classifier.py` & `stanza-1.8.2/stanza/models/classifiers/base_classifier.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/models/classifiers/cnn_classifier.py` & `stanza-1.8.2/stanza/models/classifiers/cnn_classifier.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,16 +12,15 @@
 
 import stanza.models.classifiers.data as data
 from stanza.models.classifiers.base_classifier import BaseClassifier
 from stanza.models.classifiers.data import SentimentDatum
 from stanza.models.classifiers.utils import ExtraVectors, ModelType, build_output_layers
 from stanza.models.common.bert_embedding import extract_bert_embeddings
 from stanza.models.common.data import get_long_tensor, sort_all
-from stanza.models.common.foundation_cache import load_bert
-from stanza.models.common.peft_config import build_peft_wrapper
+from stanza.models.common.utils import attach_bert_model
 from stanza.models.common.vocab import PAD_ID, UNK_ID
 
 """
 The CNN classifier is based on Yoon Kim's work:
 
 https://arxiv.org/abs/1408.5882
 
@@ -50,15 +49,15 @@
 """
 
 logger = logging.getLogger('stanza')
 tlogger = logging.getLogger('stanza.classifiers.trainer')
 
 class CNNClassifier(BaseClassifier):
     def __init__(self, pretrain, extra_vocab, labels,
-                 charmodel_forward, charmodel_backward, elmo_model, bert_model, bert_tokenizer, force_bert_saved,
+                 charmodel_forward, charmodel_backward, elmo_model, bert_model, bert_tokenizer, force_bert_saved, peft_name,
                  args):
         """
         pretrain is a pretrained word embedding.  should have .emb and .vocab
 
         extra_vocab is a collection of words in the training data to
         be used for the delta word embedding, if used.  can be set to
         None if delta word embedding is not used.
@@ -74,14 +73,17 @@
         self.labels = labels
         # existing models don't have the bert_finetune or use_peft arguments
         bert_finetune = getattr(args, "bert_finetune", False)
         use_peft = getattr(args, "use_peft", False)
         force_bert_saved = force_bert_saved or bert_finetune
         logger.debug("bert_finetune %s / force_bert_saved %s", bert_finetune, force_bert_saved)
 
+        # this may change when loaded in a new Pipeline, so it's not part of the config
+        self.peft_name = peft_name
+
         # we build a separate config out of the args so that we can easily save it in torch
         self.config = SimpleNamespace(filter_channels = args.filter_channels,
                                       filter_sizes = args.filter_sizes,
                                       fc_shapes = args.fc_shapes,
                                       dropout = args.dropout,
                                       num_classes = len(labels),
                                       wordvec_type = args.wordvec_type,
@@ -92,14 +94,15 @@
                                       charlm_projection = args.charlm_projection,
                                       has_charlm_forward = charmodel_forward is not None,
                                       has_charlm_backward = charmodel_backward is not None,
                                       use_elmo = args.use_elmo,
                                       elmo_projection = args.elmo_projection,
                                       bert_model = args.bert_model,
                                       bert_finetune = bert_finetune,
+                                      bert_hidden_layers = getattr(args, 'bert_hidden_layers', None),
                                       force_bert_saved = force_bert_saved,
 
                                       use_peft = use_peft,
                                       lora_rank = getattr(args, 'lora_rank', None),
                                       lora_alpha = getattr(args, 'lora_alpha', None),
                                       lora_dropout = getattr(args, 'lora_dropout', None),
                                       lora_modules_to_save = getattr(args, 'lora_modules_to_save', None),
@@ -127,24 +130,15 @@
                 raise ValueError("Got a backward charlm as a forward charlm!")
         self.add_unsaved_module('backward_charlm', charmodel_backward)
         if charmodel_backward is not None:
             tlogger.debug("Got backward char model of dimension {}".format(charmodel_backward.hidden_dim()))
             if charmodel_backward.is_forward_lm:
                 raise ValueError("Got a forward charlm as a backward charlm!")
 
-        if self.config.use_peft:
-            bert_model = build_peft_wrapper(bert_model, vars(self.config), tlogger)
-            # we use a peft-specific pathway for saving peft weights
-            self.add_unsaved_module('bert_model', bert_model)
-            self.bert_model.train()
-        elif force_bert_saved:
-            self.bert_model = bert_model
-        else:
-            self.add_unsaved_module('bert_model', bert_model)
-        self.add_unsaved_module('bert_tokenizer', bert_tokenizer)
+        attach_bert_model(self, bert_model, bert_tokenizer, self.config.use_peft, force_bert_saved)
 
         # The Pretrain has PAD and UNK already (indices 0 and 1), but we
         # possibly want to train UNK while freezing the rest of the embedding
         # note that the /10.0 operation has to be inside nn.Parameter unless
         # you want to spend a long time debugging this
         self.unk = nn.Parameter(torch.randn(self.embedding_dim) / np.sqrt(self.embedding_dim) / 10.0)
 
@@ -213,14 +207,28 @@
             if self.config.elmo_projection:
                 self.elmo_projection = nn.Linear(in_features=elmo_dim, out_features=self.config.elmo_projection)
                 total_embedding_dim = total_embedding_dim + self.config.elmo_projection
             else:
                 total_embedding_dim = total_embedding_dim + elmo_dim
 
         if bert_model is not None:
+            if self.config.bert_hidden_layers:
+                # The average will be offset by 1/N so that the default zeros
+                # repressents an average of the N layers
+                if self.config.bert_hidden_layers > bert_model.config.num_hidden_layers:
+                    # limit ourselves to the number of layers actually available
+                    # note that we can +1 because of the initial embedding layer
+                    self.config.bert_hidden_layers = bert_model.config.num_hidden_layers + 1
+                self.bert_layer_mix = nn.Linear(self.config.bert_hidden_layers, 1, bias=False)
+                nn.init.zeros_(self.bert_layer_mix.weight)
+            else:
+                # an average of layers 2, 3, 4 will be used
+                # (for historic reasons)
+                self.bert_layer_mix = None
+
             if bert_tokenizer is None:
                 raise ValueError("Cannot have a bert model without a tokenizer")
             self.bert_dim = self.bert_model.config.hidden_size
             total_embedding_dim += self.bert_dim
 
         if self.config.bilstm:
             conv_input_dim = self.config.bilstm_hidden_dim * 2
@@ -309,15 +317,24 @@
         for idx, rep in enumerate(char_reps):
             start = begin_paddings[idx]
             end = start + rep.shape[0]
             char_inputs[idx, start:end, :] = rep
         return char_inputs
 
     def extract_bert_embeddings(self, inputs, max_phrase_len, begin_paddings, device):
-        bert_embeddings = extract_bert_embeddings(self.config.bert_model, self.bert_tokenizer, self.bert_model, inputs, device, keep_endpoints=False, detach=not self.config.bert_finetune)
+        bert_embeddings = extract_bert_embeddings(self.config.bert_model, self.bert_tokenizer, self.bert_model, inputs, device,
+                                                  keep_endpoints=False,
+                                                  num_layers=self.bert_layer_mix.in_features if self.bert_layer_mix is not None else None,
+                                                  detach=not self.config.bert_finetune,
+                                                  peft_name=self.peft_name)
+        if self.bert_layer_mix is not None:
+            # add the average so that the default behavior is to
+            # take an average of the N layers, and anything else
+            # other than that needs to be learned
+            bert_embeddings = [self.bert_layer_mix(feature).squeeze(2) + feature.sum(axis=2) / self.bert_layer_mix.in_features for feature in bert_embeddings]
         bert_inputs = torch.zeros((len(inputs), max_phrase_len, bert_embeddings[0].shape[-1]), device=device)
         for idx, rep in enumerate(bert_embeddings):
             start = begin_paddings[idx]
             end = start + rep.shape[0]
             bert_inputs[idx, start:end, :] = rep
         return bert_inputs
 
@@ -509,15 +526,15 @@
             'config':       self.config,
             'labels':       self.labels,
             'extra_vocab':  self.extra_vocab,
         }
         if self.config.use_peft:
             # Hide import so that peft dependency is optional
             from peft import get_peft_model_state_dict
-            params["bert_lora"] = get_peft_model_state_dict(self.bert_model)
+            params["bert_lora"] = get_peft_model_state_dict(self.bert_model, adapter_name=self.peft_name)
         return params
 
     def preprocess_data(self, sentences):
         sentences = [data.update_text(s, self.config.wordvec_type) for s in sentences]
         return sentences
 
     def extract_sentences(self, doc):
```

### Comparing `stanza-1.8.1/stanza/models/classifiers/constituency_classifier.py` & `stanza-1.8.2/stanza/models/classifiers/constituency_classifier.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/models/classifiers/data.py` & `stanza-1.8.2/stanza/models/classifiers/data.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/models/classifiers/iterate_test.py` & `stanza-1.8.2/stanza/models/classifiers/iterate_test.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/models/classifiers/trainer.py` & `stanza-1.8.2/stanza/models/classifiers/trainer.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,17 +9,18 @@
 import torch
 import torch.optim as optim
 
 import stanza.models.classifiers.data as data
 import stanza.models.classifiers.cnn_classifier as cnn_classifier
 import stanza.models.classifiers.constituency_classifier as constituency_classifier
 from stanza.models.classifiers.utils import ModelType
-from stanza.models.common.foundation_cache import load_bert, load_charlm, load_pretrain
+from stanza.models.common.foundation_cache import load_bert, load_bert_with_peft, load_charlm, load_pretrain
+from stanza.models.common.peft_config import build_peft_wrapper, load_peft_wrapper
 from stanza.models.common.pretrain import Pretrain
-from stanza.models.common.utils import get_optimizer
+from stanza.models.common.utils import get_split_optimizer
 from stanza.models.constituency.tree_embedding import TreeEmbedding
 
 logger = logging.getLogger('stanza')
 
 class Trainer:
     """
     Stores a constituency model and its optimizer
@@ -50,15 +51,15 @@
         params = {
             'params':         model_params,
             'epochs_trained': epochs_trained,
             'global_step':    self.global_step,
             'best_score':     self.best_score,
         }
         if save_optimizer and self.optimizer is not None:
-            params['optimizer_state_dict'] = self.optimizer.state_dict()
+            params['optimizer_state_dict'] = {opt_name: opt.state_dict() for opt_name, opt in self.optimizer.items()}
         torch.save(params, filename, _use_new_zipfile_serialization=False)
         logger.info("Model saved to {}".format(filename))
 
     @staticmethod
     def load(filename, args, foundation_cache=None, load_optimizer=False):
         if not os.path.exists(filename):
             if args.save_dir is None:
@@ -108,70 +109,68 @@
             else:
                 charmodel_backward = None
 
             bert_model = model_params['config'].bert_model
             # TODO: can get rid of the getattr after rebuilding all models
             use_peft = getattr(model_params['config'], 'use_peft', False)
             force_bert_saved = getattr(model_params['config'], 'force_bert_saved', False)
-            if use_peft or force_bert_saved:
+            peft_name = None
+            if use_peft:
                 # if loading a peft model, we first load the base transformer
                 # the CNNClassifier code wraps the transformer in peft
                 # after creating the CNNClassifier with the peft wrapper,
                 # we *then* load the weights
+                bert_model, bert_tokenizer, peft_name = load_bert_with_peft(bert_model, "classifier", foundation_cache)
+                bert_model = load_peft_wrapper(bert_model, model_params['bert_lora'], vars(model_params['config']), logger, peft_name)
+            elif force_bert_saved:
                 bert_model, bert_tokenizer = load_bert(bert_model)
             else:
                 bert_model, bert_tokenizer = load_bert(bert_model, foundation_cache)
             model = cnn_classifier.CNNClassifier(pretrain=pretrain,
                                                  extra_vocab=model_params['extra_vocab'],
                                                  labels=model_params['labels'],
                                                  charmodel_forward=charmodel_forward,
                                                  charmodel_backward=charmodel_backward,
                                                  elmo_model=elmo_model,
                                                  bert_model=bert_model,
                                                  bert_tokenizer=bert_tokenizer,
                                                  force_bert_saved=force_bert_saved,
+                                                 peft_name=peft_name,
                                                  args=model_params['config'])
         elif model_type == ModelType.CONSTITUENCY:
             # the constituency version doesn't have a peft feature yet
             use_peft = False
             pretrain_args = {
                 'wordvec_pretrain_file': args.wordvec_pretrain_file,
                 'charlm_forward_file': args.charlm_forward_file,
                 'charlm_backward_file': args.charlm_backward_file,
             }
+            # TODO: integrate with peft for the constituency version
             tree_embedding = TreeEmbedding.model_from_params(model_params['tree_embedding'], pretrain_args, foundation_cache)
             model = constituency_classifier.ConstituencyClassifier(tree_embedding=tree_embedding,
                                                                    labels=model_params['labels'],
                                                                    args=model_params['config'])
         else:
             raise ValueError("Unknown model type {}".format(model_type))
         model.load_state_dict(model_params['model'], strict=False)
-        if use_peft:
-            # hide import so that the peft dependency is optional
-            from peft import set_peft_model_state_dict
-            # we do the peft loading after the rest of the model
-            # loading - there seems to be something in the
-            # load_state_dict which clobbers the peft scores
-            # otherwise.  probably we should be filtering those from
-            # the model files to keep the size smaller
-            set_peft_model_state_dict(model.bert_model, model_params['bert_lora'])
         model = model.to(args.device)
 
         logger.debug("-- MODEL CONFIG --")
         for k in model.config.__dict__:
             logger.debug("  --{}: {}".format(k, model.config.__dict__[k]))
 
         logger.debug("-- MODEL LABELS --")
         logger.debug("  {}".format(" ".join(model.labels)))
 
         optimizer = None
         if load_optimizer:
             optimizer = Trainer.build_optimizer(model, args)
             if checkpoint.get('optimizer_state_dict', None) is not None:
-                optimizer.load_state_dict(checkpoint['optimizer_state_dict'])
+                for opt_name, opt_state_dict in checkpoint['optimizer_state_dict'].items():
+                    optimizer[opt_name].load_state_dict(opt_state_dict)
             else:
                 logger.info("Attempted to load optimizer to resume training, but optimizer not saved.  Creating new optimizer")
 
         trainer = Trainer(model, optimizer, epochs_trained, global_step, best_score)
 
         return trainer
 
@@ -209,27 +208,34 @@
         labels = data.dataset_labels(train_set)
 
         if args.model_type == ModelType.CNN:
             pretrain = Trainer.load_pretrain(args, foundation_cache=None)
             elmo_model = utils.load_elmo(args.elmo_model) if args.use_elmo else None
             charmodel_forward = load_charlm(args.charlm_forward_file)
             charmodel_backward = load_charlm(args.charlm_backward_file)
+            peft_name = None
             bert_model, bert_tokenizer = load_bert(args.bert_model)
 
+            use_peft = getattr(args, "use_peft", False)
+            if use_peft:
+                peft_name = "sentiment"
+                bert_model = build_peft_wrapper(bert_model, vars(args), logger, adapter_name=peft_name)
+
             extra_vocab = data.dataset_vocab(train_set)
             force_bert_saved = args.bert_finetune
             model = cnn_classifier.CNNClassifier(pretrain=pretrain,
                                                  extra_vocab=extra_vocab,
                                                  labels=labels,
                                                  charmodel_forward=charmodel_forward,
                                                  charmodel_backward=charmodel_backward,
                                                  elmo_model=elmo_model,
                                                  bert_model=bert_model,
                                                  bert_tokenizer=bert_tokenizer,
                                                  force_bert_saved=force_bert_saved,
+                                                 peft_name=peft_name,
                                                  args=args)
             model = model.to(args.device)
         elif args.model_type == ModelType.CONSTITUENCY:
             # this passes flags such as "constituency_backprop" from
             # the classifier to the TreeEmbedding as the "backprop" flag
             parser_args = { x[len("constituency_"):]: y for x, y in vars(args).items() if x.startswith("constituency_") }
             parser_args.update({
@@ -259,8 +265,8 @@
         optimizer = Trainer.build_optimizer(model, args)
 
         return Trainer(model, optimizer)
 
 
     @staticmethod
     def build_optimizer(model, args):
-        return get_optimizer(args.optim.lower(), model, args.learning_rate, momentum=args.momentum, weight_decay=args.weight_decay, bert_learning_rate=args.bert_learning_rate, bert_weight_decay=args.weight_decay * args.bert_weight_decay, is_peft=args.use_peft)
+        return get_split_optimizer(args.optim.lower(), model, args.learning_rate, momentum=args.momentum, weight_decay=args.weight_decay, bert_learning_rate=args.bert_learning_rate, bert_weight_decay=args.weight_decay * args.bert_weight_decay, is_peft=args.use_peft)
```

### Comparing `stanza-1.8.1/stanza/models/classifiers/utils.py` & `stanza-1.8.2/stanza/models/classifiers/utils.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/models/common/beam.py` & `stanza-1.8.2/stanza/models/common/beam.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/models/common/bert_embedding.py` & `stanza-1.8.2/stanza/models/common/bert_embedding.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     def __init__(self, length, max_len, line_num, text):
         super().__init__("Found a text of length %d (possibly after tokenizing).  Maximum handled length is %d  Error occurred at line %d" % (length, max_len, line_num))
         self.line_num = line_num
         self.text = text
 
 
 def update_max_length(model_name, tokenizer):
-    if model_name in ('google/muril-base-cased', 'airesearch/wangchanberta-base-att-spm-uncased', 'camembert/camembert-large', 'hfl/chinese-electra-180g-large-discriminator'):
+    if model_name in ('google/muril-base-cased', 'google/muril-large-cased', 'airesearch/wangchanberta-base-att-spm-uncased', 'camembert/camembert-large', 'hfl/chinese-electra-180g-large-discriminator'):
         tokenizer.model_max_length = 512
 
 def load_tokenizer(model_name):
     if model_name:
         # note that use_fast is the default
         try:
             from transformers import AutoTokenizer
@@ -379,35 +379,15 @@
             break
         remaining_attention = remaining_attention[:, slice_len:]
         remaining_ids = id_tensor[:, slice_len:]
     slices = torch.cat(slices, axis=1)
     return slices
 
 
-def extract_bert_embeddings(model_name, tokenizer, model, data, device, keep_endpoints, num_layers=None, detach=True):
-    """
-    Extract transformer embeddings using a generic roberta extraction
-
-    data: list of list of string (the text tokens)
-    num_layers: how many to return.  If None, the average of -2, -3, -4 is returned
-    """
-    if model_name.startswith("vinai/phobert"):
-        return extract_phobert_embeddings(model_name, tokenizer, model, data, device, keep_endpoints, num_layers, detach)
-
-    if 'bart' in model_name:
-        # this should work with "vinai/bartpho-word"
-        # not sure this works with any other Bart
-        return extract_bart_word_embeddings(model_name, tokenizer, model, data, device, keep_endpoints, num_layers, detach)
-
-    if isinstance(data, tuple):
-        data = list(data)
-
-    if "xlnet" in model_name:
-        return extract_xlnet_embeddings(model_name, tokenizer, model, data, device, keep_endpoints, num_layers, detach)
-
+def extract_base_embeddings(model_name, tokenizer, model, data, device, keep_endpoints, num_layers, detach):
     data = fix_blank_tokens(tokenizer, data)
 
     #add add_prefix_space = True for RoBerTa-- error if not
     # using attention masks makes contextual embeddings much more useful for downstream tasks
     tokenized = tokenizer(data, padding="longest", is_split_into_words=True, return_offsets_mapping=False, return_attention_mask=True)
     list_offsets = [[None] * (len(sentence)+2) for sentence in data]
     for idx in range(len(data)):
@@ -442,7 +422,40 @@
         #remove the bos and eos tokens
         list_offsets = [sent[1:-1] for sent in list_offsets]
     for feature, offsets in zip(features, list_offsets):
         new_sent = feature[offsets]
         processed.append(new_sent)
 
     return processed
+
+def extract_bert_embeddings(model_name, tokenizer, model, data, device, keep_endpoints, num_layers=None, detach=True, peft_name=None):
+    """
+    Extract transformer embeddings using a generic roberta extraction
+
+    data: list of list of string (the text tokens)
+    num_layers: how many to return.  If None, the average of -2, -3, -4 is returned
+    """
+    # TODO: can maybe cache this value for a model and save some time
+    # TODO: too bad it isn't thread safe, but then again, who does?
+    if peft_name is None:
+        if model._hf_peft_config_loaded:
+            model.disable_adapters()
+    else:
+        model.enable_adapters()
+        model.set_adapter(peft_name)
+
+    if model_name.startswith("vinai/phobert"):
+        return extract_phobert_embeddings(model_name, tokenizer, model, data, device, keep_endpoints, num_layers, detach)
+
+    if 'bart' in model_name:
+        # this should work with "vinai/bartpho-word"
+        # not sure this works with any other Bart
+        return extract_bart_word_embeddings(model_name, tokenizer, model, data, device, keep_endpoints, num_layers, detach)
+
+    if isinstance(data, tuple):
+        data = list(data)
+
+    if "xlnet" in model_name:
+        return extract_xlnet_embeddings(model_name, tokenizer, model, data, device, keep_endpoints, num_layers, detach)
+
+    return extract_base_embeddings(model_name, tokenizer, model, data, device, keep_endpoints, num_layers, detach)
+
```

### Comparing `stanza-1.8.1/stanza/models/common/biaffine.py` & `stanza-1.8.2/stanza/models/common/biaffine.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/models/common/build_short_name_to_treebank.py` & `stanza-1.8.2/stanza/models/common/build_short_name_to_treebank.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/models/common/char_model.py` & `stanza-1.8.2/stanza/models/common/char_model.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/models/common/chuliu_edmonds.py` & `stanza-1.8.2/stanza/models/common/chuliu_edmonds.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/models/common/constant.py` & `stanza-1.8.2/stanza/models/common/constant.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/models/common/convert_pretrain.py` & `stanza-1.8.2/stanza/models/common/convert_pretrain.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/models/common/count_ner_coverage.py` & `stanza-1.8.2/stanza/models/common/count_ner_coverage.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/models/common/count_pretrain_coverage.py` & `stanza-1.8.2/stanza/models/common/count_pretrain_coverage.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/models/common/crf.py` & `stanza-1.8.2/stanza/models/common/crf.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/models/common/data.py` & `stanza-1.8.2/stanza/models/common/data.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/models/common/doc.py` & `stanza-1.8.2/stanza/models/common/doc.py`

 * *Files 1% similar despite different names*

```diff
@@ -384,14 +384,21 @@
             sentence.words = []
             for token in sentence.tokens:
                 token.sent = sentence
                 for word in token.words:
                     word.sent = sentence
                     word.parent = token
                     sentence.words.append(word)
+                if len(token.words) > 1 and token.start_char is not None and token.end_char is not None and "".join(word.text for word in token.words) == token.text:
+                    start_char = token.start_char
+                    for word in token.words:
+                        end_char = start_char + len(word.text)
+                        word.start_char = start_char
+                        word.end_char = end_char
+                        start_char = end_char
 
             if fake_dependencies:
                 sentence.build_fake_dependencies()
             else:
                 sentence.rebuild_dependencies()
 
         self._count_words() # update number of words & tokens
@@ -1459,19 +1466,27 @@
         self._misc = value if self._is_null(value) == False else None
 
     @property
     def start_char(self):
         """ Access the start character index for this token in the raw text. """
         return self._start_char
 
+    @start_char.setter
+    def start_char(self, value):
+        self._start_char = value
+
     @property
     def end_char(self):
         """ Access the end character index for this token in the raw text. """
         return self._end_char
 
+    @end_char.setter
+    def end_char(self, value):
+        self._end_char = value
+
     @property
     def parent(self):
         """ Access the parent token of this word. In the case of a multi-word token, a token can be the parent of
         multiple words. Note that this should return a reference to the parent token object.
         """
         return self._parent
```

### Comparing `stanza-1.8.1/stanza/models/common/dropout.py` & `stanza-1.8.2/stanza/models/common/dropout.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/models/common/hlstm.py` & `stanza-1.8.2/stanza/models/common/hlstm.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/models/common/large_margin_loss.py` & `stanza-1.8.2/stanza/models/common/large_margin_loss.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/models/common/loss.py` & `stanza-1.8.2/stanza/models/common/loss.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/models/common/maxout_linear.py` & `stanza-1.8.2/stanza/models/common/maxout_linear.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/models/common/packed_lstm.py` & `stanza-1.8.2/stanza/models/common/packed_lstm.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/models/common/pretrain.py` & `stanza-1.8.2/stanza/models/common/pretrain.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/models/common/seq2seq_model.py` & `stanza-1.8.2/stanza/models/common/seq2seq_model.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/models/common/seq2seq_modules.py` & `stanza-1.8.2/stanza/models/common/seq2seq_modules.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/models/common/seq2seq_utils.py` & `stanza-1.8.2/stanza/models/common/seq2seq_utils.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/models/common/short_name_to_treebank.py` & `stanza-1.8.2/stanza/models/common/short_name_to_treebank.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/models/common/stanza_object.py` & `stanza-1.8.2/stanza/models/common/stanza_object.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/models/common/trainer.py` & `stanza-1.8.2/stanza/models/common/trainer.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/models/common/utils.py` & `stanza-1.8.2/stanza/models/common/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -782,7 +782,21 @@
     name_len = max(len(x[0]) for x in pieces)
     norm_len = max(len(x[1]) for x in pieces)
     line_format = "  %-" + str(name_len) + "s   %" + str(norm_len) + "s     %s"
     for line in pieces:
         lines.append(line_format % line)
     logger.info("\n".join(lines))
 
+def attach_bert_model(model, bert_model, bert_tokenizer, use_peft, force_bert_saved):
+    if use_peft:
+        # we use a peft-specific pathway for saving peft weights
+        model.add_unsaved_module('bert_model', bert_model)
+        model.bert_model.train()
+    elif force_bert_saved:
+        model.bert_model = bert_model
+    elif bert_model is not None:
+        model.add_unsaved_module('bert_model', bert_model)
+        for _, parameter in bert_model.named_parameters():
+            parameter.requires_grad = False
+    else:
+        model.bert_model = None
+    model.add_unsaved_module('bert_tokenizer', bert_tokenizer)
```

### Comparing `stanza-1.8.1/stanza/models/common/vocab.py` & `stanza-1.8.2/stanza/models/common/vocab.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/models/constituency/base_model.py` & `stanza-1.8.2/stanza/models/constituency/base_model.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,18 +20,18 @@
 from abc import ABC, abstractmethod
 from collections import defaultdict
 import logging
 
 import torch
 
 from stanza.models.common import utils
-from stanza.models.constituency import parse_transitions
 from stanza.models.constituency import transition_sequence
-from stanza.models.constituency.parse_transitions import State, TransitionScheme, CloseConstituent
+from stanza.models.constituency.parse_transitions import TransitionScheme, CloseConstituent
 from stanza.models.constituency.parse_tree import Tree
+from stanza.models.constituency.state import State
 from stanza.models.constituency.tree_stack import TreeStack
 from stanza.server.parser_eval import ParseResult, ScoredTree
 
 # default unary limit.  some treebanks may have longer chains (CTB, for example)
 UNARY_LIMIT = 4
 
 logger = logging.getLogger('stanza.constituency.trainer')
@@ -161,14 +161,15 @@
         """
         Whether or not this model is TOP_DOWN
         """
         return (self._transition_scheme is TransitionScheme.TOP_DOWN or
                 self._transition_scheme is TransitionScheme.TOP_DOWN_UNARY or
                 self._transition_scheme is TransitionScheme.TOP_DOWN_COMPOUND)
 
+    @property
     def reverse_sentence(self):
         """
         Whether or not this model is built to parse backwards
         """
         return self._reverse_sentence
 
     def predict(self, states, is_legal=True):
@@ -184,15 +185,15 @@
         transitions = [y.gold_sequence[y.num_transitions()] for y in states]
         if is_legal:
             for trans, state in zip(transitions, states):
                 if not trans.is_legal(state, self):
                     raise RuntimeError("Transition {}:{} was not legal in a transition sequence:\nOriginal tree: {}\nTransitions: {}".format(state.num_transitions(), trans, state.gold_tree, state.gold_sequence))
         return None, transitions, None
 
-    def initial_state_from_preterminals(self, preterminal_lists, gold_trees):
+    def initial_state_from_preterminals(self, preterminal_lists, gold_trees, gold_sequences):
         """
         what is passed in should be a list of list of preterminals
         """
         word_queues = self.initial_word_queues(preterminal_lists)
         # this is the bottom of the TreeStack and will be the same for each State
         transitions = self.initial_transitions()
         constituents = self.initial_constituents()
@@ -204,26 +205,28 @@
                         transitions=transitions,
                         constituents=constituents,
                         word_position=0,
                         score=0.0)
                   for idx, wq in enumerate(word_queues)]
         if gold_trees:
             states = [state._replace(gold_tree=gold_tree) for gold_tree, state in zip(gold_trees, states)]
+        if gold_sequences:
+            states = [state._replace(gold_sequence=gold_sequence) for gold_sequence, state in zip(gold_sequences, states)]
         return states
 
     def initial_state_from_words(self, word_lists):
         preterminal_lists = [[Tree(tag, Tree(word)) for word, tag in words]
                              for words in word_lists]
-        return self.initial_state_from_preterminals(preterminal_lists, gold_trees=None)
+        return self.initial_state_from_preterminals(preterminal_lists, gold_trees=None, gold_sequences=None)
 
     def initial_state_from_gold_trees(self, trees):
         preterminal_lists = [[Tree(pt.label, Tree(pt.children[0].label))
                               for pt in tree.yield_preterminals()]
                              for tree in trees]
-        return self.initial_state_from_preterminals(preterminal_lists, gold_trees=trees)
+        return self.initial_state_from_preterminals(preterminal_lists, gold_trees=trees, gold_sequences=None)
 
     def build_batch_from_trees(self, batch_size, data_iterator):
         """
         Read from the data_iterator batch_size trees and turn them into new parsing states
         """
         state_batch = []
         for _ in range(batch_size):
@@ -240,15 +243,15 @@
         """
         Same as build_batch_from_trees, but use the model parameters to turn the trees into gold sequences and include the sequence
         """
         state_batch = self.build_batch_from_trees(batch_size, data_iterator)
         if len(state_batch) == 0:
             return state_batch
 
-        gold_sequences = transition_sequence.build_treebank([state.gold_tree for state in state_batch], self.transition_scheme(), self.reverse_sentence())
+        gold_sequences = transition_sequence.build_treebank([state.gold_tree for state in state_batch], self.transition_scheme(), self.reverse_sentence)
         state_batch = [state._replace(gold_sequence=sequence) for state, sequence in zip(state_batch, gold_sequences)]
         return state_batch
 
     def build_batch_from_tagged_words(self, batch_size, data_iterator):
         """
         Read from the data_iterator batch_size tagged sentences and turn them into new parsing states
 
@@ -294,29 +297,29 @@
         if keep_constituents:
             constituents = defaultdict(list)
 
         while len(state_batch) > 0:
             pred_scores, transitions, scores = transition_choice(state_batch)
             if keep_scores and scores is not None:
                 state_batch = [state._replace(score=state.score + score) for state, score in zip(state_batch, scores)]
-            state_batch = parse_transitions.bulk_apply(self, state_batch, transitions)
+            state_batch = self.bulk_apply(state_batch, transitions)
 
             if keep_constituents:
                 for t_idx, transition in enumerate(transitions):
                     if isinstance(transition, CloseConstituent):
                         # constituents is a TreeStack with information on how to build the next state of the LSTM or attn
                         # constituents.value is the TreeStack node
                         # constituents.value.value is the Constituent itself (with the tree and the embedding)
                         constituents[batch_indices[t_idx]].append(state_batch[t_idx].constituents.value.value)
 
             remove = set()
             for idx, state in enumerate(state_batch):
                 if state.finished(self):
                     predicted_tree = state.get_tree(self)
-                    if self.reverse_sentence():
+                    if self.reverse_sentence:
                         predicted_tree = predicted_tree.reverse()
                     gold_tree = state.gold_tree
                     treebank.append(ParseResult(gold_tree, [ScoredTree(predicted_tree, state.score)], state if keep_state else None, constituents[batch_indices[idx]] if keep_constituents else None))
                     treebank_indices.append(batch_indices[idx])
                     remove.add(idx)
 
             if len(remove) > 0:
@@ -382,14 +385,89 @@
 
         sentence_iterator = iter(words)
         treebank = self.parse_sentences_no_grad(sentence_iterator, self.build_batch_from_tagged_words, batch_size, self.predict, keep_state=False, keep_constituents=False)
 
         results = [t.predictions[0].tree for t in treebank]
         return results
 
+    def bulk_apply(self, state_batch, transitions, fail=False):
+        """
+        Apply the given list of Transitions to the given list of States, using the model as a reference
+
+        model: SimpleModel, LSTMModel, or any other form of model
+        state_batch: list of States
+        transitions: list of transitions, one per state
+        fail: throw an exception on a failed transition, as opposed to skipping the tree
+        """
+        remove = set()
+
+        word_positions = []
+        constituents = []
+        new_constituents = []
+        callbacks = defaultdict(list)
+
+        for idx, (tree, transition) in enumerate(zip(state_batch, transitions)):
+            if not transition:
+                error = "Got stuck and couldn't find a legal transition on the following gold tree:\n{}\n\nFinal state:\n{}".format(tree.gold_tree, tree.to_string(self))
+                if fail:
+                    raise ValueError(error)
+                else:
+                    logger.error(error)
+                    remove.add(idx)
+                    continue
+
+            if tree.num_transitions() >= len(tree.word_queue) * 20:
+                # too many transitions
+                # x20 is somewhat empirically chosen based on certain
+                # treebanks having deep unary structures, especially early
+                # on when the model is fumbling around
+                if tree.gold_tree:
+                    error = "Went infinite on the following gold tree:\n{}\n\nFinal state:\n{}".format(tree.gold_tree, tree.to_string(self))
+                else:
+                    error = "Went infinite!:\nFinal state:\n{}".format(tree.to_string(self))
+                if fail:
+                    raise ValueError(error)
+                else:
+                    logger.error(error)
+                    remove.add(idx)
+                    continue
+
+            wq, c, nc, callback = transition.update_state(tree, self)
+
+            word_positions.append(wq)
+            constituents.append(c)
+            new_constituents.append(nc)
+            if callback:
+                # not `idx` in case something was removed
+                callbacks[callback].append(len(new_constituents)-1)
+
+        for key, idxs in callbacks.items():
+            data = [new_constituents[x] for x in idxs]
+            callback_constituents = key.build_constituents(self, data)
+            for idx, constituent in zip(idxs, callback_constituents):
+                new_constituents[idx] = constituent
+
+        state_batch = [tree for idx, tree in enumerate(state_batch) if idx not in remove]
+        transitions = [trans for idx, trans in enumerate(transitions) if idx not in remove]
+
+        if len(state_batch) == 0:
+            return state_batch
+
+        new_transitions = self.push_transitions([tree.transitions for tree in state_batch], transitions)
+        new_constituents = self.push_constituents(constituents, new_constituents)
+
+        state_batch = [state._replace(num_opens=state.num_opens + transition.delta_opens(),
+                                     word_position=word_position,
+                                     transitions=transition_stack,
+                                     constituents=constituents)
+                      for (state, transition, word_position, transition_stack, constituents)
+                      in zip(state_batch, transitions, word_positions, new_transitions, new_constituents)]
+
+        return state_batch
+
 class SimpleModel(BaseModel):
     """
     This model allows pushing and popping with no extra data
 
     This class is primarily used for testing various operations which
     don't need the NN's weights
 
@@ -402,15 +480,15 @@
 
     def initial_word_queues(self, tagged_word_lists):
         word_queues = []
         for tagged_words in tagged_word_lists:
             word_queue =  [None]
             word_queue += [tag_node for tag_node in tagged_words]
             word_queue.append(None)
-            if self.reverse_sentence():
+            if self.reverse_sentence:
                 word_queue.reverse()
             word_queues.append(word_queue)
         return word_queues
 
     def initial_transitions(self):
         return TreeStack(value=None, parent=None, length=1)
```

### Comparing `stanza-1.8.1/stanza/models/constituency/dynamic_oracle.py` & `stanza-1.8.2/stanza/models/constituency/dynamic_oracle.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/models/constituency/ensemble.py` & `stanza-1.8.2/stanza/models/constituency/ensemble.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,18 +27,19 @@
 import logging
 import os
 
 import torch
 
 from stanza.models.common import utils
 from stanza.models.common.foundation_cache import FoundationCache
-from stanza.models.constituency import parse_transitions
 from stanza.models.constituency import retagging
 from stanza.models.constituency import tree_reader
-from stanza.models.constituency.trainer import Trainer, run_dev_set, parse_text, parse_dir
+from stanza.models.constituency.state import MultiState
+from stanza.models.constituency.text_processing import parse_text, parse_dir
+from stanza.models.constituency.trainer import Trainer, run_dev_set
 from stanza.models.constituency.utils import add_predict_output_args, postprocess_predict_output_args, retag_trees
 from stanza.resources.common import DEFAULT_MODEL_DIR
 from stanza.server.parser_eval import EvaluateParser, ParseResult, ScoredTree
 from stanza.utils.default_paths import get_default_paths
 
 logger = logging.getLogger('stanza.constituency.trainer')
 
@@ -66,23 +67,24 @@
                 raise ValueError("Models %s and %s are incompatible: different transitions" % (filenames[0], filenames[model_idx]))
             if self.models[0].constituents != model.constituents:
                 raise ValueError("Models %s and %s are incompatible: different constituents" % (filenames[0], filenames[model_idx]))
             if self.models[0].root_labels != model.root_labels:
                 raise ValueError("Models %s and %s are incompatible: different root_labels" % (filenames[0], filenames[model_idx]))
             if self.models[0].uses_xpos() != model.uses_xpos():
                 raise ValueError("Models %s and %s are incompatible: different uses_xpos" % (filenames[0], filenames[model_idx]))
-            if self.models[0].reverse_sentence() != model.reverse_sentence():
+            if self.models[0].reverse_sentence != model.reverse_sentence:
                 raise ValueError("Models %s and %s are incompatible: different reverse_sentence" % (filenames[0], filenames[model_idx]))
 
-        self._reverse_sentence = self.models[0].reverse_sentence()
+        self._reverse_sentence = self.models[0].reverse_sentence
 
     def eval(self):
         for model in self.models:
             model.eval()
 
+    @property
     def reverse_sentence(self):
         return self._reverse_sentence
 
     def uses_xpos(self):
         return self.models[0].uses_xpos()
 
     def build_batch_from_tagged_words(self, batch_size, data_iterator):
@@ -97,14 +99,15 @@
             if sentence is None:
                 break
             state_batch.append(sentence)
 
         if len(state_batch) > 0:
             state_batch = [model.initial_state_from_words(state_batch) for model in self.models]
             state_batch = list(zip(*state_batch))
+            state_batch = [MultiState(states, None, None, 0.0) for states in state_batch]
         return state_batch
 
     def build_batch_from_trees(self, batch_size, data_iterator):
         """
         Read from the data_iterator batch_size trees and turn them into N lists of parsing states
         """
         state_batch = []
@@ -113,18 +116,19 @@
             if gold_tree is None:
                 break
             state_batch.append(gold_tree)
 
         if len(state_batch) > 0:
             state_batch = [model.initial_state_from_gold_trees(state_batch) for model in self.models]
             state_batch = list(zip(*state_batch))
+            state_batch = [MultiState(states, None, None, 0.0) for states in state_batch]
         return state_batch
 
     def predict(self, states, is_legal=True):
-        states = list(zip(*states))
+        states = list(zip(*[x.states for x in states]))
         predictions = [model.forward(state_batch) for model, state_batch in zip(self.models, states)]
         predictions = torch.stack(predictions)
         predictions = torch.sum(predictions, dim=0)
 
         model = self.models[0]
 
         # TODO: possibly refactor with lstm_model.predict
@@ -144,14 +148,23 @@
                             break
                     else: # yeah, else on a for loop, deal with it
                         pred_trans[idx] = None
                         scores[idx] = None
 
         return predictions, pred_trans, scores.squeeze(1)
 
+    def bulk_apply(self, state_batch, transitions, fail=False):
+        new_states = []
+
+        states = list(zip(*[x.states for x in state_batch]))
+        states = [x.bulk_apply(y, transitions, fail=fail) for x, y in zip(self.models, states)]
+        states = list(zip(*states))
+        state_batch = [x._replace(states=y) for x, y in zip(state_batch, states)]
+        return state_batch
+
     def parse_sentences(self, data_iterator, build_batch_fn, batch_size, transition_choice, keep_state=False, keep_constituents=False, keep_scores=False):
         """
         Repeat transitions to build a list of trees from the input batches.
 
         The data_iterator should be anything which returns the data for a parse task via next()
         build_batch_fn is a function that turns that data into State objects
         This will be called to generate batches of size batch_size until the data is exhausted
@@ -174,39 +187,33 @@
         batch_indices = list(range(len(state_batch)))
         horizon_iterator = iter([])
 
         if keep_constituents:
             constituents = defaultdict(list)
 
         while len(state_batch) > 0:
-            #print(batch_indices)
             pred_scores, transitions, scores = transition_choice(state_batch)
             # num models lists of batch size states
-            state_batch = list(zip(*state_batch))
-            state_batch = [parse_transitions.bulk_apply(model, states, transitions) for model, states in zip(self.models, state_batch)]
+            state_batch = self.bulk_apply(state_batch, transitions)
 
             remove = set()
-            for idx, state in enumerate(state_batch[0]):
-                if state.finished(self.models[0]):
-                    predicted_tree = state.get_tree(self.models[0])
-                    if self.reverse_sentence():
+            for idx, states in enumerate(state_batch):
+                if states.finished(self):
+                    predicted_tree = states.get_tree(self)
+                    if self.reverse_sentence:
                         predicted_tree = predicted_tree.reverse()
-                    gold_tree = state.gold_tree
+                    gold_tree = states.gold_tree
                     # TODO: could easily store the score here
                     # not sure what it means to store the state,
                     # since each model is tracking its own state
                     treebank.append(ParseResult(gold_tree, [ScoredTree(predicted_tree, None)], None, None))
                     treebank_indices.append(batch_indices[idx])
                     remove.add(idx)
 
-            # batch size lists of num models tuples
-            state_batch = list(zip(*state_batch))
-
             if len(remove) > 0:
-                # remove a whole tuple of states at once
                 state_batch = [state for idx, state in enumerate(state_batch) if idx not in remove]
                 batch_indices = [batch_idx for idx, batch_idx in enumerate(batch_indices) if idx not in remove]
 
             for _ in range(batch_size - len(state_batch)):
                 horizon_state = next(horizon_iterator, None)
                 if not horizon_state:
                     horizon_batch = build_batch_fn(batch_size, data_iterator)
```

### Comparing `stanza-1.8.1/stanza/models/constituency/evaluate_treebanks.py` & `stanza-1.8.2/stanza/models/constituency/evaluate_treebanks.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/models/constituency/in_order_oracle.py` & `stanza-1.8.2/stanza/models/constituency/in_order_oracle.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/models/constituency/label_attention.py` & `stanza-1.8.2/stanza/models/constituency/label_attention.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/models/constituency/lstm_model.py` & `stanza-1.8.2/stanza/models/constituency/lstm_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,16 +34,15 @@
 
 import torch
 import torch.nn as nn
 from torch.nn.utils.rnn import pack_padded_sequence
 
 from stanza.models.common.bert_embedding import extract_bert_embeddings
 from stanza.models.common.maxout_linear import MaxoutLinear
-from stanza.models.common.peft_config import build_peft_wrapper
-from stanza.models.common.utils import unsort
+from stanza.models.common.utils import attach_bert_model, unsort
 from stanza.models.common.vocab import PAD_ID, UNK_ID
 from stanza.models.constituency.base_model import BaseModel
 from stanza.models.constituency.label_attention import LabelAttentionModule
 from stanza.models.constituency.lstm_tree_stack import LSTMTreeStack
 from stanza.models.constituency.parse_transitions import TransitionScheme
 from stanza.models.constituency.parse_tree import Tree
 from stanza.models.constituency.partitioned_transformer import PartitionedTransformerModule
@@ -208,15 +207,15 @@
     ATTN                  = 6
     TREE_LSTM_CX          = 7
     UNTIED_MAX            = 8
     KEY                   = 9
     UNTIED_KEY            = 10
 
 class LSTMModel(BaseModel, nn.Module):
-    def __init__(self, pretrain, forward_charlm, backward_charlm, bert_model, bert_tokenizer, force_bert_saved, transitions, constituents, tags, words, rare_words, root_labels, constituent_opens, unary_limit, args):
+    def __init__(self, pretrain, forward_charlm, backward_charlm, bert_model, bert_tokenizer, force_bert_saved, peft_name, transitions, constituents, tags, words, rare_words, root_labels, constituent_opens, unary_limit, args):
         """
         pretrain: a Pretrain object
         transitions: a list of all possible transitions which will be
           used to build trees
         constituents: a list of all possible constituents in the treebank
         tags: a list of all possible tags in the treebank
         words: a list of all known words, used for a delta word embedding.
@@ -348,29 +347,18 @@
         if self.sentence_boundary_vectors is not SentenceBoundary.NONE:
             self.register_parameter('word_start_embedding', torch.nn.Parameter(0.2 * torch.randn(self.word_input_size, requires_grad=True)))
             self.register_parameter('word_end_embedding', torch.nn.Parameter(0.2 * torch.randn(self.word_input_size, requires_grad=True)))
 
         # we set up the bert AFTER building word_start and word_end
         # so that we can use the charlm endpoint values rather than
         # try to train our own
-        self.force_bert_saved = force_bert_saved
-        if self.args.get('use_peft', False):
-            bert_model = build_peft_wrapper(bert_model, self.args, tlogger)
-            # we use a peft-specific pathway for saving peft weights
-            self.add_unsaved_module('bert_model', bert_model)
-            self.bert_model.train()
-        elif self.args['bert_finetune'] or self.args['stage1_bert_finetune'] or force_bert_saved:
-            self.bert_model = bert_model
-        elif bert_model is not None:
-            self.add_unsaved_module('bert_model', bert_model)
-            for _, parameter in bert_model.named_parameters():
-                parameter.requires_grad = False
-        else:
-            self.bert_model = None
-        self.add_unsaved_module('bert_tokenizer', bert_tokenizer)
+        self.force_bert_saved = force_bert_saved or self.args['bert_finetune'] or self.args['stage1_bert_finetune']
+        attach_bert_model(self, bert_model, bert_tokenizer, self.args.get('use_peft', False), self.force_bert_saved)
+        self.peft_name = peft_name
+
         if bert_model is not None:
             if bert_tokenizer is None:
                 raise ValueError("Cannot have a bert model without a tokenizer")
             self.bert_dim = self.bert_model.config.hidden_size
             if args['bert_hidden_layers']:
                 # The average will be offset by 1/N so that the default zeros
                 # repressents an average of the N layers
@@ -572,17 +560,14 @@
 
         # matrix for predicting the next transition using word/constituent/transition queues
         # word size + constituency size + transition size
         # TODO: .get() is only necessary until all models rebuilt with this param
         self.maxout_k = self.args.get('maxout_k', 0)
         self.output_layers = self.build_output_layers(self.args['num_output_layers'], len(transitions), self.maxout_k)
 
-    def reverse_sentence(self):
-        return self._reverse_sentence
-
     @staticmethod
     def uses_lattn(args):
         return args.get('use_lattn', True) and args.get('lattn_d_proj', 0) > 0 and args.get('lattn_d_l', 0) > 0
 
     @staticmethod
     def uses_pattn(args):
         return args['pattn_num_heads'] > 0 and args['pattn_num_layers'] > 0
@@ -615,15 +600,18 @@
                 # -1 so that it can be converted easier to a different parameter
                 copy_size = min(other_parameter.data.shape[-1], my_parameter.data.shape[-1])
                 #new_values = my_parameter.data.clone().detach()
                 new_values = torch.zeros_like(my_parameter.data)
                 new_values[..., :copy_size] = other_parameter.data[..., :copy_size]
                 my_parameter.data.copy_(new_values)
             else:
-                self.get_parameter(name).data.copy_(other_parameter.data)
+                try:
+                    self.get_parameter(name).data.copy_(other_parameter.data)
+                except AttributeError as e:
+                    raise AttributeError("Could not process %s" % name) from e
 
     def build_output_layers(self, num_output_layers, final_layer_size, maxout_k):
         """
         Build a ModuleList of Linear transformations for the given num_output_layers
 
         The final layer size can be specified.
         Initial layer size is the combination of word, constituent, and transition vectors
@@ -681,20 +669,20 @@
             if param.requires_grad and name not in skip:
                 zeros = torch.sum(param.abs() < 0.000001).item()
                 norm = "%.6g" % torch.norm(param).item()
                 lines.append(format_string % (name, norm, zeros, param.nelement()))
         return lines
 
     def log_norms(self):
-        lines = ["NORMS FOR MODEL PARAMTERS"]
+        lines = ["NORMS FOR MODEL PARAMETERS"]
         lines.extend(self.get_norms())
         logger.info("\n".join(lines))
 
     def log_shapes(self):
-        lines = ["NORMS FOR MODEL PARAMTERS"]
+        lines = ["NORMS FOR MODEL PARAMETERS"]
         for name, param in self.named_parameters():
             if param.requires_grad:
                 lines.append("{} {}".format(name, param.shape))
         logger.info("\n".join(lines))
 
     def initial_word_queues(self, tagged_word_lists):
         """
@@ -760,15 +748,16 @@
         if self.bert_model is not None:
             # BERT embedding extraction
             # result will be len+2 for each sentence
             # we will take 1:-1 if we don't care about the endpoints
             bert_embeddings = extract_bert_embeddings(self.args['bert_model'], self.bert_tokenizer, self.bert_model, all_word_labels, device,
                                                       keep_endpoints=self.sentence_boundary_vectors is not SentenceBoundary.NONE,
                                                       num_layers=self.bert_layer_mix.in_features if self.bert_layer_mix is not None else None,
-                                                      detach=not self.args['bert_finetune'] and not self.args['stage1_bert_finetune'])
+                                                      detach=not self.args['bert_finetune'] and not self.args['stage1_bert_finetune'],
+                                                      peft_name=self.peft_name)
             if self.bert_layer_mix is not None:
                 # add the average so that the default behavior is to
                 # take an average of the N layers, and anything else
                 # other than that needs to be learned
                 bert_embeddings = [self.bert_layer_mix(feature).squeeze(2) + feature.sum(axis=2) / self.bert_layer_mix.in_features for feature in bert_embeddings]
 
             all_word_inputs = [torch.cat((x, y), axis=1) for x, y in zip(all_word_inputs, bert_embeddings)]
@@ -814,15 +803,15 @@
                 word_queue.append(WordNode(None, sentence_output[len(tagged_words)+1, :]))
             else:
                 word_queue =  [WordNode(None, self.word_zeros)]
                 word_queue += [WordNode(tag_node, sentence_output[idx, :])
                                    for idx, tag_node in enumerate(tagged_words)]
                 word_queue.append(WordNode(None, self.word_zeros))
 
-            if self.reverse_sentence():
+            if self.reverse_sentence:
                 word_queue = list(reversed(word_queue))
             word_queues.append(word_queue)
 
         return word_queues
 
     def initial_transitions(self):
         """
@@ -1030,17 +1019,16 @@
 
     def get_top_constituent(self, constituents):
         """
         Extract only the top constituent from a state's constituent
         sequence, even though it has multiple addition pieces of
         information
         """
-        # TreeStack value -> LSTMTreeStack value -> Constituent value
-        constituent_node = constituents.value.value
-        return constituent_node.value
+        # TreeStack value -> LSTMTreeStack value -> Constituent value -> constituent
+        return constituents.value.value.value
 
     def push_transitions(self, transition_stacks, transitions):
         """
         Push all of the given transitions on to the stack as a batch operations.
 
         Significantly faster than doing one transition at a time.
         """
@@ -1050,16 +1038,16 @@
 
     def get_top_transition(self, transitions):
         """
         Extract only the top transition from a state's transition
         sequence, even though it has multiple addition pieces of
         information
         """
-        transition_node = transitions.value
-        return transition_node.value
+        # TreeStack value -> LSTMTreeStack value -> transition
+        return transitions.value.value
 
     def forward(self, states):
         """
         Return logits for a prediction of what transition to make next
 
         We've basically done all the work analyzing the state as
         part of applying the transitions, so this method is very simple
```

### Comparing `stanza-1.8.1/stanza/models/constituency/lstm_tree_stack.py` & `stanza-1.8.2/stanza/models/constituency/lstm_tree_stack.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/models/constituency/parse_transitions.py` & `stanza-1.8.2/stanza/models/constituency/parse_transitions.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 Defines a series of transitions (open a constituent, close a constituent, etc
 
 Also defines a State which holds the various data needed to build
 a parse tree out of tagged words.
 """
 
 from abc import ABC, abstractmethod
-from collections import defaultdict, namedtuple
+from collections import defaultdict
 from enum import Enum
 import functools
 import logging
 
 from stanza.models.constituency.parse_tree import Tree
 
 logger = logging.getLogger('stanza')
@@ -46,103 +46,14 @@
     # score: 0.8186
     IN_ORDER_COMPOUND  = 5
 
     # in order, with CompoundUnary on both preterminals and internal nodes
     # score: 0.8166
     IN_ORDER_UNARY     = 6
 
-class State(namedtuple('State', ['word_queue', 'transitions', 'constituents', 'gold_tree', 'gold_sequence',
-                                 'sentence_length', 'num_opens', 'word_position', 'score'])):
-    """
-    Represents a partially completed transition parse
-
-    Includes stack/buffers for unused words, already executed transitions, and partially build constituents
-    At training time, also keeps track of the gold data we are reparsing
-
-    num_opens is useful for tracking
-       1) if the parser is in a stuck state where it is making infinite opens
-       2) if a close transition is impossible because there are no previous opens
-
-    sentence_length tracks how long the sentence is so we abort if we go infinite
-
-    non-stack information such as sentence_length and num_opens
-    will be copied from the original_state if possible, with the
-    exact arguments overriding the values in the original_state
-
-    gold_tree: the original tree, if made from a gold tree.  might be None
-    gold_sequence: the original transition sequence, if available
-    Note that at runtime, gold values will not be available
-
-    word_position tracks where in the word queue we are.  cheaper than
-      manipulating the list itself.  this can be handled differently
-      from transitions and constituents as it is processed once
-      at the start of parsing
-
-    The word_queue should have both a start and an end word.
-    Those can be None in the case of the endpoints if they are unused.
-    """
-    def empty_word_queue(self):
-        # the first element of each stack is a sentinel with no value
-        # and no parent
-        return self.word_position == self.sentence_length
-
-    def empty_transitions(self):
-        # the first element of each stack is a sentinel with no value
-        # and no parent
-        return self.transitions.parent is None
-
-    def has_one_constituent(self):
-        # a length of 1 represents no constituents
-        return len(self.constituents) == 2
-
-    def num_constituents(self):
-        return len(self.constituents) - 1
-
-    def num_transitions(self):
-        # -1 for the sentinel value
-        return len(self.transitions) - 1
-
-    def get_word(self, pos):
-        # +1 to handle the initial sentinel value
-        # (which you can actually get with pos=-1)
-        return self.word_queue[pos+1]
-
-    def finished(self, model):
-        return self.empty_word_queue() and self.has_one_constituent() and model.get_top_constituent(self.constituents).label in model.get_root_labels()
-
-    def get_tree(self, model):
-        return model.get_top_constituent(self.constituents)
-
-    def all_transitions(self, model):
-        # TODO: rewrite this to be nicer / faster?  or just refactor?
-        all_transitions = []
-        transitions = self.transitions
-        while transitions.parent is not None:
-            all_transitions.append(model.get_top_transition(transitions))
-            transitions = transitions.parent
-        return list(reversed(all_transitions))
-
-    def all_constituents(self, model):
-        # TODO: rewrite this to be nicer / faster?
-        all_constituents = []
-        constituents = self.constituents
-        while constituents.parent is not None:
-            all_constituents.append(model.get_top_constituent(constituents))
-            constituents = constituents.parent
-        return list(reversed(all_constituents))
-
-    def all_words(self, model):
-        return [model.get_word(x) for x in self.word_queue]
-
-    def to_string(self, model):
-        return "State(\n  buffer:%s\n  transitions:%s\n  constituents:%s\n  word_position:%d num_opens:%d)" % (str(self.all_words(model)), str(self.all_transitions(model)), str(self.all_constituents(model)), self.word_position, self.num_opens)
-
-    def __str__(self):
-        return "State(\n  buffer:%s\n  transitions:%s\n  constituents:%s)" % (str(self.word_queue), str(self.transitions), str(self.constituents))
-
 @functools.total_ordering
 class Transition(ABC):
     """
     model is passed in as a dependency injection
     for example, an LSTM model can update hidden & output vectors when transitioning
     """
     @abstractmethod
@@ -170,15 +81,15 @@
     def apply(self, state, model):
         """
         return a new State transformed via this transition
 
         convenience method to call bulk_apply, which is significantly
         faster than single operations for an NN based model
         """
-        update = bulk_apply(model, [state], [self])
+        update = model.bulk_apply([state], [self])
         return update[0]
 
     @abstractmethod
     def is_legal(self, state, model):
         """
         assess whether or not this transition is legal in this state
 
@@ -670,82 +581,7 @@
         if trans not in train_transitions:
             for component in trans.components():
                 if component not in train_transitions:
                     raise RuntimeError("Found transition {} in the {} set which don't exist in the train set".format(trans, treebank_name))
             unknown_transitions.add(trans)
     if len(unknown_transitions) > 0:
         logger.warning("Found transitions where the components are all valid transitions, but the complete transition is unknown: %s", sorted(unknown_transitions))
-
-def bulk_apply(model, state_batch, transitions, fail=False):
-    """
-    Apply the given list of Transitions to the given list of States, using the model as a reference
-
-    model: SimpleModel, LSTMModel, or any other form of model
-    state_batch: list of States
-    transitions: list of transitions, one per state
-    fail: throw an exception on a failed transition, as opposed to skipping the tree
-    """
-    remove = set()
-
-    word_positions = []
-    constituents = []
-    new_constituents = []
-    callbacks = defaultdict(list)
-
-    for idx, (tree, transition) in enumerate(zip(state_batch, transitions)):
-        if not transition:
-            error = "Got stuck and couldn't find a legal transition on the following gold tree:\n{}\n\nFinal state:\n{}".format(tree.gold_tree, tree.to_string(model))
-            if fail:
-                raise ValueError(error)
-            else:
-                logger.error(error)
-                remove.add(idx)
-                continue
-
-        if tree.num_transitions() >= len(tree.word_queue) * 20:
-            # too many transitions
-            # x20 is somewhat empirically chosen based on certain
-            # treebanks having deep unary structures, especially early
-            # on when the model is fumbling around
-            if tree.gold_tree:
-                error = "Went infinite on the following gold tree:\n{}\n\nFinal state:\n{}".format(tree.gold_tree, tree.to_string(model))
-            else:
-                error = "Went infinite!:\nFinal state:\n{}".format(tree.to_string(model))
-            if fail:
-                raise ValueError(error)
-            else:
-                logger.error(error)
-                remove.add(idx)
-                continue
-
-        wq, c, nc, callback = transition.update_state(tree, model)
-
-        word_positions.append(wq)
-        constituents.append(c)
-        new_constituents.append(nc)
-        if callback:
-            # not `idx` in case something was removed
-            callbacks[callback].append(len(new_constituents)-1)
-
-    for key, idxs in callbacks.items():
-        data = [new_constituents[x] for x in idxs]
-        callback_constituents = key.build_constituents(model, data)
-        for idx, constituent in zip(idxs, callback_constituents):
-            new_constituents[idx] = constituent
-
-    state_batch = [tree for idx, tree in enumerate(state_batch) if idx not in remove]
-    transitions = [trans for idx, trans in enumerate(transitions) if idx not in remove]
-
-    if len(state_batch) == 0:
-        return state_batch
-
-    new_transitions = model.push_transitions([tree.transitions for tree in state_batch], transitions)
-    new_constituents = model.push_constituents(constituents, new_constituents)
-
-    state_batch = [state._replace(num_opens=state.num_opens + transition.delta_opens(),
-                                 word_position=word_position,
-                                 transitions=transition_stack,
-                                 constituents=constituents)
-                  for (state, transition, word_position, transition_stack, constituents)
-                  in zip(state_batch, transitions, word_positions, new_transitions, new_constituents)]
-
-    return state_batch
```

### Comparing `stanza-1.8.1/stanza/models/constituency/parse_tree.py` & `stanza-1.8.2/stanza/models/constituency/parse_tree.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 Tree datastructure
 """
 
 from collections import deque, Counter
+import copy
 from enum import Enum
 from io import StringIO
 import itertools
 import re
 import warnings
 
 from stanza.models.common.stanza_object import StanzaObject
@@ -14,15 +15,19 @@
 # useful more for the "is" functionality than the time savings
 CLOSE_PAREN = ')'
 SPACE_SEPARATOR = ' '
 OPEN_PAREN = '('
 
 EMPTY_CHILDREN = ()
 
-CONSTITUENT_SPLIT = re.compile("[-=#]")
+# used to split off the functional tags from various treebanks
+# for example, the Icelandic treebank (which we don't currently
+# incorporate) uses * to distinguish 'ADJP', 'ADJP*OC' but we treat
+# those as the same
+CONSTITUENT_SPLIT = re.compile("[-=#*]")
 
 # These words occur in the VLSP dataset.
 # The documentation claims there might be *O*, although those don't
 # seem to exist in practice
 WORDS_TO_PRUNE = ('*E*', '*T*', '*O*')
 
 class TreePrintMethod(Enum):
@@ -304,14 +309,16 @@
             child.visit_preorder(internal, preterminal, leaf)
 
     @staticmethod
     def get_unique_constituent_labels(trees):
         """
         Walks over all of the trees and gets all of the unique constituent names from the trees
         """
+        if isinstance(trees, Tree):
+            trees = [trees]
         constituents = Tree.get_constituent_counts(trees)
         return sorted(set(constituents.keys()))
 
     @staticmethod
     def get_constituent_counts(trees):
         """
         Walks over all of the trees and gets the count of the unique constituent names from the trees
@@ -482,14 +489,42 @@
 
         new_tree = recursive_replace_words(self)
         if any(True for _ in word_iterator):
             raise ValueError("Too many words for the given tree")
         return new_tree
 
 
+    def replace_tags(self, tags):
+        if self.is_leaf():
+            raise ValueError("Must call replace_tags with non-leaf")
+
+        tag_iterator = iter(tags)
+
+        new_tree = copy.deepcopy(self)
+        queue = deque()
+        queue.append(new_tree)
+        while len(queue) > 0:
+            next_node = queue.pop()
+            if next_node.is_preterminal():
+                try:
+                    label = next(tag_iterator)
+                except StopIteration:
+                    raise ValueError("Not enough tags in sentence for given tree")
+                next_node.label = label
+            elif next_node.is_leaf():
+                raise ValueError("Got a badly structured tree: {}".format(self))
+            else:
+                queue.extend(reversed(next_node.children))
+
+        if any(True for _ in tag_iterator):
+            raise ValueError("Too many tags for the given tree")
+
+        return new_tree
+
+
     def prune_none(self):
         """
         Return a copy of the tree, eliminating all nodes which are in one of two categories:
             they are a preterminal -NONE-, such as appears in PTB
               *E* shows up in a VLSP dataset
             they have been pruned to 0 children by the recursive call
         """
```

### Comparing `stanza-1.8.1/stanza/models/constituency/partitioned_transformer.py` & `stanza-1.8.2/stanza/models/constituency/partitioned_transformer.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/models/constituency/positional_encoding.py` & `stanza-1.8.2/stanza/models/constituency/positional_encoding.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/models/constituency/retagging.py` & `stanza-1.8.2/stanza/models/constituency/retagging.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 
 tlogger = logging.getLogger('stanza.constituency.trainer')
 
 # xpos tagger doesn't produce PP tag on the turin treebank,
 # so instead we use upos to avoid unknown tag errors
 RETAG_METHOD = {
     "da": "upos",   # the DDT has no xpos tags anyway
+    "de": "upos",   # DE GSD is also missing a few punctuation tags
     "es": "upos",   # AnCora has half-finished xpos tags
     "id": "upos",   # GSD is missing a few punctuation tags - fixed in 2.12, though
     "it": "upos",
     "pt": "upos",   # default PT model has no xpos either
     "vi": "xpos",   # the new version of UD can be merged with xpos from VLSP22
 }
```

### Comparing `stanza-1.8.1/stanza/models/constituency/score_converted_dependencies.py` & `stanza-1.8.2/stanza/models/constituency/score_converted_dependencies.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/models/constituency/top_down_oracle.py` & `stanza-1.8.2/stanza/models/constituency/top_down_oracle.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/models/constituency/trainer.py` & `stanza-1.8.2/stanza/models/constituency/trainer.py`

 * *Files 16% similar despite different names*

```diff
@@ -20,27 +20,26 @@
 import sys
 
 import torch
 from torch import nn
 
 from stanza.models.common import pretrain
 from stanza.models.common import utils
-from stanza.models.common.foundation_cache import load_bert, load_charlm, load_pretrain, FoundationCache
+from stanza.models.common.foundation_cache import load_bert, load_bert_with_peft, load_charlm, load_pretrain, FoundationCache, NoTransformerFoundationCache
 from stanza.models.common.large_margin_loss import LargeMarginInSoftmaxLoss
+from stanza.models.common.peft_config import build_peft_wrapper, load_peft_wrapper
 from stanza.models.constituency import parse_transitions
-from stanza.models.constituency import parse_tree
 from stanza.models.constituency import transition_sequence
 from stanza.models.constituency import tree_reader
-from stanza.models.constituency.base_model import SimpleModel, UNARY_LIMIT
 from stanza.models.constituency.in_order_oracle import InOrderOracle
 from stanza.models.constituency.lstm_model import LSTMModel, StackHistory
 from stanza.models.constituency.parse_transitions import TransitionScheme
 from stanza.models.constituency.parse_tree import Tree
 from stanza.models.constituency.top_down_oracle import TopDownOracle
-from stanza.models.constituency.utils import retag_tags, retag_trees, build_optimizer, build_scheduler
+from stanza.models.constituency.utils import retag_trees, build_optimizer, build_scheduler, verify_transitions, get_open_nodes, check_constituents, check_root_labels, remove_duplicate_trees, remove_singleton_trees
 from stanza.models.constituency.utils import DEFAULT_LEARNING_EPS, DEFAULT_LEARNING_RATES, DEFAULT_LEARNING_RHO, DEFAULT_WEIGHT_DECAY
 from stanza.server.parser_eval import EvaluateParser, ParseResult
 from stanza.utils.get_tqdm import get_tqdm
 # TODO: could put find_wordvec_pretrain, choose_charlm, etc in a more central place if it becomes widely used
 from stanza.utils.training.common import find_wordvec_pretrain, choose_charlm, find_charlm_file
 from stanza.resources.default_packages import default_charlms, default_pretrains
 
@@ -77,21 +76,45 @@
             'batches_trained': self.batches_trained,
             'best_f1': self.best_f1,
             'best_epoch': self.best_epoch,
         }
         if self.model.args.get('use_peft', False):
             # Hide import so that peft dependency is optional
             from peft import get_peft_model_state_dict
-            checkpoint["bert_lora"] = get_peft_model_state_dict(self.model.bert_model)
+            checkpoint["bert_lora"] = get_peft_model_state_dict(self.model.bert_model, adapter_name=self.model.peft_name)
         if save_optimizer and self.optimizer is not None:
             checkpoint['optimizer_state_dict'] = self.optimizer.state_dict()
             checkpoint['scheduler_state_dict'] = self.scheduler.state_dict()
         torch.save(checkpoint, filename, _use_new_zipfile_serialization=False)
         logger.info("Model saved to %s", filename)
 
+    def log_norms(self):
+        self.model.log_norms()
+
+    def log_shapes(self):
+        self.model.log_shapes()
+
+    @property
+    def transitions(self):
+        return self.model.transitions
+
+    @property
+    def root_labels(self):
+        return self.model.root_labels
+
+    @property
+    def device(self):
+        return next(self.model.parameters()).device
+
+    def train(self):
+        return self.model.train()
+
+    def eval(self):
+        return self.model.eval()
+
     @staticmethod
     def find_and_load_pretrain(saved_args, foundation_cache):
         if 'wordvec_pretrain_file' not in saved_args:
             return None
         if os.path.exists(saved_args['wordvec_pretrain_file']):
             return load_pretrain(saved_args['wordvec_pretrain_file'], foundation_cache)
         logger.info("Unable to find pretrain in %s  Will try to load from the default resources instead", saved_args['wordvec_pretrain_file'])
@@ -108,26 +131,27 @@
             language = saved_args['lang']
             dataset = saved_args['shorthand'].split("_")[1]
             charlm = choose_charlm(language, dataset, "default", default_charlms, {})
             charlm_file = find_charlm_file(direction, language, charlm)
             return load_charlm(charlm_file, foundation_cache)
 
     @staticmethod
-    def model_from_params(params, args, foundation_cache=None):
+    def model_from_params(params, peft_params, args, foundation_cache=None, peft_name=None):
         """
         Build a new model just from the saved params and some extra args
 
         Refactoring allows other processors to include a constituency parser as a module
         """
         saved_args = dict(params['config'])
         # some parameters which change the structure of a model have
         # to be ignored, or the model will not function when it is
         # reloaded from disk
         if args is None: args = {}
         update_args = copy.deepcopy(args)
+        # TODO: pop all the peft args as well
         update_args.pop("bert_hidden_layers", None)
         update_args.pop("constituency_composition", None)
         update_args.pop("constituent_stack", None)
         update_args.pop("num_tree_lstm_layers", None)
         update_args.pop("transition_scheme", None)
         update_args.pop("transition_stack", None)
         update_args.pop("maxout_k", None)
@@ -149,15 +173,24 @@
             saved_args["bert_finetune"] = False
         if saved_args.get("stage1_bert_finetune", None) is None:
             saved_args["stage1_bert_finetune"] = False
 
         model_type = params['model_type']
         if model_type == 'LSTM':
             pt = Trainer.find_and_load_pretrain(saved_args, foundation_cache)
-            if saved_args['bert_finetune'] or saved_args['stage1_bert_finetune'] or any(x.startswith("bert_model.") for x in params['model'].keys()):
+            if saved_args.get('use_peft', False):
+                # if loading a peft model, we first load the base transformer
+                # then we load the weights using the saved weights in the file
+                if peft_name is None:
+                    bert_model, bert_tokenizer, peft_name = load_bert_with_peft(saved_args.get('bert_model', None), "constituency", foundation_cache)
+                else:
+                    bert_model, bert_tokenizer = load_bert(saved_args.get('bert_model', None), foundation_cache)
+                bert_model = load_peft_wrapper(bert_model, peft_params, saved_args, logger, peft_name)
+                bert_saved = True
+            elif saved_args['bert_finetune'] or saved_args['stage1_bert_finetune'] or any(x.startswith("bert_model.") for x in params['model'].keys()):
                 # if bert_finetune is True, don't use the cached model!
                 # otherwise, other uses of the cached model will be ruined
                 bert_model, bert_tokenizer = load_bert(saved_args.get('bert_model', None))
                 bert_saved = True
             else:
                 bert_model, bert_tokenizer = load_bert(saved_args.get('bert_model', None), foundation_cache)
                 bert_saved = False
@@ -165,14 +198,15 @@
             backward_charlm = Trainer.find_and_load_charlm(saved_args["charlm_backward_file"], "backward", saved_args, foundation_cache)
             model = LSTMModel(pretrain=pt,
                               forward_charlm=forward_charlm,
                               backward_charlm=backward_charlm,
                               bert_model=bert_model,
                               bert_tokenizer=bert_tokenizer,
                               force_bert_saved=bert_saved,
+                              peft_name=peft_name,
                               transitions=params['transitions'],
                               constituents=params['constituents'],
                               tags=params['tags'],
                               words=params['words'],
                               rare_words=params['rare_words'],
                               root_labels=params['root_labels'],
                               constituent_opens=params['constituent_opens'],
@@ -183,15 +217,15 @@
         model.load_state_dict(params['model'], strict=False)
         # model will stay on CPU if device==None
         # can be moved elsewhere later, of course
         model = model.to(args.get('device', None))
         return model
 
     @staticmethod
-    def load(filename, args=None, load_optimizer=False, foundation_cache=None):
+    def load(filename, args=None, load_optimizer=False, foundation_cache=None, peft_name=None):
         """
         Load back a model and possibly its optimizer.
         """
         if not os.path.exists(filename):
             if args.get('save_dir', None) is None:
                 raise FileNotFoundError("Cannot find model in {} and args['save_dir'] is None".format(filename))
             elif os.path.exists(os.path.join(args['save_dir'], filename)):
@@ -202,19 +236,15 @@
             checkpoint = torch.load(filename, lambda storage, loc: storage)
         except BaseException:
             logger.exception("Cannot load model from %s", filename)
             raise
         logger.debug("Loaded model from %s", filename)
 
         params = checkpoint['params']
-        model = Trainer.model_from_params(params, args, foundation_cache)
-        if model.args.get('use_peft', False):
-            # hide import so that the peft dependency is optional
-            from peft import set_peft_model_state_dict
-            set_peft_model_state_dict(model.bert_model, checkpoint['bert_lora'])
+        model = Trainer.model_from_params(params, checkpoint.get('bert_lora', None), args, foundation_cache, peft_name)
 
         epochs_trained = checkpoint['epochs_trained']
         batches_trained = checkpoint.get('batches_trained', 0)
         best_f1 = checkpoint['best_f1']
         best_epoch = checkpoint['best_epoch']
 
         if load_optimizer:
@@ -224,15 +254,18 @@
             # to match the optimizer we build with the one that was
             # used at training time
             build_simple_adadelta = params['config']['multistage'] and epochs_trained < params['config']['epochs'] // 2
             logger.debug("Model loaded was built with multistage %s  epochs_trained %d out of total epochs %d  Building initial Adadelta optimizer: %s", params['config']['multistage'], epochs_trained, params['config']['epochs'], build_simple_adadelta)
             optimizer = build_optimizer(model.args, model, build_simple_adadelta)
 
             if checkpoint.get('optimizer_state_dict', None) is not None:
-                optimizer.load_state_dict(checkpoint['optimizer_state_dict'])
+                try:
+                    optimizer.load_state_dict(checkpoint['optimizer_state_dict'])
+                except ValueError as e:
+                    raise ValueError("Failed to load optimizer from %s" % filename) from e
             else:
                 tlogger.info("Attempted to load optimizer to resume training, but optimizer not saved.  Creating new optimizer")
 
             scheduler = build_scheduler(model.args, optimizer, first_optimizer=build_simple_adadelta)
             if 'scheduler_state_dict' in checkpoint:
                 scheduler.load_state_dict(checkpoint['scheduler_state_dict'])
         else:
@@ -242,141 +275,14 @@
         logger.debug("-- MODEL CONFIG --")
         for k in model.args.keys():
             logger.debug("  --%s: %s", k, model.args[k])
 
         return Trainer(model=model, optimizer=optimizer, scheduler=scheduler, epochs_trained=epochs_trained, batches_trained=batches_trained, best_f1=best_f1, best_epoch=best_epoch)
 
 
-def load_pretrain_or_wordvec(args):
-    """
-    Loads a pretrain based on the paths in the arguments
-
-    TODO: put this functionality in the foundation_cache?
-    or maybe do this conversion before trying to load the pretrain?
-    currently this function is not used anywhere
-    """
-    pretrain_file = pretrain.find_pretrain_file(args['wordvec_pretrain_file'], args['save_dir'], args['shorthand'], args['lang'])
-    if os.path.exists(pretrain_file):
-        vec_file = None
-    else:
-        vec_file = args['wordvec_file'] if args['wordvec_file'] else utils.get_wordvec_file(args['wordvec_dir'], args['shorthand'])
-    pt = pretrain.Pretrain(pretrain_file, vec_file, args['pretrain_max_vocab'])
-    return pt
-
-def verify_transitions(trees, sequences, transition_scheme, unary_limit, reverse, name, root_labels):
-    """
-    Given a list of trees and their transition sequences, verify that the sequences rebuild the trees
-    """
-    model = SimpleModel(transition_scheme, unary_limit, reverse, root_labels)
-    tlogger.info("Verifying the transition sequences for %d trees", len(trees))
-
-    data = zip(trees, sequences)
-    if tlogger.getEffectiveLevel() <= logging.INFO:
-        data = tqdm(zip(trees, sequences), total=len(trees))
-
-    for tree_idx, (tree, sequence) in enumerate(data):
-        # TODO: make the SimpleModel have a parse operation?
-        state = model.initial_state_from_gold_trees([tree])[0]
-        for idx, trans in enumerate(sequence):
-            if not trans.is_legal(state, model):
-                raise RuntimeError("Tree {} of {} failed: transition {}:{} was not legal in a transition sequence:\nOriginal tree: {}\nTransitions: {}".format(tree_idx, name, idx, trans, tree, sequence))
-            state = trans.apply(state, model)
-        result = model.get_top_constituent(state.constituents)
-        if reverse:
-            result = result.reverse()
-        if tree != result:
-            raise RuntimeError("Tree {} of {} failed: transition sequence did not match for a tree!\nOriginal tree:{}\nTransitions: {}\nResult tree:{}".format(tree_idx, name, tree, sequence, result))
-
-def load_model_parse_text(args, model_file, retag_pipeline):
-    """
-    Load a model, then parse text and write it to stdout or args['predict_file']
-    """
-    foundation_cache = retag_pipeline[0].foundation_cache if retag_pipeline else FoundationCache()
-    load_args = {
-        'wordvec_pretrain_file': args['wordvec_pretrain_file'],
-        'charlm_forward_file': args['charlm_forward_file'],
-        'charlm_backward_file': args['charlm_backward_file'],
-        'device': args['device'],
-    }
-    trainer = Trainer.load(model_file, args=load_args, foundation_cache=foundation_cache)
-    model = trainer.model
-    model.eval()
-    tlogger.info("Loaded model from %s", model_file)
-
-    if args['tokenized_dir']:
-        if not args['predict_dir']:
-            raise ValueError("Must specific --predict_dir to go with --tokenized_dir")
-        parse_dir(args, model, retag_pipeline, args['tokenized_dir'], args['predict_dir'])
-    else:
-        parse_text(args, model, retag_pipeline)
-
-def parse_dir(args, model, retag_pipeline, tokenized_dir, predict_dir):
-    os.makedirs(predict_dir, exist_ok=True)
-    for filename in os.listdir(tokenized_dir):
-        input_path = os.path.join(tokenized_dir, filename)
-        output_path = os.path.join(predict_dir, os.path.splitext(filename)[0] + ".mrg")
-        tlogger.info("Processing %s to %s", input_path, output_path)
-        parse_text(args, model, retag_pipeline, tokenized_file=input_path, predict_file=output_path)
-
-def read_tokenized_file(tokenized_file):
-    """
-    Read sentences from a tokenized file, potentially replacing _ with space for languages such as VI
-    """
-    with open(tokenized_file, encoding='utf-8') as fin:
-        lines = fin.readlines()
-    lines = [x.strip() for x in lines]
-    lines = [x for x in lines if x]
-    docs = [[word if all(x == '_' for x in word) else word.replace("_", " ") for word in sentence.split()] for sentence in lines]
-    return docs
-
-def parse_tokenized_sentences(args, model, retag_pipeline, sentences):
-    tags = retag_tags(sentences, retag_pipeline, model.uses_xpos())
-    words = [[(word, tag) for word, tag in zip(s_words, s_tags)] for s_words, s_tags in zip(sentences, tags)]
-    logger.info("Retagging finished.  Parsing tagged text")
-
-    assert len(words) == len(sentences)
-    treebank = model.parse_sentences_no_grad(iter(tqdm(words)), model.build_batch_from_tagged_words, args['eval_batch_size'], model.predict, keep_scores=False)
-    return treebank
-
-def parse_text(args, model, retag_pipeline, tokenized_file=None, predict_file=None):
-    """
-    Use the given model to parse text and write it
-
-    refactored so it can be used elsewhere, such as Ensemble
-
-    TODO: some of these things really ought to be separated out from trainer.py
-    """
-    model.eval()
-
-    if predict_file is None:
-        if args['predict_file']:
-            predict_file = args['predict_file']
-            if args['predict_dir']:
-                predict_file = os.path.join(args['predict_dir'], predict_file)
-
-    if tokenized_file is None:
-        tokenized_file = args['tokenized_file']
-
-    if tokenized_file is not None:
-        docs = read_tokenized_file(tokenized_file)
-        tlogger.info("Processing %d lines", len(docs))
-
-        with utils.output_stream(predict_file) as fout:
-            chunk_size = 10000
-            for chunk_start in range(0, len(docs), chunk_size):
-                chunk = docs[chunk_start:chunk_start+chunk_size]
-                tlogger.info("Processing trees %d to %d", chunk_start, chunk_start+len(chunk))
-                treebank = parse_tokenized_sentences(args, model, retag_pipeline, chunk)
-
-                for tree_idx, result in enumerate(treebank):
-                    tree = result.predictions[0].tree
-                    tree.tree_id = chunk_start + tree_idx + 1
-                    fout.write(args['predict_format'].format(tree))
-                    fout.write("\n")
-
 def evaluate(args, model_file, retag_pipeline):
     """
     Loads the given model file and tests the eval_file treebank.
 
     May retag the trees using retag_pipeline
     Uses a subprocess to run the Java EvalB code
     """
@@ -397,45 +303,34 @@
             'charlm_forward_file': args['charlm_forward_file'],
             'charlm_backward_file': args['charlm_backward_file'],
             'device': args['device'],
         }
         trainer = Trainer.load(model_file, args=load_args, foundation_cache=foundation_cache)
 
         if args['log_shapes']:
-            trainer.model.log_shapes()
+            trainer.log_shapes()
 
         treebank = tree_reader.read_treebank(args['eval_file'])
         tlogger.info("Read %d trees for evaluation", len(treebank))
 
+        retagged_treebank = treebank
         if retag_pipeline is not None:
             retag_method = trainer.model.args['retag_method']
             retag_xpos = trainer.model.args['retag_xpos']
             tlogger.info("Retagging trees using the %s tags from the %s package...", retag_method, args['retag_package'])
             retagged_treebank = retag_trees(treebank, retag_pipeline, retag_xpos)
             tlogger.info("Retagging finished")
 
         if args['log_norms']:
-            trainer.model.log_norms()
+            trainer.log_norms()
         f1, kbestF1, _ = run_dev_set(trainer.model, retagged_treebank, treebank, args, evaluator)
         tlogger.info("F1 score on %s: %f", args['eval_file'], f1)
         if kbestF1 is not None:
             tlogger.info("KBest F1 score on %s: %f", args['eval_file'], kbestF1)
 
-def get_open_nodes(trees, args):
-    """
-    Return a list of all open nodes in the given dataset.
-    Depending on the parameters, may be single or compound open transitions.
-    """
-    if args['transition_scheme'] is TransitionScheme.TOP_DOWN_COMPOUND:
-        return parse_tree.Tree.get_compound_constituents(trees)
-    elif args['transition_scheme'] is TransitionScheme.IN_ORDER_COMPOUND:
-        return parse_tree.Tree.get_compound_constituents(trees, separate_root=True)
-    else:
-        return [(x,) for x in parse_tree.Tree.get_unique_constituent_labels(trees)]
-
 def remove_optimizer(args, model_save_file, model_load_file):
     """
     A utility method to remove the optimizer from a save file
 
     Will make the save file a lot smaller
     """
     # TODO: kind of overkill to load in the pretrain rather than
@@ -455,50 +350,33 @@
     Adds a torch.clamp hook on each parameter if grad_clipping is not None
     """
     if grad_clipping is not None:
         for p in trainer.model.parameters():
             if p.requires_grad:
                 p.register_hook(lambda grad: torch.clamp(grad, -grad_clipping, grad_clipping))
 
-def check_constituents(train_constituents, trees, treebank_name):
-    """
-    Check that all the constituents in the other dataset are known in the train set
-    """
-    constituents = parse_tree.Tree.get_unique_constituent_labels(trees)
-    for con in constituents:
-        if con not in train_constituents:
-            raise RuntimeError("Found label {} in the {} set which don't exist in the train set".format(con, treebank_name))
-
-def check_root_labels(root_labels, other_trees, treebank_name):
-    """
-    Check that all the root states in the other dataset are known in the train set
-    """
-    for root_state in parse_tree.Tree.get_root_labels(other_trees):
-        if root_state not in root_labels:
-            raise RuntimeError("Found root state {} in the {} set which is not a ROOT state in the train set".format(root_state, treebank_name))
-
 def build_trainer(args, train_trees, dev_trees, silver_trees, foundation_cache, model_load_file):
     """
     Builds a Trainer (with model) and the train_sequences and transitions for the given trees.
     """
-    train_constituents = parse_tree.Tree.get_unique_constituent_labels(train_trees)
+    train_constituents = Tree.get_unique_constituent_labels(train_trees)
     tlogger.info("Unique constituents in training set: %s", train_constituents)
     if args['check_valid_states']:
         check_constituents(train_constituents, dev_trees, "dev")
         check_constituents(train_constituents, silver_trees, "silver")
-    constituent_counts = parse_tree.Tree.get_constituent_counts(train_trees)
+    constituent_counts = Tree.get_constituent_counts(train_trees)
     tlogger.info("Constituent node counts: %s", constituent_counts)
 
-    tags = parse_tree.Tree.get_unique_tags(train_trees)
+    tags = Tree.get_unique_tags(train_trees)
     if None in tags:
         raise RuntimeError("Fatal problem: the tagger put None on some of the nodes!")
     tlogger.info("Unique tags in training set: %s", tags)
     # no need to fail for missing tags between train/dev set
     # the model has an unknown tag embedding
-    for tag in parse_tree.Tree.get_unique_tags(dev_trees):
+    for tag in Tree.get_unique_tags(dev_trees):
         if tag not in tags:
             tlogger.info("Found tag in dev set which does not exist in train set: %s  Continuing...", tag)
 
     unary_limit = max(max(t.count_unary_depth() for t in train_trees),
                       max(t.count_unary_depth() for t in dev_trees)) + 1
     if silver_trees:
         unary_limit = max(unary_limit, max(t.count_unary_depth() for t in silver_trees))
@@ -511,36 +389,36 @@
     tlogger.info("Unique transitions in training set: %s", train_transitions)
     expanded_train_transitions = set(train_transitions + [x for trans in train_transitions for x in trans.components()])
     if args['check_valid_states']:
         parse_transitions.check_transitions(expanded_train_transitions, dev_transitions, "dev")
         # theoretically could just train based on the items in the silver dataset
         parse_transitions.check_transitions(expanded_train_transitions, silver_transitions, "silver")
 
-    root_labels = parse_tree.Tree.get_root_labels(train_trees)
+    root_labels = Tree.get_root_labels(train_trees)
     check_root_labels(root_labels, dev_trees, "dev")
     check_root_labels(root_labels, silver_trees, "silver")
     tlogger.info("Root labels in treebank: %s", root_labels)
 
     verify_transitions(train_trees, train_sequences, args['transition_scheme'], unary_limit, args['reversed'], "train", root_labels)
     verify_transitions(dev_trees, dev_sequences, args['transition_scheme'], unary_limit, args['reversed'], "dev", root_labels)
 
     # we don't check against the words in the dev set as it is
     # expected there will be some UNK words
-    words = parse_tree.Tree.get_unique_words(train_trees)
-    rare_words = parse_tree.Tree.get_rare_words(train_trees, args['rare_word_threshold'])
+    words = Tree.get_unique_words(train_trees)
+    rare_words = Tree.get_rare_words(train_trees, args['rare_word_threshold'])
     # rare/unknown silver words will just get UNK if they are not already known
     if silver_trees and args['use_silver_words']:
         tlogger.info("Getting silver words to add to the delta embedding")
-        silver_words = parse_tree.Tree.get_common_words(tqdm(silver_trees, postfix='Silver words'), len(words))
+        silver_words = Tree.get_common_words(tqdm(silver_trees, postfix='Silver words'), len(words))
         words = sorted(set(words + silver_words))
 
     # also, it's not actually an error if there is a pattern of
     # compound unary or compound open nodes which doesn't exist in the
     # train set.  it just means we probably won't ever get that right
-    open_nodes = get_open_nodes(train_trees, args)
+    open_nodes = get_open_nodes(train_trees, args['transition_scheme'])
     tlogger.info("Using the following open nodes:\n  %s", "\n  ".join(map(str, open_nodes)))
 
     # at this point we have:
     # pretrain
     # train_trees, dev_trees
     # lists of transitions, internal nodes, and root states the parser needs to be aware of
 
@@ -561,99 +439,98 @@
         # relearn_structure is essentially a one stage multistage
         # multistage with a checkpoint will have the proper optimizer for that epoch
         # and no special learning mode means we are training a new model and should continue
         return trainer, train_sequences, silver_sequences, train_transitions
 
     if args['finetune']:
         tlogger.info("Loading model to finetune: %s", model_load_file)
-        trainer = Trainer.load(model_load_file, args, load_optimizer=True, foundation_cache=foundation_cache)
+        trainer = Trainer.load(model_load_file, args, load_optimizer=True, foundation_cache=NoTransformerFoundationCache(foundation_cache))
         # a new finetuning will start with a new epochs_trained count
         trainer.epochs_trained = 0
     elif args['relearn_structure']:
         tlogger.info("Loading model to continue training with new structure from %s", model_load_file)
         temp_args = dict(args)
         # remove the pattn & lattn layers unless the saved model had them
         temp_args.pop('pattn_num_layers', None)
         temp_args.pop('lattn_d_proj', None)
-        trainer = Trainer.load(model_load_file, temp_args, load_optimizer=False, foundation_cache=foundation_cache)
+        trainer = Trainer.load(model_load_file, temp_args, load_optimizer=False, foundation_cache=NoTransformerFoundationCache(foundation_cache))
 
         # using the model's current values works for if the new
         # dataset is the same or smaller
         # TODO: handle a larger dataset as well
-        model = LSTMModel(pt, forward_charlm, backward_charlm, trainer.model.bert_model, trainer.model.bert_tokenizer, trainer.model.force_bert_saved, trainer.model.transitions, trainer.model.constituents, trainer.model.tags, trainer.model.delta_words, trainer.model.rare_words, trainer.model.root_labels, trainer.model.constituent_opens, trainer.model.unary_limit(), args)
+        model = LSTMModel(pt,
+                          forward_charlm,
+                          backward_charlm,
+                          trainer.model.bert_model,
+                          trainer.model.bert_tokenizer,
+                          trainer.model.force_bert_saved,
+                          trainer.model.peft_name,
+                          trainer.model.transitions,
+                          trainer.model.constituents,
+                          trainer.model.tags,
+                          trainer.model.delta_words,
+                          trainer.model.rare_words,
+                          trainer.model.root_labels,
+                          trainer.model.constituent_opens,
+                          trainer.model.unary_limit(),
+                          args)
         model = model.to(args['device'])
         model.copy_with_new_structure(trainer.model)
         optimizer = build_optimizer(args, model, False)
         scheduler = build_scheduler(args, optimizer)
         trainer = Trainer(model, optimizer, scheduler)
-    elif args['multistage']:
-        # run adadelta over the model for half the time with no pattn or lattn
-        # training then switches to a different optimizer for the rest
-        # this works surprisingly well
-        tlogger.info("Warming up model for %d iterations using AdaDelta to train the embeddings", args['epochs'] // 2)
-        temp_args = dict(args)
-        # remove the attention layers for the temporary model
-        temp_args['pattn_num_layers'] = 0
-        temp_args['lattn_d_proj'] = 0
-
-        if args['bert_finetune'] or args['stage1_bert_finetune']:
+    else:
+        if args['multistage']:
+            # run adadelta over the model for half the time with no pattn or lattn
+            # training then switches to a different optimizer for the rest
+            # this works surprisingly well
+            tlogger.info("Warming up model for %d iterations using AdaDelta to train the embeddings", args['epochs'] // 2)
+            temp_args = dict(args)
+            # remove the attention layers for the temporary model
+            temp_args['pattn_num_layers'] = 0
+            temp_args['lattn_d_proj'] = 0
+            args = temp_args
+
+        peft_name = None
+        if args['use_peft']:
+            peft_name = "constituency"
             bert_model, bert_tokenizer = load_bert(args['bert_model'])
-        else:
-            bert_model, bert_tokenizer = load_bert(args['bert_model'], foundation_cache)
-        temp_model = LSTMModel(pt, forward_charlm, backward_charlm, bert_model, bert_tokenizer, False, train_transitions, train_constituents, tags, words, rare_words, root_labels, open_nodes, unary_limit, temp_args)
-        temp_model = temp_model.to(args['device'])
-        temp_optim = build_optimizer(temp_args, temp_model, True)
-        scheduler = build_scheduler(temp_args, temp_optim, True)
-        trainer = Trainer(temp_model, temp_optim, scheduler)
-    else:     # TODO: combine with the multistage version?  could make this a single stage
-        if args['bert_finetune']:
+            bert_model = build_peft_wrapper(bert_model, temp_args, tlogger, adapter_name=peft_name)
+        elif args['bert_finetune'] or args['stage1_bert_finetune']:
             bert_model, bert_tokenizer = load_bert(args['bert_model'])
         else:
             bert_model, bert_tokenizer = load_bert(args['bert_model'], foundation_cache)
-        model = LSTMModel(pt, forward_charlm, backward_charlm, bert_model, bert_tokenizer, False, train_transitions, train_constituents, tags, words, rare_words, root_labels, open_nodes, unary_limit, args)
+        model = LSTMModel(pt,
+                          forward_charlm,
+                          backward_charlm,
+                          bert_model,
+                          bert_tokenizer,
+                          False,
+                          peft_name,
+                          train_transitions,
+                          train_constituents,
+                          tags,
+                          words,
+                          rare_words,
+                          root_labels,
+                          open_nodes,
+                          unary_limit,
+                          args)
         model = model.to(args['device'])
 
-        optimizer = build_optimizer(args, model, False)
-        scheduler = build_scheduler(args, optimizer)
+        optimizer = build_optimizer(args, model, build_simple_adadelta=args['multistage'])
+        scheduler = build_scheduler(args, optimizer, first_optimizer=args['multistage'])
 
         trainer = Trainer(model, optimizer, scheduler)
 
     tlogger.info("Number of words in the training set found in the embedding: %d out of %d", trainer.model.num_words_known(words), len(words))
     add_grad_clipping(trainer, args['grad_clipping'])
 
     return trainer, train_sequences, silver_sequences, train_transitions
 
-def remove_duplicates(trees, dataset):
-    """
-    Filter duplicates from the given dataset
-    """
-    new_trees = []
-    known_trees = set()
-    for tree in trees:
-        tree_str = "{}".format(tree)
-        if tree_str in known_trees:
-            continue
-        known_trees.add(tree_str)
-        new_trees.append(tree)
-    if len(new_trees) < len(trees):
-        tlogger.info("Filtered %d duplicates from %s dataset", (len(trees) - len(new_trees)), dataset)
-    return new_trees
-
-def remove_no_tags(trees):
-    """
-    TODO: remove these trees in the conversion instead of here
-    """
-    new_trees = [x for x in trees if
-                 len(x.children) > 1 or
-                 (len(x.children) == 1 and len(x.children[0].children) > 1) or
-                 (len(x.children) == 1 and len(x.children[0].children) == 1 and len(x.children[0].children[0].children) >= 1)]
-    if len(trees) - len(new_trees) > 0:
-        tlogger.info("Eliminated %d trees with missing structure", (len(trees) - len(new_trees)))
-    return new_trees
-
 def train(args, model_load_file, retag_pipeline):
     """
     Build a model, train it using the requested train & dev files
     """
     utils.log_training_args(args, logger)
 
     # we create the Evaluator here because otherwise the transformers
@@ -674,40 +551,40 @@
         wandb.run.define_metric('dev_score', summary='max')
 
     with EvaluateParser(kbest=kbest) as evaluator:
         utils.ensure_dir(args['save_dir'])
 
         train_trees = tree_reader.read_treebank(args['train_file'])
         tlogger.info("Read %d trees for the training set", len(train_trees))
-        train_trees = remove_duplicates(train_trees, "train")
-        train_trees = remove_no_tags(train_trees)
+        train_trees = remove_duplicate_trees(train_trees, "train")
+        train_trees = remove_singleton_trees(train_trees)
 
         dev_trees = tree_reader.read_treebank(args['eval_file'])
         tlogger.info("Read %d trees for the dev set", len(dev_trees))
-        dev_trees = remove_duplicates(dev_trees, "dev")
+        dev_trees = remove_duplicate_trees(dev_trees, "dev")
 
         silver_trees = []
         if args['silver_file']:
             silver_trees = tree_reader.read_treebank(args['silver_file'])
             tlogger.info("Read %d trees for the silver training set", len(silver_trees))
             if args['silver_remove_duplicates']:
-                silver_trees = remove_duplicates(silver_trees, "silver")
+                silver_trees = remove_duplicate_trees(silver_trees, "silver")
 
         if retag_pipeline is not None:
             tlogger.info("Retagging trees using the %s tags from the %s package...", args['retag_method'], args['retag_package'])
             train_trees = retag_trees(train_trees, retag_pipeline, args['retag_xpos'])
             dev_trees = retag_trees(dev_trees, retag_pipeline, args['retag_xpos'])
             silver_trees = retag_trees(silver_trees, retag_pipeline, args['retag_xpos'])
             tlogger.info("Retagging finished")
 
         foundation_cache = retag_pipeline[0].foundation_cache if retag_pipeline else FoundationCache()
         trainer, train_sequences, silver_sequences, train_transitions = build_trainer(args, train_trees, dev_trees, silver_trees, foundation_cache, model_load_file)
 
         if args['log_shapes']:
-            model.log_shapes()
+            trainer.log_shapes()
         trainer = iterate_training(args, trainer, train_trees, train_sequences, train_transitions, dev_trees, silver_trees, silver_sequences, foundation_cache, evaluator)
 
     if args['wandb']:
         wandb.finish()
 
     return trainer
 
@@ -728,14 +605,24 @@
     preterminal_lists = [[Tree(label=preterminal.label, children=Tree(label=preterminal.children[0].label))
                           for preterminal in tree.yield_preterminals()]
                          for tree in trees]
     data = [TrainItem(*x) for x in zip(trees, sequences, preterminal_lists)]
     return data
 
 def next_epoch_data(leftover_training_data, train_data, epoch_size):
+    """
+    Return the next epoch_size trees from the training data, starting
+    with leftover data from the previous epoch if there is any
+
+    The training loop generally operates on a fixed number of trees,
+    rather than going through all the trees in the training set
+    exactly once, and keeping the leftover training data via this
+    function ensures that each tree in the training set is touched
+    once before beginning to iterate again.
+    """
     if not train_data:
         return [], []
 
     epoch_data = leftover_training_data
     while len(epoch_data) < epoch_size:
         random.shuffle(train_data)
         epoch_data.extend(train_data)
@@ -786,16 +673,14 @@
       extract a batch of trees of the same length from the training set
       convert those trees into initial parsing states
       repeat until trees are done:
         batch predict the model's interpretation of the current states
         add the errors to the list of things to backprop
         advance the parsing state for each of the trees
     """
-    model = trainer.model
-
     # Somewhat unusual, but possibly related to the extreme variability in length of trees
     # Various experiments generally show about 0.5 F1 loss on various
     # datasets when using 'mean' instead of 'sum' for reduction
     # (Remember to adjust the weight decay when rerunning that experiment)
     if args['loss'] == 'cross':
         tlogger.info("Building CrossEntropyLoss(sum)")
         process_outputs = lambda x: x
@@ -811,19 +696,19 @@
     elif args['loss'] == 'large_margin':
         tlogger.info("Building LargeMarginInSoftmaxLoss(sum)")
         process_outputs = lambda x: x
         model_loss_function = LargeMarginInSoftmaxLoss(reduction='sum')
     else:
         raise ValueError("Unexpected loss term: %s" % args['loss'])
 
-    device = next(model.parameters()).device
+    device = trainer.device
     model_loss_function.to(device)
     transition_tensors = {x: torch.tensor(y, requires_grad=False, device=device).unsqueeze(0)
-                          for (y, x) in enumerate(model.transitions)}
-    model.train()
+                          for (y, x) in enumerate(trainer.transitions)}
+    trainer.train()
 
     train_data = compose_train_data(train_trees, train_sequences)
     silver_data = compose_train_data(silver_trees, silver_sequences)
 
     if not args['epoch_size']:
         args['epoch_size'] = len(train_data)
     if silver_data and not args['silver_epoch_size']:
@@ -834,46 +719,46 @@
         # if we're halfway, only do pattn.  save lattn for next time
         multistage_splits[args['epochs'] // 2] = (args['pattn_num_layers'], False)
         if LSTMModel.uses_lattn(args):
             multistage_splits[args['epochs'] * 3 // 4] = (args['pattn_num_layers'], True)
 
     oracle = None
     if args['transition_scheme'] is TransitionScheme.IN_ORDER:
-        oracle = InOrderOracle(model.root_labels, args['oracle_level'], args['additional_oracle_levels'])
+        oracle = InOrderOracle(trainer.root_labels, args['oracle_level'], args['additional_oracle_levels'])
     elif args['transition_scheme'] is TransitionScheme.TOP_DOWN:
-        oracle = TopDownOracle(model.root_labels, args['oracle_level'], args['additional_oracle_levels'])
+        oracle = TopDownOracle(trainer.root_labels, args['oracle_level'], args['additional_oracle_levels'])
 
     leftover_training_data = []
     leftover_silver_data = []
     if trainer.best_epoch > 0:
         tlogger.info("Restarting trainer with a model trained for %d epochs.  Best epoch %d, f1 %f", trainer.epochs_trained, trainer.best_epoch, trainer.best_f1)
 
     # if we're training a new model, save the initial state so it can be inspected
     if args['save_each_start'] == 0 and trainer.epochs_trained == 0:
         trainer.save(args['save_each_name'] % trainer.epochs_trained, save_optimizer=True)
 
     # trainer.epochs_trained+1 so that if the trainer gets saved after 1 epoch, the epochs_trained is 1
     for trainer.epochs_trained in range(trainer.epochs_trained+1, args['epochs']+1):
-        model.train()
+        trainer.train()
         tlogger.info("Starting epoch %d", trainer.epochs_trained)
         update_bert_learning_rate(args, trainer.optimizer, trainer.epochs_trained)
 
         if args['log_norms']:
-            model.log_norms()
+            trainer.log_norms()
         leftover_training_data, epoch_data = next_epoch_data(leftover_training_data, train_data, args['epoch_size'])
         leftover_silver_data, epoch_silver_data = next_epoch_data(leftover_silver_data, silver_data, args['silver_epoch_size'])
         epoch_data = epoch_data + epoch_silver_data
         epoch_data.sort(key=lambda x: len(x[1]))
 
         epoch_stats = train_model_one_epoch(trainer.epochs_trained, trainer, transition_tensors, process_outputs, model_loss_function, epoch_data, oracle, args)
 
         # print statistics
         # by now we've forgotten about the original tags on the trees,
         # but it doesn't matter for hill climbing
-        f1, _, _ = run_dev_set(model, dev_trees, dev_trees, args, evaluator)
+        f1, _, _ = run_dev_set(trainer.model, dev_trees, dev_trees, args, evaluator)
         if f1 > trainer.best_f1 or (trainer.best_epoch == 0 and trainer.best_f1 == 0.0):
             # best_epoch == 0 to force a save of an initial model
             # useful for tests which expect something, even when a
             # very simple model didn't learn anything
             tlogger.info("New best dev score: %.5f > %.5f", f1, trainer.best_f1)
             trainer.best_f1 = f1
             trainer.best_epoch = trainer.epochs_trained
@@ -888,54 +773,75 @@
         if old_lr != new_lr:
             tlogger.info("Updating learning rate from %f to %f", old_lr, new_lr)
 
         if args['wandb']:
             wandb.log({'epoch_loss': epoch_stats.epoch_loss, 'dev_score': f1}, step=trainer.epochs_trained)
             if args['wandb_norm_regex']:
                 watch_regex = re.compile(args['wandb_norm_regex'])
-                for n, p in model.named_parameters():
+                for n, p in trainer.model.named_parameters():
                     if watch_regex.search(n):
                         wandb.log({n: torch.linalg.norm(p)})
 
         # recreate the optimizer and alter the model as needed if we hit a new multistage split
         if args['multistage'] and trainer.epochs_trained in multistage_splits:
             # we may be loading a save model from an earlier epoch if the scores stopped increasing
             epochs_trained = trainer.epochs_trained
             batches_trained = trainer.batches_trained
 
             stage_pattn_layers, stage_uses_lattn = multistage_splits[epochs_trained]
 
             # when loading the model, let the saved model determine whether it has pattn or lattn
-            temp_args = copy.deepcopy(model.args)
+            temp_args = copy.deepcopy(trainer.model.args)
             temp_args.pop('pattn_num_layers', None)
             temp_args.pop('lattn_d_proj', None)
             # overwriting the old trainer & model will hopefully free memory
-            trainer = Trainer.load(args['save_name'], temp_args, load_optimizer=False, foundation_cache=foundation_cache)
+            # load a new bert, even in PEFT mode, mostly so that the bert model
+            # doesn't collect a whole bunch of PEFTs
+            # for one thing, two PEFTs would mean 2x the optimizer parameters,
+            # messing up saving and loading the optimizer without jumping
+            # through more hoops
+            # loading the trainer w/o the foundation_cache should create
+            # the necessary bert_model and bert_tokenizer, and then we
+            # can reuse those values when building out new LSTMModel
+            trainer = Trainer.load(args['save_name'], temp_args, load_optimizer=False)
             model = trainer.model
             tlogger.info("Finished stage at epoch %d.  Restarting optimizer", epochs_trained)
             tlogger.info("Previous best model was at epoch %d", trainer.epochs_trained)
 
             temp_args = dict(args)
             tlogger.info("Switching to a model with %d pattn layers and %slattn", stage_pattn_layers, "" if stage_uses_lattn else "NO ")
             temp_args['pattn_num_layers'] = stage_pattn_layers
             if not stage_uses_lattn:
                 temp_args['lattn_d_proj'] = 0
             pt = foundation_cache.load_pretrain(args['wordvec_pretrain_file'])
             forward_charlm = foundation_cache.load_charlm(args['charlm_forward_file'])
             backward_charlm = foundation_cache.load_charlm(args['charlm_backward_file'])
-            bert_model, bert_tokenizer = foundation_cache.load_bert(args['bert_model'])
-            new_model = LSTMModel(pt, forward_charlm, backward_charlm, bert_model, bert_tokenizer, model.force_bert_saved, model.transitions, model.constituents, model.tags, model.delta_words, model.rare_words, model.root_labels, model.constituent_opens, model.unary_limit(), temp_args)
+            new_model = LSTMModel(pt,
+                                  forward_charlm,
+                                  backward_charlm,
+                                  model.bert_model,
+                                  model.bert_tokenizer,
+                                  model.force_bert_saved,
+                                  model.peft_name,
+                                  model.transitions,
+                                  model.constituents,
+                                  model.tags,
+                                  model.delta_words,
+                                  model.rare_words,
+                                  model.root_labels,
+                                  model.constituent_opens,
+                                  model.unary_limit(),
+                                  temp_args)
             new_model.to(device)
             new_model.copy_with_new_structure(model)
 
             optimizer = build_optimizer(temp_args, new_model, False)
             scheduler = build_scheduler(temp_args, optimizer)
             trainer = Trainer(new_model, optimizer, scheduler, epochs_trained, batches_trained, trainer.best_f1, trainer.best_epoch)
             add_grad_clipping(trainer, args['grad_clipping'])
-            model = new_model
 
         # checkpoint needs to be saved AFTER rebuilding the optimizer
         # so that assumptions about the optimizer in the checkpoint
         # can be made based on the end of the epoch
         if args['checkpoint'] and args['checkpoint_save_name']:
             trainer.save(args['checkpoint_save_name'], save_optimizer=True)
         # same with the "each filename", actually, in case those are
@@ -945,22 +851,21 @@
 
     return trainer
 
 def train_model_one_epoch(epoch, trainer, transition_tensors, process_outputs, model_loss_function, epoch_data, oracle, args):
     interval_starts = list(range(0, len(epoch_data), args['train_batch_size']))
     random.shuffle(interval_starts)
 
-    model = trainer.model
     optimizer = trainer.optimizer
 
     epoch_stats = EpochStats(0.0, Counter(), Counter(), Counter(), 0, 0)
 
     for batch_idx, interval_start in enumerate(tqdm(interval_starts, postfix="Epoch %d" % epoch)):
         batch = epoch_data[interval_start:interval_start+args['train_batch_size']]
-        batch_stats = train_model_one_batch(epoch, batch_idx, model, batch, transition_tensors, process_outputs, model_loss_function, oracle, args)
+        batch_stats = train_model_one_batch(epoch, batch_idx, trainer.model, batch, transition_tensors, process_outputs, model_loss_function, oracle, args)
         trainer.batches_trained += 1
 
         # Early in the training, some trees will be degenerate in a
         # way that results in layers going up the tree amplifying the
         # weights until they overflow.  Generally that problem
         # resolves itself in a few iterations, so for now we just
         # ignore those batches, but report how often it happens
@@ -990,18 +895,17 @@
     It is unclear if this refactoring is useful in any way.  Might not be
 
     ... although the indentation does get pretty ridiculous if this is
     merged into train_model_one_epoch and then iterate_training
     """
     # now we add the state to the trees in the batch
     # the state is built as a bulk operation
-    initial_states = model.initial_state_from_preterminals([x.preterminals for x in training_batch], [x.tree for x in training_batch])
-    initial_states = [state._replace(gold_sequence=sequence)
-                      for (tree, sequence, _), state in zip(training_batch, initial_states)]
-    current_batch = initial_states
+    current_batch = model.initial_state_from_preterminals([x.preterminals for x in training_batch],
+                                                          [x.tree for x in training_batch],
+                                                          [x.gold_sequence for x in training_batch])
 
     transitions_correct = Counter()
     transitions_incorrect = Counter()
     repairs_used = Counter()
     fake_transitions_used = 0
 
     all_errors = []
@@ -1069,27 +973,27 @@
                 update_transitions.append(pred_transition)
             else:
                 new_batch.append(state)
                 update_transitions.append(gold_transition)
 
         if len(current_batch) > 0:
             # bulk update states - significantly faster
-            current_batch = parse_transitions.bulk_apply(model, new_batch, update_transitions, fail=True)
+            current_batch = model.bulk_apply(new_batch, update_transitions, fail=True)
 
     errors = torch.cat(all_errors)
     answers = torch.cat(all_answers)
 
     errors = process_outputs(errors)
     tree_loss = model_loss_function(errors, answers)
     tree_loss.backward()
     if args['watch_regex']:
         matched = False
         tlogger.info("Watching %s   ... epoch %d batch %d", args['watch_regex'], epoch, batch_idx)
         watch_regex = re.compile(args['watch_regex'])
-        for n, p in model.named_parameters():
+        for n, p in trainer.model.named_parameters():
             if watch_regex.search(n):
                 matched = True
                 if p.requires_grad and p.grad is not None:
                     tlogger.info("  %s norm: %f grad: %f", n, torch.linalg.norm(p), torch.linalg.norm(p.grad))
                 elif p.requires_grad:
                     tlogger.info("  %s norm: %f grad required, but is None!", n, torch.linalg.norm(p))
                 else:
```

### Comparing `stanza-1.8.1/stanza/models/constituency/transformer_tree_stack.py` & `stanza-1.8.2/stanza/models/constituency/transformer_tree_stack.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/models/constituency/transition_sequence.py` & `stanza-1.8.2/stanza/models/constituency/transition_sequence.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/models/constituency/tree_embedding.py` & `stanza-1.8.2/stanza/models/constituency/tree_embedding.py`

 * *Files 2% similar despite different names*

```diff
@@ -124,11 +124,12 @@
     @staticmethod
     def from_parser_file(args, foundation_cache=None):
         constituency_parser = Trainer.load(args['model'], args, foundation_cache)
         return TreeEmbedding(constituency_parser.model, args)
 
     @staticmethod
     def model_from_params(params, args, foundation_cache=None):
-        constituency_parser = Trainer.model_from_params(params['constituency'], args, foundation_cache)
+        # TODO: integrate with peft
+        constituency_parser = Trainer.model_from_params(params['constituency'], None, args, foundation_cache)
         model = TreeEmbedding(constituency_parser, params['config'])
         model.load_state_dict(params['model'], strict=False)
         return model
```

### Comparing `stanza-1.8.1/stanza/models/constituency/tree_reader.py` & `stanza-1.8.2/stanza/models/constituency/tree_reader.py`

 * *Files 2% similar despite different names*

```diff
@@ -203,25 +203,26 @@
     token = next(token_iterator, None)
     while token:
         if token == OPEN_PAREN:
             next_tree = read_single_tree(token_iterator, broken_ok=broken_ok)
             if next_tree is None:
                 raise ValueError("Tree reader somehow created a None tree!  Line number %d" % token_iterator.line_num)
             if tree_callback is not None:
-                tree_callback(next_tree)
+                transformed = tree_callback(next_tree)
+                if transformed is not None:
+                    trees.append(transformed)
             else:
                 trees.append(next_tree)
             token = next(token_iterator, None)
         elif token == CLOSE_PAREN:
             raise ExtraCloseTreeError(token_iterator.line_num)
         else:
             raise ValueError("Tree document had text between trees!  Line number %d" % token_iterator.line_num)
 
-    if tree_callback is None:
-        return trees
+    return trees
 
 
 def read_trees(text, broken_ok=False, tree_callback=None, use_tqdm=True):
     """
     Reads multiple trees from the text
 
     TODO: some of the error cases we hit can be recovered from
```

### Comparing `stanza-1.8.1/stanza/models/constituency/tree_stack.py` & `stanza-1.8.2/stanza/models/constituency/tree_stack.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/models/constituency/utils.py` & `stanza-1.8.2/stanza/models/constituency/utils.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 """
 Collects a few of the conparser utility methods which don't belong elsewhere
 """
 
-from collections import Counter, deque
-import copy
+from collections import Counter
 import logging
 
 import torch.nn as nn
 from torch import optim
 
 from stanza.models.common.doc import TEXT, Document
 from stanza.models.common.utils import get_optimizer
+from stanza.models.constituency.base_model import SimpleModel
+from stanza.models.constituency.parse_transitions import TransitionScheme
+from stanza.models.constituency.parse_tree import Tree
 from stanza.utils.get_tqdm import get_tqdm
 
 tqdm = get_tqdm()
 
 DEFAULT_LEARNING_RATES = { "adamw": 0.0002, "adadelta": 1.0, "sgd": 0.001, "adabelief": 0.00005, "madgrad": 0.0000007 , "mirror_madgrad": 0.00005 }
 DEFAULT_LEARNING_EPS = { "adabelief": 1e-12, "adadelta": 1e-6, "adamw": 1e-8 }
 DEFAULT_LEARNING_RHO = 0.9
@@ -34,42 +36,14 @@
 #  0.000001.out: 0.9592548741021389
 #  0.000002.out: 0.9598395477013945
 #  0.000003.out: 0.9594974271553495
 #  0.000004.out: 0.9596665982603754
 #  0.000005.out: 0.9591620720706487
 DEFAULT_WEIGHT_DECAY = { "adamw": 0.05, "adadelta": 0.02, "sgd": 0.01, "adabelief": 1.2e-6, "madgrad": 2e-6, "mirror_madgrad": 2e-6 }
 
-def replace_tags(tree, tags):
-    if tree.is_leaf():
-        raise ValueError("Must call replace_tags with non-leaf")
-
-    tag_iterator = iter(tags)
-
-    new_tree = copy.deepcopy(tree)
-    queue = deque()
-    queue.append(new_tree)
-    while len(queue) > 0:
-        next_node = queue.pop()
-        if next_node.is_preterminal():
-            try:
-                label = next(tag_iterator)
-            except StopIteration:
-                raise ValueError("Not enough tags in sentence for given tree")
-            next_node.label = label
-        elif next_node.is_leaf():
-            raise ValueError("Got a badly structured tree: {}".format(tree))
-        else:
-            queue.extend(reversed(next_node.children))
-
-    if any(True for _ in tag_iterator):
-        raise ValueError("Too many tags for the given tree")
-
-    return new_tree
-
-
 def retag_tags(doc, pipelines, xpos):
     """
     Returns a list of list of tags for the items in doc
 
     doc can be anything which feeds into the pipeline(s)
     pipelines are a list of 1 or more retag pipelines
     if multiple pipelines are given, majority vote wins
@@ -111,15 +85,17 @@
                 raise ValueError("Unable to process tree %d" % (idx + chunk_start)) from e
 
             doc = Document(sentences)
             tag_lists = retag_tags(doc, pipelines, xpos)
 
             for tree_idx, (tree, tags) in enumerate(zip(chunk, tag_lists)):
                 try:
-                    new_tree = replace_tags(tree, tags)
+                    if any(tag is None for tag in tags):
+                        raise RuntimeError("Tagged tree #{} with a None tag!\n{}\n{}".format(tree_idx, tree, tags))
+                    new_tree = tree.replace_tags(tags)
                     new_trees.append(new_tree)
                     pbar.update(1)
                 except ValueError as e:
                     raise ValueError("Failed to properly retag tree #{}: {}".format(tree_idx, tree)) from e
     if len(new_trees) != len(trees):
         raise AssertionError("Retagged tree counts did not match: {} vs {}".format(len(new_trees), len(trees)))
     return new_trees
@@ -292,7 +268,101 @@
     parser.add_argument('--predict_dir', type=str, default=".", help='Where to write the predictions during --mode predict.  Pred and orig files will be written - the orig file will be retagged if that is requested.  Writing the orig file is useful for removing None and retagging')
     parser.add_argument('--predict_file', type=str, default=None, help='Base name for writing predictions')
     parser.add_argument('--predict_format', type=str, default="{:_O}", help='Format to use when writing predictions')
 
 def postprocess_predict_output_args(args):
     if len(args['predict_format']) <= 2 or (len(args['predict_format']) <= 3 and args['predict_format'].endswith("Vi")):
         args['predict_format'] = "{:" + args['predict_format'] + "}"
+
+
+def get_open_nodes(trees, transition_scheme):
+    """
+    Return a list of all open nodes in the given dataset.
+    Depending on the parameters, may be single or compound open transitions.
+    """
+    if transition_scheme is TransitionScheme.TOP_DOWN_COMPOUND:
+        return Tree.get_compound_constituents(trees)
+    elif transition_scheme is TransitionScheme.IN_ORDER_COMPOUND:
+        return Tree.get_compound_constituents(trees, separate_root=True)
+    else:
+        return [(x,) for x in Tree.get_unique_constituent_labels(trees)]
+
+
+def verify_transitions(trees, sequences, transition_scheme, unary_limit, reverse, name, root_labels):
+    """
+    Given a list of trees and their transition sequences, verify that the sequences rebuild the trees
+    """
+    model = SimpleModel(transition_scheme, unary_limit, reverse, root_labels)
+    tlogger.info("Verifying the transition sequences for %d trees", len(trees))
+
+    data = zip(trees, sequences)
+    if tlogger.getEffectiveLevel() <= logging.INFO:
+        data = tqdm(zip(trees, sequences), total=len(trees))
+
+    for tree_idx, (tree, sequence) in enumerate(data):
+        # TODO: make the SimpleModel have a parse operation?
+        state = model.initial_state_from_gold_trees([tree])[0]
+        for idx, trans in enumerate(sequence):
+            if not trans.is_legal(state, model):
+                raise RuntimeError("Tree {} of {} failed: transition {}:{} was not legal in a transition sequence:\nOriginal tree: {}\nTransitions: {}".format(tree_idx, name, idx, trans, tree, sequence))
+            state = trans.apply(state, model)
+        result = model.get_top_constituent(state.constituents)
+        if reverse:
+            result = result.reverse()
+        if tree != result:
+            raise RuntimeError("Tree {} of {} failed: transition sequence did not match for a tree!\nOriginal tree:{}\nTransitions: {}\nResult tree:{}".format(tree_idx, name, tree, sequence, result))
+
+def check_constituents(train_constituents, trees, treebank_name):
+    """
+    Check that all the constituents in the other dataset are known in the train set
+    """
+    constituents = Tree.get_unique_constituent_labels(trees)
+    for con in constituents:
+        if con not in train_constituents:
+            first_error = None
+            num_errors = 0
+            for tree_idx, tree in enumerate(trees):
+                constituents = Tree.get_unique_constituent_labels(tree)
+                if con in constituents:
+                    num_errors += 1
+                    if first_error is None:
+                        first_error = tree_idx
+            raise RuntimeError("Found constituent label {} in the {} set which don't exist in the train set.  This constituent label occured in {} trees, with the first tree index at {} counting from 1\nThe error tree (which may have POS tags changed from the retagger and may be missing functional tags or empty nodes) is:\n{:P}".format(con, treebank_name, num_errors, (first_error+1), trees[first_error]))
+
+def check_root_labels(root_labels, other_trees, treebank_name):
+    """
+    Check that all the root states in the other dataset are known in the train set
+    """
+    for root_state in Tree.get_root_labels(other_trees):
+        if root_state not in root_labels:
+            raise RuntimeError("Found root state {} in the {} set which is not a ROOT state in the train set".format(root_state, treebank_name))
+
+def remove_duplicate_trees(trees, treebank_name):
+    """
+    Filter duplicates from the given dataset
+    """
+    new_trees = []
+    known_trees = set()
+    for tree in trees:
+        tree_str = "{}".format(tree)
+        if tree_str in known_trees:
+            continue
+        known_trees.add(tree_str)
+        new_trees.append(tree)
+    if len(new_trees) < len(trees):
+        tlogger.info("Filtered %d duplicates from %s dataset", (len(trees) - len(new_trees)), treebank_name)
+    return new_trees
+
+def remove_singleton_trees(trees):
+    """
+    remove trees which are just a root and a single word
+
+    TODO: remove these trees in the conversion instead of here
+    """
+    new_trees = [x for x in trees if
+                 len(x.children) > 1 or
+                 (len(x.children) == 1 and len(x.children[0].children) > 1) or
+                 (len(x.children) == 1 and len(x.children[0].children) == 1 and len(x.children[0].children[0].children) >= 1)]
+    if len(trees) - len(new_trees) > 0:
+        tlogger.info("Eliminated %d trees with missing structure", (len(trees) - len(new_trees)))
+    return new_trees
+
```

### Comparing `stanza-1.8.1/stanza/models/constituency_parser.py` & `stanza-1.8.2/stanza/models/constituency_parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -169,14 +169,15 @@
 from stanza.models.common import constant
 from stanza.models.common import utils
 from stanza.models.common.peft_config import add_peft_args, resolve_peft_args
 from stanza.models.constituency import retagging
 from stanza.models.constituency import trainer
 from stanza.models.constituency.lstm_model import ConstituencyComposition, SentenceBoundary, StackHistory
 from stanza.models.constituency.parse_transitions import TransitionScheme
+from stanza.models.constituency.text_processing import load_model_parse_text
 from stanza.models.constituency.utils import DEFAULT_LEARNING_EPS, DEFAULT_LEARNING_RATES, DEFAULT_MOMENTUM, DEFAULT_LEARNING_RHO, DEFAULT_WEIGHT_DECAY, NONLINEARITY, add_predict_output_args, postprocess_predict_output_args
 from stanza.resources.common import DEFAULT_MODEL_DIR
 
 logger = logging.getLogger('stanza')
 tlogger = logging.getLogger('stanza.constituency.trainer')
 
 def build_argparse():
@@ -848,13 +849,13 @@
     retag_pipeline = retagging.build_retag_pipeline(args)
 
     if args['mode'] == 'train':
         trainer.train(args, model_load_file, retag_pipeline)
     elif args['mode'] == 'predict':
         trainer.evaluate(args, model_load_file, retag_pipeline)
     elif args['mode'] == 'parse_text':
-        trainer.load_model_parse_text(args, model_load_file, retag_pipeline)
+        load_model_parse_text(args, model_load_file, retag_pipeline)
     elif args['mode'] == 'remove_optimizer':
         trainer.remove_optimizer(args, args['save_name'], model_load_file)
 
 if __name__ == '__main__':
     main()
```

### Comparing `stanza-1.8.1/stanza/models/coref/anaphoricity_scorer.py` & `stanza-1.8.2/stanza/models/coref/anaphoricity_scorer.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/models/coref/bert.py` & `stanza-1.8.2/stanza/models/coref/bert.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/models/coref/cluster_checker.py` & `stanza-1.8.2/stanza/models/coref/cluster_checker.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/models/coref/config.py` & `stanza-1.8.2/stanza/models/coref/config.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/models/coref/conll.py` & `stanza-1.8.2/stanza/models/coref/conll.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/models/coref/const.py` & `stanza-1.8.2/stanza/models/coref/const.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/models/coref/coref_chain.py` & `stanza-1.8.2/stanza/models/coref/coref_chain.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/models/coref/loss.py` & `stanza-1.8.2/stanza/models/coref/loss.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/models/coref/model.py` & `stanza-1.8.2/stanza/models/coref/model.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/models/coref/pairwise_encoder.py` & `stanza-1.8.2/stanza/models/coref/pairwise_encoder.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/models/coref/predict.py` & `stanza-1.8.2/stanza/models/coref/predict.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/models/coref/rough_scorer.py` & `stanza-1.8.2/stanza/models/coref/rough_scorer.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/models/coref/span_predictor.py` & `stanza-1.8.2/stanza/models/coref/span_predictor.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/models/coref/tokenizer_customization.py` & `stanza-1.8.2/stanza/models/coref/tokenizer_customization.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/models/coref/utils.py` & `stanza-1.8.2/stanza/models/coref/utils.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/models/coref/word_encoder.py` & `stanza-1.8.2/stanza/models/coref/word_encoder.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/models/depparse/data.py` & `stanza-1.8.2/stanza/models/depparse/data.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/models/depparse/model.py` & `stanza-1.8.2/stanza/models/depparse/model.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,114 +5,96 @@
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 from torch.nn.utils.rnn import pad_packed_sequence, pack_padded_sequence, pack_sequence, pad_sequence, PackedSequence
 
 from stanza.models.common.bert_embedding import extract_bert_embeddings
 from stanza.models.common.biaffine import DeepBiaffineScorer
-from stanza.models.common.foundation_cache import load_bert, load_charlm
+from stanza.models.common.foundation_cache import load_charlm
 from stanza.models.common.hlstm import HighwayLSTM
 from stanza.models.common.dropout import WordDropout
-from stanza.models.common.peft_config import build_peft_wrapper
+from stanza.models.common.utils import attach_bert_model
 from stanza.models.common.vocab import CompositeVocab
 from stanza.models.common.char_model import CharacterModel, CharacterLanguageModel
 from stanza.models.common import utils
 
 logger = logging.getLogger('stanza')
 
 class Parser(nn.Module):
-    def __init__(self, args, vocab, emb_matrix=None, share_hid=False, foundation_cache=None, force_bert_saved=False):
+    def __init__(self, args, vocab, emb_matrix=None, share_hid=False, foundation_cache=None, bert_model=None, bert_tokenizer=None, force_bert_saved=False, peft_name=None):
         super().__init__()
 
         self.vocab = vocab
         self.args = args
         self.share_hid = share_hid
         self.unsaved_modules = []
 
-        def add_unsaved_module(name, module):
-            self.unsaved_modules += [name]
-            setattr(self, name, module)
-
         # input layers
         input_size = 0
         if self.args['word_emb_dim'] > 0:
             # frequent word embeddings
             self.word_emb = nn.Embedding(len(vocab['word']), self.args['word_emb_dim'], padding_idx=0)
             self.lemma_emb = nn.Embedding(len(vocab['lemma']), self.args['word_emb_dim'], padding_idx=0)
             input_size += self.args['word_emb_dim'] * 2
 
         if self.args['tag_emb_dim'] > 0:
-            self.upos_emb = nn.Embedding(len(vocab['upos']), self.args['tag_emb_dim'], padding_idx=0)
-
-            if not isinstance(vocab['xpos'], CompositeVocab):
-                self.xpos_emb = nn.Embedding(len(vocab['xpos']), self.args['tag_emb_dim'], padding_idx=0)
-            else:
-                self.xpos_emb = nn.ModuleList()
-
-                for l in vocab['xpos'].lens():
-                    self.xpos_emb.append(nn.Embedding(l, self.args['tag_emb_dim'], padding_idx=0))
+            if self.args.get('use_upos', True):
+                self.upos_emb = nn.Embedding(len(vocab['upos']), self.args['tag_emb_dim'], padding_idx=0)
+            if self.args.get('use_xpos', True):
+                if not isinstance(vocab['xpos'], CompositeVocab):
+                    self.xpos_emb = nn.Embedding(len(vocab['xpos']), self.args['tag_emb_dim'], padding_idx=0)
+                else:
+                    self.xpos_emb = nn.ModuleList()
+
+                    for l in vocab['xpos'].lens():
+                        self.xpos_emb.append(nn.Embedding(l, self.args['tag_emb_dim'], padding_idx=0))
+            if self.args.get('use_upos', True) or self.args.get('use_xpos', True):
+                input_size += self.args['tag_emb_dim']
 
-            self.ufeats_emb = nn.ModuleList()
+            if self.args.get('use_ufeats', True):
+                self.ufeats_emb = nn.ModuleList()
 
-            for l in vocab['feats'].lens():
-                self.ufeats_emb.append(nn.Embedding(l, self.args['tag_emb_dim'], padding_idx=0))
+                for l in vocab['feats'].lens():
+                    self.ufeats_emb.append(nn.Embedding(l, self.args['tag_emb_dim'], padding_idx=0))
 
-            input_size += self.args['tag_emb_dim'] * 2
+                input_size += self.args['tag_emb_dim']
 
         if self.args['char'] and self.args['char_emb_dim'] > 0:
             if self.args.get('charlm', None):
                 if args['charlm_forward_file'] is None or not os.path.exists(args['charlm_forward_file']):
                     raise FileNotFoundError('Could not find forward character model: {}  Please specify with --charlm_forward_file'.format(args['charlm_forward_file']))
                 if args['charlm_backward_file'] is None or not os.path.exists(args['charlm_backward_file']):
                     raise FileNotFoundError('Could not find backward character model: {}  Please specify with --charlm_backward_file'.format(args['charlm_backward_file']))
                 logger.debug("Depparse model loading charmodels: %s and %s", args['charlm_forward_file'], args['charlm_backward_file'])
-                add_unsaved_module('charmodel_forward', load_charlm(args['charlm_forward_file'], foundation_cache=foundation_cache))
-                add_unsaved_module('charmodel_backward', load_charlm(args['charlm_backward_file'], foundation_cache=foundation_cache))
+                self.add_unsaved_module('charmodel_forward', load_charlm(args['charlm_forward_file'], foundation_cache=foundation_cache))
+                self.add_unsaved_module('charmodel_backward', load_charlm(args['charlm_backward_file'], foundation_cache=foundation_cache))
                 input_size += self.charmodel_forward.hidden_dim() + self.charmodel_backward.hidden_dim()
             else:
                 self.charmodel = CharacterModel(args, vocab)
                 self.trans_char = nn.Linear(self.args['char_hidden_dim'], self.args['transformed_dim'], bias=False)
                 input_size += self.args['transformed_dim']
 
-        # TODO: refactor with POS
-        if self.args['bert_model']:
+        self.peft_name = peft_name
+        attach_bert_model(self, bert_model, bert_tokenizer, self.args.get('use_peft', False), force_bert_saved)
+        if self.args.get('bert_model', None):
+            # TODO: refactor bert_hidden_layers between the different models
             if args.get('bert_hidden_layers', False):
                 # The average will be offset by 1/N so that the default zeros
-                # repressents an average of the N layers
+                # represents an average of the N layers
                 self.bert_layer_mix = nn.Linear(args['bert_hidden_layers'], 1, bias=False)
                 nn.init.zeros_(self.bert_layer_mix.weight)
             else:
                 # an average of layers 2, 3, 4 will be used
                 # (for historic reasons)
                 self.bert_layer_mix = None
-            if self.args.get('use_peft', False):
-                bert_model, bert_tokenizer = load_bert(self.args['bert_model'], foundation_cache)
-                bert_model = build_peft_wrapper(bert_model, self.args, logger)
-                # we use a peft-specific pathway for saving peft weights
-                add_unsaved_module('bert_model', bert_model)
-                add_unsaved_module('bert_tokenizer', bert_tokenizer)
-                self.bert_model.train()
-            elif self.args.get('bert_finetune', False) or force_bert_saved:
-                bert_model, bert_tokenizer = load_bert(self.args['bert_model'])
-                self.bert_model = bert_model
-                add_unsaved_module('bert_tokenizer', bert_tokenizer)
-            else:
-                bert_model, bert_tokenizer = load_bert(self.args['bert_model'], foundation_cache)
-                for n, p in bert_model.named_parameters():
-                    p.requires_grad = False
-                add_unsaved_module('bert_model', bert_model)
-                add_unsaved_module('bert_tokenizer', bert_tokenizer)
-            input_size += bert_model.config.hidden_size
-        else:
-            self.bert_model = None
-            self.bert_tokenizer = None
+            input_size += self.bert_model.config.hidden_size
 
         if self.args['pretrain']:
             # pretrained embeddings, by default this won't be saved into model file
-            add_unsaved_module('pretrained_emb', nn.Embedding.from_pretrained(torch.from_numpy(emb_matrix), freeze=True))
+            self.add_unsaved_module('pretrained_emb', nn.Embedding.from_pretrained(torch.from_numpy(emb_matrix), freeze=True))
             self.trans_pretrained = nn.Linear(emb_matrix.shape[1], self.args['transformed_dim'], bias=False)
             input_size += self.args['transformed_dim']
 
         # recurrent layers
         self.parserlstm = HighwayLSTM(input_size, self.args['hidden_dim'], self.args['num_layers'], batch_first=True, bidirectional=True, dropout=self.args['dropout'], rec_dropout=self.args['rec_dropout'], highway_func=torch.tanh)
         self.drop_replacement = nn.Parameter(torch.randn(input_size) / np.sqrt(input_size))
         self.parserlstm_h_init = nn.Parameter(torch.zeros(2 * self.args['num_layers'], 1, self.args['hidden_dim']))
@@ -128,18 +110,22 @@
 
         # criterion
         self.crit = nn.CrossEntropyLoss(ignore_index=-1, reduction='sum') # ignore padding
 
         self.drop = nn.Dropout(args['dropout'])
         self.worddrop = WordDropout(args['word_dropout'])
 
+    def add_unsaved_module(self, name, module):
+        self.unsaved_modules += [name]
+        setattr(self, name, module)
+
     def log_norms(self):
         utils.log_norms(self)
 
-    def forward(self, word, word_mask, wordchars, wordchars_mask, upos, xpos, ufeats, pretrained, lemma, head, deprel, word_orig_idx, sentlens, wordlens, text, detach=True):
+    def forward(self, word, word_mask, wordchars, wordchars_mask, upos, xpos, ufeats, pretrained, lemma, head, deprel, word_orig_idx, sentlens, wordlens, text):
         def pack(x):
             return pack_padded_sequence(x, sentlens, batch_first=True)
 
         inputs = []
         if self.args['pretrain']:
             pretrained_emb = self.pretrained_emb(pretrained)
             pretrained_emb = self.trans_pretrained(pretrained_emb)
@@ -153,29 +139,37 @@
             word_emb = self.word_emb(word)
             word_emb = pack(word_emb)
             lemma_emb = self.lemma_emb(lemma)
             lemma_emb = pack(lemma_emb)
             inputs += [word_emb, lemma_emb]
 
         if self.args['tag_emb_dim'] > 0:
-            pos_emb = self.upos_emb(upos)
-
-            if isinstance(self.vocab['xpos'], CompositeVocab):
-                for i in range(len(self.vocab['xpos'])):
-                    pos_emb += self.xpos_emb[i](xpos[:, :, i])
+            if self.args.get('use_upos', True):
+                pos_emb = self.upos_emb(upos)
             else:
-                pos_emb += self.xpos_emb(xpos)
-            pos_emb = pack(pos_emb)
+                pos_emb = 0
 
-            feats_emb = 0
-            for i in range(len(self.vocab['feats'])):
-                feats_emb += self.ufeats_emb[i](ufeats[:, :, i])
-            feats_emb = pack(feats_emb)
+            if self.args.get('use_xpos', True):
+                if isinstance(self.vocab['xpos'], CompositeVocab):
+                    for i in range(len(self.vocab['xpos'])):
+                        pos_emb += self.xpos_emb[i](xpos[:, :, i])
+                else:
+                    pos_emb += self.xpos_emb(xpos)
+
+            if self.args.get('use_upos', True) or self.args.get('use_xpos', True):
+                pos_emb = pack(pos_emb)
+                inputs += [pos_emb]
+
+            if self.args.get('use_ufeats', True):
+                feats_emb = 0
+                for i in range(len(self.vocab['feats'])):
+                    feats_emb += self.ufeats_emb[i](ufeats[:, :, i])
+                feats_emb = pack(feats_emb)
 
-            inputs += [pos_emb, feats_emb]
+                inputs += [pos_emb]
 
         if self.args['char'] and self.args['char_emb_dim'] > 0:
             if self.args.get('charlm', None):
                 # \n is to add a somewhat neutral "word" for the ROOT
                 charlm_text = [["\n"] + x for x in text]
                 all_forward_chars = self.charmodel_forward.build_char_representation(charlm_text)
                 all_forward_chars = pack(pad_sequence(all_forward_chars, batch_first=True))
@@ -185,24 +179,22 @@
             else:
                 char_reps = self.charmodel(wordchars, wordchars_mask, word_orig_idx, sentlens, wordlens)
                 char_reps = PackedSequence(self.trans_char(self.drop(char_reps.data)), char_reps.batch_sizes)
                 inputs += [char_reps]
 
         if self.bert_model is not None:
             device = next(self.parameters()).device
-            detach = detach or not self.args.get('bert_finetune', False) or not self.training
             processed_bert = extract_bert_embeddings(self.args['bert_model'], self.bert_tokenizer, self.bert_model, text, device, keep_endpoints=True,
                                                      num_layers=self.bert_layer_mix.in_features if self.bert_layer_mix is not None else None,
-                                                     detach=detach)
+                                                     detach=not self.args.get('bert_finetune', False) or not self.training,
+                                                     peft_name=self.peft_name)
             if self.bert_layer_mix is not None:
-                # add the average so that the default behavior is to
-                # take an average of the N layers, and anything else
-                # other than that needs to be learned
-                # TODO: refactor this
+                # use a linear layer to weighted average the embedding dynamically
                 processed_bert = [self.bert_layer_mix(feature).squeeze(2) + feature.sum(axis=2) / self.bert_layer_mix.in_features for feature in processed_bert]
+
             # we are using the first endpoint from the transformer as the "word" for ROOT
             processed_bert = [x[:-1, :] for x in processed_bert]
             processed_bert = pad_sequence(processed_bert, batch_first=True)
             inputs += [pack(processed_bert)]
 
         lstm_inputs = torch.cat([x.data for x in inputs], 1)
```

### Comparing `stanza-1.8.1/stanza/models/depparse/scorer.py` & `stanza-1.8.2/stanza/models/depparse/scorer.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/models/depparse/trainer.py` & `stanza-1.8.2/stanza/models/depparse/trainer.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,16 +11,17 @@
 try:
     import transformers
 except ImportError:
     pass
 
 from stanza.models.common.trainer import Trainer as BaseTrainer
 from stanza.models.common import utils, loss
-from stanza.models.common.foundation_cache import NoTransformerFoundationCache
+from stanza.models.common.foundation_cache import load_bert, load_bert_with_peft, NoTransformerFoundationCache
 from stanza.models.common.chuliu_edmonds import chuliu_edmonds_one_root
+from stanza.models.common.peft_config import build_peft_wrapper, load_peft_wrapper
 from stanza.models.depparse.model import Parser
 from stanza.models.pos.vocab import MultiVocab
 
 logger = logging.getLogger('stanza')
 
 def unpack_batch(batch, device):
     """ Unpack a batch from the data loader. """
@@ -55,15 +56,24 @@
                 self.global_step = 0
                 self.last_best_step = 0
                 self.dev_score_history = []
         else:
             # build model from scratch
             self.args = args
             self.vocab = vocab
-            self.model = Parser(args, vocab, emb_matrix=pretrain.emb if pretrain is not None else None)
+
+            bert_model, bert_tokenizer = load_bert(self.args['bert_model'])
+            peft_name = None
+            if self.args['use_peft']:
+                # fine tune the bert if we're using peft
+                self.args['bert_finetune'] = True
+                peft_name = "depparse"
+                bert_model = build_peft_wrapper(bert_model, self.args, logger, adapter_name=peft_name)
+
+            self.model = Parser(args, vocab, emb_matrix=pretrain.emb if pretrain is not None else None, foundation_cache=foundation_cache, bert_model=bert_model, bert_tokenizer=bert_tokenizer, force_bert_saved=self.args['bert_finetune'], peft_name=peft_name)
             self.model = self.model.to(device)
             self.__init_optim()
 
         if ignore_model_config:
             self.args = orig_args
 
         if self.args.get('wandb'):
@@ -112,17 +122,15 @@
 
         if eval:
             self.model.eval()
         else:
             self.model.train()
             for opt in self.optimizer.values():
                 opt.zero_grad()
-        # if there is no bert optimizer, we will tell the model to detach bert so it uses less GPU
-        detach = "bert_optimizer" not in self.optimizer
-        loss, _ = self.model(word, word_mask, wordchars, wordchars_mask, upos, xpos, ufeats, pretrained, lemma, head, deprel, word_orig_idx, sentlens, wordlens, text, detach=detach)
+        loss, _ = self.model(word, word_mask, wordchars, wordchars_mask, upos, xpos, ufeats, pretrained, lemma, head, deprel, word_orig_idx, sentlens, wordlens, text)
         loss_val = loss.data.item()
         if eval:
             return loss_val
 
         loss.backward()
         torch.nn.utils.clip_grad_norm_(self.model.parameters(), self.args['max_grad_norm'])
         for opt in self.optimizer.values():
@@ -161,15 +169,15 @@
                 'global_step': self.global_step,
                 'last_best_step': self.last_best_step,
                 'dev_score_history': self.dev_score_history,
                 }
         if self.args.get('use_peft', False):
             # Hide import so that peft dependency is optional
             from peft import get_peft_model_state_dict
-            params["bert_lora"] = get_peft_model_state_dict(self.model.bert_model)
+            params["bert_lora"] = get_peft_model_state_dict(self.model.bert_model, adapter_name=self.model.peft_name)
 
         if save_optimizer and self.optimizer is not None:
             params['optimizer_state_dict'] = {k: opt.state_dict() for k, opt in self.optimizer.items()}
             params['scheduler_state_dict'] = {k: scheduler.state_dict() for k, scheduler in self.scheduler.items()}
 
         try:
             torch.save(params, filename, _use_new_zipfile_serialization=False)
@@ -185,37 +193,48 @@
         try:
             checkpoint = torch.load(filename, lambda storage, loc: storage)
         except BaseException:
             logger.error("Cannot load model from {}".format(filename))
             raise
         self.args = checkpoint['config']
         if args is not None: self.args.update(args)
+
         # preserve old models which were created before transformers were added
         if 'bert_model' not in self.args:
             self.args['bert_model'] = None
+
+        lora_weights = checkpoint.get('bert_lora')
+        if lora_weights:
+            logger.debug("Found peft weights for depparse; loading a peft adapter")
+            self.args["use_peft"] = True
+
         self.vocab = MultiVocab.load_state_dict(checkpoint['vocab'])
         # load model
         emb_matrix = None
         if self.args['pretrain'] and pretrain is not None: # we use pretrain only if args['pretrain'] == True and pretrain is not None
             emb_matrix = pretrain.emb
-        if any(x.startswith("bert_model.") for x in checkpoint['model'].keys()):
-            logger.debug("Model %s has a finetuned transformer.  Not using transformer cache to make sure the finetuned version of the transformer isn't accidentally used elsewhere", filename)
-            foundation_cache = NoTransformerFoundationCache(foundation_cache)
-
-        # if we are set to not finetune bert, but there is an existing
-        # bert in the model, we need to respect that and force it to
-        # be resaved next time the model is saved
-        force_bert_saved = any(x.startswith("bert_model") for x in checkpoint['model'].keys())
 
-        self.model = Parser(self.args, self.vocab, emb_matrix=emb_matrix, foundation_cache=foundation_cache, force_bert_saved=force_bert_saved)
-        self.model.load_state_dict(checkpoint['model'], strict=False)
+        # TODO: refactor this common block of code with NER
+        force_bert_saved = False
+        peft_name = None
         if self.args.get('use_peft', False):
-            # hide import so that the peft dependency is optional
-            from peft import set_peft_model_state_dict
-            set_peft_model_state_dict(self.model.bert_model, checkpoint['bert_lora'])
+            force_bert_saved = True
+            bert_model, bert_tokenizer, peft_name = load_bert_with_peft(self.args['bert_model'], "depparse", foundation_cache)
+            bert_model = load_peft_wrapper(bert_model, lora_weights, self.args, logger, peft_name)
+            logger.debug("Loaded peft with name %s", peft_name)
+        else:
+            if any(x.startswith("bert_model.") for x in checkpoint['model'].keys()):
+                logger.debug("Model %s has a finetuned transformer.  Not using transformer cache to make sure the finetuned version of the transformer isn't accidentally used elsewhere", filename)
+                foundation_cache = NoTransformerFoundationCache(foundation_cache)
+                force_bert_saved = True
+            bert_model, bert_tokenizer = load_bert(self.args.get('bert_model'), foundation_cache)
+
+        self.model = Parser(self.args, self.vocab, emb_matrix=emb_matrix, foundation_cache=foundation_cache, bert_model=bert_model, bert_tokenizer=bert_tokenizer, force_bert_saved=force_bert_saved, peft_name=peft_name)
+        self.model.load_state_dict(checkpoint['model'], strict=False)
+
         if device is not None:
             self.model = self.model.to(device)
 
         self.__init_optim()
         optim_state_dict = checkpoint.get("optimizer_state_dict")
         if optim_state_dict:
             for k, state in optim_state_dict.items():
```

### Comparing `stanza-1.8.1/stanza/models/identity_lemmatizer.py` & `stanza-1.8.2/stanza/models/identity_lemmatizer.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/models/lang_identifier.py` & `stanza-1.8.2/stanza/models/lang_identifier.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/models/langid/create_ud_data.py` & `stanza-1.8.2/stanza/models/langid/create_ud_data.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/models/langid/data.py` & `stanza-1.8.2/stanza/models/langid/data.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/models/langid/model.py` & `stanza-1.8.2/stanza/models/langid/model.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/models/langid/trainer.py` & `stanza-1.8.2/stanza/models/langid/trainer.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/models/lemma/data.py` & `stanza-1.8.2/stanza/models/lemma/data.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/models/lemma/edit.py` & `stanza-1.8.2/stanza/models/lemma/edit.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/models/lemma/trainer.py` & `stanza-1.8.2/stanza/models/lemma/trainer.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/models/lemma/vocab.py` & `stanza-1.8.2/stanza/models/lemma/vocab.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/models/lemmatizer.py` & `stanza-1.8.2/stanza/models/lemmatizer.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/models/mwt/data.py` & `stanza-1.8.2/stanza/models/mwt/data.py`

 * *Files 3% similar despite different names*

```diff
@@ -60,44 +60,45 @@
             if self.eval:
                 tgt = src # as a placeholder
             else:
                 tgt = list(d[1])
             src = vocab.map(src)
             tgt_in = vocab.map([constant.SOS] + tgt)
             tgt_out = vocab.map(tgt + [constant.EOS])
-            processed += [[src, tgt_in, tgt_out]]
+            processed += [[src, tgt_in, tgt_out, d[0]]]
         return processed
 
     def __len__(self):
         return len(self.data)
 
     def __getitem__(self, key):
         """ Get a batch with index. """
         if not isinstance(key, int):
             raise TypeError
         if key < 0 or key >= len(self.data):
             raise IndexError
         batch = self.data[key]
         batch_size = len(batch)
         batch = list(zip(*batch))
-        assert len(batch) == 3
+        assert len(batch) == 4
 
         # sort all fields by lens for easy RNN operations
         lens = [len(x) for x in batch[0]]
         batch, orig_idx = sort_all(batch, lens)
 
         # convert to tensors
         src = batch[0]
         src = get_long_tensor(src, batch_size)
         src_mask = torch.eq(src, constant.PAD_ID)
         tgt_in = get_long_tensor(batch[1], batch_size)
         tgt_out = get_long_tensor(batch[2], batch_size)
+        orig_text = batch[3]
         assert tgt_in.size(1) == tgt_out.size(1), \
                 "Target input and output sequence sizes do not match."
-        return (src, src_mask, tgt_in, tgt_out, orig_idx)
+        return (src, src_mask, tgt_in, tgt_out, orig_text, orig_idx)
 
     def __iter__(self):
         for i in range(self.__len__()):
             yield self.__getitem__(i)
 
     def load_doc(self, doc, evaluation=False):
         data = doc.get_mwt_expansions(evaluation)
```

### Comparing `stanza-1.8.1/stanza/models/mwt/trainer.py` & `stanza-1.8.2/stanza/models/mwt/trainer.py`

 * *Files 23% similar despite different names*

```diff
@@ -17,16 +17,17 @@
 from stanza.models.mwt.vocab import Vocab
 
 logger = logging.getLogger('stanza')
 
 def unpack_batch(batch, device):
     """ Unpack a batch from the data loader. """
     inputs = [b.to(device) if b is not None else None for b in batch[:4]]
-    orig_idx = batch[4]
-    return inputs, orig_idx
+    orig_text = batch[4]
+    orig_idx = batch[5]
+    return inputs, orig_text, orig_idx
 
 class Trainer(BaseTrainer):
     """ A trainer for training models. """
     def __init__(self, args=None, vocab=None, emb_matrix=None, model_file=None, device=None):
         if model_file is not None:
             # load from file
             self.load(model_file)
@@ -38,15 +39,18 @@
         if not self.args['dict_only']:
             self.model = self.model.to(device)
             self.crit = loss.SequenceLoss(self.vocab.size).to(device)
             self.optimizer = utils.get_optimizer(self.args['optim'], self.model, self.args['lr'])
 
     def update(self, batch, eval=False):
         device = next(self.model.parameters()).device
-        inputs, orig_idx = unpack_batch(batch, device)
+        # ignore the original text when training
+        # can try to learn the correct values, even if we eventually
+        # copy directly from the original text
+        inputs, _, orig_idx = unpack_batch(batch, device)
         src, src_mask, tgt_in, tgt_out = inputs
 
         if eval:
             self.model.eval()
         else:
             self.model.train()
             self.optimizer.zero_grad()
@@ -59,23 +63,34 @@
         loss.backward()
         torch.nn.utils.clip_grad_norm_(self.model.parameters(), self.args['max_grad_norm'])
         self.optimizer.step()
         return loss_val
 
     def predict(self, batch, unsort=True):
         device = next(self.model.parameters()).device
-        inputs, orig_idx = unpack_batch(batch, device)
+        inputs, orig_text, orig_idx = unpack_batch(batch, device)
         src, src_mask, tgt, tgt_mask = inputs
 
         self.model.eval()
         batch_size = src.size(0)
         preds, _ = self.model.predict(src, src_mask, self.args['beam_size'])
         pred_seqs = [self.vocab.unmap(ids) for ids in preds] # unmap to tokens
         pred_seqs = utils.prune_decoded_seqs(pred_seqs)
-        pred_tokens = ["".join(seq) for seq in pred_seqs] # join chars to be tokens
+        if self.args.get('force_exact_pieces', False):
+            # TODO we should be able to do all this with numpy or something similar
+            pred_tokens = []
+            for pred_seq, text in zip(pred_seqs, orig_text):
+                pred_seq = np.array(list(pred_seq))
+                if sum(pred_seq != ' ') == len(text):
+                    pred_seq[pred_seq != ' '] = list(text)
+                    pred_tokens.append("".join(pred_seq))
+                else:
+                    pred_tokens.append("".join(pred_seq))
+        else:
+            pred_tokens = ["".join(seq) for seq in pred_seqs] # join chars to be tokens
         if unsort:
             pred_tokens = utils.unsort(pred_tokens, orig_idx)
         return pred_tokens
 
     def train_dict(self, pairs):
         """ Train a MWT expander given training word-expansion pairs. """
         # accumulate counter
@@ -86,37 +101,59 @@
         for p, _ in ctr.most_common():
             w, l = p
             if w not in seen and w != l:
                 self.expansion_dict[w] = l
             seen.add(w)
         return
 
+    def dict_expansion(self, word):
+        """
+        Check the expansion dictionary for the word along with a couple common lowercasings of the word
+
+        (Leadingcase and UPPERCASE)
+        """
+        expansion = self.expansion_dict.get(word)
+        if expansion is not None:
+            return expansion
+
+        if word.isupper():
+            expansion = self.expansion_dict.get(word.lower())
+            if expansion is not None:
+                return expansion.upper()
+
+        if word[0].isupper() and word[1:].islower():
+            expansion = self.expansion_dict.get(word.lower())
+            if expansion is not None:
+                return expansion[0].upper() + expansion[1:]
+
+        # could build a truecasing model of some kind to handle cRaZyCaSe...
+        # but that's probably too much effort
+        return None
+
     def predict_dict(self, words):
         """ Predict a list of expansions given words. """
         expansions = []
         for w in words:
-            if w in self.expansion_dict:
-                expansions += [self.expansion_dict[w]]
-            elif w.lower() in self.expansion_dict:
-                expansions += [self.expansion_dict[w.lower()]]
+            expansion = self.dict_expansion(w)
+            if expansion is not None:
+                expansions.append(expansion)
             else:
-                expansions += [w]
+                expansions.append(w)
         return expansions
 
     def ensemble(self, cands, other_preds):
         """ Ensemble the dict with statistical model predictions. """
         expansions = []
         assert len(cands) == len(other_preds)
         for c, pred in zip(cands, other_preds):
-            if c in self.expansion_dict:
-                expansions += [self.expansion_dict[c]]
-            elif c.lower() in self.expansion_dict:
-                expansions += [self.expansion_dict[c.lower()]]
+            expansion = self.dict_expansion(c)
+            if expansion is not None:
+                expansions.append(expansion)
             else:
-                expansions += [pred]
+                expansions.append(pred)
         return expansions
 
     def save(self, filename):
         params = {
                 'model': self.model.state_dict() if self.model is not None else None,
                 'dict': self.expansion_dict,
                 'vocab': self.vocab.state_dict(),
```

### Comparing `stanza-1.8.1/stanza/models/mwt/utils.py` & `stanza-1.8.2/stanza/models/mwt/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,26 @@
 import stanza
 
 from stanza.models.common import doc
 from stanza.models.tokenization.data import TokenizationDataset
 from stanza.models.tokenization.utils import predict, decode_predictions
 
+def mwts_composed_of_words(doc):
+    """
+    Return True/False if the MWTs in the doc are all exactly composed of the text in their words
+    """
+    for sent_idx, sentence in enumerate(doc.sentences):
+        for token_idx, token in enumerate(sentence.tokens):
+            if len(token.words) > 1:
+                expected = "".join(x.text for x in token.words)
+                if token.text != expected:
+                    return False
+    return True
+
+
 def resplit_mwt(tokens, pipeline, keep_tokens=True):
     """
     Uses the tokenize processor and the mwt processor in the pipeline to resplit tokens into MWT
 
     tokens: a list of list of string
     pipeline: a Stanza pipeline which contains, at a minimum, tokenize and mwt
```

### Comparing `stanza-1.8.1/stanza/models/mwt_expander.py` & `stanza-1.8.2/stanza/models/mwt_expander.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 import numpy as np
 import random
 import torch
 from torch import nn, optim
 import copy
 
 from stanza.models.mwt.data import DataLoader
+from stanza.models.mwt.utils import mwts_composed_of_words
 from stanza.models.mwt.vocab import Vocab
 from stanza.models.mwt.trainer import Trainer
 from stanza.models.mwt import scorer
 from stanza.models.common import utils
 import stanza.models.common.seq2seq_constant as constant
 from stanza.models.common.doc import Document
 from stanza.utils.conll import CoNLL
@@ -53,14 +54,17 @@
     parser.add_argument('--emb_dropout', type=float, default=0.5)
     parser.add_argument('--dropout', type=float, default=0.5)
     parser.add_argument('--max_dec_len', type=int, default=50)
     parser.add_argument('--beam_size', type=int, default=1)
     parser.add_argument('--attn_type', default='soft', choices=['soft', 'mlp', 'linear', 'deep'], help='Attention type')
     parser.add_argument('--no_copy', dest='copy', action='store_false', help='Do not use copy mechanism in MWT expansion. By default copy mechanism is used to improve generalization.')
 
+    parser.add_argument('--force_exact_pieces', default=None, action='store_true', help='If possible, make the text of the pieces of the MWT add up to the token itself.  (By default, this is determined from the dataset.)')
+    parser.add_argument('--no_force_exact_pieces', dest='force_exact_pieces', action='store_false', help="Don't make the text of the pieces of the MWT add up to the token itself.  (By default, this is determined from the dataset.)")
+
     parser.add_argument('--sample_train', type=float, default=1.0, help='Subsample training data.')
     parser.add_argument('--optim', type=str, default='adam', help='sgd, adagrad, adam or adamax.')
     parser.add_argument('--lr', type=float, default=1e-3, help='Learning rate')
     parser.add_argument('--lr_decay', type=float, default=0.9)
     parser.add_argument('--decay_epoch', type=int, default=30, help="Decay the lr starting from this epoch.")
     parser.add_argument('--num_epoch', type=int, default=30)
     parser.add_argument('--batch_size', type=int, default=50)
@@ -140,14 +144,17 @@
 
     if args.get('dict_only', False):
         # save dictionaries
         trainer.save(model_file)
     else:
         # train a seq2seq model
         logger.info("Training seq2seq-based MWT expander...")
+        if args['force_exact_pieces'] is None and mwts_composed_of_words(train_doc):
+            logger.info("Train MWTs entirely composed of their subwords.  Training the MWT to match that paradigm as closely as possible")
+            args['force_exact_pieces'] = True
         global_step = 0
         max_steps = len(train_batch) * args['num_epoch']
         dev_score_history = []
         best_dev_preds = []
         current_lr = args['lr']
         global_start_time = time.time()
         format_str = '{}: step {}/{} (epoch {}/{}), loss = {:.6f} ({:.3f} sec/batch), lr: {:.6f}'
```

### Comparing `stanza-1.8.1/stanza/models/ner/data.py` & `stanza-1.8.2/stanza/models/ner/data.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,16 @@
 from stanza.models.ner.vocab import MultiVocab
 from stanza.models.common.doc import *
 from stanza.models.ner.utils import process_tags, normalize_empty_tags
 
 logger = logging.getLogger('stanza')
 
 class DataLoader:
-    def __init__(self, doc, batch_size, args, pretrain=None, vocab=None, evaluation=False, preprocess_tags=True, bert_tokenizer=None, scheme=None):
+    def __init__(self, doc, batch_size, args, pretrain=None, vocab=None, evaluation=False, preprocess_tags=True, bert_tokenizer=None, scheme=None, max_batch_words=None):
+        self.max_batch_words = max_batch_words
         self.batch_size = batch_size
         self.args = args
         self.eval = evaluation
         self.shuffled = not self.eval
         self.doc = doc
         self.preprocess_tags = preprocess_tags
 
@@ -184,10 +185,22 @@
 
     def reshuffle(self):
         data = [y for x in self.data for y in x]
         random.shuffle(data)
         self.data = self.chunk_batches(data)
 
     def chunk_batches(self, data):
-        data = [data[i:i+self.batch_size] for i in range(0, len(data), self.batch_size)]
-        return data
-
+        if self.max_batch_words is None:
+            return [data[i:i+self.batch_size] for i in range(0, len(data), self.batch_size)]
+        batches = []
+        next_batch = []
+        for item in data:
+            next_batch.append(item)
+            if len(next_batch) >= self.batch_size:
+                batches.append(next_batch)
+                next_batch = []
+            if sum(len(x[0]) for x in next_batch) >= self.max_batch_words:
+                batches.append(next_batch)
+                next_batch = []
+        if len(next_batch) > 0:
+            batches.append(next_batch)
+        return batches
```

### Comparing `stanza-1.8.1/stanza/models/ner/model.py` & `stanza-1.8.2/stanza/models/ner/model.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,46 +10,45 @@
 from stanza.models.common.data import map_to_ids, get_long_tensor
 from stanza.models.common.exceptions import ForwardCharlmNotFoundError, BackwardCharlmNotFoundError
 from stanza.models.common.packed_lstm import PackedLSTM
 from stanza.models.common.dropout import WordDropout, LockedDropout
 from stanza.models.common.char_model import CharacterModel, CharacterLanguageModel
 from stanza.models.common.crf import CRFLoss
 from stanza.models.common.foundation_cache import load_bert
+from stanza.models.common.utils import attach_bert_model
 from stanza.models.common.vocab import PAD_ID, UNK_ID, EMPTY_ID
 from stanza.models.common.bert_embedding import extract_bert_embeddings
 
 logger = logging.getLogger('stanza')
 
+# this gets created in two places in trainer
+# in both places, pass in the bert model & tokenizer
 class NERTagger(nn.Module):
-    def __init__(self, args, vocab, emb_matrix=None, foundation_cache=None, force_bert_saved=False):
+    def __init__(self, args, vocab, emb_matrix=None, foundation_cache=None, bert_model=None, bert_tokenizer=None, force_bert_saved=False, peft_name=None):
         super().__init__()
 
         self.vocab = vocab
         self.args = args
         self.unsaved_modules = []
 
-        def add_unsaved_module(name, module):
-            self.unsaved_modules += [name]
-            setattr(self, name, module)
-
         # input layers
         input_size = 0
         if self.args['word_emb_dim'] > 0:
             emb_finetune = self.args.get('emb_finetune', True)
 
             # load pretrained embeddings if specified
             word_emb = nn.Embedding(len(self.vocab['word']), self.args['word_emb_dim'], PAD_ID)
             # if a model trained with no 'delta' vocab is loaded, and
             # emb_finetune is off, any resaving of the model will need
             # the updated vectors.  this is accounted for in load()
             if not emb_finetune or 'delta' in self.vocab:
                 # if emb_finetune is off
                 # or if the delta embedding is present
                 # then we won't fine tune the original embedding
-                add_unsaved_module('word_emb', word_emb)
+                self.add_unsaved_module('word_emb', word_emb)
                 self.word_emb.weight.detach_()
             else:
                 self.word_emb = word_emb
             if emb_matrix is not None:
                 self.init_emb(emb_matrix)
 
             # TODO: allow for expansion of delta embedding if new
@@ -64,56 +63,37 @@
                 # if the model was trained with a delta embedding, but emb_finetune is off now,
                 # then we will detach the delta embedding
                 if not emb_finetune:
                     self.delta_emb.weight.detach_()
 
             input_size += self.args['word_emb_dim']
 
-        # TODO: this, pos, depparse should all be refactored
-        # FIXME: possibly pos and depparse are all losing a finetuned transformer if loaded & saved
-        # (the force_bert_saved option here handles that)
+        self.peft_name = peft_name
+        attach_bert_model(self, bert_model, bert_tokenizer, self.args.get('use_peft', False), force_bert_saved)
         if self.args.get('bert_model', None):
+            # TODO: refactor bert_hidden_layers between the different models
             if args.get('bert_hidden_layers', False):
                 # The average will be offset by 1/N so that the default zeros
-                # repressents an average of the N layers
+                # represents an average of the N layers
                 self.bert_layer_mix = nn.Linear(args['bert_hidden_layers'], 1, bias=False)
                 nn.init.zeros_(self.bert_layer_mix.weight)
             else:
                 # an average of layers 2, 3, 4 will be used
                 # (for historic reasons)
                 self.bert_layer_mix = None
-            # first we load the transformer model and possibly turn off its requires_grad parameters ...
-            if self.args.get('bert_finetune', False):
-                bert_model, bert_tokenizer = load_bert(self.args['bert_model'])
-            else:
-                bert_model, bert_tokenizer = load_bert(self.args['bert_model'], foundation_cache)
-                for n, p in bert_model.named_parameters():
-                    p.requires_grad = False
-            # then we attach it to the NER model
-            # if force_bert_saved is True, that probably indicates the save file had a transformer in it
-            # thus we need to save it again in the future to avoid losing it when resaving
-            if self.args.get('bert_finetune', False) or force_bert_saved:
-                self.bert_model = bert_model
-                add_unsaved_module('bert_tokenizer', bert_tokenizer)
-            else:
-                add_unsaved_module('bert_model', bert_model)
-                add_unsaved_module('bert_tokenizer', bert_tokenizer)
             input_size += self.bert_model.config.hidden_size
-        else:
-            self.bert_model = None
-            self.bert_tokenizer = None
 
         if self.args['char'] and self.args['char_emb_dim'] > 0:
             if self.args['charlm']:
                 if args['charlm_forward_file'] is None or not os.path.exists(args['charlm_forward_file']):
                     raise ForwardCharlmNotFoundError('Could not find forward character model: {}  Please specify with --charlm_forward_file'.format(args['charlm_forward_file']), args['charlm_forward_file'])
                 if args['charlm_backward_file'] is None or not os.path.exists(args['charlm_backward_file']):
                     raise BackwardCharlmNotFoundError('Could not find backward character model: {}  Please specify with --charlm_backward_file'.format(args['charlm_backward_file']), args['charlm_backward_file'])
-                add_unsaved_module('charmodel_forward', CharacterLanguageModel.load(args['charlm_forward_file'], finetune=False))
-                add_unsaved_module('charmodel_backward', CharacterLanguageModel.load(args['charlm_backward_file'], finetune=False))
+                self.add_unsaved_module('charmodel_forward', CharacterLanguageModel.load(args['charlm_forward_file'], finetune=False))
+                self.add_unsaved_module('charmodel_backward', CharacterLanguageModel.load(args['charlm_backward_file'], finetune=False))
                 input_size += self.charmodel_forward.hidden_dim() + self.charmodel_backward.hidden_dim()
             else:
                 self.charmodel = CharacterModel(args, vocab, bidirectional=True, attention=False)
                 input_size += self.args['char_hidden_dim'] * 2
 
         # optionally add a input transformation layer
         if self.args.get('input_transform', False):
@@ -152,14 +132,18 @@
             emb_matrix = torch.from_numpy(emb_matrix)
         vocab_size = len(self.vocab['word'])
         dim = self.args['word_emb_dim']
         assert emb_matrix.size() == (vocab_size, dim), \
             "Input embedding matrix must match size: {} x {}, found {}".format(vocab_size, dim, emb_matrix.size())
         self.word_emb.weight.data.copy_(emb_matrix)
 
+    def add_unsaved_module(self, name, module):
+        self.unsaved_modules += [name]
+        setattr(self, name, module)
+
     def log_norms(self):
         lines = ["NORMS FOR MODEL PARAMTERS"]
         for name, param in self.named_parameters():
             if param.requires_grad and name.split(".")[0] not in ('charmodel_forward', 'charmodel_backward'):
                 lines.append("  %s %.6g" % (name, torch.norm(param).item()))
         logger.info("\n".join(lines))
 
@@ -204,15 +188,16 @@
             word_emb = pack(word_static_emb)
             inputs += [word_emb]
 
         if self.bert_model is not None:
             device = next(self.parameters()).device
             processed_bert = extract_bert_embeddings(self.args['bert_model'], self.bert_tokenizer, self.bert_model, sentences, device, keep_endpoints=False,
                                                      num_layers=self.bert_layer_mix.in_features if self.bert_layer_mix is not None else None,
-                                                     detach=not self.args.get('bert_finetune', False))
+                                                     detach=not self.args.get('bert_finetune', False),
+                                                     peft_name=self.peft_name)
             if self.bert_layer_mix is not None:
                 # use a linear layer to weighted average the embedding dynamically
                 processed_bert = [self.bert_layer_mix(feature).squeeze(2) + feature.sum(axis=2) / self.bert_layer_mix.in_features for feature in processed_bert]
 
             processed_bert = pad_sequence(processed_bert, batch_first=True)
             inputs += [pack(processed_bert)]
```

### Comparing `stanza-1.8.1/stanza/models/ner/scorer.py` & `stanza-1.8.2/stanza/models/ner/scorer.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/models/ner/trainer.py` & `stanza-1.8.2/stanza/models/ner/trainer.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 """
 
 import sys
 import logging
 import torch
 from torch import nn
 
-from stanza.models.common.foundation_cache import NoTransformerFoundationCache
+from stanza.models.common.foundation_cache import NoTransformerFoundationCache, load_bert, load_bert_with_peft
+from stanza.models.common.peft_config import build_peft_wrapper, load_peft_wrapper
 from stanza.models.common.trainer import Trainer as BaseTrainer
 from stanza.models.common.vocab import VOCAB_PREFIX, VOCAB_PREFIX_SIZE
 from stanza.models.common import utils, loss
 from stanza.models.ner.model import NERTagger
 from stanza.models.ner.vocab import MultiVocab
 from stanza.models.common.crf import viterbi_decode
 
-from stanza.models.common.peft_config import build_peft_wrapper
 
 logger = logging.getLogger('stanza')
 
 def unpack_batch(batch, device):
     """ Unpack a batch from the data loader. """
     inputs = [batch[0]]
     inputs += [b.to(device) if b is not None else None for b in batch[1:5]]
@@ -68,36 +68,31 @@
             # load everything from file
             self.load(model_file, pretrain, args, foundation_cache)
         else:
             assert all(var is not None for var in [args, vocab, pretrain])
             # build model from scratch
             self.args = args
             self.vocab = vocab
-            self.model = NERTagger(args, vocab, emb_matrix=pretrain.emb, foundation_cache=foundation_cache)
-
-            # PEFT the model, if needed
-            if self.args["use_peft"] and self.args["bert_model"]:
-                # fine tune the bert
-                self.args["bert_finetune"] = True
+            bert_model, bert_tokenizer = load_bert(self.args['bert_model'])
+            peft_name = None
+            if self.args['use_peft']:
+                # fine tune the bert if we're using peft
+                self.args['bert_finetune'] = True
+                peft_name = "ner"
                 # peft the lovely model
-                self.model.bert_model = build_peft_wrapper(self.model.bert_model,
-                                                           self.args, logger)
-                # because we will save this seperately ourselves within the trainer as PEFT
-                # weight loading is a tad different
-                self.model.unsaved_modules += ["bert_model"]
-                self.model.train()
-                self.model.bert_model.train()
+                bert_model = build_peft_wrapper(bert_model, self.args, logger, adapter_name=peft_name)
 
+            self.model = NERTagger(args, vocab, emb_matrix=pretrain.emb, foundation_cache=foundation_cache, bert_model=bert_model, bert_tokenizer=bert_tokenizer, force_bert_saved=self.args['bert_finetune'], peft_name=peft_name)
 
             # IMPORTANT: gradient checkpointing BREAKS peft if applied before
             # 1. Apply PEFT FIRST (looksie! it's above this line)
             # 2. Run gradient checkpointing
             # https://github.com/huggingface/peft/issues/742
             if self.args.get("gradient_checkpointing", False) and self.args.get("bert_finetune", False):
-                self.model.bert_model.gradient_checkpointing_enable()
+                self.model.bert_model.gradient_checkpointing_enable(gradient_checkpointing_kwargs={"use_reentrant": False})
 
 
         # if this wasn't set anywhere, we use a default of the 0th tagset
         # we don't set this as a default in the options so that
         # we can distinguish "intentionally set to 0" and "not set at all"
         if self.args.get('predict_tagset', None) is None:
             self.args['predict_tagset'] = 0
@@ -106,17 +101,17 @@
             logger.info('Disabling gradient for non-classifier layers')
             exclude = ['tag_clf', 'crit']
             for pname, p in self.model.named_parameters():
                 if pname.split('.')[0] not in exclude:
                     p.requires_grad = False
         self.model = self.model.to(device)
         if not second_optim:
-            self.optimizer = utils.get_optimizer(self.args['optim'], self.model, self.args['lr'], momentum=self.args['momentum'], bert_learning_rate=self.args.get('bert_learning_rate', 0.0), is_peft=bool(self.args.get("use_peft")))
+            self.optimizer = utils.get_optimizer(self.args['optim'], self.model, self.args['lr'], momentum=self.args['momentum'], bert_learning_rate=self.args.get('bert_learning_rate', 0.0), is_peft=self.args.get("use_peft"))
         else:
-            self.optimizer = utils.get_optimizer(self.args['second_optim'], self.model, self.args['second_lr'], momentum=self.args['momentum'], bert_learning_rate=self.args.get('second_bert_learning_rate', 0.0), is_peft=bool(self.args.get("use_peft")))
+            self.optimizer = utils.get_optimizer(self.args['second_optim'], self.model, self.args['second_lr'], momentum=self.args['momentum'], bert_learning_rate=self.args.get('second_bert_learning_rate', 0.0), is_peft=self.args.get("use_peft"))
 
     def update(self, batch, eval=False):
         device = next(self.model.parameters()).device
         inputs, orig_idx, word_orig_idx, char_orig_idx, sentlens, wordlens, charlens, charoffsets = unpack_batch(batch, device)
         word, wordchars, wordchars_mask, chars, tags = inputs
 
         if eval:
@@ -184,15 +179,15 @@
                 'model': model_state,
                 'vocab': self.vocab.state_dict(),
                 'config': self.args
                 }
 
         if self.args["use_peft"]:
             from peft import get_peft_model_state_dict
-            params["bert_lora"] = get_peft_model_state_dict(self.model.bert_model)
+            params["bert_lora"] = get_peft_model_state_dict(self.model.bert_model, adapter_name=self.model.peft_name)
         try:
             torch.save(params, filename, _use_new_zipfile_serialization=False)
             logger.info("Model saved to {}".format(filename))
         except (KeyboardInterrupt, SystemExit):
             raise
         except:
             logger.warning("Saving failed... continuing anyway.")
@@ -209,54 +204,56 @@
         # we use the value the model was trained with
         for keep_arg in ('predict_tagset', 'train_scheme', 'scheme'):
             if self.args.get(keep_arg, None) is None:
                 self.args[keep_arg] = checkpoint['config'].get(keep_arg, None)
 
         lora_weights = checkpoint.get('bert_lora')
         if lora_weights:
+            logger.debug("Found peft weights for NER; loading a peft adapter")
             self.args["use_peft"] = True
 
         self.vocab = MultiVocab.load_state_dict(checkpoint['vocab'])
 
         emb_matrix=None
         if pretrain is not None:
             emb_matrix = pretrain.emb
 
         force_bert_saved = False
-        if any(x.startswith("bert_model.") for x in checkpoint['model'].keys()):
-            logger.debug("Model %s has a finetuned transformer.  Not using transformer cache to make sure the finetuned version of the transformer isn't accidentally used elsewhere", filename)
-            foundation_cache = NoTransformerFoundationCache(foundation_cache)
+        peft_name = None
+        if self.args.get('use_peft', False):
             force_bert_saved = True
+            bert_model, bert_tokenizer, peft_name = load_bert_with_peft(self.args['bert_model'], "ner", foundation_cache)
+            bert_model = load_peft_wrapper(bert_model, lora_weights, self.args, logger, peft_name)
+            logger.debug("Loaded peft with name %s", peft_name)
+        else:
+            if any(x.startswith("bert_model.") for x in checkpoint['model'].keys()):
+                logger.debug("Model %s has a finetuned transformer.  Not using transformer cache to make sure the finetuned version of the transformer isn't accidentally used elsewhere", filename)
+                foundation_cache = NoTransformerFoundationCache(foundation_cache)
+                force_bert_saved = True
+            bert_model, bert_tokenizer = load_bert(self.args.get('bert_model'), foundation_cache)
+
         if any(x.startswith("crit.") for x in checkpoint['model'].keys()):
             logger.debug("Old model format detected.  Updating to the new format with one column of tags")
             checkpoint['model']['crits.0._transitions'] = checkpoint['model'].pop('crit._transitions')
             checkpoint['model']['tag_clfs.0.weight'] = checkpoint['model'].pop('tag_clf.weight')
             checkpoint['model']['tag_clfs.0.bias'] = checkpoint['model'].pop('tag_clf.bias')
-        self.model = NERTagger(self.args, self.vocab, emb_matrix=emb_matrix, foundation_cache=foundation_cache, force_bert_saved=force_bert_saved)
+        self.model = NERTagger(self.args, self.vocab, emb_matrix=emb_matrix, foundation_cache=foundation_cache, bert_model=bert_model, bert_tokenizer=bert_tokenizer, force_bert_saved=force_bert_saved, peft_name=peft_name)
         self.model.load_state_dict(checkpoint['model'], strict=False)
 
         # there is a possible issue with the delta embeddings.
         # specifically, with older models trained without the delta
         # embedding matrix
         # if those models have been trained with the embedding
         # modifications saved as part of the base embedding,
         # we need to resave the model with the updated embedding
         # otherwise the resulting model will be broken
         if 'delta' not in self.model.vocab and 'word_emb.weight' in checkpoint['model'].keys() and 'word_emb' in self.model.unsaved_modules:
             logger.debug("Removing word_emb from unsaved_modules so that resaving %s will keep the saved embedding", filename)
             self.model.unsaved_modules.remove('word_emb')
 
-        # load lora weights, which is special
-        if lora_weights:
-            from peft import set_peft_model_state_dict
-            self.model.bert_model = build_peft_wrapper(self.model.bert_model,
-                                                       self.args, logger)
-            self.model.unsaved_modules += ["bert_model"]
-            set_peft_model_state_dict(self.model.bert_model, lora_weights)
-
     def get_known_tags(self):
         """
         Return the tags known by this model
 
         Removes the S-, B-, etc, and does not include O
         """
         tags = set()
```

### Comparing `stanza-1.8.1/stanza/models/ner/utils.py` & `stanza-1.8.2/stanza/models/ner/utils.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/models/ner/vocab.py` & `stanza-1.8.2/stanza/models/ner/vocab.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/models/ner_tagger.py` & `stanza-1.8.2/stanza/models/ner_tagger.py`

 * *Files 3% similar despite different names*

```diff
@@ -101,14 +101,15 @@
 
     parser.add_argument('--ignore_tag_scores', type=str, default=None, help="Which tags to ignore, if any, when scoring dev & test sets")
 
     parser.add_argument('--max_steps', type=int, default=200000)
     parser.add_argument('--max_steps_no_improve', type=int, default=2500, help='if the model doesn\'t improve after this many steps, give up or switch to new optimizer.')
     parser.add_argument('--eval_interval', type=int, default=500)
     parser.add_argument('--batch_size', type=int, default=32)
+    parser.add_argument('--max_batch_words', type=int, default=800, help='Long sentences can overwhelm even a large GPU when finetuning a transformer on otherwise reasonable batch sizes.  This cuts off those batches early')
     parser.add_argument('--max_grad_norm', type=float, default=5.0, help='Gradient clipping.')
     parser.add_argument('--log_step', type=int, default=20, help='Print log every k steps.')
     parser.add_argument('--log_norms', action='store_true', default=False, help='Log the norms of all the parameters (noisy!)')
     parser.add_argument('--save_dir', type=str, default='saved_models/ner', help='Root dir for saving models.')
     parser.add_argument('--save_name', type=str, default="{shorthand}_{embedding}_{finetune}_nertagger.pt", help="File name to save the model")
 
     parser.add_argument('--seed', type=int, default=1234)
@@ -245,15 +246,15 @@
     # load data
     logger.info("Loading training data with batch size %d from %s", args['batch_size'], args['train_file'])
     with open(args['train_file']) as fin:
         train_doc = Document(json.load(fin))
     logger.info("Loaded %d sentences of training data", len(train_doc.sentences))
     if len(train_doc.sentences) == 0:
         raise ValueError("File %s exists but has no usable training data" % args['train_file'])
-    train_batch = DataLoader(train_doc, args['batch_size'], args, pretrain, vocab=vocab, evaluation=False, scheme=args.get('train_scheme'))
+    train_batch = DataLoader(train_doc, args['batch_size'], args, pretrain, vocab=vocab, evaluation=False, scheme=args.get('train_scheme'), max_batch_words=args['max_batch_words'])
     vocab = train_batch.vocab
     logger.info("Loading dev data from %s", args['eval_file'])
     with open(args['eval_file']) as fin:
         dev_doc = Document(json.load(fin))
     logger.info("Loaded %d sentences of dev data", len(dev_doc.sentences))
     if len(dev_doc.sentences) == 0:
         raise ValueError("File %s exists but has no usable dev data" % args['train_file'])
@@ -326,17 +327,14 @@
             global_step += 1
             loss = trainer.update(batch, eval=False) # update step
             train_loss += loss
             if global_step % args['log_step'] == 0:
                 duration = time.time() - start_time
                 logger.info(format_str.format(datetime.now().strftime("%Y-%m-%d %H:%M:%S"), global_step,
                                               max_steps, loss, duration, current_lr))
-                if args['log_norms']:
-                    trainer.model.log_norms()
-
             if global_step % args['eval_interval'] == 0:
                 # eval on dev
                 logger.info("Evaluating on dev set...")
                 dev_preds = []
                 for batch in dev_batch:
                     preds = trainer.predict(batch)
                     dev_preds += preds
@@ -358,14 +356,17 @@
                 dev_score_history += [dev_score]
                 logger.info("")
 
                 # lr schedule
                 if scheduler is not None:
                     scheduler.step(dev_score)
             
+                if args['log_norms']:
+                    trainer.model.log_norms()
+
             # check stopping
             current_lr = trainer.optimizer.param_groups[0]['lr']
             if (global_step - last_best_step) >= args['max_steps_no_improve'] or global_step >= args['max_steps'] or current_lr <= args['min_lr']:
                 if (global_step - last_best_step) >= args['max_steps_no_improve']:
                     logger.info("{} steps without improvement...".format((global_step - last_best_step)))
                 if not is_second_optim and args['second_optim'] is not None:
                     logger.info("Switching to second optimizer: {}".format(args['second_optim']))
@@ -419,45 +420,52 @@
                 fout.write("\n")
 
 def evaluate(args):
     # file paths
     model_file = model_file_name(args)
 
     loaded_args, trainer, vocab = load_model(args, model_file)
+    return evaluate_model(loaded_args, trainer, vocab, args['eval_file'])
+
+def evaluate_model(loaded_args, trainer, vocab, eval_file):
+    if loaded_args['log_norms']:
+        trainer.model.log_norms()
+
+    model_file = os.path.join(loaded_args['save_dir'], loaded_args['save_name'])
     logger.debug("Loaded model for eval from %s", model_file)
     logger.debug("Using the %d tagset for evaluation", loaded_args['predict_tagset'])
 
     # load data
-    logger.info("Loading data with batch size {}...".format(args['batch_size']))
-    with open(args['eval_file']) as fin:
+    logger.info("Loading data with batch size {}...".format(loaded_args['batch_size']))
+    with open(eval_file) as fin:
         doc = Document(json.load(fin))
-    batch = DataLoader(doc, args['batch_size'], loaded_args, vocab=vocab, evaluation=True, bert_tokenizer=trainer.model.bert_tokenizer)
+    batch = DataLoader(doc, loaded_args['batch_size'], loaded_args, vocab=vocab, evaluation=True, bert_tokenizer=trainer.model.bert_tokenizer)
     bioes_to_bio = loaded_args['train_scheme'] == 'bio' and loaded_args['scheme'] == 'bioes'
     warn_missing_tags(trainer.vocab['tag'], batch.tags, "eval_file", bioes_to_bio=bioes_to_bio)
 
     logger.info("Start evaluation...")
     preds = []
     for i, b in enumerate(batch):
         preds += trainer.predict(b)
 
     gold_tags = batch.tags
     # TODO: might still want to add multiple layers of tag evaluation to the scorer
     gold_tags = [[x[trainer.args['predict_tagset']] for x in tags] for tags in gold_tags]
 
-    _, _, score, entity_f1 = scorer.score_by_entity(preds, gold_tags, ignore_tags=args['ignore_tag_scores'])
-    _, _, _, confusion = scorer.score_by_token(preds, gold_tags, ignore_tags=args['ignore_tag_scores'])
+    _, _, score, entity_f1 = scorer.score_by_entity(preds, gold_tags, ignore_tags=loaded_args['ignore_tag_scores'])
+    _, _, _, confusion = scorer.score_by_token(preds, gold_tags, ignore_tags=loaded_args['ignore_tag_scores'])
     logger.info("Weighted f1 for non-O tokens: %5f", confusion_to_weighted_f1(confusion, exclude=["O"]))
 
-    logger.info("NER tagger score: %s %s %s %.2f", args['shorthand'], model_file, args['eval_file'], score*100)
+    logger.info("NER tagger score: %s %s %s %.2f", loaded_args['shorthand'], model_file, eval_file, score*100)
     entity_f1_lines = ["%s: %.2f" % (x, y*100) for x, y in entity_f1.items()]
     logger.info("NER Entity F1 scores:\n  %s", "\n  ".join(entity_f1_lines))
     logger.info("NER token confusion matrix:\n{}".format(format_confusion(confusion)))
 
-    if args['eval_output_file']:
-        write_ner_results(args['eval_output_file'], batch, preds, trainer.args['predict_tagset'])
+    if loaded_args['eval_output_file']:
+        write_ner_results(loaded_args['eval_output_file'], batch, preds, trainer.args['predict_tagset'])
 
     return confusion
 
 def load_model(args, model_file):
     # load model
     charlm_args = {}
     if 'charlm_forward_file' in args:
@@ -468,14 +476,17 @@
         charlm_args['predict_tagset'] = args['predict_tagset']
     pretrain = load_pretrain(args)
     trainer = Trainer(args=charlm_args, model_file=model_file, pretrain=pretrain, device=args['device'], train_classifier_only=args['train_classifier_only'])
     loaded_args, vocab = trainer.args, trainer.vocab
 
     # load config
     for k in args:
-        if k.endswith('_dir') or k.endswith('_file') or k in ['shorthand', 'mode', 'scheme']:
+        if k.endswith('_dir') or k.endswith('_file') or k in ['batch_size', 'ignore_tag_scores', 'log_norms', 'mode', 'scheme', 'shorthand']:
             loaded_args[k] = args[k]
+    save_dir, save_name = os.path.split(model_file)
+    args['save_dir'] = save_dir
+    args['save_name'] = save_name
     return loaded_args, trainer, vocab
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `stanza-1.8.1/stanza/models/parser.py` & `stanza-1.8.2/stanza/models/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,26 +40,29 @@
     parser.add_argument('--data_dir', type=str, default='data/depparse', help='Root dir for saving models.')
     parser.add_argument('--wordvec_dir', type=str, default='extern_data/word2vec', help='Directory of word vectors.')
     parser.add_argument('--wordvec_file', type=str, default=None, help='Word vectors filename.')
     parser.add_argument('--wordvec_pretrain_file', type=str, default=None, help='Exact name of the pretrain file to read')
     parser.add_argument('--train_file', type=str, default=None, help='Input file for data loader.')
     parser.add_argument('--eval_file', type=str, default=None, help='Input file for data loader.')
     parser.add_argument('--output_file', type=str, default=None, help='Output CoNLL-U file.')
-    parser.add_argument('--gold_file', type=str, default=None, help='Output CoNLL-U file.')
+    parser.add_argument('--no_gold_labels', dest='gold_labels', action='store_false', help="Don't score the eval file - perhaps it has no gold labels, for example.  Cannot be used at training time")
     parser.add_argument('--mode', default='train', choices=['train', 'predict'])
     parser.add_argument('--lang', type=str, help='Language')
     parser.add_argument('--shorthand', type=str, help="Treebank shorthand")
 
     parser.add_argument('--hidden_dim', type=int, default=400)
     parser.add_argument('--char_hidden_dim', type=int, default=400)
     parser.add_argument('--deep_biaff_hidden_dim', type=int, default=400)
     parser.add_argument('--composite_deep_biaff_hidden_dim', type=int, default=100)
     parser.add_argument('--word_emb_dim', type=int, default=75)
     parser.add_argument('--char_emb_dim', type=int, default=100)
     parser.add_argument('--tag_emb_dim', type=int, default=50)
+    parser.add_argument('--no_upos', dest='use_upos', action='store_false', default=True, help="Don't use upos tags as part of the tag embedding")
+    parser.add_argument('--no_xpos', dest='use_xpos', action='store_false', default=True, help="Don't use xpos tags as part of the tag embedding")
+    parser.add_argument('--no_ufeats', dest='use_ufeats', action='store_false', default=True, help="Don't use ufeats as part of the tag embedding")
     parser.add_argument('--transformed_dim', type=int, default=125)
     parser.add_argument('--num_layers', type=int, default=3)
     parser.add_argument('--char_num_layers', type=int, default=1)
     parser.add_argument('--checkpoint_save_name', type=str, default=None, help="File name to save the most recent checkpoint")
     parser.add_argument('--no_checkpoint', dest='checkpoint', action='store_false', help="Don't save checkpoints")
     parser.add_argument('--pretrain_max_vocab', type=int, default=250000)
     parser.add_argument('--word_dropout', type=float, default=0.33)
@@ -199,17 +202,16 @@
     logger.info("Augmented data size: {}".format(len(train_data)))
     train_doc = Document(train_data)
     train_batch = DataLoader(train_doc, args['batch_size'], args, pretrain, evaluation=False)
     vocab = train_batch.vocab
     dev_doc = CoNLL.conll2doc(input_file=args['eval_file'])
     dev_batch = DataLoader(dev_doc, args['batch_size'], args, pretrain, vocab=vocab, evaluation=True, sort_during_eval=True)
 
-    # pred and gold path
+    # pred path
     system_pred_file = args['output_file']
-    gold_file = args['gold_file']
 
     # skip training if the language does not have training or dev data
     if len(train_batch) == 0 or len(dev_batch) == 0:
         logger.info("Skip training because no data available...")
         sys.exit(0)
 
     if args['wandb']:
@@ -264,15 +266,15 @@
             if trainer.global_step % args['eval_interval'] == 0:
                 # eval on dev
                 logger.info("Evaluating on dev set...")
                 dev_preds = predict_dataset(trainer, dev_batch)
 
                 dev_batch.doc.set([HEAD, DEPREL], [y for x in dev_preds for y in x])
                 CoNLL.write_doc2conll(dev_batch.doc, system_pred_file)
-                _, _, dev_score = scorer.score(system_pred_file, gold_file)
+                _, _, dev_score = scorer.score(system_pred_file, args['eval_file'])
 
                 train_loss = train_loss / args['eval_interval'] # avg loss per batch
                 logger.info("step {}: train_loss = {:.6f}, dev_score = {:.4f}".format(trainer.global_step, train_loss, dev_score))
 
                 if args['wandb']:
                     wandb.log({'train_loss': train_loss, 'dev_score': dev_score})
 
@@ -301,15 +303,15 @@
                     trainer = Trainer(args=args, vocab=trainer.vocab, pretrain=pretrain,
                                       model_file=model_file, device=args['device'])
                     logger.info('Reloading best model to continue from current local optimum')
 
                     dev_preds = predict_dataset(trainer, dev_batch)
                     dev_batch.doc.set([HEAD, DEPREL], [y for x in dev_preds for y in x])
                     CoNLL.write_doc2conll(dev_batch.doc, system_pred_file)
-                    _, _, dev_score = scorer.score(system_pred_file, gold_file)
+                    _, _, dev_score = scorer.score(system_pred_file, args['eval_file'])
                     logger.info("Reloaded model with dev score %.4f", dev_score)
 
                     is_second_stage = True
                     trainer.global_step = global_step
                     trainer.last_best_step = global_step
                     if args['second_batch_size'] is not None:
                         train_batch.set_batch_size(args['second_batch_size'])
@@ -349,28 +351,28 @@
     else:
         logger.info("Dev set never evaluated.  Saving final model.")
         trainer.save(model_file)
 
     return trainer
 
 def evaluate(args):
-    # file paths
-    system_pred_file = args['output_file']
-    gold_file = args['gold_file']
-
     model_file = model_file_name(args)
     # load pretrained vectors if needed
     pretrain = load_pretrain(args)
 
     load_args = {'charlm_forward_file': args.get('charlm_forward_file', None),
                  'charlm_backward_file': args.get('charlm_backward_file', None)}
 
     # load model
     logger.info("Loading model from: {}".format(model_file))
     trainer = Trainer(pretrain=pretrain, model_file=model_file, device=args['device'], args=load_args)
+    return evaluate_trainer(args, trainer, pretrain)
+
+def evaluate_trainer(args, trainer, pretrain):
+    system_pred_file = args['output_file']
     loaded_args, vocab = trainer.args, trainer.vocab
 
     # load config
     for k in args:
         if k.endswith('_dir') or k.endswith('_file') or k in ['shorthand'] or k == 'mode':
             loaded_args[k] = args[k]
 
@@ -381,18 +383,24 @@
 
     preds = predict_dataset(trainer, batch)
 
     # write to file and score
     batch.doc.set([HEAD, DEPREL], [y for x in preds for y in x])
     CoNLL.write_doc2conll(batch.doc, system_pred_file)
 
-    if gold_file is not None:
-        gold_doc = CoNLL.conll2doc(input_file=gold_file)
+    if args['gold_labels']:
+        gold_doc = CoNLL.conll2doc(input_file=args['eval_file'])
+
+        # Check for None ... otherwise an inscrutable error occurs later in the scorer
+        for sent_idx, sentence in enumerate(gold_doc.sentences):
+            for word_idx, word in enumerate(sentence.words):
+                if word.deprel is None:
+                    raise ValueError("Gold document {} has a None at sentence {} word {}\n{:C}".format(args['eval_file'], sent_idx, word_idx, sentence))
 
         scorer.score_named_dependencies(batch.doc, gold_doc)
-        _, _, score = scorer.score(system_pred_file, gold_file)
+        _, _, score = scorer.score(system_pred_file, args['eval_file'])
 
         logger.info("Parser score:")
         logger.info("{} {:.2f}".format(args['shorthand'], score*100))
 
 if __name__ == '__main__':
     main()
```

### Comparing `stanza-1.8.1/stanza/models/pos/build_xpos_vocab_factory.py` & `stanza-1.8.2/stanza/models/pos/build_xpos_vocab_factory.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/models/pos/data.py` & `stanza-1.8.2/stanza/models/pos/data.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import random
 import logging
 import copy
 import torch
 from collections import namedtuple
 
 from torch.utils.data import DataLoader as DL
+from torch.utils.data.sampler import Sampler
 from torch.nn.utils.rnn import pad_sequence
 
 from stanza.models.common.bert_embedding import filter_data
 from stanza.models.common.data import map_to_ids, get_long_tensor, get_float_tensor, sort_all
 from stanza.models.common.vocab import PAD_ID, VOCAB_PREFIX, CharVocab
 from stanza.models.pos.vocab import WordVocab, XPOSVocab, FeatureVocab, MultiVocab
 from stanza.models.pos.xpos_vocab_factory import xpos_vocab_factory
@@ -217,14 +218,20 @@
     def to_loader(self, **kwargs):
         """Converts self to a DataLoader """
 
         return DL(self,
                   collate_fn=Dataset.__collate_fn,
                   **kwargs)
 
+    def to_length_limited_loader(self, batch_size, maximum_tokens):
+        sampler = LengthLimitedBatchSampler(self, batch_size, maximum_tokens)
+        return DL(self,
+                  collate_fn=Dataset.__collate_fn,
+                  batch_sampler = sampler)
+
     @staticmethod
     def __collate_fn(data):
         """Function used by DataLoader to pack data"""
         (data, idx) = zip(*data)
         (words, wordchars, upos, xpos, ufeats, pretrained, text) = zip(*data)
 
         # collate_fn is given a list of length batch size
@@ -279,14 +286,65 @@
         for sent_idx in range(len(data)):
             for tok_idx in range(len(data[sent_idx])):
                 for feat_idx in range(len(data[sent_idx][tok_idx])):
                     if data[sent_idx][tok_idx][feat_idx] is None:
                         data[sent_idx][tok_idx][feat_idx] = '_'
         return data
 
+class LengthLimitedBatchSampler(Sampler):
+    """
+    Batches up the text in batches of batch_size, but cuts off each time a batch reaches maximum_tokens
+
+    Intent is to avoid GPU OOM in situations where one sentence is significantly longer than expected,
+    leaving a batch too large to fit in the GPU
+
+    Sentences which are longer than maximum_tokens by themselves are put in their own batches
+    """
+    def __init__(self, data, batch_size, maximum_tokens):
+        """
+        Precalculate the batches, making it so len and iter just read off the precalculated batches
+        """
+        self.data = data
+        self.batch_size = batch_size
+        self.maximum_tokens = maximum_tokens
+
+        self.batches = []
+        current_batch = []
+        current_length = 0
+
+        for item, item_idx in data:
+            item_len = len(item.word)
+            if maximum_tokens and item_len > maximum_tokens:
+                if len(current_batch) > 0:
+                    self.batches.append(current_batch)
+                    current_batch = []
+                    current_length = 0
+                self.batches.append([item_idx])
+                continue
+            if len(current_batch) + 1 > batch_size or (maximum_tokens and item_len + current_length > maximum_tokens):
+                self.batches.append(current_batch)
+                current_batch = []
+                current_length = 0
+            current_batch.append(item_idx)
+            current_length += item_len
+
+        if len(current_batch) > 0:
+            self.batches.append(current_batch)
+
+    def __len__(self):
+        return len(self.batches)
+
+    def __iter__(self):
+        for batch in self.batches:
+            current_batch = []
+            for idx in batch:
+                current_batch.append(idx)
+            yield current_batch
+
+
 class ShuffledDataset:
     """A wrapper around one or more datasets which shuffles the data in batch_size chunks
 
     This means that if multiple datasets are passed in, the batches
     from each dataset are shuffled together, with one batch being
     entirely members of the same dataset.
```

### Comparing `stanza-1.8.1/stanza/models/pos/model.py` & `stanza-1.8.2/stanza/models/pos/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,33 +8,30 @@
 from torch.nn.utils.rnn import pad_packed_sequence, pack_padded_sequence, pack_sequence, pad_sequence, PackedSequence
 
 from stanza.models.common.bert_embedding import extract_bert_embeddings
 from stanza.models.common.biaffine import BiaffineScorer
 from stanza.models.common.foundation_cache import load_bert, load_charlm
 from stanza.models.common.hlstm import HighwayLSTM
 from stanza.models.common.dropout import WordDropout
+from stanza.models.common.utils import attach_bert_model
 from stanza.models.common.vocab import CompositeVocab
 from stanza.models.common.char_model import CharacterModel
 from stanza.models.common import utils
 
 logger = logging.getLogger('stanza')
 
 class Tagger(nn.Module):
-    def __init__(self, args, vocab, emb_matrix=None, share_hid=False, foundation_cache=None):
+    def __init__(self, args, vocab, emb_matrix=None, share_hid=False, foundation_cache=None, bert_model=None, bert_tokenizer=None, force_bert_saved=False, peft_name=None):
         super().__init__()
 
         self.vocab = vocab
         self.args = args
         self.share_hid = share_hid
         self.unsaved_modules = []
 
-        def add_unsaved_module(name, module):
-            self.unsaved_modules += [name]
-            setattr(self, name, module)
-
         # input layers
         input_size = 0
         if self.args['word_emb_dim'] > 0:
             # frequent word embeddings
             self.word_emb = nn.Embedding(len(vocab['word']), self.args['word_emb_dim'], padding_idx=0)
             input_size += self.args['word_emb_dim']
 
@@ -45,16 +42,16 @@
         if self.args['char'] and self.args['char_emb_dim'] > 0:
             if self.args.get('charlm', None):
                 if args['charlm_forward_file'] is None or not os.path.exists(args['charlm_forward_file']):
                     raise FileNotFoundError('Could not find forward character model: {}  Please specify with --charlm_forward_file'.format(args['charlm_forward_file']))
                 if args['charlm_backward_file'] is None or not os.path.exists(args['charlm_backward_file']):
                     raise FileNotFoundError('Could not find backward character model: {}  Please specify with --charlm_backward_file'.format(args['charlm_backward_file']))
                 logger.debug("POS model loading charmodels: %s and %s", args['charlm_forward_file'], args['charlm_backward_file'])
-                add_unsaved_module('charmodel_forward', load_charlm(args['charlm_forward_file'], foundation_cache=foundation_cache))
-                add_unsaved_module('charmodel_backward', load_charlm(args['charlm_backward_file'], foundation_cache=foundation_cache))
+                self.add_unsaved_module('charmodel_forward', load_charlm(args['charlm_forward_file'], foundation_cache=foundation_cache))
+                self.add_unsaved_module('charmodel_backward', load_charlm(args['charlm_backward_file'], foundation_cache=foundation_cache))
                 # optionally add a input transformation layer
                 if self.args.get('charlm_transform_dim', 0):
                     self.charmodel_forward_transform = nn.Linear(self.charmodel_forward.hidden_dim(), self.args['charlm_transform_dim'], bias=False)
                     self.charmodel_backward_transform = nn.Linear(self.charmodel_backward.hidden_dim(), self.args['charlm_transform_dim'], bias=False)
                     input_size += self.args['charlm_transform_dim'] * 2
                 else:
                     self.charmodel_forward_transform = None
@@ -65,42 +62,32 @@
                 self.charmodel = CharacterModel(args, vocab, bidirectional=bidirectional)
                 if bidirectional:
                     self.trans_char = nn.Linear(self.args['char_hidden_dim'] * 2, self.args['transformed_dim'], bias=False)
                 else:
                     self.trans_char = nn.Linear(self.args['char_hidden_dim'], self.args['transformed_dim'], bias=False)
                 input_size += self.args['transformed_dim']
 
-        if self.args['bert_model']:
+        self.peft_name = peft_name
+        attach_bert_model(self, bert_model, bert_tokenizer, self.args.get('use_peft', False), force_bert_saved)
+        if self.args.get('bert_model', None):
+            # TODO: refactor bert_hidden_layers between the different models
             if args.get('bert_hidden_layers', False):
                 # The average will be offset by 1/N so that the default zeros
-                # repressents an average of the N layers
+                # represents an average of the N layers
                 self.bert_layer_mix = nn.Linear(args['bert_hidden_layers'], 1, bias=False)
                 nn.init.zeros_(self.bert_layer_mix.weight)
             else:
                 # an average of layers 2, 3, 4 will be used
                 # (for historic reasons)
                 self.bert_layer_mix = None
-            if self.args.get('bert_finetune', False):
-                bert_model, bert_tokenizer = load_bert(self.args['bert_model'])
-                self.bert_model = bert_model
-                add_unsaved_module('bert_tokenizer', bert_tokenizer)
-            else:
-                bert_model, bert_tokenizer = load_bert(self.args['bert_model'], foundation_cache)
-                for n, p in bert_model.named_parameters():
-                    p.requires_grad = False
-                add_unsaved_module('bert_model', bert_model)
-                add_unsaved_module('bert_tokenizer', bert_tokenizer)
-            input_size += bert_model.config.hidden_size
-        else:
-            self.bert_model = None
-            self.bert_tokenizer = None
+            input_size += self.bert_model.config.hidden_size
 
         if self.args['pretrain']:
             # pretrained embeddings, by default this won't be saved into model file
-            add_unsaved_module('pretrained_emb', nn.Embedding.from_pretrained(torch.from_numpy(emb_matrix), freeze=True))
+            self.add_unsaved_module('pretrained_emb', nn.Embedding.from_pretrained(torch.from_numpy(emb_matrix), freeze=True))
             self.trans_pretrained = nn.Linear(emb_matrix.shape[1], self.args['transformed_dim'], bias=False)
             input_size += self.args['transformed_dim']
         
         # recurrent layers
         self.taggerlstm = HighwayLSTM(input_size, self.args['hidden_dim'], self.args['num_layers'], batch_first=True, bidirectional=True, dropout=self.args['dropout'], rec_dropout=self.args['rec_dropout'], highway_func=torch.tanh)
         self.drop_replacement = nn.Parameter(torch.randn(input_size) / np.sqrt(input_size))
         self.taggerlstm_h_init = nn.Parameter(torch.zeros(2 * self.args['num_layers'], 1, self.args['hidden_dim']))
@@ -140,14 +127,18 @@
 
         # criterion
         self.crit = nn.CrossEntropyLoss(ignore_index=0) # ignore padding
 
         self.drop = nn.Dropout(args['dropout'])
         self.worddrop = WordDropout(args['word_dropout'])
 
+    def add_unsaved_module(self, name, module):
+        self.unsaved_modules += [name]
+        setattr(self, name, module)
+
     def log_norms(self):
         utils.log_norms(self)
 
     def forward(self, word, word_mask, wordchars, wordchars_mask, upos, xpos, ufeats, pretrained, word_orig_idx, sentlens, wordlens, text):
         
         def pack(x):
             return pack_padded_sequence(x, sentlens, batch_first=True)
@@ -186,15 +177,16 @@
                 char_reps = PackedSequence(self.trans_char(self.drop(char_reps.data)), char_reps.batch_sizes)
                 inputs += [char_reps]
 
         if self.bert_model is not None:
             device = next(self.parameters()).device
             processed_bert = extract_bert_embeddings(self.args['bert_model'], self.bert_tokenizer, self.bert_model, text, device, keep_endpoints=False,
                                                      num_layers=self.bert_layer_mix.in_features if self.bert_layer_mix is not None else None,
-                                                     detach=not self.args.get('bert_finetune', False))
+                                                     detach=not self.args.get('bert_finetune', False) or not self.training,
+                                                     peft_name=self.peft_name)
 
             if self.bert_layer_mix is not None:
                 # add the average so that the default behavior is to
                 # take an average of the N layers, and anything else
                 # other than that needs to be learned
                 # TODO: refactor this
                 processed_bert = [self.bert_layer_mix(feature).squeeze(2) + feature.sum(axis=2) / self.bert_layer_mix.in_features for feature in processed_bert]
```

### Comparing `stanza-1.8.1/stanza/models/pos/scorer.py` & `stanza-1.8.2/stanza/models/pos/scorer.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/models/pos/trainer.py` & `stanza-1.8.2/stanza/models/pos/trainer.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,15 +5,16 @@
 import sys
 import logging
 import torch
 from torch import nn
 
 from stanza.models.common.trainer import Trainer as BaseTrainer
 from stanza.models.common import utils, loss
-from stanza.models.common.foundation_cache import NoTransformerFoundationCache
+from stanza.models.common.foundation_cache import load_bert, load_bert_with_peft, NoTransformerFoundationCache
+from stanza.models.common.peft_config import build_peft_wrapper, load_peft_wrapper
 from stanza.models.pos.model import Tagger
 from stanza.models.pos.vocab import MultiVocab
 
 logger = logging.getLogger('stanza')
 
 def unpack_batch(batch, device):
     """ Unpack a batch from the data loader. """
@@ -31,15 +32,25 @@
         if model_file is not None:
             # load everything from file
             self.load(model_file, pretrain, args=args, foundation_cache=foundation_cache)
         else:
             # build model from scratch
             self.args = args
             self.vocab = vocab
-            self.model = Tagger(args, vocab, emb_matrix=pretrain.emb if pretrain is not None else None, share_hid=args['share_hid'], foundation_cache=foundation_cache)
+
+            bert_model, bert_tokenizer = load_bert(self.args['bert_model'])
+            peft_name = None
+            if self.args['use_peft']:
+                # fine tune the bert if we're using peft
+                self.args['bert_finetune'] = True
+                peft_name = "pos"
+                bert_model = build_peft_wrapper(bert_model, self.args, logger, adapter_name=peft_name)
+
+            self.model = Tagger(args, vocab, emb_matrix=pretrain.emb if pretrain is not None else None, share_hid=args['share_hid'], foundation_cache=foundation_cache, bert_model=bert_model, bert_tokenizer=bert_tokenizer, force_bert_saved=self.args['bert_finetune'], peft_name=peft_name)
+
         self.model = self.model.to(device)
         self.optimizers = utils.get_split_optimizer(self.args['optim'], self.model, self.args['lr'], betas=(0.9, self.args['beta2']), eps=1e-6, weight_decay=self.args.get('initial_weight_decay', None), bert_learning_rate=self.args.get('bert_learning_rate', 0.0), is_peft=self.args.get("peft", False))
 
         self.schedulers = {}
 
         if self.args.get('bert_finetune', None):
             import transformers
@@ -102,14 +113,19 @@
             for k in skipped:
                 del model_state[k]
         params = {
                 'model': model_state,
                 'vocab': self.vocab.state_dict(),
                 'config': self.args
                 }
+        if self.args.get('use_peft', False):
+            # Hide import so that peft dependency is optional
+            from peft import get_peft_model_state_dict
+            params["bert_lora"] = get_peft_model_state_dict(self.model.bert_model, adapter_name=self.model.peft_name)
+
         try:
             torch.save(params, filename, _use_new_zipfile_serialization=False)
             logger.info("Model saved to {}".format(filename))
         except (KeyboardInterrupt, SystemExit):
             raise
         except Exception as e:
             logger.warning(f"Saving failed... {e} continuing anyway.")
@@ -122,19 +138,42 @@
         try:
             checkpoint = torch.load(filename, lambda storage, loc: storage)
         except BaseException:
             logger.error("Cannot load model from {}".format(filename))
             raise
         self.args = checkpoint['config']
         if args is not None: self.args.update(args)
+
+        # preserve old models which were created before transformers were added
         if 'bert_model' not in self.args:
             self.args['bert_model'] = None
+
+        lora_weights = checkpoint.get('bert_lora')
+        if lora_weights:
+            logger.debug("Found peft weights for POS; loading a peft adapter")
+            self.args["use_peft"] = True
+
+        # TODO: refactor this common block of code with NER
+        force_bert_saved = False
+        peft_name = None
+        if self.args.get('use_peft', False):
+            force_bert_saved = True
+            bert_model, bert_tokenizer, peft_name = load_bert_with_peft(self.args['bert_model'], "pos", foundation_cache)
+            bert_model = load_peft_wrapper(bert_model, lora_weights, self.args, logger, peft_name)
+            logger.debug("Loaded peft with name %s", peft_name)
+        else:
+            if any(x.startswith("bert_model.") for x in checkpoint['model'].keys()):
+                logger.debug("Model %s has a finetuned transformer.  Not using transformer cache to make sure the finetuned version of the transformer isn't accidentally used elsewhere", filename)
+                foundation_cache = NoTransformerFoundationCache(foundation_cache)
+                force_bert_saved = True
+            bert_model, bert_tokenizer = load_bert(self.args.get('bert_model'), foundation_cache)
+
         self.vocab = MultiVocab.load_state_dict(checkpoint['vocab'])
         # load model
         emb_matrix = None
         if self.args['pretrain'] and pretrain is not None: # we use pretrain only if args['pretrain'] == True and pretrain is not None
             emb_matrix = pretrain.emb
         if any(x.startswith("bert_model.") for x in checkpoint['model'].keys()):
             logger.debug("Model %s has a finetuned transformer.  Not using transformer cache to make sure the finetuned version of the transformer isn't accidentally used elsewhere", filename)
             foundation_cache = NoTransformerFoundationCache(foundation_cache)
-        self.model = Tagger(self.args, self.vocab, emb_matrix=emb_matrix, share_hid=self.args['share_hid'], foundation_cache=foundation_cache)
+        self.model = Tagger(self.args, self.vocab, emb_matrix=emb_matrix, share_hid=self.args['share_hid'], foundation_cache=foundation_cache, bert_model=bert_model, bert_tokenizer=bert_tokenizer, force_bert_saved=force_bert_saved, peft_name=peft_name)
         self.model.load_state_dict(checkpoint['model'], strict=False)
```

### Comparing `stanza-1.8.1/stanza/models/pos/vocab.py` & `stanza-1.8.2/stanza/models/pos/vocab.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,14 +29,17 @@
         for k in list(counter.keys()):
             if counter[k] < self.cutoff or k in self.ignore:
                 del counter[k]
 
         self._id2unit = VOCAB_PREFIX + list(sorted(list(counter.keys()), key=lambda k: counter[k], reverse=True))
         self._unit2id = {w:i for i, w in enumerate(self._id2unit)}
 
+    def __str__(self):
+        return "<{}: {}>".format(type(self), ",".join("|%s|" % x for x in self._id2unit))
+
 class XPOSVocab(CompositeVocab):
     def __init__(self, data=None, lang="", idx=0, sep="", keyed=False):
         super().__init__(data, lang, idx=idx, sep=sep, keyed=keyed)
 
 class FeatureVocab(CompositeVocab):
     def __init__(self, data=None, lang="", idx=0, sep="|", keyed=True):
         super().__init__(data, lang, idx=idx, sep=sep, keyed=keyed)
```

### Comparing `stanza-1.8.1/stanza/models/pos/xpos_vocab_factory.py` & `stanza-1.8.2/stanza/models/pos/xpos_vocab_factory.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/models/pos/xpos_vocab_utils.py` & `stanza-1.8.2/stanza/models/pos/xpos_vocab_utils.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/models/tagger.py` & `stanza-1.8.2/stanza/models/tagger.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 from stanza.models.pos.trainer import Trainer
 from stanza.models.pos import scorer
 from stanza.models.common import utils
 from stanza.models.common import pretrain
 from stanza.models.common.data import augment_punct
 from stanza.models.common.doc import *
 from stanza.models.common.foundation_cache import FoundationCache
+from stanza.models.common.peft_config import add_peft_args, resolve_peft_args
 from stanza.utils.conll import CoNLL
 from stanza.models import _training_logging
 
 logger = logging.getLogger('stanza')
 
 def build_argparse():
     parser = argparse.ArgumentParser()
@@ -99,33 +100,36 @@
 
     parser.add_argument('--max_steps', type=int, default=50000)
     parser.add_argument('--eval_interval', type=int, default=100)
     parser.add_argument('--fix_eval_interval', dest='adapt_eval_interval', action='store_false', \
             help="Use fixed evaluation interval for all treebanks, otherwise by default the interval will be increased for larger treebanks.")
     parser.add_argument('--max_steps_before_stop', type=int, default=3000, help='Changes learning method or early terminates after this many steps if the dev scores are not improving')
     parser.add_argument('--batch_size', type=int, default=250)
+    parser.add_argument('--batch_maximum_tokens', type=int, default=5000, help='When run in a Pipeline, limit a batch to this many tokens to help avoid OOM for long sentences')
     parser.add_argument('--max_grad_norm', type=float, default=1.0, help='Gradient clipping.')
     parser.add_argument('--log_step', type=int, default=20, help='Print log every k steps.')
     parser.add_argument('--log_norms', action='store_true', default=False, help='Log the norms of all the parameters (noisy!)')
     parser.add_argument('--save_dir', type=str, default='saved_models/pos', help='Root dir for saving models.')
     parser.add_argument('--save_name', type=str, default="{shorthand}_{embedding}_tagger.pt", help="File name to save the model")
     parser.add_argument('--save_each', default=False, action='store_true', help="Save each checkpoint to its own model.  Will take up a bunch of space")
 
     parser.add_argument('--seed', type=int, default=1234)
+    add_peft_args(parser)
     utils.add_device_args(parser)
 
     parser.add_argument('--augment_nopunct', type=float, default=None, help='Augment the training data by copying this fraction of punct-ending sentences as non-punct.  Default of None will aim for roughly 50%%')
 
     parser.add_argument('--wandb', action='store_true', help='Start a wandb session and write the results of training.  Only applies to training.  Use --wandb_name instead to specify a name')
     parser.add_argument('--wandb_name', default=None, help='Name of a wandb session to start when training.  Will default to the dataset short name')
     return parser
 
 def parse_args(args=None):
     parser = build_argparse()
     args = parser.parse_args(args=args)
+    resolve_peft_args(args, logger)
 
     if args.augment_nopunct is None:
         args.augment_nopunct = 0.25
 
     if args.wandb_name:
         args.wandb = True
 
@@ -172,15 +176,16 @@
     elif dev_batch.has_upos and not dev_batch.has_xpos and not dev_batch.has_feats:
         return "UPOS"
     else:
         return "AllTags"
 
 def load_training_data(args, pretrain):
     train_docs = []
-    for train_file in args['train_file'].split(";"):
+    train_files = args['train_file'].split(";")
+    for train_file in train_files:
         logger.info("Reading %s" % train_file)
         # train_data is now a list of sentences, where each sentence is a
         # list of words, in which each word is a dict of conll attributes
         train_file_data, _, _ = CoNLL.conll2dict(input_file=train_file)
         logger.info("Train File {}, Data Size: {}".format(train_file, len(train_file_data)))
         train_docs.append(Document(train_file_data))
     if sum(len(x.sentences) for x in train_docs) == 0:
@@ -189,14 +194,36 @@
     # but create batches whereby if a doc has upos/xpos tags we include them all.
     # therefore, we create seperate datasets and loaders for each input training file,
     # which will ensure the system be able to see batches with both upos available
     # and upos unavailable depending on what the availability in the file is.
     vocab = Dataset.init_vocab(train_docs, args)
     train_data = [Dataset(i, args, pretrain, vocab=vocab, evaluation=False)
                   for i in train_docs]
+    for train_file, td in zip(train_files, train_data):
+        if not td.has_upos:
+            logger.info("No UPOS in %s" % train_file)
+        if not td.has_xpos:
+            logger.info("No XPOS in %s" % train_file)
+        if not td.has_feats:
+            logger.info("No feats in %s" % train_file)
+
+    # reject partially tagged upos or xpos documents
+    # otherwise, the model will learn to output blanks for some words,
+    # which is probably a confusing result
+    # (and definitely throws off the depparse)
+    # another option would be to treat those as masked out
+    for td_idx, td in enumerate(train_data):
+        if td.has_upos:
+            upos_data = td.doc.get(UPOS, as_sentences=True)
+            for sentence_idx, sentence in enumerate(upos_data):
+                for word_idx, upos in enumerate(sentence):
+                    if upos == '_' or upos is None:
+                        conll = "{:C}".format(td.doc.sentences[sentence_idx])
+                        raise RuntimeError("Found a blank tag in the UPOS at sentence %d word %d of %s.\n%s" % ((sentence_idx+1), (word_idx+1), train_files[td_idx], conll))
+
     # here we make sure the model will learn to output _ for empty columns
     # if *any* dataset has data for the upos, xpos, or feature column,
     # we consider that data enough to train the model on that column
     # otherwise, we want to train the model to always output blanks
     if not any(td.has_upos for td in train_data):
         for td in train_data:
             td.has_upos = True
@@ -366,25 +393,28 @@
     else:
         logger.info("Dev set never evaluated.  Saving final model.")
         trainer.save(model_file)
 
 
 def evaluate(args):
     # file paths
-    system_pred_file = args['output_file']
     model_file = model_file_name(args)
 
     pretrain = load_pretrain(args)
 
     load_args = {'charlm_forward_file': args.get('charlm_forward_file', None),
                  'charlm_backward_file': args.get('charlm_backward_file', None)}
 
     # load model
     logger.info("Loading model from: {}".format(model_file))
     trainer = Trainer(pretrain=pretrain, model_file=model_file, device=args['device'], args=load_args)
+    evaluate_trainer(args, trainer, pretrain)
+
+def evaluate_trainer(args, trainer, pretrain):
+    system_pred_file = args['output_file']
     loaded_args, vocab = trainer.args, trainer.vocab
 
     # load config
     for k in args:
         if k.endswith('_dir') or k.endswith('_file') or k in ['shorthand'] or k == 'mode':
             loaded_args[k] = args[k]
```

### Comparing `stanza-1.8.1/stanza/models/tokenization/data.py` & `stanza-1.8.2/stanza/models/tokenization/data.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/models/tokenization/model.py` & `stanza-1.8.2/stanza/models/tokenization/model.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/models/tokenization/tokenize_files.py` & `stanza-1.8.2/stanza/models/tokenization/tokenize_files.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/models/tokenization/trainer.py` & `stanza-1.8.2/stanza/models/tokenization/trainer.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/models/tokenization/utils.py` & `stanza-1.8.2/stanza/models/tokenization/utils.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/models/tokenization/vocab.py` & `stanza-1.8.2/stanza/models/tokenization/vocab.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/models/tokenizer.py` & `stanza-1.8.2/stanza/models/tokenizer.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/models/wl_coref.py` & `stanza-1.8.2/stanza/models/wl_coref.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/pipeline/constituency_processor.py` & `stanza-1.8.2/stanza/pipeline/constituency_processor.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/pipeline/core.py` & `stanza-1.8.2/stanza/pipeline/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -226,16 +226,20 @@
         logger.debug('Loading resource file...')
         resources = load_resources_json(self.dir, resources_filepath)
         if lang in resources:
             if 'alias' in resources[lang]:
                 logger.info(f'"{lang}" is an alias for "{resources[lang]["alias"]}"')
                 lang = resources[lang]['alias']
             lang_name = resources[lang]['lang_name'] if 'lang_name' in resources[lang] else ''
+        elif allow_unknown_language:
+            logger.warning("Trying to create pipeline for unsupported language: %s", lang)
+            lang_name = langcode_to_lang(lang)
         else:
-            logger.warning(f'Unsupported language: {lang}.')
+            logger.warning("Unsupported language: %s  If trying to add a new language, consider using allow_unknown_language=True", lang)
+            lang_name = langcode_to_lang(lang)
 
         # Maintain load list
         if lang in resources:
             self.load_list = maintain_processor_list(resources, lang, package, processors, maybe_add_mwt=(not kwargs.get("tokenize_pretokenized")))
             self.load_list = add_dependencies(resources, lang, self.load_list)
             if download_method is not DownloadMethod.NONE:
                 # skip processors which aren't downloaded from our collection
@@ -251,15 +255,14 @@
                                 model_dir=self.dir,
                                 resources_version=resources_version,
                                 proxies=proxies,
                                 log_info=False)
         elif allow_unknown_language:
             self.load_list = [(proc, [ModelSpecification(processor=proc, package='default', dependencies=None)])
                               for proc in list(processors.keys())]
-            lang_name = langcode_to_lang(lang)
         else:
             self.load_list = []
         self.load_list = self.update_kwargs(kwargs, self.load_list)
         if len(self.load_list) == 0:
             if lang not in resources or PACKAGES not in resources[lang]:
                 raise ValueError(f'No processors to load for language {lang}.  Language {lang} is currently unsupported')
             else:
@@ -317,15 +320,15 @@
                 # suggest the user try to download the models
                 if 'model_path' in curr_processor_config:
                     model_path = curr_processor_config['model_path']
                     if e.filename == model_path or (isinstance(model_path, (tuple, list)) and e.filename in model_path):
                         model_path = e.filename
                     model_dir, model_name = os.path.split(model_path)
                     lang_dir = os.path.dirname(model_dir)
-                    if not os.path.exists(lang_dir):
+                    if lang_dir and not os.path.exists(lang_dir):
                         # model files for this language can't be found in the expected directory
                         raise LanguageNotDownloadedError(lang, lang_dir, model_path) from e
                     if processor_name not in resources[lang]:
                         # user asked for a model which doesn't exist for this language?
                         raise UnsupportedProcessorError(processor_name, lang) from e
                     if not os.path.exists(model_path):
                         model_name, _ = os.path.splitext(model_name)
```

### Comparing `stanza-1.8.1/stanza/pipeline/coref_processor.py` & `stanza-1.8.2/stanza/pipeline/coref_processor.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/pipeline/depparse_processor.py` & `stanza-1.8.2/stanza/pipeline/depparse_processor.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/pipeline/external/corenlp_converter_depparse.py` & `stanza-1.8.2/stanza/pipeline/external/corenlp_converter_depparse.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/pipeline/external/jieba.py` & `stanza-1.8.2/stanza/pipeline/external/jieba.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/pipeline/external/pythainlp.py` & `stanza-1.8.2/stanza/pipeline/external/pythainlp.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/pipeline/external/spacy.py` & `stanza-1.8.2/stanza/pipeline/external/spacy.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/pipeline/external/sudachipy.py` & `stanza-1.8.2/stanza/pipeline/external/sudachipy.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/pipeline/langid_processor.py` & `stanza-1.8.2/stanza/pipeline/langid_processor.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/pipeline/lemma_processor.py` & `stanza-1.8.2/stanza/pipeline/lemma_processor.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/pipeline/multilingual.py` & `stanza-1.8.2/stanza/pipeline/multilingual.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/pipeline/mwt_processor.py` & `stanza-1.8.2/stanza/pipeline/mwt_processor.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/pipeline/ner_processor.py` & `stanza-1.8.2/stanza/pipeline/ner_processor.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/pipeline/pos_processor.py` & `stanza-1.8.2/stanza/pipeline/pos_processor.py`

 * *Files 6% similar despite different names*

```diff
@@ -63,18 +63,21 @@
         """
         Returns the features known by this model
         """
         values = {k: v.keys() - VOCAB_PREFIX for k, v in self.vocab['feats']._unit2id.items()}
         return values
 
     def process(self, document):
+        # currently, POS models are saved w/o the batch_maximum_tokens flag
+        maximum_tokens = self.config.get('batch_maximum_tokens', 5000)
+
         dataset = Dataset(
             document, self.config, self.pretrain, vocab=self.vocab, evaluation=True,
             sort_during_eval=True)
-        batch = iter(dataset.to_loader(batch_size=self.config['batch_size']))
+        batch = iter(dataset.to_length_limited_loader(batch_size=self.config['batch_size'], maximum_tokens=maximum_tokens))
         preds = []
 
         idx = []
         with torch.no_grad():
             if self._tqdm:
                 for i, b in enumerate(tqdm(batch)):
                     idx.extend(b[-1])
```

### Comparing `stanza-1.8.1/stanza/pipeline/processor.py` & `stanza-1.8.2/stanza/pipeline/processor.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/pipeline/sentiment_processor.py` & `stanza-1.8.2/stanza/pipeline/sentiment_processor.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/pipeline/tokenize_processor.py` & `stanza-1.8.2/stanza/pipeline/tokenize_processor.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/protobuf/CoreNLP_pb2.py` & `stanza-1.8.2/stanza/protobuf/CoreNLP_pb2.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/protobuf/__init__.py` & `stanza-1.8.2/stanza/protobuf/__init__.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/resources/common.py` & `stanza-1.8.2/stanza/resources/common.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/resources/default_packages.py` & `stanza-1.8.2/stanza/resources/default_packages.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 
 # all languages will have a map which represents the available packages
 PACKAGES = "packages"
 
 # default treebank for languages
 default_treebanks = {
     "af":      "afribooms",
+    # currently not publicly released!  sent to us from the group developing this resource
+    "ang":     "nerthus",
     "ar":      "padt",
     "be":      "hse",
     "bg":      "btb",
     "bxr":     "bdt",
     "ca":      "ancora",
     "cop":     "scriptorium",
     "cs":      "pdt",
@@ -116,14 +118,15 @@
 
 
 # in some cases, we give the pretrain a name other than the original
 # name for the UD dataset
 # we will eventually do this for all of the pretrains
 specific_default_pretrains = {
     "af":      "fasttextwiki",
+    "ang":     "nerthus",
     "ar":      "conll17",
     "be":      "fasttextwiki",
     "bg":      "conll17",
     "bxr":     "fasttextwiki",
     "ca":      "conll17",
     "cs":      "conll17",
     "cu":      "conll17",
@@ -267,14 +270,15 @@
     },
 }
 
 
 # default charlms for languages
 default_charlms = {
     "af": "oscar",
+    "ang": "nerthus1024",
     "ar": "ccwiki",
     "bg": "conll17",
     "da": "oscar",
     "de": "newswiki",
     "en": "1billion",
     "es": "newswiki",
     "fa": "conll17",
@@ -384,14 +388,15 @@
     "vi": "vsfc_charlm",
     "zh-hans": "ren_charlm",
 }
 
 # also, a few languages (very few, currently) have constituency parser models
 default_constituency = {
     "da": "arboretum_charlm",
+    "de": "spmrl_charlm",
     "en": "ptb3-revised_charlm",
     "es": "combined_charlm",
     "id": "icon_charlm",
     "it": "vit_charlm",
     "ja": "alt_charlm",
     "pt": "cintil_charlm",
     #"tr": "starlang_charlm",
@@ -463,22 +468,46 @@
     #  Maltehb/aelaectra-danish-electra-small-cased
     #
     "da": "vesteinn/ScandiBERT",
 
     # As of April 2022, the bert models available have a weird
     # tokenizer issue where soft hyphen causes it to crash.
     # We attempt to compensate for that in the dev branch
-    # bert-base-german-cased
-    # dev:  2022-04-27 21:21:31 INFO: de_germeval2014 87.59
-    # test: 2022-04-27 21:21:59 INFO: de_germeval2014 86.95
-    #
-    # dbmdz/bert-base-german-cased
-    # dev:  2022-04-27 22:24:59 INFO: de_germeval2014 88.22
-    # test: 2022-04-27 22:25:27 INFO: de_germeval2014 87.80
-    "de": "dbmdz/bert-base-german-cased",
+    #
+    # NER scores
+    #     model                                       dev      text
+    # xlm-roberta-large                              86.56    85.23
+    # bert-base-german-cased                         87.59    86.95
+    # dbmdz/bert-base-german-cased                   88.27    87.47
+    # german-nlp-group/electra-base-german-uncased   88.60    87.09
+    #
+    # constituency scores w/ peft, March 2024 model, in-order
+    #    model             dev     test
+    #   xlm-roberta-base  95.17   93.34
+    #   xlm-roberta-large 95.86   94.46    (!!!)
+    #   bert-base         95.24   93.24
+    #   dbmdz/bert        95.32   93.33
+    #   german/electra    95.72   94.05
+    #
+    # POS scores
+    #    model             dev     test
+    #   None              88.65   87.28
+    #   xlm-roberta-large 89.21   88.11
+    #   bert-base         89.52   88.42
+    #   dbmdz/bert        89.67   88.54
+    #   german/electra    89.98   88.66
+    #
+    # depparse scores, LAS
+    #    model             dev     test
+    #   None              87.76   84.37
+    #   xlm-roberta-large 89.00   85.79
+    #   bert-base         88.72   85.40
+    #   dbmdz/bert        88.70   85.14
+    #   german/electra    89.21   86.06
+    "de": "german-nlp-group/electra-base-german-uncased",
 
     # experiments on various forms of roberta & electra
     #  https://huggingface.co/roberta-base
     #  https://huggingface.co/roberta-large
     #  https://huggingface.co/google/electra-small-discriminator
     #  https://huggingface.co/google/electra-base-discriminator
     #  https://huggingface.co/google/electra-large-discriminator
@@ -740,15 +769,17 @@
     "aubmindlab/araelectra-base-discriminator": "aubmind-electra",
     "aubmindlab/bert-base-arabertv2": "aubmind-bert",
 
     # da
     "vesteinn/ScandiBERT": "scandibert",
 
     # de
-    "dbmdz/bert-base-german-cased": "bert",
+    "bert-base-german-cased": "bert-base-german-cased",
+    "dbmdz/bert-base-german-cased": "dbmdz-bert-german-cased",
+    "german-nlp-group/electra-base-german-uncased": "german-nlp-electra",
 
     # en
     "bert-base-multilingual-cased": "mbert",
     "xlm-roberta-large": "xlm-roberta-large",
     "google/electra-large-discriminator": "electra-large",
     "microsoft/deberta-v3-large": "deberta-v3-large",
 
@@ -774,15 +805,15 @@
     "lgessler/microbert-ancient-greek-mxp": "grc-microbert-mxp",
     "altsoph/bert-base-ancientgreek-uncased": "grc-altsoph",
 
     # he
     "imvladikon/alephbertgimmel-base-512" : "alephbertgimmel",
 
     # hy
-    "xlm-roberta-base": "roberta",
+    "xlm-roberta-base": "xlm-roberta-base",
 
     # id
     "indolem/indobert-base-uncased":         "indobert",
     "indobenchmark/indobert-large-p1":       "indobenchmark-large-p1",
     "indobenchmark/indobert-base-p1":        "indobenchmark-base-p1",
     "indobenchmark/indobert-lite-large-p1":  "indobenchmark-lite-large-p1",
     "indobenchmark/indobert-lite-base-p1":   "indobenchmark-lite-base-p1",
```

### Comparing `stanza-1.8.1/stanza/resources/installation.py` & `stanza-1.8.2/stanza/resources/installation.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/resources/prepare_resources.py` & `stanza-1.8.2/stanza/resources/prepare_resources.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/resources/print_charlm_depparse.py` & `stanza-1.8.2/stanza/resources/print_charlm_depparse.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/server/__init__.py` & `stanza-1.8.2/stanza/server/__init__.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/server/annotator.py` & `stanza-1.8.2/stanza/server/annotator.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/server/client.py` & `stanza-1.8.2/stanza/server/client.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/server/dependency_converter.py` & `stanza-1.8.2/stanza/server/dependency_converter.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/server/java_protobuf_requests.py` & `stanza-1.8.2/stanza/server/java_protobuf_requests.py`

 * *Files 1% similar despite different names*

```diff
@@ -181,19 +181,23 @@
     """
     Add a node and possibly an edge for a word in a basic dependency graph.
     """
     node = graph.node.add()
     node.sentenceIndex = sent_idx+1
     node.index = word_idx+1
 
-    if word.head != 0:
+    if word.head != 0 and word.head is not None:
         edge = graph.edge.add()
         edge.source = word.head
         edge.target = word_idx+1
-        edge.dep = word.deprel
+        if word.deprel is not None:
+            edge.dep = word.deprel
+        else:
+            # the receiving side doesn't like null as a dependency
+            edge.dep = "_"
 
 def convert_networkx_graph(graph_proto, sentence, sent_idx):
     """
     Turns a networkx graph into a DependencyGraph from the proto file
     """
     for token in sentence.tokens:
         for word in token.words:
```

### Comparing `stanza-1.8.1/stanza/server/main.py` & `stanza-1.8.2/stanza/server/main.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/server/morphology.py` & `stanza-1.8.2/stanza/server/morphology.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/server/parser_eval.py` & `stanza-1.8.2/stanza/server/parser_eval.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/server/semgrex.py` & `stanza-1.8.2/stanza/server/semgrex.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,14 +43,16 @@
 SEMGREX_JAVA = "edu.stanford.nlp.semgraph.semgrex.ProcessSemgrexRequest"
 
 def send_semgrex_request(request):
     return send_request(request, SemgrexResponse, SEMGREX_JAVA)
 
 def build_request(doc, semgrex_patterns, enhanced=False):
     request = SemgrexRequest()
+    if isinstance(semgrex_patterns, str):
+        semgrex_patterns = [semgrex_patterns]
     for semgrex in semgrex_patterns:
         request.semgrex.append(semgrex)
 
     for sent_idx, sentence in enumerate(doc.sentences):
         query = request.query.add()
         if enhanced:
             # tokens will be added on to the graph object
```

### Comparing `stanza-1.8.1/stanza/server/ssurgeon.py` & `stanza-1.8.2/stanza/server/ssurgeon.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,36 +4,32 @@
 (Semantic graph SURGEON) query
 
 The main program in this file gives a very short intro to how to use it.
 """
 
 
 import argparse
+from collections import namedtuple
 import copy
 import os
 import re
 import sys
 
 from stanza.models.common.utils import misc_to_space_after, space_after_to_misc
 from stanza.protobuf import SsurgeonRequest, SsurgeonResponse
 from stanza.server import java_protobuf_requests
 from stanza.utils.conll import CoNLL
 
 from stanza.models.common.doc import ID, TEXT, LEMMA, UPOS, XPOS, FEATS, HEAD, DEPREL, DEPS, MISC, START_CHAR, END_CHAR, NER, Word, Token, Sentence
 
 SSURGEON_JAVA = "edu.stanford.nlp.semgraph.semgrex.ssurgeon.ProcessSsurgeonRequest"
 
-class SsurgeonEdit:
-    def __init__(self, semgrex_pattern, ssurgeon_edits, ssurgeon_id=None, notes=None, language="UniversalEnglish"):
-        # not a named tuple so we can have defaults without requiring a python upgrade
-        self.semgrex_pattern = semgrex_pattern
-        self.ssurgeon_edits = ssurgeon_edits
-        self.ssurgeon_id = ssurgeon_id
-        self.notes = notes
-        self.language = language
+SsurgeonEdit = namedtuple("SsurgeonEdit",
+                          "semgrex_pattern ssurgeon_edits ssurgeon_id notes language",
+                          defaults=[None, None, "UniversalEnglish"])
 
 def parse_ssurgeon_edits(ssurgeon_text):
     ssurgeon_text = ssurgeon_text.strip()
     ssurgeon_blocks = re.split("\n\n+", ssurgeon_text)
     ssurgeon_edits = []
     for idx, block in enumerate(ssurgeon_blocks):
         lines = block.split("\n")
```

### Comparing `stanza-1.8.1/stanza/server/tokensregex.py` & `stanza-1.8.2/stanza/server/tokensregex.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/server/tsurgeon.py` & `stanza-1.8.2/stanza/server/tsurgeon.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/server/ud_enhancer.py` & `stanza-1.8.2/stanza/server/ud_enhancer.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/tests/__init__.py` & `stanza-1.8.2/stanza/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/tests/classifiers/test_classifier.py` & `stanza-1.8.2/stanza/tests/classifiers/test_classifier.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import glob
 import os
 
 import pytest
 
 import numpy as np
 import torch
 
@@ -41,15 +42,15 @@
 
     pt = pretrain.Pretrain(str(embedding_pt), str(embedding_txt))
     pt.load()
     assert os.path.exists(embedding_pt)
     return embedding_pt
 
 class TestClassifier:
-    def build_model(self, tmp_path, fake_embeddings, train_file, dev_file, extra_args=None):
+    def build_model(self, tmp_path, fake_embeddings, train_file, dev_file, extra_args=None, checkpoint_file=None):
         """
         Build a model to be used by one of the later tests
         """
         save_dir = str(tmp_path / "classifier")
         save_name = "model.pt"
         args = ["--save_dir", save_dir,
                 "--save_name", save_name,
@@ -60,29 +61,33 @@
                 "--dev_file", str(dev_file),
                 "--max_epochs", "2",
                 "--batch_size", "60"]
         if extra_args is not None:
             args = args + extra_args
         args = classifier.parse_args(args)
         train_set = data.read_dataset(args.train_file, args.wordvec_type, args.min_train_len)
-        trainer = Trainer.build_new_model(args, train_set)
+        if checkpoint_file:
+            trainer = Trainer.load(checkpoint_file, args, load_optimizer=True)
+        else:
+            trainer = Trainer.build_new_model(args, train_set)
         return trainer, train_set, args
 
-    def run_training(self, tmp_path, fake_embeddings, train_file, dev_file, extra_args=None):
+    def run_training(self, tmp_path, fake_embeddings, train_file, dev_file, extra_args=None, checkpoint_file=None):
         """
         Iterate a couple times over a model
         """
-        trainer, train_set, args = self.build_model(tmp_path, fake_embeddings, train_file, dev_file, extra_args)
+        trainer, train_set, args = self.build_model(tmp_path, fake_embeddings, train_file, dev_file, extra_args, checkpoint_file)
         dev_set = data.read_dataset(args.dev_file, args.wordvec_type, args.min_train_len)
         labels = data.dataset_labels(train_set)
 
         save_filename = os.path.join(args.save_dir, args.save_name)
-        checkpoint_file = utils.checkpoint_name(args.save_dir, save_filename, args.checkpoint_save_name)
+        if checkpoint_file is None:
+            checkpoint_file = utils.checkpoint_name(args.save_dir, save_filename, args.checkpoint_save_name)
         classifier.train_model(trainer, save_filename, checkpoint_file, args, train_set, dev_set, labels)
-        return trainer, save_filename
+        return trainer, save_filename, checkpoint_file
 
     def test_build_model(self, tmp_path, fake_embeddings, train_file, dev_file):
         """
         Test that building a basic model works
         """
         self.build_model(tmp_path, fake_embeddings, train_file, dev_file, extra_args=["--bilstm_hidden_dim", "20"])
 
@@ -137,55 +142,111 @@
         self.run_training(tmp_path, fake_embeddings, train_file, dev_file, args)
 
         args = ["--filter_sizes", "((3,2),3)", "--filter_channels", "20", "--bilstm_hidden_dim", "20"]
         self.run_training(tmp_path, fake_embeddings, train_file, dev_file, args)
 
     def test_train_filter_channels(self, tmp_path, fake_embeddings, train_file, dev_file):
         args = ["--filter_sizes", "((3,2),3)", "--filter_channels", "20", "--no_bilstm"]
-        trainer, _ = self.run_training(tmp_path, fake_embeddings, train_file, dev_file, args)
+        trainer, _, _ = self.run_training(tmp_path, fake_embeddings, train_file, dev_file, args)
         assert trainer.model.fc_input_size == 40
 
         args = ["--filter_sizes", "((3,2),3)", "--filter_channels", "15,20", "--no_bilstm"]
-        trainer, _ = self.run_training(tmp_path, fake_embeddings, train_file, dev_file, args)
+        trainer, _, _ = self.run_training(tmp_path, fake_embeddings, train_file, dev_file, args)
         # 50 = 2x15 for the 2d conv (over 5 dim embeddings) + 20
         assert trainer.model.fc_input_size == 50
 
     def test_train_bert(self, tmp_path, fake_embeddings, train_file, dev_file):
         """
         Test on a tiny Bert WITHOUT finetuning, which hopefully does not take up too much disk space or memory
         """
         bert_model = "hf-internal-testing/tiny-bert"
 
-        trainer, save_filename = self.run_training(tmp_path, fake_embeddings, train_file, dev_file, extra_args=["--bilstm_hidden_dim", "20", "--bert_model", bert_model])
+        trainer, save_filename, _ = self.run_training(tmp_path, fake_embeddings, train_file, dev_file, extra_args=["--bilstm_hidden_dim", "20", "--bert_model", bert_model])
         assert os.path.exists(save_filename)
         saved_model = torch.load(save_filename, lambda storage, loc: storage)
         # check that the bert model wasn't saved as part of the classifier
         assert not saved_model['params']['config'].force_bert_saved
         assert not any(x.startswith("bert_model") for x in saved_model['params']['model'].keys())
 
     def test_finetune_bert(self, tmp_path, fake_embeddings, train_file, dev_file):
         """
         Test on a tiny Bert WITH finetuning, which hopefully does not take up too much disk space or memory
         """
         bert_model = "hf-internal-testing/tiny-bert"
 
-        trainer, save_filename = self.run_training(tmp_path, fake_embeddings, train_file, dev_file, extra_args=["--bilstm_hidden_dim", "20", "--bert_model", bert_model, "--bert_finetune"])
+        trainer, save_filename, _ = self.run_training(tmp_path, fake_embeddings, train_file, dev_file, extra_args=["--bilstm_hidden_dim", "20", "--bert_model", bert_model, "--bert_finetune"])
         assert os.path.exists(save_filename)
         saved_model = torch.load(save_filename, lambda storage, loc: storage)
         # after finetuning the bert model, make sure that the save file DOES contain parts of the transformer
         assert saved_model['params']['config'].force_bert_saved
         assert any(x.startswith("bert_model") for x in saved_model['params']['model'].keys())
 
+    def test_finetune_bert_layers(self, tmp_path, fake_embeddings, train_file, dev_file):
+        """Test on a tiny Bert WITH finetuning, which hopefully does not take up too much disk space or memory, using 2 layers
+
+        As an added bonus (or eager test), load the finished model and continue
+        training from there.  Then check that the initial model and
+        the middle model are different, then that the middle model and
+        final model are different
+
+        """
+        bert_model = "hf-internal-testing/tiny-bert"
+
+        trainer, save_filename, checkpoint_file = self.run_training(tmp_path, fake_embeddings, train_file, dev_file, extra_args=["--bilstm_hidden_dim", "20", "--bert_model", bert_model, "--bert_finetune", "--bert_hidden_layers", "2", "--save_intermediate_models"])
+        assert os.path.exists(save_filename)
+
+        save_path = os.path.split(save_filename)[0]
+
+        initial_model = glob.glob(os.path.join(save_path, "*E0000*"))
+        assert len(initial_model) == 1
+        initial_model = initial_model[0]
+        initial_model = torch.load(initial_model, lambda storage, loc: storage)
+
+        second_model_file = glob.glob(os.path.join(save_path, "*E0002*"))
+        assert len(second_model_file) == 1
+        second_model_file = second_model_file[0]
+        second_model = torch.load(second_model_file, lambda storage, loc: storage)
+
+        for layer_idx in range(2):
+            bert_names = [x for x in second_model['params']['model'].keys() if x.startswith("bert_model") and "layer.%d." % layer_idx in x]
+            assert len(bert_names) > 0
+            assert all(x in initial_model['params']['model'] and x in second_model['params']['model'] for x in bert_names)
+            assert not all(torch.allclose(initial_model['params']['model'].get(x), second_model['params']['model'].get(x)) for x in bert_names)
+
+        # put some random marker in the file to look for later,
+        # check the continued training didn't clobber the expected file
+        assert "asdf" not in second_model
+        second_model["asdf"] = 1234
+        torch.save(second_model, second_model_file)
+
+        trainer, save_filename, checkpoint_file = self.run_training(tmp_path, fake_embeddings, train_file, dev_file, extra_args=["--bilstm_hidden_dim", "20", "--bert_model", bert_model, "--bert_finetune", "--bert_hidden_layers", "2", "--save_intermediate_models", "--max_epochs", "5"], checkpoint_file=checkpoint_file)
+
+        second_model_file_redo = glob.glob(os.path.join(save_path, "*E0002*"))
+        assert len(second_model_file_redo) == 1
+        assert second_model_file == second_model_file_redo[0]
+        second_model = torch.load(second_model_file, lambda storage, loc: storage)
+        assert "asdf" in second_model
+
+        fifth_model_file = glob.glob(os.path.join(save_path, "*E0005*"))
+        assert len(fifth_model_file) == 1
+
+        final_model = torch.load(fifth_model_file[0], lambda storage, loc: storage)
+        for layer_idx in range(2):
+            bert_names = [x for x in final_model['params']['model'].keys() if x.startswith("bert_model") and "layer.%d." % layer_idx in x]
+            assert len(bert_names) > 0
+            assert all(x in final_model['params']['model'] and x in second_model['params']['model'] for x in bert_names)
+            assert not all(torch.allclose(final_model['params']['model'].get(x), second_model['params']['model'].get(x)) for x in bert_names)
+
     def test_finetune_peft(self, tmp_path, fake_embeddings, train_file, dev_file):
         """
         Test on a tiny Bert with PEFT finetuning
         """
         bert_model = "hf-internal-testing/tiny-bert"
 
-        trainer, save_filename = self.run_training(tmp_path, fake_embeddings, train_file, dev_file, extra_args=["--bilstm_hidden_dim", "20", "--bert_model", bert_model, "--bert_finetune", "--use_peft", "--lora_modules_to_save", "pooler"])
+        trainer, save_filename, _ = self.run_training(tmp_path, fake_embeddings, train_file, dev_file, extra_args=["--bilstm_hidden_dim", "20", "--bert_model", bert_model, "--bert_finetune", "--use_peft", "--lora_modules_to_save", "pooler"])
         assert os.path.exists(save_filename)
         saved_model = torch.load(save_filename, lambda storage, loc: storage)
         # after finetuning the bert model, make sure that the save file DOES contain parts of the transformer, but only in peft form
         assert saved_model['params']['config'].bert_model == bert_model
         assert saved_model['params']['config'].force_bert_saved
         assert saved_model['params']['config'].use_peft
 
@@ -198,7 +259,59 @@
         assert not any(x.startswith("bert_model") for x in saved_model['params']['model'].keys())
 
         # The Pipeline should load and run a PEFT trained model,
         # although obviously we don't expect the results to do
         # anything correct
         pipeline = stanza.Pipeline("en", download_method=None, model_dir=TEST_MODELS_DIR, processors="tokenize,sentiment", sentiment_model_path=save_filename, sentiment_pretrain_path=str(fake_embeddings))
         doc = pipeline("This is a test")
+
+    def test_finetune_peft_restart(self, tmp_path, fake_embeddings, train_file, dev_file):
+        """
+        Test that if we restart training on a peft model, the peft weights change
+        """
+        bert_model = "hf-internal-testing/tiny-bert"
+
+        trainer, save_file, checkpoint_file = self.run_training(tmp_path, fake_embeddings, train_file, dev_file, extra_args=["--bilstm_hidden_dim", "20", "--bert_model", bert_model, "--bert_finetune", "--use_peft", "--lora_modules_to_save", "pooler", "--save_intermediate_models"])
+
+        assert os.path.exists(save_file)
+        saved_model = torch.load(save_file, lambda storage, loc: storage)
+        assert any(x.find(".encoder.") >= 0 for x in saved_model['params']['bert_lora'])
+
+
+        trainer, save_file, checkpoint_file = self.run_training(tmp_path, fake_embeddings, train_file, dev_file, extra_args=["--bilstm_hidden_dim", "20", "--bert_model", bert_model, "--bert_finetune", "--use_peft", "--lora_modules_to_save", "pooler", "--save_intermediate_models", "--max_epochs", "5"], checkpoint_file=checkpoint_file)
+
+        save_path = os.path.split(save_file)[0]
+
+        initial_model_file = glob.glob(os.path.join(save_path, "*E0000*"))
+        assert len(initial_model_file) == 1
+        initial_model_file = initial_model_file[0]
+        initial_model = torch.load(initial_model_file, lambda storage, loc: storage)
+
+        second_model_file = glob.glob(os.path.join(save_path, "*E0002*"))
+        assert len(second_model_file) == 1
+        second_model_file = second_model_file[0]
+        second_model = torch.load(second_model_file, lambda storage, loc: storage)
+
+        final_model_file = glob.glob(os.path.join(save_path, "*E0005*"))
+        assert len(final_model_file) == 1
+        final_model_file = final_model_file[0]
+        final_model = torch.load(final_model_file, lambda storage, loc: storage)
+
+        # params in initial_model & second_model start with "base_model.model."
+        # whereas params in final_model start directly with "encoder" or "pooler"
+        initial_lora = initial_model['params']['bert_lora']
+        second_lora = second_model['params']['bert_lora']
+        final_lora = final_model['params']['bert_lora']
+        for side in ("_A.", "_B."):
+            for layer in (".0.", ".1."):
+                initial_params = sorted([x for x in initial_lora if x.find(".encoder.") > 0 and x.find(side) > 0 and x.find(layer) > 0])
+                second_params = sorted([x for x in second_lora if x.find(".encoder.") > 0 and x.find(side) > 0 and x.find(layer) > 0])
+                final_params = sorted([x for x in final_lora if x.startswith("encoder.") > 0 and x.find(side) > 0 and x.find(layer) > 0])
+                assert len(initial_params) > 0
+                assert len(initial_params) == len(second_params)
+                assert len(initial_params) == len(final_params)
+                for x, y in zip(second_params, final_params):
+                    assert x.endswith(y)
+                    if side != "_A.":  # the A tensors don't move very much, if at all
+                        assert not torch.allclose(initial_lora.get(x), second_lora.get(x))
+                        assert not torch.allclose(second_lora.get(x), final_lora.get(y))
+
```

### Comparing `stanza-1.8.1/stanza/tests/classifiers/test_constituency_classifier.py` & `stanza-1.8.2/stanza/tests/classifiers/test_constituency_classifier.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/tests/classifiers/test_data.py` & `stanza-1.8.2/stanza/tests/classifiers/test_data.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/tests/classifiers/test_process_utils.py` & `stanza-1.8.2/stanza/tests/classifiers/test_process_utils.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/tests/common/test_char_model.py` & `stanza-1.8.2/stanza/tests/common/test_char_model.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/tests/common/test_chuliu_edmonds.py` & `stanza-1.8.2/stanza/tests/common/test_chuliu_edmonds.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/tests/common/test_common_data.py` & `stanza-1.8.2/stanza/tests/common/test_common_data.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/tests/common/test_confusion.py` & `stanza-1.8.2/stanza/tests/common/test_confusion.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/tests/common/test_constant.py` & `stanza-1.8.2/stanza/tests/common/test_constant.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/tests/common/test_data_conversion.py` & `stanza-1.8.2/stanza/tests/common/test_data_conversion.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/tests/common/test_data_objects.py` & `stanza-1.8.2/stanza/tests/common/test_data_objects.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/tests/common/test_doc.py` & `stanza-1.8.2/stanza/tests/common/test_doc.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/tests/common/test_dropout.py` & `stanza-1.8.2/stanza/tests/common/test_dropout.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/tests/common/test_foundation_cache.py` & `stanza-1.8.2/stanza/tests/common/test_foundation_cache.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/tests/common/test_pretrain.py` & `stanza-1.8.2/stanza/tests/common/test_pretrain.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/tests/common/test_short_name_to_treebank.py` & `stanza-1.8.2/stanza/tests/common/test_short_name_to_treebank.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/tests/common/test_utils.py` & `stanza-1.8.2/stanza/tests/common/test_utils.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/tests/constituency/test_convert_arboretum.py` & `stanza-1.8.2/stanza/tests/constituency/test_convert_arboretum.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/tests/constituency/test_convert_it_vit.py` & `stanza-1.8.2/stanza/tests/constituency/test_convert_it_vit.py`

 * *Files 1% similar despite different names*

```diff
@@ -193,15 +193,14 @@
     mwt_map = convert_it_vit.get_mwt(ud_train_data)
     expected_trees=["(ROOT (cp (sp (part In) (sn (art gli) (sa (ag ultimi)) (nt anni))) (f (sn (art la) (n dinamica) (spd (partd di) (sn (art i) (n polo) (n di) (n attrazione)))) (ibar (ause è) (ausep stata) (savv (savv (avv sempre)) (avv più)) (vppt caratterizzata)) (compin (spda (partda da) (sn (art l') (n emergere) (spd (pd di) (sn (art una) (sa (ag crescente)) (n concorrenza) (f2 (rel che) (f (ibar (clit si) (ause è) (avv progressivamente) (vppin spostata)) (compin (spda (partda da) (sn (art le) (sa (ag singole)) (n imprese))) (sp (part a) (sn (art i) (n sistemi) (sa (coord (ag economici) (cong e) (ag territoriali))))) (fp (punt ,) (sv5 (vgt determinando) (compt (sn (art l') (nf esigenza) (spd (pd di) (sn (art una) (n riconsiderazione) (spd (partd di) (sn (art i) (n rapporti) (sv3 (ppre esistenti) (compin (sp (p tra) (sn (n soggetti) (sa (ag produttivi)))) (cong e) (sn (n ambiente) (f2 (sp (p in) (sn (relob cui))) (f (sn (deit questi)) (ibar (vin operano) (punto .))))))))))))))))))))))))))",
                     "(ROOT (dirsp (fc (congf tuttavia) (f (sn (sq (ind qualche)) (n problema)) (ir_infl (vsupir potrebbe) (vcl esserci)) (compc (clit ci) (sp (p per) (sn (art la) (n commissione) (sa (ag esteri)) (f2 (sp (part a) (art la) (relob cui) (sn (n presidenza))) (f (ibar (vc è)) (compc (sn (n candidato)) (sn (art l) (n esponente) (spd (pd di) (sn (mw Alleanza) (npro Nazionale))) (sn (mw Mirko) (nh Tremaglia))))))))))) (dirs :) (f3 (sn (art una) (n candidatura) (sc (q più) (sa (ppas subìta)) (sc (ccong che) (sa (ppas gradita))) (compt (spda (partda da) (sn (art la) (mw Lega) (npro Nord) (punt ,) (f2 (rel che) (fc (congf tuttavia) (f (ir_infl (vsupir dovrebbe) (vit rispettare)) (compt (sn (art gli) (n accordi))))))))))) (punto .))))",
                     "(ROOT (f (sn (art l) (n ottimismo) (spd (pd di) (sn (nh Kantor)))) (ir_infl (vsupir potrebbe) (congf però) (vcl rivelarsi)) (compc (clit si) (sn (in ancora) (art una) (nt volta)) (sa (ag prematuro))) (punto .)))"]
     with tsurgeon.Tsurgeon() as tsurgeon_processor:
         for con_sentence, ud_sentence, expected_tree in zip(con_sentences, ud_train_data.sentences, expected_trees):
             con_tree = convert_it_vit.raw_tree(con_sentence[1])
-            # the moveprune feature requires corenlp 4.5.0 or later
             updated_tree, _ = convert_it_vit.update_mwts_and_special_cases(con_tree, ud_sentence, mwt_map, tsurgeon_processor)
             assert str(updated_tree) == expected_tree
 
 
 CON_PERCENT_SAMPLE = """
 ID#sent_00020 f-[sn-[art-il, n-tesoro], ibar-[vt-mette], compt-[sp-[part-sul, sn-[n-mercato]], sn-[art-il, num-51%, sp-[p-a, sn-[num-2, n-lire]], sp-[p-per, sn-[n-azione]]]], punto-.]
 ID#sent_00022 dirsp-[f3-[sn-[art-le, n-novità]], dirs-':', f3-[coord-[sn-[n-voto, spd-[pd-di, sn-[n-lista]]], cong-e, sn-[n-tetto, sp-[part-agli, sn-[n-acquisti]], sv3-[vppt-limitato, comppas-[sp-[part-allo, sn-[num-0/5%]]]]]], punto-.]]
```

### Comparing `stanza-1.8.1/stanza/tests/constituency/test_convert_starlang.py` & `stanza-1.8.2/stanza/tests/constituency/test_convert_starlang.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/tests/constituency/test_in_order_oracle.py` & `stanza-1.8.2/stanza/tests/constituency/test_in_order_oracle.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/tests/constituency/test_lstm_model.py` & `stanza-1.8.2/stanza/tests/constituency/test_lstm_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,35 +64,35 @@
     functional model.
     """
     states = test_parse_transitions.build_initial_state(model, num_states)
     model(states)
 
     shift = parse_transitions.Shift()
     shifts = [shift for _ in range(num_states)]
-    states = parse_transitions.bulk_apply(model, states, shifts)
+    states = model.bulk_apply(states, shifts)
     model(states)
 
     open_transition = parse_transitions.OpenConstituent("NP")
     open_transitions = [open_transition for _ in range(num_states)]
     assert open_transition.is_legal(states[0], model)
-    states = parse_transitions.bulk_apply(model, states, open_transitions)
+    states = model.bulk_apply(states, open_transitions)
     assert states[0].num_opens == 1
     model(states)
 
-    states = parse_transitions.bulk_apply(model, states, shifts)
+    states = model.bulk_apply(states, shifts)
     model(states)
-    states = parse_transitions.bulk_apply(model, states, shifts)
+    states = model.bulk_apply(states, shifts)
     model(states)
     assert states[0].num_opens == 1
     # now should have "mox", "opal" on the constituents
 
     close_transition = parse_transitions.CloseConstituent()
     close_transitions = [close_transition for _ in range(num_states)]
     assert close_transition.is_legal(states[0], model)
-    states = parse_transitions.bulk_apply(model, states, close_transitions)
+    states = model.bulk_apply(states, close_transitions)
     assert states[0].num_opens == 0
 
     model(states)
 
 def test_unary_forward(unary_model):
     """
     Checks that the forward pass doesn't crash when run after various operations
@@ -480,18 +480,18 @@
     assert torch.allclose(torch.linalg.norm(model.word_lstm.weight_ih_l0), torch.linalg.norm(other.word_lstm.weight_ih_l0))
 
     # now, check that applying one transition to an initial state
     # results in the same values in the output states for both models
     # as the pattn layer inputs are 0, the output values should be equal
     shift = [parse_transitions.Shift()]
     model_states = test_parse_transitions.build_initial_state(model, 1)
-    model_states = parse_transitions.bulk_apply(model, model_states, shift)
+    model_states = model.bulk_apply(model_states, shift)
 
     other_states = test_parse_transitions.build_initial_state(other, 1)
-    other_states = parse_transitions.bulk_apply(other, other_states, shift)
+    other_states = other.bulk_apply(other_states, shift)
 
     for i, j in zip(other_states[0].word_queue, model_states[0].word_queue):
         assert torch.allclose(i.hx, j.hx, atol=1e-07)
     for i, j in zip(other_states[0].transitions, model_states[0].transitions):
         assert torch.allclose(i.lstm_hx, j.lstm_hx)
         assert torch.allclose(i.lstm_cx, j.lstm_cx)
     for i, j in zip(other_states[0].constituents, model_states[0].constituents):
```

### Comparing `stanza-1.8.1/stanza/tests/constituency/test_parse_transitions.py` & `stanza-1.8.2/stanza/tests/constituency/test_parse_transitions.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/tests/constituency/test_parse_tree.py` & `stanza-1.8.2/stanza/tests/constituency/test_parse_tree.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/tests/constituency/test_positional_encoding.py` & `stanza-1.8.2/stanza/tests/constituency/test_positional_encoding.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/tests/constituency/test_selftrain_vi_quad.py` & `stanza-1.8.2/stanza/tests/constituency/test_selftrain_vi_quad.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/tests/constituency/test_top_down_oracle.py` & `stanza-1.8.2/stanza/tests/constituency/test_top_down_oracle.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/tests/constituency/test_trainer.py` & `stanza-1.8.2/stanza/tests/constituency/test_trainer.py`

 * *Files 0% similar despite different names*

```diff
@@ -212,31 +212,32 @@
                 if args['grad_clipping'] is not None:
                     assert len(p._backward_hooks) == 1
                 else:
                     assert p._backward_hooks is None
 
         # check that the model can be loaded back
         assert os.path.exists(args['save_name'])
-        tr = trainer.Trainer.load(args['save_name'], load_optimizer=True, foundation_cache=retag_pipeline.foundation_cache)
+        peft_name = trained_model.model.peft_name
+        tr = trainer.Trainer.load(args['save_name'], load_optimizer=True, foundation_cache=retag_pipeline.foundation_cache, peft_name=trained_model.model.peft_name)
         assert tr.optimizer is not None
         assert tr.scheduler is not None
         assert tr.epochs_trained >= 1
         for p in tr.model.parameters():
             if p.requires_grad:
                 assert p._backward_hooks is None
 
-        tr = trainer.Trainer.load(args['checkpoint_save_name'], load_optimizer=True, foundation_cache=retag_pipeline.foundation_cache)
+        tr = trainer.Trainer.load(args['checkpoint_save_name'], load_optimizer=True, foundation_cache=retag_pipeline.foundation_cache, peft_name=trained_model.model.peft_name)
         assert tr.optimizer is not None
         assert tr.scheduler is not None
         assert tr.epochs_trained == num_epochs
 
         for i in range(1, num_epochs+1):
             model_name = each_name % i
             assert os.path.exists(model_name)
-            tr = trainer.Trainer.load(model_name, load_optimizer=True, foundation_cache=retag_pipeline.foundation_cache)
+            tr = trainer.Trainer.load(model_name, load_optimizer=True, foundation_cache=retag_pipeline.foundation_cache, peft_name=trained_model.model.peft_name)
             assert tr.epochs_trained == i
             assert tr.batches_trained == (4 * i if use_silver else 2 * i)
 
         return args, trained_model
 
     def test_train(self, wordvec_pretrain_file):
         """
@@ -575,19 +576,18 @@
 
     def test_bert_finetune_one_layer(self, wordvec_pretrain_file):
         self.one_layer_finetune_transformer_test(wordvec_pretrain_file, 'hf-internal-testing/tiny-bert')
 
     def test_xlnet_finetune_one_layer(self, wordvec_pretrain_file, tiny_random_xlnet):
         self.one_layer_finetune_transformer_test(wordvec_pretrain_file, tiny_random_xlnet)
 
-    def test_peft_finetune(self, wordvec_pretrain_file):
-        with tempfile.TemporaryDirectory(dir=TEST_WORKING_DIR) as tmpdirname:
-            transformer_name = 'hf-internal-testing/tiny-bert'
-            args = ['--bert_model', transformer_name, '--bert_finetune', '--optim', 'adamw', '--use_peft']
-            args, trained_model = self.run_train_test(wordvec_pretrain_file, tmpdirname, extra_args=args)
+    def test_peft_finetune(self, tmp_path, wordvec_pretrain_file):
+        transformer_name = 'hf-internal-testing/tiny-bert'
+        args = ['--bert_model', transformer_name, '--bert_finetune', '--optim', 'adamw', '--use_peft']
+        args, trained_model = self.run_train_test(wordvec_pretrain_file, str(tmp_path), extra_args=args)
 
     def test_peft_twostage_finetune(self, wordvec_pretrain_file):
         with tempfile.TemporaryDirectory(dir=TEST_WORKING_DIR) as tmpdirname:
             num_epochs = 6
             transformer_name = 'hf-internal-testing/tiny-bert'
             args = ['--bert_model', transformer_name, '--stage1_bert_finetune', '--optim', 'adamw', '--use_peft']
             args, trained_model = self.run_train_test(wordvec_pretrain_file, tmpdirname, num_epochs=num_epochs, extra_args=args)
```

### Comparing `stanza-1.8.1/stanza/tests/constituency/test_transformer_tree_stack.py` & `stanza-1.8.2/stanza/tests/constituency/test_transformer_tree_stack.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/tests/constituency/test_transition_sequence.py` & `stanza-1.8.2/stanza/tests/constituency/test_transition_sequence.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     states = model.initial_state_from_gold_trees([tree])
     assert(len(states)) == 1
     assert states[0].num_transitions() == 0
 
     # TODO: could fold this into parse_sentences (similar to verify_transitions in trainer.py)
     for idx, t in enumerate(sequence):
         assert t.is_legal(states[0], model), "Transition {} not legal at step {} in sequence {}".format(t, idx, sequence)
-        states = parse_transitions.bulk_apply(model, states, [t])
+        states = model.bulk_apply(states, [t])
 
     result_tree = states[0].constituents.value
     if reverse:
         result_tree = result_tree.reverse()
     return result_tree
 
 def check_reproduce_tree(transition_scheme):
```

### Comparing `stanza-1.8.1/stanza/tests/constituency/test_tree_reader.py` & `stanza-1.8.2/stanza/tests/constituency/test_tree_reader.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/tests/constituency/test_tree_stack.py` & `stanza-1.8.2/stanza/tests/constituency/test_tree_stack.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/tests/constituency/test_utils.py` & `stanza-1.8.2/stanza/tests/constituency/test_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -50,19 +50,19 @@
     """
     text = "((S (VP (X Find)) (NP (X Mox) (X Opal))))"
     expected = "((S (VP (A Find)) (NP (B Mox) (C Opal))))"
 
     trees = tree_reader.read_trees(text)
 
     new_tags = ["A", "B", "C"]
-    new_tree = utils.replace_tags(trees[0], new_tags)
+    new_tree = trees[0].replace_tags(new_tags)
 
     assert new_tree == tree_reader.read_trees(expected)[0]
 
     with pytest.raises(ValueError):
         new_tags = ["A", "B"]
-        new_tree = utils.replace_tags(trees[0], new_tags)
+        new_tree = trees[0].replace_tags(new_tags)
 
     with pytest.raises(ValueError):
         new_tags = ["A", "B", "C", "D"]
-        new_tree = utils.replace_tags(trees[0], new_tags)
+        new_tree = trees[0].replace_tags(new_tags)
```

### Comparing `stanza-1.8.1/stanza/tests/constituency/test_vietnamese.py` & `stanza-1.8.2/stanza/tests/constituency/test_vietnamese.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/tests/datasets/ner/test_prepare_ner_file.py` & `stanza-1.8.2/stanza/tests/datasets/ner/test_prepare_ner_file.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/tests/datasets/ner/test_utils.py` & `stanza-1.8.2/stanza/tests/datasets/ner/test_utils.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/tests/datasets/test_common.py` & `stanza-1.8.2/stanza/tests/datasets/test_common.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/tests/datasets/test_vietnamese_renormalization.py` & `stanza-1.8.2/stanza/tests/datasets/test_vietnamese_renormalization.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/tests/depparse/test_depparse_data.py` & `stanza-1.8.2/stanza/tests/depparse/test_depparse_data.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/tests/depparse/test_parser.py` & `stanza-1.8.2/stanza/tests/depparse/test_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,15 +93,14 @@
 
         with open(dev_file, "w", encoding="utf-8") as fout:
             fout.write(dev_text)
 
         args = ["--wordvec_pretrain_file", wordvec_pretrain_file,
                 "--train_file", train_file,
                 "--eval_file", dev_file,
-                "--gold_file", dev_file,
                 "--output_file", pred_file,
                 "--log_step", "10",
                 "--eval_interval", "20",
                 "--max_steps", "100",
                 "--shorthand", "en_test",
                 "--save_dir", str(tmp_path),
                 "--save_name", save_name,
```

### Comparing `stanza-1.8.1/stanza/tests/langid/test_langid.py` & `stanza-1.8.2/stanza/tests/langid/test_langid.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/tests/langid/test_multilingual.py` & `stanza-1.8.2/stanza/tests/langid/test_multilingual.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/tests/lemma/test_data.py` & `stanza-1.8.2/stanza/tests/lemma/test_data.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/tests/lemma/test_lemma_trainer.py` & `stanza-1.8.2/stanza/tests/lemma/test_lemma_trainer.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/tests/lemma/test_lowercase.py` & `stanza-1.8.2/stanza/tests/lemma/test_lowercase.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/tests/mwt/test_utils.py` & `stanza-1.8.2/stanza/tests/mwt/test_utils.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/tests/ner/test_bsf_2_beios.py` & `stanza-1.8.2/stanza/tests/ner/test_bsf_2_beios.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/tests/ner/test_bsf_2_iob.py` & `stanza-1.8.2/stanza/tests/ner/test_bsf_2_iob.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/tests/ner/test_combine_ner_datasets.py` & `stanza-1.8.2/stanza/tests/ner/test_combine_ner_datasets.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/tests/ner/test_convert_amt.py` & `stanza-1.8.2/stanza/tests/ner/test_convert_amt.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/tests/ner/test_convert_nkjp.py` & `stanza-1.8.2/stanza/tests/ner/test_convert_nkjp.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/tests/ner/test_convert_starlang_ner.py` & `stanza-1.8.2/stanza/tests/ner/test_convert_starlang_ner.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/tests/ner/test_models_ner_scorer.py` & `stanza-1.8.2/stanza/tests/ner/test_models_ner_scorer.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/tests/ner/test_ner_tagger.py` & `stanza-1.8.2/stanza/tests/ner/test_ner_tagger.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/tests/ner/test_ner_trainer.py` & `stanza-1.8.2/stanza/tests/ner/test_ner_trainer.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/tests/ner/test_ner_training.py` & `stanza-1.8.2/stanza/tests/ner/test_ner_training.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/tests/ner/test_ner_utils.py` & `stanza-1.8.2/stanza/tests/ner/test_ner_utils.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/tests/ner/test_pay_amt_annotators.py` & `stanza-1.8.2/stanza/tests/ner/test_pay_amt_annotators.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/tests/ner/test_split_wikiner.py` & `stanza-1.8.2/stanza/tests/ner/test_split_wikiner.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/tests/ner/test_suc3.py` & `stanza-1.8.2/stanza/tests/ner/test_suc3.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/tests/pipeline/pipeline_device_tests.py` & `stanza-1.8.2/stanza/tests/pipeline/pipeline_device_tests.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/tests/pipeline/test_arabic_pipeline.py` & `stanza-1.8.2/stanza/tests/pipeline/test_arabic_pipeline.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/tests/pipeline/test_core.py` & `stanza-1.8.2/stanza/tests/pipeline/test_core.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/tests/pipeline/test_decorators.py` & `stanza-1.8.2/stanza/tests/pipeline/test_decorators.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/tests/pipeline/test_depparse.py` & `stanza-1.8.2/stanza/tests/pipeline/test_depparse.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/tests/pipeline/test_english_pipeline.py` & `stanza-1.8.2/stanza/tests/pipeline/test_english_pipeline.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/tests/pipeline/test_french_pipeline.py` & `stanza-1.8.2/stanza/tests/pipeline/test_french_pipeline.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/tests/pipeline/test_lemmatizer.py` & `stanza-1.8.2/stanza/tests/pipeline/test_lemmatizer.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/tests/pipeline/test_pipeline_constituency_processor.py` & `stanza-1.8.2/stanza/tests/pipeline/test_pipeline_constituency_processor.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/tests/pipeline/test_pipeline_depparse_processor.py` & `stanza-1.8.2/stanza/tests/pipeline/test_pipeline_depparse_processor.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/tests/pipeline/test_pipeline_mwt_expander.py` & `stanza-1.8.2/stanza/tests/pipeline/test_pipeline_mwt_expander.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
 
 import pytest
 import stanza
 
 from stanza.tests import *
 
-pytestmark = pytest.mark.pipeline
+pytestmark = [pytest.mark.pipeline, pytest.mark.travis]
 
 # mwt data for testing
 FR_MWT_SENTENCE = "Alors encore inconnu du grand public, Emmanuel Macron devient en 2014 ministre de l'Économie, de " \
                   "l'Industrie et du Numérique."
 
 
 FR_MWT_TOKEN_TO_WORDS_GOLD = """
```

### Comparing `stanza-1.8.1/stanza/tests/pipeline/test_pipeline_ner_processor.py` & `stanza-1.8.2/stanza/tests/pipeline/test_pipeline_ner_processor.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/tests/pipeline/test_pipeline_pos_processor.py` & `stanza-1.8.2/stanza/tests/pipeline/test_pipeline_pos_processor.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/tests/pipeline/test_pipeline_sentiment_processor.py` & `stanza-1.8.2/stanza/tests/pipeline/test_pipeline_sentiment_processor.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/tests/pipeline/test_requirements.py` & `stanza-1.8.2/stanza/tests/pipeline/test_requirements.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/tests/pipeline/test_tokenizer.py` & `stanza-1.8.2/stanza/tests/pipeline/test_tokenizer.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/tests/pos/test_tagger.py` & `stanza-1.8.2/stanza/tests/pos/test_tagger.py`

 * *Files 0% similar despite different names*

```diff
@@ -284,9 +284,9 @@
     def test_with_bert(self, tmp_path, wordvec_pretrain_file):
         self.run_training(tmp_path, wordvec_pretrain_file, TRAIN_DATA, DEV_DATA, extra_args=['--bert_model', 'hf-internal-testing/tiny-bert'])
 
     def test_with_bert_nlayers(self, tmp_path, wordvec_pretrain_file):
         self.run_training(tmp_path, wordvec_pretrain_file, TRAIN_DATA, DEV_DATA, extra_args=['--bert_model', 'hf-internal-testing/tiny-bert', '--bert_hidden_layers', '2'])
 
     def test_with_bert_finetune(self, tmp_path, wordvec_pretrain_file):
-        self.run_training(tmp_path, wordvec_pretrain_file, TRAIN_DATA, DEV_DATA, extra_args=['--bert_model', 'hf-internal-testing/tiny-bert', '--bert_finetune', '--bert_learning_rate', '0.01'])
+        self.run_training(tmp_path, wordvec_pretrain_file, TRAIN_DATA, DEV_DATA, extra_args=['--bert_model', 'hf-internal-testing/tiny-bert', '--bert_finetune', '--bert_learning_rate', '0.01', '--bert_hidden_layers', '2'])
```

### Comparing `stanza-1.8.1/stanza/tests/pos/test_xpos_vocab_factory.py` & `stanza-1.8.2/stanza/tests/pos/test_xpos_vocab_factory.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/tests/resources/test_charlm_depparse.py` & `stanza-1.8.2/stanza/tests/resources/test_charlm_depparse.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/tests/resources/test_common.py` & `stanza-1.8.2/stanza/tests/resources/test_common.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/tests/resources/test_default_packages.py` & `stanza-1.8.2/stanza/tests/resources/test_default_packages.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/tests/resources/test_installation.py` & `stanza-1.8.2/stanza/tests/resources/test_installation.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/tests/resources/test_prepare_resources.py` & `stanza-1.8.2/stanza/tests/resources/test_prepare_resources.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/tests/server/test_client.py` & `stanza-1.8.2/stanza/tests/server/test_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -157,16 +157,14 @@
                        'spanString': 'with Stanford CoreNLP', 'namedNodes': []}}
             ]
         }
 
     def test_tregex_trees(self, corenlp_client):
         """
         Test the results of tregex run on trees w/o parsing
-
-        TODO: this needs a CoreNLP more recent than 4.5.1
         """
         trees = tree_reader.read_trees("(ROOT (S (NP (NNP Jennifer)) (VP (VBZ has) (NP (JJ blue) (NN skin)))))   (ROOT (S (NP (PRP I)) (VP (VBP like) (NP (PRP$ her) (NNS antennae)))))")
         pattern = "VP < NP"
         matches = corenlp_client.tregex(pattern=pattern, trees=trees)
         assert matches == {
             'sentences': [
                 {'0': {'sentIndex': 0, 'match': '(VP (VBZ has)\n  (NP (JJ blue) (NN skin)))\n', 'spanString': 'has blue skin', 'namedNodes': []}},
```

### Comparing `stanza-1.8.1/stanza/tests/server/test_java_protobuf_requests.py` & `stanza-1.8.2/stanza/tests/server/test_java_protobuf_requests.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/tests/server/test_morphology.py` & `stanza-1.8.2/stanza/tests/server/test_morphology.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/tests/server/test_parser_eval.py` & `stanza-1.8.2/stanza/tests/server/test_parser_eval.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/tests/server/test_protobuf.py` & `stanza-1.8.2/stanza/tests/server/test_protobuf.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/tests/server/test_server_misc.py` & `stanza-1.8.2/stanza/tests/server/test_server_misc.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/tests/server/test_server_pretokenized.py` & `stanza-1.8.2/stanza/tests/server/test_server_pretokenized.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/tests/server/test_server_request.py` & `stanza-1.8.2/stanza/tests/server/test_server_request.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/tests/server/test_server_start.py` & `stanza-1.8.2/stanza/tests/server/test_server_start.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/tests/server/test_ssurgeon.py` & `stanza-1.8.2/stanza/tests/server/test_ssurgeon.py`

 * *Files 14% similar despite different names*

```diff
@@ -369,7 +369,57 @@
     Check the SpaceAfter=No on an MWT (rather than a word)
 
     the RandomFeature=foo is on account of a silly bug in the initial
     version of passing in MWT misc features
     """
     check_empty_test(ITALIAN_MWT_MISC_INPUT)
 
+SINDHI_ROOT_EXAMPLE = """
+# sent_id = 1
+# text = غلام رهڻ سان ماڻهو منافق ٿئي ٿو .
+1	غلام	غلام	NOUN	NN__اسم	Case=Acc|Gender=Masc|Number=Sing|Person=3	2	compound	_	_
+2	رهڻ	ره	VERB	VB__فعل	Number=Sing	6	advcl	_	_
+3	سان	سان	ADP	IN__حرفِ_جر	Number=Sing	2	mark	_	_
+4	ماڻهو	ماڻهو	NOUN	NN__اسم	Case=Nom|Gender=Masc|Number=Sing|Person=3	6	nsubj	_	_
+5	منافق	منافق	ADJ	JJ__صفت	Case=Acc|Number=Sing|Person=3	6	xcomp	_	_
+6	ٿئي	ٿي	VERB	VB__فعل	Number=Sing	_	_	_	_
+7	ٿو	ٿو	AUX	VB__فعل	Number=Sing	6	aux	_	_
+8	.	.	PUNCT	-__پورو_دم	_	6	punct	_	_
+""".lstrip()
+
+SINDHI_ROOT_EXPECTED = """
+# sent_id = 1
+# text = غلام رهڻ سان ماڻهو منافق ٿئي ٿو .
+1	غلام	غلام	NOUN	NN__اسم	Case=Acc|Gender=Masc|Number=Sing|Person=3	2	compound	_	_
+2	رهڻ	ره	VERB	VB__فعل	Number=Sing	6	advcl	_	_
+3	سان	سان	ADP	IN__حرفِ_جر	Number=Sing	2	mark	_	_
+4	ماڻهو	ماڻهو	NOUN	NN__اسم	Case=Nom|Gender=Masc|Number=Sing|Person=3	6	nsubj	_	_
+5	منافق	منافق	ADJ	JJ__صفت	Case=Acc|Number=Sing|Person=3	6	xcomp	_	_
+6	ٿئي	ٿي	VERB	VB__فعل	Number=Sing	0	root	_	_
+7	ٿو	ٿو	AUX	VB__فعل	Number=Sing	6	aux	_	_
+8	.	.	PUNCT	-__پورو_دم	_	6	punct	_	_
+""".strip()
+
+SINDHI_EDIT = """
+{}=root !< {}
+setRoots root
+"""
+
+def test_ssurgeon_rewrite_sindhi_roots():
+    """
+    A user / contributor sent a dependency file with blank roots
+    """
+    edits = ssurgeon.parse_ssurgeon_edits(SINDHI_EDIT)
+    expected_edits = [ssurgeon.SsurgeonEdit(semgrex_pattern='{}=root !< {}',
+                                            ssurgeon_edits=['setRoots root'],
+                                            ssurgeon_id='1', notes='', language='UniversalEnglish')]
+    assert edits == expected_edits
+
+    blank_dep_doc = CoNLL.conll2doc(input_str=SINDHI_ROOT_EXAMPLE)
+    # test that the conversion will work w/o crashing, such as because of a missing root edge
+    request = ssurgeon.build_request(blank_dep_doc, edits)
+
+    response = ssurgeon.process_doc(blank_dep_doc, edits)
+    updated_doc = ssurgeon.convert_response_to_doc(blank_dep_doc, response)
+
+    result = "{:C}".format(updated_doc)
+    assert result == SINDHI_ROOT_EXPECTED
```

### Comparing `stanza-1.8.1/stanza/tests/server/test_tokensregex.py` & `stanza-1.8.2/stanza/tests/server/test_tokensregex.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/tests/server/test_tsurgeon.py` & `stanza-1.8.2/stanza/tests/server/test_tsurgeon.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/tests/server/test_ud_enhancer.py` & `stanza-1.8.2/stanza/tests/server/test_ud_enhancer.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/tests/setup.py` & `stanza-1.8.2/stanza/tests/setup.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/tests/tokenization/test_prepare_tokenizer_treebank.py` & `stanza-1.8.2/stanza/tests/tokenization/test_prepare_tokenizer_treebank.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/tests/tokenization/test_replace_long_tokens.py` & `stanza-1.8.2/stanza/tests/tokenization/test_replace_long_tokens.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/tests/tokenization/test_spaces.py` & `stanza-1.8.2/stanza/tests/tokenization/test_spaces.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,16 +35,16 @@
     result = result.strip()
     assert EXPECTED_NO_MWT == result
 
 EXPECTED_MWT = """
 # text = She's not a nice person.
 # sent_id = 0
 1-2	She's	_	_	_	_	_	_	_	start_char=2|end_char=7|SpacesBefore=\\s\\s
-1	She	_	_	_	_	0	_	_	_
-2	's	_	_	_	_	1	_	_	_
+1	She	_	_	_	_	0	_	_	start_char=2|end_char=5
+2	's	_	_	_	_	1	_	_	start_char=5|end_char=7
 3	not	_	_	_	_	2	_	_	start_char=8|end_char=11
 4	a	_	_	_	_	3	_	_	start_char=12|end_char=13
 5	nice	_	_	_	_	4	_	_	start_char=14|end_char=18
 6	person	_	_	_	_	5	_	_	start_char=19|end_char=25|SpaceAfter=No
 7	.	_	_	_	_	6	_	_	start_char=25|end_char=26|SpacesAfter=\\s\\s
 
 # text = However, the best antennae on the Cerritos are Jennifer's.
@@ -55,16 +55,16 @@
 4	best	_	_	_	_	3	_	_	start_char=41|end_char=45
 5	antennae	_	_	_	_	4	_	_	start_char=46|end_char=54
 6	on	_	_	_	_	5	_	_	start_char=55|end_char=57
 7	the	_	_	_	_	6	_	_	start_char=58|end_char=61
 8	Cerritos	_	_	_	_	7	_	_	start_char=62|end_char=70
 9	are	_	_	_	_	8	_	_	start_char=71|end_char=74
 10-11	Jennifer's	_	_	_	_	_	_	_	start_char=75|end_char=85|SpaceAfter=No
-10	Jennifer	_	_	_	_	9	_	_	_
-11	's	_	_	_	_	10	_	_	_
+10	Jennifer	_	_	_	_	9	_	_	start_char=75|end_char=83
+11	's	_	_	_	_	10	_	_	start_char=83|end_char=85
 12	.	_	_	_	_	11	_	_	start_char=85|end_char=86|SpacesAfter=\\s\\s
 """.strip()
 
 def test_spaces_mwt():
     """
     Similar to the above test, but now we test it with MWT
     """
```

### Comparing `stanza-1.8.1/stanza/tests/tokenization/test_tokenization_lst20.py` & `stanza-1.8.2/stanza/tests/tokenization/test_tokenization_lst20.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/tests/tokenization/test_tokenization_orchid.py` & `stanza-1.8.2/stanza/tests/tokenization/test_tokenization_orchid.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/tests/tokenization/test_tokenize_data.py` & `stanza-1.8.2/stanza/tests/tokenization/test_tokenize_data.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/tests/tokenization/test_tokenize_files.py` & `stanza-1.8.2/stanza/tests/tokenization/test_tokenize_files.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/tests/tokenization/test_tokenize_utils.py` & `stanza-1.8.2/stanza/tests/tokenization/test_tokenize_utils.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/utils/charlm/conll17_to_text.py` & `stanza-1.8.2/stanza/utils/charlm/conll17_to_text.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/utils/charlm/dump_oscar.py` & `stanza-1.8.2/stanza/utils/charlm/dump_oscar.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/utils/charlm/make_lm_data.py` & `stanza-1.8.2/stanza/utils/charlm/make_lm_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -138,20 +138,20 @@
         if total < 3:
             raise RuntimeError("Something went wrong!  %d file(s) produced by shuffle and split, expected at least 3" % total)
 
         dev_file = f"{tgt_dir}/dev.txt"
         test_file = f"{tgt_dir}/test.txt"
         if make_test_file:
             print("--> Creating dev and test files...")
-            shutil.move(f"{train_dir}/{lang}-{dataset_name}-000.txt", dev_file)
-            shutil.move(f"{train_dir}/{lang}-{dataset_name}-001.txt", test_file)
+            shutil.move(f"{train_dir}/{lang}-{dataset_name}-0000.txt", dev_file)
+            shutil.move(f"{train_dir}/{lang}-{dataset_name}-0001.txt", test_file)
             txt_files = [dev_file, test_file] + glob.glob(f'{train_dir}/*.txt')
         else:
             print("--> Creating dev file...")
-            shutil.move(f"{train_dir}/{lang}-{dataset_name}-000.txt", dev_file)
+            shutil.move(f"{train_dir}/{lang}-{dataset_name}-0000.txt", dev_file)
             txt_files = [dev_file] + glob.glob(f'{train_dir}/*.txt')
 
         if compress:
             print("--> Compressing files...")
             for txt_file in tqdm(txt_files):
                 subprocess.run(['xz', txt_file])
```

### Comparing `stanza-1.8.1/stanza/utils/charlm/oscar_to_text.py` & `stanza-1.8.2/stanza/utils/charlm/oscar_to_text.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/utils/confusion.py` & `stanza-1.8.2/stanza/utils/confusion.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/utils/conll.py` & `stanza-1.8.2/stanza/utils/conll.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/utils/conll18_ud_eval.py` & `stanza-1.8.2/stanza/utils/conll18_ud_eval.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/utils/datasets/add_fake_dependencies.py` & `stanza-1.8.2/stanza/utils/datasets/add_fake_dependencies.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/utils/datasets/common.py` & `stanza-1.8.2/stanza/utils/datasets/common.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/utils/datasets/conllu_to_text.pl` & `stanza-1.8.2/stanza/utils/datasets/conllu_to_text.pl`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/utils/datasets/constituency/build_silver_dataset.py` & `stanza-1.8.2/stanza/utils/datasets/constituency/build_silver_dataset.py`

 * *Files 25% similar despite different names*

```diff
@@ -2,25 +2,27 @@
 Given two ensembles and a tokenized file, output the trees for which those ensembles agree and report how many of the sub-models agree on those trees.
 
 For example:
 
 python3 -m stanza.utils.datasets.constituency.build_silver_dataset --tokenized_file /u/nlp/data/constituency-parser/italian/2024_wiki_tokenization/it_wiki_tokenized_AA.txt --lang it --output_file asdf.out --e1 saved_models/constituency/it_vit_electra_100?_top_constituency.pt --e2 saved_models/constituency/it_vit_electra_100?_constituency.pt
 
 for i in `echo f g h i j k l m n o p q r s t`; do nlprun -d a6000 "python3 -m stanza.utils.datasets.constituency.build_silver_dataset --tokenized_file /u/nlp/data/constituency-parser/italian/2024_wiki_tokenization/it_wiki_tok_6M_a$i.txt --lang it --output_file /u/nlp/data/constituency-parser/italian/2024_it_vit_electra/a$i.trees --e1 saved_models/constituency/it_vit_electra_100?_top_constituency.pt --e2 saved_models/constituency/it_vit_electra_100?_constituency.pt" -o /u/nlp/data/constituency-parser/italian/2024_it_vit_electra/a$i.out; done
+
+for i in `echo a b c d`; do nlprun -d a6000 "python3 -m stanza.utils.datasets.constituency.build_silver_dataset --tokenized_file /u/nlp/data/constituency-parser/english/en_wiki_2023/shuf_1M.a$i --lang en --output_file /u/nlp/data/constituency-parser/english/2024_en_ptb3_electra/forward_a$i.trees --e1 saved_models/constituency/en_ptb3_electra-large_100?_in_constituency.pt --e2 saved_models/constituency/en_ptb3_electra-large_100?_top_constituency.pt" -o /u/nlp/data/constituency-parser/english/2024_en_ptb3_electra/forward_a$i.out; done
 """
 
 import argparse
 import json
 
 import logging
 
 from stanza.models.common import utils
 from stanza.models.common.foundation_cache import FoundationCache
 from stanza.models.constituency import retagging
-from stanza.models.constituency import trainer
+from stanza.models.constituency import text_processing
 from stanza.models.constituency.ensemble import Ensemble
 from stanza.utils.get_tqdm import get_tqdm
 
 tqdm = get_tqdm()
 
 logger = logging.getLogger('stanza.constituency.trainer')
 
@@ -40,14 +42,19 @@
 
     parser.add_argument('--eval_batch_size', type=int, default=50, help='How many trees to batch when running eval')
     parser.add_argument('--e1', type=str, nargs='+', default=None, help="Which model(s) to load in the first ensemble")
     parser.add_argument('--e2', type=str, nargs='+', default=None, help="Which model(s) to load in the second ensemble")
 
     parser.add_argument('--mode', default='predict', choices=['parse_text', 'predict'])
 
+    # another option would be to include the tree idx in each entry in an existing saved file
+    # the processing could then pick up at exactly the last known idx
+    parser.add_argument('--start_tree', type=int, default=0, help='Where to start... most useful if the previous incarnation crashed')
+    parser.add_argument('--end_tree', type=int, default=None, help='Where to end.  If unset, will process to the end of the file')
+
     retagging.add_retag_args(parser)
 
     args = vars(parser.parse_args())
 
     retagging.postprocess_args(args)
     args['num_generate'] = 0
 
@@ -61,27 +68,28 @@
     foundation_cache = retag_pipeline[0].foundation_cache if retag_pipeline else FoundationCache()
 
     logger.info("Building ensemble #1 out of %s", args['e1'])
     e1 = Ensemble(args['e1'], args, foundation_cache)
     logger.info("Building ensemble #2 out of %s", args['e2'])
     e2 = Ensemble(args['e2'], args, foundation_cache)
 
-    tokenized_sentences = trainer.read_tokenized_file(args['tokenized_file'])
+    tokenized_sentences = text_processing.read_tokenized_file(args['tokenized_file'])
     logger.info("Read %d tokenized sentences", len(tokenized_sentences))
 
     all_models = e1.models + e2.models
 
     chunk_size = 1000
     with open(args['output_file'], 'w', encoding='utf-8') as fout:
-        for chunk_start in tqdm(range(0, len(tokenized_sentences), chunk_size)):
+        end_tree = len(tokenized_sentences) if args['end_tree'] is None else args['end_tree']
+        for chunk_start in tqdm(range(args['start_tree'], end_tree, chunk_size)):
             chunk = tokenized_sentences[chunk_start:chunk_start+chunk_size]
             logger.info("Processing trees %d to %d", chunk_start, chunk_start+len(chunk))
-            parsed1 = trainer.parse_tokenized_sentences(args, e1, retag_pipeline, chunk)
+            parsed1 = text_processing.parse_tokenized_sentences(args, e1, retag_pipeline, chunk)
             parsed1 = [x.predictions[0].tree for x in parsed1]
-            parsed2 = trainer.parse_tokenized_sentences(args, e2, retag_pipeline, chunk)
+            parsed2 = text_processing.parse_tokenized_sentences(args, e2, retag_pipeline, chunk)
             parsed2 = [x.predictions[0].tree for x in parsed2]
             matching = [t for t, t2 in zip(parsed1, parsed2) if t == t2]
             logger.info("%d trees matched", len(matching))
             model_counts = [0] * len(matching)
             for model in all_models:
                 model_chunk = model.parse_sentences_no_grad(iter(matching), model.build_batch_from_trees, args['eval_batch_size'], model.predict)
                 model_chunk = [x.predictions[0].tree for x in model_chunk]
```

### Comparing `stanza-1.8.1/stanza/utils/datasets/constituency/convert_alt.py` & `stanza-1.8.2/stanza/utils/datasets/constituency/convert_alt.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/utils/datasets/constituency/convert_arboretum.py` & `stanza-1.8.2/stanza/utils/datasets/constituency/convert_arboretum.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/utils/datasets/constituency/convert_cintil.py` & `stanza-1.8.2/stanza/utils/datasets/constituency/convert_cintil.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/utils/datasets/constituency/convert_ctb.py` & `stanza-1.8.2/stanza/utils/datasets/constituency/convert_ctb.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/utils/datasets/constituency/convert_it_turin.py` & `stanza-1.8.2/stanza/utils/datasets/constituency/convert_it_turin.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/utils/datasets/constituency/convert_it_vit.py` & `stanza-1.8.2/stanza/utils/datasets/constituency/convert_it_vit.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/utils/datasets/constituency/convert_starlang.py` & `stanza-1.8.2/stanza/utils/datasets/constituency/convert_starlang.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/utils/datasets/constituency/extract_silver_dataset.py` & `stanza-1.8.2/stanza/utils/datasets/constituency/extract_silver_dataset.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/utils/datasets/constituency/prepare_con_dataset.py` & `stanza-1.8.2/stanza/utils/datasets/constituency/prepare_con_dataset.py`

 * *Files 3% similar despite different names*

```diff
@@ -160,14 +160,21 @@
 
 zh_ctb-90 is the 9.0 version of CTB
   put LDC2016T13 in $CONSTITUENCY_BASE/chinese
   python3 -m stanza.utils.datasets.constituency.prepare_con_dataset zh_ctb-90
 
   the splits used are the ones from the file docs/ctb9.0-file-list.txt
     included in the CTB 9.0 release
+
+SPMRL adds several treebanks
+  https://www.spmrl.org/
+  https://www.spmrl.org/sancl-posters2014.html
+  Currently only German is converted, the German version being a
+    version of the Tiger Treebank
+  python3 -m stanza.utils.datasets.constituency.prepare_con_dataset de_spmrl  
 """
 
 import argparse
 import os
 import random
 import sys
 import tempfile
@@ -182,14 +189,15 @@
 from stanza.utils.datasets.constituency import utils
 from stanza.utils.datasets.constituency.convert_alt import convert_alt
 from stanza.utils.datasets.constituency.convert_arboretum import convert_tiger_treebank
 from stanza.utils.datasets.constituency.convert_cintil import convert_cintil_treebank
 import stanza.utils.datasets.constituency.convert_ctb as convert_ctb
 from stanza.utils.datasets.constituency.convert_it_turin import convert_it_turin
 from stanza.utils.datasets.constituency.convert_it_vit import convert_it_vit
+from stanza.utils.datasets.constituency.convert_spmrl import convert_spmrl
 from stanza.utils.datasets.constituency.convert_starlang import read_starlang
 from stanza.utils.datasets.constituency.utils import SHARDS, write_dataset
 import stanza.utils.datasets.constituency.vtb_convert as vtb_convert
 import stanza.utils.datasets.constituency.vtb_split as vtb_split
 
 class UnknownDatasetError(ValueError):
     def __init__(self, dataset, text):
@@ -449,17 +457,28 @@
     test_trees = tree_reader.read_directory(os.path.join(bracket_dir, "23"))
     test_trees = [t.remap_constituent_labels(label_map) for t in test_trees]
     print("Read %d train trees, %d dev trees, and %d test trees" % (len(train_trees), len(dev_trees), len(test_trees)))
     datasets = [train_trees, dev_trees, test_trees]
     write_dataset(datasets, output_dir, dataset_name)
 
 
+def process_spmrl(paths, dataset_name, *args):
+    if dataset_name != 'de_spmrl':
+        raise ValueError("SPMRL dataset %s currently not supported" % dataset_name)
+
+    output_directory = paths["CONSTITUENCY_DATA_DIR"]
+    input_directory = os.path.join(paths["CONSTITUENCY_BASE"], "spmrl", "SPMRL_SHARED_2014", "GERMAN_SPMRL", "gold", "ptb")
+
+    convert_spmrl(input_directory, output_directory, dataset_name)
+
 DATASET_MAPPING = {
     'da_arboretum': process_arboretum,
 
+    'de_spmrl':     process_spmrl,
+
     'en_ptb3-revised': process_ptb3_revised,
 
     'id_icon':      process_id_icon,
 
     'it_turin':     process_it_turin,
     'it_vit':       process_it_vit,
```

### Comparing `stanza-1.8.1/stanza/utils/datasets/constituency/relabel_tags.py` & `stanza-1.8.2/stanza/utils/datasets/constituency/relabel_tags.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/utils/datasets/constituency/selftrain.py` & `stanza-1.8.2/stanza/utils/datasets/constituency/selftrain.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/utils/datasets/constituency/selftrain_it.py` & `stanza-1.8.2/stanza/utils/datasets/constituency/selftrain_it.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/utils/datasets/constituency/selftrain_single_file.py` & `stanza-1.8.2/stanza/utils/datasets/constituency/selftrain_single_file.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/utils/datasets/constituency/selftrain_vi_quad.py` & `stanza-1.8.2/stanza/utils/datasets/constituency/selftrain_vi_quad.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/utils/datasets/constituency/selftrain_wiki.py` & `stanza-1.8.2/stanza/utils/datasets/constituency/selftrain_wiki.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/utils/datasets/constituency/silver_variance.py` & `stanza-1.8.2/stanza/utils/datasets/constituency/silver_variance.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/utils/datasets/constituency/tokenize_wiki.py` & `stanza-1.8.2/stanza/utils/datasets/constituency/tokenize_wiki.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/utils/datasets/constituency/treebank_to_labeled_brackets.py` & `stanza-1.8.2/stanza/utils/datasets/constituency/treebank_to_labeled_brackets.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/utils/datasets/constituency/utils.py` & `stanza-1.8.2/stanza/utils/datasets/constituency/utils.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/utils/datasets/constituency/vtb_convert.py` & `stanza-1.8.2/stanza/utils/datasets/constituency/vtb_convert.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/utils/datasets/constituency/vtb_split.py` & `stanza-1.8.2/stanza/utils/datasets/constituency/vtb_split.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/utils/datasets/contract_mwt.py` & `stanza-1.8.2/stanza/utils/datasets/contract_mwt.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/utils/datasets/coref/convert_ontonotes.py` & `stanza-1.8.2/stanza/utils/datasets/coref/convert_ontonotes.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/utils/datasets/corenlp_segmenter_dataset.py` & `stanza-1.8.2/stanza/utils/datasets/corenlp_segmenter_dataset.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/utils/datasets/ner/build_en_combined.py` & `stanza-1.8.2/stanza/utils/datasets/ner/build_en_combined.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/utils/datasets/ner/check_for_duplicates.py` & `stanza-1.8.2/stanza/utils/datasets/ner/check_for_duplicates.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/utils/datasets/ner/combine_ner_datasets.py` & `stanza-1.8.2/stanza/utils/datasets/ner/combine_ner_datasets.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/utils/datasets/ner/compare_entities.py` & `stanza-1.8.2/stanza/utils/datasets/ner/compare_entities.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/utils/datasets/ner/conll_to_iob.py` & `stanza-1.8.2/stanza/utils/datasets/ner/conll_to_iob.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/utils/datasets/ner/convert_amt.py` & `stanza-1.8.2/stanza/utils/datasets/ner/convert_amt.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/utils/datasets/ner/convert_ar_aqmar.py` & `stanza-1.8.2/stanza/utils/datasets/ner/convert_ar_aqmar.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/utils/datasets/ner/convert_bn_daffodil.py` & `stanza-1.8.2/stanza/utils/datasets/ner/convert_bn_daffodil.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/utils/datasets/ner/convert_bsf_to_beios.py` & `stanza-1.8.2/stanza/utils/datasets/ner/convert_bsf_to_beios.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/utils/datasets/ner/convert_bsnlp.py` & `stanza-1.8.2/stanza/utils/datasets/ner/convert_bsnlp.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/utils/datasets/ner/convert_en_conll03.py` & `stanza-1.8.2/stanza/utils/datasets/ner/convert_en_conll03.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/utils/datasets/ner/convert_fire_2013.py` & `stanza-1.8.2/stanza/utils/datasets/ner/convert_fire_2013.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/utils/datasets/ner/convert_hy_armtdp.py` & `stanza-1.8.2/stanza/utils/datasets/ner/convert_hy_armtdp.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/utils/datasets/ner/convert_ijc.py` & `stanza-1.8.2/stanza/utils/datasets/ner/convert_ijc.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/utils/datasets/ner/convert_kk_kazNERD.py` & `stanza-1.8.2/stanza/utils/datasets/ner/convert_kk_kazNERD.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/utils/datasets/ner/convert_lst20.py` & `stanza-1.8.2/stanza/utils/datasets/ner/convert_lst20.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/utils/datasets/ner/convert_mr_l3cube.py` & `stanza-1.8.2/stanza/utils/datasets/ner/convert_mr_l3cube.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/utils/datasets/ner/convert_my_ucsy.py` & `stanza-1.8.2/stanza/utils/datasets/ner/convert_my_ucsy.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/utils/datasets/ner/convert_nkjp.py` & `stanza-1.8.2/stanza/utils/datasets/ner/convert_nkjp.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/utils/datasets/ner/convert_nner22.py` & `stanza-1.8.2/stanza/utils/datasets/ner/convert_nner22.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/utils/datasets/ner/convert_nytk.py` & `stanza-1.8.2/stanza/utils/datasets/ner/convert_nytk.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/utils/datasets/ner/convert_ontonotes.py` & `stanza-1.8.2/stanza/utils/datasets/ner/convert_ontonotes.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/utils/datasets/ner/convert_rgai.py` & `stanza-1.8.2/stanza/utils/datasets/ner/convert_rgai.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/utils/datasets/ner/convert_sindhi_siner.py` & `stanza-1.8.2/stanza/utils/datasets/ner/convert_sindhi_siner.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/utils/datasets/ner/convert_starlang_ner.py` & `stanza-1.8.2/stanza/utils/datasets/ner/convert_starlang_ner.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/utils/datasets/ner/count_entities.py` & `stanza-1.8.2/stanza/utils/datasets/ner/count_entities.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/utils/datasets/ner/json_to_bio.py` & `stanza-1.8.2/stanza/utils/datasets/ner/json_to_bio.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/utils/datasets/ner/misc_to_date.py` & `stanza-1.8.2/stanza/utils/datasets/ner/misc_to_date.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/utils/datasets/ner/ontonotes_multitag.py` & `stanza-1.8.2/stanza/utils/datasets/ner/ontonotes_multitag.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/utils/datasets/ner/prepare_ner_dataset.py` & `stanza-1.8.2/stanza/utils/datasets/ner/prepare_ner_dataset.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/utils/datasets/ner/prepare_ner_file.py` & `stanza-1.8.2/stanza/utils/datasets/ner/prepare_ner_file.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/utils/datasets/ner/preprocess_wikiner.py` & `stanza-1.8.2/stanza/utils/datasets/ner/preprocess_wikiner.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/utils/datasets/ner/simplify_en_worldwide.py` & `stanza-1.8.2/stanza/utils/datasets/ner/simplify_en_worldwide.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/utils/datasets/ner/simplify_ontonotes_to_worldwide.py` & `stanza-1.8.2/stanza/utils/datasets/ner/simplify_ontonotes_to_worldwide.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/utils/datasets/ner/split_wikiner.py` & `stanza-1.8.2/stanza/utils/datasets/ner/split_wikiner.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/utils/datasets/ner/suc_conll_to_iob.py` & `stanza-1.8.2/stanza/utils/datasets/ner/suc_conll_to_iob.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/utils/datasets/ner/suc_to_iob.py` & `stanza-1.8.2/stanza/utils/datasets/ner/suc_to_iob.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/utils/datasets/ner/utils.py` & `stanza-1.8.2/stanza/utils/datasets/ner/utils.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/utils/datasets/pos/convert_trees_to_pos.py` & `stanza-1.8.2/stanza/utils/datasets/pos/convert_trees_to_pos.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/utils/datasets/prepare_depparse_treebank.py` & `stanza-1.8.2/stanza/utils/datasets/prepare_depparse_treebank.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/utils/datasets/prepare_lemma_treebank.py` & `stanza-1.8.2/stanza/utils/datasets/prepare_lemma_treebank.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/utils/datasets/prepare_pos_treebank.py` & `stanza-1.8.2/stanza/utils/datasets/prepare_pos_treebank.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/utils/datasets/prepare_tokenizer_data.py` & `stanza-1.8.2/stanza/utils/datasets/prepare_tokenizer_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -138,14 +138,14 @@
         status_line = 'Tokenizer labels written to %s\n  ' % args.output
 
     mwts = Counter(mwt_expansions)
     if args.mwt_output is None:
         print('MWTs:', mwts)
     else:
         with open(args.mwt_output, 'w') as f:
-            json.dump(list(mwts.items()), f)
+            json.dump(list(mwts.items()), f, indent=2)
 
         status_line = status_line + '{} unique MWTs found in data.  MWTs written to {}'.format(len(mwts), args.mwt_output)
         print(status_line)
 
 if __name__ == '__main__':
     main(sys.argv[1:])
```

### Comparing `stanza-1.8.1/stanza/utils/datasets/prepare_tokenizer_treebank.py` & `stanza-1.8.2/stanza/utils/datasets/prepare_tokenizer_treebank.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,15 @@
     sents = read_sentences_from_conllu(original)
     write_sentences_to_conllu(copied, sents)
 
 def copy_conllu_treebank(treebank, model_type, paths, dest_dir, postprocess=None, augment=True):
     """
     This utility method copies only the conllu files to the given destination directory.
 
-    Both POS and lemma annotators need this.
+    Both POS, lemma, and depparse annotators need this.
     """
     os.makedirs(dest_dir, exist_ok=True)
 
     short_name = treebank_to_short_name(treebank)
     short_language = short_name.split("_")[0]
 
     with tempfile.TemporaryDirectory() as tokenizer_dir:
@@ -75,15 +75,15 @@
         if postprocess is None:
             postprocess = copy_conllu_file
 
         # now we copy the processed conllu data files
         postprocess(tokenizer_dir, "train.gold", dest_dir, "train.in", short_name)
         postprocess(tokenizer_dir, "dev.gold", dest_dir, "dev.in", short_name)
         postprocess(tokenizer_dir, "test.gold", dest_dir, "test.in", short_name)
-        if model_type is not common.ModelType.POS:
+        if model_type is not common.ModelType.POS and model_type is not common.ModelType.DEPPARSE:
             copy_conllu_file(dest_dir, "dev.in", dest_dir, "dev.gold", short_name)
             copy_conllu_file(dest_dir, "test.in", dest_dir, "test.gold", short_name)
 
 def split_train_file(treebank, train_input_conllu, train_output_conllu, dev_output_conllu):
     # set the seed for each data file so that the results are the same
     # regardless of how many treebanks are processed at once
     random.seed(1234)
@@ -839,23 +839,61 @@
             sents.extend(new_sents)
     else:
         ewt_conllu = common.find_treebank_dataset_file("UD_English-EWT", udbase_dir, dataset, "conllu")
         sents = read_sentences_from_conllu(ewt_conllu)
 
     return sents
 
+def add_english_sentence_final_punctuation(handparsed_sentences):
+    """
+    Add a period to the end of a sentence with no punct at the end.
+
+    The next-to-last word has SpaceAfter=No added as well.
+
+    Possibly English-specific because of the xpos.  Could be upgraded
+    to handle multiple languages by passing in the xpos as an argument
+    """
+    new_sents = []
+    for sent in handparsed_sentences:
+        root_id = None
+        max_id = None
+        last_punct = False
+        for line in sent:
+            if line.startswith("#"):
+                continue
+            pieces = line.split("\t")
+            if MWT_OR_COPY_RE.match(pieces[0]):
+                continue
+            if pieces[6] == '0':
+                root_id = pieces[0]
+            max_id = int(pieces[0])
+            last_punct = pieces[3] == 'PUNCT'
+        if not last_punct:
+            new_sent = list(sent)
+            pieces = new_sent[-1].split("\t")
+            pieces[-1] = add_space_after_no(pieces[-1])
+            new_sent[-1] = "\t".join(pieces)
+            new_sent.append("%d\t.\t.\tPUNCT\t.\t_\t%s\tpunct\t%s:punct\t_" % (max_id+1, root_id, root_id))
+            new_sents.append(new_sent)
+        else:
+            new_sents.append(sent)
+    return new_sents
+
+
 def build_extra_combined_english_dataset(paths, dataset):
     """
     Extra sentences we don't want augmented
     """
     handparsed_dir = paths["HANDPARSED_DIR"]
     sents = []
     if dataset == 'train':
         handparsed_path = os.path.join(handparsed_dir, "english-handparsed", "english.conll")
-        sents.extend(read_sentences_from_conllu(handparsed_path))
+        handparsed_sentences = read_sentences_from_conllu(handparsed_path)
+        handparsed_sentences = add_english_sentence_final_punctuation(handparsed_sentences)
+        sents.extend(handparsed_sentences)
         print("Loaded %d sentences from %s" % (len(sents), handparsed_path))
     return sents
 
 def build_extra_combined_italian_dataset(paths, dataset):
     """
     Extra data - the MWT data for Italian
     """
```

### Comparing `stanza-1.8.1/stanza/utils/datasets/pretrain/word_in_pretrain.py` & `stanza-1.8.2/stanza/utils/datasets/pretrain/word_in_pretrain.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/utils/datasets/random_split_conllu.py` & `stanza-1.8.2/stanza/utils/datasets/random_split_conllu.py`

 * *Files 20% similar despite different names*

```diff
@@ -20,21 +20,19 @@
     parser.add_argument('--train', type=float, default=0.8, help='Fraction of the data to use for train')
     parser.add_argument('--dev', type=float, default=0.1, help='Fraction of the data to use for dev')
     parser.add_argument('--test', type=float, default=0.1, help='Fraction of the data to use for test')
     parser.add_argument('--seed', default='1234', help='Random seed to use')
     parser.add_argument('--short_name', default='sd_isra', help='Dataset name to use when writing output files')
     parser.add_argument('--no_remove_xpos', default=True, action='store_false', dest='remove_xpos', help='By default, we remove the xpos from the dataset')
     parser.add_argument('--no_remove_feats', default=True, action='store_false', dest='remove_feats', help='By default, we remove the feats from the dataset')
+    parser.add_argument('--output_directory', default=get_default_paths()["POS_DATA_DIR"], help="Where to put the split conllu")
     args = parser.parse_args()
 
     weights = (args.train, args.dev, args.test)
 
-    paths = get_default_paths()
-    output_directory = paths["POS_DATA_DIR"]
-
     doc = CoNLL.conll2doc(args.filename)
     random.seed(args.seed)
 
     train_doc = ([], [])
     dev_doc = ([], [])
     test_doc = ([], [])
     splits = [train_doc, dev_doc, test_doc]
@@ -48,14 +46,14 @@
                 x.pop('feats', None)
         split = random.choices(splits, weights)[0]
         split[0].append(sentence_dict)
         split[1].append(sentence.comments)
 
     splits = [Document(split[0], comments=split[1]) for split in splits]
     for split_doc, split_name in zip(splits, ("train", "dev", "test")):
-        filename = os.path.join(output_directory, "%s.%s.in.conllu" % (args.short_name, split_name))
+        filename = os.path.join(args.output_directory, "%s.%s.in.conllu" % (args.short_name, split_name))
         print("Outputting %d sentences to %s" % (len(split_doc.sentences), filename))
         CoNLL.write_doc2conll(split_doc, filename)
 
 if __name__ == '__main__':
     main()
```

### Comparing `stanza-1.8.1/stanza/utils/datasets/sentiment/add_constituency.py` & `stanza-1.8.2/stanza/utils/datasets/sentiment/add_constituency.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/utils/datasets/sentiment/convert_italian_poetry_classification.py` & `stanza-1.8.2/stanza/utils/datasets/sentiment/convert_italian_poetry_classification.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/utils/datasets/sentiment/convert_italian_sentence_classification.py` & `stanza-1.8.2/stanza/utils/datasets/sentiment/convert_italian_sentence_classification.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/utils/datasets/sentiment/prepare_sentiment_dataset.py` & `stanza-1.8.2/stanza/utils/datasets/sentiment/prepare_sentiment_dataset.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/utils/datasets/sentiment/process_MELD.py` & `stanza-1.8.2/stanza/utils/datasets/sentiment/process_MELD.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/utils/datasets/sentiment/process_airline.py` & `stanza-1.8.2/stanza/utils/datasets/sentiment/process_airline.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/utils/datasets/sentiment/process_arguana_xml.py` & `stanza-1.8.2/stanza/utils/datasets/sentiment/process_arguana_xml.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/utils/datasets/sentiment/process_corona.py` & `stanza-1.8.2/stanza/utils/datasets/sentiment/process_corona.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/utils/datasets/sentiment/process_es_tass2020.py` & `stanza-1.8.2/stanza/utils/datasets/sentiment/process_es_tass2020.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/utils/datasets/sentiment/process_it_sentipolc16.py` & `stanza-1.8.2/stanza/utils/datasets/sentiment/process_it_sentipolc16.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/utils/datasets/sentiment/process_ren_chinese.py` & `stanza-1.8.2/stanza/utils/datasets/sentiment/process_ren_chinese.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/utils/datasets/sentiment/process_sb10k.py` & `stanza-1.8.2/stanza/utils/datasets/sentiment/process_sb10k.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/utils/datasets/sentiment/process_scare.py` & `stanza-1.8.2/stanza/utils/datasets/sentiment/process_scare.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/utils/datasets/sentiment/process_slsd.py` & `stanza-1.8.2/stanza/utils/datasets/sentiment/process_slsd.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/utils/datasets/sentiment/process_sst.py` & `stanza-1.8.2/stanza/utils/datasets/sentiment/process_sst.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/utils/datasets/sentiment/process_usage_german.py` & `stanza-1.8.2/stanza/utils/datasets/sentiment/process_usage_german.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/utils/datasets/sentiment/process_utils.py` & `stanza-1.8.2/stanza/utils/datasets/sentiment/process_utils.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/utils/datasets/sentiment/process_vsfc_vietnamese.py` & `stanza-1.8.2/stanza/utils/datasets/sentiment/process_vsfc_vietnamese.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/utils/datasets/thai_syllable_dict_generator.py` & `stanza-1.8.2/stanza/utils/datasets/thai_syllable_dict_generator.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/utils/datasets/tokenization/convert_ml_cochin.py` & `stanza-1.8.2/stanza/utils/datasets/tokenization/convert_ml_cochin.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/utils/datasets/tokenization/convert_my_alt.py` & `stanza-1.8.2/stanza/utils/datasets/tokenization/convert_my_alt.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/utils/datasets/tokenization/convert_text_files.py` & `stanza-1.8.2/stanza/utils/datasets/tokenization/convert_text_files.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/utils/datasets/tokenization/convert_th_best.py` & `stanza-1.8.2/stanza/utils/datasets/tokenization/convert_th_best.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/utils/datasets/tokenization/convert_th_lst20.py` & `stanza-1.8.2/stanza/utils/datasets/tokenization/convert_th_lst20.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/utils/datasets/tokenization/convert_th_orchid.py` & `stanza-1.8.2/stanza/utils/datasets/tokenization/convert_th_orchid.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/utils/datasets/tokenization/convert_vi_vlsp.py` & `stanza-1.8.2/stanza/utils/datasets/tokenization/convert_vi_vlsp.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/utils/datasets/tokenization/process_thai_tokenization.py` & `stanza-1.8.2/stanza/utils/datasets/tokenization/process_thai_tokenization.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/utils/datasets/vietnamese/renormalize.py` & `stanza-1.8.2/stanza/utils/datasets/vietnamese/renormalize.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/utils/default_paths.py` & `stanza-1.8.2/stanza/utils/default_paths.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/utils/get_tqdm.py` & `stanza-1.8.2/stanza/utils/get_tqdm.py`

 * *Files 7% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     if 'zmqshell' in ipy_str:
         from tqdm import tqdm_notebook as tqdm
         return tqdm
     if 'terminal' in ipy_str:
         from tqdm import tqdm
         return tqdm
 
-    if sys.stderr is not None and sys.stderr.isatty():
+    if sys.stderr is not None and hasattr(sys.stderr, "isatty") and sys.stderr.isatty():
         from tqdm import tqdm
         return tqdm
 
     from tqdm import tqdm
     def hidden_tqdm(*args, **kwargs):
         if "disable" in kwargs:
             return tqdm(*args, **kwargs)
```

### Comparing `stanza-1.8.1/stanza/utils/helper_func.py` & `stanza-1.8.2/stanza/utils/helper_func.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/utils/languages/kazakh_transliteration.py` & `stanza-1.8.2/stanza/utils/languages/kazakh_transliteration.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/utils/lemma/count_ambiguous_lemmas.py` & `stanza-1.8.2/stanza/utils/lemma/count_ambiguous_lemmas.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/utils/ner/flair_ner_tag_dataset.py` & `stanza-1.8.2/stanza/utils/ner/flair_ner_tag_dataset.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/utils/ner/paying_annotators.py` & `stanza-1.8.2/stanza/utils/ner/paying_annotators.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/utils/ner/spacy_ner_tag_dataset.py` & `stanza-1.8.2/stanza/utils/ner/spacy_ner_tag_dataset.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/utils/pretrain/compare_pretrains.py` & `stanza-1.8.2/stanza/utils/pretrain/compare_pretrains.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/utils/training/common.py` & `stanza-1.8.2/stanza/utils/training/common.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/utils/training/compose_ete_results.py` & `stanza-1.8.2/stanza/utils/training/compose_ete_results.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/utils/training/remove_constituency_optimizer.py` & `stanza-1.8.2/stanza/utils/training/remove_constituency_optimizer.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/utils/training/run_charlm.py` & `stanza-1.8.2/stanza/utils/training/run_charlm.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/utils/training/run_constituency.py` & `stanza-1.8.2/stanza/utils/training/run_constituency.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/utils/training/run_depparse.py` & `stanza-1.8.2/stanza/utils/training/run_depparse.py`

 * *Files 22% similar despite different names*

```diff
@@ -43,20 +43,22 @@
                  temp_output_file, command_args, extra_args):
     short_language, dataset = short_name.split("_")
 
     # TODO: refactor these blocks?
     depparse_dir   = paths["DEPPARSE_DATA_DIR"]
     train_file     = f"{depparse_dir}/{short_name}.train.in.conllu"
     dev_in_file    = f"{depparse_dir}/{short_name}.dev.in.conllu"
-    dev_gold_file  = f"{depparse_dir}/{short_name}.dev.gold.conllu"
     dev_pred_file  = temp_output_file if temp_output_file else f"{depparse_dir}/{short_name}.dev.pred.conllu"
     test_in_file   = f"{depparse_dir}/{short_name}.test.in.conllu"
-    test_gold_file = f"{depparse_dir}/{short_name}.test.gold.conllu"
     test_pred_file = temp_output_file if temp_output_file else f"{depparse_dir}/{short_name}.test.pred.conllu"
 
+    eval_file = None
+    if '--eval_file' in extra_args:
+        eval_file = extra_args[extra_args.index('--eval_file') + 1]
+
     charlm_args = build_depparse_charlm_args(short_language, dataset, command_args.charlm)
 
     bert_args = choose_transformer(short_language, command_args, extra_args)
 
     if mode == Mode.TRAIN:
         if not os.path.exists(train_file):
             logger.error("TRAIN FILE NOT FOUND: %s ... skipping" % train_file)
@@ -71,57 +73,60 @@
             # 'UD_Czech-CLTT', 'UD_Galician-TreeGal', 'UD_Latvian-LVTB' 'Romanian-SiMoNERo'
             batch_size = "3000"
         else:
             batch_size = "5000"
 
         train_args = ["--wordvec_dir", paths["WORDVEC_DIR"],
                       "--train_file", train_file,
-                      "--eval_file", dev_in_file,
+                      "--eval_file", eval_file if eval_file else dev_in_file,
                       "--output_file", dev_pred_file,
-                      "--gold_file", dev_gold_file,
                       "--batch_size", batch_size,
                       "--lang", short_language,
                       "--shorthand", short_name,
                       "--mode", "train"]
         train_args = train_args + wordvec_args(short_language, dataset, extra_args) + charlm_args + bert_args
         train_args = train_args + extra_args
         logger.info("Running train depparse for {} with args {}".format(treebank, train_args))
         parser.main(train_args)
 
     if mode == Mode.SCORE_DEV or mode == Mode.TRAIN:
         dev_args = ["--wordvec_dir", paths["WORDVEC_DIR"],
-                    "--eval_file", dev_in_file,
+                    "--eval_file", eval_file if eval_file else dev_in_file,
                     "--output_file", dev_pred_file,
-                    "--gold_file", dev_gold_file,
                     "--lang", short_language,
                     "--shorthand", short_name,
                     "--mode", "predict"]
         dev_args = dev_args + wordvec_args(short_language, dataset, extra_args) + charlm_args + bert_args
         dev_args = dev_args + extra_args
         logger.info("Running dev depparse for {} with args {}".format(treebank, dev_args))
         parser.main(dev_args)
 
-        results = common.run_eval_script_depparse(dev_gold_file, dev_pred_file)
-        logger.info("Finished running dev set on\n{}\n{}".format(treebank, results))
+        if '--no_gold_labels' not in extra_args:
+            results = common.run_eval_script_depparse(eval_file if eval_file else dev_in_file, dev_pred_file)
+            logger.info("Finished running dev set on\n{}\n{}".format(treebank, results))
+        if not temp_output_file:
+            logger.info("Output saved to %s", dev_pred_file)
 
     if mode == Mode.SCORE_TEST:
         test_args = ["--wordvec_dir", paths["WORDVEC_DIR"],
-                     "--eval_file", test_in_file,
+                     "--eval_file", eval_file if eval_file else test_in_file,
                      "--output_file", test_pred_file,
-                     "--gold_file", test_gold_file,
                      "--lang", short_language,
                      "--shorthand", short_name,
                      "--mode", "predict"]
         test_args = test_args + wordvec_args(short_language, dataset, extra_args) + charlm_args + bert_args
         test_args = test_args + extra_args
         logger.info("Running test depparse for {} with args {}".format(treebank, test_args))
         parser.main(test_args)
 
-        results = common.run_eval_script_depparse(test_gold_file, test_pred_file)
-        logger.info("Finished running test set on\n{}\n{}".format(treebank, results))
+        if '--no_gold_labels' not in extra_args:
+            results = common.run_eval_script_depparse(eval_file if eval_file else test_in_file, test_pred_file)
+            logger.info("Finished running test set on\n{}\n{}".format(treebank, results))
+        if not temp_output_file:
+            logger.info("Output saved to %s", test_pred_file)
 
 
 def main():
     common.main(run_treebank, "depparse", "parser", add_depparse_args, sub_argparse=parser.build_argparse(), build_model_filename=build_model_filename, choose_charlm_method=choose_depparse_charlm)
 
 if __name__ == "__main__":
     main()
```

### Comparing `stanza-1.8.1/stanza/utils/training/run_ete.py` & `stanza-1.8.2/stanza/utils/training/run_ete.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/utils/training/run_lemma.py` & `stanza-1.8.2/stanza/utils/training/run_lemma.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/utils/training/run_mwt.py` & `stanza-1.8.2/stanza/utils/training/run_mwt.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/utils/training/run_ner.py` & `stanza-1.8.2/stanza/utils/training/run_ner.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/utils/training/run_pos.py` & `stanza-1.8.2/stanza/utils/training/run_pos.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/utils/training/run_sentiment.py` & `stanza-1.8.2/stanza/utils/training/run_sentiment.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/utils/training/run_tokenizer.py` & `stanza-1.8.2/stanza/utils/training/run_tokenizer.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza/utils/training/separate_ner_pretrain.py` & `stanza-1.8.2/stanza/utils/training/separate_ner_pretrain.py`

 * *Files identical despite different names*

### Comparing `stanza-1.8.1/stanza.egg-info/PKG-INFO` & `stanza-1.8.2/stanza.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stanza
-Version: 1.8.1
+Version: 1.8.2
 Summary: A Python NLP Library for Many Human Languages, by the Stanford NLP Group
 Home-page: https://github.com/stanfordnlp/stanza
 Author: Stanford Natural Language Processing Group
 Author-email: jebolton@stanford.edu
 License: Apache License 2.0
 Keywords: natural-language-processing nlp natural-language-understanding stanford-nlp deep-learning
 Classifier: Development Status :: 4 - Beta
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: stanza Version: 1.8.1 Summary: A Python NLP Library
+Metadata-Version: 2.1 Name: stanza Version: 1.8.2 Summary: A Python NLP Library
 for Many Human Languages, by the Stanford NLP Group Home-page: https://
 github.com/stanfordnlp/stanza Author: Stanford Natural Language Processing
 Group Author-email: jebolton@stanford.edu License: Apache License 2.0 Keywords:
 natural-language-processing nlp natural-language-understanding stanford-nlp
 deep-learning Classifier: Development Status :: 4 - Beta Classifier: Intended
 Audience :: Developers Classifier: Intended Audience :: Education Classifier:
 Intended Audience :: Science/Research Classifier: Intended Audience ::
```

### Comparing `stanza-1.8.1/stanza.egg-info/SOURCES.txt` & `stanza-1.8.2/stanza.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -50,14 +50,15 @@
 stanza/models/common/hlstm.py
 stanza/models/common/large_margin_loss.py
 stanza/models/common/loss.py
 stanza/models/common/maxout_linear.py
 stanza/models/common/packed_lstm.py
 stanza/models/common/peft_config.py
 stanza/models/common/pretrain.py
+stanza/models/common/relative_attn.py
 stanza/models/common/seq2seq_constant.py
 stanza/models/common/seq2seq_model.py
 stanza/models/common/seq2seq_modules.py
 stanza/models/common/seq2seq_utils.py
 stanza/models/common/short_name_to_treebank.py
 stanza/models/common/stanza_object.py
 stanza/models/common/trainer.py
@@ -74,14 +75,16 @@
 stanza/models/constituency/lstm_tree_stack.py
 stanza/models/constituency/parse_transitions.py
 stanza/models/constituency/parse_tree.py
 stanza/models/constituency/partitioned_transformer.py
 stanza/models/constituency/positional_encoding.py
 stanza/models/constituency/retagging.py
 stanza/models/constituency/score_converted_dependencies.py
+stanza/models/constituency/state.py
+stanza/models/constituency/text_processing.py
 stanza/models/constituency/top_down_oracle.py
 stanza/models/constituency/trainer.py
 stanza/models/constituency/transformer_tree_stack.py
 stanza/models/constituency/transition_sequence.py
 stanza/models/constituency/tree_embedding.py
 stanza/models/constituency/tree_reader.py
 stanza/models/constituency/tree_stack.py
@@ -212,20 +215,22 @@
 stanza/tests/common/test_pretrain.py
 stanza/tests/common/test_short_name_to_treebank.py
 stanza/tests/common/test_utils.py
 stanza/tests/constituency/__init__.py
 stanza/tests/constituency/test_convert_arboretum.py
 stanza/tests/constituency/test_convert_it_vit.py
 stanza/tests/constituency/test_convert_starlang.py
+stanza/tests/constituency/test_ensemble.py
 stanza/tests/constituency/test_in_order_oracle.py
 stanza/tests/constituency/test_lstm_model.py
 stanza/tests/constituency/test_parse_transitions.py
 stanza/tests/constituency/test_parse_tree.py
 stanza/tests/constituency/test_positional_encoding.py
 stanza/tests/constituency/test_selftrain_vi_quad.py
+stanza/tests/constituency/test_text_processing.py
 stanza/tests/constituency/test_top_down_oracle.py
 stanza/tests/constituency/test_trainer.py
 stanza/tests/constituency/test_transformer_tree_stack.py
 stanza/tests/constituency/test_transition_sequence.py
 stanza/tests/constituency/test_tree_reader.py
 stanza/tests/constituency/test_tree_stack.py
 stanza/tests/constituency/test_utils.py
@@ -243,14 +248,16 @@
 stanza/tests/langid/test_langid.py
 stanza/tests/langid/test_multilingual.py
 stanza/tests/lemma/__init__.py
 stanza/tests/lemma/test_data.py
 stanza/tests/lemma/test_lemma_trainer.py
 stanza/tests/lemma/test_lowercase.py
 stanza/tests/mwt/__init__.py
+stanza/tests/mwt/test_english_corner_cases.py
+stanza/tests/mwt/test_prepare_mwt.py
 stanza/tests/mwt/test_utils.py
 stanza/tests/ner/__init__.py
 stanza/tests/ner/test_bsf_2_beios.py
 stanza/tests/ner/test_bsf_2_iob.py
 stanza/tests/ner/test_combine_ner_datasets.py
 stanza/tests/ner/test_convert_amt.py
 stanza/tests/ner/test_convert_nkjp.py
@@ -350,14 +357,15 @@
 stanza/utils/datasets/constituency/common_trees.py
 stanza/utils/datasets/constituency/convert_alt.py
 stanza/utils/datasets/constituency/convert_arboretum.py
 stanza/utils/datasets/constituency/convert_cintil.py
 stanza/utils/datasets/constituency/convert_ctb.py
 stanza/utils/datasets/constituency/convert_it_turin.py
 stanza/utils/datasets/constituency/convert_it_vit.py
+stanza/utils/datasets/constituency/convert_spmrl.py
 stanza/utils/datasets/constituency/convert_starlang.py
 stanza/utils/datasets/constituency/count_common_words.py
 stanza/utils/datasets/constituency/extract_silver_dataset.py
 stanza/utils/datasets/constituency/prepare_con_dataset.py
 stanza/utils/datasets/constituency/relabel_tags.py
 stanza/utils/datasets/constituency/selftrain.py
 stanza/utils/datasets/constituency/selftrain_it.py
```

