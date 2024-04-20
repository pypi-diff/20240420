# Comparing `tmp/bullmq-2.7.1.tar.gz` & `tmp/bullmq-2.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bullmq-2.7.1.tar", last modified: Thu Apr 18 01:24:08 2024, max compression
+gzip compressed data, was "bullmq-2.7.2.tar", last modified: Sat Apr 20 05:32:55 2024, max compression
```

## Comparing `bullmq-2.7.1.tar` & `bullmq-2.7.2.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 01:24:08.097629 bullmq-2.7.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-04-18 01:24:08.097629 bullmq-2.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      999 2024-04-18 01:22:34.000000 bullmq-2.7.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 01:24:08.089629 bullmq-2.7.1/bullmq/
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-18 01:24:06.000000 bullmq-2.7.1/bullmq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-04-18 01:22:34.000000 bullmq-2.7.1/bullmq/backoffs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 01:24:08.097629 bullmq-2.7.1/bullmq/commands/
--rw-r--r--   0 runner    (1001) docker     (127)    10913 2024-04-18 01:23:46.000000 bullmq-2.7.1/bullmq/commands/addDelayedJob-6.lua
--rw-r--r--   0 runner    (1001) docker     (127)    10334 2024-04-18 01:23:46.000000 bullmq-2.7.1/bullmq/commands/addParentJob-4.lua
--rw-r--r--   0 runner    (1001) docker     (127)    10691 2024-04-18 01:23:46.000000 bullmq-2.7.1/bullmq/commands/addPrioritizedJob-7.lua
--rw-r--r--   0 runner    (1001) docker     (127)    10780 2024-04-18 01:23:46.000000 bullmq-2.7.1/bullmq/commands/addStandardJob-7.lua
--rw-r--r--   0 runner    (1001) docker     (127)     2400 2024-04-18 01:23:46.000000 bullmq-2.7.1/bullmq/commands/changeDelay-4.lua
--rw-r--r--   0 runner    (1001) docker     (127)     2242 2024-04-18 01:23:46.000000 bullmq-2.7.1/bullmq/commands/changePriority-6.lua
--rw-r--r--   0 runner    (1001) docker     (127)     9965 2024-04-18 01:23:46.000000 bullmq-2.7.1/bullmq/commands/cleanJobsInSet-2.lua
--rw-r--r--   0 runner    (1001) docker     (127)     6412 2024-04-18 01:23:46.000000 bullmq-2.7.1/bullmq/commands/drain-4.lua
--rw-r--r--   0 runner    (1001) docker     (127)      501 2024-04-18 01:23:46.000000 bullmq-2.7.1/bullmq/commands/extendLock-2.lua
--rw-r--r--   0 runner    (1001) docker     (127)      868 2024-04-18 01:23:46.000000 bullmq-2.7.1/bullmq/commands/getCounts-1.lua
--rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-04-18 01:23:46.000000 bullmq-2.7.1/bullmq/commands/getRanges-1.lua
--rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-04-18 01:23:46.000000 bullmq-2.7.1/bullmq/commands/getState-8.lua
--rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-04-18 01:23:46.000000 bullmq-2.7.1/bullmq/commands/getStateV2-8.lua
--rw-r--r--   0 runner    (1001) docker     (127)      897 2024-04-18 01:23:46.000000 bullmq-2.7.1/bullmq/commands/isFinished-3.lua
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-18 01:23:46.000000 bullmq-2.7.1/bullmq/commands/isJobInList-1.lua
--rw-r--r--   0 runner    (1001) docker     (127)     2706 2024-04-18 01:23:46.000000 bullmq-2.7.1/bullmq/commands/moveJobFromActiveToWait-10.lua
--rw-r--r--   0 runner    (1001) docker     (127)     2931 2024-04-18 01:23:46.000000 bullmq-2.7.1/bullmq/commands/moveJobsToWait-7.lua
--rw-r--r--   0 runner    (1001) docker     (127)    17377 2024-04-18 01:23:46.000000 bullmq-2.7.1/bullmq/commands/moveStalledJobsToWait-9.lua
--rw-r--r--   0 runner    (1001) docker     (127)     7295 2024-04-18 01:23:46.000000 bullmq-2.7.1/bullmq/commands/moveToActive-11.lua
--rw-r--r--   0 runner    (1001) docker     (127)     3439 2024-04-18 01:23:46.000000 bullmq-2.7.1/bullmq/commands/moveToDelayed-8.lua
--rw-r--r--   0 runner    (1001) docker     (127)    25897 2024-04-18 01:23:46.000000 bullmq-2.7.1/bullmq/commands/moveToFinished-14.lua
--rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-04-18 01:23:46.000000 bullmq-2.7.1/bullmq/commands/moveToWaitingChildren-5.lua
--rw-r--r--   0 runner    (1001) docker     (127)     8393 2024-04-18 01:23:46.000000 bullmq-2.7.1/bullmq/commands/obliterate-2.lua
--rw-r--r--   0 runner    (1001) docker     (127)     3742 2024-04-18 01:23:46.000000 bullmq-2.7.1/bullmq/commands/paginate-1.lua
--rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-04-18 01:23:46.000000 bullmq-2.7.1/bullmq/commands/pause-7.lua
--rw-r--r--   0 runner    (1001) docker     (127)     2673 2024-04-18 01:23:46.000000 bullmq-2.7.1/bullmq/commands/promote-8.lua
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-18 01:23:46.000000 bullmq-2.7.1/bullmq/commands/releaseLock-1.lua
--rw-r--r--   0 runner    (1001) docker     (127)     4903 2024-04-18 01:23:46.000000 bullmq-2.7.1/bullmq/commands/removeChildDependency-1.lua
--rw-r--r--   0 runner    (1001) docker     (127)     9216 2024-04-18 01:23:46.000000 bullmq-2.7.1/bullmq/commands/removeJob-1.lua
--rw-r--r--   0 runner    (1001) docker     (127)      690 2024-04-18 01:23:46.000000 bullmq-2.7.1/bullmq/commands/removeRepeatable-2.lua
--rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-04-18 01:23:46.000000 bullmq-2.7.1/bullmq/commands/reprocessJob-7.lua
--rw-r--r--   0 runner    (1001) docker     (127)     4917 2024-04-18 01:23:46.000000 bullmq-2.7.1/bullmq/commands/retryJob-11.lua
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-18 01:23:46.000000 bullmq-2.7.1/bullmq/commands/saveStacktrace-1.lua
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-18 01:23:46.000000 bullmq-2.7.1/bullmq/commands/updateData-1.lua
--rw-r--r--   0 runner    (1001) docker     (127)      915 2024-04-18 01:23:46.000000 bullmq-2.7.1/bullmq/commands/updateProgress-3.lua
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 01:24:08.097629 bullmq-2.7.1/bullmq/custom_errors/
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-18 01:22:34.000000 bullmq-2.7.1/bullmq/custom_errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-18 01:22:34.000000 bullmq-2.7.1/bullmq/custom_errors/waiting_children_error.py
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-18 01:22:34.000000 bullmq-2.7.1/bullmq/error_code.py
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-18 01:22:34.000000 bullmq-2.7.1/bullmq/event_emitter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4621 2024-04-18 01:22:34.000000 bullmq-2.7.1/bullmq/flow_producer.py
--rw-r--r--   0 runner    (1001) docker     (127)    10416 2024-04-18 01:22:34.000000 bullmq-2.7.1/bullmq/job.py
--rw-r--r--   0 runner    (1001) docker     (127)    10683 2024-04-18 01:22:34.000000 bullmq-2.7.1/bullmq/queue.py
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-04-18 01:22:34.000000 bullmq-2.7.1/bullmq/queue_keys.py
--rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-04-18 01:22:34.000000 bullmq-2.7.1/bullmq/redis_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)    24556 2024-04-18 01:22:34.000000 bullmq-2.7.1/bullmq/scripts.py
--rw-r--r--   0 runner    (1001) docker     (127)      699 2024-04-18 01:22:34.000000 bullmq-2.7.1/bullmq/timer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 01:24:08.097629 bullmq-2.7.1/bullmq/types/
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-18 01:22:34.000000 bullmq-2.7.1/bullmq/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-18 01:22:34.000000 bullmq-2.7.1/bullmq/types/backoff_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     1920 2024-04-18 01:22:34.000000 bullmq-2.7.1/bullmq/types/job_options.py
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-18 01:22:34.000000 bullmq-2.7.1/bullmq/types/keep_jobs.py
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-18 01:22:34.000000 bullmq-2.7.1/bullmq/types/promote_jobs_options.py
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-18 01:22:34.000000 bullmq-2.7.1/bullmq/types/queue_options.py
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-18 01:22:34.000000 bullmq-2.7.1/bullmq/types/retry_jobs_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-04-18 01:22:34.000000 bullmq-2.7.1/bullmq/types/worker_options.py
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-18 01:22:34.000000 bullmq-2.7.1/bullmq/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    10302 2024-04-18 01:22:34.000000 bullmq-2.7.1/bullmq/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 01:24:08.097629 bullmq-2.7.1/bullmq.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-04-18 01:24:08.000000 bullmq-2.7.1/bullmq.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1997 2024-04-18 01:24:08.000000 bullmq-2.7.1/bullmq.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 01:24:08.000000 bullmq-2.7.1/bullmq.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-18 01:24:08.000000 bullmq-2.7.1/bullmq.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-18 01:24:08.000000 bullmq-2.7.1/bullmq.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-04-18 01:24:06.000000 bullmq-2.7.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 01:24:08.097629 bullmq-2.7.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-18 01:22:34.000000 bullmq-2.7.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 05:32:55.263938 bullmq-2.7.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-04-20 05:32:55.263938 bullmq-2.7.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2024-04-20 05:31:28.000000 bullmq-2.7.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 05:32:55.251938 bullmq-2.7.2/bullmq/
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-20 05:32:53.000000 bullmq-2.7.2/bullmq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-04-20 05:31:28.000000 bullmq-2.7.2/bullmq/backoffs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 05:32:55.259938 bullmq-2.7.2/bullmq/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)    10913 2024-04-20 05:32:27.000000 bullmq-2.7.2/bullmq/commands/addDelayedJob-6.lua
+-rw-r--r--   0 runner    (1001) docker     (127)    10334 2024-04-20 05:32:27.000000 bullmq-2.7.2/bullmq/commands/addParentJob-4.lua
+-rw-r--r--   0 runner    (1001) docker     (127)    10691 2024-04-20 05:32:27.000000 bullmq-2.7.2/bullmq/commands/addPrioritizedJob-7.lua
+-rw-r--r--   0 runner    (1001) docker     (127)    10780 2024-04-20 05:32:27.000000 bullmq-2.7.2/bullmq/commands/addStandardJob-7.lua
+-rw-r--r--   0 runner    (1001) docker     (127)     2400 2024-04-20 05:32:27.000000 bullmq-2.7.2/bullmq/commands/changeDelay-4.lua
+-rw-r--r--   0 runner    (1001) docker     (127)     2242 2024-04-20 05:32:27.000000 bullmq-2.7.2/bullmq/commands/changePriority-6.lua
+-rw-r--r--   0 runner    (1001) docker     (127)     9965 2024-04-20 05:32:27.000000 bullmq-2.7.2/bullmq/commands/cleanJobsInSet-2.lua
+-rw-r--r--   0 runner    (1001) docker     (127)     6412 2024-04-20 05:32:27.000000 bullmq-2.7.2/bullmq/commands/drain-4.lua
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-04-20 05:32:27.000000 bullmq-2.7.2/bullmq/commands/extendLock-2.lua
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-04-20 05:32:27.000000 bullmq-2.7.2/bullmq/commands/getCounts-1.lua
+-rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-04-20 05:32:27.000000 bullmq-2.7.2/bullmq/commands/getRanges-1.lua
+-rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-04-20 05:32:27.000000 bullmq-2.7.2/bullmq/commands/getState-8.lua
+-rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-04-20 05:32:27.000000 bullmq-2.7.2/bullmq/commands/getStateV2-8.lua
+-rw-r--r--   0 runner    (1001) docker     (127)      897 2024-04-20 05:32:27.000000 bullmq-2.7.2/bullmq/commands/isFinished-3.lua
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-20 05:32:27.000000 bullmq-2.7.2/bullmq/commands/isJobInList-1.lua
+-rw-r--r--   0 runner    (1001) docker     (127)     2706 2024-04-20 05:32:27.000000 bullmq-2.7.2/bullmq/commands/moveJobFromActiveToWait-10.lua
+-rw-r--r--   0 runner    (1001) docker     (127)     2931 2024-04-20 05:32:27.000000 bullmq-2.7.2/bullmq/commands/moveJobsToWait-7.lua
+-rw-r--r--   0 runner    (1001) docker     (127)    17377 2024-04-20 05:32:27.000000 bullmq-2.7.2/bullmq/commands/moveStalledJobsToWait-9.lua
+-rw-r--r--   0 runner    (1001) docker     (127)     7295 2024-04-20 05:32:27.000000 bullmq-2.7.2/bullmq/commands/moveToActive-11.lua
+-rw-r--r--   0 runner    (1001) docker     (127)     3439 2024-04-20 05:32:27.000000 bullmq-2.7.2/bullmq/commands/moveToDelayed-8.lua
+-rw-r--r--   0 runner    (1001) docker     (127)    25897 2024-04-20 05:32:27.000000 bullmq-2.7.2/bullmq/commands/moveToFinished-14.lua
+-rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-04-20 05:32:27.000000 bullmq-2.7.2/bullmq/commands/moveToWaitingChildren-5.lua
+-rw-r--r--   0 runner    (1001) docker     (127)     8393 2024-04-20 05:32:27.000000 bullmq-2.7.2/bullmq/commands/obliterate-2.lua
+-rw-r--r--   0 runner    (1001) docker     (127)     3742 2024-04-20 05:32:27.000000 bullmq-2.7.2/bullmq/commands/paginate-1.lua
+-rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-04-20 05:32:27.000000 bullmq-2.7.2/bullmq/commands/pause-7.lua
+-rw-r--r--   0 runner    (1001) docker     (127)     2673 2024-04-20 05:32:27.000000 bullmq-2.7.2/bullmq/commands/promote-8.lua
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-20 05:32:27.000000 bullmq-2.7.2/bullmq/commands/releaseLock-1.lua
+-rw-r--r--   0 runner    (1001) docker     (127)     4903 2024-04-20 05:32:27.000000 bullmq-2.7.2/bullmq/commands/removeChildDependency-1.lua
+-rw-r--r--   0 runner    (1001) docker     (127)     9216 2024-04-20 05:32:27.000000 bullmq-2.7.2/bullmq/commands/removeJob-1.lua
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-04-20 05:32:27.000000 bullmq-2.7.2/bullmq/commands/removeRepeatable-2.lua
+-rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-04-20 05:32:27.000000 bullmq-2.7.2/bullmq/commands/reprocessJob-7.lua
+-rw-r--r--   0 runner    (1001) docker     (127)     4917 2024-04-20 05:32:27.000000 bullmq-2.7.2/bullmq/commands/retryJob-11.lua
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-20 05:32:27.000000 bullmq-2.7.2/bullmq/commands/saveStacktrace-1.lua
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-20 05:32:27.000000 bullmq-2.7.2/bullmq/commands/updateData-1.lua
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-04-20 05:32:27.000000 bullmq-2.7.2/bullmq/commands/updateProgress-3.lua
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 05:32:55.259938 bullmq-2.7.2/bullmq/custom_errors/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-20 05:31:28.000000 bullmq-2.7.2/bullmq/custom_errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-20 05:31:28.000000 bullmq-2.7.2/bullmq/custom_errors/waiting_children_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-20 05:31:28.000000 bullmq-2.7.2/bullmq/error_code.py
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-20 05:31:28.000000 bullmq-2.7.2/bullmq/event_emitter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4621 2024-04-20 05:31:28.000000 bullmq-2.7.2/bullmq/flow_producer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10416 2024-04-20 05:31:28.000000 bullmq-2.7.2/bullmq/job.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10683 2024-04-20 05:31:28.000000 bullmq-2.7.2/bullmq/queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-04-20 05:31:28.000000 bullmq-2.7.2/bullmq/queue_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-04-20 05:31:28.000000 bullmq-2.7.2/bullmq/redis_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24556 2024-04-20 05:31:28.000000 bullmq-2.7.2/bullmq/scripts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-04-20 05:31:28.000000 bullmq-2.7.2/bullmq/timer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 05:32:55.263938 bullmq-2.7.2/bullmq/types/
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-20 05:31:28.000000 bullmq-2.7.2/bullmq/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-20 05:31:28.000000 bullmq-2.7.2/bullmq/types/backoff_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1920 2024-04-20 05:31:28.000000 bullmq-2.7.2/bullmq/types/job_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-20 05:31:28.000000 bullmq-2.7.2/bullmq/types/keep_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-20 05:31:28.000000 bullmq-2.7.2/bullmq/types/promote_jobs_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-20 05:31:28.000000 bullmq-2.7.2/bullmq/types/queue_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-20 05:31:28.000000 bullmq-2.7.2/bullmq/types/retry_jobs_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-04-20 05:31:28.000000 bullmq-2.7.2/bullmq/types/worker_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-20 05:31:28.000000 bullmq-2.7.2/bullmq/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10296 2024-04-20 05:31:28.000000 bullmq-2.7.2/bullmq/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 05:32:55.263938 bullmq-2.7.2/bullmq.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-04-20 05:32:55.000000 bullmq-2.7.2/bullmq.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1997 2024-04-20 05:32:55.000000 bullmq-2.7.2/bullmq.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 05:32:55.000000 bullmq-2.7.2/bullmq.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-20 05:32:55.000000 bullmq-2.7.2/bullmq.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-20 05:32:55.000000 bullmq-2.7.2/bullmq.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-04-20 05:32:53.000000 bullmq-2.7.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 05:32:55.263938 bullmq-2.7.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-20 05:31:28.000000 bullmq-2.7.2/setup.py
```

### Comparing `bullmq-2.7.1/PKG-INFO` & `bullmq-2.7.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bullmq
-Version: 2.7.1
+Version: 2.7.2
 Summary: BullMQ for Python
 Author-email: "Taskforce.sh Inc." <manast@taskforce.sh>
 Project-URL: Homepage, https://bullmq.io
 Project-URL: Bug Tracker, https://github.com/taskforcesh/bullmq/issues
 Keywords: python,bullmq,queues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `bullmq-2.7.1/README.md` & `bullmq-2.7.2/README.md`

 * *Files identical despite different names*

### Comparing `bullmq-2.7.1/bullmq/backoffs.py` & `bullmq-2.7.2/bullmq/backoffs.py`

 * *Files identical despite different names*

### Comparing `bullmq-2.7.1/bullmq/commands/addDelayedJob-6.lua` & `bullmq-2.7.2/bullmq/commands/addDelayedJob-6.lua`

 * *Files identical despite different names*

### Comparing `bullmq-2.7.1/bullmq/commands/addParentJob-4.lua` & `bullmq-2.7.2/bullmq/commands/addParentJob-4.lua`

 * *Files identical despite different names*

### Comparing `bullmq-2.7.1/bullmq/commands/addPrioritizedJob-7.lua` & `bullmq-2.7.2/bullmq/commands/addPrioritizedJob-7.lua`

 * *Files identical despite different names*

### Comparing `bullmq-2.7.1/bullmq/commands/addStandardJob-7.lua` & `bullmq-2.7.2/bullmq/commands/addStandardJob-7.lua`

 * *Files identical despite different names*

### Comparing `bullmq-2.7.1/bullmq/commands/changeDelay-4.lua` & `bullmq-2.7.2/bullmq/commands/changeDelay-4.lua`

 * *Files identical despite different names*

### Comparing `bullmq-2.7.1/bullmq/commands/changePriority-6.lua` & `bullmq-2.7.2/bullmq/commands/changePriority-6.lua`

 * *Files identical despite different names*

### Comparing `bullmq-2.7.1/bullmq/commands/cleanJobsInSet-2.lua` & `bullmq-2.7.2/bullmq/commands/cleanJobsInSet-2.lua`

 * *Files identical despite different names*

### Comparing `bullmq-2.7.1/bullmq/commands/drain-4.lua` & `bullmq-2.7.2/bullmq/commands/drain-4.lua`

 * *Files identical despite different names*

### Comparing `bullmq-2.7.1/bullmq/commands/getCounts-1.lua` & `bullmq-2.7.2/bullmq/commands/getCounts-1.lua`

 * *Files identical despite different names*

### Comparing `bullmq-2.7.1/bullmq/commands/getRanges-1.lua` & `bullmq-2.7.2/bullmq/commands/getRanges-1.lua`

 * *Files identical despite different names*

### Comparing `bullmq-2.7.1/bullmq/commands/getState-8.lua` & `bullmq-2.7.2/bullmq/commands/getState-8.lua`

 * *Files identical despite different names*

### Comparing `bullmq-2.7.1/bullmq/commands/getStateV2-8.lua` & `bullmq-2.7.2/bullmq/commands/getStateV2-8.lua`

 * *Files identical despite different names*

### Comparing `bullmq-2.7.1/bullmq/commands/isFinished-3.lua` & `bullmq-2.7.2/bullmq/commands/isFinished-3.lua`

 * *Files identical despite different names*

### Comparing `bullmq-2.7.1/bullmq/commands/moveJobFromActiveToWait-10.lua` & `bullmq-2.7.2/bullmq/commands/moveJobFromActiveToWait-10.lua`

 * *Files identical despite different names*

### Comparing `bullmq-2.7.1/bullmq/commands/moveJobsToWait-7.lua` & `bullmq-2.7.2/bullmq/commands/moveJobsToWait-7.lua`

 * *Files identical despite different names*

### Comparing `bullmq-2.7.1/bullmq/commands/moveStalledJobsToWait-9.lua` & `bullmq-2.7.2/bullmq/commands/moveStalledJobsToWait-9.lua`

 * *Files identical despite different names*

### Comparing `bullmq-2.7.1/bullmq/commands/moveToActive-11.lua` & `bullmq-2.7.2/bullmq/commands/moveToActive-11.lua`

 * *Files identical despite different names*

### Comparing `bullmq-2.7.1/bullmq/commands/moveToDelayed-8.lua` & `bullmq-2.7.2/bullmq/commands/moveToDelayed-8.lua`

 * *Files identical despite different names*

### Comparing `bullmq-2.7.1/bullmq/commands/moveToFinished-14.lua` & `bullmq-2.7.2/bullmq/commands/moveToFinished-14.lua`

 * *Files identical despite different names*

### Comparing `bullmq-2.7.1/bullmq/commands/moveToWaitingChildren-5.lua` & `bullmq-2.7.2/bullmq/commands/moveToWaitingChildren-5.lua`

 * *Files identical despite different names*

### Comparing `bullmq-2.7.1/bullmq/commands/obliterate-2.lua` & `bullmq-2.7.2/bullmq/commands/obliterate-2.lua`

 * *Files identical despite different names*

### Comparing `bullmq-2.7.1/bullmq/commands/paginate-1.lua` & `bullmq-2.7.2/bullmq/commands/paginate-1.lua`

 * *Files identical despite different names*

### Comparing `bullmq-2.7.1/bullmq/commands/pause-7.lua` & `bullmq-2.7.2/bullmq/commands/pause-7.lua`

 * *Files identical despite different names*

### Comparing `bullmq-2.7.1/bullmq/commands/promote-8.lua` & `bullmq-2.7.2/bullmq/commands/promote-8.lua`

 * *Files identical despite different names*

### Comparing `bullmq-2.7.1/bullmq/commands/removeChildDependency-1.lua` & `bullmq-2.7.2/bullmq/commands/removeChildDependency-1.lua`

 * *Files identical despite different names*

### Comparing `bullmq-2.7.1/bullmq/commands/removeJob-1.lua` & `bullmq-2.7.2/bullmq/commands/removeJob-1.lua`

 * *Files identical despite different names*

### Comparing `bullmq-2.7.1/bullmq/commands/removeRepeatable-2.lua` & `bullmq-2.7.2/bullmq/commands/removeRepeatable-2.lua`

 * *Files identical despite different names*

### Comparing `bullmq-2.7.1/bullmq/commands/reprocessJob-7.lua` & `bullmq-2.7.2/bullmq/commands/reprocessJob-7.lua`

 * *Files identical despite different names*

### Comparing `bullmq-2.7.1/bullmq/commands/retryJob-11.lua` & `bullmq-2.7.2/bullmq/commands/retryJob-11.lua`

 * *Files identical despite different names*

### Comparing `bullmq-2.7.1/bullmq/commands/updateProgress-3.lua` & `bullmq-2.7.2/bullmq/commands/updateProgress-3.lua`

 * *Files identical despite different names*

### Comparing `bullmq-2.7.1/bullmq/event_emitter.py` & `bullmq-2.7.2/bullmq/event_emitter.py`

 * *Files identical despite different names*

### Comparing `bullmq-2.7.1/bullmq/flow_producer.py` & `bullmq-2.7.2/bullmq/flow_producer.py`

 * *Files identical despite different names*

### Comparing `bullmq-2.7.1/bullmq/job.py` & `bullmq-2.7.2/bullmq/job.py`

 * *Files identical despite different names*

### Comparing `bullmq-2.7.1/bullmq/queue.py` & `bullmq-2.7.2/bullmq/queue.py`

 * *Files identical despite different names*

### Comparing `bullmq-2.7.1/bullmq/queue_keys.py` & `bullmq-2.7.2/bullmq/queue_keys.py`

 * *Files identical despite different names*

### Comparing `bullmq-2.7.1/bullmq/redis_connection.py` & `bullmq-2.7.2/bullmq/redis_connection.py`

 * *Files identical despite different names*

### Comparing `bullmq-2.7.1/bullmq/scripts.py` & `bullmq-2.7.2/bullmq/scripts.py`

 * *Files identical despite different names*

### Comparing `bullmq-2.7.1/bullmq/timer.py` & `bullmq-2.7.2/bullmq/timer.py`

 * *Files identical despite different names*

### Comparing `bullmq-2.7.1/bullmq/types/job_options.py` & `bullmq-2.7.2/bullmq/types/job_options.py`

 * *Files identical despite different names*

### Comparing `bullmq-2.7.1/bullmq/types/worker_options.py` & `bullmq-2.7.2/bullmq/types/worker_options.py`

 * *Files identical despite different names*

### Comparing `bullmq-2.7.1/bullmq/utils.py` & `bullmq-2.7.2/bullmq/utils.py`

 * *Files identical despite different names*

### Comparing `bullmq-2.7.1/bullmq/worker.py` & `bullmq-2.7.2/bullmq/worker.py`

 * *Files 2% similar despite different names*

```diff
@@ -166,15 +166,15 @@
         return 0
 
     def getBlockTimeout(self, block_until: int):
         if block_until:
             block_timeout = None
             block_delay = block_until - int(time.time() * 1000)
             if block_delay < self.minimumBlockTimeout * 1000:
-                block_timeout = minimum_block_timeout
+                return self.minimumBlockTimeout
             else:
                 block_timeout = block_delay / 1000
             # We restrict the maximum block timeout to 10 second to avoid
             # blocking the connection for too long in the case of reconnections
             # reference: https://github.com/taskforcesh/bullmq/issues/1658
             return min(block_timeout, maximum_block_timeout)
         else:
```

### Comparing `bullmq-2.7.1/bullmq.egg-info/PKG-INFO` & `bullmq-2.7.2/bullmq.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bullmq
-Version: 2.7.1
+Version: 2.7.2
 Summary: BullMQ for Python
 Author-email: "Taskforce.sh Inc." <manast@taskforce.sh>
 Project-URL: Homepage, https://bullmq.io
 Project-URL: Bug Tracker, https://github.com/taskforcesh/bullmq/issues
 Keywords: python,bullmq,queues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `bullmq-2.7.1/bullmq.egg-info/SOURCES.txt` & `bullmq-2.7.2/bullmq.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bullmq-2.7.1/pyproject.toml` & `bullmq-2.7.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "bullmq"
-version = "2.7.1"
+version = "2.7.2"
 description='BullMQ for Python'
 readme="README.md"
 authors = [
     {name = "Taskforce.sh Inc.", email = "manast@taskforce.sh"},
 ]
 requires-python = ">=3.10.0"
 classifiers=[
```

