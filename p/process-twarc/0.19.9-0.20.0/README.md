# Comparing `tmp/process-twarc-0.19.9.tar.gz` & `tmp/process-twarc-0.20.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "process-twarc-0.19.9.tar", last modified: Mon Mar 18 20:16:54 2024, max compression
+gzip compressed data, was "process-twarc-0.20.0.tar", last modified: Sat Apr 20 13:31:27 2024, max compression
```

## Comparing `process-twarc-0.19.9.tar` & `process-twarc-0.20.0.tar`

### file list

```diff
@@ -1,38 +1,39 @@
-drwxrwxrwx   0        0        0        0 2024-03-18 20:16:54.695521 process-twarc-0.19.9/
--rw-rw-rw-   0        0        0     1077 2023-07-07 10:42:07.000000 process-twarc-0.19.9/LICENSE.txt
--rw-rw-rw-   0        0        0      694 2024-03-18 20:16:54.695521 process-twarc-0.19.9/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-07-07 10:42:22.000000 process-twarc-0.19.9/README.md
-drwxrwxrwx   0        0        0        0 2024-03-18 20:16:54.628059 process-twarc-0.19.9/process_twarc/
--rw-rw-rw-   0        0        0        0 2023-07-07 10:27:29.000000 process-twarc-0.19.9/process_twarc/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-18 20:16:54.661440 process-twarc-0.19.9/process_twarc/build_base_model/
--rw-rw-rw-   0        0        0        0 2024-03-18 20:13:51.000000 process-twarc-0.19.9/process_twarc/build_base_model/__init__.py
--rw-rw-rw-   0        0        0     7976 2024-03-18 20:13:50.000000 process-twarc-0.19.9/process_twarc/build_base_model/build_training_corpus.py
--rw-rw-rw-   0        0        0     5269 2024-03-18 20:13:49.000000 process-twarc-0.19.9/process_twarc/build_base_model/configure_base_model.py
--rw-rw-rw-   0        0        0     3548 2024-03-18 10:41:03.000000 process-twarc-0.19.9/process_twarc/build_base_model/pre_tokenize.py
--rw-rw-rw-   0        0        0     5299 2024-03-18 20:13:46.000000 process-twarc-0.19.9/process_twarc/build_base_model/train_tokenizer.py
--rw-rw-rw-   0        0        0     1339 2023-11-07 15:51:45.000000 process-twarc-0.19.9/process_twarc/cluster.py
-drwxrwxrwx   0        0        0        0 2024-03-18 20:16:54.666336 process-twarc-0.19.9/process_twarc/corpus_analysis/
--rw-rw-rw-   0        0        0        0 2024-01-28 21:00:56.000000 process-twarc-0.19.9/process_twarc/corpus_analysis/__init__.py
--rw-rw-rw-   0        0        0    11132 2024-03-16 07:28:25.000000 process-twarc-0.19.9/process_twarc/corpus_analysis/count.py
--rw-rw-rw-   0        0        0    12559 2024-03-18 20:15:26.000000 process-twarc-0.19.9/process_twarc/corpus_analysis/pos.py
--rw-rw-rw-   0        0        0    15961 2024-03-14 15:19:07.000000 process-twarc-0.19.9/process_twarc/corpus_analysis/tabulate.py
-drwxrwxrwx   0        0        0        0 2024-03-18 20:16:54.678700 process-twarc-0.19.9/process_twarc/simulate_tweet/
--rw-rw-rw-   0        0        0        0 2023-12-15 22:42:40.000000 process-twarc-0.19.9/process_twarc/simulate_tweet/__init__.py
--rw-rw-rw-   0        0        0     2872 2023-12-05 20:38:51.000000 process-twarc-0.19.9/process_twarc/simulate_tweet/default-pfp.png
--rw-rw-rw-   0        0        0    10020 2024-03-14 15:15:16.000000 process-twarc-0.19.9/process_twarc/simulate_tweet/generate.py
-drwxrwxrwx   0        0        0        0 2024-03-18 20:16:54.695521 process-twarc-0.19.9/process_twarc/train/
--rw-rw-rw-   0        0        0     2470 2024-02-04 16:59:52.000000 process-twarc-0.19.9/process_twarc/train/MLM.py
--rw-rw-rw-   0        0        0        0 2023-10-17 21:50:10.000000 process-twarc-0.19.9/process_twarc/train/__init__.py
--rw-rw-rw-   0        0        0     1276 2024-03-17 20:21:53.000000 process-twarc-0.19.9/process_twarc/train/classifier.py
--rw-rw-rw-   0        0        0     8747 2023-11-12 19:10:44.000000 process-twarc-0.19.9/process_twarc/train/evaluate.py
--rw-rw-rw-   0        0        0     7229 2024-03-14 15:17:03.000000 process-twarc-0.19.9/process_twarc/train/preprocess.py
--rw-rw-rw-   0        0        0    29423 2024-03-14 13:23:41.000000 process-twarc-0.19.9/process_twarc/train/util.py
--rw-rw-rw-   0        0        0     8364 2024-03-15 08:06:13.000000 process-twarc-0.19.9/process_twarc/util.py
-drwxrwxrwx   0        0        0        0 2024-03-18 20:16:54.646286 process-twarc-0.19.9/process_twarc.egg-info/
--rw-rw-rw-   0        0        0      694 2024-03-18 20:16:54.000000 process-twarc-0.19.9/process_twarc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1022 2024-03-18 20:16:54.000000 process-twarc-0.19.9/process_twarc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-18 20:16:54.000000 process-twarc-0.19.9/process_twarc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2024-03-18 20:16:54.000000 process-twarc-0.19.9/process_twarc.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-03-18 20:16:54.000000 process-twarc-0.19.9/process_twarc.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       56 2024-03-18 20:16:54.699284 process-twarc-0.19.9/setup.cfg
--rw-rw-rw-   0        0        0     1184 2024-03-18 20:16:19.000000 process-twarc-0.19.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-20 13:31:27.522455 process-twarc-0.20.0/
+-rw-rw-rw-   0        0        0     1077 2023-07-07 10:42:07.000000 process-twarc-0.20.0/LICENSE.txt
+-rw-rw-rw-   0        0        0      694 2024-04-20 13:31:27.522455 process-twarc-0.20.0/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-07-07 10:42:22.000000 process-twarc-0.20.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-20 13:31:27.450188 process-twarc-0.20.0/process_twarc/
+-rw-rw-rw-   0        0        0        0 2024-03-18 20:17:48.000000 process-twarc-0.20.0/process_twarc/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-20 13:31:27.484193 process-twarc-0.20.0/process_twarc/build_base_model/
+-rw-rw-rw-   0        0        0        0 2024-03-18 20:17:48.000000 process-twarc-0.20.0/process_twarc/build_base_model/__init__.py
+-rw-rw-rw-   0        0        0    11979 2024-03-22 11:09:06.000000 process-twarc-0.20.0/process_twarc/build_base_model/build_training_corpus.py
+-rw-rw-rw-   0        0        0    11585 2024-03-19 12:52:54.000000 process-twarc-0.20.0/process_twarc/build_base_model/configure_base_model.py
+-rw-rw-rw-   0        0        0     1339 2024-03-18 20:17:48.000000 process-twarc-0.20.0/process_twarc/cluster.py
+drwxrwxrwx   0        0        0        0 2024-04-20 13:31:27.494457 process-twarc-0.20.0/process_twarc/corpus_analysis/
+-rw-rw-rw-   0        0        0        0 2024-03-18 20:17:48.000000 process-twarc-0.20.0/process_twarc/corpus_analysis/__init__.py
+-rw-rw-rw-   0        0        0      476 2024-03-22 11:08:59.000000 process-twarc-0.20.0/process_twarc/corpus_analysis/calculate.py
+-rw-rw-rw-   0        0        0    11203 2024-04-01 17:17:24.000000 process-twarc-0.20.0/process_twarc/corpus_analysis/count.py
+-rw-rw-rw-   0        0        0     9540 2024-01-28 21:02:58.000000 process-twarc-0.20.0/process_twarc/corpus_analysis/ner.py
+-rw-rw-rw-   0        0        0    38302 2024-04-09 11:21:39.000000 process-twarc-0.20.0/process_twarc/corpus_analysis/plot.py
+-rw-rw-rw-   0        0        0    12801 2024-03-19 15:44:50.000000 process-twarc-0.20.0/process_twarc/corpus_analysis/pos.py
+-rw-rw-rw-   0        0        0    20996 2024-03-20 15:07:31.000000 process-twarc-0.20.0/process_twarc/corpus_analysis/tabulate.py
+drwxrwxrwx   0        0        0        0 2024-04-20 13:31:27.510456 process-twarc-0.20.0/process_twarc/simulate_tweet/
+-rw-rw-rw-   0        0        0        0 2024-03-18 20:17:48.000000 process-twarc-0.20.0/process_twarc/simulate_tweet/__init__.py
+-rw-rw-rw-   0        0        0     2872 2024-03-18 20:17:48.000000 process-twarc-0.20.0/process_twarc/simulate_tweet/default-pfp.png
+-rw-rw-rw-   0        0        0    10020 2024-03-18 20:17:48.000000 process-twarc-0.20.0/process_twarc/simulate_tweet/generate.py
+drwxrwxrwx   0        0        0        0 2024-04-20 13:31:27.521472 process-twarc-0.20.0/process_twarc/train/
+-rw-rw-rw-   0        0        0     2200 2024-04-19 17:46:16.000000 process-twarc-0.20.0/process_twarc/train/MLM.py
+-rw-rw-rw-   0        0        0        0 2024-03-18 20:17:48.000000 process-twarc-0.20.0/process_twarc/train/__init__.py
+-rw-rw-rw-   0        0        0     1227 2024-04-19 17:44:49.000000 process-twarc-0.20.0/process_twarc/train/classifier.py
+-rw-rw-rw-   0        0        0    22179 2024-04-20 13:29:57.000000 process-twarc-0.20.0/process_twarc/train/evaluate.py
+-rw-rw-rw-   0        0        0    11136 2024-04-01 13:28:06.000000 process-twarc-0.20.0/process_twarc/train/preprocess.py
+-rw-rw-rw-   0        0        0    29978 2024-04-20 13:26:45.000000 process-twarc-0.20.0/process_twarc/train/util.py
+-rw-rw-rw-   0        0        0    12055 2024-04-01 13:27:54.000000 process-twarc-0.20.0/process_twarc/util.py
+drwxrwxrwx   0        0        0        0 2024-04-20 13:31:27.479289 process-twarc-0.20.0/process_twarc.egg-info/
+-rw-rw-rw-   0        0        0      694 2024-04-20 13:31:27.000000 process-twarc-0.20.0/process_twarc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1043 2024-04-20 13:31:27.000000 process-twarc-0.20.0/process_twarc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-20 13:31:27.000000 process-twarc-0.20.0/process_twarc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2024-04-20 13:31:27.000000 process-twarc-0.20.0/process_twarc.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-20 13:31:27.000000 process-twarc-0.20.0/process_twarc.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       56 2024-04-20 13:31:27.525486 process-twarc-0.20.0/setup.cfg
+-rw-rw-rw-   0        0        0     1184 2024-04-20 13:30:58.000000 process-twarc-0.20.0/setup.py
```

### Comparing `process-twarc-0.19.9/LICENSE.txt` & `process-twarc-0.20.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `process-twarc-0.19.9/PKG-INFO` & `process-twarc-0.20.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: process-twarc
-Version: 0.19.9
+Version: 0.20.0
 Summary: Tools for transforming raw data from Twarc2 to structured data for Masked Language Modeling.
 Home-page: https://github.com/user/Lone-Wolfgang
 Author: Jordan Wolfgang Klein
 Author-email: jordan.klein.21@um.edu.mt
 License: MIT
 Keywords: Twitter,Deduplication,Tokenization,Language Modeling
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `process-twarc-0.19.9/process_twarc/cluster.py` & `process-twarc-0.20.0/process_twarc/cluster.py`

 * *Files identical despite different names*

### Comparing `process-twarc-0.19.9/process_twarc/corpus_analysis/count.py` & `process-twarc-0.20.0/process_twarc/corpus_analysis/count.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,30 +21,35 @@
     Args:
         file_path (str): Path to a dataset.
         output_dir (str, optional): Path to a directory where the output will be saved.
 
     Returns:
         character_counts (dict): A dictionary of characters and their counts.
     """
-    dataset = load_dataset(file_path, output_type="Dataset", columns="text")
-    unique_characters = lambda text: list(set(text))
-    character_sets = list(map(unique_characters, dataset["text"]))
-    character_sets = itertools.chain.from_iterable(character_sets)
-    character_counts = FreqDist(character_sets)
-    result = pd.DataFrame(character_counts.items(), columns=["character", "count"])
+    dataset = load_dataset(
+        file_path, 
+        output_type="Dataset", 
+        columns="text")
+    def charset_fn(text):
+        return list(set(text))
+    
+    dataset = dataset.map(lambda example: {"charset": charset_fn(example["text"])})
+    characters = itertools.chain.from_iterable(dataset["charset"])
+    result = FreqDist(characters)
+    result = pd.DataFrame(result.items(), columns=["character", "count"])
     result = result.sort_values(by="count", ascending=False)
     if output_dir:
         path_to_output = get_output_path(file_path, output_dir, file_type="csv")
         result.to_csv(path_to_output, index=False)
     return result
 
 def character_count_pipeline(
         data_dir: str,
-        intermediate_dir: str,
-        output_dir: str="charcter_counts",
+        intermediate_dir: str= "character_counts/files/",
+        output_dir: str="character_counts/combined",
         batch_number: int=None,
         batch_size: int=10,
         combine_counts: bool=False
         
 ):
     """Pipeline that will count characters by file, and then combine files."""
```

### Comparing `process-twarc-0.19.9/process_twarc/corpus_analysis/pos.py` & `process-twarc-0.20.0/process_twarc/corpus_analysis/pos.py`

 * *Files 10% similar despite different names*

```diff
@@ -200,29 +200,32 @@
     def tabulate_onehots(
             df: pd.DataFrame, 
             tokenizers: dict=tokenizers) -> pd.DataFrame:
         
         """Tabulates the onehot encodings of UPOS tags for each word in the dataset."""
         
         output = {}
-        for name, _ in tokenizers.items():
+        for name, tokenizer in tokenizers.items():
             
             result = [json.loads(x) for x in df[f"{name}_result"]]
             df[f"{name}_result"] = result
             result = df[f"{name}_result"].apply(pd.Series).stack().to_frame().reset_index()
             get_column = lambda col: result[0].apply(lambda x: x[col] if col in x else None)
 
             result["word"] = get_column("word")
             result["upos_onehot"] = get_column("upos_onehot")
             for pos in UPOS:
                 result[pos] = result["upos_onehot"].apply(lambda x: x[pos2idx[pos]])
             result = result[["word"] + UPOS]
-            result = result.groupby("word").sum().reset_index()
+            result = result.groupby("word").sum().reset_index(drop=True)
+            
+            vocab = set(tokenizer.get_vocab().keys())
+            result = result[result["word"].isin(vocab)].reset_index(drop=True)
 
-            output[name] = result.reset_index(drop=True)
+            output[name] = result
         return output
 
     def process(
             data_dir: str=data_dir,
             tokenizers: dict=tokenizers,
             masks: list[str]=masks,
             test: bool=test,
@@ -304,40 +307,39 @@
         path_to_output = get_output_path(file, intermediate_dir)
         save_to_parquet(df, path_to_output)
 
 
 def combine_tables(
         pos_type: str,
         intermediate_dir: str,
-        output_dir: str="") -> pd.DataFrame:
+        path_to_output: str="") -> pd.DataFrame:
     
     """Combines all results. Compresses retults into a single table with realtive values for each POS tag.
     Also assigns the most likely POS tag for each word, adding the top 5 most likely POS tags as columns."""
 
     files = get_files(intermediate_dir)
 
     combined = pd.concat([pd.read_parquet(file) for file in files]).groupby("word").sum()
+    combined = combined[combined.index.isin(vocab)]
     pos_columns = combined.columns
     combined = combined.div(combined.sum(axis=1), axis=0)
-    combined[f"{pos_type}"] = combined.idxmax(axis=1)
+    
 
-    def get_nlargest(x, n):
+    def get_top_n_tags(x, n=5):
         try:
+            # Get the nlargest n values' indices (POS tags)
             largest_values = x.nlargest(n)
-            if largest_values.iloc[-1] > 0.1:
-                return largest_values.index[-1]
-            else:
-                return None
+            # Filter out any indices where the value is <= 0.1 to adhere to the original intent
+            filtered_indices = largest_values[largest_values > 0.1].index.tolist()
+            return filtered_indices
         except TypeError:
             # Handle or ignore columns where nlargest cannot be applied
-            return None
-        
-    for n in range(6):
-        combined[f"{pos_type}{n}"] = combined[pos_columns].apply(lambda x: get_nlargest(x, n), axis=1)
+            return []
     
     combined[pos_columns] = combined[pos_columns].applymap(lambda x: round(x, 2))
-    
-    if output_dir:
-        os.makedirs(output_dir, exist_ok=True)
-        output_path = os.path.join(output_dir, f"{pos_type}.csv")
-        combined.to_csv(output_path)
+    combined = combined.reset_index()
+
+    combined[f"{pos_type}"] = combined[pos_columns].apply(get_top_n_tags, axis=1)
+    if path_to_output:
+        os.makedirs(os.path.dirname(path_to_output), exist_ok=True)
+        combined.to_csv(path_to_output, index=False)
     return combined
```

### Comparing `process-twarc-0.19.9/process_twarc/simulate_tweet/default-pfp.png` & `process-twarc-0.20.0/process_twarc/simulate_tweet/default-pfp.png`

 * *Files identical despite different names*

### Comparing `process-twarc-0.19.9/process_twarc/simulate_tweet/generate.py` & `process-twarc-0.20.0/process_twarc/simulate_tweet/generate.py`

 * *Files identical despite different names*

### Comparing `process-twarc-0.19.9/process_twarc/train/MLM.py` & `process-twarc-0.20.0/process_twarc/train/MLM.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,29 +3,26 @@
 from process_twarc.util import  load_dict
 from process_twarc.train.util import  init_run, reinit_run, check_if_complete, complete_trial, launch_study
 
 def initiate_trial(
     data_dir:str,
     path_to_config: str,
     path_to_storage: str,
-    pretrained_token_indices: list=[],
     override_parameters: dict={},
     group: str="",
     preprocessed_data: bool=True,
     pause_on_epoch: bool=False
 ):
 
     def objective(trial):
         parameters, paths, trainer, stop_epoch = init_run(
             trial, 
             config, 
-            AutoModelForMaskedLM,
             datasets,
             tokenizer,
-            pretrained_token_indices=pretrained_token_indices,
             group=group, 
             override_parameters=override_parameters, 
             pause_on_epoch=pause_on_epoch
             )
         
    
         trainer.train()
@@ -56,26 +53,23 @@
 
 
 def resume_trial(
     data_dir:str,
     path_to_config: str,
     trial_checkpoint: str,
     override_parameters: dict={},
-    pretrained_token_indices: list=[],
     preprocessed_data: bool=True,
     pause_on_epoch: bool=False
 ):
     
     config = load_dict(path_to_config)
     paths, parameters, datasets, trainer, stop_epoch = reinit_run(
         trial_checkpoint, 
         config, 
-        AutoModelForMaskedLM,
         data_dir,
-        pretrained_token_indices=pretrained_token_indices,
         override_parameters=override_parameters,
         preprocessed_data=preprocessed_data,
         pause_on_epoch=pause_on_epoch
         )
 
     trainer.train(resume_from_checkpoint=paths["last_checkpoint"])
     complete = check_if_complete(trainer, parameters, stop_epoch)
```

### Comparing `process-twarc-0.19.9/process_twarc/train/classifier.py` & `process-twarc-0.20.0/process_twarc/train/classifier.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,15 +14,14 @@
     should_prune: bool=False,
 ):
     
     def objective(trial):
         parameters, paths, trainer, _ = init_run(
             trial, 
             config,
-            AutoModelForSequenceClassification,
             datasets,
             tokenizer,
             override_parameters=override_parameters,
             group=group,
             should_prune=should_prune
             )
```

### Comparing `process-twarc-0.19.9/process_twarc/train/util.py` & `process-twarc-0.20.0/process_twarc/train/util.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,37 @@
 from transformers import AutoTokenizer, TrainerCallback, Trainer, get_constant_schedule_with_warmup, get_linear_schedule_with_warmup, get_cosine_schedule_with_warmup, get_cosine_with_hard_restarts_schedule_with_warmup, DataCollatorWithPadding, DataCollatorForLanguageModeling, TrainingArguments, EarlyStoppingCallback, AutoModelForMaskedLM, AutoModelForSequenceClassification
+# from adapters import AdapterTrainer, AutoAdapterModel
 from process_twarc.util import load_dataset, load_dict
 import torch
 from torch.optim import AdamW
 import wandb
 import optuna
 from ntpath import basename
 import evaluate
 import numpy as np
 import os
 import shutil
+# import adapters
+# from adapters.heads import PredictionHead, SequenceClassifierOutput
+# from adapters.configuration.adapter_config import (
+#     SeqBnConfig,
+#     DoubleSeqBnConfig,
+#     ParBnConfig,
+#     SeqBnInvConfig,
+#     DoubleSeqBnInvConfig,
+#     CompacterPlusPlusConfig,
+#     CompacterConfig,
+#     PrefixTuningConfig,
+#     PromptTuningConfig,
+#     LoRAConfig,
+#     IA3Config,
+#     MAMConfig,
+#     UniPELTConfig
+# )
+
 
 
 def login_to_wandb(path_to_keys: str="keys/keys.json"):
     key = load_dict(path_to_keys)["wandb_api_key"]
     wandb.login(key=key)
     return
 
@@ -28,54 +47,54 @@
             raise optuna.TrialPruned()
         
 class StopCallback(TrainerCallback):
     def on_epoch_end(self, args, state, control, logs=None, **kwargs):
         control.should_training_stop = True
         control.should_save = True
 
-class DualLearningRateTrainer(Trainer):
-    def __init__(self, *args, pretrained_token_indices: list=[], **kwargs):
-        super().__init__(*args, **kwargs)
-        self.pretrained_token_indices = pretrained_token_indices
-        self.reduced_lr_factor = self.args.reduced_lr_factor
-
-    def _get_current_lr(self):
-        # Retrieve the current learning rate from the optimizer
-        return self.optimizer.param_groups[0]["lr"]
-    
-    def training_step(self, model, inputs):
-        model.train()
-        inputs = self._prepare_inputs(inputs)
-
-        loss = self.compute_loss(model, inputs)
-        if self.args.gradient_accumulation_steps > 1:
-            loss = loss / self.args.gradient_accumulation_steps
-        
-        loss.backward()
-
-        if "word_embeddings" in model.base_model.named_parameters():
-            word_embeddings = model.base_model.get_input_embeddings()
-            if self.pretrained_token_indices:
-                word_embeddings.weight.grad[self.pretrained_token_indices] *= self.reduced_lr_factor
-            
-        if "wandb" in self.args.report_to:
-            lr = self._get_current_lr()
-            reduced_lr = lr * self.reduced_lr_factor
-            wandb.log({"learning_rate": lr, "reduced_learning_rate": reduced_lr})
-
-        return loss.detach()
     
 class CustomTrainingArguments(TrainingArguments):
-    def __init__(self, *args, reduced_lr_factor=None, wandb_run_id=None, **kwargs):
+    def __init__(self, *args, wandb_run_id=None, **kwargs):
         super().__init__(*args, **kwargs)
-        if reduced_lr_factor:
-            self.reduced_lr_factor = reduced_lr_factor
         if wandb_run_id:
             self.wandb_run_id = wandb_run_id
 
+
+
+# def get_adapter_config(parameters):
+
+#     adapter_params = {p.replace("adapter_", ""):v for p,v in parameters.items() if "adapter" in p and p not in ["adapter_config", "adapter_name"]}
+#     config = parameters["adapter_config"]
+#     if config == "seq_bn":
+#         return SeqBnConfig(**adapter_params)
+#     elif config == "double_seq_bn":
+#         return DoubleSeqBnConfig(**adapter_params)
+#     elif config == "par_bn":
+#         return ParBnConfig(**adapter_params)
+#     elif config == "seq_bn_inv":
+#         return SeqBnInvConfig(**adapter_params)
+#     elif config == "double_seq_bn_inv":
+#         return DoubleSeqBnInvConfig(**adapter_params)
+#     elif config == "compacter++":
+#         return CompacterPlusPlusConfig(**adapter_params)
+#     elif config == "compacter":
+#         return CompacterConfig(**adapter_params)
+#     elif config == "prefix_tuning":
+#         return PrefixTuningConfig(**adapter_params)
+#     elif config == "prompt_tuning":
+#         return PromptTuningConfig(**adapter_params)
+#     elif config == "lora":
+#         return LoRAConfig(**adapter_params)
+#     elif config == "ia3":
+#         return IA3Config(**adapter_params)
+#     elif config == "mam":
+#         return MAMConfig(**adapter_params)
+#     elif config == "unipelt":
+#         return UniPELTConfig(**adapter_params)
+
 def get_compute_metrics(parameters):
     argmax_ = lambda x: np.argmax(x, axis=1)
 
     metrics = parameters["metrics"]
     metrics = [metrics] if type(metrics) == str else metrics
     if "accuracy" in metrics:
         def compute_accuracy(eval_pred):
@@ -83,16 +102,16 @@
             predictions, labels = eval_pred
             if parameters["label_type"] == "hard":  
                 predictions = argmax_(predictions)
             elif parameters["label_type"] == "soft":
                 predictions, labels = argmax_(predictions), argmax_(labels)
             return accuracy.compute(predictions=predictions, references=labels)
         return compute_accuracy
-
-def load_datasets(
+    
+def load_splits(
         data_dir: str,
         splits: list=["train", "validation", "development"],
         preprocessed_data: bool=False,
         label_column: str="",
         tokenizer: object=None):
     
     def load_(split, label_column: str=""):
@@ -106,14 +125,16 @@
             dataset = load_dataset(path, output_type="Dataset", columns=columns)
             if tokenizer:
                 dataset = dataset.map(lambda example: tokenizer(example["text"]), batched=True)
             if label_column not in ["", "label"]:
                 dataset = dataset.rename_column(
                     original_column_name=label_column,
                     new_column_name= "label")
+            if label_column and dataset.features["label"].dtype == 'list':
+                dataset = dataset.map(lambda example: {"label": torch.tensor(example['label'], dtype=torch.float32)}, batched=True)          
         return dataset
 
     tokenized_datasets = {split: load_(split, label_column) for split in splits}
 
     return tokenized_datasets
 
 def get_study_name(config, group: str=None):
@@ -146,32 +167,41 @@
                 choices = param["choices"]   
             return choices
         
         search_field = {k:get_choices(k) for k in search_field.keys()}
         sampler = optuna.samplers.GridSampler(search_field)
     return sampler
 
-def get_model(model_class, parameters, tokenizer):
-    if model_class == AutoModelForSequenceClassification:
-        model = model_class.from_pretrained(
+def get_data_collator(parameters, tokenizer):
+    if parameters["task"] == "sequence_classification":
+        return DataCollatorWithPadding(tokenizer=tokenizer)
+    elif parameters["task"] == "MLM":
+        return DataCollatorForLanguageModeling(tokenizer=tokenizer)
+
+def get_model(parameters):
+    if parameters["task"] == "sequence_classification":
+        model = AutoModelForSequenceClassification.from_pretrained(
             parameters["path_to_model"],
             num_labels=parameters["num_labels"],
-            id2label=parameters["id2label"],
-            label2id=parameters["label2id"]
+            id2label=parameters["id2label"]
         )
-        collator_class = DataCollatorWithPadding
 
-    elif model_class == AutoModelForMaskedLM:
-        model = model_class.from_pretrained(
+    elif parameters["task"] == "MLM":
+        model = AutoModelForMaskedLM.from_pretrained(
             parameters["path_to_model"]
             )
-        collator_class = DataCollatorForLanguageModeling
+    
+    # if parameters.get("adapter_config", None):
+    #     adapters.init(model)
+    #     adapter_config = get_adapter_config(parameters)
+    #     model.add_adapter(parameters["adapter_name"], adapter_config)
+    #     model.set_active_adapters(parameters["adapter_name"])
+    #     model.train_adapter(parameters["adapter_name"])
 
-    data_collator = collator_class(tokenizer=tokenizer)
-    return model, data_collator
+    return model
 
 
 def get_optimizer(model, parameters, optimizer_state: str=None):
     get = lambda parameter: parameters[parameter] if parameter in parameters.keys() else None
     optimizer = AdamW(
         params=model.parameters(),
         lr=get("learning_rate"),
@@ -184,28 +214,30 @@
         optimizer.load_state_dict(optimizer_state)
 
     return optimizer
 
 
 def get_scheduler(train_dataset, parameters, optimizer, scheduler_state: str=None):
 
-    get = lambda parameter, default: parameters[parameter] if parameter in parameters.keys() else default
+    get = lambda parameter, default: parameters.get(parameter, default)
 
     lr_scheduler_type = get("lr_scheduler_type", "constant")
     batch_size = get("per_device_train_batch_size", 15)
     num_train_epochs = get("num_train_epochs", 1)
     num_cycles = get("num_cycles", 0.5)
     num_restarts = get("num_restarts", 0)
     warmup_steps = get("warmup_steps", 0)
     inverse_warmup_ratio = get("inverse_warmup_ratio", 0.0)
 
     num_training_steps = len(train_dataset) // batch_size * num_train_epochs
     if inverse_warmup_ratio:
         warmup_steps = num_training_steps // inverse_warmup_ratio
         parameters["warmup_steps"] = warmup_steps
+    
+
 
 
     if lr_scheduler_type == "constant":
         scheduler = get_constant_schedule_with_warmup(
             optimizer=optimizer,
             num_warmup_steps=warmup_steps
         )
@@ -249,16 +281,16 @@
     return load_dict(os.path.join(last_checkpoint, "trainer_state.json"))["epoch"]
 
 def get_paths(trial, parameters):
     join = lambda parent, child: os.path.join(parent, child)
     start = parameters["trial_number_start"] if "trial_number_start" in parameters.keys() else 1
     trial_number = str(trial.number+start).zfill(3)
     
-    run_name = f"{parameters['group']}/trial-{trial_number}"
-    dir_path = f"{parameters['project']}/{run_name}"
+    run_name = join(parameters["group"], f"trial-{trial_number}")
+    dir_path = join(parameters["project"], run_name)
 
     paths = {
         "run_name": run_name,
         "trial_checkpoint": join(parameters["checkpoint_dir"], dir_path),
         "trial_complete": join(parameters["completed_dir"], dir_path)
     }
     return paths
@@ -351,53 +383,59 @@
             model, config, parameters = update(model, "dropout_prob", None)
     return model, config, parameters
 
 
 def configure_training_args(
         parameters,
         paths,
+        train_dataset
 ):
-    if "interval" in parameters.keys():
+    get = lambda parameter, default: parameters.get(parameter, default)
+    if get("interval", None):
         evaluation_strategy = save_strategy = "steps"
         eval_steps = save_steps = 1 / parameters["interval"] / parameters["num_train_epochs"]
     else:
         evaluation_strategy = save_strategy = "epoch"
         eval_steps = save_steps = 1
+    
+    if get("eval_delay", None) and evaluation_strategy == "steps":
+        parameters["eval_delay"] = len(train_dataset) // parameters["per_device_train_batch_size"] * parameters["eval_delay"]
+    
+    if get("warmup_epochs", None):
+        warmup_steps = parameters["warmup_epochs"] * len(train_dataset) // parameters["per_device_train_batch_size"]
+        parameters["warmup_steps"] = warmup_steps
 
-    get = lambda parameter: parameters[parameter] if parameter in parameters.keys() else None
+    
     training_args = CustomTrainingArguments(
-        adam_beta1=get("adam_beta1"),
-        adam_beta2=get("adam_beta2"),
-        adam_epsilon=get("adam_epsilon"),
+        adam_beta1=get("adam_beta1", 0.9),
+        adam_beta2=get("adam_beta2", 0.999),
+        adam_epsilon=get("adam_epsilon", 1e-8),
         eval_steps=eval_steps,
+        eval_delay = parameters.get("eval_delay", 0),
         evaluation_strategy=evaluation_strategy,
-        logging_steps=get("logging_steps"),
-        learning_rate=get("learning_rate"),
-        load_best_model_at_end=get("load_best_model_at_end"),
-        lr_scheduler_type=get("lr_scheduler_type"),
-        metric_for_best_model=get("metric_for_best_model"),
-        num_train_epochs=get("num_train_epochs"),
+        logging_steps=get("logging_steps", 500),
+        learning_rate=get("learning_rate", 1e-5),
+        load_best_model_at_end=get("load_best_model_at_end", False),
+        lr_scheduler_type=get("lr_scheduler_type", "constant"),
+        metric_for_best_model=get("metric_for_best_model", "loss"),
+        num_train_epochs=get("num_train_epochs", 1),
         output_dir=paths["trial_checkpoint"],
-        per_device_train_batch_size=get("per_device_train_batch_size"),
-        per_device_eval_batch_size=get("per_device_eval_batch_size"),
-        push_to_hub=get("push_to_hub"),
-        reduced_lr_factor=get("reduced_lr_factor"),
-        report_to=get("report_to"),
+        per_device_train_batch_size=get("per_device_train_batch_size", 8),
+        per_device_eval_batch_size=get("per_device_eval_batch_size", 8),
+        push_to_hub=get("push_to_hub", False),
+        report_to=get("report_to", "none"),
         save_strategy=save_strategy,
         save_steps=save_steps,
-        save_total_limit=get("patience") if get("patience") != 1 else 2,
-        wandb_run_id=get("wandb_run_id"),
-        weight_decay=get("weight_decay")
+        save_total_limit=get("patience", 99) if get("patience", 99) != 1 else 2,
+        warmup_steps=get("warmup_steps", 0),
+        wandb_run_id=get("wandb_run_id", None),
+        weight_decay=get("weight_decay", 0)
         )
-    if get("inverse_warmup_ratio"):
-        training_args.warmup_ratio = 1/get("inverse_warmup_ratio")
-    elif get("warmup_steps"):
-        training_args.warmup_steps = get("warmup_steps")
     
-    return training_args
+    return training_args, parameters
 
 
 def suggest_parameter(trial, search_space, param_name):
 
             param_space = search_space[param_name]
             dtype = param_space["type"]
             if dtype == "fixed":
@@ -449,30 +487,33 @@
 
     search_field = config["variable_parameters"]["search_field"]
     
     suggest = lambda variable: suggest_parameter(trial, search_field, variable)
     variable_parameters = {variable: suggest(variable) for variable in search_field.keys()}
 
     parameters = {**fixed_parameters, **group_parameters, **variable_parameters, **override_parameters}
+
+    if "report_to" in parameters.keys():
+        if type(parameters["report_to"]) == str:
+            parameters["report_to"] = [parameters["report_to"]]
     return parameters
 
 def init_wandb(parameters, paths, reinit: bool=False):
     trial_checkpoint, run_name = paths["trial_checkpoint"], paths["run_name"]
     project, group, entity = parameters["project"], parameters["group"], parameters["entity"]
-    
+    parameters["wandb_url"] = f"https://wandb.ai/{entity}/{project}/runs/{run_name}"
 
     if not reinit:
         os.makedirs(trial_checkpoint, exist_ok=True)
         wandb_run_id = wandb.util.generate_id()
         parameters["wandb_run_id"] = wandb_run_id
 
         wandb.init(
             project=project,
             id=parameters["wandb_run_id"],
-            dir=trial_checkpoint,
             group=group,
             entity=entity,
             name=run_name,
             resume="allow",
             config=parameters,
             reinit=True
         )
@@ -483,106 +524,103 @@
         wandb.init(
             project= project,
             id=wandb_run_id,
             resume="must"
             )
     return parameters
 
-def print_parameters(config, parameters, pretrained_token_indices: list=[]):
+def print_parameters(config, parameters):
     
     print("\nFixed Params:")
-    for key, value in config["fixed_parameters"].items():
-        print(f"{key}: {value}")
+    for key in config["fixed_parameters"].keys():
+        print(f"{key}: {parameters[key]}")
 
     if "group_parameters" in config.keys():
         print("\nGroup Params:")
         groups = list(config["group_parameters"].keys())
         for key in config["group_parameters"][groups[0]].keys():
             print(f"{key}: {parameters[key]}")
 
     print("\nVariable Params:")
     for key in config["variable_parameters"]["search_field"].keys():
         if key in parameters.keys():
             print(f"{key}: {parameters[key]}")
-    
-    if "reduced_lr_factor" in parameters.keys():
-        print("Daul Learning Rate Enabled")
-        print(f"Reduced Learning Rate Factor: {parameters['reduced_lr_factor']}")
-        print(f"Total Pretrained Tokens: {len(pretrained_token_indices)}")
+
     return
 
-def print_run_init(model, config, parameters, paths, pretrained_token_indices: list=[], reinit: bool=False):
+def print_run_init(model, config, parameters, paths, reinit: bool=False):
     print("\n", model.config)
-    print_parameters(config, parameters, pretrained_token_indices=pretrained_token_indices)
+    print_parameters(config, parameters)
 
+    if parameters.get("wandb_url", None):
+        print("Wandb URL:", parameters["wandb_url"])
     if not reinit:
         print(f"Beginning {basename(paths['trial_checkpoint'])}. . .")
 
     else:
         print(f"Resuming {basename(paths['trial_checkpoint'])}. . .")
     return
 
+
 def get_trainer(
         model,
         args,
         data_collator,
         datasets,
         tokenizer,
         compute_metrics,
         optimizers,
         callbacks,
-        parameters,
-        pretrained_token_indices: list=[],
+        parameters
 ):
-    trainer_args = {
-        "model": model,
-        "args": args,
-        "data_collator": data_collator,
-        "train_dataset": datasets["train"],
-        "eval_dataset": datasets["validation"],
-        "tokenizer": tokenizer,
-        "compute_metrics": compute_metrics,
-        "optimizers": optimizers,
-        "callbacks": callbacks
-    }
-    if "reduced_lr_factor" in parameters.keys():
-        trainer_args["pretrained_token_indices"] = pretrained_token_indices
-        trainer = DualLearningRateTrainer(**trainer_args)
-    else:
-        trainer = Trainer(**trainer_args)
+
+
+ 
+    trainer_args= dict(
+        model=model,
+        args=args,
+        data_collator=data_collator,
+        train_dataset=datasets["train"],
+        eval_dataset=datasets["validation"],
+        tokenizer=tokenizer,
+        compute_metrics=compute_metrics,
+        optimizers=optimizers,
+        callbacks=callbacks
+    )
+    trainer = Trainer(**trainer_args)
+    
     return trainer
      
 
 def init_run(
         trial, 
         config: dict, 
-        model_class: object,
         datasets: dict,
         tokenizer,
-        pretrained_token_indices: list=[],
         group: str="", 
         override_parameters: dict={}, 
         pause_on_epoch: bool=False, 
         should_prune: bool=False):
     
     device = "cuda" if torch.cuda.is_available() else RuntimeError("No GPU available.")
     parameters = init_parameters(
         trial, 
         config,
-        override_parameters=override_parameters, 
+        override_parameters=override_parameters,  
         group=group)
     paths = get_paths(trial, parameters)
-    model, data_collator = get_model(model_class, parameters, tokenizer)
+    model = get_model(parameters)
+    data_collator = get_data_collator(parameters, tokenizer)
     model, config, parameters = configure_dropout(model, config, parameters)
     model.to(device)
 
-    if parameters["report_to"] == "wandb":
+    if "wandb" in list(parameters["report_to"]) :
         parameters = init_wandb(parameters, paths)
 
-    training_args = configure_training_args(parameters, paths)
+    training_args, parameters = configure_training_args(parameters, paths, datasets["train"])
     optimizers, parameters = get_optimizers(model, parameters, datasets["train"])
     if parameters["warmup_steps"]:
         training_args.warmup_steps = parameters["warmup_steps"]
     
     compute_metrics = get_compute_metrics(parameters)
 
     callbacks, stop_epoch = get_callbacks(
@@ -596,106 +634,101 @@
         training_args,
         data_collator,
         datasets,
         tokenizer,
         compute_metrics,
         optimizers,
         callbacks,
-        parameters,
-        pretrained_token_indices=pretrained_token_indices
+        parameters
     )
 
     print_run_init(
         model, 
         config, 
         parameters,
-        paths,
-        pretrained_token_indices=pretrained_token_indices)
+        paths
+        )
     
     return parameters, paths, trainer, stop_epoch
 
 def get_last_checkpoint(trial_checkpoint: str):
 
     checkpoints = [os.path.join(trial_checkpoint, checkpoint) for checkpoint in os.listdir(trial_checkpoint) if os.path.isdir(os.path.join(trial_checkpoint, checkpoint))]
     return max(checkpoints, key=os.path.getctime)
 
-def retrieve_parameters(trial_checkpoint, config, model_class, override_parameters={}):
+def retrieve_parameters(trial_checkpoint, config, override_parameters={}):
 
     paths= retrieve_paths(trial_checkpoint, config)
     get = lambda target: os.path.join(paths["last_checkpoint"], target)
     training_args = torch.load(get("training_args.bin"))
     training_args_dict = {k:v for k,v in training_args.__dict__.items() if k != "callbacks"}
 
     model_config = load_dict(get("config.json"))
-    parameters = {**training_args_dict, **model_config, **config["fixed_parameters"], **override_parameters}
+    parameters = {**config["fixed_parameters"], **training_args_dict, **model_config, **override_parameters}
     tokenizer = AutoTokenizer.from_pretrained(parameters["path_to_model"])
 
-    model, data_collator = get_model(model_class, parameters, tokenizer)
+    model = get_model(parameters)
+    data_collator = get_data_collator(parameters, tokenizer)
     model.config.update(model_config)
 
     device = "cuda" if torch.cuda.is_available() else RuntimeError("No GPU available.")
     model.to(device)
     return paths, training_args, parameters, tokenizer, model, data_collator
 
 def reinit_run(
         trial_checkpoint, 
         config, 
-        model_class,
         data_dir,
-        pretrained_token_indices: list=[],
         override_parameters: dict={},
         preprocessed_data: bool=True,
         pause_on_epoch: bool=False
         ):
-
+    
     paths, training_args, parameters, tokenizer, model, data_collator = retrieve_parameters(
         trial_checkpoint, 
         config,
-        model_class,
         override_parameters=override_parameters)
-
-    datasets = load_datasets(
+    
+    datasets = load_splits(
         data_dir,
         preprocessed_data=preprocessed_data,
-        label_column=parameters["label_column"] if "label_column" in parameters.keys() else "",
+        label_column=parameters.get("label_column", ""),
         tokenizer=tokenizer if not preprocessed_data else None
-        )   
+        )
     
     
     optimizers, parameters = get_optimizers(model, parameters, datasets["train"], paths["last_checkpoint"])
     callbacks, stop_epoch = get_callbacks(
         parameters,
         pause_on_epoch=pause_on_epoch,
         current_epoch=get_current_epoch(paths["last_checkpoint"]),
     )
 
     compute_metrics = get_compute_metrics(parameters)
 
-    if parameters["report_to"] == "wandb":
+    if "wandb" in list(parameters["report_to"]):
         init_wandb(parameters, paths, reinit=True)
 
     trainer = get_trainer(
         model,
         training_args,
         data_collator,
         datasets,
         tokenizer,
         compute_metrics,
         optimizers,
         callbacks,
-        parameters,
-        pretrained_token_indices=pretrained_token_indices
+        parameters
     )
 
     print_run_init(
         model,
         config,
         parameters,
         paths,
-        pretrained_token_indices=pretrained_token_indices,
         reinit=True
     ) 
     return paths, parameters, datasets, trainer, stop_epoch
 
 def check_if_complete(trainer, parameters, stop_epoch):
     def early_stopping_triggered():
         if "early_stopping" in parameters["callbacks"]:
@@ -727,21 +760,19 @@
     if "development" in datasets.keys():
         test_dataset = datasets["development"]
     else:
         test_dataset = datasets["test"]
 
     results = trainer.evaluate(test_dataset)
     print("\nResults:", results)
+
     trainer.save_model(trial_complete)
-    if parameters["report_to"] == "wandb":
+    if "wandb" in parameters["report_to"]:
         wandb.log(results)
         wandb.finish()
-        #move wandb directory to completed directory
-        wandb_dir = os.path.join(trial_checkpoint, "wandb")
-        shutil.move(wandb_dir, trial_complete)
     #deletes the trial directory
     shutil.rmtree(trial_checkpoint)
 
     get = lambda parameter: parameters[parameter] if parameter in parameters.keys() else None
     if get("metric_for_best_trial"):
         trial_value = results[get("metric_for_best_trial")]
     elif get("metric_for_best_model"):
@@ -771,15 +802,15 @@
 
     elif parameters["metric_for_best_trial"] in ["loss", "eval_loss"]:
         direction = "minimize"
 
     tokenizer = AutoTokenizer.from_pretrained(parameters["path_to_model"], print_details=False)
 
     get = lambda parameter: parameters[parameter] if parameter in parameters.keys() else None
-    datasets = load_datasets(
+    datasets = load_splits(
         data_dir,
         preprocessed_data=preprocessed_data,
         label_column = get("label_column"),
         tokenizer=tokenizer
         )
 
     study = optuna.create_study(
```

### Comparing `process-twarc-0.19.9/process_twarc.egg-info/PKG-INFO` & `process-twarc-0.20.0/process_twarc.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: process-twarc
-Version: 0.19.9
+Version: 0.20.0
 Summary: Tools for transforming raw data from Twarc2 to structured data for Masked Language Modeling.
 Home-page: https://github.com/user/Lone-Wolfgang
 Author: Jordan Wolfgang Klein
 Author-email: jordan.klein.21@um.edu.mt
 License: MIT
 Keywords: Twitter,Deduplication,Tokenization,Language Modeling
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `process-twarc-0.19.9/process_twarc.egg-info/SOURCES.txt` & `process-twarc-0.20.0/process_twarc.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -9,18 +9,19 @@
 process_twarc.egg-info/SOURCES.txt
 process_twarc.egg-info/dependency_links.txt
 process_twarc.egg-info/requires.txt
 process_twarc.egg-info/top_level.txt
 process_twarc/build_base_model/__init__.py
 process_twarc/build_base_model/build_training_corpus.py
 process_twarc/build_base_model/configure_base_model.py
-process_twarc/build_base_model/pre_tokenize.py
-process_twarc/build_base_model/train_tokenizer.py
 process_twarc/corpus_analysis/__init__.py
+process_twarc/corpus_analysis/calculate.py
 process_twarc/corpus_analysis/count.py
+process_twarc/corpus_analysis/ner.py
+process_twarc/corpus_analysis/plot.py
 process_twarc/corpus_analysis/pos.py
 process_twarc/corpus_analysis/tabulate.py
 process_twarc/simulate_tweet/__init__.py
 process_twarc/simulate_tweet/default-pfp.png
 process_twarc/simulate_tweet/generate.py
 process_twarc/train/MLM.py
 process_twarc/train/__init__.py
```

### Comparing `process-twarc-0.19.9/setup.py` & `process-twarc-0.20.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='process-twarc',
-    version='0.19.9',
+    version='0.20.0',
     license='MIT',
     description='Tools for transforming raw data from Twarc2 to structured data for Masked Language Modeling.',
     author='Jordan Wolfgang Klein',
     author_email='jordan.klein.21@um.edu.mt',
     url='https://github.com/user/Lone-Wolfgang',
     keywords=['Twitter', 'Deduplication', 'Tokenization', 'Language Modeling'],
     install_requires=[
```

