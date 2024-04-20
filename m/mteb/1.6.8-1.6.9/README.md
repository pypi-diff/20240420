# Comparing `tmp/mteb-1.6.8.tar.gz` & `tmp/mteb-1.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mteb-1.6.8.tar", last modified: Mon Apr 15 13:20:53 2024, max compression
+gzip compressed data, was "mteb-1.6.9.tar", last modified: Mon Apr 15 20:34:30 2024, max compression
```

## Comparing `mteb-1.6.8.tar` & `mteb-1.6.9.tar`

### file list

```diff
@@ -1,479 +1,482 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 13:20:53.687756 mteb-1.6.8/
--rw-r--r--   0 root         (0) root         (0)    11357 2024-04-15 13:20:49.000000 mteb-1.6.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)    23576 2024-04-15 13:20:53.687756 mteb-1.6.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     9185 2024-04-15 13:20:49.000000 mteb-1.6.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 13:20:53.619756 mteb-1.6.8/mteb/
--rw-r--r--   0 root         (0) root         (0)     2135 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 13:20:53.623756 mteb-1.6.8/mteb/abstasks/
--rw-r--r--   0 root         (0) root         (0)     2347 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/abstasks/AbsTask.py
--rw-r--r--   0 root         (0) root         (0)     3063 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/abstasks/AbsTaskBitextMining.py
--rw-r--r--   0 root         (0) root         (0)     5881 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/abstasks/AbsTaskClassification.py
--rw-r--r--   0 root         (0) root         (0)     2389 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/abstasks/AbsTaskClustering.py
--rw-r--r--   0 root         (0) root         (0)     2542 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/abstasks/AbsTaskPairClassification.py
--rw-r--r--   0 root         (0) root         (0)     1120 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/abstasks/AbsTaskReranking.py
--rw-r--r--   0 root         (0) root         (0)    11806 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/abstasks/AbsTaskRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     2007 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/abstasks/AbsTaskSTS.py
--rw-r--r--   0 root         (0) root         (0)     2296 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/abstasks/AbsTaskSummarization.py
--rw-r--r--   0 root         (0) root         (0)      880 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/abstasks/CrosslingualTask.py
--rw-r--r--   0 root         (0) root         (0)     2831 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/abstasks/LangMapping.py
--rw-r--r--   0 root         (0) root         (0)     1031 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/abstasks/MultilingualTask.py
--rw-r--r--   0 root         (0) root         (0)     9841 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/abstasks/TaskMetadata.py
--rw-r--r--   0 root         (0) root         (0)      422 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/abstasks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7082 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/abstasks/iso_15924_to_script.json
--rw-r--r--   0 root         (0) root         (0)   193114 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/abstasks/iso_639_3_to_language.json
--rw-r--r--   0 root         (0) root         (0)      542 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/abstasks/languages.py
--rw-r--r--   0 root         (0) root         (0)     5225 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/cmd.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 13:20:53.627755 mteb-1.6.8/mteb/evaluation/
--rw-r--r--   0 root         (0) root         (0)    12990 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/evaluation/MTEB.py
--rw-r--r--   0 root         (0) root         (0)       56 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/evaluation/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 13:20:53.627755 mteb-1.6.8/mteb/evaluation/evaluators/
--rw-r--r--   0 root         (0) root         (0)     5849 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/evaluation/evaluators/BitextMiningEvaluator.py
--rw-r--r--   0 root         (0) root         (0)     8942 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/evaluation/evaluators/ClassificationEvaluator.py
--rw-r--r--   0 root         (0) root         (0)     1463 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/evaluation/evaluators/ClusteringEvaluator.py
--rw-r--r--   0 root         (0) root         (0)      744 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/evaluation/evaluators/Evaluator.py
--rw-r--r--   0 root         (0) root         (0)     7140 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/evaluation/evaluators/PairClassificationEvaluator.py
--rw-r--r--   0 root         (0) root         (0)     9613 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/evaluation/evaluators/RerankingEvaluator.py
--rw-r--r--   0 root         (0) root         (0)    12487 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/evaluation/evaluators/RetrievalEvaluator.py
--rw-r--r--   0 root         (0) root         (0)     2394 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/evaluation/evaluators/STSEvaluator.py
--rw-r--r--   0 root         (0) root         (0)     4841 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/evaluation/evaluators/SummarizationEvaluator.py
--rw-r--r--   0 root         (0) root         (0)      324 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/evaluation/evaluators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5482 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/evaluation/evaluators/utils.py
--rw-r--r--   0 root         (0) root         (0)      835 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/logging.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 13:20:53.627755 mteb-1.6.8/mteb/tasks/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 13:20:53.627755 mteb-1.6.8/mteb/tasks/BitextMining/
--rw-r--r--   0 root         (0) root         (0)      420 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/BitextMining/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 13:20:53.627755 mteb-1.6.8/mteb/tasks/BitextMining/dan/
--rw-r--r--   0 root         (0) root         (0)     1443 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/BitextMining/dan/BornholmskBitextMining.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/BitextMining/dan/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 13:20:53.631756 mteb-1.6.8/mteb/tasks/BitextMining/multilingual/
--rw-r--r--   0 root         (0) root         (0)     1199 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/BitextMining/multilingual/BUCCBitextMining.py
--rw-r--r--   0 root         (0) root         (0)     2281 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/BitextMining/multilingual/DiaBLaBitextMining.py
--rw-r--r--   0 root         (0) root         (0)     5969 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/BitextMining/multilingual/FloresBitextMining.py
--rw-r--r--   0 root         (0) root         (0)     1423 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/BitextMining/multilingual/NorwegianCourtsBitextMining.py
--rw-r--r--   0 root         (0) root         (0)     5709 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/BitextMining/multilingual/TatoebaBitextMining.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/BitextMining/multilingual/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1363 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/BitextMining/multilingual/norwegian_courts_bitext_mining.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 13:20:53.631756 mteb-1.6.8/mteb/tasks/BitextMining/vie/
--rw-r--r--   0 root         (0) root         (0)     2889 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/BitextMining/vie/VieMedEVBitextMining.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/BitextMining/vie/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 13:20:53.631756 mteb-1.6.8/mteb/tasks/Classification/
--rw-r--r--   0 root         (0) root         (0)     1425 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Classification/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 13:20:53.631756 mteb-1.6.8/mteb/tasks/Classification/dan/
--rw-r--r--   0 root         (0) root         (0)     1322 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Classification/dan/AngryTweetsClassification.py
--rw-r--r--   0 root         (0) root         (0)     1621 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Classification/dan/DKHateClassification.py
--rw-r--r--   0 root         (0) root         (0)     2511 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Classification/dan/DalajClassification.py
--rw-r--r--   0 root         (0) root         (0)     1616 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Classification/dan/DanishPoliticalCommentsClassification.py
--rw-r--r--   0 root         (0) root         (0)     2943 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Classification/dan/DdiscoCohesionClassification.py
--rw-r--r--   0 root         (0) root         (0)     1261 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Classification/dan/LccSentimentClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Classification/dan/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 13:20:53.635756 mteb-1.6.8/mteb/tasks/Classification/eng/
--rw-r--r--   0 root         (0) root         (0)     1041 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Classification/eng/AmazonPolarityClassification.py
--rw-r--r--   0 root         (0) root         (0)     1054 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Classification/eng/Banking77Classification.py
--rw-r--r--   0 root         (0) root         (0)     1374 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Classification/eng/EmotionClassification.py
--rw-r--r--   0 root         (0) root         (0)      990 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Classification/eng/ImdbClassification.py
--rw-r--r--   0 root         (0) root         (0)     1085 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Classification/eng/NewsClassification.py
--rw-r--r--   0 root         (0) root         (0)     1406 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Classification/eng/ToxicConversationsClassification.py
--rw-r--r--   0 root         (0) root         (0)     1281 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Classification/eng/TweetSentimentExtractionClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Classification/eng/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 13:20:53.635756 mteb-1.6.8/mteb/tasks/Classification/hin/
--rw-r--r--   0 root         (0) root         (0)     2195 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Classification/hin/HindiDiscourseClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Classification/hin/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 13:20:53.635756 mteb-1.6.8/mteb/tasks/Classification/jpn/
--rw-r--r--   0 root         (0) root         (0)     3550 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Classification/jpn/WRIMEClassification.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 13:20:53.635756 mteb-1.6.8/mteb/tasks/Classification/multilingual/
--rw-r--r--   0 root         (0) root         (0)     1575 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Classification/multilingual/AmazonCounterfactualClassification.py
--rw-r--r--   0 root         (0) root         (0)     1377 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Classification/multilingual/AmazonReviewsClassification.py
--rw-r--r--   0 root         (0) root         (0)     1275 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Classification/multilingual/MTOPDomainClassification.py
--rw-r--r--   0 root         (0) root         (0)     1275 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Classification/multilingual/MTOPIntentClassification.py
--rw-r--r--   0 root         (0) root         (0)     1627 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Classification/multilingual/MasakhaNEWSClassification.py
--rw-r--r--   0 root         (0) root         (0)     2537 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Classification/multilingual/MassiveIntentClassification.py
--rw-r--r--   0 root         (0) root         (0)     2543 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Classification/multilingual/MassiveScenarioClassification.py
--rw-r--r--   0 root         (0) root         (0)     1611 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Classification/multilingual/NordicLangClassification.py
--rw-r--r--   0 root         (0) root         (0)     6099 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Classification/multilingual/ScalaClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Classification/multilingual/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 13:20:53.635756 mteb-1.6.8/mteb/tasks/Classification/nob/
--rw-r--r--   0 root         (0) root         (0)     1121 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Classification/nob/NoRecClassification.py
--rw-r--r--   0 root         (0) root         (0)     1173 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Classification/nob/NorwegianParliamentClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Classification/nob/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 13:20:53.635756 mteb-1.6.8/mteb/tasks/Classification/pol/
--rw-r--r--   0 root         (0) root         (0)     4922 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Classification/pol/PolishClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Classification/pol/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 13:20:53.639756 mteb-1.6.8/mteb/tasks/Classification/swe/
--rw-r--r--   0 root         (0) root         (0)     1043 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Classification/swe/SweRecClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Classification/swe/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 13:20:53.639756 mteb-1.6.8/mteb/tasks/Classification/vie/
--rw-r--r--   0 root         (0) root         (0)     3368 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Classification/vie/VieStudentFeedbackClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Classification/vie/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 13:20:53.639756 mteb-1.6.8/mteb/tasks/Classification/zho/
--rw-r--r--   0 root         (0) root         (0)     6571 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Classification/zho/CMTEBClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Classification/zho/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 13:20:53.639756 mteb-1.6.8/mteb/tasks/Clustering/
--rw-r--r--   0 root         (0) root         (0)     1278 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Clustering/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 13:20:53.639756 mteb-1.6.8/mteb/tasks/Clustering/deu/
--rw-r--r--   0 root         (0) root         (0)     1132 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Clustering/deu/BlurbsClusteringP2P.py
--rw-r--r--   0 root         (0) root         (0)     1124 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Clustering/deu/BlurbsClusteringS2S.py
--rw-r--r--   0 root         (0) root         (0)     1100 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Clustering/deu/TenKGnadClusteringP2P.py
--rw-r--r--   0 root         (0) root         (0)     1080 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Clustering/deu/TenKGnadClusteringS2S.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Clustering/deu/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 13:20:53.643756 mteb-1.6.8/mteb/tasks/Clustering/eng/
--rw-r--r--   0 root         (0) root         (0)     1101 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Clustering/eng/ArxivClusteringP2P.py
--rw-r--r--   0 root         (0) root         (0)     1087 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Clustering/eng/ArxivClusteringS2S.py
--rw-r--r--   0 root         (0) root         (0)     1128 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Clustering/eng/BigPatentClustering.py
--rw-r--r--   0 root         (0) root         (0)     1071 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Clustering/eng/BiorxivClusteringP2P.py
--rw-r--r--   0 root         (0) root         (0)     1061 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Clustering/eng/BiorxivClusteringS2S.py
--rw-r--r--   0 root         (0) root         (0)     1072 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Clustering/eng/MedrxivClusteringP2P.py
--rw-r--r--   0 root         (0) root         (0)     1062 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Clustering/eng/MedrxivClusteringS2S.py
--rw-r--r--   0 root         (0) root         (0)     1102 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Clustering/eng/RedditClustering.py
--rw-r--r--   0 root         (0) root         (0)     1091 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Clustering/eng/RedditClusteringP2P.py
--rw-r--r--   0 root         (0) root         (0)     1127 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Clustering/eng/StackExchangeClustering.py
--rw-r--r--   0 root         (0) root         (0)     1115 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Clustering/eng/StackExchangeClusteringP2P.py
--rw-r--r--   0 root         (0) root         (0)     1084 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Clustering/eng/TwentyNewsgroupsClustering.py
--rw-r--r--   0 root         (0) root         (0)     1135 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Clustering/eng/WikiCitiesClustering.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Clustering/eng/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 13:20:53.643756 mteb-1.6.8/mteb/tasks/Clustering/fra/
--rw-r--r--   0 root         (0) root         (0)     1911 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Clustering/fra/AlloProfClusteringP2P.py
--rw-r--r--   0 root         (0) root         (0)     1757 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Clustering/fra/AlloProfClusteringS2S.py
--rw-r--r--   0 root         (0) root         (0)     1625 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Clustering/fra/HALClusteringS2S.py
--rw-r--r--   0 root         (0) root         (0)     1942 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Clustering/fra/MLSUMClusteringP2P.py
--rw-r--r--   0 root         (0) root         (0)     1757 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Clustering/fra/MLSUMClusteringS2S.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Clustering/fra/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 13:20:53.643756 mteb-1.6.8/mteb/tasks/Clustering/multilingual/
--rw-r--r--   0 root         (0) root         (0)     2723 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Clustering/multilingual/MasakhaNEWSClusteringP2P.py
--rw-r--r--   0 root         (0) root         (0)     2737 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Clustering/multilingual/MasakhaNEWSClusteringS2S.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Clustering/multilingual/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 13:20:53.643756 mteb-1.6.8/mteb/tasks/Clustering/nob/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Clustering/nob/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3442 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Clustering/nob/snl_clustering.py
--rw-r--r--   0 root         (0) root         (0)     3596 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Clustering/nob/vg_clustering.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 13:20:53.643756 mteb-1.6.8/mteb/tasks/Clustering/pol/
--rw-r--r--   0 root         (0) root         (0)     1137 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Clustering/pol/PolishClustering.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Clustering/pol/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 13:20:53.643756 mteb-1.6.8/mteb/tasks/Clustering/spa/
--rw-r--r--   0 root         (0) root         (0)     1042 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Clustering/spa/FloresClusteringS2S.py
--rw-r--r--   0 root         (0) root         (0)     1060 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Clustering/spa/SpanishNewsClusteringP2P.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Clustering/spa/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 13:20:53.647756 mteb-1.6.8/mteb/tasks/Clustering/swe/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Clustering/swe/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3926 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Clustering/swe/swedn_clustering.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 13:20:53.647756 mteb-1.6.8/mteb/tasks/Clustering/zho/
--rw-r--r--   0 root         (0) root         (0)     3639 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Clustering/zho/CMTEBClustering.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Clustering/zho/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 13:20:53.647756 mteb-1.6.8/mteb/tasks/PairClassification/
--rw-r--r--   0 root         (0) root         (0)      344 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/PairClassification/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 13:20:53.647756 mteb-1.6.8/mteb/tasks/PairClassification/deu/
--rw-r--r--   0 root         (0) root         (0)     2862 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/PairClassification/deu/FalseFriendsDeEnPC.py
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/PairClassification/deu/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 13:20:53.647756 mteb-1.6.8/mteb/tasks/PairClassification/eng/
--rw-r--r--   0 root         (0) root         (0)     1152 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/PairClassification/eng/SprintDuplicateQuestionsPC.py
--rw-r--r--   0 root         (0) root         (0)     1086 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/PairClassification/eng/TwitterSemEval2015PC.py
--rw-r--r--   0 root         (0) root         (0)     1040 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/PairClassification/eng/TwitterURLCorpusPC.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/PairClassification/eng/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 13:20:53.647756 mteb-1.6.8/mteb/tasks/PairClassification/multilingual/
--rw-r--r--   0 root         (0) root         (0)     2798 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/PairClassification/multilingual/OpusparcusPC.py
--rw-r--r--   0 root         (0) root         (0)     1768 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/PairClassification/multilingual/PawsX.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/PairClassification/multilingual/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 13:20:53.647756 mteb-1.6.8/mteb/tasks/PairClassification/pol/
--rw-r--r--   0 root         (0) root         (0)     3577 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/PairClassification/pol/PolishPC.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/PairClassification/pol/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 13:20:53.647756 mteb-1.6.8/mteb/tasks/PairClassification/zho/
--rw-r--r--   0 root         (0) root         (0)     1849 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/PairClassification/zho/CMTEBPairClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/PairClassification/zho/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 13:20:53.647756 mteb-1.6.8/mteb/tasks/Reranking/
--rw-r--r--   0 root         (0) root         (0)      346 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Reranking/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 13:20:53.651756 mteb-1.6.8/mteb/tasks/Reranking/eng/
--rw-r--r--   0 root         (0) root         (0)     1118 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Reranking/eng/AskUbuntuDupQuestions.py
--rw-r--r--   0 root         (0) root         (0)     1103 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Reranking/eng/MindSmallReranking.py
--rw-r--r--   0 root         (0) root         (0)     3054 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Reranking/eng/SciDocsReranking.py
--rw-r--r--   0 root         (0) root         (0)     1137 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Reranking/eng/StackOverflowDupQuestions.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Reranking/eng/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 13:20:53.651756 mteb-1.6.8/mteb/tasks/Reranking/fra/
--rw-r--r--   0 root         (0) root         (0)     1195 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Reranking/fra/AlloprofReranking.py
--rw-r--r--   0 root         (0) root         (0)     1065 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Reranking/fra/SyntecReranking.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Reranking/fra/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 13:20:53.651756 mteb-1.6.8/mteb/tasks/Reranking/multilingual/
--rw-r--r--   0 root         (0) root         (0)     1269 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Reranking/multilingual/MIRACLReranking.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Reranking/multilingual/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 13:20:53.651756 mteb-1.6.8/mteb/tasks/Reranking/zho/
--rw-r--r--   0 root         (0) root         (0)     3528 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Reranking/zho/CMTEBReranking.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Reranking/zho/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 13:20:53.651756 mteb-1.6.8/mteb/tasks/Retrieval/
--rw-r--r--   0 root         (0) root         (0)     3005 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Retrieval/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 13:20:53.651756 mteb-1.6.8/mteb/tasks/Retrieval/code/
--rw-r--r--   0 root         (0) root         (0)     3377 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Retrieval/code/CodeSearchNetRetrieval.py
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Retrieval/code/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 13:20:53.651756 mteb-1.6.8/mteb/tasks/Retrieval/dan/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Retrieval/dan/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3794 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Retrieval/dan/dan_fever.py
--rw-r--r--   0 root         (0) root         (0)     2583 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Retrieval/dan/t2nord_retrieval.py
--rw-r--r--   0 root         (0) root         (0)     3148 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Retrieval/dan/twitterhjerne.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 13:20:53.655756 mteb-1.6.8/mteb/tasks/Retrieval/deu/
--rw-r--r--   0 root         (0) root         (0)     2048 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Retrieval/deu/GerDaLIRRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1228 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Retrieval/deu/GerDaLIRSmallRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     2876 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Retrieval/deu/GermanDPRRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     2127 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Retrieval/deu/GermanQuADRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1052 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Retrieval/deu/LegalQuADRetrieval.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Retrieval/deu/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 13:20:53.659756 mteb-1.6.8/mteb/tasks/Retrieval/eng/
--rw-r--r--   0 root         (0) root         (0)     1118 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Retrieval/eng/AILACasedocsRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1086 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Retrieval/eng/AILAStatutesRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1011 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Retrieval/eng/ArguAnaRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1065 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Retrieval/eng/CQADupstackAndroidRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1065 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Retrieval/eng/CQADupstackEnglishRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1062 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Retrieval/eng/CQADupstackGamingRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1053 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Retrieval/eng/CQADupstackGisRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1077 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Retrieval/eng/CQADupstackMathematicaRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1065 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Retrieval/eng/CQADupstackPhysicsRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1077 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Retrieval/eng/CQADupstackProgrammersRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1059 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Retrieval/eng/CQADupstackStatsRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1053 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Retrieval/eng/CQADupstackTexRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1056 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Retrieval/eng/CQADupstackUnixRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1074 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Retrieval/eng/CQADupstackWebmastersRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1071 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Retrieval/eng/CQADupstackWordpressRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1095 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Retrieval/eng/ClimateFEVERRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1031 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Retrieval/eng/DBPediaRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1175 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Retrieval/eng/FEVERRetrieval.py
--rw-r--r--   0 root         (0) root         (0)      983 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Retrieval/eng/FiQA2018Retrieval.py
--rw-r--r--   0 root         (0) root         (0)     3705 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Retrieval/eng/HagridRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1151 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Retrieval/eng/HotpotQARetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1146 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Retrieval/eng/LegalBenchConsumerContractsQARetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1150 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Retrieval/eng/LegalBenchCorporateLobbyingRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1147 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Retrieval/eng/LegalSummarizationRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1009 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Retrieval/eng/MSMARCORetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1039 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Retrieval/eng/MSMARCOv2Retrieval.py
--rw-r--r--   0 root         (0) root         (0)     1650 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Retrieval/eng/MedicalQARetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1024 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Retrieval/eng/NFCorpusRetrieval.py
--rw-r--r--   0 root         (0) root         (0)      999 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Retrieval/eng/NQRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1991 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Retrieval/eng/NarrativeQARetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1155 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Retrieval/eng/QuoraRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1114 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Retrieval/eng/SCIDOCSRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1046 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Retrieval/eng/SciFactRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1069 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Retrieval/eng/TRECCOVIDRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1009 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Retrieval/eng/Touche2020Retrieval.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Retrieval/eng/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 13:20:53.659756 mteb-1.6.8/mteb/tasks/Retrieval/fra/
--rw-r--r--   0 root         (0) root         (0)     2145 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Retrieval/fra/AlloprofRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     2475 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Retrieval/fra/BSARDRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     2127 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Retrieval/fra/SyntecRetrieval.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Retrieval/fra/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 13:20:53.659756 mteb-1.6.8/mteb/tasks/Retrieval/jpn/
--rw-r--r--   0 root         (0) root         (0)     2853 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Retrieval/jpn/JaQuADRetrieval.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 13:20:53.663756 mteb-1.6.8/mteb/tasks/Retrieval/kor/
--rw-r--r--   0 root         (0) root         (0)      906 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Retrieval/kor/KoMiracl.py
--rw-r--r--   0 root         (0) root         (0)      922 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Retrieval/kor/KoStrategyQA.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Retrieval/kor/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 13:20:53.663756 mteb-1.6.8/mteb/tasks/Retrieval/multilingual/
--rw-r--r--   0 root         (0) root         (0)     3277 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Retrieval/multilingual/MIRACLRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     3052 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Retrieval/multilingual/MintakaRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     3432 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Retrieval/multilingual/MultiLongDocRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     2979 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Retrieval/multilingual/XMarketRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     3145 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Retrieval/multilingual/XPQARetrieval.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Retrieval/multilingual/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 13:20:53.663756 mteb-1.6.8/mteb/tasks/Retrieval/nob/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Retrieval/nob/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3952 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Retrieval/nob/norquad.py
--rw-r--r--   0 root         (0) root         (0)     2708 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Retrieval/nob/snl_retrieval.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 13:20:53.663756 mteb-1.6.8/mteb/tasks/Retrieval/pol/
--rw-r--r--   0 root         (0) root         (0)      967 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Retrieval/pol/ArguAnaPLRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1040 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Retrieval/pol/DBPediaPLRetrieval.py
--rw-r--r--   0 root         (0) root         (0)      984 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Retrieval/pol/FiQAPLRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1112 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Retrieval/pol/HotpotQAPLRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1009 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Retrieval/pol/MSMARCOPLRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1040 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Retrieval/pol/NFCorpusPLRetrieval.py
--rw-r--r--   0 root         (0) root         (0)      997 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Retrieval/pol/NQPLRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1130 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Retrieval/pol/QuoraPLRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1091 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Retrieval/pol/SCIDOCSPLRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1053 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Retrieval/pol/SciFactPLRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1085 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Retrieval/pol/TRECCOVIDPLRetrieval.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Retrieval/pol/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 13:20:53.663756 mteb-1.6.8/mteb/tasks/Retrieval/spa/
--rw-r--r--   0 root         (0) root         (0)     2125 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Retrieval/spa/SpanishPassageRetrievalS2P.py
--rw-r--r--   0 root         (0) root         (0)     2056 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Retrieval/spa/SpanishPassageRetrievalS2S.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Retrieval/spa/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 13:20:53.667756 mteb-1.6.8/mteb/tasks/Retrieval/swe/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Retrieval/swe/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3219 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Retrieval/swe/swedn_retrieval.py
--rw-r--r--   0 root         (0) root         (0)     2619 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Retrieval/swe/swefaq_retrieval.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 13:20:53.667756 mteb-1.6.8/mteb/tasks/Retrieval/vie/
--rw-r--r--   0 root         (0) root         (0)     3798 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Retrieval/vie/VieQuADRetrieval.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Retrieval/vie/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 13:20:53.667756 mteb-1.6.8/mteb/tasks/Retrieval/zho/
--rw-r--r--   0 root         (0) root         (0)    10384 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Retrieval/zho/CMTEBRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1121 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Retrieval/zho/LeCaRDv2Retrieval.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Retrieval/zho/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 13:20:53.667756 mteb-1.6.8/mteb/tasks/STS/
--rw-r--r--   0 root         (0) root         (0)      575 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/STS/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 13:20:53.667756 mteb-1.6.8/mteb/tasks/STS/deu/
--rw-r--r--   0 root         (0) root         (0)     1370 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/STS/deu/GermanSTSBenchmarkSTS.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/STS/deu/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 13:20:53.667756 mteb-1.6.8/mteb/tasks/STS/eng/
--rw-r--r--   0 root         (0) root         (0)     1184 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/STS/eng/BiossesSTS.py
--rw-r--r--   0 root         (0) root         (0)     1153 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/STS/eng/STS12STS.py
--rw-r--r--   0 root         (0) root         (0)     1150 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/STS/eng/STS13STS.py
--rw-r--r--   0 root         (0) root         (0)     1184 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/STS/eng/STS14STS.py
--rw-r--r--   0 root         (0) root         (0)     1148 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/STS/eng/STS15STS.py
--rw-r--r--   0 root         (0) root         (0)     1148 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/STS/eng/STS16STS.py
--rw-r--r--   0 root         (0) root         (0)     1208 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/STS/eng/STSBenchmarkSTS.py
--rw-r--r--   0 root         (0) root         (0)     1185 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/STS/eng/SickrSTS.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/STS/eng/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 13:20:53.667756 mteb-1.6.8/mteb/tasks/STS/fra/
--rw-r--r--   0 root         (0) root         (0)     1472 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/STS/fra/SickFrSTS.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/STS/fra/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 13:20:53.667756 mteb-1.6.8/mteb/tasks/STS/multilingual/
--rw-r--r--   0 root         (0) root         (0)     1600 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/STS/multilingual/STS17CrosslingualSTS.py
--rw-r--r--   0 root         (0) root         (0)     1832 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/STS/multilingual/STS22CrosslingualSTS.py
--rw-r--r--   0 root         (0) root         (0)     2712 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/STS/multilingual/STSBenchmarkMultilingualSTS.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/STS/multilingual/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 13:20:53.667756 mteb-1.6.8/mteb/tasks/STS/pol/
--rw-r--r--   0 root         (0) root         (0)     2268 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/STS/pol/PolishSTS.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/STS/pol/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 13:20:53.667756 mteb-1.6.8/mteb/tasks/STS/spa/
--rw-r--r--   0 root         (0) root         (0)     1486 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/STS/spa/STSES.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/STS/spa/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 13:20:53.671756 mteb-1.6.8/mteb/tasks/STS/zho/
--rw-r--r--   0 root         (0) root         (0)     7122 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/STS/zho/CMTEBSTS.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/STS/zho/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 13:20:53.671756 mteb-1.6.8/mteb/tasks/Summarization/
--rw-r--r--   0 root         (0) root         (0)      124 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Summarization/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 13:20:53.671756 mteb-1.6.8/mteb/tasks/Summarization/eng/
--rw-r--r--   0 root         (0) root         (0)     1243 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Summarization/eng/SummEvalSummarization.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Summarization/eng/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 13:20:53.671756 mteb-1.6.8/mteb/tasks/Summarization/fra/
--rw-r--r--   0 root         (0) root         (0)     1304 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Summarization/fra/SummEvalFrSummarization.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/Summarization/fra/__init__.py
--rw-r--r--   0 root         (0) root         (0)      252 2024-04-15 13:20:49.000000 mteb-1.6.8/mteb/tasks/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 13:20:53.687756 mteb-1.6.8/mteb.egg-info/
--rw-r--r--   0 root         (0) root         (0)    23576 2024-04-15 13:20:53.000000 mteb-1.6.8/mteb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    19125 2024-04-15 13:20:53.000000 mteb-1.6.8/mteb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-15 13:20:53.000000 mteb-1.6.8/mteb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       39 2024-04-15 13:20:53.000000 mteb-1.6.8/mteb.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      234 2024-04-15 13:20:53.000000 mteb-1.6.8/mteb.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       31 2024-04-15 13:20:53.000000 mteb-1.6.8/mteb.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     2169 2024-04-15 13:20:50.000000 mteb-1.6.8/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 13:20:53.615756 mteb-1.6.8/results/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 13:20:53.671756 mteb-1.6.8/results/intfloat__multilingual-e5-small/
--rw-r--r--   0 root         (0) root         (0)     5524 2024-04-15 13:20:49.000000 mteb-1.6.8/results/intfloat__multilingual-e5-small/CodeSearchNetRetrieval.json
--rw-r--r--   0 root         (0) root         (0)     1016 2024-04-15 13:20:49.000000 mteb-1.6.8/results/intfloat__multilingual-e5-small/DanFEVER.json
--rw-r--r--   0 root         (0) root         (0)     1027 2024-04-15 13:20:49.000000 mteb-1.6.8/results/intfloat__multilingual-e5-small/JaQuADRetrieval.json
--rw-r--r--   0 root         (0) root         (0)     1025 2024-04-15 13:20:49.000000 mteb-1.6.8/results/intfloat__multilingual-e5-small/MedicalQARetrieval.json
--rw-r--r--   0 root         (0) root         (0)      371 2024-04-15 13:20:49.000000 mteb-1.6.8/results/intfloat__multilingual-e5-small/NewsClassification.json
--rw-r--r--   0 root         (0) root         (0)     1021 2024-04-15 13:20:49.000000 mteb-1.6.8/results/intfloat__multilingual-e5-small/NorQuadRetrieval.json
--rw-r--r--   0 root         (0) root         (0)      374 2024-04-15 13:20:49.000000 mteb-1.6.8/results/intfloat__multilingual-e5-small/NorwegianCourtsBitextMining.json
--rw-r--r--   0 root         (0) root         (0)      298 2024-04-15 13:20:49.000000 mteb-1.6.8/results/intfloat__multilingual-e5-small/SNLClustering.json
--rw-r--r--   0 root         (0) root         (0)     1023 2024-04-15 13:20:49.000000 mteb-1.6.8/results/intfloat__multilingual-e5-small/SNLRetrieval.json
--rw-r--r--   0 root         (0) root         (0)     1015 2024-04-15 13:20:49.000000 mteb-1.6.8/results/intfloat__multilingual-e5-small/SweFaqRetrieval.json
--rw-r--r--   0 root         (0) root         (0)      304 2024-04-15 13:20:49.000000 mteb-1.6.8/results/intfloat__multilingual-e5-small/SwednClustering.json
--rw-r--r--   0 root         (0) root         (0)     1023 2024-04-15 13:20:49.000000 mteb-1.6.8/results/intfloat__multilingual-e5-small/SwednRetrieval.json
--rw-r--r--   0 root         (0) root         (0)     1021 2024-04-15 13:20:49.000000 mteb-1.6.8/results/intfloat__multilingual-e5-small/TV2Nordretrieval.json
--rw-r--r--   0 root         (0) root         (0)     1034 2024-04-15 13:20:49.000000 mteb-1.6.8/results/intfloat__multilingual-e5-small/TwitterHjerneRetrieval.json
--rw-r--r--   0 root         (0) root         (0)      303 2024-04-15 13:20:49.000000 mteb-1.6.8/results/intfloat__multilingual-e5-small/VGClustering.json
--rw-r--r--   0 root         (0) root         (0)      351 2024-04-15 13:20:49.000000 mteb-1.6.8/results/intfloat__multilingual-e5-small/VieMedEVBitextMining.json
--rw-r--r--   0 root         (0) root         (0)     1028 2024-04-15 13:20:49.000000 mteb-1.6.8/results/intfloat__multilingual-e5-small/VieQuADRetrieval.json
--rw-r--r--   0 root         (0) root         (0)      377 2024-04-15 13:20:49.000000 mteb-1.6.8/results/intfloat__multilingual-e5-small/VieStudentFeedbackClassification.json
--rw-r--r--   0 root         (0) root         (0)      364 2024-04-15 13:20:49.000000 mteb-1.6.8/results/intfloat__multilingual-e5-small/WRIMEClassification.json
--rw-r--r--   0 root         (0) root         (0)      111 2024-04-15 13:20:49.000000 mteb-1.6.8/results/intfloat__multilingual-e5-small/model_meta.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 13:20:53.675756 mteb-1.6.8/results/sentence-transformers__all-MiniLM-L6-v2/
--rw-r--r--   0 root         (0) root         (0)      385 2024-04-15 13:20:49.000000 mteb-1.6.8/results/sentence-transformers__all-MiniLM-L6-v2/Banking77Classification.json
--rw-r--r--   0 root         (0) root         (0)      340 2024-04-15 13:20:49.000000 mteb-1.6.8/results/sentence-transformers__all-MiniLM-L6-v2/BornholmBitextMining.json
--rw-r--r--   0 root         (0) root         (0)     1020 2024-04-15 13:20:49.000000 mteb-1.6.8/results/sentence-transformers__all-MiniLM-L6-v2/DanFEVER.json
--rw-r--r--   0 root         (0) root         (0)     1027 2024-04-15 13:20:49.000000 mteb-1.6.8/results/sentence-transformers__all-MiniLM-L6-v2/NorQuadRetrieval.json
--rw-r--r--   0 root         (0) root         (0)      374 2024-04-15 13:20:49.000000 mteb-1.6.8/results/sentence-transformers__all-MiniLM-L6-v2/NorwegianCourtsBitextMining.json
--rw-r--r--   0 root         (0) root         (0)      303 2024-04-15 13:20:49.000000 mteb-1.6.8/results/sentence-transformers__all-MiniLM-L6-v2/SNLClustering.json
--rw-r--r--   0 root         (0) root         (0)     1021 2024-04-15 13:20:49.000000 mteb-1.6.8/results/sentence-transformers__all-MiniLM-L6-v2/SNLRetrieval.json
--rw-r--r--   0 root         (0) root         (0)     1014 2024-04-15 13:20:49.000000 mteb-1.6.8/results/sentence-transformers__all-MiniLM-L6-v2/SweFaqRetrieval.json
--rw-r--r--   0 root         (0) root         (0)      306 2024-04-15 13:20:49.000000 mteb-1.6.8/results/sentence-transformers__all-MiniLM-L6-v2/SwednClustering.json
--rw-r--r--   0 root         (0) root         (0)     1025 2024-04-15 13:20:49.000000 mteb-1.6.8/results/sentence-transformers__all-MiniLM-L6-v2/SwednRetrieval.json
--rw-r--r--   0 root         (0) root         (0)     1021 2024-04-15 13:20:49.000000 mteb-1.6.8/results/sentence-transformers__all-MiniLM-L6-v2/TV2Nordretrieval.json
--rw-r--r--   0 root         (0) root         (0)     1034 2024-04-15 13:20:49.000000 mteb-1.6.8/results/sentence-transformers__all-MiniLM-L6-v2/TwitterHjerneRetrieval.json
--rw-r--r--   0 root         (0) root         (0)      302 2024-04-15 13:20:49.000000 mteb-1.6.8/results/sentence-transformers__all-MiniLM-L6-v2/VGClustering.json
--rw-r--r--   0 root         (0) root         (0)      194 2024-04-15 13:20:49.000000 mteb-1.6.8/results/sentence-transformers__all-MiniLM-L6-v2/model.json
--rw-r--r--   0 root         (0) root         (0)      194 2024-04-15 13:20:49.000000 mteb-1.6.8/results/sentence-transformers__all-MiniLM-L6-v2/model_meta.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 13:20:53.679756 mteb-1.6.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/
--rw-r--r--   0 root         (0) root         (0)     1001 2024-04-15 13:20:49.000000 mteb-1.6.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/BUCC.json
--rw-r--r--   0 root         (0) root         (0)      344 2024-04-15 13:20:49.000000 mteb-1.6.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/BornholmBitextMining.json
--rw-r--r--   0 root         (0) root         (0)     5535 2024-04-15 13:20:49.000000 mteb-1.6.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CodeSearchNetRetrieval.json
--rw-r--r--   0 root         (0) root         (0)     1020 2024-04-15 13:20:49.000000 mteb-1.6.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/DanFEVER.json
--rw-r--r--   0 root         (0) root         (0)      603 2024-04-15 13:20:49.000000 mteb-1.6.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/DiaBlaBitextMining.json
--rw-r--r--   0 root         (0) root         (0)      291 2024-04-15 13:20:49.000000 mteb-1.6.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/FloresClusteringS2S.json
--rw-r--r--   0 root         (0) root         (0)     1020 2024-04-15 13:20:49.000000 mteb-1.6.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/GerDaLIR.json
--rw-r--r--   0 root         (0) root         (0)     1025 2024-04-15 13:20:49.000000 mteb-1.6.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/JaQuADRetrieval.json
--rw-r--r--   0 root         (0) root         (0)     1021 2024-04-15 13:20:49.000000 mteb-1.6.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/MedicalQARetrieval.json
--rw-r--r--   0 root         (0) root         (0)      370 2024-04-15 13:20:49.000000 mteb-1.6.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/NewsClassification.json
--rw-r--r--   0 root         (0) root         (0)     1027 2024-04-15 13:20:49.000000 mteb-1.6.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/NorQuadRetrieval.json
--rw-r--r--   0 root         (0) root         (0)      374 2024-04-15 13:20:49.000000 mteb-1.6.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/NorwegianCourtsBitextMining.json
--rw-r--r--   0 root         (0) root         (0)    16669 2024-04-15 13:20:49.000000 mteb-1.6.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/OpusparcusPC.json
--rw-r--r--   0 root         (0) root         (0)    18247 2024-04-15 13:20:49.000000 mteb-1.6.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/PawsX.json
--rw-r--r--   0 root         (0) root         (0)      300 2024-04-15 13:20:49.000000 mteb-1.6.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SNLClustering.json
--rw-r--r--   0 root         (0) root         (0)     1011 2024-04-15 13:20:49.000000 mteb-1.6.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SNLRetrieval.json
--rw-r--r--   0 root         (0) root         (0)     1021 2024-04-15 13:20:49.000000 mteb-1.6.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SweFaqRetrieval.json
--rw-r--r--   0 root         (0) root         (0)      303 2024-04-15 13:20:49.000000 mteb-1.6.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SwednClustering.json
--rw-r--r--   0 root         (0) root         (0)     1022 2024-04-15 13:20:49.000000 mteb-1.6.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SwednRetrieval.json
--rw-r--r--   0 root         (0) root         (0)     1027 2024-04-15 13:20:49.000000 mteb-1.6.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/TV2Nordretrieval.json
--rw-r--r--   0 root         (0) root         (0)     1035 2024-04-15 13:20:49.000000 mteb-1.6.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/TwitterHjerneRetrieval.json
--rw-r--r--   0 root         (0) root         (0)      300 2024-04-15 13:20:49.000000 mteb-1.6.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/VGClustering.json
--rw-r--r--   0 root         (0) root         (0)      351 2024-04-15 13:20:49.000000 mteb-1.6.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/VieMedEVBitextMining.json
--rw-r--r--   0 root         (0) root         (0)     1029 2024-04-15 13:20:49.000000 mteb-1.6.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/VieQuADRetrieval.json
--rw-r--r--   0 root         (0) root         (0)      376 2024-04-15 13:20:49.000000 mteb-1.6.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/VieStudentFeedbackClassification.json
--rw-r--r--   0 root         (0) root         (0)      366 2024-04-15 13:20:49.000000 mteb-1.6.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/WRIMEClassification.json
--rw-r--r--   0 root         (0) root         (0)      294 2024-04-15 13:20:49.000000 mteb-1.6.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/WikiCitiesClustering.json
--rw-r--r--   0 root         (0) root         (0)      176 2024-04-15 13:20:49.000000 mteb-1.6.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/model_meta.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 13:20:53.683756 mteb-1.6.8/scripts/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 13:20:53.683756 mteb-1.6.8/scripts/data/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 13:20:53.683756 mteb-1.6.8/scripts/data/amazon_polarity/
--rw-r--r--   0 root         (0) root         (0)      842 2024-04-15 13:20:49.000000 mteb-1.6.8/scripts/data/amazon_polarity/create_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 13:20:53.683756 mteb-1.6.8/scripts/data/amazon_reviews_multi/
--rw-r--r--   0 root         (0) root         (0)     1379 2024-04-15 13:20:49.000000 mteb-1.6.8/scripts/data/amazon_reviews_multi/create_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 13:20:53.683756 mteb-1.6.8/scripts/data/arxiv/
--rw-r--r--   0 root         (0) root         (0)     3146 2024-04-15 13:20:49.000000 mteb-1.6.8/scripts/data/arxiv/script_clustering.py
--rw-r--r--   0 root         (0) root         (0)     1451 2024-04-15 13:20:49.000000 mteb-1.6.8/scripts/data/arxiv/script_raw.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 13:20:53.683756 mteb-1.6.8/scripts/data/biorxiv/
--rw-r--r--   0 root         (0) root         (0)     1781 2024-04-15 13:20:49.000000 mteb-1.6.8/scripts/data/biorxiv/script_clustering.py
--rw-r--r--   0 root         (0) root         (0)     1674 2024-04-15 13:20:49.000000 mteb-1.6.8/scripts/data/biorxiv/script_raw.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 13:20:53.683756 mteb-1.6.8/scripts/data/bucc/
--rw-r--r--   0 root         (0) root         (0)     1171 2024-04-15 13:20:49.000000 mteb-1.6.8/scripts/data/bucc/create_data.py
--rw-r--r--   0 root         (0) root         (0)     5929 2024-04-15 13:20:49.000000 mteb-1.6.8/scripts/data/create_task_table.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 13:20:53.683756 mteb-1.6.8/scripts/data/germanquad/
--rw-r--r--   0 root         (0) root         (0)     2132 2024-04-15 13:20:49.000000 mteb-1.6.8/scripts/data/germanquad/process_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 13:20:53.683756 mteb-1.6.8/scripts/data/hal/
--rw-r--r--   0 root         (0) root         (0)     1512 2024-04-15 13:20:49.000000 mteb-1.6.8/scripts/data/hal/create_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 13:20:53.683756 mteb-1.6.8/scripts/data/imdb/
--rw-r--r--   0 root         (0) root         (0)      682 2024-04-15 13:20:49.000000 mteb-1.6.8/scripts/data/imdb/create_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 13:20:53.683756 mteb-1.6.8/scripts/data/medicalqaretrieval/
--rw-r--r--   0 root         (0) root         (0)     1889 2024-04-15 13:20:49.000000 mteb-1.6.8/scripts/data/medicalqaretrieval/create_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 13:20:53.683756 mteb-1.6.8/scripts/data/medrxiv/
--rw-r--r--   0 root         (0) root         (0)     1780 2024-04-15 13:20:49.000000 mteb-1.6.8/scripts/data/medrxiv/script_clustering.py
--rw-r--r--   0 root         (0) root         (0)     1617 2024-04-15 13:20:49.000000 mteb-1.6.8/scripts/data/medrxiv/script_raw.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 13:20:53.683756 mteb-1.6.8/scripts/data/mind/
--rw-r--r--   0 root         (0) root         (0)     1377 2024-04-15 13:20:49.000000 mteb-1.6.8/scripts/data/mind/prepare_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 13:20:53.683756 mteb-1.6.8/scripts/data/redditp2p/
--rw-r--r--   0 root         (0) root         (0)     1880 2024-04-15 13:20:49.000000 mteb-1.6.8/scripts/data/redditp2p/script_clustering.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 13:20:53.683756 mteb-1.6.8/scripts/data/stackexchangep2p/
--rw-r--r--   0 root         (0) root         (0)     1627 2024-04-15 13:20:49.000000 mteb-1.6.8/scripts/data/stackexchangep2p/script_clustering.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 13:20:53.687756 mteb-1.6.8/scripts/data/sts22-crosslingual-sts/
--rw-r--r--   0 root         (0) root         (0)     2436 2024-04-15 13:20:49.000000 mteb-1.6.8/scripts/data/sts22-crosslingual-sts/create_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 13:20:53.687756 mteb-1.6.8/scripts/data/summeval_fr/
--rw-r--r--   0 root         (0) root         (0)     1692 2024-04-15 13:20:49.000000 mteb-1.6.8/scripts/data/summeval_fr/create_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 13:20:53.687756 mteb-1.6.8/scripts/data/toxic_conversations_50k/
--rw-r--r--   0 root         (0) root         (0)     1151 2024-04-15 13:20:49.000000 mteb-1.6.8/scripts/data/toxic_conversations_50k/create_data.py
--rw-r--r--   0 root         (0) root         (0)     2516 2024-04-15 13:20:49.000000 mteb-1.6.8/scripts/merge_cqadupstack.py
--rw-r--r--   0 root         (0) root         (0)     5217 2024-04-15 13:20:49.000000 mteb-1.6.8/scripts/mteb_meta.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 13:20:53.619756 mteb-1.6.8/scripts/results/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 13:20:53.687756 mteb-1.6.8/scripts/results/intfloat__multilingual-e5-small/
--rw-r--r--   0 root         (0) root         (0)      376 2024-04-15 13:20:49.000000 mteb-1.6.8/scripts/results/intfloat__multilingual-e5-small/HindiDiscourseClassification.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 13:20:53.687756 mteb-1.6.8/scripts/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/
--rw-r--r--   0 root         (0) root         (0)      376 2024-04-15 13:20:49.000000 mteb-1.6.8/scripts/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/HindiDiscourseClassification.json
--rw-r--r--   0 root         (0) root         (0)      673 2024-04-15 13:20:49.000000 mteb-1.6.8/scripts/run_mteb_chinese.py
--rw-r--r--   0 root         (0) root         (0)     2819 2024-04-15 13:20:49.000000 mteb-1.6.8/scripts/run_mteb_english.py
--rw-r--r--   0 root         (0) root         (0)     1689 2024-04-15 13:20:49.000000 mteb-1.6.8/scripts/run_mteb_french.py
--rw-r--r--   0 root         (0) root         (0)     1334 2024-04-15 13:20:49.000000 mteb-1.6.8/scripts/run_mteb_german.py
--rw-r--r--   0 root         (0) root         (0)      988 2024-04-15 13:20:49.000000 mteb-1.6.8/scripts/run_mteb_korean.py
--rw-r--r--   0 root         (0) root         (0)      876 2024-04-15 13:20:49.000000 mteb-1.6.8/scripts/run_mteb_law.py
--rw-r--r--   0 root         (0) root         (0)      975 2024-04-15 13:20:49.000000 mteb-1.6.8/scripts/run_mteb_polish.py
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-15 13:20:53.687756 mteb-1.6.8/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 13:20:53.687756 mteb-1.6.8/tests/
--rw-r--r--   0 root         (0) root         (0)      632 2024-04-15 13:20:49.000000 mteb-1.6.8/tests/test_ClusteringEvaluator.py
--rw-r--r--   0 root         (0) root         (0)     1560 2024-04-15 13:20:49.000000 mteb-1.6.8/tests/test_PairClassificationEvaluator.py
--rw-r--r--   0 root         (0) root         (0)     1130 2024-04-15 13:20:49.000000 mteb-1.6.8/tests/test_RerankingEvaluator.py
--rw-r--r--   0 root         (0) root         (0)     1113 2024-04-15 13:20:49.000000 mteb-1.6.8/tests/test_RetrievalEvaluator.py
--rw-r--r--   0 root         (0) root         (0)     3715 2024-04-15 13:20:49.000000 mteb-1.6.8/tests/test_TaskMetadata.py
--rw-r--r--   0 root         (0) root         (0)     2269 2024-04-15 13:20:49.000000 mteb-1.6.8/tests/test_all_abstasks.py
--rw-r--r--   0 root         (0) root         (0)     1420 2024-04-15 13:20:49.000000 mteb-1.6.8/tests/test_mteb.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.878722 mteb-1.6.9/
+-rw-r--r--   0 root         (0) root         (0)    11357 2024-04-15 20:34:26.000000 mteb-1.6.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    23576 2024-04-15 20:34:30.878722 mteb-1.6.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     9185 2024-04-15 20:34:26.000000 mteb-1.6.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.806722 mteb-1.6.9/mteb/
+-rw-r--r--   0 root         (0) root         (0)     2135 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.810722 mteb-1.6.9/mteb/abstasks/
+-rw-r--r--   0 root         (0) root         (0)     2347 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/abstasks/AbsTask.py
+-rw-r--r--   0 root         (0) root         (0)     3063 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/abstasks/AbsTaskBitextMining.py
+-rw-r--r--   0 root         (0) root         (0)     5881 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/abstasks/AbsTaskClassification.py
+-rw-r--r--   0 root         (0) root         (0)     2389 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/abstasks/AbsTaskClustering.py
+-rw-r--r--   0 root         (0) root         (0)     2542 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/abstasks/AbsTaskPairClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1120 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/abstasks/AbsTaskReranking.py
+-rw-r--r--   0 root         (0) root         (0)    11806 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/abstasks/AbsTaskRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     2007 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/abstasks/AbsTaskSTS.py
+-rw-r--r--   0 root         (0) root         (0)     2296 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/abstasks/AbsTaskSummarization.py
+-rw-r--r--   0 root         (0) root         (0)      880 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/abstasks/CrosslingualTask.py
+-rw-r--r--   0 root         (0) root         (0)     2831 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/abstasks/LangMapping.py
+-rw-r--r--   0 root         (0) root         (0)     1031 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/abstasks/MultilingualTask.py
+-rw-r--r--   0 root         (0) root         (0)     9841 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/abstasks/TaskMetadata.py
+-rw-r--r--   0 root         (0) root         (0)      422 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/abstasks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7082 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/abstasks/iso_15924_to_script.json
+-rw-r--r--   0 root         (0) root         (0)   193114 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/abstasks/iso_639_3_to_language.json
+-rw-r--r--   0 root         (0) root         (0)      542 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/abstasks/languages.py
+-rw-r--r--   0 root         (0) root         (0)     5225 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/cmd.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.810722 mteb-1.6.9/mteb/evaluation/
+-rw-r--r--   0 root         (0) root         (0)    12990 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/evaluation/MTEB.py
+-rw-r--r--   0 root         (0) root         (0)       56 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/evaluation/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.814722 mteb-1.6.9/mteb/evaluation/evaluators/
+-rw-r--r--   0 root         (0) root         (0)     5849 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/evaluation/evaluators/BitextMiningEvaluator.py
+-rw-r--r--   0 root         (0) root         (0)     8942 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/evaluation/evaluators/ClassificationEvaluator.py
+-rw-r--r--   0 root         (0) root         (0)     1463 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/evaluation/evaluators/ClusteringEvaluator.py
+-rw-r--r--   0 root         (0) root         (0)      744 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/evaluation/evaluators/Evaluator.py
+-rw-r--r--   0 root         (0) root         (0)     7140 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/evaluation/evaluators/PairClassificationEvaluator.py
+-rw-r--r--   0 root         (0) root         (0)     9613 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/evaluation/evaluators/RerankingEvaluator.py
+-rw-r--r--   0 root         (0) root         (0)    12487 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/evaluation/evaluators/RetrievalEvaluator.py
+-rw-r--r--   0 root         (0) root         (0)     2394 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/evaluation/evaluators/STSEvaluator.py
+-rw-r--r--   0 root         (0) root         (0)     4841 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/evaluation/evaluators/SummarizationEvaluator.py
+-rw-r--r--   0 root         (0) root         (0)      324 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/evaluation/evaluators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5482 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/evaluation/evaluators/utils.py
+-rw-r--r--   0 root         (0) root         (0)      835 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/logging.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.814722 mteb-1.6.9/mteb/tasks/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.814722 mteb-1.6.9/mteb/tasks/BitextMining/
+-rw-r--r--   0 root         (0) root         (0)      420 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/BitextMining/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.814722 mteb-1.6.9/mteb/tasks/BitextMining/dan/
+-rw-r--r--   0 root         (0) root         (0)     1443 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/BitextMining/dan/BornholmskBitextMining.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/BitextMining/dan/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.814722 mteb-1.6.9/mteb/tasks/BitextMining/multilingual/
+-rw-r--r--   0 root         (0) root         (0)     1199 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/BitextMining/multilingual/BUCCBitextMining.py
+-rw-r--r--   0 root         (0) root         (0)     2281 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/BitextMining/multilingual/DiaBLaBitextMining.py
+-rw-r--r--   0 root         (0) root         (0)     5969 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/BitextMining/multilingual/FloresBitextMining.py
+-rw-r--r--   0 root         (0) root         (0)     1423 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/BitextMining/multilingual/NorwegianCourtsBitextMining.py
+-rw-r--r--   0 root         (0) root         (0)     5709 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/BitextMining/multilingual/TatoebaBitextMining.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/BitextMining/multilingual/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1363 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/BitextMining/multilingual/norwegian_courts_bitext_mining.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.814722 mteb-1.6.9/mteb/tasks/BitextMining/vie/
+-rw-r--r--   0 root         (0) root         (0)     2889 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/BitextMining/vie/VieMedEVBitextMining.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/BitextMining/vie/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.814722 mteb-1.6.9/mteb/tasks/Classification/
+-rw-r--r--   0 root         (0) root         (0)     1520 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Classification/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.818722 mteb-1.6.9/mteb/tasks/Classification/dan/
+-rw-r--r--   0 root         (0) root         (0)     1322 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Classification/dan/AngryTweetsClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1621 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Classification/dan/DKHateClassification.py
+-rw-r--r--   0 root         (0) root         (0)     2511 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Classification/dan/DalajClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1616 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Classification/dan/DanishPoliticalCommentsClassification.py
+-rw-r--r--   0 root         (0) root         (0)     2943 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Classification/dan/DdiscoCohesionClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1261 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Classification/dan/LccSentimentClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Classification/dan/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.818722 mteb-1.6.9/mteb/tasks/Classification/eng/
+-rw-r--r--   0 root         (0) root         (0)     1041 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Classification/eng/AmazonPolarityClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1054 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Classification/eng/Banking77Classification.py
+-rw-r--r--   0 root         (0) root         (0)     1374 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Classification/eng/EmotionClassification.py
+-rw-r--r--   0 root         (0) root         (0)      990 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Classification/eng/ImdbClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1085 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Classification/eng/NewsClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1406 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Classification/eng/ToxicConversationsClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1281 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Classification/eng/TweetSentimentExtractionClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Classification/eng/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.818722 mteb-1.6.9/mteb/tasks/Classification/hin/
+-rw-r--r--   0 root         (0) root         (0)     2195 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Classification/hin/HindiDiscourseClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Classification/hin/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.818722 mteb-1.6.9/mteb/tasks/Classification/jpn/
+-rw-r--r--   0 root         (0) root         (0)     3550 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Classification/jpn/WRIMEClassification.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.822722 mteb-1.6.9/mteb/tasks/Classification/multilingual/
+-rw-r--r--   0 root         (0) root         (0)     1575 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Classification/multilingual/AmazonCounterfactualClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1377 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Classification/multilingual/AmazonReviewsClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1275 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Classification/multilingual/MTOPDomainClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1275 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Classification/multilingual/MTOPIntentClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1627 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Classification/multilingual/MasakhaNEWSClassification.py
+-rw-r--r--   0 root         (0) root         (0)     2537 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Classification/multilingual/MassiveIntentClassification.py
+-rw-r--r--   0 root         (0) root         (0)     2543 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Classification/multilingual/MassiveScenarioClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1611 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Classification/multilingual/NordicLangClassification.py
+-rw-r--r--   0 root         (0) root         (0)     6099 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Classification/multilingual/ScalaClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Classification/multilingual/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.822722 mteb-1.6.9/mteb/tasks/Classification/nob/
+-rw-r--r--   0 root         (0) root         (0)     1121 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Classification/nob/NoRecClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1173 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Classification/nob/NorwegianParliamentClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Classification/nob/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.822722 mteb-1.6.9/mteb/tasks/Classification/pol/
+-rw-r--r--   0 root         (0) root         (0)     4922 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Classification/pol/PolishClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Classification/pol/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.822722 mteb-1.6.9/mteb/tasks/Classification/swe/
+-rw-r--r--   0 root         (0) root         (0)     1043 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Classification/swe/SweRecClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Classification/swe/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.822722 mteb-1.6.9/mteb/tasks/Classification/vie/
+-rw-r--r--   0 root         (0) root         (0)     3368 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Classification/vie/VieStudentFeedbackClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Classification/vie/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.822722 mteb-1.6.9/mteb/tasks/Classification/zho/
+-rw-r--r--   0 root         (0) root         (0)     6571 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Classification/zho/CMTEBClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1729 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Classification/zho/YueOpenriceReviewClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Classification/zho/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.822722 mteb-1.6.9/mteb/tasks/Clustering/
+-rw-r--r--   0 root         (0) root         (0)     1278 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Clustering/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.822722 mteb-1.6.9/mteb/tasks/Clustering/deu/
+-rw-r--r--   0 root         (0) root         (0)     1132 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Clustering/deu/BlurbsClusteringP2P.py
+-rw-r--r--   0 root         (0) root         (0)     1124 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Clustering/deu/BlurbsClusteringS2S.py
+-rw-r--r--   0 root         (0) root         (0)     1100 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Clustering/deu/TenKGnadClusteringP2P.py
+-rw-r--r--   0 root         (0) root         (0)     1080 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Clustering/deu/TenKGnadClusteringS2S.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Clustering/deu/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.826722 mteb-1.6.9/mteb/tasks/Clustering/eng/
+-rw-r--r--   0 root         (0) root         (0)     1101 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Clustering/eng/ArxivClusteringP2P.py
+-rw-r--r--   0 root         (0) root         (0)     1087 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Clustering/eng/ArxivClusteringS2S.py
+-rw-r--r--   0 root         (0) root         (0)     1128 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Clustering/eng/BigPatentClustering.py
+-rw-r--r--   0 root         (0) root         (0)     1071 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Clustering/eng/BiorxivClusteringP2P.py
+-rw-r--r--   0 root         (0) root         (0)     1061 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Clustering/eng/BiorxivClusteringS2S.py
+-rw-r--r--   0 root         (0) root         (0)     1072 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Clustering/eng/MedrxivClusteringP2P.py
+-rw-r--r--   0 root         (0) root         (0)     1062 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Clustering/eng/MedrxivClusteringS2S.py
+-rw-r--r--   0 root         (0) root         (0)     1102 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Clustering/eng/RedditClustering.py
+-rw-r--r--   0 root         (0) root         (0)     1091 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Clustering/eng/RedditClusteringP2P.py
+-rw-r--r--   0 root         (0) root         (0)     1127 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Clustering/eng/StackExchangeClustering.py
+-rw-r--r--   0 root         (0) root         (0)     1115 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Clustering/eng/StackExchangeClusteringP2P.py
+-rw-r--r--   0 root         (0) root         (0)     1084 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Clustering/eng/TwentyNewsgroupsClustering.py
+-rw-r--r--   0 root         (0) root         (0)     1135 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Clustering/eng/WikiCitiesClustering.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Clustering/eng/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.826722 mteb-1.6.9/mteb/tasks/Clustering/fra/
+-rw-r--r--   0 root         (0) root         (0)     1911 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Clustering/fra/AlloProfClusteringP2P.py
+-rw-r--r--   0 root         (0) root         (0)     1757 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Clustering/fra/AlloProfClusteringS2S.py
+-rw-r--r--   0 root         (0) root         (0)     1625 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Clustering/fra/HALClusteringS2S.py
+-rw-r--r--   0 root         (0) root         (0)     1942 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Clustering/fra/MLSUMClusteringP2P.py
+-rw-r--r--   0 root         (0) root         (0)     1757 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Clustering/fra/MLSUMClusteringS2S.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Clustering/fra/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.830722 mteb-1.6.9/mteb/tasks/Clustering/multilingual/
+-rw-r--r--   0 root         (0) root         (0)     2723 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Clustering/multilingual/MasakhaNEWSClusteringP2P.py
+-rw-r--r--   0 root         (0) root         (0)     2737 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Clustering/multilingual/MasakhaNEWSClusteringS2S.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Clustering/multilingual/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.830722 mteb-1.6.9/mteb/tasks/Clustering/nob/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Clustering/nob/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3442 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Clustering/nob/snl_clustering.py
+-rw-r--r--   0 root         (0) root         (0)     3596 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Clustering/nob/vg_clustering.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.830722 mteb-1.6.9/mteb/tasks/Clustering/pol/
+-rw-r--r--   0 root         (0) root         (0)     1137 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Clustering/pol/PolishClustering.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Clustering/pol/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.830722 mteb-1.6.9/mteb/tasks/Clustering/spa/
+-rw-r--r--   0 root         (0) root         (0)     1042 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Clustering/spa/FloresClusteringS2S.py
+-rw-r--r--   0 root         (0) root         (0)     1060 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Clustering/spa/SpanishNewsClusteringP2P.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Clustering/spa/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.830722 mteb-1.6.9/mteb/tasks/Clustering/swe/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Clustering/swe/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3926 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Clustering/swe/swedn_clustering.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.830722 mteb-1.6.9/mteb/tasks/Clustering/zho/
+-rw-r--r--   0 root         (0) root         (0)     3639 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Clustering/zho/CMTEBClustering.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Clustering/zho/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.830722 mteb-1.6.9/mteb/tasks/PairClassification/
+-rw-r--r--   0 root         (0) root         (0)      344 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/PairClassification/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.830722 mteb-1.6.9/mteb/tasks/PairClassification/deu/
+-rw-r--r--   0 root         (0) root         (0)     2862 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/PairClassification/deu/FalseFriendsDeEnPC.py
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/PairClassification/deu/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.830722 mteb-1.6.9/mteb/tasks/PairClassification/eng/
+-rw-r--r--   0 root         (0) root         (0)     1152 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/PairClassification/eng/SprintDuplicateQuestionsPC.py
+-rw-r--r--   0 root         (0) root         (0)     1086 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/PairClassification/eng/TwitterSemEval2015PC.py
+-rw-r--r--   0 root         (0) root         (0)     1040 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/PairClassification/eng/TwitterURLCorpusPC.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/PairClassification/eng/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.834722 mteb-1.6.9/mteb/tasks/PairClassification/multilingual/
+-rw-r--r--   0 root         (0) root         (0)     2798 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/PairClassification/multilingual/OpusparcusPC.py
+-rw-r--r--   0 root         (0) root         (0)     1768 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/PairClassification/multilingual/PawsX.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/PairClassification/multilingual/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.834722 mteb-1.6.9/mteb/tasks/PairClassification/pol/
+-rw-r--r--   0 root         (0) root         (0)     3577 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/PairClassification/pol/PolishPC.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/PairClassification/pol/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.834722 mteb-1.6.9/mteb/tasks/PairClassification/zho/
+-rw-r--r--   0 root         (0) root         (0)     1849 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/PairClassification/zho/CMTEBPairClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/PairClassification/zho/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.834722 mteb-1.6.9/mteb/tasks/Reranking/
+-rw-r--r--   0 root         (0) root         (0)      346 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Reranking/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.834722 mteb-1.6.9/mteb/tasks/Reranking/eng/
+-rw-r--r--   0 root         (0) root         (0)     1118 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Reranking/eng/AskUbuntuDupQuestions.py
+-rw-r--r--   0 root         (0) root         (0)     1103 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Reranking/eng/MindSmallReranking.py
+-rw-r--r--   0 root         (0) root         (0)     3054 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Reranking/eng/SciDocsReranking.py
+-rw-r--r--   0 root         (0) root         (0)     1137 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Reranking/eng/StackOverflowDupQuestions.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Reranking/eng/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.834722 mteb-1.6.9/mteb/tasks/Reranking/fra/
+-rw-r--r--   0 root         (0) root         (0)     1195 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Reranking/fra/AlloprofReranking.py
+-rw-r--r--   0 root         (0) root         (0)     1065 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Reranking/fra/SyntecReranking.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Reranking/fra/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.834722 mteb-1.6.9/mteb/tasks/Reranking/multilingual/
+-rw-r--r--   0 root         (0) root         (0)     1269 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Reranking/multilingual/MIRACLReranking.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Reranking/multilingual/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.834722 mteb-1.6.9/mteb/tasks/Reranking/zho/
+-rw-r--r--   0 root         (0) root         (0)     3528 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Reranking/zho/CMTEBReranking.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Reranking/zho/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.834722 mteb-1.6.9/mteb/tasks/Retrieval/
+-rw-r--r--   0 root         (0) root         (0)     3005 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.838722 mteb-1.6.9/mteb/tasks/Retrieval/code/
+-rw-r--r--   0 root         (0) root         (0)     3377 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/code/CodeSearchNetRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/code/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.838722 mteb-1.6.9/mteb/tasks/Retrieval/dan/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/dan/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3794 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/dan/dan_fever.py
+-rw-r--r--   0 root         (0) root         (0)     2583 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/dan/t2nord_retrieval.py
+-rw-r--r--   0 root         (0) root         (0)     3148 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/dan/twitterhjerne.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.838722 mteb-1.6.9/mteb/tasks/Retrieval/deu/
+-rw-r--r--   0 root         (0) root         (0)     2048 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/deu/GerDaLIRRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1228 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/deu/GerDaLIRSmallRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     2876 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/deu/GermanDPRRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     2127 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/deu/GermanQuADRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1052 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/deu/LegalQuADRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/deu/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.846722 mteb-1.6.9/mteb/tasks/Retrieval/eng/
+-rw-r--r--   0 root         (0) root         (0)     1118 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/eng/AILACasedocsRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1086 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/eng/AILAStatutesRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1011 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/eng/ArguAnaRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1065 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/eng/CQADupstackAndroidRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1065 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/eng/CQADupstackEnglishRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1062 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/eng/CQADupstackGamingRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1053 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/eng/CQADupstackGisRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1077 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/eng/CQADupstackMathematicaRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1065 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/eng/CQADupstackPhysicsRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1077 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/eng/CQADupstackProgrammersRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1059 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/eng/CQADupstackStatsRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1053 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/eng/CQADupstackTexRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1056 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/eng/CQADupstackUnixRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1074 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/eng/CQADupstackWebmastersRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1071 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/eng/CQADupstackWordpressRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1095 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/eng/ClimateFEVERRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1031 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/eng/DBPediaRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1175 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/eng/FEVERRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)      983 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/eng/FiQA2018Retrieval.py
+-rw-r--r--   0 root         (0) root         (0)     3705 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/eng/HagridRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1151 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/eng/HotpotQARetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1146 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/eng/LegalBenchConsumerContractsQARetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1150 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/eng/LegalBenchCorporateLobbyingRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1147 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/eng/LegalSummarizationRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1009 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/eng/MSMARCORetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1039 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/eng/MSMARCOv2Retrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1650 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/eng/MedicalQARetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1024 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/eng/NFCorpusRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)      999 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/eng/NQRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1991 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/eng/NarrativeQARetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1155 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/eng/QuoraRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1114 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/eng/SCIDOCSRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1046 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/eng/SciFactRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1069 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/eng/TRECCOVIDRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1009 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/eng/Touche2020Retrieval.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/eng/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.846722 mteb-1.6.9/mteb/tasks/Retrieval/fra/
+-rw-r--r--   0 root         (0) root         (0)     2145 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/fra/AlloprofRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     2475 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/fra/BSARDRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     2127 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/fra/SyntecRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/fra/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.846722 mteb-1.6.9/mteb/tasks/Retrieval/jpn/
+-rw-r--r--   0 root         (0) root         (0)     2853 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/jpn/JaQuADRetrieval.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.846722 mteb-1.6.9/mteb/tasks/Retrieval/kor/
+-rw-r--r--   0 root         (0) root         (0)      906 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/kor/KoMiracl.py
+-rw-r--r--   0 root         (0) root         (0)      922 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/kor/KoStrategyQA.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/kor/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.846722 mteb-1.6.9/mteb/tasks/Retrieval/multilingual/
+-rw-r--r--   0 root         (0) root         (0)     3277 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/multilingual/MIRACLRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     3052 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/multilingual/MintakaRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     3432 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/multilingual/MultiLongDocRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     2979 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/multilingual/XMarketRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     3145 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/multilingual/XPQARetrieval.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/multilingual/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.846722 mteb-1.6.9/mteb/tasks/Retrieval/nob/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/nob/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3952 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/nob/norquad.py
+-rw-r--r--   0 root         (0) root         (0)     2708 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/nob/snl_retrieval.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.850722 mteb-1.6.9/mteb/tasks/Retrieval/pol/
+-rw-r--r--   0 root         (0) root         (0)      967 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/pol/ArguAnaPLRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1040 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/pol/DBPediaPLRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)      984 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/pol/FiQAPLRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1112 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/pol/HotpotQAPLRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1009 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/pol/MSMARCOPLRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1040 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/pol/NFCorpusPLRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)      997 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/pol/NQPLRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1130 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/pol/QuoraPLRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1091 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/pol/SCIDOCSPLRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1053 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/pol/SciFactPLRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1085 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/pol/TRECCOVIDPLRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/pol/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.850722 mteb-1.6.9/mteb/tasks/Retrieval/spa/
+-rw-r--r--   0 root         (0) root         (0)     2125 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/spa/SpanishPassageRetrievalS2P.py
+-rw-r--r--   0 root         (0) root         (0)     2056 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/spa/SpanishPassageRetrievalS2S.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/spa/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.850722 mteb-1.6.9/mteb/tasks/Retrieval/swe/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/swe/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3219 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/swe/swedn_retrieval.py
+-rw-r--r--   0 root         (0) root         (0)     2619 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/swe/swefaq_retrieval.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.850722 mteb-1.6.9/mteb/tasks/Retrieval/vie/
+-rw-r--r--   0 root         (0) root         (0)     3798 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/vie/VieQuADRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/vie/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.850722 mteb-1.6.9/mteb/tasks/Retrieval/zho/
+-rw-r--r--   0 root         (0) root         (0)    10384 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/zho/CMTEBRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1121 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/zho/LeCaRDv2Retrieval.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Retrieval/zho/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.850722 mteb-1.6.9/mteb/tasks/STS/
+-rw-r--r--   0 root         (0) root         (0)      575 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/STS/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.854722 mteb-1.6.9/mteb/tasks/STS/deu/
+-rw-r--r--   0 root         (0) root         (0)     1370 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/STS/deu/GermanSTSBenchmarkSTS.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/STS/deu/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.854722 mteb-1.6.9/mteb/tasks/STS/eng/
+-rw-r--r--   0 root         (0) root         (0)     1184 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/STS/eng/BiossesSTS.py
+-rw-r--r--   0 root         (0) root         (0)     1153 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/STS/eng/STS12STS.py
+-rw-r--r--   0 root         (0) root         (0)     1150 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/STS/eng/STS13STS.py
+-rw-r--r--   0 root         (0) root         (0)     1184 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/STS/eng/STS14STS.py
+-rw-r--r--   0 root         (0) root         (0)     1148 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/STS/eng/STS15STS.py
+-rw-r--r--   0 root         (0) root         (0)     1148 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/STS/eng/STS16STS.py
+-rw-r--r--   0 root         (0) root         (0)     1208 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/STS/eng/STSBenchmarkSTS.py
+-rw-r--r--   0 root         (0) root         (0)     1185 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/STS/eng/SickrSTS.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/STS/eng/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.854722 mteb-1.6.9/mteb/tasks/STS/fra/
+-rw-r--r--   0 root         (0) root         (0)     1472 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/STS/fra/SickFrSTS.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/STS/fra/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.854722 mteb-1.6.9/mteb/tasks/STS/multilingual/
+-rw-r--r--   0 root         (0) root         (0)     1600 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/STS/multilingual/STS17CrosslingualSTS.py
+-rw-r--r--   0 root         (0) root         (0)     1832 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/STS/multilingual/STS22CrosslingualSTS.py
+-rw-r--r--   0 root         (0) root         (0)     2712 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/STS/multilingual/STSBenchmarkMultilingualSTS.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/STS/multilingual/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.854722 mteb-1.6.9/mteb/tasks/STS/pol/
+-rw-r--r--   0 root         (0) root         (0)     2268 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/STS/pol/PolishSTS.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/STS/pol/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.854722 mteb-1.6.9/mteb/tasks/STS/spa/
+-rw-r--r--   0 root         (0) root         (0)     1486 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/STS/spa/STSES.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/STS/spa/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.854722 mteb-1.6.9/mteb/tasks/STS/zho/
+-rw-r--r--   0 root         (0) root         (0)     7122 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/STS/zho/CMTEBSTS.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/STS/zho/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.854722 mteb-1.6.9/mteb/tasks/Summarization/
+-rw-r--r--   0 root         (0) root         (0)      124 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Summarization/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.858722 mteb-1.6.9/mteb/tasks/Summarization/eng/
+-rw-r--r--   0 root         (0) root         (0)     1243 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Summarization/eng/SummEvalSummarization.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Summarization/eng/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.858722 mteb-1.6.9/mteb/tasks/Summarization/fra/
+-rw-r--r--   0 root         (0) root         (0)     1304 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Summarization/fra/SummEvalFrSummarization.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/Summarization/fra/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      252 2024-04-15 20:34:26.000000 mteb-1.6.9/mteb/tasks/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.878722 mteb-1.6.9/mteb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    23576 2024-04-15 20:34:30.000000 mteb-1.6.9/mteb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    19373 2024-04-15 20:34:30.000000 mteb-1.6.9/mteb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-15 20:34:30.000000 mteb-1.6.9/mteb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       39 2024-04-15 20:34:30.000000 mteb-1.6.9/mteb.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      234 2024-04-15 20:34:30.000000 mteb-1.6.9/mteb.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2024-04-15 20:34:30.000000 mteb-1.6.9/mteb.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     2169 2024-04-15 20:34:27.000000 mteb-1.6.9/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.798722 mteb-1.6.9/results/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.862722 mteb-1.6.9/results/intfloat__multilingual-e5-small/
+-rw-r--r--   0 root         (0) root         (0)     5524 2024-04-15 20:34:26.000000 mteb-1.6.9/results/intfloat__multilingual-e5-small/CodeSearchNetRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)     1016 2024-04-15 20:34:26.000000 mteb-1.6.9/results/intfloat__multilingual-e5-small/DanFEVER.json
+-rw-r--r--   0 root         (0) root         (0)     1027 2024-04-15 20:34:26.000000 mteb-1.6.9/results/intfloat__multilingual-e5-small/JaQuADRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)     1025 2024-04-15 20:34:26.000000 mteb-1.6.9/results/intfloat__multilingual-e5-small/MedicalQARetrieval.json
+-rw-r--r--   0 root         (0) root         (0)      371 2024-04-15 20:34:26.000000 mteb-1.6.9/results/intfloat__multilingual-e5-small/NewsClassification.json
+-rw-r--r--   0 root         (0) root         (0)     1021 2024-04-15 20:34:26.000000 mteb-1.6.9/results/intfloat__multilingual-e5-small/NorQuadRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)      374 2024-04-15 20:34:26.000000 mteb-1.6.9/results/intfloat__multilingual-e5-small/NorwegianCourtsBitextMining.json
+-rw-r--r--   0 root         (0) root         (0)      298 2024-04-15 20:34:26.000000 mteb-1.6.9/results/intfloat__multilingual-e5-small/SNLClustering.json
+-rw-r--r--   0 root         (0) root         (0)     1023 2024-04-15 20:34:26.000000 mteb-1.6.9/results/intfloat__multilingual-e5-small/SNLRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)     1015 2024-04-15 20:34:26.000000 mteb-1.6.9/results/intfloat__multilingual-e5-small/SweFaqRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)      304 2024-04-15 20:34:26.000000 mteb-1.6.9/results/intfloat__multilingual-e5-small/SwednClustering.json
+-rw-r--r--   0 root         (0) root         (0)     1023 2024-04-15 20:34:26.000000 mteb-1.6.9/results/intfloat__multilingual-e5-small/SwednRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)     1021 2024-04-15 20:34:26.000000 mteb-1.6.9/results/intfloat__multilingual-e5-small/TV2Nordretrieval.json
+-rw-r--r--   0 root         (0) root         (0)     1034 2024-04-15 20:34:26.000000 mteb-1.6.9/results/intfloat__multilingual-e5-small/TwitterHjerneRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)      303 2024-04-15 20:34:26.000000 mteb-1.6.9/results/intfloat__multilingual-e5-small/VGClustering.json
+-rw-r--r--   0 root         (0) root         (0)      351 2024-04-15 20:34:26.000000 mteb-1.6.9/results/intfloat__multilingual-e5-small/VieMedEVBitextMining.json
+-rw-r--r--   0 root         (0) root         (0)     1028 2024-04-15 20:34:26.000000 mteb-1.6.9/results/intfloat__multilingual-e5-small/VieQuADRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)      377 2024-04-15 20:34:26.000000 mteb-1.6.9/results/intfloat__multilingual-e5-small/VieStudentFeedbackClassification.json
+-rw-r--r--   0 root         (0) root         (0)      364 2024-04-15 20:34:26.000000 mteb-1.6.9/results/intfloat__multilingual-e5-small/WRIMEClassification.json
+-rw-r--r--   0 root         (0) root         (0)      387 2024-04-15 20:34:26.000000 mteb-1.6.9/results/intfloat__multilingual-e5-small/YueOpenriceReviewClassification.json
+-rw-r--r--   0 root         (0) root         (0)      111 2024-04-15 20:34:26.000000 mteb-1.6.9/results/intfloat__multilingual-e5-small/model_meta.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.862722 mteb-1.6.9/results/sentence-transformers__all-MiniLM-L6-v2/
+-rw-r--r--   0 root         (0) root         (0)      385 2024-04-15 20:34:26.000000 mteb-1.6.9/results/sentence-transformers__all-MiniLM-L6-v2/Banking77Classification.json
+-rw-r--r--   0 root         (0) root         (0)      340 2024-04-15 20:34:26.000000 mteb-1.6.9/results/sentence-transformers__all-MiniLM-L6-v2/BornholmBitextMining.json
+-rw-r--r--   0 root         (0) root         (0)     1020 2024-04-15 20:34:26.000000 mteb-1.6.9/results/sentence-transformers__all-MiniLM-L6-v2/DanFEVER.json
+-rw-r--r--   0 root         (0) root         (0)     1027 2024-04-15 20:34:26.000000 mteb-1.6.9/results/sentence-transformers__all-MiniLM-L6-v2/NorQuadRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)      374 2024-04-15 20:34:26.000000 mteb-1.6.9/results/sentence-transformers__all-MiniLM-L6-v2/NorwegianCourtsBitextMining.json
+-rw-r--r--   0 root         (0) root         (0)      303 2024-04-15 20:34:26.000000 mteb-1.6.9/results/sentence-transformers__all-MiniLM-L6-v2/SNLClustering.json
+-rw-r--r--   0 root         (0) root         (0)     1021 2024-04-15 20:34:26.000000 mteb-1.6.9/results/sentence-transformers__all-MiniLM-L6-v2/SNLRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)     1014 2024-04-15 20:34:26.000000 mteb-1.6.9/results/sentence-transformers__all-MiniLM-L6-v2/SweFaqRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)      306 2024-04-15 20:34:26.000000 mteb-1.6.9/results/sentence-transformers__all-MiniLM-L6-v2/SwednClustering.json
+-rw-r--r--   0 root         (0) root         (0)     1025 2024-04-15 20:34:26.000000 mteb-1.6.9/results/sentence-transformers__all-MiniLM-L6-v2/SwednRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)     1021 2024-04-15 20:34:26.000000 mteb-1.6.9/results/sentence-transformers__all-MiniLM-L6-v2/TV2Nordretrieval.json
+-rw-r--r--   0 root         (0) root         (0)     1034 2024-04-15 20:34:26.000000 mteb-1.6.9/results/sentence-transformers__all-MiniLM-L6-v2/TwitterHjerneRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)      302 2024-04-15 20:34:26.000000 mteb-1.6.9/results/sentence-transformers__all-MiniLM-L6-v2/VGClustering.json
+-rw-r--r--   0 root         (0) root         (0)      194 2024-04-15 20:34:26.000000 mteb-1.6.9/results/sentence-transformers__all-MiniLM-L6-v2/model.json
+-rw-r--r--   0 root         (0) root         (0)      194 2024-04-15 20:34:26.000000 mteb-1.6.9/results/sentence-transformers__all-MiniLM-L6-v2/model_meta.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.870722 mteb-1.6.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/
+-rw-r--r--   0 root         (0) root         (0)     1001 2024-04-15 20:34:26.000000 mteb-1.6.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/BUCC.json
+-rw-r--r--   0 root         (0) root         (0)      344 2024-04-15 20:34:26.000000 mteb-1.6.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/BornholmBitextMining.json
+-rw-r--r--   0 root         (0) root         (0)     5535 2024-04-15 20:34:26.000000 mteb-1.6.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CodeSearchNetRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)     1020 2024-04-15 20:34:26.000000 mteb-1.6.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/DanFEVER.json
+-rw-r--r--   0 root         (0) root         (0)      603 2024-04-15 20:34:26.000000 mteb-1.6.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/DiaBlaBitextMining.json
+-rw-r--r--   0 root         (0) root         (0)      291 2024-04-15 20:34:26.000000 mteb-1.6.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/FloresClusteringS2S.json
+-rw-r--r--   0 root         (0) root         (0)     1020 2024-04-15 20:34:26.000000 mteb-1.6.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/GerDaLIR.json
+-rw-r--r--   0 root         (0) root         (0)     1025 2024-04-15 20:34:26.000000 mteb-1.6.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/JaQuADRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)     1021 2024-04-15 20:34:26.000000 mteb-1.6.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/MedicalQARetrieval.json
+-rw-r--r--   0 root         (0) root         (0)      370 2024-04-15 20:34:26.000000 mteb-1.6.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/NewsClassification.json
+-rw-r--r--   0 root         (0) root         (0)     1027 2024-04-15 20:34:26.000000 mteb-1.6.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/NorQuadRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)      374 2024-04-15 20:34:26.000000 mteb-1.6.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/NorwegianCourtsBitextMining.json
+-rw-r--r--   0 root         (0) root         (0)    16669 2024-04-15 20:34:26.000000 mteb-1.6.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/OpusparcusPC.json
+-rw-r--r--   0 root         (0) root         (0)    18247 2024-04-15 20:34:26.000000 mteb-1.6.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/PawsX.json
+-rw-r--r--   0 root         (0) root         (0)      300 2024-04-15 20:34:26.000000 mteb-1.6.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SNLClustering.json
+-rw-r--r--   0 root         (0) root         (0)     1011 2024-04-15 20:34:26.000000 mteb-1.6.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SNLRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)     1021 2024-04-15 20:34:26.000000 mteb-1.6.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SweFaqRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)      303 2024-04-15 20:34:26.000000 mteb-1.6.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SwednClustering.json
+-rw-r--r--   0 root         (0) root         (0)     1022 2024-04-15 20:34:26.000000 mteb-1.6.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SwednRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)     1027 2024-04-15 20:34:26.000000 mteb-1.6.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/TV2Nordretrieval.json
+-rw-r--r--   0 root         (0) root         (0)     1035 2024-04-15 20:34:26.000000 mteb-1.6.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/TwitterHjerneRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)      300 2024-04-15 20:34:26.000000 mteb-1.6.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/VGClustering.json
+-rw-r--r--   0 root         (0) root         (0)      351 2024-04-15 20:34:26.000000 mteb-1.6.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/VieMedEVBitextMining.json
+-rw-r--r--   0 root         (0) root         (0)     1029 2024-04-15 20:34:26.000000 mteb-1.6.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/VieQuADRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)      376 2024-04-15 20:34:26.000000 mteb-1.6.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/VieStudentFeedbackClassification.json
+-rw-r--r--   0 root         (0) root         (0)      366 2024-04-15 20:34:26.000000 mteb-1.6.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/WRIMEClassification.json
+-rw-r--r--   0 root         (0) root         (0)      294 2024-04-15 20:34:26.000000 mteb-1.6.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/WikiCitiesClustering.json
+-rw-r--r--   0 root         (0) root         (0)      387 2024-04-15 20:34:26.000000 mteb-1.6.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/YueOpenriceReviewClassification.json
+-rw-r--r--   0 root         (0) root         (0)      176 2024-04-15 20:34:26.000000 mteb-1.6.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/model_meta.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.870722 mteb-1.6.9/scripts/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.870722 mteb-1.6.9/scripts/data/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.870722 mteb-1.6.9/scripts/data/amazon_polarity/
+-rw-r--r--   0 root         (0) root         (0)      842 2024-04-15 20:34:26.000000 mteb-1.6.9/scripts/data/amazon_polarity/create_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.870722 mteb-1.6.9/scripts/data/amazon_reviews_multi/
+-rw-r--r--   0 root         (0) root         (0)     1379 2024-04-15 20:34:26.000000 mteb-1.6.9/scripts/data/amazon_reviews_multi/create_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.870722 mteb-1.6.9/scripts/data/arxiv/
+-rw-r--r--   0 root         (0) root         (0)     3146 2024-04-15 20:34:26.000000 mteb-1.6.9/scripts/data/arxiv/script_clustering.py
+-rw-r--r--   0 root         (0) root         (0)     1451 2024-04-15 20:34:26.000000 mteb-1.6.9/scripts/data/arxiv/script_raw.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.870722 mteb-1.6.9/scripts/data/biorxiv/
+-rw-r--r--   0 root         (0) root         (0)     1781 2024-04-15 20:34:26.000000 mteb-1.6.9/scripts/data/biorxiv/script_clustering.py
+-rw-r--r--   0 root         (0) root         (0)     1674 2024-04-15 20:34:26.000000 mteb-1.6.9/scripts/data/biorxiv/script_raw.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.874722 mteb-1.6.9/scripts/data/bucc/
+-rw-r--r--   0 root         (0) root         (0)     1171 2024-04-15 20:34:26.000000 mteb-1.6.9/scripts/data/bucc/create_data.py
+-rw-r--r--   0 root         (0) root         (0)     5929 2024-04-15 20:34:26.000000 mteb-1.6.9/scripts/data/create_task_table.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.874722 mteb-1.6.9/scripts/data/germanquad/
+-rw-r--r--   0 root         (0) root         (0)     2132 2024-04-15 20:34:26.000000 mteb-1.6.9/scripts/data/germanquad/process_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.874722 mteb-1.6.9/scripts/data/hal/
+-rw-r--r--   0 root         (0) root         (0)     1512 2024-04-15 20:34:26.000000 mteb-1.6.9/scripts/data/hal/create_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.874722 mteb-1.6.9/scripts/data/imdb/
+-rw-r--r--   0 root         (0) root         (0)      682 2024-04-15 20:34:26.000000 mteb-1.6.9/scripts/data/imdb/create_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.874722 mteb-1.6.9/scripts/data/medicalqaretrieval/
+-rw-r--r--   0 root         (0) root         (0)     1889 2024-04-15 20:34:26.000000 mteb-1.6.9/scripts/data/medicalqaretrieval/create_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.874722 mteb-1.6.9/scripts/data/medrxiv/
+-rw-r--r--   0 root         (0) root         (0)     1780 2024-04-15 20:34:26.000000 mteb-1.6.9/scripts/data/medrxiv/script_clustering.py
+-rw-r--r--   0 root         (0) root         (0)     1617 2024-04-15 20:34:26.000000 mteb-1.6.9/scripts/data/medrxiv/script_raw.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.874722 mteb-1.6.9/scripts/data/mind/
+-rw-r--r--   0 root         (0) root         (0)     1377 2024-04-15 20:34:26.000000 mteb-1.6.9/scripts/data/mind/prepare_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.874722 mteb-1.6.9/scripts/data/redditp2p/
+-rw-r--r--   0 root         (0) root         (0)     1880 2024-04-15 20:34:26.000000 mteb-1.6.9/scripts/data/redditp2p/script_clustering.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.874722 mteb-1.6.9/scripts/data/stackexchangep2p/
+-rw-r--r--   0 root         (0) root         (0)     1627 2024-04-15 20:34:26.000000 mteb-1.6.9/scripts/data/stackexchangep2p/script_clustering.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.874722 mteb-1.6.9/scripts/data/sts22-crosslingual-sts/
+-rw-r--r--   0 root         (0) root         (0)     2436 2024-04-15 20:34:26.000000 mteb-1.6.9/scripts/data/sts22-crosslingual-sts/create_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.874722 mteb-1.6.9/scripts/data/summeval_fr/
+-rw-r--r--   0 root         (0) root         (0)     1692 2024-04-15 20:34:26.000000 mteb-1.6.9/scripts/data/summeval_fr/create_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.874722 mteb-1.6.9/scripts/data/toxic_conversations_50k/
+-rw-r--r--   0 root         (0) root         (0)     1151 2024-04-15 20:34:26.000000 mteb-1.6.9/scripts/data/toxic_conversations_50k/create_data.py
+-rw-r--r--   0 root         (0) root         (0)     2516 2024-04-15 20:34:26.000000 mteb-1.6.9/scripts/merge_cqadupstack.py
+-rw-r--r--   0 root         (0) root         (0)     5217 2024-04-15 20:34:26.000000 mteb-1.6.9/scripts/mteb_meta.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.802722 mteb-1.6.9/scripts/results/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.874722 mteb-1.6.9/scripts/results/intfloat__multilingual-e5-small/
+-rw-r--r--   0 root         (0) root         (0)      376 2024-04-15 20:34:26.000000 mteb-1.6.9/scripts/results/intfloat__multilingual-e5-small/HindiDiscourseClassification.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.874722 mteb-1.6.9/scripts/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/
+-rw-r--r--   0 root         (0) root         (0)      376 2024-04-15 20:34:26.000000 mteb-1.6.9/scripts/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/HindiDiscourseClassification.json
+-rw-r--r--   0 root         (0) root         (0)      673 2024-04-15 20:34:26.000000 mteb-1.6.9/scripts/run_mteb_chinese.py
+-rw-r--r--   0 root         (0) root         (0)     2819 2024-04-15 20:34:26.000000 mteb-1.6.9/scripts/run_mteb_english.py
+-rw-r--r--   0 root         (0) root         (0)     1689 2024-04-15 20:34:26.000000 mteb-1.6.9/scripts/run_mteb_french.py
+-rw-r--r--   0 root         (0) root         (0)     1334 2024-04-15 20:34:26.000000 mteb-1.6.9/scripts/run_mteb_german.py
+-rw-r--r--   0 root         (0) root         (0)      988 2024-04-15 20:34:26.000000 mteb-1.6.9/scripts/run_mteb_korean.py
+-rw-r--r--   0 root         (0) root         (0)      876 2024-04-15 20:34:26.000000 mteb-1.6.9/scripts/run_mteb_law.py
+-rw-r--r--   0 root         (0) root         (0)      975 2024-04-15 20:34:26.000000 mteb-1.6.9/scripts/run_mteb_polish.py
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-15 20:34:30.878722 mteb-1.6.9/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:34:30.878722 mteb-1.6.9/tests/
+-rw-r--r--   0 root         (0) root         (0)      632 2024-04-15 20:34:26.000000 mteb-1.6.9/tests/test_ClusteringEvaluator.py
+-rw-r--r--   0 root         (0) root         (0)     1560 2024-04-15 20:34:26.000000 mteb-1.6.9/tests/test_PairClassificationEvaluator.py
+-rw-r--r--   0 root         (0) root         (0)     1130 2024-04-15 20:34:26.000000 mteb-1.6.9/tests/test_RerankingEvaluator.py
+-rw-r--r--   0 root         (0) root         (0)     1113 2024-04-15 20:34:26.000000 mteb-1.6.9/tests/test_RetrievalEvaluator.py
+-rw-r--r--   0 root         (0) root         (0)     3715 2024-04-15 20:34:26.000000 mteb-1.6.9/tests/test_TaskMetadata.py
+-rw-r--r--   0 root         (0) root         (0)     2269 2024-04-15 20:34:26.000000 mteb-1.6.9/tests/test_all_abstasks.py
+-rw-r--r--   0 root         (0) root         (0)     1420 2024-04-15 20:34:26.000000 mteb-1.6.9/tests/test_mteb.py
```

### Comparing `mteb-1.6.8/LICENSE` & `mteb-1.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/PKG-INFO` & `mteb-1.6.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mteb
-Version: 1.6.8
+Version: 1.6.9
 Summary: Massive Text Embedding Benchmark
 Author-email: MTEB Contributors <niklas@huggingface.co>, nouamane@huggingface.co, info@nils-reimers.de
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `mteb-1.6.8/README.md` & `mteb-1.6.9/README.md`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/__init__.py` & `mteb-1.6.9/mteb/__init__.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/abstasks/AbsTask.py` & `mteb-1.6.9/mteb/abstasks/AbsTask.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/abstasks/AbsTaskBitextMining.py` & `mteb-1.6.9/mteb/abstasks/AbsTaskBitextMining.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/abstasks/AbsTaskClassification.py` & `mteb-1.6.9/mteb/abstasks/AbsTaskClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/abstasks/AbsTaskClustering.py` & `mteb-1.6.9/mteb/abstasks/AbsTaskClustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/abstasks/AbsTaskPairClassification.py` & `mteb-1.6.9/mteb/abstasks/AbsTaskPairClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/abstasks/AbsTaskReranking.py` & `mteb-1.6.9/mteb/abstasks/AbsTaskReranking.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/abstasks/AbsTaskRetrieval.py` & `mteb-1.6.9/mteb/abstasks/AbsTaskRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/abstasks/AbsTaskSTS.py` & `mteb-1.6.9/mteb/abstasks/AbsTaskSTS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/abstasks/AbsTaskSummarization.py` & `mteb-1.6.9/mteb/abstasks/AbsTaskSummarization.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/abstasks/CrosslingualTask.py` & `mteb-1.6.9/mteb/abstasks/CrosslingualTask.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/abstasks/LangMapping.py` & `mteb-1.6.9/mteb/abstasks/LangMapping.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/abstasks/MultilingualTask.py` & `mteb-1.6.9/mteb/abstasks/MultilingualTask.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/abstasks/TaskMetadata.py` & `mteb-1.6.9/mteb/abstasks/TaskMetadata.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/abstasks/iso_15924_to_script.json` & `mteb-1.6.9/mteb/abstasks/iso_15924_to_script.json`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/abstasks/iso_639_3_to_language.json` & `mteb-1.6.9/mteb/abstasks/iso_639_3_to_language.json`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/abstasks/languages.py` & `mteb-1.6.9/mteb/abstasks/languages.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/cmd.py` & `mteb-1.6.9/mteb/cmd.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/evaluation/MTEB.py` & `mteb-1.6.9/mteb/evaluation/MTEB.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/evaluation/evaluators/BitextMiningEvaluator.py` & `mteb-1.6.9/mteb/evaluation/evaluators/BitextMiningEvaluator.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/evaluation/evaluators/ClassificationEvaluator.py` & `mteb-1.6.9/mteb/evaluation/evaluators/ClassificationEvaluator.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/evaluation/evaluators/ClusteringEvaluator.py` & `mteb-1.6.9/mteb/evaluation/evaluators/ClusteringEvaluator.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/evaluation/evaluators/Evaluator.py` & `mteb-1.6.9/mteb/evaluation/evaluators/Evaluator.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/evaluation/evaluators/PairClassificationEvaluator.py` & `mteb-1.6.9/mteb/evaluation/evaluators/PairClassificationEvaluator.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/evaluation/evaluators/RerankingEvaluator.py` & `mteb-1.6.9/mteb/evaluation/evaluators/RerankingEvaluator.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/evaluation/evaluators/RetrievalEvaluator.py` & `mteb-1.6.9/mteb/evaluation/evaluators/RetrievalEvaluator.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/evaluation/evaluators/STSEvaluator.py` & `mteb-1.6.9/mteb/evaluation/evaluators/STSEvaluator.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/evaluation/evaluators/SummarizationEvaluator.py` & `mteb-1.6.9/mteb/evaluation/evaluators/SummarizationEvaluator.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/evaluation/evaluators/utils.py` & `mteb-1.6.9/mteb/evaluation/evaluators/utils.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/logging.py` & `mteb-1.6.9/mteb/logging.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/BitextMining/dan/BornholmskBitextMining.py` & `mteb-1.6.9/mteb/tasks/BitextMining/dan/BornholmskBitextMining.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/BitextMining/multilingual/BUCCBitextMining.py` & `mteb-1.6.9/mteb/tasks/BitextMining/multilingual/BUCCBitextMining.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/BitextMining/multilingual/DiaBLaBitextMining.py` & `mteb-1.6.9/mteb/tasks/BitextMining/multilingual/DiaBLaBitextMining.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/BitextMining/multilingual/FloresBitextMining.py` & `mteb-1.6.9/mteb/tasks/BitextMining/multilingual/FloresBitextMining.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/BitextMining/multilingual/NorwegianCourtsBitextMining.py` & `mteb-1.6.9/mteb/tasks/BitextMining/multilingual/NorwegianCourtsBitextMining.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/BitextMining/multilingual/TatoebaBitextMining.py` & `mteb-1.6.9/mteb/tasks/BitextMining/multilingual/TatoebaBitextMining.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/BitextMining/multilingual/norwegian_courts_bitext_mining.py` & `mteb-1.6.9/mteb/tasks/BitextMining/multilingual/norwegian_courts_bitext_mining.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/BitextMining/vie/VieMedEVBitextMining.py` & `mteb-1.6.9/mteb/tasks/BitextMining/vie/VieMedEVBitextMining.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/Classification/__init__.py` & `mteb-1.6.9/mteb/tasks/Classification/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -25,7 +25,8 @@
 from .multilingual.ScalaClassification import *
 from .nob.NoRecClassification import *
 from .nob.NorwegianParliamentClassification import *
 from .pol.PolishClassification import *
 from .swe.SweRecClassification import *
 from .vie.VieStudentFeedbackClassification import *
 from .zho.CMTEBClassification import *
+from .zho.YueOpenriceReviewClassification import YueOpenriceReviewClassification  # noqa: F401
```

### Comparing `mteb-1.6.8/mteb/tasks/Classification/dan/AngryTweetsClassification.py` & `mteb-1.6.9/mteb/tasks/Classification/dan/AngryTweetsClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/Classification/dan/DKHateClassification.py` & `mteb-1.6.9/mteb/tasks/Classification/dan/DKHateClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/Classification/dan/DalajClassification.py` & `mteb-1.6.9/mteb/tasks/Classification/dan/DalajClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/Classification/dan/DanishPoliticalCommentsClassification.py` & `mteb-1.6.9/mteb/tasks/Classification/dan/DanishPoliticalCommentsClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/Classification/dan/DdiscoCohesionClassification.py` & `mteb-1.6.9/mteb/tasks/Classification/dan/DdiscoCohesionClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/Classification/dan/LccSentimentClassification.py` & `mteb-1.6.9/mteb/tasks/Classification/dan/LccSentimentClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/Classification/eng/AmazonPolarityClassification.py` & `mteb-1.6.9/mteb/tasks/Classification/eng/AmazonPolarityClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/Classification/eng/Banking77Classification.py` & `mteb-1.6.9/mteb/tasks/Classification/eng/Banking77Classification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/Classification/eng/EmotionClassification.py` & `mteb-1.6.9/mteb/tasks/Classification/eng/EmotionClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/Classification/eng/ImdbClassification.py` & `mteb-1.6.9/mteb/tasks/Classification/eng/ImdbClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/Classification/eng/NewsClassification.py` & `mteb-1.6.9/mteb/tasks/Classification/eng/NewsClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/Classification/eng/ToxicConversationsClassification.py` & `mteb-1.6.9/mteb/tasks/Classification/eng/ToxicConversationsClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/Classification/eng/TweetSentimentExtractionClassification.py` & `mteb-1.6.9/mteb/tasks/Classification/eng/TweetSentimentExtractionClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/Classification/hin/HindiDiscourseClassification.py` & `mteb-1.6.9/mteb/tasks/Classification/hin/HindiDiscourseClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/Classification/jpn/WRIMEClassification.py` & `mteb-1.6.9/mteb/tasks/Classification/jpn/WRIMEClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/Classification/multilingual/AmazonCounterfactualClassification.py` & `mteb-1.6.9/mteb/tasks/Classification/multilingual/AmazonCounterfactualClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/Classification/multilingual/AmazonReviewsClassification.py` & `mteb-1.6.9/mteb/tasks/Classification/multilingual/AmazonReviewsClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/Classification/multilingual/MTOPDomainClassification.py` & `mteb-1.6.9/mteb/tasks/Classification/multilingual/MTOPDomainClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/Classification/multilingual/MTOPIntentClassification.py` & `mteb-1.6.9/mteb/tasks/Classification/multilingual/MTOPIntentClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/Classification/multilingual/MasakhaNEWSClassification.py` & `mteb-1.6.9/mteb/tasks/Classification/multilingual/MasakhaNEWSClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/Classification/multilingual/MassiveIntentClassification.py` & `mteb-1.6.9/mteb/tasks/Classification/multilingual/MassiveIntentClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/Classification/multilingual/MassiveScenarioClassification.py` & `mteb-1.6.9/mteb/tasks/Classification/multilingual/MassiveScenarioClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/Classification/multilingual/NordicLangClassification.py` & `mteb-1.6.9/mteb/tasks/Classification/multilingual/NordicLangClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/Classification/multilingual/ScalaClassification.py` & `mteb-1.6.9/mteb/tasks/Classification/multilingual/ScalaClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/Classification/nob/NoRecClassification.py` & `mteb-1.6.9/mteb/tasks/Classification/nob/NoRecClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/Classification/nob/NorwegianParliamentClassification.py` & `mteb-1.6.9/mteb/tasks/Classification/nob/NorwegianParliamentClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/Classification/pol/PolishClassification.py` & `mteb-1.6.9/mteb/tasks/Classification/pol/PolishClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/Classification/swe/SweRecClassification.py` & `mteb-1.6.9/mteb/tasks/Classification/swe/SweRecClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/Classification/vie/VieStudentFeedbackClassification.py` & `mteb-1.6.9/mteb/tasks/Classification/vie/VieStudentFeedbackClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/Classification/zho/CMTEBClassification.py` & `mteb-1.6.9/mteb/tasks/Classification/zho/CMTEBClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/Clustering/__init__.py` & `mteb-1.6.9/mteb/tasks/Clustering/__init__.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/Clustering/deu/BlurbsClusteringP2P.py` & `mteb-1.6.9/mteb/tasks/Clustering/deu/BlurbsClusteringP2P.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/Clustering/deu/BlurbsClusteringS2S.py` & `mteb-1.6.9/mteb/tasks/Clustering/deu/BlurbsClusteringS2S.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/Clustering/deu/TenKGnadClusteringP2P.py` & `mteb-1.6.9/mteb/tasks/Clustering/deu/TenKGnadClusteringP2P.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/Clustering/deu/TenKGnadClusteringS2S.py` & `mteb-1.6.9/mteb/tasks/Clustering/deu/TenKGnadClusteringS2S.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/Clustering/eng/ArxivClusteringP2P.py` & `mteb-1.6.9/mteb/tasks/Clustering/eng/ArxivClusteringP2P.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/Clustering/eng/ArxivClusteringS2S.py` & `mteb-1.6.9/mteb/tasks/Clustering/eng/ArxivClusteringS2S.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/Clustering/eng/BigPatentClustering.py` & `mteb-1.6.9/mteb/tasks/Clustering/eng/BigPatentClustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/Clustering/eng/BiorxivClusteringP2P.py` & `mteb-1.6.9/mteb/tasks/Clustering/eng/BiorxivClusteringP2P.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/Clustering/eng/BiorxivClusteringS2S.py` & `mteb-1.6.9/mteb/tasks/Clustering/eng/BiorxivClusteringS2S.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/Clustering/eng/MedrxivClusteringP2P.py` & `mteb-1.6.9/mteb/tasks/Clustering/eng/MedrxivClusteringP2P.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/Clustering/eng/MedrxivClusteringS2S.py` & `mteb-1.6.9/mteb/tasks/Clustering/eng/MedrxivClusteringS2S.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/Clustering/eng/RedditClustering.py` & `mteb-1.6.9/mteb/tasks/Clustering/eng/RedditClustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/Clustering/eng/RedditClusteringP2P.py` & `mteb-1.6.9/mteb/tasks/Clustering/eng/RedditClusteringP2P.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/Clustering/eng/StackExchangeClustering.py` & `mteb-1.6.9/mteb/tasks/Clustering/eng/StackExchangeClustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/Clustering/eng/StackExchangeClusteringP2P.py` & `mteb-1.6.9/mteb/tasks/Clustering/eng/StackExchangeClusteringP2P.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/Clustering/eng/TwentyNewsgroupsClustering.py` & `mteb-1.6.9/mteb/tasks/Clustering/eng/TwentyNewsgroupsClustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/Clustering/eng/WikiCitiesClustering.py` & `mteb-1.6.9/mteb/tasks/Clustering/eng/WikiCitiesClustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/Clustering/fra/AlloProfClusteringP2P.py` & `mteb-1.6.9/mteb/tasks/Clustering/fra/AlloProfClusteringP2P.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/Clustering/fra/AlloProfClusteringS2S.py` & `mteb-1.6.9/mteb/tasks/Clustering/fra/AlloProfClusteringS2S.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/Clustering/fra/HALClusteringS2S.py` & `mteb-1.6.9/mteb/tasks/Clustering/fra/HALClusteringS2S.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/Clustering/fra/MLSUMClusteringP2P.py` & `mteb-1.6.9/mteb/tasks/Clustering/fra/MLSUMClusteringP2P.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/Clustering/fra/MLSUMClusteringS2S.py` & `mteb-1.6.9/mteb/tasks/Clustering/fra/MLSUMClusteringS2S.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/Clustering/multilingual/MasakhaNEWSClusteringP2P.py` & `mteb-1.6.9/mteb/tasks/Clustering/multilingual/MasakhaNEWSClusteringP2P.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/Clustering/multilingual/MasakhaNEWSClusteringS2S.py` & `mteb-1.6.9/mteb/tasks/Clustering/multilingual/MasakhaNEWSClusteringS2S.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/Clustering/nob/snl_clustering.py` & `mteb-1.6.9/mteb/tasks/Clustering/nob/snl_clustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/Clustering/nob/vg_clustering.py` & `mteb-1.6.9/mteb/tasks/Clustering/nob/vg_clustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/Clustering/pol/PolishClustering.py` & `mteb-1.6.9/mteb/tasks/Clustering/pol/PolishClustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/Clustering/spa/FloresClusteringS2S.py` & `mteb-1.6.9/mteb/tasks/Clustering/spa/FloresClusteringS2S.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/Clustering/spa/SpanishNewsClusteringP2P.py` & `mteb-1.6.9/mteb/tasks/Clustering/spa/SpanishNewsClusteringP2P.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/Clustering/swe/swedn_clustering.py` & `mteb-1.6.9/mteb/tasks/Clustering/swe/swedn_clustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/Clustering/zho/CMTEBClustering.py` & `mteb-1.6.9/mteb/tasks/Clustering/zho/CMTEBClustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/PairClassification/deu/FalseFriendsDeEnPC.py` & `mteb-1.6.9/mteb/tasks/PairClassification/deu/FalseFriendsDeEnPC.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/PairClassification/eng/SprintDuplicateQuestionsPC.py` & `mteb-1.6.9/mteb/tasks/PairClassification/eng/SprintDuplicateQuestionsPC.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/PairClassification/eng/TwitterSemEval2015PC.py` & `mteb-1.6.9/mteb/tasks/PairClassification/eng/TwitterSemEval2015PC.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/PairClassification/eng/TwitterURLCorpusPC.py` & `mteb-1.6.9/mteb/tasks/PairClassification/eng/TwitterURLCorpusPC.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/PairClassification/multilingual/OpusparcusPC.py` & `mteb-1.6.9/mteb/tasks/PairClassification/multilingual/OpusparcusPC.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/PairClassification/multilingual/PawsX.py` & `mteb-1.6.9/mteb/tasks/PairClassification/multilingual/PawsX.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/PairClassification/pol/PolishPC.py` & `mteb-1.6.9/mteb/tasks/PairClassification/pol/PolishPC.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/PairClassification/zho/CMTEBPairClassification.py` & `mteb-1.6.9/mteb/tasks/PairClassification/zho/CMTEBPairClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/Reranking/eng/AskUbuntuDupQuestions.py` & `mteb-1.6.9/mteb/tasks/Reranking/eng/AskUbuntuDupQuestions.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/Reranking/eng/MindSmallReranking.py` & `mteb-1.6.9/mteb/tasks/Reranking/eng/MindSmallReranking.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/Reranking/eng/SciDocsReranking.py` & `mteb-1.6.9/mteb/tasks/Reranking/eng/SciDocsReranking.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/Reranking/eng/StackOverflowDupQuestions.py` & `mteb-1.6.9/mteb/tasks/Reranking/eng/StackOverflowDupQuestions.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/Reranking/fra/AlloprofReranking.py` & `mteb-1.6.9/mteb/tasks/Reranking/fra/AlloprofReranking.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/Reranking/fra/SyntecReranking.py` & `mteb-1.6.9/mteb/tasks/Reranking/fra/SyntecReranking.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/Reranking/multilingual/MIRACLReranking.py` & `mteb-1.6.9/mteb/tasks/Reranking/multilingual/MIRACLReranking.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/Reranking/zho/CMTEBReranking.py` & `mteb-1.6.9/mteb/tasks/Reranking/zho/CMTEBReranking.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/Retrieval/__init__.py` & `mteb-1.6.9/mteb/tasks/Retrieval/__init__.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/Retrieval/code/CodeSearchNetRetrieval.py` & `mteb-1.6.9/mteb/tasks/Retrieval/code/CodeSearchNetRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/Retrieval/dan/dan_fever.py` & `mteb-1.6.9/mteb/tasks/Retrieval/dan/dan_fever.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/Retrieval/dan/t2nord_retrieval.py` & `mteb-1.6.9/mteb/tasks/Retrieval/dan/t2nord_retrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/Retrieval/dan/twitterhjerne.py` & `mteb-1.6.9/mteb/tasks/Retrieval/dan/twitterhjerne.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/Retrieval/deu/GerDaLIRRetrieval.py` & `mteb-1.6.9/mteb/tasks/Retrieval/deu/GerDaLIRRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/Retrieval/deu/GerDaLIRSmallRetrieval.py` & `mteb-1.6.9/mteb/tasks/Retrieval/deu/GerDaLIRSmallRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/Retrieval/deu/GermanDPRRetrieval.py` & `mteb-1.6.9/mteb/tasks/Retrieval/deu/GermanDPRRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/Retrieval/deu/GermanQuADRetrieval.py` & `mteb-1.6.9/mteb/tasks/Retrieval/deu/GermanQuADRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/Retrieval/deu/LegalQuADRetrieval.py` & `mteb-1.6.9/mteb/tasks/Retrieval/deu/LegalQuADRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/Retrieval/eng/AILACasedocsRetrieval.py` & `mteb-1.6.9/mteb/tasks/Retrieval/eng/AILACasedocsRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/Retrieval/eng/AILAStatutesRetrieval.py` & `mteb-1.6.9/mteb/tasks/Retrieval/eng/AILAStatutesRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/Retrieval/eng/ArguAnaRetrieval.py` & `mteb-1.6.9/mteb/tasks/Retrieval/eng/ArguAnaRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/Retrieval/eng/CQADupstackAndroidRetrieval.py` & `mteb-1.6.9/mteb/tasks/Retrieval/eng/CQADupstackAndroidRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/Retrieval/eng/CQADupstackEnglishRetrieval.py` & `mteb-1.6.9/mteb/tasks/Retrieval/eng/CQADupstackEnglishRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/Retrieval/eng/CQADupstackGamingRetrieval.py` & `mteb-1.6.9/mteb/tasks/Retrieval/eng/CQADupstackGamingRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/Retrieval/eng/CQADupstackGisRetrieval.py` & `mteb-1.6.9/mteb/tasks/Retrieval/eng/CQADupstackGisRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/Retrieval/eng/CQADupstackMathematicaRetrieval.py` & `mteb-1.6.9/mteb/tasks/Retrieval/eng/CQADupstackMathematicaRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/Retrieval/eng/CQADupstackPhysicsRetrieval.py` & `mteb-1.6.9/mteb/tasks/Retrieval/eng/CQADupstackPhysicsRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/Retrieval/eng/CQADupstackProgrammersRetrieval.py` & `mteb-1.6.9/mteb/tasks/Retrieval/eng/CQADupstackProgrammersRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/Retrieval/eng/CQADupstackStatsRetrieval.py` & `mteb-1.6.9/mteb/tasks/Retrieval/eng/CQADupstackStatsRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/Retrieval/eng/CQADupstackTexRetrieval.py` & `mteb-1.6.9/mteb/tasks/Retrieval/eng/CQADupstackTexRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/Retrieval/eng/CQADupstackUnixRetrieval.py` & `mteb-1.6.9/mteb/tasks/Retrieval/eng/CQADupstackUnixRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/Retrieval/eng/CQADupstackWebmastersRetrieval.py` & `mteb-1.6.9/mteb/tasks/Retrieval/eng/CQADupstackWebmastersRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/Retrieval/eng/CQADupstackWordpressRetrieval.py` & `mteb-1.6.9/mteb/tasks/Retrieval/eng/CQADupstackWordpressRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/Retrieval/eng/ClimateFEVERRetrieval.py` & `mteb-1.6.9/mteb/tasks/Retrieval/eng/ClimateFEVERRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/Retrieval/eng/DBPediaRetrieval.py` & `mteb-1.6.9/mteb/tasks/Retrieval/eng/DBPediaRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/Retrieval/eng/FEVERRetrieval.py` & `mteb-1.6.9/mteb/tasks/Retrieval/eng/FEVERRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/Retrieval/eng/FiQA2018Retrieval.py` & `mteb-1.6.9/mteb/tasks/Retrieval/eng/FiQA2018Retrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/Retrieval/eng/HagridRetrieval.py` & `mteb-1.6.9/mteb/tasks/Retrieval/eng/HagridRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/Retrieval/eng/HotpotQARetrieval.py` & `mteb-1.6.9/mteb/tasks/Retrieval/eng/HotpotQARetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/Retrieval/eng/LegalBenchConsumerContractsQARetrieval.py` & `mteb-1.6.9/mteb/tasks/Retrieval/eng/LegalBenchConsumerContractsQARetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/Retrieval/eng/LegalBenchCorporateLobbyingRetrieval.py` & `mteb-1.6.9/mteb/tasks/Retrieval/eng/LegalBenchCorporateLobbyingRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/Retrieval/eng/LegalSummarizationRetrieval.py` & `mteb-1.6.9/mteb/tasks/Retrieval/eng/LegalSummarizationRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/Retrieval/eng/MSMARCORetrieval.py` & `mteb-1.6.9/mteb/tasks/Retrieval/eng/MSMARCORetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/Retrieval/eng/MSMARCOv2Retrieval.py` & `mteb-1.6.9/mteb/tasks/Retrieval/eng/MSMARCOv2Retrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/Retrieval/eng/MedicalQARetrieval.py` & `mteb-1.6.9/mteb/tasks/Retrieval/eng/MedicalQARetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/Retrieval/eng/NFCorpusRetrieval.py` & `mteb-1.6.9/mteb/tasks/Retrieval/eng/NFCorpusRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/Retrieval/eng/NQRetrieval.py` & `mteb-1.6.9/mteb/tasks/Retrieval/eng/NQRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/Retrieval/eng/NarrativeQARetrieval.py` & `mteb-1.6.9/mteb/tasks/Retrieval/eng/NarrativeQARetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/Retrieval/eng/QuoraRetrieval.py` & `mteb-1.6.9/mteb/tasks/Retrieval/eng/QuoraRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/Retrieval/eng/SCIDOCSRetrieval.py` & `mteb-1.6.9/mteb/tasks/Retrieval/eng/SCIDOCSRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/Retrieval/eng/SciFactRetrieval.py` & `mteb-1.6.9/mteb/tasks/Retrieval/eng/SciFactRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/Retrieval/eng/TRECCOVIDRetrieval.py` & `mteb-1.6.9/mteb/tasks/Retrieval/eng/TRECCOVIDRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/Retrieval/eng/Touche2020Retrieval.py` & `mteb-1.6.9/mteb/tasks/Retrieval/eng/Touche2020Retrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/Retrieval/fra/AlloprofRetrieval.py` & `mteb-1.6.9/mteb/tasks/Retrieval/fra/AlloprofRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/Retrieval/fra/BSARDRetrieval.py` & `mteb-1.6.9/mteb/tasks/Retrieval/fra/BSARDRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/Retrieval/fra/SyntecRetrieval.py` & `mteb-1.6.9/mteb/tasks/Retrieval/fra/SyntecRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/Retrieval/jpn/JaQuADRetrieval.py` & `mteb-1.6.9/mteb/tasks/Retrieval/jpn/JaQuADRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/Retrieval/kor/KoMiracl.py` & `mteb-1.6.9/mteb/tasks/Retrieval/kor/KoMiracl.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/Retrieval/kor/KoStrategyQA.py` & `mteb-1.6.9/mteb/tasks/Retrieval/kor/KoStrategyQA.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/Retrieval/multilingual/MIRACLRetrieval.py` & `mteb-1.6.9/mteb/tasks/Retrieval/multilingual/MIRACLRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/Retrieval/multilingual/MintakaRetrieval.py` & `mteb-1.6.9/mteb/tasks/Retrieval/multilingual/MintakaRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/Retrieval/multilingual/MultiLongDocRetrieval.py` & `mteb-1.6.9/mteb/tasks/Retrieval/multilingual/MultiLongDocRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/Retrieval/multilingual/XMarketRetrieval.py` & `mteb-1.6.9/mteb/tasks/Retrieval/multilingual/XMarketRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/Retrieval/multilingual/XPQARetrieval.py` & `mteb-1.6.9/mteb/tasks/Retrieval/multilingual/XPQARetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/Retrieval/nob/norquad.py` & `mteb-1.6.9/mteb/tasks/Retrieval/nob/norquad.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/Retrieval/nob/snl_retrieval.py` & `mteb-1.6.9/mteb/tasks/Retrieval/nob/snl_retrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/Retrieval/pol/ArguAnaPLRetrieval.py` & `mteb-1.6.9/mteb/tasks/Retrieval/pol/ArguAnaPLRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/Retrieval/pol/DBPediaPLRetrieval.py` & `mteb-1.6.9/mteb/tasks/Retrieval/pol/DBPediaPLRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/Retrieval/pol/FiQAPLRetrieval.py` & `mteb-1.6.9/mteb/tasks/Retrieval/pol/FiQAPLRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/Retrieval/pol/HotpotQAPLRetrieval.py` & `mteb-1.6.9/mteb/tasks/Retrieval/pol/HotpotQAPLRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/Retrieval/pol/MSMARCOPLRetrieval.py` & `mteb-1.6.9/mteb/tasks/Retrieval/pol/MSMARCOPLRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/Retrieval/pol/NFCorpusPLRetrieval.py` & `mteb-1.6.9/mteb/tasks/Retrieval/pol/NFCorpusPLRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/Retrieval/pol/NQPLRetrieval.py` & `mteb-1.6.9/mteb/tasks/Retrieval/pol/NQPLRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/Retrieval/pol/QuoraPLRetrieval.py` & `mteb-1.6.9/mteb/tasks/Retrieval/pol/QuoraPLRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/Retrieval/pol/SCIDOCSPLRetrieval.py` & `mteb-1.6.9/mteb/tasks/Retrieval/pol/SCIDOCSPLRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/Retrieval/pol/SciFactPLRetrieval.py` & `mteb-1.6.9/mteb/tasks/Retrieval/pol/SciFactPLRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/Retrieval/pol/TRECCOVIDPLRetrieval.py` & `mteb-1.6.9/mteb/tasks/Retrieval/pol/TRECCOVIDPLRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/Retrieval/spa/SpanishPassageRetrievalS2P.py` & `mteb-1.6.9/mteb/tasks/Retrieval/spa/SpanishPassageRetrievalS2P.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/Retrieval/spa/SpanishPassageRetrievalS2S.py` & `mteb-1.6.9/mteb/tasks/Retrieval/spa/SpanishPassageRetrievalS2S.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/Retrieval/swe/swedn_retrieval.py` & `mteb-1.6.9/mteb/tasks/Retrieval/swe/swedn_retrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/Retrieval/swe/swefaq_retrieval.py` & `mteb-1.6.9/mteb/tasks/Retrieval/swe/swefaq_retrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/Retrieval/vie/VieQuADRetrieval.py` & `mteb-1.6.9/mteb/tasks/Retrieval/vie/VieQuADRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/Retrieval/zho/CMTEBRetrieval.py` & `mteb-1.6.9/mteb/tasks/Retrieval/zho/CMTEBRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/Retrieval/zho/LeCaRDv2Retrieval.py` & `mteb-1.6.9/mteb/tasks/Retrieval/zho/LeCaRDv2Retrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/STS/__init__.py` & `mteb-1.6.9/mteb/tasks/STS/__init__.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/STS/deu/GermanSTSBenchmarkSTS.py` & `mteb-1.6.9/mteb/tasks/STS/deu/GermanSTSBenchmarkSTS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/STS/eng/BiossesSTS.py` & `mteb-1.6.9/mteb/tasks/STS/eng/BiossesSTS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/STS/eng/STS12STS.py` & `mteb-1.6.9/mteb/tasks/STS/eng/STS12STS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/STS/eng/STS13STS.py` & `mteb-1.6.9/mteb/tasks/STS/eng/STS13STS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/STS/eng/STS14STS.py` & `mteb-1.6.9/mteb/tasks/STS/eng/STS14STS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/STS/eng/STS15STS.py` & `mteb-1.6.9/mteb/tasks/STS/eng/STS15STS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/STS/eng/STS16STS.py` & `mteb-1.6.9/mteb/tasks/STS/eng/STS16STS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/STS/eng/STSBenchmarkSTS.py` & `mteb-1.6.9/mteb/tasks/STS/eng/STSBenchmarkSTS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/STS/eng/SickrSTS.py` & `mteb-1.6.9/mteb/tasks/STS/eng/SickrSTS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/STS/fra/SickFrSTS.py` & `mteb-1.6.9/mteb/tasks/STS/fra/SickFrSTS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/STS/multilingual/STS17CrosslingualSTS.py` & `mteb-1.6.9/mteb/tasks/STS/multilingual/STS17CrosslingualSTS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/STS/multilingual/STS22CrosslingualSTS.py` & `mteb-1.6.9/mteb/tasks/STS/multilingual/STS22CrosslingualSTS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/STS/multilingual/STSBenchmarkMultilingualSTS.py` & `mteb-1.6.9/mteb/tasks/STS/multilingual/STSBenchmarkMultilingualSTS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/STS/pol/PolishSTS.py` & `mteb-1.6.9/mteb/tasks/STS/pol/PolishSTS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/STS/spa/STSES.py` & `mteb-1.6.9/mteb/tasks/STS/spa/STSES.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/STS/zho/CMTEBSTS.py` & `mteb-1.6.9/mteb/tasks/STS/zho/CMTEBSTS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/Summarization/eng/SummEvalSummarization.py` & `mteb-1.6.9/mteb/tasks/Summarization/eng/SummEvalSummarization.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb/tasks/Summarization/fra/SummEvalFrSummarization.py` & `mteb-1.6.9/mteb/tasks/Summarization/fra/SummEvalFrSummarization.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/mteb.egg-info/PKG-INFO` & `mteb-1.6.9/mteb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mteb
-Version: 1.6.8
+Version: 1.6.9
 Summary: Massive Text Embedding Benchmark
 Author-email: MTEB Contributors <niklas@huggingface.co>, nouamane@huggingface.co, info@nils-reimers.de
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `mteb-1.6.8/mteb.egg-info/SOURCES.txt` & `mteb-1.6.9/mteb.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -88,14 +88,15 @@
 mteb/tasks/Classification/pol/PolishClassification.py
 mteb/tasks/Classification/pol/__init__.py
 mteb/tasks/Classification/swe/SweRecClassification.py
 mteb/tasks/Classification/swe/__init__.py
 mteb/tasks/Classification/vie/VieStudentFeedbackClassification.py
 mteb/tasks/Classification/vie/__init__.py
 mteb/tasks/Classification/zho/CMTEBClassification.py
+mteb/tasks/Classification/zho/YueOpenriceReviewClassification.py
 mteb/tasks/Classification/zho/__init__.py
 mteb/tasks/Clustering/__init__.py
 mteb/tasks/Clustering/deu/BlurbsClusteringP2P.py
 mteb/tasks/Clustering/deu/BlurbsClusteringS2S.py
 mteb/tasks/Clustering/deu/TenKGnadClusteringP2P.py
 mteb/tasks/Clustering/deu/TenKGnadClusteringS2S.py
 mteb/tasks/Clustering/deu/__init__.py
@@ -294,14 +295,15 @@
 results/intfloat__multilingual-e5-small/TV2Nordretrieval.json
 results/intfloat__multilingual-e5-small/TwitterHjerneRetrieval.json
 results/intfloat__multilingual-e5-small/VGClustering.json
 results/intfloat__multilingual-e5-small/VieMedEVBitextMining.json
 results/intfloat__multilingual-e5-small/VieQuADRetrieval.json
 results/intfloat__multilingual-e5-small/VieStudentFeedbackClassification.json
 results/intfloat__multilingual-e5-small/WRIMEClassification.json
+results/intfloat__multilingual-e5-small/YueOpenriceReviewClassification.json
 results/intfloat__multilingual-e5-small/model_meta.json
 results/sentence-transformers__all-MiniLM-L6-v2/Banking77Classification.json
 results/sentence-transformers__all-MiniLM-L6-v2/BornholmBitextMining.json
 results/sentence-transformers__all-MiniLM-L6-v2/DanFEVER.json
 results/sentence-transformers__all-MiniLM-L6-v2/NorQuadRetrieval.json
 results/sentence-transformers__all-MiniLM-L6-v2/NorwegianCourtsBitextMining.json
 results/sentence-transformers__all-MiniLM-L6-v2/SNLClustering.json
@@ -337,14 +339,15 @@
 results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/TwitterHjerneRetrieval.json
 results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/VGClustering.json
 results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/VieMedEVBitextMining.json
 results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/VieQuADRetrieval.json
 results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/VieStudentFeedbackClassification.json
 results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/WRIMEClassification.json
 results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/WikiCitiesClustering.json
+results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/YueOpenriceReviewClassification.json
 results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/model_meta.json
 scripts/merge_cqadupstack.py
 scripts/mteb_meta.py
 scripts/run_mteb_chinese.py
 scripts/run_mteb_english.py
 scripts/run_mteb_french.py
 scripts/run_mteb_german.py
```

### Comparing `mteb-1.6.8/pyproject.toml` & `mteb-1.6.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=42", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mteb"
-version = "1.6.8"
+version = "1.6.9"
 description = "Massive Text Embedding Benchmark"
 readme = "README.md"
 authors = [
     { name = "MTEB Contributors", email = "niklas@huggingface.co" },
     { email = "nouamane@huggingface.co" },
     { email = "info@nils-reimers.de" },
 ]
```

### Comparing `mteb-1.6.8/results/intfloat__multilingual-e5-small/CodeSearchNetRetrieval.json` & `mteb-1.6.9/results/intfloat__multilingual-e5-small/CodeSearchNetRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/results/intfloat__multilingual-e5-small/DanFEVER.json` & `mteb-1.6.9/results/intfloat__multilingual-e5-small/DanFEVER.json`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/results/intfloat__multilingual-e5-small/JaQuADRetrieval.json` & `mteb-1.6.9/results/intfloat__multilingual-e5-small/JaQuADRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/results/intfloat__multilingual-e5-small/MedicalQARetrieval.json` & `mteb-1.6.9/results/intfloat__multilingual-e5-small/MedicalQARetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/results/intfloat__multilingual-e5-small/NorQuadRetrieval.json` & `mteb-1.6.9/results/intfloat__multilingual-e5-small/NorQuadRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/results/intfloat__multilingual-e5-small/SNLRetrieval.json` & `mteb-1.6.9/results/intfloat__multilingual-e5-small/SNLRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/results/intfloat__multilingual-e5-small/SweFaqRetrieval.json` & `mteb-1.6.9/results/intfloat__multilingual-e5-small/SweFaqRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/results/intfloat__multilingual-e5-small/SwednRetrieval.json` & `mteb-1.6.9/results/intfloat__multilingual-e5-small/SwednRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/results/intfloat__multilingual-e5-small/TV2Nordretrieval.json` & `mteb-1.6.9/results/intfloat__multilingual-e5-small/TV2Nordretrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/results/intfloat__multilingual-e5-small/TwitterHjerneRetrieval.json` & `mteb-1.6.9/results/intfloat__multilingual-e5-small/TwitterHjerneRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/results/intfloat__multilingual-e5-small/VieQuADRetrieval.json` & `mteb-1.6.9/results/intfloat__multilingual-e5-small/VieQuADRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/results/sentence-transformers__all-MiniLM-L6-v2/DanFEVER.json` & `mteb-1.6.9/results/sentence-transformers__all-MiniLM-L6-v2/DanFEVER.json`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/results/sentence-transformers__all-MiniLM-L6-v2/NorQuadRetrieval.json` & `mteb-1.6.9/results/sentence-transformers__all-MiniLM-L6-v2/NorQuadRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/results/sentence-transformers__all-MiniLM-L6-v2/SNLRetrieval.json` & `mteb-1.6.9/results/sentence-transformers__all-MiniLM-L6-v2/SNLRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/results/sentence-transformers__all-MiniLM-L6-v2/SweFaqRetrieval.json` & `mteb-1.6.9/results/sentence-transformers__all-MiniLM-L6-v2/SweFaqRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/results/sentence-transformers__all-MiniLM-L6-v2/SwednRetrieval.json` & `mteb-1.6.9/results/sentence-transformers__all-MiniLM-L6-v2/SwednRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/results/sentence-transformers__all-MiniLM-L6-v2/TV2Nordretrieval.json` & `mteb-1.6.9/results/sentence-transformers__all-MiniLM-L6-v2/TV2Nordretrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/results/sentence-transformers__all-MiniLM-L6-v2/TwitterHjerneRetrieval.json` & `mteb-1.6.9/results/sentence-transformers__all-MiniLM-L6-v2/TwitterHjerneRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/BUCC.json` & `mteb-1.6.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/BUCC.json`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CodeSearchNetRetrieval.json` & `mteb-1.6.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CodeSearchNetRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/DanFEVER.json` & `mteb-1.6.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/DanFEVER.json`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/DiaBlaBitextMining.json` & `mteb-1.6.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/DiaBlaBitextMining.json`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/GerDaLIR.json` & `mteb-1.6.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/GerDaLIR.json`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/JaQuADRetrieval.json` & `mteb-1.6.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/JaQuADRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/MedicalQARetrieval.json` & `mteb-1.6.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/MedicalQARetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/NorQuadRetrieval.json` & `mteb-1.6.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/NorQuadRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/OpusparcusPC.json` & `mteb-1.6.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/OpusparcusPC.json`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/PawsX.json` & `mteb-1.6.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/PawsX.json`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SNLRetrieval.json` & `mteb-1.6.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SNLRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SweFaqRetrieval.json` & `mteb-1.6.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SweFaqRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SwednRetrieval.json` & `mteb-1.6.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SwednRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/TV2Nordretrieval.json` & `mteb-1.6.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/TV2Nordretrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/TwitterHjerneRetrieval.json` & `mteb-1.6.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/TwitterHjerneRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/VieQuADRetrieval.json` & `mteb-1.6.9/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/VieQuADRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/scripts/data/amazon_polarity/create_data.py` & `mteb-1.6.9/scripts/data/amazon_polarity/create_data.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/scripts/data/amazon_reviews_multi/create_data.py` & `mteb-1.6.9/scripts/data/amazon_reviews_multi/create_data.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/scripts/data/arxiv/script_clustering.py` & `mteb-1.6.9/scripts/data/arxiv/script_clustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/scripts/data/arxiv/script_raw.py` & `mteb-1.6.9/scripts/data/arxiv/script_raw.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/scripts/data/biorxiv/script_clustering.py` & `mteb-1.6.9/scripts/data/biorxiv/script_clustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/scripts/data/biorxiv/script_raw.py` & `mteb-1.6.9/scripts/data/biorxiv/script_raw.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/scripts/data/bucc/create_data.py` & `mteb-1.6.9/scripts/data/bucc/create_data.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/scripts/data/create_task_table.py` & `mteb-1.6.9/scripts/data/create_task_table.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/scripts/data/germanquad/process_data.py` & `mteb-1.6.9/scripts/data/germanquad/process_data.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/scripts/data/hal/create_data.py` & `mteb-1.6.9/scripts/data/hal/create_data.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/scripts/data/imdb/create_data.py` & `mteb-1.6.9/scripts/data/imdb/create_data.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/scripts/data/medicalqaretrieval/create_data.py` & `mteb-1.6.9/scripts/data/medicalqaretrieval/create_data.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/scripts/data/medrxiv/script_clustering.py` & `mteb-1.6.9/scripts/data/medrxiv/script_clustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/scripts/data/medrxiv/script_raw.py` & `mteb-1.6.9/scripts/data/medrxiv/script_raw.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/scripts/data/mind/prepare_data.py` & `mteb-1.6.9/scripts/data/mind/prepare_data.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/scripts/data/redditp2p/script_clustering.py` & `mteb-1.6.9/scripts/data/redditp2p/script_clustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/scripts/data/stackexchangep2p/script_clustering.py` & `mteb-1.6.9/scripts/data/stackexchangep2p/script_clustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/scripts/data/sts22-crosslingual-sts/create_data.py` & `mteb-1.6.9/scripts/data/sts22-crosslingual-sts/create_data.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/scripts/data/summeval_fr/create_data.py` & `mteb-1.6.9/scripts/data/summeval_fr/create_data.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/scripts/data/toxic_conversations_50k/create_data.py` & `mteb-1.6.9/scripts/data/toxic_conversations_50k/create_data.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/scripts/merge_cqadupstack.py` & `mteb-1.6.9/scripts/merge_cqadupstack.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/scripts/mteb_meta.py` & `mteb-1.6.9/scripts/mteb_meta.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/scripts/run_mteb_chinese.py` & `mteb-1.6.9/scripts/run_mteb_chinese.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/scripts/run_mteb_english.py` & `mteb-1.6.9/scripts/run_mteb_english.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/scripts/run_mteb_french.py` & `mteb-1.6.9/scripts/run_mteb_french.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/scripts/run_mteb_german.py` & `mteb-1.6.9/scripts/run_mteb_german.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/scripts/run_mteb_korean.py` & `mteb-1.6.9/scripts/run_mteb_korean.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/scripts/run_mteb_law.py` & `mteb-1.6.9/scripts/run_mteb_law.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/scripts/run_mteb_polish.py` & `mteb-1.6.9/scripts/run_mteb_polish.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/tests/test_ClusteringEvaluator.py` & `mteb-1.6.9/tests/test_ClusteringEvaluator.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/tests/test_PairClassificationEvaluator.py` & `mteb-1.6.9/tests/test_PairClassificationEvaluator.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/tests/test_RerankingEvaluator.py` & `mteb-1.6.9/tests/test_RerankingEvaluator.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/tests/test_RetrievalEvaluator.py` & `mteb-1.6.9/tests/test_RetrievalEvaluator.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/tests/test_TaskMetadata.py` & `mteb-1.6.9/tests/test_TaskMetadata.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/tests/test_all_abstasks.py` & `mteb-1.6.9/tests/test_all_abstasks.py`

 * *Files identical despite different names*

### Comparing `mteb-1.6.8/tests/test_mteb.py` & `mteb-1.6.9/tests/test_mteb.py`

 * *Files identical despite different names*

