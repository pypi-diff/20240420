# Comparing `tmp/musicntwrk-2.2.9.tar.gz` & `tmp/musicntwrk-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/musicntwrk-2.2.9.tar", last modified: Mon Nov 22 17:40:00 2021, max compression
+gzip compressed data, was "musicntwrk-2.3.0.tar", last modified: Sat Apr 20 13:15:10 2024, max compression
```

## Comparing `musicntwrk-2.2.9.tar` & `musicntwrk-2.3.0.tar`

### file list

```diff
@@ -1,160 +1,184 @@
-drwxr-xr-x   0 marco      (502) staff       (20)        0 2021-11-22 17:40:00.494081 musicntwrk-2.2.9/
--rw-r--r--   0 marco      (502) staff       (20)     8042 2021-11-22 17:40:00.493583 musicntwrk-2.2.9/PKG-INFO
--rw-r--r--   0 marco      (502) staff       (20)     6875 2021-08-07 16:52:58.000000 musicntwrk-2.2.9/README.md
-drwxr-xr-x   0 marco      (502) staff       (20)        0 2021-11-22 17:40:00.398421 musicntwrk-2.2.9/musicntwrk.egg-info/
--rw-r--r--   0 marco      (502) staff       (20)     8042 2021-11-22 17:39:59.000000 musicntwrk-2.2.9/musicntwrk.egg-info/PKG-INFO
--rw-r--r--   0 marco      (502) staff       (20)     4149 2021-11-22 17:39:59.000000 musicntwrk-2.2.9/musicntwrk.egg-info/SOURCES.txt
--rw-r--r--   0 marco      (502) staff       (20)        1 2021-11-22 17:39:59.000000 musicntwrk-2.2.9/musicntwrk.egg-info/dependency_links.txt
--rw-r--r--   0 marco      (502) staff       (20)      159 2021-11-22 17:39:59.000000 musicntwrk-2.2.9/musicntwrk.egg-info/requires.txt
--rw-r--r--   0 marco      (502) staff       (20)       11 2021-11-22 17:39:59.000000 musicntwrk-2.2.9/musicntwrk.egg-info/top_level.txt
--rw-r--r--   0 marco      (502) staff       (20)       38 2021-11-22 17:40:00.494254 musicntwrk-2.2.9/setup.cfg
--rw-r--r--   0 marco      (502) staff       (20)     1398 2021-11-22 17:38:55.000000 musicntwrk-2.2.9/setup.py
-drwxr-xr-x   0 marco      (502) staff       (20)        0 2021-11-22 17:40:00.399381 musicntwrk-2.2.9/src/
--rw-r--r--   0 marco      (502) staff       (20)        0 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/__init__.py
-drwxr-xr-x   0 marco      (502) staff       (20)        0 2021-11-22 17:40:00.402073 musicntwrk-2.2.9/src/comptools/
--rw-r--r--   0 marco      (502) staff       (20)    39621 2021-05-31 23:27:25.000000 musicntwrk-2.2.9/src/comptools/MidiFile.py
--rw-r--r--   0 marco      (502) staff       (20)     2786 2021-09-23 16:53:48.000000 musicntwrk-2.2.9/src/comptools/genmidi.py
--rw-r--r--   0 marco      (502) staff       (20)     7760 2021-09-26 20:51:51.000000 musicntwrk-2.2.9/src/comptools/music.py
--rw-r--r--   0 marco      (502) staff       (20)     1888 2021-05-31 23:27:25.000000 musicntwrk-2.2.9/src/comptools/notation.py
-drwxr-xr-x   0 marco      (502) staff       (20)        0 2021-11-22 17:40:00.413246 musicntwrk-2.2.9/src/data/
--rw-r--r--   0 marco      (502) staff       (20)      828 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/data/MIDImap.py
--rw-r--r--   0 marco      (502) staff       (20)     2559 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/data/MIDImidi.py
--rw-r--r--   0 marco      (502) staff       (20)      915 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/data/MIDIscore.py
--rw-r--r--   0 marco      (502) staff       (20)     1275 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/data/WRITEscore.py
--rw-r--r--   0 marco      (502) staff       (20)     1013 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/data/WRITEscoreNoTime.py
--rw-r--r--   0 marco      (502) staff       (20)     1985 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/data/WRITEscoreOps.py
--rw-r--r--   0 marco      (502) staff       (20)     3272 2021-10-26 23:20:31.000000 musicntwrk-2.2.9/src/data/WRITEscoreOpsMIDI.py
--rw-r--r--   0 marco      (502) staff       (20)        0 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/data/__init__.py
--rw-r--r--   0 marco      (502) staff       (20)     2919 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/data/analyzeSound.py
--rw-r--r--   0 marco      (502) staff       (20)     3947 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/data/analyzeTimbre.py
--rw-r--r--   0 marco      (502) staff       (20)   114667 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/data/ctcsound.py
--rw-r--r--   0 marco      (502) staff       (20)     3993 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/data/i_spectral.py
--rw-r--r--   0 marco      (502) staff       (20)     3275 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/data/i_spectral2.py
--rw-r--r--   0 marco      (502) staff       (20)     1921 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/data/i_spectral_pure.py
--rw-r--r--   0 marco      (502) staff       (20)     2597 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/data/i_spectral_pyo.py
--rw-r--r--   0 marco      (502) staff       (20)     6358 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/data/i_time_series.py
--rw-r--r--   0 marco      (502) staff       (20)     1270 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/data/r_1Ddata.py
--rw-r--r--   0 marco      (502) staff       (20)    10624 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/data/scaleMapping.py
-drwxr-xr-x   0 marco      (502) staff       (20)        0 2021-11-22 17:40:00.428003 musicntwrk-2.2.9/src/harmony/
--rw-r--r--   0 marco      (502) staff       (20)       66 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/harmony/__init__.py
--rw-r--r--   0 marco      (502) staff       (20)     2035 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/harmony/applyOps.py
--rw-r--r--   0 marco      (502) staff       (20)     1256 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/harmony/changePoint.py
--rw-r--r--   0 marco      (502) staff       (20)     2640 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/harmony/chinese_postman.py
--rw-r--r--   0 marco      (502) staff       (20)     1703 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/harmony/enharmonicDictionary.py
--rw-r--r--   0 marco      (502) staff       (20)     1309 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/harmony/getRN.py
--rw-r--r--   0 marco      (502) staff       (20)     4084 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/harmony/harmonicDesign.py
--rw-r--r--   0 marco      (502) staff       (20)     2364 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/harmony/keySections.py
--rw-r--r--   0 marco      (502) staff       (20)     3022 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/harmony/lookupOps.py
--rw-r--r--   0 marco      (502) staff       (20)      884 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/harmony/lookupProgr.py
--rw-r--r--   0 marco      (502) staff       (20)     1265 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/harmony/lookupWrapper.py
--rw-r--r--   0 marco      (502) staff       (20)     2348 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/harmony/networkHarmonyGen.py
--rw-r--r--   0 marco      (502) staff       (20)     2769 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/harmony/plotHarmonicTable.py
--rw-r--r--   0 marco      (502) staff       (20)     2752 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/harmony/rhythmicDesign.py
--rw-r--r--   0 marco      (502) staff       (20)     4765 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/harmony/scoreAnalysis.py
--rw-r--r--   0 marco      (502) staff       (20)     1257 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/harmony/scoreDesign.py
--rw-r--r--   0 marco      (502) staff       (20)     2307 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/harmony/scoreFilter.py
--rw-r--r--   0 marco      (502) staff       (20)     2492 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/harmony/shortHands.py
--rw-r--r--   0 marco      (502) staff       (20)     2002 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/harmony/showAnalysis.py
--rw-r--r--   0 marco      (502) staff       (20)     4352 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/harmony/spiralChordSpace.py
--rw-r--r--   0 marco      (502) staff       (20)     2921 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/harmony/tonalAnalysis.py
--rw-r--r--   0 marco      (502) staff       (20)     7684 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/harmony/tonalHarmonyCalculator.py
--rw-r--r--   0 marco      (502) staff       (20)     4652 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/harmony/tonalHarmonyModels.py
--rw-r--r--   0 marco      (502) staff       (20)     1899 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/harmony/tonalPartition.py
--rw-r--r--   0 marco      (502) staff       (20)     2411 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/harmony/tonnentz.py
-drwxr-xr-x   0 marco      (502) staff       (20)        0 2021-11-22 17:40:00.433596 musicntwrk-2.2.9/src/ml_utils/
--rw-r--r--   0 marco      (502) staff       (20)       88 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/ml_utils/__init__.py
--rw-r--r--   0 marco      (502) staff       (20)     2690 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/ml_utils/checkRun.py
--rw-r--r--   0 marco      (502) staff       (20)     1401 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/ml_utils/modelDump.py
--rw-r--r--   0 marco      (502) staff       (20)     1473 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/ml_utils/modelLoad.py
--rw-r--r--   0 marco      (502) staff       (20)     1513 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/ml_utils/multiModelPredictor.py
--rw-r--r--   0 marco      (502) staff       (20)     1432 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/ml_utils/prepareDataSet.py
--rw-r--r--   0 marco      (502) staff       (20)     2014 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/ml_utils/readModels.py
--rw-r--r--   0 marco      (502) staff       (20)      814 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/ml_utils/scaleDataSet.py
--rw-r--r--   0 marco      (502) staff       (20)     3227 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/ml_utils/trainCNNmodel.py
--rw-r--r--   0 marco      (502) staff       (20)     2213 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/ml_utils/trainNNmodel.py
--rw-r--r--   0 marco      (502) staff       (20)    68768 2021-11-15 16:16:23.000000 musicntwrk-2.2.9/src/musicntwrk.py
-drwxr-xr-x   0 marco      (502) staff       (20)        0 2021-11-22 17:40:00.451282 musicntwrk-2.2.9/src/networks/
--rw-r--r--   0 marco      (502) staff       (20)        0 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/networks/__init__.py
--rw-r--r--   0 marco      (502) staff       (20)     2577 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/networks/orchestralNetwork.py
--rw-r--r--   0 marco      (502) staff       (20)     2375 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/networks/orchestralVector.py
--rw-r--r--   0 marco      (502) staff       (20)     1636 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/networks/orchestralVectorColor.py
--rw-r--r--   0 marco      (502) staff       (20)     4780 2021-11-11 23:43:00.000000 musicntwrk-2.2.9/src/networks/pcsDictionary.py
--rw-r--r--   0 marco      (502) staff       (20)     5760 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/networks/pcsEgoNetwork.py
--rw-r--r--   0 marco      (502) staff       (20)     4822 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/networks/pcsNetwork.py
--rw-r--r--   0 marco      (502) staff       (20)     2920 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/networks/rLeadNetwork.py
--rw-r--r--   0 marco      (502) staff       (20)     2470 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/networks/readScore.py
--rw-r--r--   0 marco      (502) staff       (20)     3321 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/networks/rhythmDictionary.py
--rw-r--r--   0 marco      (502) staff       (20)     4253 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/networks/rhythmNetwork.py
--rw-r--r--   0 marco      (502) staff       (20)     4186 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/networks/rhythmPDictionary.py
--rw-r--r--   0 marco      (502) staff       (20)     2456 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/networks/scoreDictionary.py
--rw-r--r--   0 marco      (502) staff       (20)     1592 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/networks/scoreMIDIDictionary.py
--rw-r--r--   0 marco      (502) staff       (20)     5142 2021-11-19 01:24:07.000000 musicntwrk-2.2.9/src/networks/scoreNetwork.py
--rw-r--r--   0 marco      (502) staff       (20)     5367 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/networks/scoreSubNetwork.py
--rw-r--r--   0 marco      (502) staff       (20)     3680 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/networks/timbralNetwork.py
--rw-r--r--   0 marco      (502) staff       (20)     4033 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/networks/vLeadNetwork.py
--rw-r--r--   0 marco      (502) staff       (20)     4553 2021-11-19 16:56:36.000000 musicntwrk-2.2.9/src/networks/vLeadNetworkByName.py
--rw-r--r--   0 marco      (502) staff       (20)     2890 2021-11-12 19:23:59.000000 musicntwrk-2.2.9/src/networks/vLeadNetworkByNameVec.py
--rw-r--r--   0 marco      (502) staff       (20)     2588 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/networks/vLeadNetworkVec.py
-drwxr-xr-x   0 marco      (502) staff       (20)        0 2021-11-22 17:40:00.458930 musicntwrk-2.2.9/src/plotting/
--rw-r--r--   0 marco      (502) staff       (20)     1061 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/plotting/barplot.py
--rw-r--r--   0 marco      (502) staff       (20)    25524 2021-10-28 22:26:22.000000 musicntwrk-2.2.9/src/plotting/chordspace.py
--rw-r--r--   0 marco      (502) staff       (20)     7250 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/plotting/drawMultiLayerNetwork.py
--rw-r--r--   0 marco      (502) staff       (20)     2811 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/plotting/drawNetwork.py
--rw-r--r--   0 marco      (502) staff       (20)     2222 2021-11-22 17:29:08.000000 musicntwrk-2.2.9/src/plotting/drawNetworkViz.py
--rw-r--r--   0 marco      (502) staff       (20)     1246 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/plotting/drawNetworkX.py
--rw-r--r--   0 marco      (502) staff       (20)      890 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/plotting/plotCC.py
--rw-r--r--   0 marco      (502) staff       (20)      716 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/plotting/plotCurveXY.py
--rw-r--r--   0 marco      (502) staff       (20)      711 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/plotting/plotCurveY.py
--rw-r--r--   0 marco      (502) staff       (20)     1864 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/plotting/plotOpsHistogram.py
-drwxr-xr-x   0 marco      (502) staff       (20)        0 2021-11-22 17:40:00.468108 musicntwrk-2.2.9/src/timbre/
--rw-r--r--   0 marco      (502) staff       (20)        0 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/timbre/__init__.py
--rw-r--r--   0 marco      (502) staff       (20)     1743 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/timbre/computeASCBW.py
--rw-r--r--   0 marco      (502) staff       (20)     1550 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/timbre/computeCompMPS.py
--rw-r--r--   0 marco      (502) staff       (20)     1661 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/timbre/computeMFCC.py
--rw-r--r--   0 marco      (502) staff       (20)     2646 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/timbre/computeModifiedASCBW.py
--rw-r--r--   0 marco      (502) staff       (20)     1475 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/timbre/computePSCC.py
--rw-r--r--   0 marco      (502) staff       (20)     2261 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/timbre/computeStandardizedMFCC.py
--rw-r--r--   0 marco      (502) staff       (20)     1769 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/timbre/computeStandardizedMFPS.py
--rw-r--r--   0 marco      (502) staff       (20)     1928 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/timbre/computeStandardizedPSCC.py
--rw-r--r--   0 marco      (502) staff       (20)     1194 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/timbre/mfccSoundDecay.py
--rw-r--r--   0 marco      (502) staff       (20)      848 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/timbre/mfccSoundDecayOptimal.py
--rw-r--r--   0 marco      (502) staff       (20)     1395 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/timbre/mfccSoundDecayPiecewise.py
--rw-r--r--   0 marco      (502) staff       (20)     2092 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/timbre/minimizeBKPT.py
--rw-r--r--   0 marco      (502) staff       (20)      974 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/timbre/normSoundDecay.py
--rw-r--r--   0 marco      (502) staff       (20)     1342 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/timbre/normSoundDecay2.py
-drwxr-xr-x   0 marco      (502) staff       (20)        0 2021-11-22 17:40:00.492662 musicntwrk-2.2.9/src/utils/
--rw-r--r--   0 marco      (502) staff       (20)      737 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/utils/Remove.py
--rw-r--r--   0 marco      (502) staff       (20)     1962 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/utils/SegmentedLinearReg.py
--rw-r--r--   0 marco      (502) staff       (20)      884 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/utils/Sublists.py
--rw-r--r--   0 marco      (502) staff       (20)        0 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/utils/__init__.py
--rw-r--r--   0 marco      (502) staff       (20)     3121 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/utils/communications.py
--rw-r--r--   0 marco      (502) staff       (20)     9768 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/utils/diffusionEntropyAnalyis.py
--rw-r--r--   0 marco      (502) staff       (20)     5511 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/utils/diffusionEntropyAnalyisNew.py
--rw-r--r--   0 marco      (502) staff       (20)     1758 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/utils/entropyKLdiv.py
--rw-r--r--   0 marco      (502) staff       (20)     1005 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/utils/extractByString.py
--rw-r--r--   0 marco      (502) staff       (20)      830 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/utils/fetchWaves.py
--rw-r--r--   0 marco      (502) staff       (20)     1086 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/utils/findLengthMax.py
--rw-r--r--   0 marco      (502) staff       (20)      883 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/utils/flatten.py
--rw-r--r--   0 marco      (502) staff       (20)      591 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/utils/floatize.py
--rw-r--r--   0 marco      (502) staff       (20)     1669 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/utils/generalizedOpsHistogram.py
--rw-r--r--   0 marco      (502) staff       (20)     1541 2021-11-19 01:21:35.000000 musicntwrk-2.2.9/src/utils/generalizedOpsName.py
--rw-r--r--   0 marco      (502) staff       (20)      760 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/utils/init_list_of_objects.py
--rw-r--r--   0 marco      (502) staff       (20)     1700 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/utils/load_balancing.py
--rw-r--r--   0 marco      (502) staff       (20)     1398 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/utils/minimalDistance.py
--rw-r--r--   0 marco      (502) staff       (20)     1297 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/utils/minimalDistanceVec.py
--rw-r--r--   0 marco      (502) staff       (20)     1401 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/utils/minimalNoBijDistance.py
--rw-r--r--   0 marco      (502) staff       (20)     1053 2021-11-19 16:54:18.000000 musicntwrk-2.2.9/src/utils/opsCheckByName.py
--rw-r--r--   0 marco      (502) staff       (20)      827 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/utils/opsCheckByNameVec.py
--rw-r--r--   0 marco      (502) staff       (20)      878 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/utils/opsDistance.py
--rw-r--r--   0 marco      (502) staff       (20)     1653 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/utils/opsHistogram.py
--rw-r--r--   0 marco      (502) staff       (20)     1537 2021-11-12 22:37:47.000000 musicntwrk-2.2.9/src/utils/opsName.py
--rw-r--r--   0 marco      (502) staff       (20)     2413 2021-11-19 01:35:52.000000 musicntwrk-2.2.9/src/utils/opsNameFull.py
--rw-r--r--   0 marco      (502) staff       (20)     1638 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/utils/opsNameVec.py
--rw-r--r--   0 marco      (502) staff       (20)      721 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/utils/play_with_simpleaudio.py
--rw-r--r--   0 marco      (502) staff       (20)     4681 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/utils/powerFit.py
--rw-r--r--   0 marco      (502) staff       (20)     1384 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/utils/rhythmDistance.py
--rw-r--r--   0 marco      (502) staff       (20)     2605 2021-08-06 01:36:29.000000 musicntwrk-2.2.9/src/utils/scaleFreeFit.py
--rw-r--r--   0 marco      (502) staff       (20)     1130 2021-11-22 17:37:40.000000 musicntwrk-2.2.9/src/utils/score2vLead.py
--rw-r--r--   0 marco      (502) staff       (20)      730 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/utils/str2float.py
--rw-r--r--   0 marco      (502) staff       (20)      702 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/utils/str2frac.py
--rw-r--r--   0 marco      (502) staff       (20)      963 2021-06-25 20:55:30.000000 musicntwrk-2.2.9/src/utils/vectorDistance.py
+drwxr-xr-x   0 marco      (502) staff       (20)        0 2024-04-20 13:15:10.920813 musicntwrk-2.3.0/
+-rw-r--r--   0 marco      (502) staff       (20)     7568 2024-04-20 13:15:10.920588 musicntwrk-2.3.0/PKG-INFO
+-rw-r--r--   0 marco      (502) staff       (20)     6849 2022-07-24 12:39:52.000000 musicntwrk-2.3.0/README.md
+drwxr-xr-x   0 marco      (502) staff       (20)        0 2024-04-20 13:15:10.920206 musicntwrk-2.3.0/musicntwrk.egg-info/
+-rw-r--r--   0 marco      (502) staff       (20)     7568 2024-04-20 13:15:10.000000 musicntwrk-2.3.0/musicntwrk.egg-info/PKG-INFO
+-rw-r--r--   0 marco      (502) staff       (20)     4731 2024-04-20 13:15:10.000000 musicntwrk-2.3.0/musicntwrk.egg-info/SOURCES.txt
+-rw-r--r--   0 marco      (502) staff       (20)        1 2024-04-20 13:15:10.000000 musicntwrk-2.3.0/musicntwrk.egg-info/dependency_links.txt
+-rw-r--r--   0 marco      (502) staff       (20)      159 2024-04-20 13:15:10.000000 musicntwrk-2.3.0/musicntwrk.egg-info/requires.txt
+-rw-r--r--   0 marco      (502) staff       (20)       11 2024-04-20 13:15:10.000000 musicntwrk-2.3.0/musicntwrk.egg-info/top_level.txt
+-rw-r--r--   0 marco      (502) staff       (20)       97 2023-06-23 23:50:54.000000 musicntwrk-2.3.0/pyproject.toml
+-rw-r--r--   0 marco      (502) staff       (20)       38 2024-04-20 13:15:10.920858 musicntwrk-2.3.0/setup.cfg
+-rw-r--r--   0 marco      (502) staff       (20)     1422 2024-04-20 12:32:57.000000 musicntwrk-2.3.0/setup.py
+drwxr-xr-x   0 marco      (502) staff       (20)        0 2024-04-20 13:15:10.899414 musicntwrk-2.3.0/src/
+-rw-r--r--   0 marco      (502) staff       (20)        0 2021-06-25 20:55:30.000000 musicntwrk-2.3.0/src/__init__.py
+drwxr-xr-x   0 marco      (502) staff       (20)        0 2024-04-20 13:15:10.900221 musicntwrk-2.3.0/src/comptools/
+-rw-r--r--   0 marco      (502) staff       (20)    39621 2023-08-02 08:22:01.000000 musicntwrk-2.3.0/src/comptools/MidiFile.py
+-rw-r--r--   0 marco      (502) staff       (20)     1762 2024-03-14 00:36:27.000000 musicntwrk-2.3.0/src/comptools/displayNotes.py
+-rw-r--r--   0 marco      (502) staff       (20)     2786 2023-08-02 08:22:01.000000 musicntwrk-2.3.0/src/comptools/genmidi.py
+-rw-r--r--   0 marco      (502) staff       (20)     7771 2023-08-02 08:22:01.000000 musicntwrk-2.3.0/src/comptools/music.py
+-rw-r--r--   0 marco      (502) staff       (20)     1888 2023-08-02 08:22:01.000000 musicntwrk-2.3.0/src/comptools/notation.py
+drwxr-xr-x   0 marco      (502) staff       (20)        0 2024-04-20 13:15:10.902762 musicntwrk-2.3.0/src/data/
+-rw-r--r--   0 marco      (502) staff       (20)      828 2023-08-02 08:22:01.000000 musicntwrk-2.3.0/src/data/MIDImap.py
+-rw-r--r--   0 marco      (502) staff       (20)     2559 2023-08-02 08:22:01.000000 musicntwrk-2.3.0/src/data/MIDImidi.py
+-rw-r--r--   0 marco      (502) staff       (20)      988 2023-08-02 08:22:01.000000 musicntwrk-2.3.0/src/data/MIDIscore.py
+-rw-r--r--   0 marco      (502) staff       (20)     1275 2023-08-02 08:22:01.000000 musicntwrk-2.3.0/src/data/WRITEscore.py
+-rw-r--r--   0 marco      (502) staff       (20)     1013 2023-08-02 08:22:01.000000 musicntwrk-2.3.0/src/data/WRITEscoreNoTime.py
+-rw-r--r--   0 marco      (502) staff       (20)     2086 2023-08-02 08:22:01.000000 musicntwrk-2.3.0/src/data/WRITEscoreOps.py
+-rw-r--r--   0 marco      (502) staff       (20)     3272 2023-08-02 08:22:01.000000 musicntwrk-2.3.0/src/data/WRITEscoreOpsMIDI.py
+-rw-r--r--   0 marco      (502) staff       (20)        0 2023-08-02 08:22:01.000000 musicntwrk-2.3.0/src/data/__init__.py
+-rw-r--r--   0 marco      (502) staff       (20)     2921 2023-08-02 08:22:01.000000 musicntwrk-2.3.0/src/data/analyzeSound.py
+-rw-r--r--   0 marco      (502) staff       (20)     3951 2023-08-02 08:22:01.000000 musicntwrk-2.3.0/src/data/analyzeTimbre.py
+-rw-r--r--   0 marco      (502) staff       (20)   114667 2023-08-02 08:22:01.000000 musicntwrk-2.3.0/src/data/ctcsound.py
+-rw-r--r--   0 marco      (502) staff       (20)     3993 2023-08-02 08:22:01.000000 musicntwrk-2.3.0/src/data/i_spectral.py
+-rw-r--r--   0 marco      (502) staff       (20)     3275 2023-08-02 08:22:01.000000 musicntwrk-2.3.0/src/data/i_spectral2.py
+-rw-r--r--   0 marco      (502) staff       (20)     1921 2023-08-02 08:22:01.000000 musicntwrk-2.3.0/src/data/i_spectral_pure.py
+-rw-r--r--   0 marco      (502) staff       (20)     2597 2023-08-02 08:22:01.000000 musicntwrk-2.3.0/src/data/i_spectral_pyo.py
+-rw-r--r--   0 marco      (502) staff       (20)     6358 2023-08-02 08:22:01.000000 musicntwrk-2.3.0/src/data/i_time_series.py
+-rw-r--r--   0 marco      (502) staff       (20)     1270 2023-08-02 08:22:01.000000 musicntwrk-2.3.0/src/data/r_1Ddata.py
+-rw-r--r--   0 marco      (502) staff       (20)    10624 2023-08-02 08:22:01.000000 musicntwrk-2.3.0/src/data/scaleMapping.py
+drwxr-xr-x   0 marco      (502) staff       (20)        0 2024-04-20 13:15:10.906137 musicntwrk-2.3.0/src/harmony/
+-rw-r--r--   0 marco      (502) staff       (20)       66 2023-08-02 08:22:01.000000 musicntwrk-2.3.0/src/harmony/__init__.py
+-rw-r--r--   0 marco      (502) staff       (20)     2035 2023-08-02 08:22:01.000000 musicntwrk-2.3.0/src/harmony/applyOps.py
+-rw-r--r--   0 marco      (502) staff       (20)     1256 2023-08-02 08:22:01.000000 musicntwrk-2.3.0/src/harmony/changePoint.py
+-rw-r--r--   0 marco      (502) staff       (20)     2640 2023-08-02 08:22:01.000000 musicntwrk-2.3.0/src/harmony/chinese_postman.py
+-rw-r--r--   0 marco      (502) staff       (20)     1703 2023-08-02 08:22:01.000000 musicntwrk-2.3.0/src/harmony/enharmonicDictionary.py
+-rw-r--r--   0 marco      (502) staff       (20)     1309 2023-08-02 08:22:01.000000 musicntwrk-2.3.0/src/harmony/getRN.py
+-rw-r--r--   0 marco      (502) staff       (20)     4084 2023-08-02 08:22:01.000000 musicntwrk-2.3.0/src/harmony/harmonicDesign.py
+-rw-r--r--   0 marco      (502) staff       (20)     2905 2023-08-02 08:22:01.000000 musicntwrk-2.3.0/src/harmony/keySections.py
+-rw-r--r--   0 marco      (502) staff       (20)     3022 2023-08-02 08:22:01.000000 musicntwrk-2.3.0/src/harmony/lookupOps.py
+-rw-r--r--   0 marco      (502) staff       (20)      884 2023-08-02 08:22:01.000000 musicntwrk-2.3.0/src/harmony/lookupProgr.py
+-rw-r--r--   0 marco      (502) staff       (20)     1265 2023-08-02 08:22:01.000000 musicntwrk-2.3.0/src/harmony/lookupWrapper.py
+-rw-r--r--   0 marco      (502) staff       (20)     2416 2023-08-02 08:26:29.000000 musicntwrk-2.3.0/src/harmony/networkHarmonyGen.py
+-rw-r--r--   0 marco      (502) staff       (20)     2769 2023-08-02 08:22:01.000000 musicntwrk-2.3.0/src/harmony/plotHarmonicTable.py
+-rw-r--r--   0 marco      (502) staff       (20)     2784 2023-12-28 02:44:32.000000 musicntwrk-2.3.0/src/harmony/rhythmicDesign.py
+-rw-r--r--   0 marco      (502) staff       (20)     4765 2023-08-02 08:22:01.000000 musicntwrk-2.3.0/src/harmony/scoreAnalysis.py
+-rw-r--r--   0 marco      (502) staff       (20)     1257 2023-08-02 08:22:01.000000 musicntwrk-2.3.0/src/harmony/scoreDesign.py
+-rw-r--r--   0 marco      (502) staff       (20)     2307 2023-08-02 08:22:01.000000 musicntwrk-2.3.0/src/harmony/scoreFilter.py
+-rw-r--r--   0 marco      (502) staff       (20)     2492 2023-08-02 08:22:01.000000 musicntwrk-2.3.0/src/harmony/shortHands.py
+-rw-r--r--   0 marco      (502) staff       (20)     2002 2023-08-02 08:22:01.000000 musicntwrk-2.3.0/src/harmony/showAnalysis.py
+-rw-r--r--   0 marco      (502) staff       (20)     4473 2023-08-02 08:24:49.000000 musicntwrk-2.3.0/src/harmony/spiralChordSpace.py
+-rw-r--r--   0 marco      (502) staff       (20)     2921 2023-08-02 08:22:01.000000 musicntwrk-2.3.0/src/harmony/tonalAnalysis.py
+-rw-r--r--   0 marco      (502) staff       (20)     7685 2023-08-02 08:22:01.000000 musicntwrk-2.3.0/src/harmony/tonalHarmonyCalculator.py
+-rw-r--r--   0 marco      (502) staff       (20)     4652 2023-08-02 08:22:01.000000 musicntwrk-2.3.0/src/harmony/tonalHarmonyModels.py
+-rw-r--r--   0 marco      (502) staff       (20)     1899 2023-08-02 08:22:01.000000 musicntwrk-2.3.0/src/harmony/tonalPartition.py
+-rw-r--r--   0 marco      (502) staff       (20)     2411 2023-08-02 08:22:01.000000 musicntwrk-2.3.0/src/harmony/tonnentz.py
+drwxr-xr-x   0 marco      (502) staff       (20)        0 2024-04-20 13:15:10.907314 musicntwrk-2.3.0/src/ml_utils/
+-rw-r--r--   0 marco      (502) staff       (20)       88 2023-08-02 08:22:01.000000 musicntwrk-2.3.0/src/ml_utils/__init__.py
+-rw-r--r--   0 marco      (502) staff       (20)     2695 2024-04-14 21:34:16.000000 musicntwrk-2.3.0/src/ml_utils/checkRun.py
+-rw-r--r--   0 marco      (502) staff       (20)     1407 2024-04-14 21:35:54.000000 musicntwrk-2.3.0/src/ml_utils/modelDump.py
+-rw-r--r--   0 marco      (502) staff       (20)     1479 2024-04-14 22:54:15.000000 musicntwrk-2.3.0/src/ml_utils/modelLoad.py
+-rw-r--r--   0 marco      (502) staff       (20)     1513 2023-08-02 08:22:01.000000 musicntwrk-2.3.0/src/ml_utils/multiModelPredictor.py
+-rw-r--r--   0 marco      (502) staff       (20)     1432 2023-08-02 08:22:01.000000 musicntwrk-2.3.0/src/ml_utils/prepareDataSet.py
+-rw-r--r--   0 marco      (502) staff       (20)     2024 2024-04-15 02:03:11.000000 musicntwrk-2.3.0/src/ml_utils/readModels.py
+-rw-r--r--   0 marco      (502) staff       (20)      814 2023-08-02 08:22:01.000000 musicntwrk-2.3.0/src/ml_utils/scaleDataSet.py
+-rw-r--r--   0 marco      (502) staff       (20)     3299 2024-04-14 22:11:15.000000 musicntwrk-2.3.0/src/ml_utils/trainCNNmodel.py
+-rw-r--r--   0 marco      (502) staff       (20)     2260 2024-04-14 21:50:15.000000 musicntwrk-2.3.0/src/ml_utils/trainNNmodel.py
+drwxr-xr-x   0 marco      (502) staff       (20)        0 2024-04-20 13:15:10.909625 musicntwrk-2.3.0/src/msctools/
+-rw-r--r--   0 marco      (502) staff       (20)     8840 2023-01-15 21:28:01.000000 musicntwrk-2.3.0/src/msctools/base.py
+-rw-r--r--   0 marco      (502) staff       (20)      597 2024-04-20 12:53:06.000000 musicntwrk-2.3.0/src/msctools/cfg.py
+-rw-r--r--   0 marco      (502) staff       (20)     2248 2023-09-08 07:15:36.000000 musicntwrk-2.3.0/src/msctools/converters.py
+-rw-r--r--   0 marco      (502) staff       (20)      336 2024-01-30 00:27:07.000000 musicntwrk-2.3.0/src/msctools/decorators.py
+-rw-r--r--   0 marco      (502) staff       (20)     7069 2022-12-03 20:17:50.000000 musicntwrk-2.3.0/src/msctools/devices.py
+-rw-r--r--   0 marco      (502) staff       (20)    78504 2024-01-20 15:29:09.000000 musicntwrk-2.3.0/src/msctools/dictionaries.py
+-rw-r--r--   0 marco      (502) staff       (20)    48647 2023-11-09 23:14:46.000000 musicntwrk-2.3.0/src/msctools/dsp.py
+-rw-r--r--   0 marco      (502) staff       (20)     5940 2024-04-17 17:59:59.000000 musicntwrk-2.3.0/src/msctools/envelopes.py
+-rw-r--r--   0 marco      (502) staff       (20)    19624 2024-04-20 12:45:11.000000 musicntwrk-2.3.0/src/msctools/networks.py
+-rw-r--r--   0 marco      (502) staff       (20)      865 2023-04-13 16:06:16.000000 musicntwrk-2.3.0/src/msctools/oscserver.py
+-rw-r--r--   0 marco      (502) staff       (20)     1285 2022-12-20 16:04:25.000000 musicntwrk-2.3.0/src/msctools/osctools.py
+-rw-r--r--   0 marco      (502) staff       (20)      472 2022-11-22 00:46:09.000000 musicntwrk-2.3.0/src/msctools/pan.py
+-rw-r--r--   0 marco      (502) staff       (20)     4807 2024-04-20 12:31:37.000000 musicntwrk-2.3.0/src/msctools/players.py
+-rw-r--r--   0 marco      (502) staff       (20)     1637 2024-02-13 23:17:01.000000 musicntwrk-2.3.0/src/msctools/pyoPlayer.py
+-rw-r--r--   0 marco      (502) staff       (20)    17002 2024-04-20 13:03:26.000000 musicntwrk-2.3.0/src/msctools/pyotools.py
+-rw-r--r--   0 marco      (502) staff       (20)     1355 2024-04-20 12:31:32.000000 musicntwrk-2.3.0/src/msctools/session.py
+-rw-r--r--   0 marco      (502) staff       (20)      434 2023-01-02 23:35:19.000000 musicntwrk-2.3.0/src/msctools/utils.py
+-rw-r--r--   0 marco      (502) staff       (20)     5386 2023-04-13 16:05:54.000000 musicntwrk-2.3.0/src/msctools/videocapture.py
+-rw-r--r--   0 marco      (502) staff       (20)    68822 2024-01-26 02:18:22.000000 musicntwrk-2.3.0/src/musicntwrk.py
+drwxr-xr-x   0 marco      (502) staff       (20)        0 2024-04-20 13:15:10.912529 musicntwrk-2.3.0/src/networks/
+-rw-r--r--   0 marco      (502) staff       (20)        0 2023-08-02 08:22:01.000000 musicntwrk-2.3.0/src/networks/__init__.py
+-rw-r--r--   0 marco      (502) staff       (20)     2580 2023-08-02 08:22:01.000000 musicntwrk-2.3.0/src/networks/analysisNetwork.py
+-rw-r--r--   0 marco      (502) staff       (20)     2646 2023-08-02 08:22:01.000000 musicntwrk-2.3.0/src/networks/orchestralNetwork.py
+-rw-r--r--   0 marco      (502) staff       (20)     2388 2023-08-02 08:22:01.000000 musicntwrk-2.3.0/src/networks/orchestralVector.py
+-rw-r--r--   0 marco      (502) staff       (20)     1636 2023-08-02 08:22:01.000000 musicntwrk-2.3.0/src/networks/orchestralVectorColor.py
+-rw-r--r--   0 marco      (502) staff       (20)     4780 2023-08-02 08:22:01.000000 musicntwrk-2.3.0/src/networks/pcsDictionary.py
+-rw-r--r--   0 marco      (502) staff       (20)     5852 2023-08-02 08:22:01.000000 musicntwrk-2.3.0/src/networks/pcsEgoNetwork.py
+-rw-r--r--   0 marco      (502) staff       (20)     4914 2023-08-02 08:22:01.000000 musicntwrk-2.3.0/src/networks/pcsNetwork.py
+-rw-r--r--   0 marco      (502) staff       (20)     2966 2023-08-02 08:22:01.000000 musicntwrk-2.3.0/src/networks/rLeadNetwork.py
+-rw-r--r--   0 marco      (502) staff       (20)     2470 2023-08-02 08:22:01.000000 musicntwrk-2.3.0/src/networks/readScore.py
+-rw-r--r--   0 marco      (502) staff       (20)     3085 2023-08-02 08:22:01.000000 musicntwrk-2.3.0/src/networks/rhythmDictionary.py
+-rw-r--r--   0 marco      (502) staff       (20)     4322 2023-08-02 08:22:01.000000 musicntwrk-2.3.0/src/networks/rhythmNetwork.py
+-rw-r--r--   0 marco      (502) staff       (20)     4053 2023-12-28 02:35:13.000000 musicntwrk-2.3.0/src/networks/rhythmPDictionary.py
+-rw-r--r--   0 marco      (502) staff       (20)     2456 2023-08-02 08:22:01.000000 musicntwrk-2.3.0/src/networks/scoreDictionary.py
+-rw-r--r--   0 marco      (502) staff       (20)     1592 2023-08-02 08:22:01.000000 musicntwrk-2.3.0/src/networks/scoreMIDIDictionary.py
+-rw-r--r--   0 marco      (502) staff       (20)     5809 2023-08-02 08:22:01.000000 musicntwrk-2.3.0/src/networks/scoreNetwork.py
+-rw-r--r--   0 marco      (502) staff       (20)     5791 2023-08-02 08:22:01.000000 musicntwrk-2.3.0/src/networks/scoreSubNetwork.py
+-rw-r--r--   0 marco      (502) staff       (20)     3697 2023-08-02 08:22:01.000000 musicntwrk-2.3.0/src/networks/timbralNetwork.py
+-rw-r--r--   0 marco      (502) staff       (20)     4102 2023-08-02 08:22:01.000000 musicntwrk-2.3.0/src/networks/vLeadNetwork.py
+-rw-r--r--   0 marco      (502) staff       (20)     4789 2023-08-02 08:22:01.000000 musicntwrk-2.3.0/src/networks/vLeadNetworkByName.py
+-rw-r--r--   0 marco      (502) staff       (20)     2936 2023-08-02 08:22:01.000000 musicntwrk-2.3.0/src/networks/vLeadNetworkByNameVec.py
+-rw-r--r--   0 marco      (502) staff       (20)     2634 2023-08-02 08:22:01.000000 musicntwrk-2.3.0/src/networks/vLeadNetworkVec.py
+drwxr-xr-x   0 marco      (502) staff       (20)        0 2024-04-20 13:15:10.914093 musicntwrk-2.3.0/src/plotting/
+-rw-r--r--   0 marco      (502) staff       (20)     1061 2023-08-02 08:22:01.000000 musicntwrk-2.3.0/src/plotting/barplot.py
+-rw-r--r--   0 marco      (502) staff       (20)    24919 2023-12-21 02:30:18.000000 musicntwrk-2.3.0/src/plotting/chordspace.py
+-rw-r--r--   0 marco      (502) staff       (20)     7250 2023-08-02 08:22:01.000000 musicntwrk-2.3.0/src/plotting/drawMultiLayerNetwork.py
+-rw-r--r--   0 marco      (502) staff       (20)     2888 2023-08-02 08:22:01.000000 musicntwrk-2.3.0/src/plotting/drawNetwork.py
+-rw-r--r--   0 marco      (502) staff       (20)     6340 2023-08-02 09:17:49.000000 musicntwrk-2.3.0/src/plotting/drawNetwork3D.py
+-rw-r--r--   0 marco      (502) staff       (20)     2256 2023-08-02 08:22:01.000000 musicntwrk-2.3.0/src/plotting/drawNetworkViz.py
+-rw-r--r--   0 marco      (502) staff       (20)     1246 2023-08-02 08:22:01.000000 musicntwrk-2.3.0/src/plotting/drawNetworkX.py
+-rw-r--r--   0 marco      (502) staff       (20)      890 2023-08-02 08:22:01.000000 musicntwrk-2.3.0/src/plotting/plotCC.py
+-rw-r--r--   0 marco      (502) staff       (20)      716 2023-08-02 08:22:01.000000 musicntwrk-2.3.0/src/plotting/plotCurveXY.py
+-rw-r--r--   0 marco      (502) staff       (20)      711 2023-08-02 08:22:01.000000 musicntwrk-2.3.0/src/plotting/plotCurveY.py
+-rw-r--r--   0 marco      (502) staff       (20)     1680 2023-08-02 14:25:53.000000 musicntwrk-2.3.0/src/plotting/plotDegreeAnalysis.py
+-rw-r--r--   0 marco      (502) staff       (20)     1864 2023-08-02 08:22:01.000000 musicntwrk-2.3.0/src/plotting/plotOpsHistogram.py
+drwxr-xr-x   0 marco      (502) staff       (20)        0 2024-04-20 13:15:10.915850 musicntwrk-2.3.0/src/timbre/
+-rw-r--r--   0 marco      (502) staff       (20)        0 2023-08-02 08:22:01.000000 musicntwrk-2.3.0/src/timbre/__init__.py
+-rw-r--r--   0 marco      (502) staff       (20)     1743 2023-08-02 08:22:01.000000 musicntwrk-2.3.0/src/timbre/computeASCBW.py
+-rw-r--r--   0 marco      (502) staff       (20)     1552 2023-08-02 08:22:01.000000 musicntwrk-2.3.0/src/timbre/computeCompMPS.py
+-rw-r--r--   0 marco      (502) staff       (20)     1663 2023-08-02 08:22:01.000000 musicntwrk-2.3.0/src/timbre/computeMFCC.py
+-rw-r--r--   0 marco      (502) staff       (20)     2648 2023-08-02 08:22:01.000000 musicntwrk-2.3.0/src/timbre/computeModifiedASCBW.py
+-rw-r--r--   0 marco      (502) staff       (20)     1475 2023-08-02 08:22:01.000000 musicntwrk-2.3.0/src/timbre/computePSCC.py
+-rw-r--r--   0 marco      (502) staff       (20)     2263 2023-08-02 08:22:01.000000 musicntwrk-2.3.0/src/timbre/computeStandardizedMFCC.py
+-rw-r--r--   0 marco      (502) staff       (20)     1769 2023-08-02 08:22:01.000000 musicntwrk-2.3.0/src/timbre/computeStandardizedMFPS.py
+-rw-r--r--   0 marco      (502) staff       (20)     1926 2023-08-02 08:22:01.000000 musicntwrk-2.3.0/src/timbre/computeStandardizedPSCC.py
+-rw-r--r--   0 marco      (502) staff       (20)     1194 2023-08-02 08:22:01.000000 musicntwrk-2.3.0/src/timbre/mfccSoundDecay.py
+-rw-r--r--   0 marco      (502) staff       (20)      848 2023-08-02 08:22:01.000000 musicntwrk-2.3.0/src/timbre/mfccSoundDecayOptimal.py
+-rw-r--r--   0 marco      (502) staff       (20)     1395 2023-08-02 08:22:01.000000 musicntwrk-2.3.0/src/timbre/mfccSoundDecayPiecewise.py
+-rw-r--r--   0 marco      (502) staff       (20)     2092 2023-08-02 08:22:01.000000 musicntwrk-2.3.0/src/timbre/minimizeBKPT.py
+-rw-r--r--   0 marco      (502) staff       (20)      974 2023-08-02 08:22:01.000000 musicntwrk-2.3.0/src/timbre/normSoundDecay.py
+-rw-r--r--   0 marco      (502) staff       (20)     1342 2023-08-02 08:22:01.000000 musicntwrk-2.3.0/src/timbre/normSoundDecay2.py
+drwxr-xr-x   0 marco      (502) staff       (20)        0 2024-04-20 13:15:10.920015 musicntwrk-2.3.0/src/utils/
+-rw-r--r--   0 marco      (502) staff       (20)     1142 2023-08-02 08:22:01.000000 musicntwrk-2.3.0/src/utils/Remove.py
+-rw-r--r--   0 marco      (502) staff       (20)     1962 2023-08-02 08:22:01.000000 musicntwrk-2.3.0/src/utils/SegmentedLinearReg.py
+-rw-r--r--   0 marco      (502) staff       (20)      884 2023-08-02 08:22:01.000000 musicntwrk-2.3.0/src/utils/Sublists.py
+-rw-r--r--   0 marco      (502) staff       (20)        0 2023-08-02 08:22:01.000000 musicntwrk-2.3.0/src/utils/__init__.py
+-rw-r--r--   0 marco      (502) staff       (20)     3121 2023-08-02 08:22:01.000000 musicntwrk-2.3.0/src/utils/communications.py
+-rw-r--r--   0 marco      (502) staff       (20)     9768 2023-08-02 08:22:01.000000 musicntwrk-2.3.0/src/utils/diffusionEntropyAnalyis.py
+-rw-r--r--   0 marco      (502) staff       (20)     5511 2023-08-02 08:22:01.000000 musicntwrk-2.3.0/src/utils/diffusionEntropyAnalyisNew.py
+-rw-r--r--   0 marco      (502) staff       (20)     1758 2023-08-02 08:22:01.000000 musicntwrk-2.3.0/src/utils/entropyKLdiv.py
+-rw-r--r--   0 marco      (502) staff       (20)     1005 2023-08-02 08:22:01.000000 musicntwrk-2.3.0/src/utils/extractByString.py
+-rw-r--r--   0 marco      (502) staff       (20)      830 2023-08-02 08:22:01.000000 musicntwrk-2.3.0/src/utils/fetchWaves.py
+-rw-r--r--   0 marco      (502) staff       (20)     1086 2023-08-02 08:22:01.000000 musicntwrk-2.3.0/src/utils/findLengthMax.py
+-rw-r--r--   0 marco      (502) staff       (20)      883 2023-08-02 08:22:01.000000 musicntwrk-2.3.0/src/utils/flatten.py
+-rw-r--r--   0 marco      (502) staff       (20)      591 2023-08-02 08:22:01.000000 musicntwrk-2.3.0/src/utils/floatize.py
+-rw-r--r--   0 marco      (502) staff       (20)     1669 2023-08-02 08:22:01.000000 musicntwrk-2.3.0/src/utils/generalizedOpsHistogram.py
+-rw-r--r--   0 marco      (502) staff       (20)     1541 2023-08-02 08:22:01.000000 musicntwrk-2.3.0/src/utils/generalizedOpsName.py
+-rw-r--r--   0 marco      (502) staff       (20)      760 2023-08-02 08:22:01.000000 musicntwrk-2.3.0/src/utils/init_list_of_objects.py
+-rw-r--r--   0 marco      (502) staff       (20)     1700 2023-08-02 08:22:01.000000 musicntwrk-2.3.0/src/utils/load_balancing.py
+-rw-r--r--   0 marco      (502) staff       (20)     1398 2023-08-02 08:22:01.000000 musicntwrk-2.3.0/src/utils/minimalDistance.py
+-rw-r--r--   0 marco      (502) staff       (20)     1297 2023-08-02 08:22:01.000000 musicntwrk-2.3.0/src/utils/minimalDistanceVec.py
+-rw-r--r--   0 marco      (502) staff       (20)     1401 2023-08-02 08:22:01.000000 musicntwrk-2.3.0/src/utils/minimalNoBijDistance.py
+-rw-r--r--   0 marco      (502) staff       (20)     1053 2023-08-02 08:22:01.000000 musicntwrk-2.3.0/src/utils/opsCheckByName.py
+-rw-r--r--   0 marco      (502) staff       (20)      827 2023-08-02 08:22:01.000000 musicntwrk-2.3.0/src/utils/opsCheckByNameVec.py
+-rw-r--r--   0 marco      (502) staff       (20)      878 2023-08-02 08:22:01.000000 musicntwrk-2.3.0/src/utils/opsDistance.py
+-rw-r--r--   0 marco      (502) staff       (20)     1653 2023-08-02 08:22:01.000000 musicntwrk-2.3.0/src/utils/opsHistogram.py
+-rw-r--r--   0 marco      (502) staff       (20)     1537 2023-08-02 08:22:01.000000 musicntwrk-2.3.0/src/utils/opsName.py
+-rw-r--r--   0 marco      (502) staff       (20)     2413 2023-08-02 08:22:01.000000 musicntwrk-2.3.0/src/utils/opsNameFull.py
+-rw-r--r--   0 marco      (502) staff       (20)     1638 2023-08-02 08:22:01.000000 musicntwrk-2.3.0/src/utils/opsNameVec.py
+-rw-r--r--   0 marco      (502) staff       (20)      721 2023-08-02 08:22:01.000000 musicntwrk-2.3.0/src/utils/play_with_simpleaudio.py
+-rw-r--r--   0 marco      (502) staff       (20)     4681 2023-08-02 08:22:01.000000 musicntwrk-2.3.0/src/utils/powerFit.py
+-rw-r--r--   0 marco      (502) staff       (20)     1384 2023-08-02 08:22:01.000000 musicntwrk-2.3.0/src/utils/rhythmDistance.py
+-rw-r--r--   0 marco      (502) staff       (20)     2605 2023-08-02 08:22:01.000000 musicntwrk-2.3.0/src/utils/scaleFreeFit.py
+-rw-r--r--   0 marco      (502) staff       (20)     1130 2023-08-02 08:22:01.000000 musicntwrk-2.3.0/src/utils/score2vLead.py
+-rw-r--r--   0 marco      (502) staff       (20)      730 2023-08-02 08:22:01.000000 musicntwrk-2.3.0/src/utils/str2float.py
+-rw-r--r--   0 marco      (502) staff       (20)      702 2023-08-02 08:22:01.000000 musicntwrk-2.3.0/src/utils/str2frac.py
+-rw-r--r--   0 marco      (502) staff       (20)      963 2023-08-02 08:22:01.000000 musicntwrk-2.3.0/src/utils/vectorDistance.py
```

### Comparing `musicntwrk-2.2.9/PKG-INFO` & `musicntwrk-2.3.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,119 +1,107 @@
-Metadata-Version: 2.1
-Name: musicntwrk
-Version: 2.2.9
-Summary: music as data, data as music
-Home-page: https://www.musicntwrk.com
-Author: Marco Buongiorno Nardelli
-Author-email: mbn@unt.edu
-License: UNKNOWN
-Description: <p></p>
-        <p align="center">
-          <a href="https://www.musicntwrk.com">
-            <img src="https://raw.githubusercontent.com/marcobn/musicntwrk/master/IMAGES/logo.png" alt="musicntwrk logo" height="84">
-          </a>
-        </p>
-        
-        <h3 align="center">music as data, data as music</h3>
-        
-        <p align="center">
-          <em>unleashing data tools for music theory, analysis and composition</em>
-          <br>
-          <br>
-        A python library for pitch class set and rhythmic sequences classification and manipulation, the generation of networks in generalized music and sound spaces, deep learning algorithms for timbre recognition, and the sonification of arbitrary data
-        <br>
-        </p>
-        
-        ## Table of contents
-        
-        - [Quick start](#quick-start)
-        - [What's included](#whats-included)
-        - [Documentation](#documentation)
-        - [Author](#author)
-        - [Citation](#citation)
-        - [Thanks](#thanks)
-        
-        ## Quick start
-        
-        ## pip install musicntwrk
-        or
-        ## pip install musicntwrk[with_MPI]
-        (if there is a pre-existing installation of MPI, pip will automatically install the mpi4pi wrapper)
-        
-        - [OR download the latest release from GitHub](https://github.com/marcobn/musicntwrk/)
-        - Clone the repo: `git clone https://github.com/marcobn/musicntwrk.git`
-        - cd musicntwrk-2.0
-        - pip install .
-        
-        ## - [Examples and support files can be downloaded here](https://github.com/marcobn/musicntwrk/tree/master/musicntwrk-2.0/examples)
-        There are three example notebooks: basic, advanced harmony, advanced timbre. See the ipynb files for a full description.
-        
-        ## What's included
-        **musicntwrk** is a project written for python 3 and comprised of a main module, `musicntwrk`, and many additional helper packages included in the distribution:
-        - `musicntwrk` - is the main module and contains helper clasess for pitch class set classification and manipulation in any arbitrary temperament (PCSet, PCSetR and PCSrow), and the main class musicntwrk that allows the construction of generalized musical space networks using distances between common descriptors (interval vectors, voice leadings, rhythm distance, etc.); the analysis of scores, the sonification of data and the generation of compositional frameworks. `musicntwrk` acts as a wrapper for the various functions organized in the following sub projects:
-          - `networks` - contains all the modules to construct dictionaries and networks of pitch class set spaces including voice leading, rhythmic spaces, timbral spaces and score network and orchestarion analysis 
-          - `data` - sonification of arbitrary data structures, including automatic score (musicxml) and MIDI generation
-          - `timbre` - analysis and characterization of timbre from a (psycho-)acoustical point of view. In particular, it provides: the characterization of sound using, among others, Mel Frequency or Power Spectrum Cepstrum Coefficients (MFCC or PSCC); the construction of timbral networks using descriptors based on MF- or PS-CCs
-          - `harmony` - helper functions for harmonic analysis, design and autonomous scoring
-          - `ml_utils` - machine learning models for timbre recognition through the TensorFlow Keras framework
-          - `plotting` - plotting function including a module for automated network drawing
-          - `utils` - utility functions used by other modules
-        
-        ## Documentation
-        
-        - [musicntwrk](https://github.com/marcobn/musicntwrk/blob/master/DOCS/musicntwrk.md)
-        - [networks](https://github.com/marcobn/musicntwrk/blob/master/DOCS/networks.md)
-        - [data](https://github.com/marcobn/musicntwrk/blob/master/DOCS/data.md)
-        - [timbre](https://github.com/marcobn/musicntwrk/blob/master/DOCS/timbre.md)
-        - [harmony](https://github.com/marcobn/musicntwrk/blob/master/DOCS/harmony.md)
-        - [ml_utils](https://github.com/marcobn/musicntwrk/blob/master/DOCS/ml_utils.md)
-        - [plotting](https://github.com/marcobn/musicntwrk/blob/master/DOCS/plotting.md)
-        
-        The most computationally intensive parts of the modules can be run on parallel processors using the MPI (Message Passing Interface) protocol. Communications are handled by two additional modules: `communications` and `load_balancing`. Since the user will never have to interact with these modules, we omit here a detailed description of their functions.
-        
-        ## Author
-        
-        **Marco Buongiorno Nardelli**
-        
-        Marco Buongiorno Nardelli is University Distinguished Research Professor at the University of North Texas: composer, flutist, computational materials physicist, and a member of CEMI, the Center for Experimental Music and Intermedia, and iARTA, the Initiative for Advanced Research in Technology and the Arts. He is a Fellow of the American Physical Society and of the Institute of Physics, and a Parma Recordings artist. See [here](https://www.materialssoundmusic.com/long-bio) for a longer bio-sketch.
-        
-        ## Citation
-        
-        Marco Buongiorno Nardelli, _"musicntwrk, a python library for pitch class set and rhythmic sequences classification and manipulation, the generation of networks in generalized music and sound spaces, deep learning algorithms for timbre recognition, and the sonification of arbitrary data"_, www.musicntwrk.com (2019).
-        
-        ## Thanks
-        
-        This project has been made possible by contributions from the following institutions:
-        <p align="center">
-          <a href="https://www.unt.edu">
-            <img src="https://raw.githubusercontent.com/marcobn/musicntwrk/master/IMAGES//unt.png" alt="UNT logo" height="148" align="bottom">
-          </a>&ensp;&ensp;&ensp;
-          <a href="https://cemi.music.unt.edu">
-            <img src="https://raw.githubusercontent.com/marcobn/musicntwrk/master/IMAGES/cemi.png" alt="CEMI logo" height="84" align="bottom">
-          </a>&ensp;&ensp;&ensp;
-          <a href="https://www.prism.cnrs.fr">
-            <img src="https://raw.githubusercontent.com/marcobn/musicntwrk/master/IMAGES/prism.png" alt="PRISM logo" height="132" align="bottom">
-          </a>&ensp;&ensp;&ensp;
-          <a href="https://imera.univ-amu.fr">
-            <img src="https://raw.githubusercontent.com/marcobn/musicntwrk/master/IMAGES//imera.png" alt="IMeRA logo" height="72" align="bottom">
-          </a>
-        </p>
-        <p>
-        <hr>
-        </p>
-        
-        <p align="center">
-        <strong>musicntwrk</strong> is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
-        This program is distributed in the hope that it will be useful, but <strong>WITHOUT ANY WARRANTY</strong>; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
-        You should have received a copy of the GNU General Public License along with this program. If not, see <a href="http://www.gnu.org/licenses/"> http://www.gnu.org/licenses/</a>.
-        </p>
-        <p></p>
-        <p align="center">
-        Copyright (C) 2018-2020 Marco Buongiorno Nardelli  <br>
-        <a href="https://www.materialssoundmusic.com"> www.materialssoundmusic.com <br>
-        <a href="https://www.musicntwrk.com"> www.musicntwrk.com <br>
-        <a href="mailto:mbn@unt.edu"> mbn@unt.edu <br>
-        </p>
-        
-Platform: OS independent
-Description-Content-Type: text/markdown
-Provides-Extra: with_MPI
+<p></p>
+<p align="center">
+  <a href="https://www.musicntwrk.com">
+    <img src="https://raw.githubusercontent.com/marcobn/musicntwrk/master/IMAGES/logo.png" alt="musicntwrk logo" height="84">
+  </a>
+</p>
+
+<h3 align="center">music as data, data as music</h3>
+
+<p align="center">
+  <em>unleashing data tools for music theory, analysis and composition</em>
+  <br>
+  <br>
+A python library for pitch class set and rhythmic sequences classification and manipulation, the generation of networks in generalized music and sound spaces, deep learning algorithms for timbre recognition, and the sonification of arbitrary data
+<br>
+</p>
+
+## Table of contents
+
+- [Quick start](#quick-start)
+- [What's included](#whats-included)
+- [Documentation](#documentation)
+- [Author](#author)
+- [Citation](#citation)
+- [Thanks](#thanks)
+
+## Quick start
+
+## pip install musicntwrk
+or
+## pip install musicntwrk[with_MPI]
+(if there is a pre-existing installation of MPI, pip will automatically install the mpi4pi wrapper)
+
+- [OR download the latest release from GitHub](https://github.com/marcobn/musicntwrk/)
+- Clone the repo: `git clone https://github.com/marcobn/musicntwrk.git`
+- cd musicntwrk-2.0
+- pip install .
+
+## - [Examples and support files can be downloaded here](https://github.com/marcobn/musicntwrk/tree/master/musicntwrk-2.0/examples)
+There are three example notebooks: basic, advanced harmony, advanced timbre. See the ipynb files for a full description.
+
+## What's included
+**musicntwrk** is a project written for python 3 and comprised of a main module, `musicntwrk`, and many additional helper packages included in the distribution:
+- `musicntwrk` - is the main module and contains helper clasess for pitch class set classification and manipulation in any arbitrary temperament (PCSet, PCSetR and PCSrow), and the main class musicntwrk that allows the construction of generalized musical space networks using distances between common descriptors (interval vectors, voice leadings, rhythm distance, etc.); the analysis of scores, the sonification of data and the generation of compositional frameworks. `musicntwrk` acts as a wrapper for the various functions organized in the following sub projects:
+  - `networks` - contains all the modules to construct dictionaries and networks of pitch class set spaces including voice leading, rhythmic spaces, timbral spaces and score network and orchestarion analysis 
+  - `data` - sonification of arbitrary data structures, including automatic score (musicxml) and MIDI generation
+  - `timbre` - analysis and characterization of timbre from a (psycho-)acoustical point of view. In particular, it provides: the characterization of sound using, among others, Mel Frequency or Power Spectrum Cepstrum Coefficients (MFCC or PSCC); the construction of timbral networks using descriptors based on MF- or PS-CCs
+  - `harmony` - helper functions for harmonic analysis, design and autonomous scoring
+  - `ml_utils` - machine learning models for timbre recognition through the TensorFlow Keras framework
+  - `plotting` - plotting function including a module for automated network drawing
+  - `utils` - utility functions used by other modules
+
+## Documentation
+
+- [musicntwrk](https://github.com/marcobn/musicntwrk/blob/master/DOCS/musicntwrk.md)
+- [networks](https://github.com/marcobn/musicntwrk/blob/master/DOCS/networks.md)
+- [data](https://github.com/marcobn/musicntwrk/blob/master/DOCS/data.md)
+- [timbre](https://github.com/marcobn/musicntwrk/blob/master/DOCS/timbre.md)
+- [harmony](https://github.com/marcobn/musicntwrk/blob/master/DOCS/harmony.md)
+- [ml_utils](https://github.com/marcobn/musicntwrk/blob/master/DOCS/ml_utils.md)
+- [plotting](https://github.com/marcobn/musicntwrk/blob/master/DOCS/plotting.md)
+
+The most computationally intensive parts of the modules can be run on parallel processors using the MPI (Message Passing Interface) protocol. Communications are handled by two additional modules: `communications` and `load_balancing`. Since the user will never have to interact with these modules, we omit here a detailed description of their functions.
+
+## Author
+
+**Marco Buongiorno Nardelli**
+
+Marco Buongiorno Nardelli is Regents Professor at the University of North Texas: composer, flutist, computational materials physicist, and a member of CEMI, the Center for Experimental Music and Intermedia, and iARTA, the Initiative for Advanced Research in Technology and the Arts. He is a Fellow of the American Physical Society and of the Institute of Physics, and a Parma Recordings artist. See [here](https://www.materialssoundmusic.com/long-bio) for a longer bio-sketch.
+
+## Citation
+
+Marco Buongiorno Nardelli, _"musicntwrk, a python library for pitch class set and rhythmic sequences classification and manipulation, the generation of networks in generalized music and sound spaces, deep learning algorithms for timbre recognition, and the sonification of arbitrary data"_, www.musicntwrk.com (2019).
+
+## Thanks
+
+This project has been made possible by contributions from the following institutions:
+<p align="center">
+  <a href="https://www.unt.edu">
+    <img src="https://raw.githubusercontent.com/marcobn/musicntwrk/master/IMAGES//unt.png" alt="UNT logo" height="148" align="bottom">
+  </a>&ensp;&ensp;&ensp;
+  <a href="https://cemi.music.unt.edu">
+    <img src="https://raw.githubusercontent.com/marcobn/musicntwrk/master/IMAGES/cemi.png" alt="CEMI logo" height="84" align="bottom">
+  </a>&ensp;&ensp;&ensp;
+  <a href="https://www.prism.cnrs.fr">
+    <img src="https://raw.githubusercontent.com/marcobn/musicntwrk/master/IMAGES/prism.png" alt="PRISM logo" height="132" align="bottom">
+  </a>&ensp;&ensp;&ensp;
+  <a href="https://imera.univ-amu.fr">
+    <img src="https://raw.githubusercontent.com/marcobn/musicntwrk/master/IMAGES//imera.png" alt="IMeRA logo" height="72" align="bottom">
+  </a>
+</p>
+<p>
+<hr>
+</p>
+
+<p align="center">
+<strong>musicntwrk</strong> is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
+This program is distributed in the hope that it will be useful, but <strong>WITHOUT ANY WARRANTY</strong>; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
+You should have received a copy of the GNU General Public License along with this program. If not, see <a href="http://www.gnu.org/licenses/"> http://www.gnu.org/licenses/</a>.
+</p>
+<p></p>
+<p align="center">
+Copyright (C) 2018-2020 Marco Buongiorno Nardelli  <br>
+<a href="https://www.materialssoundmusic.com"> www.materialssoundmusic.com <br>
+<a href="https://www.musicntwrk.com"> www.musicntwrk.com <br>
+<a href="mailto:mbn@unt.edu"> mbn@unt.edu <br>
+</p>
```

#### html2text {}

```diff
@@ -1,10 +1,7 @@
-Metadata-Version: 2.1 Name: musicntwrk Version: 2.2.9 Summary: music as data,
-data as music Home-page: https://www.musicntwrk.com Author: Marco Buongiorno
-Nardelli Author-email: mbn@unt.edu License: UNKNOWN Description:
                                _[_m_u_s_i_c_n_t_w_r_k_ _l_o_g_o_]
                     ******** mmuussiicc aass ddaattaa,, ddaattaa aass mmuussiicc ********
        uunnlleeaasshhiinngg ddaattaa ttoooollss ffoorr mmuussiicc tthheeoorryy,, aannaallyyssiiss aanndd ccoommppoossiittiioonn
 
 A python library for pitch class set and rhythmic sequences classification and
 manipulation, the generation of networks in generalized music and sound spaces,
    deep learning algorithms for timbre recognition, and the sonification of
@@ -51,36 +48,33 @@
 github.com/marcobn/musicntwrk/blob/master/DOCS/ml_utils.md) - [plotting](https:
 //github.com/marcobn/musicntwrk/blob/master/DOCS/plotting.md) The most
 computationally intensive parts of the modules can be run on parallel
 processors using the MPI (Message Passing Interface) protocol. Communications
 are handled by two additional modules: `communications` and `load_balancing`.
 Since the user will never have to interact with these modules, we omit here a
 detailed description of their functions. ## Author **Marco Buongiorno
-Nardelli** Marco Buongiorno Nardelli is University Distinguished Research
-Professor at the University of North Texas: composer, flutist, computational
-materials physicist, and a member of CEMI, the Center for Experimental Music
-and Intermedia, and iARTA, the Initiative for Advanced Research in Technology
-and the Arts. He is a Fellow of the American Physical Society and of the
-Institute of Physics, and a Parma Recordings artist. See [here](https://
-www.materialssoundmusic.com/long-bio) for a longer bio-sketch. ## Citation
-Marco Buongiorno Nardelli, _"musicntwrk, a python library for pitch class set
-and rhythmic sequences classification and manipulation, the generation of
-networks in generalized music and sound spaces, deep learning algorithms for
-timbre recognition, and the sonification of arbitrary data"_,
-www.musicntwrk.com (2019). ## Thanks This project has been made possible by
-contributions from the following institutions:
+Nardelli** Marco Buongiorno Nardelli is Regents Professor at the University of
+North Texas: composer, flutist, computational materials physicist, and a member
+of CEMI, the Center for Experimental Music and Intermedia, and iARTA, the
+Initiative for Advanced Research in Technology and the Arts. He is a Fellow of
+the American Physical Society and of the Institute of Physics, and a Parma
+Recordings artist. See [here](https://www.materialssoundmusic.com/long-bio) for
+a longer bio-sketch. ## Citation Marco Buongiorno Nardelli, _"musicntwrk, a
+python library for pitch class set and rhythmic sequences classification and
+manipulation, the generation of networks in generalized music and sound spaces,
+deep learning algorithms for timbre recognition, and the sonification of
+arbitrary data"_, www.musicntwrk.com (2019). ## Thanks This project has been
+made possible by contributions from the following institutions:
            _[_U_N_T_ _l_o_g_o_]    _[_C_E_M_I_ _l_o_g_o_]    _[_P_R_I_S_M_ _l_o_g_o_]   _[_I_M_e_R_A_ _l_o_g_o_]
 ===============================================================================
 mmuussiiccnnttwwrrkk is free software: you can redistribute it and/or modify it under the
    terms of the GNU General Public License as published by the Free Software
   Foundation, either version 3 of the License, or (at your option) any later
  version. This program is distributed in the hope that it will be useful, but
  WWIITTHHOOUUTT AANNYY WWAARRRRAANNTTYY; without even the implied warranty of MERCHANTABILITY or
  FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more
   details. You should have received a copy of the GNU General Public License
       along with this program. If not, see _h_t_t_p_:_/_/_w_w_w_._g_n_u_._o_r_g_/_l_i_c_e_n_s_e_s_/.
               Copyright (C) 2018-2020 Marco Buongiorno Nardelli
                          _w_w_w_._m_a_t_e_r_i_a_l_s_s_o_u_n_d_m_u_s_i_c_._c_o_m_ 
                               _w_w_w_._m_u_s_i_c_n_t_w_r_k_._c_o_m_ 
                                   _m_b_n_@_u_n_t_._e_d_u
-Platform: OS independent Description-Content-Type: text/markdown Provides-
-Extra: with_MPI
```

### Comparing `musicntwrk-2.2.9/README.md` & `musicntwrk-2.3.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,36 @@
+Metadata-Version: 2.1
+Name: musicntwrk
+Version: 2.3.0
+Summary: music as data, data as music
+Home-page: https://www.musicntwrk.com
+Author: Marco Buongiorno Nardelli
+Author-email: mbn@unt.edu
+Platform: OS independent
+Description-Content-Type: text/markdown
+Requires-Dist: numpy
+Requires-Dist: scipy
+Requires-Dist: pandas
+Requires-Dist: python-louvain
+Requires-Dist: networkx
+Requires-Dist: music21
+Requires-Dist: librosa
+Requires-Dist: numba
+Requires-Dist: pyo
+Requires-Dist: matplotlib
+Requires-Dist: tensorflow
+Requires-Dist: powerlaw
+Requires-Dist: vpython
+Requires-Dist: wget
+Requires-Dist: PySimpleGUI
+Requires-Dist: pydub
+Requires-Dist: ruptures
+Provides-Extra: with-mpi
+Requires-Dist: mpi4py; extra == "with-mpi"
+
 <p></p>
 <p align="center">
   <a href="https://www.musicntwrk.com">
     <img src="https://raw.githubusercontent.com/marcobn/musicntwrk/master/IMAGES/logo.png" alt="musicntwrk logo" height="84">
   </a>
 </p>
 
@@ -62,15 +91,15 @@
 
 The most computationally intensive parts of the modules can be run on parallel processors using the MPI (Message Passing Interface) protocol. Communications are handled by two additional modules: `communications` and `load_balancing`. Since the user will never have to interact with these modules, we omit here a detailed description of their functions.
 
 ## Author
 
 **Marco Buongiorno Nardelli**
 
-Marco Buongiorno Nardelli is University Distinguished Research Professor at the University of North Texas: composer, flutist, computational materials physicist, and a member of CEMI, the Center for Experimental Music and Intermedia, and iARTA, the Initiative for Advanced Research in Technology and the Arts. He is a Fellow of the American Physical Society and of the Institute of Physics, and a Parma Recordings artist. See [here](https://www.materialssoundmusic.com/long-bio) for a longer bio-sketch.
+Marco Buongiorno Nardelli is Regents Professor at the University of North Texas: composer, flutist, computational materials physicist, and a member of CEMI, the Center for Experimental Music and Intermedia, and iARTA, the Initiative for Advanced Research in Technology and the Arts. He is a Fellow of the American Physical Society and of the Institute of Physics, and a Parma Recordings artist. See [here](https://www.materialssoundmusic.com/long-bio) for a longer bio-sketch.
 
 ## Citation
 
 Marco Buongiorno Nardelli, _"musicntwrk, a python library for pitch class set and rhythmic sequences classification and manipulation, the generation of networks in generalized music and sound spaces, deep learning algorithms for timbre recognition, and the sonification of arbitrary data"_, www.musicntwrk.com (2019).
 
 ## Thanks
```

#### html2text {}

```diff
@@ -1,7 +1,17 @@
+Metadata-Version: 2.1 Name: musicntwrk Version: 2.3.0 Summary: music as data,
+data as music Home-page: https://www.musicntwrk.com Author: Marco Buongiorno
+Nardelli Author-email: mbn@unt.edu Platform: OS independent Description-
+Content-Type: text/markdown Requires-Dist: numpy Requires-Dist: scipy Requires-
+Dist: pandas Requires-Dist: python-louvain Requires-Dist: networkx Requires-
+Dist: music21 Requires-Dist: librosa Requires-Dist: numba Requires-Dist: pyo
+Requires-Dist: matplotlib Requires-Dist: tensorflow Requires-Dist: powerlaw
+Requires-Dist: vpython Requires-Dist: wget Requires-Dist: PySimpleGUI Requires-
+Dist: pydub Requires-Dist: ruptures Provides-Extra: with-mpi Requires-Dist:
+mpi4py; extra == "with-mpi"
                                _[_m_u_s_i_c_n_t_w_r_k_ _l_o_g_o_]
                     ******** mmuussiicc aass ddaattaa,, ddaattaa aass mmuussiicc ********
        uunnlleeaasshhiinngg ddaattaa ttoooollss ffoorr mmuussiicc tthheeoorryy,, aannaallyyssiiss aanndd ccoommppoossiittiioonn
 
 A python library for pitch class set and rhythmic sequences classification and
 manipulation, the generation of networks in generalized music and sound spaces,
    deep learning algorithms for timbre recognition, and the sonification of
@@ -48,27 +58,26 @@
 github.com/marcobn/musicntwrk/blob/master/DOCS/ml_utils.md) - [plotting](https:
 //github.com/marcobn/musicntwrk/blob/master/DOCS/plotting.md) The most
 computationally intensive parts of the modules can be run on parallel
 processors using the MPI (Message Passing Interface) protocol. Communications
 are handled by two additional modules: `communications` and `load_balancing`.
 Since the user will never have to interact with these modules, we omit here a
 detailed description of their functions. ## Author **Marco Buongiorno
-Nardelli** Marco Buongiorno Nardelli is University Distinguished Research
-Professor at the University of North Texas: composer, flutist, computational
-materials physicist, and a member of CEMI, the Center for Experimental Music
-and Intermedia, and iARTA, the Initiative for Advanced Research in Technology
-and the Arts. He is a Fellow of the American Physical Society and of the
-Institute of Physics, and a Parma Recordings artist. See [here](https://
-www.materialssoundmusic.com/long-bio) for a longer bio-sketch. ## Citation
-Marco Buongiorno Nardelli, _"musicntwrk, a python library for pitch class set
-and rhythmic sequences classification and manipulation, the generation of
-networks in generalized music and sound spaces, deep learning algorithms for
-timbre recognition, and the sonification of arbitrary data"_,
-www.musicntwrk.com (2019). ## Thanks This project has been made possible by
-contributions from the following institutions:
+Nardelli** Marco Buongiorno Nardelli is Regents Professor at the University of
+North Texas: composer, flutist, computational materials physicist, and a member
+of CEMI, the Center for Experimental Music and Intermedia, and iARTA, the
+Initiative for Advanced Research in Technology and the Arts. He is a Fellow of
+the American Physical Society and of the Institute of Physics, and a Parma
+Recordings artist. See [here](https://www.materialssoundmusic.com/long-bio) for
+a longer bio-sketch. ## Citation Marco Buongiorno Nardelli, _"musicntwrk, a
+python library for pitch class set and rhythmic sequences classification and
+manipulation, the generation of networks in generalized music and sound spaces,
+deep learning algorithms for timbre recognition, and the sonification of
+arbitrary data"_, www.musicntwrk.com (2019). ## Thanks This project has been
+made possible by contributions from the following institutions:
            _[_U_N_T_ _l_o_g_o_]    _[_C_E_M_I_ _l_o_g_o_]    _[_P_R_I_S_M_ _l_o_g_o_]   _[_I_M_e_R_A_ _l_o_g_o_]
 ===============================================================================
 mmuussiiccnnttwwrrkk is free software: you can redistribute it and/or modify it under the
    terms of the GNU General Public License as published by the Free Software
   Foundation, either version 3 of the License, or (at your option) any later
  version. This program is distributed in the hope that it will be useful, but
  WWIITTHHOOUUTT AANNYY WWAARRRRAANNTTYY; without even the implied warranty of MERCHANTABILITY or
```

### Comparing `musicntwrk-2.2.9/musicntwrk.egg-info/SOURCES.txt` & `musicntwrk-2.3.0/musicntwrk.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 README.md
+pyproject.toml
 setup.py
 musicntwrk.egg-info/PKG-INFO
 musicntwrk.egg-info/SOURCES.txt
 musicntwrk.egg-info/dependency_links.txt
 musicntwrk.egg-info/requires.txt
 musicntwrk.egg-info/top_level.txt
 src/__init__.py
 src/musicntwrk.py
 src/comptools/MidiFile.py
+src/comptools/displayNotes.py
 src/comptools/genmidi.py
 src/comptools/music.py
 src/comptools/notation.py
 src/data/MIDImap.py
 src/data/MIDImidi.py
 src/data/MIDIscore.py
 src/data/WRITEscore.py
@@ -60,15 +62,34 @@
 src/ml_utils/modelLoad.py
 src/ml_utils/multiModelPredictor.py
 src/ml_utils/prepareDataSet.py
 src/ml_utils/readModels.py
 src/ml_utils/scaleDataSet.py
 src/ml_utils/trainCNNmodel.py
 src/ml_utils/trainNNmodel.py
+src/msctools/base.py
+src/msctools/cfg.py
+src/msctools/converters.py
+src/msctools/decorators.py
+src/msctools/devices.py
+src/msctools/dictionaries.py
+src/msctools/dsp.py
+src/msctools/envelopes.py
+src/msctools/networks.py
+src/msctools/oscserver.py
+src/msctools/osctools.py
+src/msctools/pan.py
+src/msctools/players.py
+src/msctools/pyoPlayer.py
+src/msctools/pyotools.py
+src/msctools/session.py
+src/msctools/utils.py
+src/msctools/videocapture.py
 src/networks/__init__.py
+src/networks/analysisNetwork.py
 src/networks/orchestralNetwork.py
 src/networks/orchestralVector.py
 src/networks/orchestralVectorColor.py
 src/networks/pcsDictionary.py
 src/networks/pcsEgoNetwork.py
 src/networks/pcsNetwork.py
 src/networks/rLeadNetwork.py
@@ -85,19 +106,21 @@
 src/networks/vLeadNetworkByName.py
 src/networks/vLeadNetworkByNameVec.py
 src/networks/vLeadNetworkVec.py
 src/plotting/barplot.py
 src/plotting/chordspace.py
 src/plotting/drawMultiLayerNetwork.py
 src/plotting/drawNetwork.py
+src/plotting/drawNetwork3D.py
 src/plotting/drawNetworkViz.py
 src/plotting/drawNetworkX.py
 src/plotting/plotCC.py
 src/plotting/plotCurveXY.py
 src/plotting/plotCurveY.py
+src/plotting/plotDegreeAnalysis.py
 src/plotting/plotOpsHistogram.py
 src/timbre/__init__.py
 src/timbre/computeASCBW.py
 src/timbre/computeCompMPS.py
 src/timbre/computeMFCC.py
 src/timbre/computeModifiedASCBW.py
 src/timbre/computePSCC.py
```

### Comparing `musicntwrk-2.2.9/setup.py` & `musicntwrk-2.3.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -19,23 +19,25 @@
 this_directory = './'
 #with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
 with open(path.join(this_directory, 'README.md')) as f:
 	long_description = f.read()
 
 
 setup(name='musicntwrk',
-	version='2.2.9',
+
+	version='2.3.0',
+
 	description='music as data, data as music',
 	long_description=long_description,
 	long_description_content_type='text/markdown',
 	author='Marco Buongiorno Nardelli',
 	author_email='mbn@unt.edu',
 	platforms='OS independent',
 	url='https://www.musicntwrk.com',
 	packages=['musicntwrk', 'musicntwrk.data','musicntwrk.harmony','musicntwrk.ml_utils','musicntwrk.networks','musicntwrk.plotting',
-		'musicntwrk.timbre','musicntwrk.utils','musicntwrk.comptools'],
+		'musicntwrk.timbre','musicntwrk.utils','musicntwrk.comptools','musicntwrk.msctools'],
 	package_dir={'musicntwrk':'src'},
 	install_requires=['numpy','scipy','pandas','python-louvain','networkx','music21','librosa','numba','pyo',
 		'matplotlib','tensorflow','powerlaw','vpython','wget','PySimpleGUI','pydub','ruptures'],
 	extras_require=extras
 )
```

### Comparing `musicntwrk-2.2.9/src/comptools/MidiFile.py` & `musicntwrk-2.3.0/src/comptools/MidiFile.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.9/src/comptools/genmidi.py` & `musicntwrk-2.3.0/src/comptools/genmidi.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.9/src/comptools/music.py` & `musicntwrk-2.3.0/src/comptools/music.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import collections
+from collections.abc import MutableSequence, Iterable
 import copy
 from .notation import parse_note, parse_notes
 
 
 class MusiclibError(Exception):
     pass
 
@@ -99,15 +99,15 @@
         note_value = (2 * index) - value
         return Note(note_value, octv, self.dur, self.volume)
 
     def stretch_dur(self, factor):
         return Note(self.value, self.octave, self.dur * factor, self.volume)
 
 
-class NoteSeq(collections.MutableSequence):
+class NoteSeq(MutableSequence):
     @staticmethod
     def _is_note_or_rest(args):
         return all([True if isinstance(x, Note) or isinstance(x, Rest) else False for x in args])
 
     @staticmethod
     def _make_note_or_rest(note_list):
         if note_list[0] is not None:
@@ -127,15 +127,15 @@
         if isinstance(args, str):
             if args.startswith("file://"):
                 filename = args.replace("file://", "")
                 note_lists = parse_notes(self._parse_score(filename))
             else:
                 note_lists = parse_notes(args.split())
             self.items = [self._make_note_or_rest(x) for x in note_lists]
-        elif isinstance(args, collections.Iterable):
+        elif isinstance(args, Iterable):
             if self._is_note_or_rest(args):
                 self.items = args
             else:
                 raise MusiclibError("Every argument have to be a Note or a Rest.")
         elif args is None:
             self.items = []
         else:
```

### Comparing `musicntwrk-2.2.9/src/comptools/notation.py` & `musicntwrk-2.3.0/src/comptools/notation.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.9/src/data/MIDImap.py` & `musicntwrk-2.3.0/src/data/MIDImap.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.9/src/data/MIDImidi.py` & `musicntwrk-2.3.0/src/data/MIDImidi.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.9/src/data/MIDIscore.py` & `musicntwrk-2.3.0/src/data/MIDIscore.py`

 * *Files 19% similar despite different names*

```diff
@@ -11,19 +11,22 @@
 # GNU General Public License. See the file `License'
 # in the root directory of the present distribution,
 # or http://www.gnu.org/copyleft/gpl.txt .
 #
 
 import music21 as m21
 
-def MIDIscore(yvf,dur=2,w=None,outxml='./music',outmidi='./music'):
+def MIDIscore(yvf,dvf=None,dur=2,w=None,outxml='./music',outmidi='./music'):
 	s1 = m21.stream.Stream()
 	for i in range(yvf.shape[0]):
 		n = m21.note.Note(yvf[i])
-		n.duration = m21.duration.Duration((abs(yvf[i]-yvf[i-1])+1)/dur)
+		try:
+			n.duration = m21.duration.Duration(dvf[i])
+		except:
+			n.duration = m21.duration.Duration((abs(yvf[i]-yvf[i-1])+1)/dur)
 		s1.append(n)
 	if w == 'musicxml':
 		s1.write('musicxml',outxml+'.xml')
 	elif w == 'MIDI':
 		s1.write('midi',outmidi+'.mid')
 	else:
 		s1.show()
```

### Comparing `musicntwrk-2.2.9/src/data/WRITEscore.py` & `musicntwrk-2.3.0/src/data/WRITEscore.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.9/src/data/WRITEscoreNoTime.py` & `musicntwrk-2.3.0/src/data/WRITEscoreNoTime.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.9/src/data/WRITEscoreOps.py` & `musicntwrk-2.3.0/src/data/WRITEscoreOps.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,26 +16,30 @@
 import music21 as m21
 import numpy as np
 
 from ..utils.generalizedOpsName import generalizedOpsName
 from ..utils.opsName import opsName
 
 def WRITEscoreOps(nseq,w=None,outxml='./music',outmidi='./music',keysig=None,abs=False,TET=12,distance='euclidean'):
+    fac = TET/12
     try:
         ntot = nseq.shape[0]
     except:
         ntot = len(nseq)
     m = m21.stream.Stream()
     m.append(m21.meter.TimeSignature('4/4'))
     for i in range(ntot):
         ch = np.copy(nseq[i])
         for n in range(1,len(ch)):
             if ch[n] < ch[n-1]: ch[n] += 12
         ch += 60
-        n = m21.chord.Chord(ch.tolist())
+        c = []
+        for k in range(len(ch)):
+            c.append(m21.note.Note(ch[k]/fac))
+        n = m21.chord.Chord(c)
         if i < ntot-1: 
             n.addLyric(str(i)+' '+generalizedOpsName(nseq[i],nseq[i+1],TET,distance)[1])
             if abs:
                 if len(nseq[i]) == len(nseq[i+1]):
                     n.addLyric(str(i)+' '+opsName(nseq[i],nseq[i+1]))
                 else:
                     r = generalizedOpsName(nseq[i],nseq[i+1],TET,distance)[0]
@@ -48,8 +52,8 @@
             n.addLyric(str(rn.figure))
         m.append(n)    
     if w == True:
         m.show('musicxml')
     elif w == 'MIDI':
         m.write('midi',outmidi+'.mid')
     else:
-        m.show()
+        m.show()
```

### Comparing `musicntwrk-2.2.9/src/data/WRITEscoreOpsMIDI.py` & `musicntwrk-2.3.0/src/data/WRITEscoreOpsMIDI.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.9/src/data/analyzeSound.py` & `musicntwrk-2.3.0/src/data/analyzeSound.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,23 +27,23 @@
 def analyzeSound(soundfile,outlist,plot=True,crm=True,tms=True,xml=False):
     var = {}        
     # load soundfile
     y, sr = librosa.load(soundfile)
     var['y'] = y
     var['sr'] = sr
     # analyze onsets
-    o_env = librosa.onset.onset_strength(y, sr=sr)
+    o_env = librosa.onset.onset_strength(y=y, sr=sr)
     times = librosa.frames_to_time(np.arange(len(o_env)), sr=sr)
     onset_frames = librosa.onset.onset_detect(onset_envelope=o_env, sr=sr)
     var['onset_frames'] = onset_frames
     var['times'] = times
     if plot:
         plt.figure(figsize=(18,8))
         ax1 = plt.subplot(2, 1, 1)
-        librosa.display.waveplot(y[:])
+        librosa.display.waveshow(y[:])
         plt.title('Waveshape')
         plt.subplot(2, 1, 2, sharex=ax1)
         plt.plot(times, o_env, label='Onset strength')
         plt.vlines(times[onset_frames], 0, o_env.max(), color='r', alpha=0.9,linestyle='--', label='Onsets')
         plt.axis('tight')
         plt.legend(frameon=True, framealpha=0.75)
     p = None
```

### Comparing `musicntwrk-2.2.9/src/data/analyzeTimbre.py` & `musicntwrk-2.3.0/src/data/analyzeTimbre.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 def analyzeTimbre(soundfile,outlist=[],zero=1.0e-10,plot=True,crm=True,tms=True,xml=False,mps=True):
     var = {}        
     # load soundfile
     y, sr = librosa.load(soundfile)
     var['y'] = y
     var['sr'] = sr
     # analyze onsets
-    o_env = librosa.onset.onset_strength(y, sr=sr)
+    o_env = librosa.onset.onset_strength(y=y, sr=sr)
     times = librosa.frames_to_time(np.arange(len(o_env)), sr=sr)
     onset_frames = librosa.onset.onset_detect(onset_envelope=o_env, sr=sr)
     var['onset_frames'] = onset_frames
     var['times'] = times
     # analyze decay constants and specral features
     maxsp = int(np.argwhere(np.abs(y) < zero)[0])
     a,alpha,t = normSoundDecay(y[onset_frames[0]:],sr)
@@ -45,15 +45,15 @@
     cent = librosa.feature.spectral_centroid(y=y, sr=sr,hop_length=maxsp)
     print('spectral centroid = ',cent[0][0])
     spec_bw = librosa.feature.spectral_bandwidth(y=y, sr=sr,hop_length=maxsp)
     print('spectral bandwidth = ',spec_bw[0][0])
     if plot:
         plt.figure(figsize=(18,8))
         ax1 = plt.subplot(2, 1, 1)
-        librosa.display.waveplot(y[:])
+        librosa.display.waveshow(y[:])
         plt.title('Waveshape')
         plt.subplot(2, 1, 2, sharex=ax1)
         plt.plot(times, o_env, label='Onset strength')
         plt.vlines(times[onset_frames], 0, o_env.max(), color='r', alpha=0.9,linestyle='--', label='Onsets')
         plt.axis('tight')
         plt.legend(frameon=True, framealpha=0.75)
     p = None
@@ -84,15 +84,15 @@
         beat = librosa.frames_to_time(onset_frames, sr=sr)
         beat = RHYTHMSeq((np.diff(beat)*16).round(0)/16,REF='e')
         var['beat'] = beat
         var['tempo'] = int(tempo[0])
         if plot: beat.displayRhythm(xml)
     if mps:
         # mel-scaled power (energy-squared) spectrogram
-        S = librosa.feature.melspectrogram(y, sr=sr, n_mels=16) #,hop_length=len(y))
+        S = librosa.feature.melspectrogram(y=y, sr=sr, n_mels=16) #,hop_length=len(y))
         # Convert to log scale (dB). We'll use the peak power (max) as reference.
         log_S = librosa.power_to_db(S, ref=np.max)
         librosa.display.specshow(log_S, sr=sr, x_axis='time', y_axis='mel')
         _,var['mfcc'],_ = computeMFCC('./',soundfile,nmel=16,ncc=13,zero=True)
     output = []
     for out in outlist:
         output.append(var[out])
```

### Comparing `musicntwrk-2.2.9/src/data/ctcsound.py` & `musicntwrk-2.3.0/src/data/ctcsound.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.9/src/data/i_spectral.py` & `musicntwrk-2.3.0/src/data/i_spectral.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.9/src/data/i_spectral2.py` & `musicntwrk-2.3.0/src/data/i_spectral2.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.9/src/data/i_spectral_pure.py` & `musicntwrk-2.3.0/src/data/i_spectral_pure.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.9/src/data/i_spectral_pyo.py` & `musicntwrk-2.3.0/src/data/i_spectral_pyo.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.9/src/data/i_time_series.py` & `musicntwrk-2.3.0/src/data/i_time_series.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.9/src/data/r_1Ddata.py` & `musicntwrk-2.3.0/src/data/r_1Ddata.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.9/src/data/scaleMapping.py` & `musicntwrk-2.3.0/src/data/scaleMapping.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.9/src/harmony/applyOps.py` & `musicntwrk-2.3.0/src/harmony/applyOps.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.9/src/harmony/changePoint.py` & `musicntwrk-2.3.0/src/harmony/changePoint.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.9/src/harmony/chinese_postman.py` & `musicntwrk-2.3.0/src/harmony/chinese_postman.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.9/src/harmony/enharmonicDictionary.py` & `musicntwrk-2.3.0/src/harmony/enharmonicDictionary.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.9/src/harmony/getRN.py` & `musicntwrk-2.3.0/src/harmony/getRN.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.9/src/harmony/harmonicDesign.py` & `musicntwrk-2.3.0/src/harmony/harmonicDesign.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.9/src/harmony/keySections.py` & `musicntwrk-2.3.0/src/harmony/keySections.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # or http://www.gnu.org/copyleft/gpl.txt .
 #
 
 import numpy as np
 import pandas as pd
 import music21 as m21
 
-def keySections(sections,GxsecDi,dnodes):
+def keySections(sections,GxsecDi,dnodes,measure=None):
     # key identification in the different regions
     # this is based on the ansatz that the tonic triad is the most connected (highest degree) 
     # node of the region's network
     prevalent_key = []
     for n in range(len(sections)-1):
         prevalent_chord = str(dnodes.set_index("Label", drop = True).\
                                 iloc[int(sorted((value, key) for (key,value) in GxsecDi[n].degree)[-1][1])]).split()[2].replace(",","")
@@ -46,16 +46,24 @@
             key.append(str(n.root()))
         elif n.isMinorTriad():
             key.append(str(n.root()).lower())
         elif n.isDominantSeventh():
             key.append(str(n.getChordStep(3).transpose(1).name))
         else:
             key.append(str(n.root()))
-            
-    keySections = pd.DataFrame(None,columns=['Section','chord range','prevalent_chord','region'])
-    for i in range(len(key)):    
-        tmp = pd.DataFrame([[str(i),str(sections[i])+'-'+str(sections[i+1])
-                            ,str(prevalent_key[i].pitchNames),key[i]]],
-                            columns=['Section','chord range','prevalent_chord','region'])
-        keySections = keySections.append(tmp)
+    
+    if measure != None:
+        keySections = pd.DataFrame(None,columns=['Section','measures','prevalent_chord','region'])
+        for i in range(len(key)):    
+            tmp = pd.DataFrame([[str(i),str(np.asarray(fmeasure)[sections[i]])+'-'+str(np.asarray(fmeasure)[sections[i+1]])
+                                ,str(prevalent_key[i].pitchNames),key[i]]],
+                                columns=['Section','measures','prevalent_chord','region'])
+            keySections = keySections.append(tmp)
+    else:
+        keySections = pd.DataFrame(None,columns=['Section','chord range','prevalent_chord','region'])
+        for i in range(len(key)):    
+            tmp = pd.DataFrame([[str(i),str(sections[i])+'-'+str(sections[i+1])
+                                ,str(prevalent_key[i].pitchNames),key[i]]],
+                                columns=['Section','chord range','prevalent_chord','region'])
+            keySections = keySections.append(tmp)
 
     return(key,keySections)
```

### Comparing `musicntwrk-2.2.9/src/harmony/lookupOps.py` & `musicntwrk-2.3.0/src/harmony/lookupOps.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.9/src/harmony/lookupProgr.py` & `musicntwrk-2.3.0/src/harmony/lookupProgr.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.9/src/harmony/lookupWrapper.py` & `musicntwrk-2.3.0/src/harmony/lookupWrapper.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.9/src/harmony/networkHarmonyGen.py` & `musicntwrk-2.3.0/src/harmony/networkHarmonyGen.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,10 +45,11 @@
         if len(names) != len(probs):
             print('names not matching probabilities!')
         else:
             for n in range(len(names)):
                 nodes,dedges = mk.network(space='vLead',ops=True,name=names[n],
                                            pcslabel=True,dictionary=dictionary,distance=distance,
                                            prob=probs[n],write=False)
-                edges = edges.append(dedges)
+#               edges = edges.append(dedges)
+                edges = pd.concat([edges,dedges],ignore_index=True)
 
     return(nodes,edges)
```

### Comparing `musicntwrk-2.2.9/src/harmony/plotHarmonicTable.py` & `musicntwrk-2.3.0/src/harmony/plotHarmonicTable.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.9/src/harmony/rhythmicDesign.py` & `musicntwrk-2.3.0/src/harmony/rhythmicDesign.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,28 +19,28 @@
 
 from ..musicntwrk import RHYTHMSeq
 from ..harmony.chinese_postman import chinese_postman
 from ..utils.floatize import floatize
 
 
 def rhythmicDesign(dictionary,nnodes,nedges,refnodes,refedges,nstart=None,seed=None,reverse=None,
-                   random=None):
+                   random=None,write=False):
     # network generator (see documentation on networkx)
     scfree = nx.barabasi_albert_graph(nnodes,nedges,seed)
     # node degree distribution
     node = np.zeros((nnodes),dtype=int)
     weight = np.zeros((nnodes),dtype=int)
     for n in range(nnodes):
         node[n] = np.array(scfree.degree())[n][0]
         weight[n] = np.array(scfree.degree())[n][1]
     idx = np.argsort(weight)[::-1]
     if nstart == None:
         nstart = idx[0]
     euler_circuit = chinese_postman(scfree,nstart)
-    print('Length of Eulerian circuit: {}'.format(len(euler_circuit)))
+    if write: print('Length of Eulerian circuit: {}'.format(len(euler_circuit)))
     # reference node degree distribution
     try:
         bnet = nx.from_pandas_edgelist(refedges,'Source','Target',['Weight','Label'])
     except:
         bnet = nx.from_pandas_edgelist(refedges,'Source','Target',['Weight'])
     bnode = np.zeros((nnodes),dtype=int)
     bweight = np.zeros((nnodes),dtype=int)
@@ -55,17 +55,17 @@
     # write score
     dict_cell = dictionary.set_index("cell", drop = True)
     eulerseq = []
     for i in range(len(euler_circuit)):
         label = np.asarray(refnodes)[eudict[int(euler_circuit[i][0])]].tolist()[0]
         if random:
             dur = RHYTHMSeq(np.random.permutation(list(map(floatize,list(map(
-                    lambda x: fr.Fraction(x),dict_cell.loc[label][0].split())))))).rseq
+                    lambda x: fr.Fraction(x),dict_cell.loc[label].iloc[0].split())))))).rseq
         else:
             dur = RHYTHMSeq(np.array(list(map(floatize,list(map(
-                    lambda x: fr.Fraction(x),dict_cell.loc[label][0].split())))))).rseq
+                    lambda x: fr.Fraction(x),dict_cell.loc[label].iloc[0].split())))))).rseq
         for j in range(len(dur)):
             eulerseq.append(m21.duration.Duration(4*dur[j]))
 
     if reverse: eulerseq = eulerseq[::-1]
 
     return(eulerseq)
```

### Comparing `musicntwrk-2.2.9/src/harmony/scoreAnalysis.py` & `musicntwrk-2.3.0/src/harmony/scoreAnalysis.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.9/src/harmony/scoreDesign.py` & `musicntwrk-2.3.0/src/harmony/scoreDesign.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.9/src/harmony/scoreFilter.py` & `musicntwrk-2.3.0/src/harmony/scoreFilter.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.9/src/harmony/shortHands.py` & `musicntwrk-2.3.0/src/harmony/shortHands.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.9/src/harmony/showAnalysis.py` & `musicntwrk-2.3.0/src/harmony/showAnalysis.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.9/src/harmony/spiralChordSpace.py` & `musicntwrk-2.3.0/src/harmony/spiralChordSpace.py`

 * *Files 7% similar despite different names*

```diff
@@ -106,27 +106,28 @@
 #     build the network
     df = np.asarray(dictionary)
 #     nodes
     dnodes = pd.DataFrame(None,columns=['Label'])
     for n in range(len(df)):
         s = ','
         p = s.join(df[n,0])
-        dnodes = dnodes.append(pd.DataFrame([[str(p)]],columns=['Label']))
+#       dnodes = dnodes.append(pd.DataFrame([[str(p)]],columns=['Label']))
+        dnodes = pd.concat([dnodes,pd.DataFrame([[str(p)]],columns=['Label'])],ignore_index=True)
 
 #     edges according to a metric
     thup = np.sqrt(thup)
 
     N = df[:,1].shape[0]
     dedges = pd.DataFrame(None,columns=['Source','Target','Weight','Label'])
     for i in range(N):
         a  = np.asarray(df[i,1])
         for j in range(i,N):
             b  = np.asarray(df[j,1])
             pair = sklm.pairwise_distances(a.reshape(1, -1),b.reshape(1, -1),metric=distance)[0]
             if pair <= thup and pair >= thdw:
                 tmp = pd.DataFrame([[str(i),str(j),str(1/pair[0]),str(int(np.round(pair[0]**2,0)))]],
                                    columns=['Source','Target','Weight','Label'])
-                dedges = dedges.append(tmp)
+                dedges = pd.concat([dedges,tmp],ignore_index=True)
     
     Gxu = nx.from_pandas_edgelist(dedges,'Source','Target',['Weight','Label'])
     
     return(dictionary,dnodes,dedges,Gxu)
```

### Comparing `musicntwrk-2.2.9/src/harmony/tonalAnalysis.py` & `musicntwrk-2.3.0/src/harmony/tonalAnalysis.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.9/src/harmony/tonalHarmonyCalculator.py` & `musicntwrk-2.3.0/src/harmony/tonalHarmonyCalculator.py`

 * *Files 0% similar despite different names*

```diff
@@ -69,15 +69,15 @@
             print('tonal model - is the table that stores the operators that connect every chord of a chosen tonal model')
             print('(in roman numeral form).')
             print('The chords that are included in the model can be chosen in tonalHarmonyModels that produces the final')
             print('table. it is read by clicking on "Submit".')
             print('A minimal model can be downloaded from')
             print('https://github.com/marcobn/musicntwrk/tree/master/musicntwrk-2.0/examples')
             print('')
-            print('The next set of enties depend on the action that is requested by the user. They can be filled with:')
+            print('The next set of entries depend on the action that is requested by the user. They can be filled with:')
             print('')
             print('operator - voice leading operator as O(i,j,k,...) ')
             print('')
             print('initial chord - chord in roman numeral or pcs as list of integers')
             print('')
             print('final chord - chord in roman numeral or pcs as list of integers or key as letter (A,a,C#, Bb etc.)')
             print('')
```

### Comparing `musicntwrk-2.2.9/src/harmony/tonalHarmonyModels.py` & `musicntwrk-2.3.0/src/harmony/tonalHarmonyModels.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.9/src/harmony/tonalPartition.py` & `musicntwrk-2.3.0/src/harmony/tonalPartition.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.9/src/harmony/tonnentz.py` & `musicntwrk-2.3.0/src/harmony/tonnentz.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.9/src/ml_utils/checkRun.py` & `musicntwrk-2.3.0/src/ml_utils/checkRun.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # GNU General Public License. See the file `License'
 # in the root directory of the present distribution,
 # or http://www.gnu.org/copyleft/gpl.txt .
 #
 
 import matplotlib.pyplot as plt
 import matplotlib.style as ms
-ms.use('seaborn-muted')
+ms.use('seaborn-v0_8-muted')
 
 def checkRun(train,modelfiles):
     # plot accuracy and loss for training and validation sets over epochs
     try:
         try:
             accuracy = train.history['accuracy']
             val_accuracy = train.history['val_accuracy']
```

### Comparing `musicntwrk-2.2.9/src/ml_utils/modelDump.py` & `musicntwrk-2.3.0/src/ml_utils/modelDump.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,24 +15,24 @@
 
 import os, pickle, time
 import numpy as np
 import joblib as jlib
 
 def modelDump(model,x_train,y_train,x_test,y_test,scaler,normal,res,train):
     filename = str(hex(int(time.time())))+'_'+str(round(res,3))
-    model.save(filename+'.h5')
+    model.save(filename+'.keras')
     np.save(filename+'.test',x_test)
     np.save(filename+'.name_test',y_test)
     np.save(filename+'.train',x_train)
     np.save(filename+'.name_train',y_train)
     jlib.dump(scaler, filename+'.scaler') 
     jlib.dump(normal, filename+'.normal')
     with open(filename+'.train.dict','wb') as file_pi:
         pickle.dump(train.history, file_pi)
     os.system('tar cvf '+filename+'.tar '+filename+'*')
-    os.system('rm '+filename+'.h5')
+    os.system('rm '+filename+'.keras')
     os.system('rm '+filename+'*.npy')
     os.system('rm '+filename+'.scaler')
     os.system('rm '+filename+'.normal')
     os.system('rm '+filename+'*.dict')
     print('model saved in ',filename)
```

### Comparing `musicntwrk-2.2.9/src/ml_utils/modelLoad.py` & `musicntwrk-2.3.0/src/ml_utils/modelLoad.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,19 +11,19 @@
 # GNU General Public License. See the file `License'
 # in the root directory of the present distribution,
 # or http://www.gnu.org/copyleft/gpl.txt .
 #
 
 import pickle
 import joblib as jlib
-import tensorflow as tf
+from tensorflow import keras
 import numpy as np
-
+ 
 def modelLoad(filename,npy=False):
-    model = tf.keras.models.load_model(filename+'.h5')
+    model = keras.models.load_model(filename+'.keras')
     scaler = jlib.load(filename+'.scaler') 
     normal = jlib.load(filename+'.normal')
     try:
         with open(filename+'.train.dict','rb') as file_pi:
             trdict=pickle.load(file_pi)
     except:
         try:
```

### Comparing `musicntwrk-2.2.9/src/ml_utils/multiModelPredictor.py` & `musicntwrk-2.3.0/src/ml_utils/multiModelPredictor.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.9/src/ml_utils/prepareDataSet.py` & `musicntwrk-2.3.0/src/ml_utils/prepareDataSet.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.9/src/ml_utils/readModels.py` & `musicntwrk-2.3.0/src/ml_utils/readModels.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,42 +16,42 @@
 import os, glob, tarfile
 from .modelLoad import modelLoad
 
 def readModels(path,filename):
 
     def extract_files(members):
         for tarinfo in members:
-            if os.path.splitext(tarinfo.name)[1] == ".h5": 
+            if os.path.splitext(tarinfo.name)[1] == ".keras": 
                 yield tarinfo
             elif os.path.splitext(tarinfo.name)[1] == ".normal":
                 yield tarinfo
             elif os.path.splitext(tarinfo.name)[1] == ".scaler":
                 yield tarinfo
             elif os.path.splitext(tarinfo.name)[1] == ".dict":
                 yield tarinfo
-
+ 
     # extract data from tar files
     tar_files = list(glob.glob(os.path.join(path,filename)))
     for file in tar_files:
         tar = tarfile.open(file)
         member=extract_files(tar)
         tar.extractall(members=member)
         tar.close()
 
     # load model parameters, scaler and normalizer for each model
-    modelfiles = list(glob.glob(os.path.join(path,'*.h5')))
+    modelfiles = list(glob.glob(os.path.join(path,'*.keras')))
     ynew = []
     models = {}
     scalers = {}
     normals = {}
     trdicts = {}
     n = 0 
     for file in modelfiles:
         try:
-            models[str(n)],scalers[str(n)],normals[str(n)],trdicts[str(n)] = modelLoad(str(file[+2:-3]))
+            models[str(n)],scalers[str(n)],normals[str(n)],trdicts[str(n)] = modelLoad(str(file[+2:-6]))
         except:
-            models[str(n)],scalers[str(n)],normals[str(n)] = modelLoad(str(file[+2:-3]))
+            models[str(n)],scalers[str(n)],normals[str(n)] = modelLoad(str(file[+2:-6]))
             trdicts[str(n)] = None
         n += 1
-        os.system('rm '+str(file[+2:-3])+'.h5 '+str(file[+2:-3])+'.scaler '+str(file[+2:-3])+'.normal '+str(file[+2:-3])+'.train.dict')
+        os.system('rm '+str(file[+2:-6])+'.keras '+str(file[+2:-6])+'.scaler '+str(file[+2:-6])+'.normal '+str(file[+2:-6])+'.train.dict')
     return(models,scalers,normals,trdicts,modelfiles)
```

### Comparing `musicntwrk-2.2.9/src/ml_utils/scaleDataSet.py` & `musicntwrk-2.3.0/src/ml_utils/scaleDataSet.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.9/src/ml_utils/trainCNNmodel.py` & `musicntwrk-2.3.0/src/ml_utils/trainCNNmodel.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 
 import numpy as np
 
 from tensorflow.keras.models import Sequential,Model
 from tensorflow.keras.layers import Dense, Dropout, Flatten
 from tensorflow.keras.layers import Conv2D, MaxPooling2D
 from tensorflow.keras.layers import LeakyReLU
+import tensorflow as tf
 
 from .modelDump import modelDump
 from .prepareDataSet import prepareDataSet
 
 def trainCNNmodel(mfcc,label,gpu=0,cpu=4,niter=100,nstep=10,neur=16,test=0.08,num_classes=2,
                                     epoch=30,verb=0,thr=0.85,w=False):
     # Convolutional NN
@@ -57,17 +58,18 @@
         model.add(Dropout(0.4))
         model.add(Flatten())
         model.add(Dense(4*nnn, activation='linear'))
         model.add(LeakyReLU(alpha=0.1))  
         model.add(Dropout(0.3))
         model.add(Dense(num_classes, activation='softmax'))
 
-        model.compile(optimizer='adam',
-                                    loss='sparse_categorical_crossentropy',
-                                    metrics=['accuracy'])
+        optimizer = tf.keras.optimizers.legacy.Adam(learning_rate=0.001)
+        model.compile(optimizer=optimizer,
+                      loss='sparse_categorical_crossentropy',
+                      metrics=['accuracy'])
 
         train = model.fit(x_train, y_train, epochs=epoch, verbose=verb,validation_data=(x_test,y_test))
 
         res = model.evaluate(x_test, y_test, verbose=0)
         print('loss ',res[0],'accuracy ',res[1])
         if res[1] >= thr and w == True:
             print('found good match ',round(res[1],3))
```

### Comparing `musicntwrk-2.2.9/src/ml_utils/trainNNmodel.py` & `musicntwrk-2.3.0/src/ml_utils/trainNNmodel.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,18 +36,18 @@
         model = tf.keras.models.Sequential([
             tf.keras.layers.Flatten(input_shape=shapedata),
             tf.keras.layers.Dense(nnn, activation=tf.nn.relu),
             tf.keras.layers.Dropout(0.3),
             tf.keras.layers.Dense(2*nnn, activation=tf.nn.relu),
             tf.keras.layers.Dropout(0.2),
             tf.keras.layers.Dense(num_classes, activation=tf.nn.softmax)])
-
-        model.compile(optimizer='adam',
-                                    loss='sparse_categorical_crossentropy',
-                                    metrics=['accuracy'])
+        optimizer = tf.keras.optimizers.legacy.Adam(learning_rate=0.001)
+        model.compile(optimizer=optimizer,
+                      loss='sparse_categorical_crossentropy',
+                      metrics=['accuracy'])
 
         train = model.fit(x_train, y_train, epochs=epoch, verbose=verb,validation_data=(x_test,y_test))
 
         res = model.evaluate(x_test, y_test, verbose=0)
         print('loss ',res[0],'accuracy ',res[1])
         if res[1] > thr and w == True:
             print('found good match ',round(res[1],3))
```

### Comparing `musicntwrk-2.2.9/src/musicntwrk.py` & `musicntwrk-2.3.0/src/musicntwrk.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 #
 # A python library for pitch class set and rhythmic sequences classification and manipulation, 
 # the generation of networks in generalized musical spaces, and the sonification of arbitrary data 
 # See documentation at www.musicntwrk.com
 #
 # Copyright (C) 2018,2019,2020,2021 Marco Buongiorno Nardelli http://www.materialssoundmusic.com, mbn@unt.edu
 # This file is distributed under the terms of the GNU General Public License. See the file `License' 
-#in the root directory of the present distribution, or http://www.gnu.org/copyleft/gpl.txt .
+# in the root directory of the present distribution, or http://www.gnu.org/copyleft/gpl.txt .
 #
 
 import re, sys, time
 import numpy as np
 import music21 as m21
 from functools import reduce
 import fractions as fr
@@ -742,14 +742,15 @@
                 Tr = Tr.tolist()
                 Pr = np.roll(np.linspace(0,length-1,length),-(length+double_transposition[1]))\
                     .astype(int).tolist()
                 if verbose: print('Tr = ',Tr,'  Pr = ',Pr)
             else:
                 pass
 
+        L = len(scala)
         if len(scala) == 1:
             scala = scala[0]
     
             idx = []
             for p in self.pitches:
                 try:
                     idx.append(np.argwhere(scala==p)[0][0])
@@ -782,28 +783,28 @@
                     return
             idx = np.array(idx)
     
             pitches = []
             for l in range(len(scala)):
                 pitches.append(PCmidiR([scala[l][idx[l]]]).midi[0])
             seq = [pitches]
-            for n in range(L):
+            for n in range(len(scala)):
                 idx += Tr
                 pitches = []
                 for l in range(len(scala)):
                     if mode == 0:
                         pitches.append(PCmidiR([scala[l][idx[Pr][l]]]).midi[0])
                     elif mode == 1:
                         pitches.append(PCmidiR([scala[Pr[l]][idx[Pr][l]]]).midi[0])
                     else:
                         print('mode not known')
                         return
                 seq.append(pitches)
                 idx = idx[Pr]
-            return(seq)
+            return(seq,idx)
     
     def displayNotes(self,show=True,xml=False,chord=False):
         '''
         •	Display pcs in score in musicxml format. If chord is True 
             displays the note cluster
         '''
         fac = self.TET/12
@@ -1190,15 +1191,15 @@
         reference.append(entry)
         entry = ['Q',(self.Q().pcs)]
         reference.append(entry)
         entry = ['M',(self.M().pcs)]
         reference.append(entry)
         star = pd.DataFrame(reference,columns=['Op','Row'])
         return(star)
-        
+
 class RHYTHMSeq:
 
     def __init__(self,rseq,REF='e',ORD=False):
         '''
         •	rseq (int)– rhythm sequence as list of strings/fractions/floats
         •	REF = reference duration for prime form (str)
         '''
@@ -1623,36 +1624,36 @@
     def sonify(self,descriptor=None,engine='pyo',data=None,length=None,midi=None,scalemap=None,ini=None,fin=None,
                fac=None,dur=None,transp=None,col=None,write=None,vnorm=None,plot=None,crm=None,tms=None,xml=None,
                sigpath=None,sigfil=None,firpath=None,firsig=None):
         '''
         sonification strategies - simple sound (spectral) or score (melodic progression)
         '''
         from .data.r_1Ddata import r_1Ddata
-        from .data.i_spectral_pyo import i_spectral_pyo
-        from .data.i_spectral import i_spectral
-        from .data.i_spectral2 import i_spectral2
-        from .data.i_spectral_pure import i_spectral_pure
-        
+
         if descriptor == 'spectrum':
             if engine == engine == 'pyo':
+                from .data.i_spectral_pyo import i_spectral_pyo
                 x, y = r_1Ddata(data)
                 s,a = i_spectral_pyo(x,y[0])
                 s.start()
                 time.sleep(length)
                 s.stop()
                 s.shutdown()
             elif engine == 'csound':
+                from .data.i_spectral import i_spectral
                 # Full csound
                 x, y = r_1Ddata(data)
                 i_spectral(x,y[0],itime=length)
             elif engine == 'csound+scipy':
+                from .data.i_spectral2 import i_spectral2
                 # csound + scipy for FIR
                 x, y = r_1Ddata(data)
                 i_spectral2(x,y[0],itime=length)
             elif engine == 'scipy':
+                from .data.i_spectral_pure import i_spectral_pure
                 # Full scipy
                 x, y = r_1Ddata(data)
                 s = i_spectral_pure(sigpath,sigfil,firpath,firsig)
                 return(s)
             else:
                 print('no engine specified for sound')
                 sts.exit()
@@ -1668,8 +1669,8 @@
             MIDIscore(MIDImap(y[col],scale,nnote)-transp,dur=dur,w=write)
             if midi: MIDImidi(MIDImap(y[col],scale,nnote)-transp,dur=2*dur,vnorm=vnorm)
         
         if descriptor == 'sound':
             from .data.analyzeSound import analyzeSound
             from .data.WRITEscore import WRITEscore
             nseq,beat,prob = analyzeSound(data,outlist=['nseq','beat','prob'],plot=plot,crm=crm,tms=tms,xml=xml)
-            WRITEscore(data,nseq.pcs,beat.rseq,w=write)
+            WRITEscore(data,nseq.pcs,beat.rseq,w=write)
```

### Comparing `musicntwrk-2.2.9/src/networks/orchestralNetwork.py` & `musicntwrk-2.3.0/src/networks/rLeadNetwork.py`

 * *Files 23% similar despite different names*

```diff
@@ -9,60 +9,67 @@
 #
 # This file is distributed under the terms of the
 # GNU General Public License. See the file `License'
 # in the root directory of the present distribution,
 # or http://www.gnu.org/copyleft/gpl.txt .
 #
 
+import time,re,os
 import numpy as np
+import fractions as fr
 import pandas as pd
-import networkx as nx
-import community as cm
 
-from ..utils.minimalDistance import minimalDistance
+from ..musicntwrk import RHYTHMSeq
+from ..utils.floatize import floatize
+from ..utils.rhythmDistance import rhythmDistance
 
-def orchestralNetwork(seq,distance,TET):
-    
-    ''' 
-    •    generates the directional network of orchestration vectors from any score in musicxml format
-    •    seq (int) – list of orchestration vectors extracted from the score
-    •    use orchestralScore() to import the score data as sequence
+def rLeadNetwork(dictionary,thup,thdw,distance,prob,write):
+        
+    '''
+    •	generation of the network of all minimal rhythm leadings in a generalized musical space of Nc-dim rhythmic cells – based on the rhythm distance operator
+    •	input_csv (str)– file containing the dictionary generated by rhythmNetwork
+    •	thup, thdw (float)– upper and lower thresholds for edge creation
+    •	w (logical) – if True it writes the nodes.csv and edges.csv files in csv format
+    •	returns nodes and edges tables as pandas DataFrames
     '''
-    # build the directional network of the full orchestration progression
 
-    dedges = pd.DataFrame(None,columns=['Source','Target','Weight'])
-    dnodes = pd.DataFrame(None,columns=['Label'])
-    for n in range(len(seq)):
-        nameseq = pd.DataFrame([np.array2string(seq[n]).replace(" ","").replace("[","").replace("]","")],\
-                               columns=['Label'])
-        dnodes = dnodes.append(nameseq)
-    df = np.asarray(dnodes)
-    dnodes = pd.DataFrame(None,columns=['Label'])
-    dff,idx = np.unique(df,return_inverse=True)
-    for n in range(dff.shape[0]):
-        nameseq = pd.DataFrame([[str(dff[n])]],columns=['Label'])
-        dnodes = dnodes.append(nameseq)
-    for n in range(1,len(seq)):
-        a = np.asarray(seq[n-1])
-        b = np.asarray(seq[n])
-        pair,r = minimalDistance(a,b,TET,distance)
-        tmp = pd.DataFrame([[str(idx[n-1]),str(idx[n]),str(pair+0.1)]],
-                           columns=['Source','Target','Weight'])
-        dedges = dedges.append(tmp)
+    start=time.time()    
+    # Create network of minimal rhythm leadings from the rhythmDictionary
     
-    # evaluate average degree and modularity
-    gbch = nx.from_pandas_edgelist(dedges,'Source','Target','Weight',create_using=nx.DiGraph())
-    gbch_u = nx.from_pandas_edgelist(dedges,'Source','Target','Weight')
-    # modularity 
-    part = cm.best_partition(gbch_u)
-    modul = cm.modularity(part,gbch_u)
-    # average degree
-    nnodes=gbch.number_of_nodes()
-     # average degree
-    nnodes=gbch.number_of_nodes()
-    avg = 0
-    for node in gbch.in_degree():
-        avg += node[1]
-    avgdeg = avg/float(nnodes)
-        
-    return(dnodes,dedges,avgdeg,modul,part,gbch,gbch_u)
+    df = np.asarray(dictionary)
+
+    # write csv for nodes
+    dnodes = pd.DataFrame(df[:,0],columns=['Label'])
+    if write: dnodes.to_csv('nodes.csv',index=False)
+    #dnodes.to_json('nodes.json')
+    
+    # find edges according to a metric
+    N = df[:,1].shape[0]
+    dedges = pd.DataFrame(None,columns=['Source','Target','Weight'])
+    np.random.seed(int(time.process_time()*10000))
+    for i in range(N):
+        vector_i = []
+        for l in range(len(df[:,1][0].split())):
+            vector_i.append(fr.Fraction(df[:,1][i].split()[l]))
+        vector_i  = RHYTHMSeq(vector_i)
+        for j in range(i,N):
+            vector_j = []
+            for l in range(len(df[:,1][0].split())):
+                vector_j.append(fr.Fraction(df[:,1][j].split()[l]))
+            vector_j  = RHYTHMSeq(vector_j)
+            pair = floatize(rhythmDistance(vector_i,vector_j,distance))
+            if pair < thup and pair > thdw:
+                if prob == 1:
+                    tmp = pd.DataFrame([[str(i),str(j),str(pair)]],columns=['Source','Target','Weight'])
+                    dedges = pd.concat([dedges,tmp],ignore_index=True)
+                else:
+                    r = np.random.rand()
+                    if r <= prob:
+                        tmp = pd.DataFrame([[str(i),str(j),str(pair)]],columns=['Source','Target','Weight'])
+                        dedges = pd.concat([dedges,tmp],ignore_index=True)
+                    else:
+                        pass
+
+    # write csv for edges
+    if write: dedges.to_csv('edges.csv',index=False)
 
+    return(dnodes,dedges)
```

### Comparing `musicntwrk-2.2.9/src/networks/orchestralVector.py` & `musicntwrk-2.3.0/src/networks/orchestralVector.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,15 +38,15 @@
                         if n.isRest:
                             orch[p].append(0)
                         else:
                             orch[p].append(1)
             except:
                 print('exception: most likely an error in the voicing of the musicxml score',\
                       'part ',p,'measure ',m)
-    orch = np.asarray(orch).T
+    orch = np.asarray(orch,dtype=object).T
     if len(orch.shape) == 1:
         print('WARNING: the number of beats per part is not constant')
         print('         check the musicxml file for internal consistency')
         a = []
         for i in range(orch.shape[0]):
             a.append(len(orch[i]))
         clean = np.zeros((min(a),orch.shape[0]),dtype=int)
```

### Comparing `musicntwrk-2.2.9/src/networks/orchestralVectorColor.py` & `musicntwrk-2.3.0/src/networks/orchestralVectorColor.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.9/src/networks/pcsDictionary.py` & `musicntwrk-2.3.0/src/networks/pcsDictionary.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.9/src/networks/pcsEgoNetwork.py` & `musicntwrk-2.3.0/src/networks/pcsEgoNetwork.py`

 * *Files 6% similar despite different names*

```diff
@@ -80,15 +80,15 @@
     dedges = pd.DataFrame(None,columns=['Source','Target','Weight'])
     for j in range(N):
         vector[j] = np.asarray(list(map(int,re.findall('\d+',dict_class.loc[name[j]][1]))))
     pair = sklm.pairwise_distances(ego.reshape(1, -1), vector, metric=distance)
     for j in range(N):
         if pair[0,j] <= thup_e and pair[0,j] >= thdw_e:
             tmp = pd.DataFrame([[str(i),str(j),str(1/pair[0,j])]],columns=['Source','Target','Weight'])
-            dedges = dedges.append(tmp)
+            dedges = pd.concat([dedges,tmp],ignore_index=True)
     # write csv for ego's edges
     if write: dedges.to_csv('edges_ego.csv',index=False)   
     edges_ego = dedges     
     
     # alters edges
     # parallelize over interval vector to optimize the vectorization in sklm.pairwise_distances
     if size != 1:
@@ -99,44 +99,44 @@
         index = np.linspace(0,N,N,dtype=int)
         dedges = pd.DataFrame(None,columns=['Source','Target','Weight'])
         for i in range(nsize):
             tmp = pd.DataFrame(None,columns=['Source','Target','Weight'])
             tmp['Source'] = (i+ini)*np.ones(N,dtype=int)[:]
             tmp['Target'] = index[:]
             tmp['Weight'] = pair[i,:]
-            dedges = dedges.append(tmp)
+            dedges = pd.concat([dedges,tmp],ignore_index=True)
         dedges = dedges.query('Weight<='+str(thup)).query('Weight>='+str(thdw))
         dedges['Weight'] = dedges['Weight'].apply(lambda x: 1/x)
         # do some cleaning
         cond = dedges.Source > dedges.Target
         dedges.loc[cond, ['Source', 'Target']] = dedges.loc[cond, ['Target', 'Source']].values
         dedges = dedges.drop_duplicates(subset=['Source', 'Target'])
 
         # write csv for partial edges
         dedges.to_csv('edges'+str(rank)+'.csv',index=False)
         
         if rank == 0:
             dedges = pd.DataFrame(None,columns=['Source','Target','Weight'])
             for i in range(size):
                 tmp = pd.read_csv('edges'+str(i)+'.csv')
-                dedges = dedges.append(tmp)
+                dedges = pd.concat([dedges,tmp],ignore_index=True)
                 os.remove('edges'+str(i)+'.csv')
             # write csv for edges
             if write: dedges.to_csv('edges_alters.csv',index=False)
             edges_alters = dedges
     else:
         N = len(name)-1
         dedges = pd.DataFrame(None,columns=['Source','Target','Weight'])
         for i in range(N):
             vector_i = np.asarray(list(map(int,re.findall('\d+',dict_class.loc[name[i]][1]))))
             for j in range(i,N):
                 vector_j = np.asarray(list(map(int,re.findall('\d+',dict_class.loc[name[j]][1]))))
                 pair = sklm.pairwise.paired_euclidean_distances(vector_i.reshape(1, -1),vector_j.reshape(1, -1))
                 if pair <= thup and pair >= thdw:
                     tmp = pd.DataFrame([[str(i),str(j),str(1/pair[0])]],columns=['Source','Target','Weight'])
-                    dedges = dedges.append(tmp)
+                    dedges = pd.concat([dedges,tmp],ignore_index=True)
 
         # write csv for alters' edges
         if write: dedges.to_csv('edges_alters.csv',index=False)
         edges_alters = dedges
     
     return(nodes_ego, edges_ego, edges_alters)
```

### Comparing `musicntwrk-2.2.9/src/networks/pcsNetwork.py` & `musicntwrk-2.3.0/src/networks/pcsNetwork.py`

 * *Files 5% similar despite different names*

```diff
@@ -57,15 +57,15 @@
         for n in range(len(df)):
             p = PCSet(np.asarray(list(map(int,re.findall('\d+',df[n,1])))))
             if p.pcs.shape[0] == 1:
                 nn = ''.join(m21.chord.Chord(p.pcs.tolist()).pitchNames)
             else:
                 nn = ''.join(m21.chord.Chord(p.normalOrder().tolist()).pitchNames)
             nameseq = pd.DataFrame([[str(nn)]],columns=['Label'])
-            dnodes = dnodes.append(nameseq)
+            dnodes = pd.concat([dnodes,nameseq],ignore_index=True)
     else:
         dnodes = pd.DataFrame(df[:,0],columns=['Label'])
     if write: dnodes.to_csv('nodes.csv',index=False)
 
     if para: comm.Barrier()
     
     # find edges according to a metric
@@ -84,19 +84,19 @@
     for i in range(nsize):
         tmp = pd.DataFrame(None,columns=['Source','Target','Weight'])
         tmp['Source'] = (i+ini)*np.ones(vector.shape[0],dtype=int)[:]
         tmp['Target'] = index[:]
         tmp['Weight'] = np.sqrt(np.sum((vaux[i,:]-vector[:,:])**2,axis=1))
         tmp = tmp.query('Weight<='+str(thup)).query('Weight>='+str(thdw))
         if prob == 1:
-            dedges = dedges.append(tmp)
+            dedges = pd.concat([dedges,tmp],ignore_index=True)
         else:
             np.random.seed(int(time.time()))
             if np.random.rand() >= prob:
-                dedges = dedges.append(tmp)
+                dedges = pd.concat([dedges,tmp],ignore_index=True)
             else:
                 pass
             
     dedges = dedges.query('Weight<='+str(thup)).query('Weight>='+str(thdw))
     dedges['Weight'] = dedges['Weight'].apply(lambda x: 1/x)
     # do some cleaning
     cond = dedges.Source > dedges.Target
@@ -107,15 +107,15 @@
     dedges.to_csv('edges'+str(rank)+'.csv',index=False)
     if para: comm.Barrier()
     
     if size != 1 and rank == 0:
         dedges = pd.DataFrame(None,columns=['Source','Target','Weight'])
         for i in range(size):
             tmp = pd.read_csv('edges'+str(i)+'.csv')
-            dedges = dedges.append(tmp)
+            dedges = pd.concat([dedges,tmp],ignore_index=True)
             os.remove('edges'+str(i)+'.csv')
         # do some cleaning
         cond = dedges.Source > dedges.Target
         dedges.loc[cond, ['Source', 'Target']] = dedges.loc[cond, ['Target', 'Source']].values
         dedges = dedges.drop_duplicates(subset=['Source', 'Target'])
         # write csv for edges
         if write: dedges.to_csv('edges.csv',index=False)
```

### Comparing `musicntwrk-2.2.9/src/networks/rLeadNetwork.py` & `musicntwrk-2.3.0/src/networks/vLeadNetworkVec.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,67 +9,65 @@
 #
 # This file is distributed under the terms of the
 # GNU General Public License. See the file `License'
 # in the root directory of the present distribution,
 # or http://www.gnu.org/copyleft/gpl.txt .
 #
 
-import time,re,os
+import time,re
 import numpy as np
-import fractions as fr
+import itertools as iter
 import pandas as pd
+import music21 as m21
 
-from ..musicntwrk import RHYTHMSeq
-from ..utils.floatize import floatize
-from ..utils.rhythmDistance import rhythmDistance
-
-def rLeadNetwork(dictionary,thup,thdw,distance,prob,write):
-        
-    '''
-    •	generation of the network of all minimal rhythm leadings in a generalized musical space of Nc-dim rhythmic cells – based on the rhythm distance operator
-    •	input_csv (str)– file containing the dictionary generated by rhythmNetwork
-    •	thup, thdw (float)– upper and lower thresholds for edge creation
-    •	w (logical) – if True it writes the nodes.csv and edges.csv files in csv format
-    •	returns nodes and edges tables as pandas DataFrames
-    '''
+from ..musicntwrk import PCSet
+from ..utils.minimalDistanceVec import minimalDistanceVec
 
-    start=time.time()    
-    # Create network of minimal rhythm leadings from the rhythmDictionary
+def vLeadNetworkVec(dictionary,thup,thdw,distance,prob,write,pcslabel,TET):
     
+    # Create network of minimal voice leadings from the pcsDictionary
+    # vector version
+
     df = np.asarray(dictionary)
 
     # write csv for nodes
-    dnodes = pd.DataFrame(df[:,0],columns=['Label'])
+    if pcslabel:
+        dnodes = pd.DataFrame(None,columns=['Label'])
+        for n in range(len(df)):
+            p = PCSet(np.asarray(list(map(int,re.findall('\d+',df[n,1])))))
+            if p.pcs.shape[0] == 1:
+                nn = ''.join(m21.chord.Chord(p.pcs.tolist()).pitchNames)
+            else:
+                nn = ''.join(m21.chord.Chord(p.normalOrder().tolist()).pitchNames)
+            nameseq = pd.DataFrame([[str(nn)]],columns=['Label'])
+            dnodes = pd.concat([dnodes,nameseq],ignore_index=True)
+    else:
+        dnodes = pd.DataFrame(df[:,0],columns=['Label'])
     if write: dnodes.to_csv('nodes.csv',index=False)
-    #dnodes.to_json('nodes.json')
-    
+
     # find edges according to a metric
     N = df[:,1].shape[0]
     dedges = pd.DataFrame(None,columns=['Source','Target','Weight'])
-    np.random.seed(int(time.process_time()*10000))
+    vector_i = np.zeros((N,len(list(map(int,re.findall('\d+',df[0,1]))))),dtype=int)
+    pair = np.zeros((N,N),dtype=float)
+    dis = np.zeros((N,N),dtype=float)
+    # vector of pcs
+    for i in range(N):
+        vector_i[i] = np.asarray(list(map(int,re.findall('\d+',df[i,1]))))
+
+    # vectors of distances
     for i in range(N):
-        vector_i = []
-        for l in range(len(df[:,1][0].split())):
-            vector_i.append(fr.Fraction(df[:,1][i].split()[l]))
-        vector_i  = RHYTHMSeq(vector_i)
-        for j in range(i,N):
-            vector_j = []
-            for l in range(len(df[:,1][0].split())):
-                vector_j.append(fr.Fraction(df[:,1][j].split()[l]))
-            vector_j  = RHYTHMSeq(vector_j)
-            pair = floatize(rhythmDistance(vector_i,vector_j,distance))
-            if pair < thup and pair > thdw:
-                if prob == 1:
-                    tmp = pd.DataFrame([[str(i),str(j),str(pair)]],columns=['Source','Target','Weight'])
-                    dedges = dedges.append(tmp)
-                else:
-                    r = np.random.rand()
-                    if r <= prob:
-                        tmp = pd.DataFrame([[str(i),str(j),str(pair)]],columns=['Source','Target','Weight'])
-                        dedges = dedges.append(tmp)
-                    else:
-                        pass
+        pair[i,:] = minimalDistanceVec(vector_i,np.roll(vector_i,-i,axis=0),TET,distance)
+
+    for i in range(N):
+        dis += np.diag(pair[i,:(N-i)],k=i)
+
+    ix,iy = np.nonzero(dis)
+    for n in range(ix.shape[0]):
+        if dis[ix[n],iy[n]] < thup and dis[ix[n],iy[n]] > thdw:
+            tmp = pd.DataFrame([[str(ix[n]),str(iy[n]),str(1/dis[ix[n],iy[n]])]],columns=['Source','Target','Weight'])
+            dedges = pd.concat([dedges,tmp],ignore_index=True)
 
     # write csv for edges
     if write: dedges.to_csv('edges.csv',index=False)
-
+    
     return(dnodes,dedges)
```

### Comparing `musicntwrk-2.2.9/src/networks/readScore.py` & `musicntwrk-2.3.0/src/networks/readScore.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.9/src/networks/rhythmDictionary.py` & `musicntwrk-2.3.0/src/networks/rhythmDictionary.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,22 +16,14 @@
 import sys
 import itertools as itr
 import numpy as np
 import pandas as pd
 
 from ..musicntwrk import RHYTHMSeq
 
-from ..utils.communications import *
-from ..utils.load_balancing import *
-
-# initialize parallel execution
-comm=MPI.COMM_WORLD
-rank = comm.Get_rank()
-size = comm.Get_size()
-
 def rhythmDictionary(Nc,a,REF):
 
     '''
     •	Generate the dictionary of all possible rhythmic sequences of Nc length in a generalized meter 
         space of N durations
     •	Nc (int)– cell length
     •	a is the list of durations in the rhythm sequence (str)
@@ -72,26 +64,25 @@
         for i in range(perm.shape[0]):
             if RHYTHMSeq(perm[i].tolist(),REF).isNonRetro():
                 name[n] = name[n]+'N'
     
     # find those that are Z-related (have same duration vector)
     
     ZrelT = None
-    if rank == 0:
-        # find pc sets in Z relation
-        u, indeces = np.unique(vector, return_inverse=True,axis=0)
-        ZrelT = []
-        for n in range(u.shape[0]):
-            if np.array(np.where(indeces == n)).shape[1] != 1:
-                indx = np.array(np.where(indeces == n))[0]
-                Zrel = []
-                for m in range(indx.shape[0]):
-                    name[indx[m]] = name[indx[m]]+'Z'
-                    Zrel.append(name[indx[m]])
-                ZrelT.append(Zrel)
+    # find pc sets in Z relation
+    u, indeces = np.unique(vector, return_inverse=True,axis=0)
+    ZrelT = []
+    for n in range(u.shape[0]):
+        if np.array(np.where(indeces == n)).shape[1] != 1:
+            indx = np.array(np.where(indeces == n))[0]
+            Zrel = []
+            for m in range(indx.shape[0]):
+                name[indx[m]] = name[indx[m]]+'Z'
+                Zrel.append(name[indx[m]])
+            ZrelT.append(Zrel)
                     
     # Create dictionary of rhythmic cells
     reference = []
     for n in range(len(name)):
         entry = [name[n],prime[n],
                 np.array2string(vector[n,:],separator=',').replace(" ","")]
         reference.append(entry)
```

### Comparing `musicntwrk-2.2.9/src/networks/rhythmNetwork.py` & `musicntwrk-2.3.0/src/networks/rhythmNetwork.py`

 * *Files 5% similar despite different names*

```diff
@@ -71,19 +71,19 @@
     for i in range(nsize):
         tmp = pd.DataFrame(None,columns=['Source','Target','Weight'])
         tmp['Source'] = (i+ini)*np.ones(vector.shape[0],dtype=int)[:]
         tmp['Target'] = index[:]
         tmp['Weight'] = np.sqrt(np.sum((vaux[i,:]-vector[:,:])**2,axis=1))
         tmp = tmp.query('Weight<='+str(thup)).query('Weight>='+str(thdw))
         if prob == 1:
-            dedges = dedges.append(tmp)
+            dedges = pd.concat([dedges,tmp],ignore_index=True)
         else:
             np.random.seed(int(time.time()))
             if np.random.rand() >= prob:
-                dedges = dedges.append(tmp)
+                dedges = pd.concat([dedges,tmp],ignore_index=True)
             else:
                 pass
             
     dedges = dedges.query('Weight<='+str(thup)).query('Weight>='+str(thdw))
     dedges['Weight'] = dedges['Weight'].apply(lambda x: 1/x)
     # do some cleaning
     cond = dedges.Source > dedges.Target
@@ -94,15 +94,15 @@
     dedges.to_csv('edges'+str(rank)+'.csv',index=False)
     if para: comm.Barrier()
     
     if size != 1 and rank == 0:
         dedges = pd.DataFrame(None,columns=['Source','Target','Weight'])
         for i in range(size):
             tmp = pd.read_csv('edges'+str(i)+'.csv')
-            dedges = dedges.append(tmp)
+            dedges = pd.concat([dedges,tmp],ignore_index=True)
             os.remove('edges'+str(i)+'.csv')
         # do some cleaning
         cond = dedges.Source > dedges.Target
         dedges.loc[cond, ['Source', 'Target']] = dedges.loc[cond, ['Target', 'Source']].values
         dedges = dedges.drop_duplicates(subset=['Source', 'Target'])
         # write csv for edges
         if write: dedges.to_csv('edges.csv',index=False)
```

### Comparing `musicntwrk-2.2.9/src/networks/rhythmPDictionary.py` & `musicntwrk-2.3.0/src/networks/rhythmPDictionary.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,26 +16,19 @@
 import sys
 import itertools as itr
 import numpy as np
 import pandas as pd
 
 from ..musicntwrk import RHYTHMSeq
 
-from ..utils.communications import *
-from ..utils.load_balancing import *
 from ..utils.Sublists import *
 from ..utils.Remove import *
 from ..utils.str2frac import *
 from ..utils.str2float import *
 
-# initialize parallel execution
-comm=MPI.COMM_WORLD
-rank = comm.Get_rank()
-size = comm.Get_size()
-
 def rhythmPDictionary(N,Nc,REF):
 
     '''
     •	Generate the dictionary of all possible rhythmic sequences from all possible groupings of N 
         REF durations
     •	N (int)– number of REF units
     •	Nc cardinality of the grouping
@@ -92,35 +85,35 @@
         reference.append(entry)
 
     dictionary = pd.DataFrame(reference,columns=['cell','r-seq','r-vec'])
     dictionary = dictionary.drop_duplicates(subset=['r-seq', 'r-vec'])
     
     # clean dictionary
     for n in range(len(dictionary)):
-        dictionary.loc[n][1] = str(RHYTHMSeq(str2frac(dictionary.loc[n][1])).normalOrder())\
+        dictionary.loc[n].iloc[1] = str(RHYTHMSeq(str2frac(dictionary.loc[n].iloc[1])).normalOrder())\
         .replace('Fraction','').replace(', ','/').replace('(','').replace(')','')\
         .replace('\n','').replace('[','').replace(']','')
     dictionary = dictionary.drop_duplicates(subset=['r-seq', 'r-vec']).reset_index(drop=True)
     
     # rename entries in ascending order and check for non-retrogradability
     for n in range(len(dictionary)):
-        dictionary.loc[n][0] = str(Nc)+'-'+str(n+1)
-        if RHYTHMSeq(str2frac(dictionary.loc[n][1])).isNonRetro(): 
-            dictionary.loc[n][0] += 'N'
+        dictionary.loc[n].iloc[0] = str(Nc)+'-'+str(n+1)
+        if RHYTHMSeq(str2frac(dictionary.loc[n].iloc[1])).isNonRetro(): 
+            dictionary.loc[n].iloc[0] += 'N'
     
     # find those that are Z-related (have same interval onset vector)
     
     vector = []
     for n in range(len(dictionary)):
         vector.append(str2float(dictionary['r-vec'][n]))
     u, indeces = np.unique(vector, return_inverse=True,axis=0)
     ZrelT = []
     for n in range(u.shape[0]):
         if np.array(np.where(indeces == n)).shape[1] != 1:
             indx = np.array(np.where(indeces == n))[0]
             Zrel = []
             for m in range(indx.shape[0]):
-                dictionary.loc[indx[m]][0] = dictionary.loc[indx[m]][0]+'Z'
-                Zrel.append(dictionary.loc[indx[m]][0])
+                dictionary.loc[indx[m]].iloc[0] = dictionary.loc[indx[m]].iloc[0]+'Z'
+                Zrel.append(dictionary.loc[indx[m]].iloc[0])
             ZrelT.append(Zrel)    
     return(dictionary,ZrelT)
```

### Comparing `musicntwrk-2.2.9/src/networks/scoreDictionary.py` & `musicntwrk-2.3.0/src/networks/scoreDictionary.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.9/src/networks/scoreMIDIDictionary.py` & `musicntwrk-2.3.0/src/networks/scoreMIDIDictionary.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.9/src/networks/scoreNetwork.py` & `musicntwrk-2.3.0/src/networks/scoreNetwork.py`

 * *Files 10% similar despite different names*

```diff
@@ -48,57 +48,67 @@
             dict24 = {'C':0,'C~':1,'C#':2,'D-':2,'D`':3,'D':4,'D~':5,'D#':6,'E-':6,'E`':7,'E':8,
                                 'E~':9,'F`':9,'F':10,'F~':11,'F#':12,'G-':12,'G`':13,'G':14,'G~':15,'G#':16,
                                 'A-':16,'A`':17,'A':18,'A~':19,'A#':20,'B-':20,'B`':21,'B':22,'B~':23,'C`':23}
             tmp = []
             for i in p.pcs:
                 tmp.append(list(dict24.keys())[list(dict24.values()).index(i)]) 
             nameseq = pd.DataFrame([[''.join(tmp)]],columns=['Label'])
-        dnodes = dnodes.append(nameseq)
+#       dnodes = pd.concat([dnodes,nameseq],ignore_index=True)
+        dnodes = pd.concat([dnodes,nameseq],ignore_index=True)
     df = np.asarray(dnodes)
     dnodes = pd.DataFrame(None,columns=['Label'])
     dcounts = pd.DataFrame(None,columns=['Label','Counts'])
     dff,idx,cnt = np.unique(df,return_inverse=True,return_counts=True)
     for n in range(dff.shape[0]):
         nameseq = pd.DataFrame([[str(dff[n])]],columns=['Label'])
-        dnodes = dnodes.append(nameseq)
+#       dnodes = pd.concat([dnodes,nameseq],ignore_index=True)
+        dnodes = pd.concat([dnodes,nameseq],ignore_index=True)
         namecnt = pd.DataFrame([[str(dff[n]),cnt[n]]],columns=['Label','Counts'])
-        dcounts = dcounts.append(namecnt)
+#       dcounts = dcounts.append(namecnt)
+        dcounts = pd.concat([dnodes,namecnt],ignore_index=True)
 
     for n in range(1,len(seq)):
         if len(seq[n-1]) == len(seq[n]):
             a = np.asarray(seq[n-1])
             b = np.asarray(seq[n])
             pair,r = minimalDistance(a,b,TET,distance)
+            name = generalizedOpsName(a,b,TET,distance)[1]
+            nameAbs = generalizedOpsNameAbs(a,b,TET,distance)[1]
         else:
             if len(seq[n-1]) > len(seq[n]):
                 a = np.asarray(seq[n-1])
                 b = np.asarray(seq[n])
                 pair,r = minimalNoBijDistance(a,b,TET,distance)
+                name = generalizedOpsName(a,r,TET,distance)[1]
+                nameAbs = generalizedOpsNameAbs(a,r,TET,distance)[1]
             else: 
                 b = np.asarray(seq[n-1])
                 a = np.asarray(seq[n])
                 pair,r = minimalNoBijDistance(a,b,TET,distance)
+                name = generalizedOpsName(r,a,TET,distance)[1]
+                nameAbs = generalizedOpsNameAbs(r,a,TET,distance)[1]
         if pair != 0:
             if general == False:
-                tmp = pd.DataFrame([[str(idx[n-1]),str(idx[n]),str(1/pair),generalizedOpsNameAbs(a,r,TET,distance)[1]]],
+                tmp = pd.DataFrame([[str(idx[n-1]),str(idx[n]),str(1/pair),nameAbs]],
                                     columns=['Source','Target','Weight','Label'])
             else:
-                tmp = pd.DataFrame([[str(idx[n-1]),str(idx[n]),str(1/pair),generalizedOpsName(a,r,TET,distance)[1]]],
+                tmp = pd.DataFrame([[str(idx[n-1]),str(idx[n]),str(1/pair),name]],
                                     columns=['Source','Target','Weight','Label'])
-            dedges = dedges.append(tmp)
+#           dedges = pd.concat([dedges,tmp],ignore_index=True)
+            dedges = pd.concat([dedges,tmp],ignore_index=True)
             
 # write dataframe with pcs rather than indeces
 #           if pair != 0:
 #                if general == False:
 #                    tmp = pd.DataFrame([[str(seq[n-1]),str(seq[n]),str(1/pair),opsName(a,r,TET)]],
 #                                        columns=['Source','Target','Weight','Label'])
 #                else:
 #                    tmp = pd.DataFrame([[str(seq[n-1]),str(seq[n]),str(1/pair),generalizedOpsName(a,r,TET)[1]]],
 #                                        columns=['Source','Target','Weight','Label'])
-#                dedges = dedges.append(tmp)
+#                dedges = pd.concat([dedges,tmp],ignore_index=True)
 
     
     if ntx:
         # evaluate average degree and modularity
         gbch = nx.from_pandas_edgelist(dedges,'Source','Target',['Weight','Label'],create_using=nx.DiGraph())
         gbch_u = nx.from_pandas_edgelist(dedges,'Source','Target',['Weight','Label'])
         # modularity 
@@ -109,7 +119,8 @@
         avg = 0
         for node in gbch.degree():
             avg += node[1]
         avgdeg = avg/float(nnodes)
         return(dnodes,dedges,dcounts,avgdeg,modul,gbch,gbch_u)
     else:
         return(dnodes,dedges,dcounts)
+
```

### Comparing `musicntwrk-2.2.9/src/networks/scoreSubNetwork.py` & `musicntwrk-2.3.0/src/networks/scoreSubNetwork.py`

 * *Files 12% similar despite different names*

```diff
@@ -47,24 +47,27 @@
             dict24 = {'C':0,'C~':1,'C#':2,'D-':2,'D`':3,'D':4,'D~':5,'D#':6,'E-':6,'E`':7,'E':8,
                                 'E~':9,'F`':9,'F':10,'F~':11,'F#':12,'G-':12,'G`':13,'G':14,'G~':15,'G#':16,
                                 'A-':16,'A`':17,'A':18,'A~':19,'A#':20,'B-':20,'B`':21,'B':22,'B~':23,'C`':23}
             tmp = []
             for i in p.pcs:
                 tmp.append(list(dict24.keys())[list(dict24.values()).index(i)]) 
             nameseq = pd.DataFrame([[''.join(tmp)]],columns=['Label'])
-        dnodes = dnodes.append(nameseq)
+#       dnodes = pd.concat([dnodes,nameseq],ignore_index=True)
+        dnodes = pd.concat([dnodes,nameseq],ignore_index=True)
     df = np.asarray(dnodes)
     dnodes = pd.DataFrame(None,columns=['Label'])
     dcounts = pd.DataFrame(None,columns=['Label','Counts'])
     dff,idx,cnt = np.unique(df,return_inverse=True,return_counts=True)
     for n in range(dff.shape[0]):
         nameseq = pd.DataFrame([[str(dff[n])]],columns=['Label'])
-        dnodes = dnodes.append(nameseq)
+#       dnodes = pd.concat([dnodes,nameseq],ignore_index=True)
+        dnodes = pd.concat([dnodes,nameseq],ignore_index=True)
         namecnt = pd.DataFrame([[str(dff[n]),cnt[n]]],columns=['Label','Counts'])
-        dcounts = dcounts.append(namecnt)
+#       dcounts = dcounts.append(namecnt)
+        dcounts = pd.concat([dnodes,namecnt],ignore_index=True)
 
     for n in range(1,len(seq)):
         if len(seq[n-1]) == len(seq[n]):
             a = np.asarray(seq[n-1])
             b = np.asarray(seq[n])
             pair,r = minimalDistance(a,b,TET,distance)
         else:
@@ -80,23 +83,25 @@
             if general == False:
                 if n >= start and n < end:
                     tmp = pd.DataFrame([[str(idx[n-1]),str(idx[n]),str(1/pair),opsName(a,r,TET)]],
                                         columns=['Source','Target','Weight','Label'])
 #                 else:
 #                     tmp = pd.DataFrame([[str(idx[n-1]),str(idx[n]),str(0),opsName(a,r,TET)]],
 #                                         columns=['Source','Target','Weight','Label'])
-                    dedges = dedges.append(tmp)
+#                   dedges = pd.concat([dedges,tmp],ignore_index=True)
+                    dedges = pd.concat([dedges,tmp],ignore_index=True)
             else:
                 if n >= start and n < end:
                     tmp = pd.DataFrame([[str(idx[n-1]),str(idx[n]),str(1/pair),generalizedOpsName(a,r,TET,distance)[1]]],
                                         columns=['Source','Target','Weight','Label'])
 #                 else:
 #                     tmp = pd.DataFrame([[str(idx[n-1]),str(idx[n]),str(0),generalizedOpsName(a,r,TET)[1]]],
 #                                         columns=['Source','Target','Weight','Label'])
-                    dedges = dedges.append(tmp)
+#                   dedges = pd.concat([dedges,tmp],ignore_index=True)
+                    dedges = pd.concat([dedges,tmp],ignore_index=True)
     
     if ntx:
         # evaluate average degree and modularity
         if grphtype == 'directed':
             gbch = nx.from_pandas_edgelist(dedges,'Source','Target',['Weight','Label'],create_using=nx.DiGraph())
         elif grphtype == 'multi':
             gbch = nx.from_pandas_edgelist(dedges,'Source','Target',['Weight','Label'],create_using=nx.MultiDiGraph())
```

### Comparing `musicntwrk-2.2.9/src/networks/timbralNetwork.py` & `musicntwrk-2.3.0/src/networks/timbralNetwork.py`

 * *Files 12% similar despite different names*

```diff
@@ -42,38 +42,36 @@
     '''
     # build the network
 
     dedges = pd.DataFrame(None,columns=['Source','Target','Weight'])
     dnodes = pd.DataFrame(None,columns=['Label'])
     for n in range(len(waves)):
         nameseq = pd.DataFrame([waves[n].split('/')[-1].split('.')[0]],columns=['Label'])
-        dnodes = dnodes.append(nameseq)
+        dnodes = pd.concat([dnodes,nameseq],ignore_index=True)
     df = np.array(dnodes)
     dnodes = pd.DataFrame(None,columns=['Label'])
     dff,idx = np.unique(df,return_inverse=True)
     for n in range(dff.shape[0]):
         nameseq = pd.DataFrame([[str(dff[n])]],columns=['Label'])
-        dnodes = dnodes.append(nameseq)
+        dnodes = pd.concat([dnodes,nameseq],ignore_index=True)
     
     N = vector.shape[0]
     index = np.linspace(0,vector.shape[0]-1,vector.shape[0],dtype=int)
     # parallelize over interval vector to optimize the vectorization in sklm.pairwise_distances
     ini,end = load_balancing(size, rank, N)
     nsize = end-ini
     vaux = scatter_array(vector)
     #pair = sklm.pairwise_distances(vaux,vector,metric=distance)
     dedges = pd.DataFrame(None,columns=['Source','Target','Weight'])
     for i in range(nsize):
-        tmp = pd.DataFrame(None,columns=['Source','Target','Weight'])
-        tmp['Source'] = (i+ini)*np.ones(vector.shape[0],dtype=int)[:]
-        tmp['Target'] = index[:]
-        tmp['Weight'] = np.sqrt(np.sum((vaux[i,:]-vector[:,:])**2,axis=1))
-        tmp = tmp.query('Weight<='+str(thup)).query('Weight>='+str(thdw))
-        dedges = dedges.append(tmp)
-            
+        tmp0 = (i+ini)*np.ones(vector.shape[0],dtype=int)
+        tmp1 = index[:]
+        tmp2 = np.sqrt(np.sum((vaux[i,:]-vector[:,:])**2,axis=(1,2)))
+        dedges = dedges.append(pd.DataFrame(data=np.column_stack((tmp0,tmp1,tmp2)),
+                                            columns=['Source','Target','Weight']))
     dedges = dedges.query('Weight<='+str(thup)).query('Weight>='+str(thdw))
     dedges['Weight'] = dedges['Weight'].apply(lambda x: 1/x)
     # do some cleaning
     cond = dedges.Source > dedges.Target
     dedges.loc[cond, ['Source', 'Target']] = dedges.loc[cond, ['Target', 'Source']].values
     dedges = dedges.drop_duplicates(subset=['Source', 'Target'])
 
@@ -81,15 +79,15 @@
     dedges.to_csv('edges'+str(rank)+'.csv',index=False)
     if para: comm.Barrier()
     
     if size != 1 and rank == 0:
         dedges = pd.DataFrame(None,columns=['Source','Target','Weight'])
         for i in range(size):
             tmp = pd.read_csv('edges'+str(i)+'.csv')
-            dedges = dedges.append(tmp)
+            dedges = pd.concat([dedges,tmp],ignore_index=True)
             os.remove('edges'+str(i)+'.csv')
         # do some cleaning
         cond = dedges.Source > dedges.Target
         dedges.loc[cond, ['Source', 'Target']] = dedges.loc[cond, ['Target', 'Source']].values
         dedges = dedges.drop_duplicates(subset=['Source', 'Target'])
         # write csv for edges
         dedges.to_csv('edges.csv',index=False)
```

### Comparing `musicntwrk-2.2.9/src/networks/vLeadNetwork.py` & `musicntwrk-2.3.0/src/networks/vLeadNetwork.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,15 +42,15 @@
         for n in range(len(df)):
             p = PCSet(np.asarray(list(map(int,re.findall('\d+',df[n,1])))))
             if p.pcs.shape[0] == 1:
                 nn = ''.join(m21.chord.Chord(p.pcs.tolist()).pitchNames)
             else:
                 nn = ''.join(m21.chord.Chord(p.normalOrder().tolist()).pitchNames)
             nameseq = pd.DataFrame([[str(nn)]],columns=['Label'])
-            dnodes = dnodes.append(nameseq)
+            dnodes = pd.concat([dnodes,nameseq],ignore_index=True)
     else:
         dnodes = pd.DataFrame(df[:,0],columns=['Label'])
     if write: dnodes.to_csv('nodes.csv',index=False)
     
     # find edges according to a metric - allows for non-bijective voice leading
     N = df[:,1].shape[0]
     dedges = pd.DataFrame(None,columns=['Source','Target','Weight'])
@@ -77,20 +77,20 @@
                 dist = np.zeros(r.shape[0])
                 for l in range(r.shape[0]):
                     dist[l],_ = minimalDistance(a,r[l])
                 pair = min(dist)
             if pair <= thup and pair >= thdw:
                 if prob == 1:
                     tmp = pd.DataFrame([[str(i),str(j),str(1/pair)]],columns=['Source','Target','Weight'])
-                    dedges = dedges.append(tmp)
+                    dedges = pd.concat([dedges,tmp],ignore_index=True)
                 else:
                     r = np.random.rand()
                     if r <= prob:
                         tmp = pd.DataFrame([[str(i),str(j),str(1/pair)]],columns=['Source','Target','Weight'])
-                        dedges = dedges.append(tmp)
+                        dedges = pd.concat([dedges,tmp],ignore_index=True)
                     else:
                         pass
 
     # write csv for edges
     if write: dedges.to_csv('edges.csv',index=False)
     
     return(dnodes,dedges)
```

### Comparing `musicntwrk-2.2.9/src/networks/vLeadNetworkByName.py` & `musicntwrk-2.3.0/src/networks/vLeadNetworkByName.py`

 * *Files 10% similar despite different names*

```diff
@@ -45,15 +45,15 @@
         for n in range(len(df)):
             p = PCSet(np.asarray(list(map(int,re.findall('\d+',df[n,1])))))
             if p.pcs.shape[0] == 1:
                 nn = ''.join(m21.chord.Chord(p.pcs.tolist()).pitchNames)
             else:
                 nn = ''.join(m21.chord.Chord(p.normalOrder().tolist()).pitchNames)
             nameseq = pd.DataFrame([[str(nn)]],columns=['Label'])
-            dnodes = dnodes.append(nameseq)
+            dnodes = pd.concat([dnodes,nameseq],ignore_index=True)
     else:
         dnodes = pd.DataFrame(df[:,0],columns=['Label'])
     if write: dnodes.to_csv('nodes.csv',index=False)
     
     # find edges according to a metric - allows for non-bijective voice leading
 
     if not isinstance(name,list):
@@ -63,44 +63,46 @@
     np.random.seed(int(time.process_time()*10000))
     for i in range(N):
         vector_i  = np.asarray(list(map(int,re.findall('\d+',df[i,1]))))
         for j in range(i,N):
             vector_j  = np.asarray(list(map(int,re.findall('\d+',df[j,1]))))
             if vector_i.shape[0] == vector_j.shape[0]:
                 dis,_ = minimalDistance(vector_i,vector_j,TET,distance)
-                pair = np.array([opsCheckByName(vector_i,vector_j,nam,TET) for nam in name])
+                pair = np.array([opsCheckByNameAbs(vector_i,vector_j,nam,TET) for nam in name])
                 # pair = opsCheckByName(vector_i,vector_j,name,TET)
             else:
                 if vector_i.shape[0] > vector_j.shape[0]:
                     a = vector_i 
                     b = vector_j
                 else:
                     b = vector_i 
                     a = vector_j
-                ndif = np.sort(np.array([a.shape[0],b.shape[0]]))[1] - np.sort(np.array([a.shape[0],b.shape[0]]))[0]
-                c = np.asarray(list(iter.combinations_with_replacement(b,ndif)))
-                r = np.zeros((c.shape[0],a.shape[0]))
-                for l in range(c.shape[0]):
-                    r[l,:b.shape[0]] = b
-                    r[l,b.shape[0]:] = c[l]
-                dist = np.zeros(r.shape[0])
-                for l in range(r.shape[0]):
-                    dist[l],_= minimalNoBijDistance(a,r[l],TET,distance)
-                imin = np.argmin(dist)
-                pair = np.array([opsCheckByNameAbs(a,r[imin],nam,TET) for nam in name])
-                dis = min(dist)
+                # ndif = np.sort(np.array([a.shape[0],b.shape[0]]))[1] - np.sort(np.array([a.shape[0],b.shape[0]]))[0]
+                # c = np.asarray(list(iter.combinations_with_replacement(b,ndif)))
+                # r = np.zeros((c.shape[0],a.shape[0]))
+                # for l in range(c.shape[0]):
+                #     r[l,:b.shape[0]] = b
+                #     r[l,b.shape[0]:] = c[l]
+                # dist = np.zeros(r.shape[0])
+                # for l in range(r.shape[0]):
+                #     dist[l],_= minimalDistance(a,r[l],TET,distance)
+                # imin = np.argmin(dist)
+                dis,r = minimalNoBijDistance(a,b,TET,distance)
+                pair = np.array([opsCheckByNameAbs(a,r,nam,TET) for nam in name])
+                # pair = np.array([opsCheckByNameAbs(a,r[imin],nam,TET) for nam in name])
+                # dis = min(dist)
             if pair.any() == True:
                 if prob == 1:
                     tmp = pd.DataFrame([[str(i),str(j),str(1/dis)]],columns=['Source','Target','Weight'])
-                    dedges = dedges.append(tmp)
+                    dedges = pd.concat([dedges,tmp],ignore_index=True)
                 else:
                     r = np.random.rand()
                     if r <= prob:
                         tmp = pd.DataFrame([[str(i),str(j),str(1/dis)]],columns=['Source','Target','Weight'])
-                        dedges = dedges.append(tmp)
+                        dedges = pd.concat([dedges,tmp],ignore_index=True)
                     else:
                         pass
 
     # write csv for edges
     if write: dedges.to_csv('edges.csv',index=False)
 
     return(dnodes,dedges)
```

### Comparing `musicntwrk-2.2.9/src/networks/vLeadNetworkByNameVec.py` & `musicntwrk-2.3.0/src/networks/vLeadNetworkByNameVec.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,15 +36,15 @@
         for n in range(len(df)):
             p = PCSet(np.asarray(list(map(int,re.findall('\d+',df[n,1])))))
             if p.pcs.shape[0] == 1:
                 nn = ''.join(m21.chord.Chord(p.pcs.tolist()).pitchNames)
             else:
                 nn = ''.join(m21.chord.Chord(p.normalOrder().tolist()).pitchNames)
             nameseq = pd.DataFrame([[str(nn)]],columns=['Label'])
-            dnodes = dnodes.append(nameseq)
+            dnodes = pd.concat([dnodes,nameseq],ignore_index=True)
     else:
         dnodes = pd.DataFrame(df[:,0],columns=['Label'])
     if write: dnodes.to_csv('nodes.csv',index=False)
 
     # find edges according to a metric
     N = df[:,1].shape[0]
     dedges = pd.DataFrame(None,columns=['Source','Target','Weight'])
@@ -65,13 +65,13 @@
         dis += np.diag(disx[i,:(N-i)],k=i)
         pair += np.diag(pairx[i,:(N-i)],k=i)
     print(len(name))    
     ix,iy = np.nonzero(dis)
     for n in range(ix.shape[0]):
         if pair[ix[n],iy[n]]:
             tmp = pd.DataFrame([[str(ix[n]),str(iy[n]),str(1/dis[ix[n],iy[n]])]],columns=['Source','Target','Weight'])
-            dedges = dedges.append(tmp)
+            dedges = pd.concat([dedges,tmp],ignore_index=True)
 
     # write csv for edges
     if write: dedges.to_csv('edges.csv',index=False)
     
     return(dnodes,dedges)
```

### Comparing `musicntwrk-2.2.9/src/plotting/barplot.py` & `musicntwrk-2.3.0/src/plotting/barplot.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.9/src/plotting/chordspace.py` & `musicntwrk-2.3.0/src/plotting/chordspace.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,586 +1,586 @@
-#
-# MUSIC𝄞NTWRK
-#
-# A python library for pitch class set and rhythmic sequences classification and manipulation,
-# the generation of networks in generalized music and sound spaces, and the sonification of arbitrary data
-#
-# Copyright (C) 2018 Marco Buongiorno Nardelli
-# http://www.materialssoundmusic.com, mbn@unt.edu
-#
-# This file is distributed under the terms of the
-# GNU General Public License. See the file `License'
-# in the root directory of the present distribution,
-# or http://www.gnu.org/copyleft/gpl.txt .
-#
-# The following code has been extracted from the original program written by Dmitri Tymoczko, www.madmusicalscience.com
-
-"""
-Draw an abstract picture of chord space, emphsizing its circular dimension and the line containing n-note chords, which winds around this 
-dimension n times.
-
-Plots points showing how the chords in a scale are distributed on this abstract picture; clicking on this picture will play the chords
-
-Usage:
-
-	c = chordspace.ChordSpace(startNotes = [60, 64, 67], startScale = [0, 2, 4, 5, 7, 9, 11])
-
-	startNotes
-		if list: starting midi notes for playback
-		if int: the size of the chord, the number of times the transpositions wind around chord space
-	startScale
-		the scale to use.
-
-	There are many defaults built into the program; so you can just call chordspace.go(3, 12) (etc.).  It will select appropriately.
-
-Many graphic parameters you can fiddle with, such as:
-
-	gapAngle = a graphical parameter determining what proportion of the circle is taken up by the twist (.2 = 20%).  Adjust to taste.
-	circleSeparation = how far apart the circles are drawn
-
-Can draw arrows representing my chord lattices
-
-Also:
-	chordspace.line() draws a very simple (noninteractive) picture of the situation in pitch space, with no octave equivalence ... useful just as a point of contrast
-
-"""
-import matplotlib
-import matplotlib.pyplot as plt
-import numpy as np
-import time
-from threading import Timer
-from music21 import *
-
-matplotlib.rcParams['pdf.fonttype'] = 42
-matplotlib.rcParams['ps.fonttype'] = 42
-
-for s in ['keymap.all_axes', 'keymap.back', 'keymap.forward', 'keymap.fullscreen', 'keymap.grid', 'keymap.home', 
-			'keymap.pan', 'keymap.quit', 'keymap.save', 'keymap.xscale', 'keymap.yscale', 'keymap.zoom']:
-	plt.rcParams[s] = ''
-
-def linear_map(value, firstRange, secondRange):
-	pct = 1.0 * (value - firstRange[0])/(firstRange[1] - firstRange[0])
-	output = secondRange[0] + pct*(secondRange[1] - secondRange[0])
-	return output
-
-def euclidean_distance(l1, l2):
-	return pow(sum([(l2[i] - l1[i])**2 for i in range(len(l1))]), .5)
-
-def line(spacing = 1.7, offset = -.2):	
-	"""Just draw a silly line with points on it, to contrast with the circular case"""
-	plt.figure(figsize=(8,8))
-	plt.subplots_adjust(left=0.1, right=0.9, top=0.9, bottom=0.1)
-	fig, ax = plt.subplots()
-	plt.ioff()
-	ax.axes.get_xaxis().set_visible(False)
-	ax.axes.get_yaxis().set_visible(False)
-	ax.grid(False)
-	ax.set_xlim([-8, 8])
-	ax.set_ylim([-8, 8])
-	yCoords = np.arange(-10 + offset, 10 + offset, spacing)
-	xCoords = [0]*len(yCoords)
-	ax.plot([-10, 10], [0, 0], color = 'black')
-	ax.scatter(yCoords, xCoords, s = 50, c = 'black')
-	ax.set_yticks([])  # no ticks
-	ax.set_xticks([])
-	plt.show()
-
-class ChordSpace():
-	
-	def __init__(self, startNotes = 2, startScale = 7, **kwargs):
-		
-		"""PRESET: (6, 11): {3:[.1, -.15], 5: [-.1, 0], 7: [-.1, 0]},"""
-	
-		"""Arrow Presets 1 is the first two voice leadings on the generalized circle of fifths; preset 2 is the first square"""
-		
-		self.attributeDict = {	"labels": True, 
-								"arrows": [], 
-								"bigAngleDict": {},
-								"gapAngle": .2, 
-								"circleSeparation": 1, 
-								"pointRotation": 0, 
-								"labelAdjustments": False,
-								"_CIRCLESIZE": 50,
-								"_CLICKRADIUS": .5,
-								"masterLetters": ['Fn', 'Cn', 'Gn', 'Dn', 'An', 'En', 'Bn', 'Fs', 'Cs', 'Gs', 'Ef', 'Bf'],
-								"standardRList": [[0, 5, 50], [5, 7, 50]],
-								"medWrapAround": [[0, 2, 100], [2, 10, 100]],
-								"bigWrapAround": [[0, 1, 150], [1, 3, 100], [3, 6, 100]],
-								"arrowPresets": {1: [[0, 1, .9], [1, 2, .9]], 2: [[0, 1, .9, None, 0, 'r'], [1, 2, .9], [1, 2, .9, 0], ['lastDest', 2, .9, None, 0, 'r']]},
-								"globalWinding": 0,
-								"shouldQuit": False,
-								"keysPressed": [],
-								"theCoords": False,
-								"startNotes": None,
-								"standardAdjustments": {
-														(2, 12): {2:[-.1, 0]},
-														(3, 12): {9: [-.1, 0], 11: [.1, 0]},
-														(3, 7): {5: [-.1, 0]},
-														(4, 10): {0: [0, -.1], 1: [-.03, .03], 3: [-.15, 0], 5: [0, -.1], 9: [.05, .1]},
-														(4, 12): {0: [0, -.1], 3: [0, -.1], 6: [0, -.1], 9: [0, -.1], 1: [.1, .3], 4: [.1, .3], 7: [.1, .3], 10: [.1, .3],
-																2: [0, .3], 5: [-.1, .3], 8: [-.1, .3], 11: [-.1, .3]},
-														(5, 12): {0:[0, -.15], 1: [0, .3], 2: [.3, 0], 3: [-.1, 0], 4: [.15, -.08], 5: [-.05, -.1], 6: [0, .1], 7: [.05, -.1], 8: [-.1, 0], 9:[.1, 0], 10:[-.1, 0], 11:[0, .1]},
-														(6, 11): {0:[0, 0], 10: [0, 0], 9: [0, 0], 8: [0, 0], 7: [-.15, 0], 6: [0, 0], 5: [-.1, 0], 4:[0, 0], 3:[-.1, 0], 2: [0, 0], 1:[0, 0]},
-														(6, 12): {0:[0, -.5], 10: [0, -.5], 9: [0, .5], 8: [0, -.5], 7: [0, .5], 6: [0, -.5], 5: [0, .5], 4:[0, -.5], 3:[0, .5], 2: [0, -.5], 1:[0, .5], 11: [0, .5]},
-														(7, 12): {0:[0, -.15], 1: [.1, .1], 2: [.05, -.05], 3: [-.1, 0], 4:[.2, .3], 5: [.2, .1], 6: [0, 0], 7: [-.1, 0.], 8: [-.1, 0], 9: [0, -.2], 10: [-.1, 0], 11: [.2, .1]},
-																
-														},
-								"defaultPitches": {(1, 12): [[60], []], (2, 7): [[72, 76], []], (2, 11): [[72, 76], []], (2, 12): [[72, 76], []], (3, 7): [[60, 64, 67], []], (3, 12): [[60, 64, 67], []], 
-													(4, 7): [[60, 64, 67, 71], []], (4, 12): [[60, 64, 67, 70], []], (4, 10): [[60, 63, 66, 68], [0, 1, 2, 3, 4, 6, 7, 8, 9, 10]], (6, 11): [[60, 62, 64, 65, 67, 69],[]]
-													},
-								"internalPresets": {(3, 7): {"clickRadius": .9}, (7, 12): {"arpeggiate": .015, "clickRadius": .9, "rAdjustment": .6, "gapAngle": .23}, (6, 11): {"arpeggiate":.2, "allNotesOff":False, "rAdjustment": .6}},
-								"preset": 0,
-								"presetDict": {	1: {"startNotes": [43, 50, 57, 64, 66, 72, 77], "theScale": range(12), "rAdjustment": .6, "gapAngle": .23}, 2: {"startNotes": [67, 68, 69, 70, 71], "theScale": range(12), "voiceVelocities": [80, 54, 80, 54, 80]},
-												3: {"startNotes": [60, 74], "theScale": [0, 2, 4, 5, 7, 9, 11], "baseVL": [2, 0]}, 4: {'startNotes': [50, 67, 69, 72], "theScale": [0, 2, 4, 5, 7, 9, 11], "voiceVelocities": [90, 72, 72, 72]},
-												5: {'startNotes': [48, 55, 62, 65, 69, 76], "theScale": range(11)},
-												10: {"startNotes": [60, 64, 67], "theScale": range(12), "alphaLabels": {x:.3 for x in [1, 11, 4, 8, 6, 3]}},
-												11: {"startNotes": [60, 64, 67], "theScale": range(12), "alphaLabels": {x:.3 for x in [1, 11, 4, 8, 6, 3]}}},
-								"graphs": [[[48, 85, 62, 75, 64], range(12)], [[60, 67, 76], 7], [60, 65, 67, 71], 7],
-								"mainChordGraph": False,
-								"midiin": False,
-								"midiout": False,
-								"bigPoint": False,
-								"lastPoint": False,
-								"lastIndex": 0,
-								"lastChordNumber": 0,
-								"chordIndex": 0,
-								"arpeggiate": False, 
-								"defaultScales": {5: [0, 2, 4, 7, 9], 7: [0, 2, 4, 5, 7, 9, 11], 10: [0, 1, 2, 3, 4, 6, 7, 8, 9, 10]},
-								"lastClick": 0,
-								"diatonicObjectKeywords": {},
-								"allNotesOff": True,
-								"theScale": False,
-								"activeNotes": [], 
-								"notesPlayed": 0,
-								"slices": 15,
-								"sliceDelay": .001,
-								"rAdjustment": .4,
-								"recordTimer": None,
-								"outputStream": stream.Stream(),
-								"minimumRecordingDuration": .2,
-								"deltaList": [],
-								"_GLOBALREFLECTION": False,
-								"lowercase": False,
-								"suppressLabels": False,
-								"quarterTone": False,
-								"radius": 4,
-								"alphaLabels": {},
-								"innerRadius": 0,
-								"outerRadius": 0,
-								"isTsymmetrical": False,
-								"drawPoints": True,
-								"drawPie": False,
-								"saveName": False, 
-								"drawTarget": False,
-								"baseAlpha": 1.,
-								"drawMatrix": False,
-								"matrixChords": False,
-								"originalScaleSize": False,
-								"graphCommas": [],
-								"manualLabels": []
-		 				   		}										
-																	
-		for key, value in self.attributeDict.items():
-			if key in kwargs:
-				setattr(self, key, kwargs[key])
-			else:
-				setattr(self, key, value)
-		
-		"""Lots of boring code to deal with various ways you can initialize the scale and chord: using midi notes, integers, etc."""
-		
-		if self.preset in self.presetDict:
-			for key, value in self.presetDict[self.preset].items():
-				setattr(self, key, value)
-			self.chordSize = len(self.startNotes)
-			# print(self.chordSize)
-			self.scaleSize = len(self.theScale)
-		else:		
-			if type(startNotes) is int and type(startScale) is int:
-				if (startNotes, startScale) in self.defaultPitches:
-					self.startNotes, self.tempScale = self.defaultPitches[(startNotes, startScale)]
-					if self.tempScale:
-						self.theScale = self.tempScale[:]
-						self.scaleSize = len(self.theScale)
-						startScale = None
-					self.chordSize = startNotes
-					
-				if (startNotes, startScale) in self.internalPresets:
-					presetDict = self.internalPresets[(startNotes, startScale)]
-					for key, value in presetDict.items():
-						if key not in kwargs:
-							setattr(self, key, value)
-				if self.startNotes:
-					startNotes = None
-			if type(startScale) is int:
-				self.scaleSize = startScale
-				if startScale in self.defaultScales:
-					self.theScale = self.defaultScales[startScale]
-				elif startScale:
-					self.theScale = range(startScale)
-				startScale = None
-			elif type(startScale) is list:
-				self.theScale = startScale
-				self.scaleSize = len(self.theScale)
-			if type(startNotes) is int:
-				self.chordSize = startNotes
-				if self.theScale:
-					self.startNotes = [60 + self.theScale[x] for x in self.get_maximally_even()]
-			elif type(startNotes) is list:
-				self.chordSize = len(startNotes)
-				if max(startNotes) < 12:
-					self.startNotes = [60 + self.theScale[x] for x in startNotes]
-				else:
-					self.startNotes = startNotes
-		
-		if (self.scaleSize) and (11 < max(self.theScale) < 24 or not (all([x == int(x) for x in self.theScale])) or not (all([x == int(x) for x in self.startNotes]))):
-			self.quarterTone = True
-		
-		if self.preset == 11:
-			self.masterLetters = ['VII', 'I', 'fII', 'II', 'fIII', 'III', 'IV', 'fV', 'V', 'fVI', 'VI', 'fVII']
-		
-		"""manage diatonic object keywords, which get passed to underlying diatonic object"""
-		for s in ['baseVL']:
-			if s in kwargs:
-				self.diatonicObjectKeywords[s] = kwargs[s]
-			elif hasattr(self, s):
-				self.diatonicObjectKeywords[s] = getattr(self, s)
-		
-		if 'voiceVelocities' in kwargs:
-			self.voiceVelocities = kwargs['voiceVelocities']
-		elif not hasattr(self, 'voiceVelocities'):
-			self.voiceVelocities = [72] * self.chordSize
-		
-		"""Deal with transpositional symmetry here"""
-			
-		self.setClass = [self.theScale.index(x % 12) if (x % 12) in self.theScale else -1 for x in self.startNotes]
-		self.originalScaleSize = self.scaleSize
-		
-		"""GAPANGLE is the portion of the circle where the lines wind into each other"""
-		
-		if self.chordSize == 1:
-			self._GAPANGLE = 2 * np.pi
-		else:
-			self._GAPANGLE = (1. - self.gapAngle) * 2 * np.pi
-
-		if type(self.arrows) is int or type(self.arrows) is str:
-			self.arrows = self.arrowPresets[self.arrows]
-		
-		"""Pyplot initialization code"""	
-		if not self.drawTarget:
-			sizeFactor = 10./8
-			if self.drawMatrix:
-				self.fig = plt.figure(figsize=(sizeFactor * 8, 8))
-			else:
-				self.fig = plt.figure(figsize=(8,8))
-			plt.subplots_adjust(left=0.1, right=0.9, top=0.9, bottom=0.1)
-			self.ax = plt.subplot()
-		
-			self.ax.axes.get_xaxis().set_visible(False)
-			self.ax.axes.get_yaxis().set_visible(False)
-			self.ax.grid(False)
-		
-			self.bound = self.radius + (self.chordSize * self.circleSeparation) + 1
-			
-			if self.drawMatrix:
-				newSize = 2 * self.bound * sizeFactor
-				self.ax.set_xlim([-self.bound, newSize - self.bound])
-				self.matrixLocation = newSize - self.bound
-				self.make_matrix()
-			else:
-				self.ax.set_xlim([-self.bound, self.bound])
-			self.ax.set_ylim([-self.bound, self.bound])
-		else:
-			self.fig = self.drawTarget.fig			# for drawing multiple graphs on one canvas
-			self.ax = self.drawTarget.ax
-		
-		"""draw the circles without the connectors, leaving out an arc for connections"""
-		for i in range(int(self.chordSize)):
-			theCircle = ChordSpace.draw_circle(r = self.radius + (self.circleSeparation*i), thetaMax = self._GAPANGLE)
-			self.ax.plot(*theCircle, color = 'black', alpha = self.baseAlpha)
-		
-		"""draw the internal connectors"""
-		for i in range(int(self.chordSize) - 1):
-			self.newAngles, self.newRs = ChordSpace.interpolate_between_circles(self._GAPANGLE, self.radius + (self.circleSeparation*i),
-					 2*np.pi, self.radius + (self.circleSeparation*(i + 1)), self.standardRList)
-
-			self.newAngles = [(2*np.pi * (self.chordSize - 1 - i)) + x for x in self.newAngles]
-			self.bigAngleDict.update({self.newAngles[i]:self.newRs[i] for i in range(len(self.newAngles))})
-			connection = ChordSpace.poltocar(self.newAngles, self.newRs)
-			self.ax.plot(*connection, color = 'black', alpha = self.baseAlpha)
-		
-		"""draw the wraparound connector"""
-		if self.chordSize > 1:
-			if self.chordSize >= 5:
-				wrapInts = self.bigWrapAround
-			else:
-				wrapInts = self.medWrapAround
-			self.newAngles, self.newRs = ChordSpace.interpolate_between_circles(self._GAPANGLE, self.radius, 2*np.pi, self.radius + (self.circleSeparation*(self.chordSize-1)), wrapInts)
-			self.newRs = self.newRs[::-1]	
-			connection = ChordSpace.poltocar(self.newAngles, self.newRs)
-			self.bigAngleDict.update({self.newAngles[i]:self.newRs[i] for i in range(len(self.newAngles))})
-			self.ax.plot(*connection, color = 'black', alpha = self.baseAlpha)
-		
-		"""boundaries to represent the annulus"""
-		if self.innerRadius:
-			self.innerCircle = plt.Circle((0, 0), self.innerRadius, color='black', fill=False, linestyle = '--', alpha = .5)
-			self.ax.add_artist(self.innerCircle)
-		
-		if self.outerRadius:
-			self.outerCircle = plt.Circle((0, 0), self.outerRadius, color='black', fill=False, linestyle = '--', alpha = .5)
-			self.ax.add_artist(self.outerCircle)
-			
-		if self.scaleSize and self.drawPie:
-			r = self.radius + (self.circleSeparation*self.chordSize)
-			a = (2*np.pi)/self.scaleSize
-			for i in range(self.scaleSize):
-				newSlice = ChordSpace.poltocar([0, i*a], [0, r])
-				self.ax.plot(*newSlice, color = 'black', alpha = .5)
-		
-		"""you don't have to specify a scale, but if you do, the program will draw chords
-		  	 
-			 bigAngleDict[theta] = radius	
-					shows the radius at each theta position; needed to draw the circles on the wraparound spot; theta can be greater than 2*pi (when winding multiple times)
-			"""
-		if self.scaleSize and self.drawPoints:
-			
-			self.theKeys = sorted(self.bigAngleDict.keys())
-			self.totalDist = 2 * np.pi * self.chordSize
-			self.theAngles = np.linspace(0 + self.pointRotation, self.totalDist + self.pointRotation, self.scaleSize + 1)
-			self.basicDist = self.theAngles[1]
-			self.theAngles = self.theAngles[:-1]
-			self.theRs = []
-			
-			if self.graphCommas:					# for non-ET graphs
-				self.theAngles = [self.theAngles[x] + self.graphCommas[x] for x in range(len(self.theAngles))]	 
-				
-			for a in self.theAngles:
-				self.theRs.append(self.getRvalue(a))
-			
-			self.theCoords = ChordSpace.poltocar(self.theAngles, self.theRs)
-			self.ax.scatter(*self.theCoords, s = self._CIRCLESIZE, c = 'black', alpha = self.baseAlpha)
-			
-			"""calculate the clickable radius of each circle as half the minimum distance between adjacent circles"""
-			
-			minDist = 10000
-			
-			for i in range(len(self.theCoords[0]) - 1):
-				for j in range(i+1, len(self.theCoords[0])):
-					d = euclidean_distance([self.theCoords[0][i], self.theCoords[1][i]], [self.theCoords[0][j], self.theCoords[1][j]])
-					if d < minDist:
-						minDist = d
-			
-			self._CLICKRADIUS = minDist/2.
-			
-			if self.drawTarget:
-				self.drawTarget._CLICKRADIUS = 10
-			
-			"""thePoints
-			
-				a list whose elements are [angle % 2pi, angleWithWrapAround, radius]
-				ordered chromatically (C, C#, D etc.)
-			
-			"""
-			
-			self.thePoints = [[round(x[0] % (2 * np.pi), 4)] + list(x) for x in zip(self.theAngles, self.theRs)]
-			self.orderedPoints = sorted(self.thePoints)
-			
-			"""todo: need to account for pointRotation here in the sorting!"""
-			
-			self.simpleAngles = sorted(list(set([x[0] for x in self.thePoints])))
-			self.fundamentalAngle = self.simpleAngles[1]
-			
-			self.zeroPoints = [x[1:] for x in self.thePoints if x[0] == self.thePoints[0][0]]
-			self.zeroPointNumber = len(self.zeroPoints)
-			self.crossSections = int(self.scaleSize/self.zeroPointNumber)
-			
-			"""
-		
-			The two cases of lattice:
-			
-				0 = size of chord relatively prime to size of scale (single generator)
-				1 = size of chord divides or shares a common factor with the size of scale (two generators)
-			
-			For moving around the lattice, we require extra code to manage the second generator
-			
-			"""
-			
-			self.latticeStructure = int(not(self.zeroPointNumber == 1))
-			
-			"""simple code to attach letters to circles;
-			
-				standardAdjustments manually arranges the letters so as to avoid collisions.
-			
-			"""
-			if self.labels and not self.suppressLabels:
-				if self.scaleSize > 12:
-					self.letterNames = [str(x + 1) for x in range(self.scaleSize)]
-				else:
-					if self.manualLabels:
-						self.letterNames = self.manualLabels[:]
-					elif self.isTsymmetrical:
-						self.letterNames = sorted(self.masterLetters)
-						self.letterNames = self.letterNames[self.letterNames.index('Cn'):] + self.letterNames[:self.letterNames.index('Cn')]
-						self.letterNames = [x.replace('n', '') for x in self.letterNames[:self.scaleSize]]
-					elif self.scaleSize == 5:
-						self.letterNames = [x.replace('n', '') for x in sorted(self.masterLetters[1:6])]						
-					elif self.preset != 11:
-						self.letterNames = [x.replace('n', '') for x in sorted(self.masterLetters[:self.scaleSize])]
-						self.letterNames = self.letterNames[self.letterNames.index('C'):] + self.letterNames[:self.letterNames.index('C')]
-						if self.scaleSize == 11:
-							self.letterNames[-1] = 'Bf'
-					else:
-						self.letterNames = self.masterLetters[self.masterLetters.index('I'):] + self.masterLetters[:self.masterLetters.index('I')]	
-					
-				if self.preset == 11:
-					adjustmentTable = {0: [.04, 0], 1: [-.25, 0], 2: [-.1, 0], 3: [-.025, 0], 4: [-.1, -.05], 5: [-.05, 0], 6: [0, 0], 7: [-.05, 0], 8: [-.07, -.05], 9: [-.07, 0], 11: [.15, 0]}
-				elif (self.chordSize, self.scaleSize) in self.standardAdjustments:
-					adjustmentTable = self.standardAdjustments[(self.chordSize, self.scaleSize)]
-#					print('here')
-				else:
-					adjustmentTable = {}
-				
-				self.letterNames = [self.letterNames[0]] + self.letterNames[len(self.letterNames):0:-1]
-				
-				if self.lowercase:
-					self.letterNames = [x.lower() for x in self.letterNames]
-					
-				for i in range(self.scaleSize):
-					myTheta, myR = self.thePoints[i][1:]
-					myR = myR - self.rAdjustment
-					myCoord = ChordSpace.poltocar([myTheta], [myR])	# x, y?
-					myAdjustment = adjustmentTable.get(i, [0, 0])
-					theText = self.letterNames[i]
-					if theText.count('I') > 0 or theText.count('V') > 0:
-						plainText = filter(lambda x: x in 'IViv', theText)
-						theText = filter(lambda x: x not in 'IViv', theText)
-						self.ax.text(myCoord[0][0] - .1 + myAdjustment[0], myCoord[1][0] + myAdjustment[1], plainText, alpha = self.alphaLabels.get(i, 1.), verticalalignment = 'center', horizontalalignment = 'left', fontname = 'Helvetica')
-						self.ax.text(myCoord[0][0] - .3 + myAdjustment[0], myCoord[1][0] + .04 + myAdjustment[1], theText, alpha = self.alphaLabels.get(i, 1.), verticalalignment = 'center', horizontalalignment = 'left', fontname = 'EngraverTextT')
-					else:
-						self.ax.text(myCoord[0][0] + myAdjustment[0], myCoord[1][0] + myAdjustment[1], theText, alpha = self.alphaLabels.get(i, 1.), verticalalignment = 'center', horizontalalignment = 'center', fontname = 'EngraverTextT')
-			
-			"""Print generators"""
-			if len(self.zeroPoints) > 1:
-				self.theTransps = [[int(.001 + x[0] / (2. * np.pi)), int(.001 + x[0] / self.basicDist)] for x in self.zeroPoints[1:]]
-				print("Zero sum generator", -self.theTransps[0][0], self.theTransps[0][1])
-		
-			if len(self.simpleAngles) > 1 and self.chordSize > len(self.zeroPoints):
-				myPoints = []
-				for p in self.thePoints:
-					if abs(p[0] - self.fundamentalAngle) < .001:
-						myPoints.append(p[1:])
-				self.theTransps = [[int(.001 + x[0] / (2. * np.pi)), int(.001 + x[0] / self.basicDist)] for x in myPoints]
-				print("Sum-1 generator", -self.theTransps[0][0], self.theTransps[0][1])
-			
-			"""add arrows"""
-			if self.arrows:
-				
-				self.cartesianPoints = [ChordSpace.poltocar([x[1]], [x[2]]) for x in self.orderedPoints]
-				self.cartesianPoints = [[x[0][0], x[1][0]] for x in self.cartesianPoints]
-				
-				for arrowItem in self.arrows:			# startpoint, endpoint, %of distance, newStartPoint, rotation, color
-					defaultArrow = [arrowItem[0], None, .9, None, 0, 'black']
-					newArrowItem = [arrowItem[i] if i < len(arrowItem) else defaultArrow[i] for i in range(len(defaultArrow))]
-					#newArrowItem = arrowItem + [None] * (6 - len(arrowItem))
-					i, j, pct, newStartPoint, rot, col = newArrowItem
-					if i == 'lastDest':
-						startPoint = lastDest[:]
-					else:
-						startPoint = self.cartesianPoints[i]
-						if not j:
-							j = (i + 1) % self.scaleSize
-					deltaX, deltaY = [self.cartesianPoints[j][x] - startPoint[x] for x in [0, 1]]
-					if newStartPoint != None:
-						startPoint = self.cartesianPoints[newStartPoint]
-					if rot != None:
-						deltaX, deltaY = ChordSpace.rotate([deltaX, deltaY], rot*self.fundamentalAngle)
-					lastDest = [startPoint[0] + deltaX, startPoint[1] + deltaY]
-					self.ax.arrow(startPoint[0], startPoint[1], deltaX * pct, deltaY * pct, head_width=0.2, head_length=0.2, fc=col, ec=col)
-		
-		self.ax.set_yticks([]) 
-		self.ax.set_xticks([])
-		if self.saveName:
-			plt.savefig(self.saveName, bbox_inches='tight')
-		else:
-			self.show()
-		
-	def show(self):			# would be nice to be able to reopen this, but that seems not to be possible
-		plt.ion()
-		plt.show()
-		plt.pause(.0001)
-	
-	"""NOTE OFF CODE CAUSED THE PROGRAM TO BE SLUGGISH WHEN QUITTING, waiting for the Timers to quit; also produced sonic artifacts"""
-
-	def getRvalue(self, a):
-		
-		"""utility code to get an R value for an angle a"""
-		winding = int(a / (2 * np.pi))
-		generalTheta = a % (2 * np.pi)
-		if winding == 0:
-			rCoord = self.radius
-		else:
-			rCoord = self.radius + ((self.chordSize - winding) * self.circleSeparation)
-		if generalTheta < self._GAPANGLE:
-			return rCoord
-		else:
-			for i, k in enumerate(self.theKeys):
-				if k > a:
-					rCoord = self.bigAngleDict[self.theKeys[i-1]]
-					break
-			return rCoord
-	
-	def get_maximally_even(self):
-		return [int(x) for x in [f*(1.0*self.scaleSize)/self.chordSize for f in range(self.chordSize)]]
-		
-	@staticmethod
-	def poltocar(theta, R):
-		xCoords = []
-		yCoords = []
-		for i in range(len(theta)):
-			t = theta[i]
-			r = R[i]
-			xCoords.append(r*np.sin(t))
-			yCoords.append(r*np.cos(t))
-		return [xCoords, yCoords]
-		
-	@staticmethod
-	def draw_circle(thetaMin = 0, thetaMax = 0, r = 4, rMax = -1):
-		theta = np.linspace(thetaMin, thetaMax, int((thetaMax - thetaMin) / 0.01))
-		if rMax == -1:
-			newR = [r] * len(theta)
-		else:
-			newR = np.linspace(r, rMax, len(theta))
-		myCoords = ChordSpace.poltocar(theta, newR)
-		return myCoords
-
-	@staticmethod	
-	def rotate(p, theta):
-		return [p[0]*np.cos(theta) - p[1]*np.sin(theta), p[0]*np.sin(theta) + p[1]*np.cos(theta)]
-
-	@staticmethod
-	def make_RList(diffRanges):
-		
-		"""
-		utility routine for drawing smooth curves, interpolating between one circle and noather
-		you supply a list [firstdelta, seconddelta, numberofpoints], these are deltas between successive radii points
-		
-		example: 
-		
-			self.standardRList [[0, 5, 50], [5, 7, 50]] goes from 0 to 5 in 50 steps, then 5 to 7 in 50 steps (first steep then flattening)
-		
-		this program makes a symmetrical curve, so it adds the retrograde of the input pattern (this might not be the way to do things)
-		
-		"""
-		diffSeq = []
-		rangeList = [0]
-		for r in diffRanges:
-			diffSeq += list(np.linspace(*r))
-		diffSeq += diffSeq[::-1]
-		for d in diffSeq:
-			rangeList.append(rangeList[-1] + d)
-		return [linear_map(x, [rangeList[0], rangeList[-1]], [1, 0]) for x in rangeList]
-
-	@staticmethod
-	def interpolate_between_circles(firstAngle, firstR, secondAngle, secondR, rList):
-		rList = ChordSpace.make_RList(rList)
-		tempRList = [linear_map(x, [0, 1], [firstR, secondR]) for x in rList]
-		newAngles = np.linspace(firstAngle, secondAngle, len(tempRList))
-		return newAngles, tempRList
+#
+# MUSIC𝄞NTWRK
+#
+# A python library for pitch class set and rhythmic sequences classification and manipulation,
+# the generation of networks in generalized music and sound spaces, and the sonification of arbitrary data
+#
+# Copyright (C) 2018 Marco Buongiorno Nardelli
+# http://www.materialssoundmusic.com, mbn@unt.edu
+#
+# This file is distributed under the terms of the
+# GNU General Public License. See the file `License'
+# in the root directory of the present distribution,
+# or http://www.gnu.org/copyleft/gpl.txt .
+#
+# The following code has been extracted from the original program written by Dmitri Tymoczko, www.madmusicalscience.com
+
+"""
+Draw an abstract picture of chord space, emphsizing its circular dimension and the line containing n-note chords, which winds around this 
+dimension n times.
+
+Plots points showing how the chords in a scale are distributed on this abstract picture; clicking on this picture will play the chords
+
+Usage:
+
+	c = chordspace.ChordSpace(startNotes = [60, 64, 67], startScale = [0, 2, 4, 5, 7, 9, 11])
+
+	startNotes
+		if list: starting midi notes for playback
+		if int: the size of the chord, the number of times the transpositions wind around chord space
+	startScale
+		the scale to use.
+
+	There are many defaults built into the program; so you can just call chordspace.go(3, 12) (etc.).  It will select appropriately.
+
+Many graphic parameters you can fiddle with, such as:
+
+	gapAngle = a graphical parameter determining what proportion of the circle is taken up by the twist (.2 = 20%).  Adjust to taste.
+	circleSeparation = how far apart the circles are drawn
+
+Can draw arrows representing my chord lattices
+
+Also:
+	chordspace.line() draws a very simple (noninteractive) picture of the situation in pitch space, with no octave equivalence ... useful just as a point of contrast
+
+"""
+import matplotlib
+import matplotlib.pyplot as plt
+import numpy as np
+import time
+from threading import Timer
+from music21 import *
+
+matplotlib.rcParams['pdf.fonttype'] = 42
+matplotlib.rcParams['ps.fonttype'] = 42
+
+for s in ['keymap.back', 'keymap.forward', 'keymap.fullscreen', 'keymap.grid', 'keymap.home', 
+			'keymap.pan', 'keymap.quit', 'keymap.save', 'keymap.xscale', 'keymap.yscale', 'keymap.zoom']:
+	plt.rcParams[s] = ''
+
+def linear_map(value, firstRange, secondRange):
+	pct = 1.0 * (value - firstRange[0])/(firstRange[1] - firstRange[0])
+	output = secondRange[0] + pct*(secondRange[1] - secondRange[0])
+	return output
+
+def euclidean_distance(l1, l2):
+	return pow(sum([(l2[i] - l1[i])**2 for i in range(len(l1))]), .5)
+
+def line(spacing = 1.7, offset = -.2):	
+	"""Just draw a silly line with points on it, to contrast with the circular case"""
+	plt.figure(figsize=(8,8))
+	plt.subplots_adjust(left=0.1, right=0.9, top=0.9, bottom=0.1)
+	fig, ax = plt.subplots()
+	plt.ioff()
+	ax.axes.get_xaxis().set_visible(False)
+	ax.axes.get_yaxis().set_visible(False)
+	ax.grid(False)
+	ax.set_xlim([-8, 8])
+	ax.set_ylim([-8, 8])
+	yCoords = np.arange(-10 + offset, 10 + offset, spacing)
+	xCoords = [0]*len(yCoords)
+	ax.plot([-10, 10], [0, 0], color = 'black')
+	ax.scatter(yCoords, xCoords, s = 50, c = 'black')
+	ax.set_yticks([])  # no ticks
+	ax.set_xticks([])
+	plt.show()
+
+class ChordSpace():
+	
+	def __init__(self, startNotes = 2, startScale = 7, **kwargs):
+		
+		"""PRESET: (6, 11): {3:[.1, -.15], 5: [-.1, 0], 7: [-.1, 0]},"""
+	
+		"""Arrow Presets 1 is the first two voice leadings on the generalized circle of fifths; preset 2 is the first square"""
+		
+		self.attributeDict = {	"labels": True, 
+								"arrows": [], 
+								"bigAngleDict": {},
+								"gapAngle": .2, 
+								"circleSeparation": 1, 
+								"pointRotation": 0, 
+								"labelAdjustments": False,
+								"_CIRCLESIZE": 50,
+								"_CLICKRADIUS": .5,
+								"masterLetters": ['Fn', 'Cn', 'Gn', 'Dn', 'An', 'En', 'Bn', 'Fs', 'Cs', 'Gs', 'Ef', 'Bf'],
+								"standardRList": [[0, 5, 50], [5, 7, 50]],
+								"medWrapAround": [[0, 2, 100], [2, 10, 100]],
+								"bigWrapAround": [[0, 1, 150], [1, 3, 100], [3, 6, 100]],
+								"arrowPresets": {1: [[0, 1, .9], [1, 2, .9]], 2: [[0, 1, .9, None, 0, 'r'], [1, 2, .9], [1, 2, .9, 0], ['lastDest', 2, .9, None, 0, 'r']]},
+								"globalWinding": 0,
+								"shouldQuit": False,
+								"keysPressed": [],
+								"theCoords": False,
+								"startNotes": None,
+								"standardAdjustments": {
+														(2, 12): {2:[-.1, 0]},
+														(3, 12): {9: [-.1, 0], 11: [.1, 0]},
+														(3, 7): {5: [-.1, 0]},
+														(4, 10): {0: [0, -.1], 1: [-.03, .03], 3: [-.15, 0], 5: [0, -.1], 9: [.05, .1]},
+														(4, 12): {0: [0, -.1], 3: [0, -.1], 6: [0, -.1], 9: [0, -.1], 1: [.1, .3], 4: [.1, .3], 7: [.1, .3], 10: [.1, .3],
+																2: [0, .3], 5: [-.1, .3], 8: [-.1, .3], 11: [-.1, .3]},
+														(5, 12): {0:[0, -.15], 1: [0, .3], 2: [.3, 0], 3: [-.1, 0], 4: [.15, -.08], 5: [-.05, -.1], 6: [0, .1], 7: [.05, -.1], 8: [-.1, 0], 9:[.1, 0], 10:[-.1, 0], 11:[0, .1]},
+														(6, 11): {0:[0, 0], 10: [0, 0], 9: [0, 0], 8: [0, 0], 7: [-.15, 0], 6: [0, 0], 5: [-.1, 0], 4:[0, 0], 3:[-.1, 0], 2: [0, 0], 1:[0, 0]},
+														(6, 12): {0:[0, -.5], 10: [0, -.5], 9: [0, .5], 8: [0, -.5], 7: [0, .5], 6: [0, -.5], 5: [0, .5], 4:[0, -.5], 3:[0, .5], 2: [0, -.5], 1:[0, .5], 11: [0, .5]},
+														(7, 12): {0:[0, -.15], 1: [.1, .1], 2: [.05, -.05], 3: [-.1, 0], 4:[.2, .3], 5: [.2, .1], 6: [0, 0], 7: [-.1, 0.], 8: [-.1, 0], 9: [0, -.2], 10: [-.1, 0], 11: [.2, .1]},
+																
+														},
+								"defaultPitches": {(1, 12): [[60], []], (2, 7): [[72, 76], []], (2, 11): [[72, 76], []], (2, 12): [[72, 76], []], (3, 7): [[60, 64, 67], []], (3, 12): [[60, 64, 67], []], 
+													(4, 7): [[60, 64, 67, 71], []], (4, 12): [[60, 64, 67, 70], []], (4, 10): [[60, 63, 66, 68], [0, 1, 2, 3, 4, 6, 7, 8, 9, 10]], (6, 11): [[60, 62, 64, 65, 67, 69],[]]
+													},
+								"internalPresets": {(3, 7): {"clickRadius": .9}, (7, 12): {"arpeggiate": .015, "clickRadius": .9, "rAdjustment": .6, "gapAngle": .23}, (6, 11): {"arpeggiate":.2, "allNotesOff":False, "rAdjustment": .6}},
+								"preset": 0,
+								"presetDict": {	1: {"startNotes": [43, 50, 57, 64, 66, 72, 77], "theScale": range(12), "rAdjustment": .6, "gapAngle": .23}, 2: {"startNotes": [67, 68, 69, 70, 71], "theScale": range(12), "voiceVelocities": [80, 54, 80, 54, 80]},
+												3: {"startNotes": [60, 74], "theScale": [0, 2, 4, 5, 7, 9, 11], "baseVL": [2, 0]}, 4: {'startNotes': [50, 67, 69, 72], "theScale": [0, 2, 4, 5, 7, 9, 11], "voiceVelocities": [90, 72, 72, 72]},
+												5: {'startNotes': [48, 55, 62, 65, 69, 76], "theScale": range(11)},
+												10: {"startNotes": [60, 64, 67], "theScale": range(12), "alphaLabels": {x:.3 for x in [1, 11, 4, 8, 6, 3]}},
+												11: {"startNotes": [60, 64, 67], "theScale": range(12), "alphaLabels": {x:.3 for x in [1, 11, 4, 8, 6, 3]}}},
+								"graphs": [[[48, 85, 62, 75, 64], range(12)], [[60, 67, 76], 7], [60, 65, 67, 71], 7],
+								"mainChordGraph": False,
+								"midiin": False,
+								"midiout": False,
+								"bigPoint": False,
+								"lastPoint": False,
+								"lastIndex": 0,
+								"lastChordNumber": 0,
+								"chordIndex": 0,
+								"arpeggiate": False, 
+								"defaultScales": {5: [0, 2, 4, 7, 9], 7: [0, 2, 4, 5, 7, 9, 11], 10: [0, 1, 2, 3, 4, 6, 7, 8, 9, 10]},
+								"lastClick": 0,
+								"diatonicObjectKeywords": {},
+								"allNotesOff": True,
+								"theScale": False,
+								"activeNotes": [], 
+								"notesPlayed": 0,
+								"slices": 15,
+								"sliceDelay": .001,
+								"rAdjustment": .4,
+								"recordTimer": None,
+								"outputStream": stream.Stream(),
+								"minimumRecordingDuration": .2,
+								"deltaList": [],
+								"_GLOBALREFLECTION": False,
+								"lowercase": False,
+								"suppressLabels": False,
+								"quarterTone": False,
+								"radius": 4,
+								"alphaLabels": {},
+								"innerRadius": 0,
+								"outerRadius": 0,
+								"isTsymmetrical": False,
+								"drawPoints": True,
+								"drawPie": False,
+								"saveName": False, 
+								"drawTarget": False,
+								"baseAlpha": 1.,
+								"drawMatrix": False,
+								"matrixChords": False,
+								"originalScaleSize": False,
+								"graphCommas": [],
+								"manualLabels": []
+		 				   		}										
+																	
+		for key, value in self.attributeDict.items():
+			if key in kwargs:
+				setattr(self, key, kwargs[key])
+			else:
+				setattr(self, key, value)
+		
+		"""Lots of boring code to deal with various ways you can initialize the scale and chord: using midi notes, integers, etc."""
+		
+		if self.preset in self.presetDict:
+			for key, value in self.presetDict[self.preset].items():
+				setattr(self, key, value)
+			self.chordSize = len(self.startNotes)
+			# print(self.chordSize)
+			self.scaleSize = len(self.theScale)
+		else:		
+			if type(startNotes) is int and type(startScale) is int:
+				if (startNotes, startScale) in self.defaultPitches:
+					self.startNotes, self.tempScale = self.defaultPitches[(startNotes, startScale)]
+					if self.tempScale:
+						self.theScale = self.tempScale[:]
+						self.scaleSize = len(self.theScale)
+						startScale = None
+					self.chordSize = startNotes
+					
+				if (startNotes, startScale) in self.internalPresets:
+					presetDict = self.internalPresets[(startNotes, startScale)]
+					for key, value in presetDict.items():
+						if key not in kwargs:
+							setattr(self, key, value)
+				if self.startNotes:
+					startNotes = None
+			if type(startScale) is int:
+				self.scaleSize = startScale
+				if startScale in self.defaultScales:
+					self.theScale = self.defaultScales[startScale]
+				elif startScale:
+					self.theScale = range(startScale)
+				startScale = None
+			elif type(startScale) is list:
+				self.theScale = startScale
+				self.scaleSize = len(self.theScale)
+			if type(startNotes) is int:
+				self.chordSize = startNotes
+				if self.theScale:
+					self.startNotes = [60 + self.theScale[x] for x in self.get_maximally_even()]
+			elif type(startNotes) is list:
+				self.chordSize = len(startNotes)
+				if max(startNotes) < 12:
+					self.startNotes = [60 + self.theScale[x] for x in startNotes]
+				else:
+					self.startNotes = startNotes
+		
+		if (self.scaleSize) and (11 < max(self.theScale) < 24 or not (all([x == int(x) for x in self.theScale])) or not (all([x == int(x) for x in self.startNotes]))):
+			self.quarterTone = True
+		
+		if self.preset == 11:
+			self.masterLetters = ['VII', 'I', 'fII', 'II', 'fIII', 'III', 'IV', 'fV', 'V', 'fVI', 'VI', 'fVII']
+		
+		"""manage diatonic object keywords, which get passed to underlying diatonic object"""
+		for s in ['baseVL']:
+			if s in kwargs:
+				self.diatonicObjectKeywords[s] = kwargs[s]
+			elif hasattr(self, s):
+				self.diatonicObjectKeywords[s] = getattr(self, s)
+		
+		if 'voiceVelocities' in kwargs:
+			self.voiceVelocities = kwargs['voiceVelocities']
+		elif not hasattr(self, 'voiceVelocities'):
+			self.voiceVelocities = [72] * self.chordSize
+		
+		"""Deal with transpositional symmetry here"""
+			
+		self.setClass = [self.theScale.index(x % 12) if (x % 12) in self.theScale else -1 for x in self.startNotes]
+		self.originalScaleSize = self.scaleSize
+		
+		"""GAPANGLE is the portion of the circle where the lines wind into each other"""
+		
+		if self.chordSize == 1:
+			self._GAPANGLE = 2 * np.pi
+		else:
+			self._GAPANGLE = (1. - self.gapAngle) * 2 * np.pi
+
+		if type(self.arrows) is int or type(self.arrows) is str:
+			self.arrows = self.arrowPresets[self.arrows]
+		
+		"""Pyplot initialization code"""	
+		if not self.drawTarget:
+			sizeFactor = 10./8
+			if self.drawMatrix:
+				self.fig = plt.figure(figsize=(sizeFactor * 8, 8))
+			else:
+				self.fig = plt.figure(figsize=(8,8))
+			plt.subplots_adjust(left=0.1, right=0.9, top=0.9, bottom=0.1)
+			self.ax = plt.subplot()
+		
+			self.ax.axes.get_xaxis().set_visible(False)
+			self.ax.axes.get_yaxis().set_visible(False)
+			self.ax.grid(False)
+		
+			self.bound = self.radius + (self.chordSize * self.circleSeparation) + 1
+			
+			if self.drawMatrix:
+				newSize = 2 * self.bound * sizeFactor
+				self.ax.set_xlim([-self.bound, newSize - self.bound])
+				self.matrixLocation = newSize - self.bound
+				self.make_matrix()
+			else:
+				self.ax.set_xlim([-self.bound, self.bound])
+			self.ax.set_ylim([-self.bound, self.bound])
+		else:
+			self.fig = self.drawTarget.fig			# for drawing multiple graphs on one canvas
+			self.ax = self.drawTarget.ax
+		
+		"""draw the circles without the connectors, leaving out an arc for connections"""
+		for i in range(int(self.chordSize)):
+			theCircle = ChordSpace.draw_circle(r = self.radius + (self.circleSeparation*i), thetaMax = self._GAPANGLE)
+			self.ax.plot(*theCircle, color = 'black', alpha = self.baseAlpha)
+		
+		"""draw the internal connectors"""
+		for i in range(int(self.chordSize) - 1):
+			self.newAngles, self.newRs = ChordSpace.interpolate_between_circles(self._GAPANGLE, self.radius + (self.circleSeparation*i),
+					 2*np.pi, self.radius + (self.circleSeparation*(i + 1)), self.standardRList)
+
+			self.newAngles = [(2*np.pi * (self.chordSize - 1 - i)) + x for x in self.newAngles]
+			self.bigAngleDict.update({self.newAngles[i]:self.newRs[i] for i in range(len(self.newAngles))})
+			connection = ChordSpace.poltocar(self.newAngles, self.newRs)
+			self.ax.plot(*connection, color = 'black', alpha = self.baseAlpha)
+		
+		"""draw the wraparound connector"""
+		if self.chordSize > 1:
+			if self.chordSize >= 5:
+				wrapInts = self.bigWrapAround
+			else:
+				wrapInts = self.medWrapAround
+			self.newAngles, self.newRs = ChordSpace.interpolate_between_circles(self._GAPANGLE, self.radius, 2*np.pi, self.radius + (self.circleSeparation*(self.chordSize-1)), wrapInts)
+			self.newRs = self.newRs[::-1]	
+			connection = ChordSpace.poltocar(self.newAngles, self.newRs)
+			self.bigAngleDict.update({self.newAngles[i]:self.newRs[i] for i in range(len(self.newAngles))})
+			self.ax.plot(*connection, color = 'black', alpha = self.baseAlpha)
+		
+		"""boundaries to represent the annulus"""
+		if self.innerRadius:
+			self.innerCircle = plt.Circle((0, 0), self.innerRadius, color='black', fill=False, linestyle = '--', alpha = .5)
+			self.ax.add_artist(self.innerCircle)
+		
+		if self.outerRadius:
+			self.outerCircle = plt.Circle((0, 0), self.outerRadius, color='black', fill=False, linestyle = '--', alpha = .5)
+			self.ax.add_artist(self.outerCircle)
+			
+		if self.scaleSize and self.drawPie:
+			r = self.radius + (self.circleSeparation*self.chordSize)
+			a = (2*np.pi)/self.scaleSize
+			for i in range(self.scaleSize):
+				newSlice = ChordSpace.poltocar([0, i*a], [0, r])
+				self.ax.plot(*newSlice, color = 'black', alpha = .5)
+		
+		"""you don't have to specify a scale, but if you do, the program will draw chords
+		  	 
+			 bigAngleDict[theta] = radius	
+					shows the radius at each theta position; needed to draw the circles on the wraparound spot; theta can be greater than 2*pi (when winding multiple times)
+			"""
+		if self.scaleSize and self.drawPoints:
+			
+			self.theKeys = sorted(self.bigAngleDict.keys())
+			self.totalDist = 2 * np.pi * self.chordSize
+			self.theAngles = np.linspace(0 + self.pointRotation, self.totalDist + self.pointRotation, self.scaleSize + 1)
+			self.basicDist = self.theAngles[1]
+			self.theAngles = self.theAngles[:-1]
+			self.theRs = []
+			
+			if self.graphCommas:					# for non-ET graphs
+				self.theAngles = [self.theAngles[x] + self.graphCommas[x] for x in range(len(self.theAngles))]	 
+				
+			for a in self.theAngles:
+				self.theRs.append(self.getRvalue(a))
+			
+			self.theCoords = ChordSpace.poltocar(self.theAngles, self.theRs)
+			self.ax.scatter(*self.theCoords, s = self._CIRCLESIZE, c = 'black', alpha = self.baseAlpha)
+			
+			"""calculate the clickable radius of each circle as half the minimum distance between adjacent circles"""
+			
+			minDist = 10000
+			
+			for i in range(len(self.theCoords[0]) - 1):
+				for j in range(i+1, len(self.theCoords[0])):
+					d = euclidean_distance([self.theCoords[0][i], self.theCoords[1][i]], [self.theCoords[0][j], self.theCoords[1][j]])
+					if d < minDist:
+						minDist = d
+			
+			self._CLICKRADIUS = minDist/2.
+			
+			if self.drawTarget:
+				self.drawTarget._CLICKRADIUS = 10
+			
+			"""thePoints
+			
+				a list whose elements are [angle % 2pi, angleWithWrapAround, radius]
+				ordered chromatically (C, C#, D etc.)
+			
+			"""
+			
+			self.thePoints = [[round(x[0] % (2 * np.pi), 4)] + list(x) for x in zip(self.theAngles, self.theRs)]
+			self.orderedPoints = sorted(self.thePoints)
+			
+			"""todo: need to account for pointRotation here in the sorting!"""
+			
+			self.simpleAngles = sorted(list(set([x[0] for x in self.thePoints])))
+			self.fundamentalAngle = self.simpleAngles[1]
+			
+			self.zeroPoints = [x[1:] for x in self.thePoints if x[0] == self.thePoints[0][0]]
+			self.zeroPointNumber = len(self.zeroPoints)
+			self.crossSections = int(self.scaleSize/self.zeroPointNumber)
+			
+			"""
+		
+			The two cases of lattice:
+			
+				0 = size of chord relatively prime to size of scale (single generator)
+				1 = size of chord divides or shares a common factor with the size of scale (two generators)
+			
+			For moving around the lattice, we require extra code to manage the second generator
+			
+			"""
+			
+			self.latticeStructure = int(not(self.zeroPointNumber == 1))
+			
+			"""simple code to attach letters to circles;
+			
+				standardAdjustments manually arranges the letters so as to avoid collisions.
+			
+			"""
+			if self.labels and not self.suppressLabels:
+				if self.scaleSize > 12:
+					self.letterNames = [str(x + 1) for x in range(self.scaleSize)]
+				else:
+					if self.manualLabels:
+						self.letterNames = self.manualLabels[:]
+					elif self.isTsymmetrical:
+						self.letterNames = sorted(self.masterLetters)
+						self.letterNames = self.letterNames[self.letterNames.index('Cn'):] + self.letterNames[:self.letterNames.index('Cn')]
+						self.letterNames = [x.replace('n', '') for x in self.letterNames[:self.scaleSize]]
+					elif self.scaleSize == 5:
+						self.letterNames = [x.replace('n', '') for x in sorted(self.masterLetters[1:6])]						
+					elif self.preset != 11:
+						self.letterNames = [x.replace('n', '') for x in sorted(self.masterLetters[:self.scaleSize])]
+						self.letterNames = self.letterNames[self.letterNames.index('C'):] + self.letterNames[:self.letterNames.index('C')]
+						if self.scaleSize == 11:
+							self.letterNames[-1] = 'Bf'
+					else:
+						self.letterNames = self.masterLetters[self.masterLetters.index('I'):] + self.masterLetters[:self.masterLetters.index('I')]	
+					
+				if self.preset == 11:
+					adjustmentTable = {0: [.04, 0], 1: [-.25, 0], 2: [-.1, 0], 3: [-.025, 0], 4: [-.1, -.05], 5: [-.05, 0], 6: [0, 0], 7: [-.05, 0], 8: [-.07, -.05], 9: [-.07, 0], 11: [.15, 0]}
+				elif (self.chordSize, self.scaleSize) in self.standardAdjustments:
+					adjustmentTable = self.standardAdjustments[(self.chordSize, self.scaleSize)]
+#					print('here')
+				else:
+					adjustmentTable = {}
+				
+				self.letterNames = [self.letterNames[0]] + self.letterNames[len(self.letterNames):0:-1]
+				
+				if self.lowercase:
+					self.letterNames = [x.lower() for x in self.letterNames]
+					
+				for i in range(self.scaleSize):
+					myTheta, myR = self.thePoints[i][1:]
+					myR = myR - self.rAdjustment
+					myCoord = ChordSpace.poltocar([myTheta], [myR])	# x, y?
+					myAdjustment = adjustmentTable.get(i, [0, 0])
+					theText = self.letterNames[i]
+					if theText.count('I') > 0 or theText.count('V') > 0:
+						plainText = filter(lambda x: x in 'IViv', theText)
+						theText = filter(lambda x: x not in 'IViv', theText)
+						self.ax.text(myCoord[0][0] - .1 + myAdjustment[0], myCoord[1][0] + myAdjustment[1], plainText, alpha = self.alphaLabels.get(i, 1.), verticalalignment = 'center', horizontalalignment = 'left', fontname = 'Helvetica')
+						self.ax.text(myCoord[0][0] - .3 + myAdjustment[0], myCoord[1][0] + .04 + myAdjustment[1], theText, alpha = self.alphaLabels.get(i, 1.), verticalalignment = 'center', horizontalalignment = 'left', fontname = 'EngraverTextT')
+					else:
+						self.ax.text(myCoord[0][0] + myAdjustment[0], myCoord[1][0] + myAdjustment[1], theText, alpha = self.alphaLabels.get(i, 1.), verticalalignment = 'center', horizontalalignment = 'center', fontname = 'EngraverTextT')
+			
+			"""Print generators"""
+			if len(self.zeroPoints) > 1:
+				self.theTransps = [[int(.001 + x[0] / (2. * np.pi)), int(.001 + x[0] / self.basicDist)] for x in self.zeroPoints[1:]]
+				print("Zero sum generator", -self.theTransps[0][0], self.theTransps[0][1])
+		
+			if len(self.simpleAngles) > 1 and self.chordSize > len(self.zeroPoints):
+				myPoints = []
+				for p in self.thePoints:
+					if abs(p[0] - self.fundamentalAngle) < .001:
+						myPoints.append(p[1:])
+				self.theTransps = [[int(.001 + x[0] / (2. * np.pi)), int(.001 + x[0] / self.basicDist)] for x in myPoints]
+				print("Sum-1 generator", -self.theTransps[0][0], self.theTransps[0][1])
+			
+			"""add arrows"""
+			if self.arrows:
+				
+				self.cartesianPoints = [ChordSpace.poltocar([x[1]], [x[2]]) for x in self.orderedPoints]
+				self.cartesianPoints = [[x[0][0], x[1][0]] for x in self.cartesianPoints]
+				
+				for arrowItem in self.arrows:			# startpoint, endpoint, %of distance, newStartPoint, rotation, color
+					defaultArrow = [arrowItem[0], None, .9, None, 0, 'black']
+					newArrowItem = [arrowItem[i] if i < len(arrowItem) else defaultArrow[i] for i in range(len(defaultArrow))]
+					#newArrowItem = arrowItem + [None] * (6 - len(arrowItem))
+					i, j, pct, newStartPoint, rot, col = newArrowItem
+					if i == 'lastDest':
+						startPoint = lastDest[:]
+					else:
+						startPoint = self.cartesianPoints[i]
+						if not j:
+							j = (i + 1) % self.scaleSize
+					deltaX, deltaY = [self.cartesianPoints[j][x] - startPoint[x] for x in [0, 1]]
+					if newStartPoint != None:
+						startPoint = self.cartesianPoints[newStartPoint]
+					if rot != None:
+						deltaX, deltaY = ChordSpace.rotate([deltaX, deltaY], rot*self.fundamentalAngle)
+					lastDest = [startPoint[0] + deltaX, startPoint[1] + deltaY]
+					self.ax.arrow(startPoint[0], startPoint[1], deltaX * pct, deltaY * pct, head_width=0.2, head_length=0.2, fc=col, ec=col)
+		
+		self.ax.set_yticks([]) 
+		self.ax.set_xticks([])
+		if self.saveName:
+			plt.savefig(self.saveName, bbox_inches='tight')
+		else:
+			self.show()
+		
+	def show(self):			# would be nice to be able to reopen this, but that seems not to be possible
+		plt.ion()
+		plt.show()
+		plt.pause(.0001)
+	
+	"""NOTE OFF CODE CAUSED THE PROGRAM TO BE SLUGGISH WHEN QUITTING, waiting for the Timers to quit; also produced sonic artifacts"""
+
+	def getRvalue(self, a):
+		
+		"""utility code to get an R value for an angle a"""
+		winding = int(a / (2 * np.pi))
+		generalTheta = a % (2 * np.pi)
+		if winding == 0:
+			rCoord = self.radius
+		else:
+			rCoord = self.radius + ((self.chordSize - winding) * self.circleSeparation)
+		if generalTheta < self._GAPANGLE:
+			return rCoord
+		else:
+			for i, k in enumerate(self.theKeys):
+				if k > a:
+					rCoord = self.bigAngleDict[self.theKeys[i-1]]
+					break
+			return rCoord
+	
+	def get_maximally_even(self):
+		return [int(x) for x in [f*(1.0*self.scaleSize)/self.chordSize for f in range(self.chordSize)]]
+		
+	@staticmethod
+	def poltocar(theta, R):
+		xCoords = []
+		yCoords = []
+		for i in range(len(theta)):
+			t = theta[i]
+			r = R[i]
+			xCoords.append(r*np.sin(t))
+			yCoords.append(r*np.cos(t))
+		return [xCoords, yCoords]
+		
+	@staticmethod
+	def draw_circle(thetaMin = 0, thetaMax = 0, r = 4, rMax = -1):
+		theta = np.linspace(thetaMin, thetaMax, int((thetaMax - thetaMin) / 0.01))
+		if rMax == -1:
+			newR = [r] * len(theta)
+		else:
+			newR = np.linspace(r, rMax, len(theta))
+		myCoords = ChordSpace.poltocar(theta, newR)
+		return myCoords
+
+	@staticmethod	
+	def rotate(p, theta):
+		return [p[0]*np.cos(theta) - p[1]*np.sin(theta), p[0]*np.sin(theta) + p[1]*np.cos(theta)]
+
+	@staticmethod
+	def make_RList(diffRanges):
+		
+		"""
+		utility routine for drawing smooth curves, interpolating between one circle and noather
+		you supply a list [firstdelta, seconddelta, numberofpoints], these are deltas between successive radii points
+		
+		example: 
+		
+			self.standardRList [[0, 5, 50], [5, 7, 50]] goes from 0 to 5 in 50 steps, then 5 to 7 in 50 steps (first steep then flattening)
+		
+		this program makes a symmetrical curve, so it adds the retrograde of the input pattern (this might not be the way to do things)
+		
+		"""
+		diffSeq = []
+		rangeList = [0]
+		for r in diffRanges:
+			diffSeq += list(np.linspace(*r))
+		diffSeq += diffSeq[::-1]
+		for d in diffSeq:
+			rangeList.append(rangeList[-1] + d)
+		return [linear_map(x, [rangeList[0], rangeList[-1]], [1, 0]) for x in rangeList]
+
+	@staticmethod
+	def interpolate_between_circles(firstAngle, firstR, secondAngle, secondR, rList):
+		rList = ChordSpace.make_RList(rList)
+		tempRList = [linear_map(x, [0, 1], [firstR, secondR]) for x in rList]
+		newAngles = np.linspace(firstAngle, secondAngle, len(tempRList))
+		return newAngles, tempRList
```

### Comparing `musicntwrk-2.2.9/src/plotting/drawMultiLayerNetwork.py` & `musicntwrk-2.3.0/src/plotting/drawMultiLayerNetwork.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.9/src/plotting/drawNetwork.py` & `musicntwrk-2.3.0/src/plotting/drawNetwork.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 import numpy as np
 import networkx as nx
 import community as cm
 import matplotlib.pyplot as plt
 
 def drawNetwork(Gx=None,Gxu=None,nodes=None,edges=None,forceiter=100,grphtype='undirected',dx=10,dy=10,colormap='jet',scale=1.0,
-    layout='force',drawlabels=True,giant=False,equi=False,res=0.5,k=None,edge_labels=False,font=12):
+    layout='force',drawlabels=True,giant=False,equi=False,res=0.5,k=None,edge_labels=False,noloop=True,font=12):
 
     if grphtype == 'directed':
         if Gx == None and Gxu == None:
             Gx = nx.from_pandas_edgelist(edges,'Source','Target',['Weight'],create_using=nx.DiGraph())
             Gxu = nx.from_pandas_edgelist(edges,'Source','Target',['Weight'])
         if giant: 
             print('not implemented')
@@ -58,12 +58,13 @@
         values = [part.get(node) for node in Gx.nodes()]
     d = nx.degree(Gx)
     dsize = [(d[v]+1)*100*scale for v in Gx.nodes()]
     plt.figure(figsize=(dx, dy))
     if edge_labels:
         edge_labels = nx.get_edge_attributes(Gx, 'Label')
         nx.draw_networkx_edge_labels(Gx, pos, edge_labels, font_size=font)
+    if noloop: Gx.remove_edges_from(list(nx.selfloop_edges(Gx)))
     nx.draw_networkx(Gx,pos=pos,labels=labels,with_labels=drawlabels,cmap=plt.get_cmap(colormap),node_color=values,
                     node_size=dsize)
     plt.show()
```

### Comparing `musicntwrk-2.2.9/src/plotting/drawNetworkViz.py` & `musicntwrk-2.3.0/src/plotting/drawNetworkViz.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,28 +12,28 @@
 # in the root directory of the present distribution,
 # or http://www.gnu.org/copyleft/gpl.txt .
 #
 
 import numpy as np
 from graphviz import Digraph
 
-def drawNetworkViz(nodes,edges,view=True,seed=None,engine='circo',format='svg',size='20,20',ratio='0.9',colorlist=None):
+def drawNetworkViz(nodes,edges,view=True,seed=None,engine='circo',format='svg',strict=True,size='20,20',ratio='0.9',colorlist=None):
 
     if colorlist == None:
         colorlist=['black','red','blue','green','cyan','magenta']
     
     if seed == None:
         np.random.seed(seed)
 
     # Generate graph using GraphViz
 
-    G = Digraph(engine=engine,format=format,strict=True)
+    G = Digraph(engine=engine,format=format,strict=strict)
 
     G.attr(rankdir='LR',model='subset',ratio=ratio,size=size,pad='0.2',splines='ortho',
-           overlap='false',mode='KK')
+           overlap='false',concentrate='false',mode='KK')
     G.attr('graph',label='',fontname='Helvetica Neue',fontsize='32',labelloc='t',nodesep='0.01')
     G.attr('node', shape='rectangle',fontname='Helvetica Neue',fontsize='16')
     G.attr('edge',arrowType='normal')
 
     nodelist = []
     if not isinstance(edges,list):
         edges = [edges]
```

### Comparing `musicntwrk-2.2.9/src/plotting/drawNetworkX.py` & `musicntwrk-2.3.0/src/plotting/drawNetworkX.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.9/src/plotting/plotCC.py` & `musicntwrk-2.3.0/src/plotting/plotCC.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.9/src/plotting/plotCurveXY.py` & `musicntwrk-2.3.0/src/plotting/plotCurveXY.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.9/src/plotting/plotCurveY.py` & `musicntwrk-2.3.0/src/plotting/plotCurveY.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.9/src/plotting/plotOpsHistogram.py` & `musicntwrk-2.3.0/src/plotting/plotOpsHistogram.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.9/src/timbre/computeASCBW.py` & `musicntwrk-2.3.0/src/timbre/computeASCBW.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.9/src/timbre/computeCompMPS.py` & `musicntwrk-2.3.0/src/timbre/computeCompMPS.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 #
 def computeCompMPS(input_path,input_file,n_mels=13,barplot=True):
     # read audio files in repository and compute the MPS
     waves = list(glob.glob(os.path.join(input_path,input_file)))
     mps0 = []
     for wav in np.sort(waves):
         y, sr = librosa.load(wav)
-        S = librosa.feature.melspectrogram(y, sr=sr, n_mels=n_mels)
+        S = librosa.feature.melspectrogram(y=y, sr=sr, n_mels=n_mels)
         # Here we decompose the MPS in a one-dim component and an activation matrix
         comps, acts = librosa.decompose.decompose(S, n_components=1,sort=True)
         comps = np.reshape(comps,comps.shape[0])
         mps0.append(comps)
     mps0 = np.array(mps0)
     if barplot:
         # print the mps0 matrix for all sounds
```

### Comparing `musicntwrk-2.2.9/src/timbre/computeMFCC.py` & `musicntwrk-2.3.0/src/timbre/computeMFCC.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 def computeMFCC(input_path,input_file,nmel,ncc,zero):
     # read audio files in repository and compute the MFCC
     waves = list(glob.glob(os.path.join(input_path,input_file)))
     mfcc0 = []
     for wav in np.sort(waves):
         y, sr = librosa.load(wav)
-        S = librosa.feature.melspectrogram(y, sr=sr, n_mels=nmel)
+        S = librosa.feature.melspectrogram(y=y, sr=sr, n_mels=nmel)
         log_S = librosa.power_to_db(S, ref=np.max)
         mfcc = librosa.feature.mfcc(S=log_S, n_mfcc=ncc)
 #        # Here we take the average over a single impulse (for lack of a better measure...)
 #        mfcc0.append(np.sum(mfcc,axis=1)/mfcc.shape[1])
         # use mfcc[0] as weighting function for the average of the mfcc's over the full impulse
         mfnorm = (mfcc[0]-np.min(mfcc[0]))/np.max(mfcc[0]-np.min(mfcc[0]))
         mfcc0.append(mfcc.dot(mfnorm)/mfcc.shape[1])
```

### Comparing `musicntwrk-2.2.9/src/timbre/computeModifiedASCBW.py` & `musicntwrk-2.3.0/src/timbre/computeModifiedASCBW.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     waves = list(glob.glob(os.path.join(input_path,input_file)))
     ascbw = []
     for wav in np.sort(waves):
         y, sr = librosa.load(wav)
         maxsp = int(np.argwhere(np.abs(y) < eps)[0])
         cent = librosa.feature.spectral_centroid(y=y, sr=sr,hop_length=maxsp)
         spec_bw = librosa.feature.spectral_bandwidth(y=y, sr=sr,hop_length=maxsp)
-        S = librosa.feature.melspectrogram(y, sr=sr, n_mels=16)
+        S = librosa.feature.melspectrogram(y=y, sr=sr, n_mels=16)
         log_S = librosa.power_to_db(S, ref=np.max)
         mfcc = librosa.feature.mfcc(S=log_S, n_mfcc=13)
         try:
             a,_,_,_,_ = mfccSoundDecayPiecewise(mfcc[0],breakpoints=minimizeBKPT(mfcc[0],method=method,nstep=nstep)[1])
         except:
             print(wav)
             break
```

### Comparing `musicntwrk-2.2.9/src/timbre/computePSCC.py` & `musicntwrk-2.3.0/src/timbre/computePSCC.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.9/src/timbre/computeStandardizedMFCC.py` & `musicntwrk-2.3.0/src/timbre/computeStandardizedPSCC.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,52 +13,43 @@
 # or http://www.gnu.org/copyleft/gpl.txt .
 #
 
 import numpy as np
 import glob, os
 import librosa
 
-def computeStandardizedMFCC(input_path,input_file,nmel,nmfcc,lmax,maxi,nbins):
+def computeStandardizedPSCC(input_path,input_file,ncc,lmax,maxi,nbins):
     # read audio files in repository and compute the standardized (equal number of samples per file) 
-    # and normalized MFCC
+    # and normalized PSCC
     waves = list(glob.glob(os.path.join(input_path,input_file)))
     wf = []
     for wav in np.sort(waves):
         y, sr = librosa.load(wav)
         wf.append(y)
-    wf = np.asarray(wf)
+    wf = np.array(wf)
     # standardization of the number of sample in every sound wav
     if lmax == None:
         lwf = []
         for n in range(wf.shape[0]):
             lwf.append(wf[n].shape[0])
         lwf = np.asarray(lwf)
         lmax = np.max(lwf)
-    mfcc = []
+    pscc = []
     for n in range(wf.shape[0]):
         if wf[n].shape[0] <= lmax:
             wtmp = np.pad(wf[n], (0, lmax-wf[n].shape[0]), 'constant')
         else:
             wtmp = wf[n][:lmax]
         if nbins == None:
             hopl = 512
         else:
-            hopl = hopl = int((lmax/nbins)*2/2+1) #round(int(lmax/nbins)/2)*2
-        S = librosa.feature.melspectrogram(wtmp, sr=sr, n_mels=nmel,hop_length=hopl)
-        log_S = librosa.power_to_db(S, ref=np.max)
-        temp = librosa.feature.mfcc(S=log_S, n_mfcc=nmfcc)
-        # normalize mfcc[0] first
-        try:
-#            print(n,np.max(temp[0]),np.min(temp[0]))
-            temp[0] = (temp[0]-np.min(temp[0]))/(np.max(temp[0])-np.min(temp[0]))
-        except:
-            print(n,np.max(temp[0]),np.min(temp[0]))
-#        temp = np.abs(temp)
-#        if maxi == None:
-#            maxtemp = np.max(temp[1:])
-#        else:
-#            maxtemp = maxi
-#        temp[1:] = temp[1:]/maxtemp
-        mfcc.append(temp)
-    mfcc = np.asarray(mfcc)
-    return(np.sort(waves),mfcc,lmax)
-
+            hopl = int((lmax/nbins)*2/2+1)
+        # power (energy-squared) spectrogram
+        D = np.abs(librosa.stft(wtmp,hop_length=hopl))**2
+        log_D = librosa.power_to_db(D, ref=np.max)
+        temp = librosa.feature.mfcc(S=log_D, n_mfcc=ncc)
+        # normalize pscc[0] first
+        temp[0] = (temp[0]-np.min(temp[0]))/(np.max(temp[0])-np.min(temp[0]))
+        pscc.append(temp)
+    pscc = np.asarray(pscc)
+    return(np.sort(waves),pscc,lmax)
+
```

### Comparing `musicntwrk-2.2.9/src/timbre/computeStandardizedMFPS.py` & `musicntwrk-2.3.0/src/timbre/computeStandardizedMFPS.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     # read audio files in repository and compute the standardized (equal number of samples per file) 
     # and normalized MFCC
     waves = list(glob.glob(os.path.join(input_path,input_file)))
     wf = []
     for wav in np.sort(waves):
         y, sr = librosa.load(wav)
         wf.append(y)
-    wf = np.asarray(wf)
+    wf = np.array(wf)
     # standardization of the number of sample in every sound wav
     if lmax == None:
         lwf = []
         for n in range(wf.shape[0]):
             lwf.append(wf[n].shape[0])
         lwf = np.asarray(lwf)
         lmax = np.max(lwf)
@@ -39,13 +39,13 @@
             wtmp = np.pad(wf[n], (0, lmax-wf[n].shape[0]), 'constant')
         else:
             wtmp = wf[n][:lmax]
         if nbins == None:
             hopl = 512
         else:
             hopl = hopl = int((lmax/nbins)*2/2+1) #round(int(lmax/nbins)/2)*2
-        S = librosa.feature.melspectrogram(wtmp, sr=sr, n_mels=nmel,hop_length=hopl)
+        S = librosa.feature.melspectrogram(y=wtmp, sr=sr, n_mels=nmel,hop_length=hopl)
         log_S = librosa.power_to_db(S, ref=np.max)
         mfcc.append(log_S)
     mfcc = np.asarray(mfcc)
     return(np.sort(waves),mfcc,lmax)
```

### Comparing `musicntwrk-2.2.9/src/timbre/computeStandardizedPSCC.py` & `musicntwrk-2.3.0/src/timbre/computeStandardizedMFCC.py`

 * *Files 22% similar despite different names*

```diff
@@ -13,43 +13,52 @@
 # or http://www.gnu.org/copyleft/gpl.txt .
 #
 
 import numpy as np
 import glob, os
 import librosa
 
-def computeStandardizedPSCC(input_path,input_file,ncc,lmax,maxi,nbins):
+def computeStandardizedMFCC(input_path,input_file,nmel,nmfcc,lmax,maxi,nbins):
     # read audio files in repository and compute the standardized (equal number of samples per file) 
-    # and normalized PSCC
+    # and normalized MFCC
     waves = list(glob.glob(os.path.join(input_path,input_file)))
     wf = []
     for wav in np.sort(waves):
         y, sr = librosa.load(wav)
-        wf.append(y)
-    wf = np.asarray(wf)
+        wf.append(np.array(y))
+#   wf = np.array(wf)
     # standardization of the number of sample in every sound wav
     if lmax == None:
         lwf = []
-        for n in range(wf.shape[0]):
+        for n in range(len(wf)):
             lwf.append(wf[n].shape[0])
         lwf = np.asarray(lwf)
         lmax = np.max(lwf)
-    pscc = []
-    for n in range(wf.shape[0]):
+    mfcc = []
+    for n in range(len(wf)):
         if wf[n].shape[0] <= lmax:
             wtmp = np.pad(wf[n], (0, lmax-wf[n].shape[0]), 'constant')
         else:
             wtmp = wf[n][:lmax]
         if nbins == None:
             hopl = 512
         else:
-            hopl = int((lmax/nbins)*2/2+1)
-        # power (energy-squared) spectrogram
-        D = np.abs(librosa.stft(wtmp,hop_length=hopl))**2
-        log_D = librosa.power_to_db(D, ref=np.max)
-        temp = librosa.feature.mfcc(S=log_D, n_mfcc=ncc)
-        # normalize pscc[0] first
-        temp[0] = (temp[0]-np.min(temp[0]))/(np.max(temp[0])-np.min(temp[0]))
-        pscc.append(temp)
-    pscc = np.asarray(pscc)
-    return(np.sort(waves),pscc,lmax)
-        
+            hopl = hopl = int((lmax/nbins)*2/2+1) #round(int(lmax/nbins)/2)*2
+        S = librosa.feature.melspectrogram(y=wtmp, sr=sr, n_mels=nmel,hop_length=hopl)
+        log_S = librosa.power_to_db(S, ref=np.max)
+        temp = librosa.feature.mfcc(S=log_S, n_mfcc=nmfcc)
+        # normalize mfcc[0] first
+        try:
+#            print(n,np.max(temp[0]),np.min(temp[0]))
+            temp[0] = (temp[0]-np.min(temp[0]))/(np.max(temp[0])-np.min(temp[0]))
+        except:
+            print(n,np.max(temp[0]),np.min(temp[0]))
+#        temp = np.abs(temp)
+#        if maxi == None:
+#            maxtemp = np.max(temp[1:])
+#        else:
+#            maxtemp = maxi
+#        temp[1:] = temp[1:]/maxtemp
+        mfcc.append(temp)
+    mfcc = np.asarray(mfcc)
+    return(np.sort(waves),mfcc,lmax)
+
```

### Comparing `musicntwrk-2.2.9/src/timbre/mfccSoundDecay.py` & `musicntwrk-2.3.0/src/timbre/mfccSoundDecay.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.9/src/timbre/mfccSoundDecayOptimal.py` & `musicntwrk-2.3.0/src/timbre/mfccSoundDecayOptimal.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.9/src/timbre/mfccSoundDecayPiecewise.py` & `musicntwrk-2.3.0/src/timbre/mfccSoundDecayPiecewise.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.9/src/timbre/minimizeBKPT.py` & `musicntwrk-2.3.0/src/timbre/minimizeBKPT.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.9/src/timbre/normSoundDecay.py` & `musicntwrk-2.3.0/src/timbre/normSoundDecay.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.9/src/timbre/normSoundDecay2.py` & `musicntwrk-2.3.0/src/timbre/normSoundDecay2.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.9/src/utils/SegmentedLinearReg.py` & `musicntwrk-2.3.0/src/utils/SegmentedLinearReg.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.9/src/utils/Sublists.py` & `musicntwrk-2.3.0/src/utils/Sublists.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.9/src/utils/communications.py` & `musicntwrk-2.3.0/src/utils/communications.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.9/src/utils/diffusionEntropyAnalyis.py` & `musicntwrk-2.3.0/src/utils/diffusionEntropyAnalyis.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.9/src/utils/diffusionEntropyAnalyisNew.py` & `musicntwrk-2.3.0/src/utils/diffusionEntropyAnalyisNew.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.9/src/utils/entropyKLdiv.py` & `musicntwrk-2.3.0/src/utils/entropyKLdiv.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.9/src/utils/extractByString.py` & `musicntwrk-2.3.0/src/utils/extractByString.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.9/src/utils/fetchWaves.py` & `musicntwrk-2.3.0/src/utils/fetchWaves.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.9/src/utils/findLengthMax.py` & `musicntwrk-2.3.0/src/utils/findLengthMax.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.9/src/utils/flatten.py` & `musicntwrk-2.3.0/src/utils/flatten.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.9/src/utils/floatize.py` & `musicntwrk-2.3.0/src/utils/floatize.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.9/src/utils/generalizedOpsHistogram.py` & `musicntwrk-2.3.0/src/utils/generalizedOpsHistogram.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.9/src/utils/generalizedOpsName.py` & `musicntwrk-2.3.0/src/utils/generalizedOpsName.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.9/src/utils/init_list_of_objects.py` & `musicntwrk-2.3.0/src/utils/init_list_of_objects.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.9/src/utils/load_balancing.py` & `musicntwrk-2.3.0/src/utils/load_balancing.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.9/src/utils/minimalDistance.py` & `musicntwrk-2.3.0/src/utils/minimalDistance.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.9/src/utils/minimalDistanceVec.py` & `musicntwrk-2.3.0/src/utils/minimalDistanceVec.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.9/src/utils/minimalNoBijDistance.py` & `musicntwrk-2.3.0/src/utils/minimalNoBijDistance.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.9/src/utils/opsCheckByName.py` & `musicntwrk-2.3.0/src/utils/opsCheckByName.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.9/src/utils/opsCheckByNameVec.py` & `musicntwrk-2.3.0/src/utils/opsCheckByNameVec.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.9/src/utils/opsDistance.py` & `musicntwrk-2.3.0/src/utils/opsDistance.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.9/src/utils/opsHistogram.py` & `musicntwrk-2.3.0/src/utils/opsHistogram.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.9/src/utils/opsName.py` & `musicntwrk-2.3.0/src/utils/opsName.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.9/src/utils/opsNameFull.py` & `musicntwrk-2.3.0/src/utils/opsNameFull.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.9/src/utils/opsNameVec.py` & `musicntwrk-2.3.0/src/utils/opsNameVec.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.9/src/utils/play_with_simpleaudio.py` & `musicntwrk-2.3.0/src/utils/play_with_simpleaudio.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.9/src/utils/powerFit.py` & `musicntwrk-2.3.0/src/utils/powerFit.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.9/src/utils/rhythmDistance.py` & `musicntwrk-2.3.0/src/utils/rhythmDistance.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.9/src/utils/scaleFreeFit.py` & `musicntwrk-2.3.0/src/utils/scaleFreeFit.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.9/src/utils/score2vLead.py` & `musicntwrk-2.3.0/src/utils/score2vLead.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.9/src/utils/str2float.py` & `musicntwrk-2.3.0/src/utils/str2float.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.9/src/utils/str2frac.py` & `musicntwrk-2.3.0/src/utils/str2frac.py`

 * *Files identical despite different names*

### Comparing `musicntwrk-2.2.9/src/utils/vectorDistance.py` & `musicntwrk-2.3.0/src/utils/vectorDistance.py`

 * *Files identical despite different names*

