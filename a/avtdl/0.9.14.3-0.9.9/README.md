# Comparing `tmp/avtdl-0.9.14.3.tar.gz` & `tmp/avtdl-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "avtdl-0.9.14.3.tar", last modified: Sat Apr 20 20:35:21 2024, max compression
+gzip compressed data, was "avtdl-0.9.9.tar", last modified: Wed Jan 31 21:32:02 2024, max compression
```

## Comparing `avtdl-0.9.14.3.tar` & `avtdl-0.9.9.tar`

### file list

```diff
@@ -1,88 +1,83 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 20:35:21.820501 avtdl-0.9.14.3/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 20:35:21.804500 avtdl-0.9.14.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 20:35:21.808501 avtdl-0.9.14.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1618 2024-04-20 20:35:17.000000 avtdl-0.9.14.3/.github/workflows/publish-exe.yml
--rw-r--r--   0 runner    (1001) docker     (127)      925 2024-04-20 20:35:17.000000 avtdl-0.9.14.3/.github/workflows/publish-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-20 20:35:17.000000 avtdl-0.9.14.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-04-20 20:35:17.000000 avtdl-0.9.14.3/DESCRIPTION.md
--rw-r--r--   0 runner    (1001) docker     (127)    12907 2024-04-20 20:35:17.000000 avtdl-0.9.14.3/EXAMPLES.md
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-20 20:35:17.000000 avtdl-0.9.14.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-04-20 20:35:21.820501 avtdl-0.9.14.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    56745 2024-04-20 20:35:17.000000 avtdl-0.9.14.3/PLUGINS.md
--rw-r--r--   0 runner    (1001) docker     (127)    36076 2024-04-20 20:35:17.000000 avtdl-0.9.14.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 20:35:21.808501 avtdl-0.9.14.3/avtdl/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 20:35:17.000000 avtdl-0.9.14.3/avtdl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-20 20:35:21.000000 avtdl-0.9.14.3/avtdl/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     4038 2024-04-20 20:35:17.000000 avtdl-0.9.14.3/avtdl/avtdl.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 20:35:21.812501 avtdl-0.9.14.3/avtdl/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 20:35:17.000000 avtdl-0.9.14.3/avtdl/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3255 2024-04-20 20:35:17.000000 avtdl-0.9.14.3/avtdl/core/chain.py
--rw-r--r--   0 runner    (1001) docker     (127)     6277 2024-04-20 20:35:17.000000 avtdl-0.9.14.3/avtdl/core/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3429 2024-04-20 20:35:17.000000 avtdl-0.9.14.3/avtdl/core/db.py
--rw-r--r--   0 runner    (1001) docker     (127)     8976 2024-04-20 20:35:17.000000 avtdl-0.9.14.3/avtdl/core/download.py
--rw-r--r--   0 runner    (1001) docker     (127)     9541 2024-04-20 20:35:17.000000 avtdl-0.9.14.3/avtdl/core/info.py
--rw-r--r--   0 runner    (1001) docker     (127)     8839 2024-04-20 20:35:17.000000 avtdl-0.9.14.3/avtdl/core/interfaces.py
--rw-r--r--   0 runner    (1001) docker     (127)     2529 2024-04-20 20:35:17.000000 avtdl-0.9.14.3/avtdl/core/loggers.py
--rw-r--r--   0 runner    (1001) docker     (127)    26196 2024-04-20 20:35:17.000000 avtdl-0.9.14.3/avtdl/core/monitors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2571 2024-04-20 20:35:17.000000 avtdl-0.9.14.3/avtdl/core/plugins.py
--rw-r--r--   0 runner    (1001) docker     (127)    17806 2024-04-20 20:35:17.000000 avtdl-0.9.14.3/avtdl/core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 20:35:21.812501 avtdl-0.9.14.3/avtdl/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 20:35:17.000000 avtdl-0.9.14.3/avtdl/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 20:35:21.812501 avtdl-0.9.14.3/avtdl/plugins/discord/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-20 20:35:17.000000 avtdl-0.9.14.3/avtdl/plugins/discord/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11021 2024-04-20 20:35:17.000000 avtdl-0.9.14.3/avtdl/plugins/discord/webhook.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 20:35:21.812501 avtdl-0.9.14.3/avtdl/plugins/execute/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-20 20:35:17.000000 avtdl-0.9.14.3/avtdl/plugins/execute/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11876 2024-04-20 20:35:17.000000 avtdl-0.9.14.3/avtdl/plugins/execute/run_command.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 20:35:21.816501 avtdl-0.9.14.3/avtdl/plugins/fc2/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-20 20:35:17.000000 avtdl-0.9.14.3/avtdl/plugins/fc2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5546 2024-04-20 20:35:17.000000 avtdl-0.9.14.3/avtdl/plugins/fc2/fc2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 20:35:21.816501 avtdl-0.9.14.3/avtdl/plugins/file/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-20 20:35:17.000000 avtdl-0.9.14.3/avtdl/plugins/file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11393 2024-04-20 20:35:17.000000 avtdl-0.9.14.3/avtdl/plugins/file/download.py
--rw-r--r--   0 runner    (1001) docker     (127)     8362 2024-04-20 20:35:17.000000 avtdl-0.9.14.3/avtdl/plugins/file/text_file.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 20:35:21.816501 avtdl-0.9.14.3/avtdl/plugins/filters/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-20 20:35:17.000000 avtdl-0.9.14.3/avtdl/plugins/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11923 2024-04-20 20:35:17.000000 avtdl-0.9.14.3/avtdl/plugins/filters/filters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 20:35:21.816501 avtdl-0.9.14.3/avtdl/plugins/nitter/
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-20 20:35:17.000000 avtdl-0.9.14.3/avtdl/plugins/nitter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16651 2024-04-20 20:35:17.000000 avtdl-0.9.14.3/avtdl/plugins/nitter/nitter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 20:35:21.816501 avtdl-0.9.14.3/avtdl/plugins/rss/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-20 20:35:17.000000 avtdl-0.9.14.3/avtdl/plugins/rss/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7560 2024-04-20 20:35:17.000000 avtdl-0.9.14.3/avtdl/plugins/rss/generic_rss.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 20:35:21.816501 avtdl-0.9.14.3/avtdl/plugins/twitcast/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-20 20:35:17.000000 avtdl-0.9.14.3/avtdl/plugins/twitcast/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5750 2024-04-20 20:35:17.000000 avtdl-0.9.14.3/avtdl/plugins/twitcast/twitcast_monitor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 20:35:21.816501 avtdl-0.9.14.3/avtdl/plugins/twitch/
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-20 20:35:17.000000 avtdl-0.9.14.3/avtdl/plugins/twitch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5351 2024-04-20 20:35:17.000000 avtdl-0.9.14.3/avtdl/plugins/twitch/twitch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 20:35:21.816501 avtdl-0.9.14.3/avtdl/plugins/url/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-20 20:35:17.000000 avtdl-0.9.14.3/avtdl/plugins/url/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-04-20 20:35:17.000000 avtdl-0.9.14.3/avtdl/plugins/url/url.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 20:35:21.816501 avtdl-0.9.14.3/avtdl/plugins/xmpp/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-20 20:35:17.000000 avtdl-0.9.14.3/avtdl/plugins/xmpp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3518 2024-04-20 20:35:17.000000 avtdl-0.9.14.3/avtdl/plugins/xmpp/msg2jbr_aioxmpp.py
--rw-r--r--   0 runner    (1001) docker     (127)     4888 2024-04-20 20:35:17.000000 avtdl-0.9.14.3/avtdl/plugins/xmpp/msg2jbr_slixmpp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2264 2024-04-20 20:35:17.000000 avtdl-0.9.14.3/avtdl/plugins/xmpp/send_jabber.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 20:35:21.820501 avtdl-0.9.14.3/avtdl/plugins/youtube/
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-20 20:35:17.000000 avtdl-0.9.14.3/avtdl/plugins/youtube/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10140 2024-04-20 20:35:17.000000 avtdl-0.9.14.3/avtdl/plugins/youtube/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     4607 2024-04-20 20:35:17.000000 avtdl-0.9.14.3/avtdl/plugins/youtube/community_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     6536 2024-04-20 20:35:17.000000 avtdl-0.9.14.3/avtdl/plugins/youtube/feed_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     8982 2024-04-20 20:35:17.000000 avtdl-0.9.14.3/avtdl/plugins/youtube/video_info.py
--rw-r--r--   0 runner    (1001) docker     (127)    21806 2024-04-20 20:35:17.000000 avtdl-0.9.14.3/avtdl/plugins/youtube/youtube_chat.py
--rw-r--r--   0 runner    (1001) docker     (127)    10237 2024-04-20 20:35:17.000000 avtdl-0.9.14.3/avtdl/plugins/youtube/youtube_community.py
--rw-r--r--   0 runner    (1001) docker     (127)    12145 2024-04-20 20:35:17.000000 avtdl-0.9.14.3/avtdl/plugins/youtube/youtube_feed.py
--rw-r--r--   0 runner    (1001) docker     (127)    11209 2024-04-20 20:35:17.000000 avtdl-0.9.14.3/avtdl/plugins/youtube/youtube_rss.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 20:35:21.820501 avtdl-0.9.14.3/avtdl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-04-20 20:35:21.000000 avtdl-0.9.14.3/avtdl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-04-20 20:35:21.000000 avtdl-0.9.14.3/avtdl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 20:35:21.000000 avtdl-0.9.14.3/avtdl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-20 20:35:21.000000 avtdl-0.9.14.3/avtdl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-20 20:35:21.000000 avtdl-0.9.14.3/avtdl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-20 20:35:21.000000 avtdl-0.9.14.3/avtdl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-20 20:35:17.000000 avtdl-0.9.14.3/avtdl.py
--rw-r--r--   0 runner    (1001) docker     (127)     3212 2024-04-20 20:35:17.000000 avtdl-0.9.14.3/example.config.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-04-20 20:35:17.000000 avtdl-0.9.14.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-20 20:35:17.000000 avtdl-0.9.14.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 20:35:21.820501 avtdl-0.9.14.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 21:32:02.306739 avtdl-0.9.9/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 21:32:02.294739 avtdl-0.9.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 21:32:02.298739 avtdl-0.9.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      925 2024-01-31 21:31:53.000000 avtdl-0.9.9/.github/workflows/publish-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-01-31 21:31:53.000000 avtdl-0.9.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-01-31 21:31:53.000000 avtdl-0.9.9/DESCRIPTION.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-01-31 21:31:53.000000 avtdl-0.9.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2329 2024-01-31 21:32:02.306739 avtdl-0.9.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    52195 2024-01-31 21:31:53.000000 avtdl-0.9.9/PLUGINS.md
+-rw-r--r--   0 runner    (1001) docker     (127)    26417 2024-01-31 21:31:53.000000 avtdl-0.9.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 21:32:02.298739 avtdl-0.9.9/avtdl/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-31 21:31:53.000000 avtdl-0.9.9/avtdl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-01-31 21:32:02.000000 avtdl-0.9.9/avtdl/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4414 2024-01-31 21:31:53.000000 avtdl-0.9.9/avtdl/avtdl.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 21:32:02.298739 avtdl-0.9.9/avtdl/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-31 21:31:53.000000 avtdl-0.9.9/avtdl/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3255 2024-01-31 21:31:53.000000 avtdl-0.9.9/avtdl/core/chain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5242 2024-01-31 21:31:53.000000 avtdl-0.9.9/avtdl/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3429 2024-01-31 21:31:53.000000 avtdl-0.9.9/avtdl/core/db.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6417 2024-01-31 21:31:53.000000 avtdl-0.9.9/avtdl/core/info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6636 2024-01-31 21:31:53.000000 avtdl-0.9.9/avtdl/core/interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2529 2024-01-31 21:31:53.000000 avtdl-0.9.9/avtdl/core/loggers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24573 2024-01-31 21:31:53.000000 avtdl-0.9.9/avtdl/core/monitors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2463 2024-01-31 21:31:53.000000 avtdl-0.9.9/avtdl/core/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14611 2024-01-31 21:31:53.000000 avtdl-0.9.9/avtdl/core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 21:32:02.298739 avtdl-0.9.9/avtdl/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-31 21:31:53.000000 avtdl-0.9.9/avtdl/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 21:32:02.302739 avtdl-0.9.9/avtdl/plugins/discord/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-01-31 21:31:53.000000 avtdl-0.9.9/avtdl/plugins/discord/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10189 2024-01-31 21:31:53.000000 avtdl-0.9.9/avtdl/plugins/discord/webhook.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 21:32:02.302739 avtdl-0.9.9/avtdl/plugins/execute/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-01-31 21:31:53.000000 avtdl-0.9.9/avtdl/plugins/execute/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11210 2024-01-31 21:31:53.000000 avtdl-0.9.9/avtdl/plugins/execute/run_command.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 21:32:02.302739 avtdl-0.9.9/avtdl/plugins/fc2/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-01-31 21:31:53.000000 avtdl-0.9.9/avtdl/plugins/fc2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4937 2024-01-31 21:31:53.000000 avtdl-0.9.9/avtdl/plugins/fc2/fc2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 21:32:02.302739 avtdl-0.9.9/avtdl/plugins/file/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-01-31 21:31:53.000000 avtdl-0.9.9/avtdl/plugins/file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7828 2024-01-31 21:31:53.000000 avtdl-0.9.9/avtdl/plugins/file/text_file.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 21:32:02.302739 avtdl-0.9.9/avtdl/plugins/filters/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-01-31 21:31:53.000000 avtdl-0.9.9/avtdl/plugins/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11923 2024-01-31 21:31:53.000000 avtdl-0.9.9/avtdl/plugins/filters/filters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 21:32:02.302739 avtdl-0.9.9/avtdl/plugins/nitter/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-01-31 21:31:53.000000 avtdl-0.9.9/avtdl/plugins/nitter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16651 2024-01-31 21:31:53.000000 avtdl-0.9.9/avtdl/plugins/nitter/nitter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 21:32:02.302739 avtdl-0.9.9/avtdl/plugins/rss/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-01-31 21:31:53.000000 avtdl-0.9.9/avtdl/plugins/rss/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7445 2024-01-31 21:31:53.000000 avtdl-0.9.9/avtdl/plugins/rss/generic_rss.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 21:32:02.302739 avtdl-0.9.9/avtdl/plugins/twitcast/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-01-31 21:31:53.000000 avtdl-0.9.9/avtdl/plugins/twitcast/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5186 2024-01-31 21:31:53.000000 avtdl-0.9.9/avtdl/plugins/twitcast/twitcast_monitor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 21:32:02.302739 avtdl-0.9.9/avtdl/plugins/twitch/
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-01-31 21:31:53.000000 avtdl-0.9.9/avtdl/plugins/twitch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4328 2024-01-31 21:31:53.000000 avtdl-0.9.9/avtdl/plugins/twitch/twitch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 21:32:02.302739 avtdl-0.9.9/avtdl/plugins/url/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-01-31 21:31:53.000000 avtdl-0.9.9/avtdl/plugins/url/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-01-31 21:31:53.000000 avtdl-0.9.9/avtdl/plugins/url/url.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 21:32:02.302739 avtdl-0.9.9/avtdl/plugins/xmpp/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-01-31 21:31:53.000000 avtdl-0.9.9/avtdl/plugins/xmpp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3518 2024-01-31 21:31:53.000000 avtdl-0.9.9/avtdl/plugins/xmpp/msg2jbr_aioxmpp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4451 2024-01-31 21:31:53.000000 avtdl-0.9.9/avtdl/plugins/xmpp/msg2jbr_slixmpp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2259 2024-01-31 21:31:53.000000 avtdl-0.9.9/avtdl/plugins/xmpp/send_jabber.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 21:32:02.306739 avtdl-0.9.9/avtdl/plugins/youtube/
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-01-31 21:31:53.000000 avtdl-0.9.9/avtdl/plugins/youtube/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9624 2024-01-31 21:31:53.000000 avtdl-0.9.9/avtdl/plugins/youtube/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4242 2024-01-31 21:31:53.000000 avtdl-0.9.9/avtdl/plugins/youtube/community_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6300 2024-01-31 21:31:53.000000 avtdl-0.9.9/avtdl/plugins/youtube/feed_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10065 2024-01-31 21:31:53.000000 avtdl-0.9.9/avtdl/plugins/youtube/video_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19982 2024-01-31 21:31:53.000000 avtdl-0.9.9/avtdl/plugins/youtube/youtube_chat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10036 2024-01-31 21:31:53.000000 avtdl-0.9.9/avtdl/plugins/youtube/youtube_community.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10410 2024-01-31 21:31:53.000000 avtdl-0.9.9/avtdl/plugins/youtube/youtube_feed.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10815 2024-01-31 21:31:53.000000 avtdl-0.9.9/avtdl/plugins/youtube/youtube_rss.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 21:32:02.306739 avtdl-0.9.9/avtdl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2329 2024-01-31 21:32:02.000000 avtdl-0.9.9/avtdl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1716 2024-01-31 21:32:02.000000 avtdl-0.9.9/avtdl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-31 21:32:02.000000 avtdl-0.9.9/avtdl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-01-31 21:32:02.000000 avtdl-0.9.9/avtdl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-01-31 21:32:02.000000 avtdl-0.9.9/avtdl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-01-31 21:32:02.000000 avtdl-0.9.9/avtdl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-01-31 21:31:53.000000 avtdl-0.9.9/avtdl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-01-31 21:31:53.000000 avtdl-0.9.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-01-31 21:31:53.000000 avtdl-0.9.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-31 21:32:02.306739 avtdl-0.9.9/setup.cfg
```

### Comparing `avtdl-0.9.14.3/.github/workflows/publish-pypi.yml` & `avtdl-0.9.9/.github/workflows/publish-pypi.yml`

 * *Files identical despite different names*

### Comparing `avtdl-0.9.14.3/DESCRIPTION.md` & `avtdl-0.9.9/DESCRIPTION.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 ## avtdl
 
 Tool to monitor Youtube and some other streaming platforms for new streams and uploads and execute user-defined commands when it happens. It aims to provide a highly configurable environment for setting up automated archiving of new content with filtering and notification support. It does not try to provide downloading streams itself and instead relies on executing commonly used well-known solutions for the task, such as `yt-dlp`.
 
-Refer to [documentation](https://github.com/15532th/avtdl?tab=readme-ov-file#avtdl) for full list of available features and description of configuration process.
+Refer to documentation for full list of available features and description of configuration process.
 
 ### Features overview
 
 Some of the supported features include:
 
 - monitoring Youtube channels using RSS feed
 - monitoring Youtube channels, individual tabs of a channel or playlists by parsing html. With authorization cookies from Youtube account it's possible to get notifications for member-only and in any other way restricted streams and uploads, as well as to monitor the entire subscriptions feed
```

### Comparing `avtdl-0.9.14.3/LICENSE` & `avtdl-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `avtdl-0.9.14.3/PKG-INFO` & `avtdl-0.9.9/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: avtdl
-Version: 0.9.14.3
+Version: 0.9.9
 Summary: Monitoring and automation tool for Youtube and other streaming platforms
 Author: 15532th
 Project-URL: Homepage, https://github.com/15532th/avtdl
 Project-URL: Documentation, https://github.com/15532th/avtdl
 Project-URL: Repository, https://github.com/15532th/avtdl.git
 Project-URL: Issues, https://github.com/15532th/avtdl/issues
 Classifier: Environment :: Console
@@ -23,15 +23,15 @@
 Requires-Dist: Markdown
 Requires-Dist: jsonpath-python==1.0.6
 
 ## avtdl
 
 Tool to monitor Youtube and some other streaming platforms for new streams and uploads and execute user-defined commands when it happens. It aims to provide a highly configurable environment for setting up automated archiving of new content with filtering and notification support. It does not try to provide downloading streams itself and instead relies on executing commonly used well-known solutions for the task, such as `yt-dlp`.
 
-Refer to [documentation](https://github.com/15532th/avtdl?tab=readme-ov-file#avtdl) for full list of available features and description of configuration process.
+Refer to documentation for full list of available features and description of configuration process.
 
 ### Features overview
 
 Some of the supported features include:
 
 - monitoring Youtube channels using RSS feed
 - monitoring Youtube channels, individual tabs of a channel or playlists by parsing html. With authorization cookies from Youtube account it's possible to get notifications for member-only and in any other way restricted streams and uploads, as well as to monitor the entire subscriptions feed
```

### Comparing `avtdl-0.9.14.3/PLUGINS.md` & `avtdl-0.9.9/PLUGINS.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,110 +1,195 @@
 
-<!-- This file is autogenerated as part of avtdl 0.9.dev0+ga5c0e58.d20240216 at 2024-03-11 00:42:28.976228 -->
+<!-- This file is manually crafted as part of avtdl -->
 
 ## Description and configuration of available plugins
+
+---
 ### Table of content:
+
 <!-- [TOC] -->
 
-* [Monitors:](#monitors)
-  * [fc2 - Monitor for live.fc2.com](#fc2---monitor-for-livefc2com)
-  * [from_file - Monitor content of a text file](#from_file---monitor-content-of-a-text-file)
-  * [nitter - Monitor for Nitter instances](#nitter---monitor-for-nitter-instances)
-  * [generic_rss - RSS feed monitor](#generic_rss---rss-feed-monitor)
-  * [twitcast - Monitor for twitcasting.tv](#twitcast---monitor-for-twitcastingtv)
-  * [twitch - Monitor for twitch.tv](#twitch---monitor-for-twitchtv)
-  * [get_url - Monitor web page text](#get_url---monitor-web-page-text)
-  * [rss - Youtube channel RSS feed monitor](#rss---youtube-channel-rss-feed-monitor)
-  * [community - Youtube community page monitor](#community---youtube-community-page-monitor)
-  * [channel - Youtube channel monitor](#channel---youtube-channel-monitor)
-  * [prechat - Youtube livechat monitor](#prechat---youtube-livechat-monitor)
-* [Filters:](#filters)
-  * [filter.noop - Pass everything through](#filternoop---pass-everything-through)
-  * [filter.void - Drop everything](#filtervoid---drop-everything)
-  * [filter.match - Keep records with specific words](#filtermatch---keep-records-with-specific-words)
-  * [filter.exclude - Drop records with specific words](#filterexclude---drop-records-with-specific-words)
-  * [filter.event - Filter for records with "Event" type](#filterevent---filter-for-records-with-event-type)
-  * [filter.type - Filter for records of specific type](#filtertype---filter-for-records-of-specific-type)
-  * [filter.json - Format record as JSON](#filterjson---format-record-as-json)
-  * [filter.format - Format record as text](#filterformat---format-record-as-text)
-  * [filter.deduplicate - Drop already seen records](#filterdeduplicate---drop-already-seen-records)
-  * [filter.nitter.pick - Pick NitterRecord with specified properties](#filternitterpick---pick-nitterrecord-with-specified-properties)
-  * [filter.nitter.drop - Drop NitterRecord without specified properties.](#filternitterdrop---drop-nitterrecord-without-specified-properties)
-  * [filter.channel - Pick YoutubeVideoRecord with specified properties](#filterchannel---pick-youtubevideorecord-with-specified-properties)
-* [Actions:](#actions)
-  * [discord.hook - Send record to Discord using webhook](#discordhook---send-record-to-discord-using-webhook)
-  * [execute - Run pre-defined shell command](#execute---run-pre-defined-shell-command)
-  * [to_file - Write record to a text file](#to_file---write-record-to-a-text-file)
-  * [download - Download a file](#download---download-a-file)
-  * [xmpp - Send records as Jabber messages](#xmpp---send-records-as-jabber-messages)
+* [`discord.hook` - Send record to Discord using webhook](#discordhook---send-record-to-discord-using-webhook)
+* [`execute` - Run pre-defined shell command](#execute---run-pre-defined-shell-command)
+* [`fc2` - Monitor for live.fc2.com](#fc2---monitor-for-livefc2com)
+* [`from_file` - Monitor content of a text file](#fromfile---monitor-content-of-a-text-file)
+* [`to_file` - Write record to a text file](#tofile---write-record-to-a-text-file)
+* [`filter.noop` - Pass everything through](#filternoop---pass-everything-through)
+* [`filter.void` - Drop everything](#filtervoid---drop-everything)
+* [`filter.match` - Keep records with specific words](#filtermatch---keep-records-with-specific-words)
+* [`filter.exclude` - Drop records with specific words](#filterexclude---drop-records-with-specific-words)
+* [`filter.event` - Filter for records with "Event" type](#filterevent---filter-for-records-with-event-type)
+* [`filter.type` - Filter for records of specific type](#filtertype---filter-for-records-of-specific-type)
+* [`filter.json` - Format record as JSON](#filterjson---format-record-as-json)
+* [`filter.format` - Format record as text](#filterformat---format-record-as-text)
+* [`filter.deduplicate` - Drop already seen records](#filterdeduplicate---drop-already-seen-records)
+* [`nitter` - Monitor for Nitter instances](#nitter---monitor-for-nitter-instances)
+* [`filter.nitter.pick` - Pick `NitterRecord` with specified properties](#filternitterpick---pick-nitterrecord-with-specified-properties)
+* [`filter.nitter.drop` - Drop `NitterRecord` without specified properties.](#filternitterdrop---drop-nitterrecord-without-specified-properties)
+* [`generic_rss` - RSS feed monitor](#genericrss---rss-feed-monitor)
+* [`twitcast` - Monitor for twitcasting.tv](#twitcast---monitor-for-twitcastingtv)
+* [`twitch` - Monitor for twitch.tv](#twitch---monitor-for-twitchtv)
+* [`get_url` - Monitor web page text](#geturl---monitor-web-page-text)
+* [`xmpp` - Send record as a Jabber message](#xmpp---send-record-as-a-jabber-message)
+* [`rss` - Youtube channel RSS feed monitor](#rss---youtube-channel-rss-feed-monitor)
+* [`community` - Youtube community page monitor](#community---youtube-community-page-monitor)
+* [`channel` - Youtube channel monitor](#channel---youtube-channel-monitor)
+* [`filter.channel` - Pick `YoutubeVideoRecord` with specified properties](#filterchannel---pick-youtubevideorecord-with-specified-properties)
+* [`prechat` - Youtube livechat monitor](#prechat---youtube-livechat-monitor)
+
+---
+
+### `discord.hook` - Send record to Discord using webhook
+
+To generate webhook url follow instructions in "Making a Webhook" section of
+<https://support.discord.com/hc/en-us/articles/228383668-Intro-to-Webhooks>
+
+Some record types support rich formatting when sent to Discord, such as
+showing author's avatar and links to attached images. Youtube videos will
+show thumbnail, however embedding video itself is not supported.
+
+Records coming within six seconds one after another will be batched together into a single message.
+When too many records are received at once, they will be sent with delays to conform Discord
+rate limits. Records deemed to be too long to fit in Discord message
+[length limits](https://discord.com/developers/docs/resources/channel#create-message-jsonform-params)
+will be dropped with a warning.
+
+
+#### Entity configuration options:
+* `name`: name of specific entity. Used to reference it in `Chains` section. Must be unique within a plugin. Required.
+* `url`: webhook url. Required.
+##### 
+* `timezone`: takes timezone name from <https://en.wikipedia.org/wiki/List_of_tz_database_time_zones> (or OS settings if omitted), converts record fields containing date and time to this timezone. Not required.
 
-<!-- [TOC] -->
 ---
 
-## Monitors:
+### `execute` - Run pre-defined shell command
 
+Take `command` string, replace keywords provided in `placeholders` with corresponding fields
+of currently processed record. For example, if `command` is set to
+
+    "yt-dlp {url}"`
+
+and currently processed record comes from Youtube RSS feed and has `url` field value
+`https://www.youtube.com/watch?v=L692Sxz3thw`, then with default `placeholders`
+resulting command will be
+
+    yt-dlp https://www.youtube.com/watch?v=L692Sxz3thw
+
+Note that placeholders do not have to be wrapped in `{}` and can, in fact, be any
+arbitrary text strings. However, placeholders are replaced by corresponding values
+one after another, so using piece of text that might come up in record field might
+produce unexpected results.
+
+Make sure the executable the command uses (`yt-dlp` in this case) is installed and
+can be run from working directory by current user. It is advised to confirm command
+can be executed manually and finishes without errors before automating it.
+
+For each entity separate working directory can be configured. Output is shown
+in the same window by default, but can be redirected in file, with either static
+or autogenerated name.
+
+Produces Events on beginning, successful end and failure of executed command
+if corresponding entity settings are enabled. They can be used to send Discord
+or Jabber notifications or execute another command when it happens.
+
+Processed record itself can also be passed down the chain if command failed,
+providing a way to try a different one as a fallback. For example, record with
+Youtube url could be first handled by `ytarchive` and passed to `yt-dlp` if
+it happens to fail due to video link not being a livestream.
+
+
+#### Entity configuration options:
+* `name`: name of specific entity. Used to reference it in `Chains` section. Must be unique within a plugin. Required.
+* `command`: shell command to be executed on every received record. Supports placeholders that will be replaced with currently processed record fields values. Required.
+##### 
+* `working_dir`: path to directory where command will be executed. If not set current working directory is used. Not required.
+* `log_dir`: write executed process output to a file in this directory if set. If it is not set, output will not be redirected to file. Not required.
+* `log_filename`: filename to write executed process output to. If not defined is generated automatically based on command and entity name. Not required.
+* `placeholders`: parts of `command` string that should be replaced with processed record fields, defined  as mapping `'placeholder': 'record field name'`. Default value is `"{url}": "url", "{title}": "title", "{text}": "text"`.
+* `static_placeholders`: parts of `command` string that will be replaced with provided values, defined as mapping `'placeholder': 'replacement string'`. Intended to allow reusing same `command` template for multiple entities. Not required.
+* `forward_failed`: emit currently processed record down the chain if subprocess returned non-zero exit code. Can be used to define fallback command in case this one fails. Default value is `false`.
+* `report_failed`: emit Event with type "error" if subprocess returned non-zero exit code or raised exception. Default value is `true`.
+* `report_finished`: emit Event with type "finished" if subprocess returned zero as exit code. Default value is `false`.
+* `report_started`: emit Event with type "started" before starting subprocess. Default value is `false`.
+
+
+#### Produced records types:
+
+
+<details markdown="block">
+  <summary>Event</summary>
+
+Record produced by internal event (usually error) inside the plugin
+
+
+* `event_type`: text describing the nature of event, can be used to filter classes of events, such as errors. 
+* `text`: text describing specific even details. 
+
+</details>
+
+---
 
 ### `fc2` - Monitor for live.fc2.com
 
-Monitors fc2.com user with given id, produces a record when it goes live.
-For user `https://live.fc2.com/24374512/`, user id would be `24374512`.
+Monitors fc2.com user with given id, produces record when it goes live.
+For user `https://live.fc2.com/24374512/` user id would be `24374512`.
 
-Since the endpoint used for monitoring does not provide the user's nickname,
-the name of the configuration entity is used instead.
+Since endpoint used for monitoring does not provide user nickname,
+the name of configuration entity is used instead.
 
 
 #### Entity configuration options:
-* `name`: name of a specific entity. Used to reference it in `chains` section. Must be unique within a plugin. Required.
+* `name`: name of specific entity. Used to reference it in `Chains` section. Must be unique within a plugin. Required.
 * `user_id`: user id, numeric part at the end of livestream url. Required.
 ##### 
-* `update_interval`: how often the monitored channel will be checked, in seconds. Default value is `120`.
-* `cookies_file`: path to a text file containing cookies in Netscape format. Not required.
+* `update_interval`: how often monitored channel will be checked, in seconds. Default value is `120`.
+* `cookies_file`: path to text file containing cookies in Netscape format. Not required.
 * `headers`: custom HTTP headers as pairs "key": value". "Set-Cookie" header will be ignored, use `cookies_file` option instead. Default value is `"Accept-Language": "en-US,en;q=0.9"`.
 
 
 #### Produced records types:
 
 
 <details markdown="block">
   <summary>FC2Record</summary>
 
 Represents event of a stream going live on FC2
 
 
 * `name`: name of the config entity for this user. 
 * `url`: url of the user stream. 
-* `user_id`: unique for the given user/channel part of the stream url. 
+* `user_id`: unique for given user/channel part of the stream url. 
 * `title`: stream title. 
 * `info`: stream description. 
-* `start`: time of the stream start. 
-* `start_timestamp`: UNIX timestamp of the stream start. 
-* `avatar_url`: link to the user's avatar. 
-* `login_only`: whether logging in is required to view current livestream. 
+* `start`: timestamp of the stream start. 
+* `avatar_url`: link to user's avatar. 
+* `login_only`: Whether logging in is required to view current livestream. 
 
 </details>
 
 ---
 
 ### `from_file` - Monitor content of a text file
 
-On specified intervals, check existence and last modification time
-of target file, and if it has changed, read file contents
+On specified intervals check existence and last modification time
+of target file, and if it changed read file content
 either line by line or as a whole and emit it as a text record(s).
 
 Records are not checked for uniqueness, so appending content to the end
 of the existing file will produce duplicates of already sent records.
 
 
 #### Entity configuration options:
-* `name`: name of a specific entity. Used to reference it in `chains` section. Must be unique within a plugin. Required.
-* `path`: path to the monitored file. Required.
+* `name`: name of specific entity. Used to reference it in `Chains` section. Must be unique within a plugin. Required.
+* `path`: path to monitored file. Required.
 ##### 
-* `update_interval`: how often the monitored file should be checked, in seconds. Default value is `60`.
-* `encoding`: encoding used to open the monitored file. If not specified, default system-wide encoding is used. Not required.
-* `split_lines`: if true, each line of the file will create a separate record. Otherwise, a single record will be generated with the entire file content. Default value is `false`.
+* `update_interval`: how often monitored file should be checked, in seconds. Default value is `60`.
+* `encoding`: encoding used to open monitored file. If not specified default system-wide encoding is used. Not required.
+* `split_lines`: if true, each line of the file will create a separate record. Otherwise, a single record will be generated with entire file content. Default value is `false`.
 
 
 #### Produced records types:
 
 
 <details markdown="block">
   <summary>TextRecord</summary>
@@ -114,59 +199,320 @@
 
 * `text`: content of the record. 
 
 </details>
 
 ---
 
+### `to_file` - Write record to a text file
+
+Takes record coming from a Chain, converts it to text representation,
+and write to a file in given directory. When file already exists,
+new records can be appended to the end of the file or overwrite it.
+
+Output file name can be static or generated dynamically based on template
+filled with values from the record fields: every occurrence of `{text}`
+in filename will be replaced with value of the `text` field of processed
+record, if the record has one.
+
+Allows writing record as human-readable text representation or as names and
+values of the record fields in json format. For custom format template pass record
+through `filter.format` plugin prior to this one.
+
+Produces `Event` with `error` type if writing to target file fails.
+
+Note discrepancy between default value of `encoding` setting between `from_file`
+and `to_file` plugins. Former is expected to be able to read files produced by
+different software and therefore relies on system-wide settings. It would make
+sense to do the same in latter, but it would introduce possibility of failing
+to write records containing text with Unicode codepoints that cannot be represented
+using system-wide encoding.
+
+
+#### Entity configuration options:
+* `name`: name of specific entity. Used to reference it in `Chains` section. Must be unique within a plugin. Required.
+* `filename`: name of the output file. Supports templating with `{...}`. Required.
+##### 
+* `path`: directory where output file should be created. Default is current directory. Not required.
+* `encoding`: output file encoding. Default value is `utf8`.
+* `output_format`: one of `str`, `repr`, `json`, `pretty_json`, `hash`. Default value is `text`.
+* `overwrite`: whether file should be overwritten in if it already exists. Default value is `true`.
+* `append`: if true, new record will be written in the end of the file without overwriting already present lines. Default value is `true`.
+* `prefix`: string that will be appended before record text. Can be used to separate records from each other or for simple templating. Not required.
+* `postfix`: string that will be appended after record text. Not required.
+
+
+#### Produced records types:
+
+
+<details markdown="block">
+  <summary>Event</summary>
+
+Record produced by internal event (usually error) inside the plugin
+
+
+* `event_type`: text describing the nature of event, can be used to filter classes of events, such as errors. 
+* `text`: text describing specific even details. 
+
+</details>
+
+---
+
+### `filter.noop` - Pass everything through
+
+Lets all coming records pass through unchanged, effectively
+doing nothing with them. As any other filter it has entities,
+so it can be used as a merging point to gather records from
+multiple chains and process then in a single place.
+
+
+#### Entity configuration options:
+* `name`: name of specific entity. Used to reference it in `Chains` section. Must be unique within a plugin. Required.
+
+---
+
+### `filter.void` - Drop everything
+
+Does not produce anything, dropping any incoming records.
+Can be used to stuff multiple chains in one if the need ever arise.
+
+
+#### Entity configuration options:
+* `name`: name of specific entity. Used to reference it in `Chains` section. Must be unique within a plugin. Required.
+
+---
+
+### `filter.match` - Keep records with specific words
+
+This filter lets through records, that has one of values
+defined by `patterns` list found in any (or specified) field of the record.
+
+
+#### Entity configuration options:
+* `name`: name of specific entity. Used to reference it in `Chains` section. Must be unique within a plugin. Required.
+* `patterns`: list of strings to search in the record. Required.
+##### 
+* `fields`: field names to search patterns in. If not specified all fields are checked. Not required.
+
+---
+
+### `filter.exclude` - Drop records with specific words
+
+This filter lets through records, that has none of values
+defined by `patterns` list found in any (or specified) field of the record.
+
+
+#### Entity configuration options:
+* `name`: name of specific entity. Used to reference it in `Chains` section. Must be unique within a plugin. Required.
+* `patterns`: list of strings to search in the record. Required.
+##### 
+* `fields`: field names to search patterns in. If not specified all fields are checked. Not required.
+
+---
+
+### `filter.event` - Filter for records with "Event" type
+
+Only lets through Events and not normal Records. Can be used to
+set up notifications on events (such as errors) from, for example,
+`execute` plugin within the same chain that uses it, by separating
+them from regular records.
+
+
+#### Entity configuration options:
+* `name`: name of specific entity. Used to reference it in `Chains` section. Must be unique within a plugin. Required.
+##### 
+* `event_types`: list of event types. See descriptions of plugins producing events for possible values. Not required.
+
+
+#### Produced records types:
+
+
+<details markdown="block">
+  <summary>Event</summary>
+
+Record produced by internal event (usually error) inside the plugin
+
+
+* `event_type`: text describing the nature of event, can be used to filter classes of events, such as errors. 
+* `text`: text describing specific even details. 
+
+</details>
+
+---
+
+### `filter.type` - Filter for records of specific type
+
+Only lets through records of specified types, such as `Event` or `YoutubeVideoRecord`.
+
+
+#### Entity configuration options:
+* `name`: name of specific entity. Used to reference it in `Chains` section. Must be unique within a plugin. Required.
+* `types`: list of records class names, such as "Record" and "Event" . Required.
+##### 
+* `exact_match`: whether match should check for exact record type or look in entire records hierarchy up to Record. Default value is `false`.
+
+---
+
+### `filter.json` - Format record as JSON
+
+Takes record and produces a new `TextRecord` rendering fields of the
+original record in JSON format, with option for pretty-print.
+
+
+#### Entity configuration options:
+* `name`: name of specific entity. Used to reference it in `Chains` section. Must be unique within a plugin. Required.
+##### 
+* `prettify`: whether output should be multiline and indented or a single line. Default value is `false`.
+
+
+#### Produced records types:
+
+
+<details markdown="block">
+  <summary>TextRecord</summary>
+
+Simplest record, containing only a single text field
+
+
+* `text`: content of the record. 
+
+</details>
+
+---
+
+### `filter.format` - Format record as text
+
+Takes record and produces a new `TextRecord` by taking `template` string
+and replacing "{placeholder}" with value of `placeholder` field of the
+current record, where `placeholder` is any field the record might have.
+If one of placeholders is not a field of specific record, it will be
+replaced with value defined in `missing` parameter if it is specified,
+otherwise it will be left intact.
+
+
+#### Entity configuration options:
+* `name`: name of specific entity. Used to reference it in `Chains` section. Must be unique within a plugin. Required.
+* `template`: template string with placeholders that will be filled with corresponding values from current record. Required.
+##### 
+* `missing`: if specified, will be used to fill template placeholders that do not have corresponding fields in current record. Not required.
+
+
+#### Produced records types:
+
+
+<details markdown="block">
+  <summary>TextRecord</summary>
+
+Simplest record, containing only a single text field
+
+
+* `text`: content of the record. 
+
+</details>
+
+---
+
+### `filter.deduplicate` - Drop already seen records
+
+Checks if the `field` field value of the current record has already been
+present in one of the previous records and only let it through otherwise.
+
+`field` might be either a record field name or one of `hash` or `as_json`
+for sha1 and fulltext comparison. If `field` is not present in the current
+record, it will be passed through as if it's new.
+
+This filter will work with records of any type, as long as they have defined
+field (all records have `hash` and `as_json`). For example, it is possible
+to ensure no multiple records for a single video will be produced
+in a chain, that gather records from Youtube channel and Youtube RSS monitors,
+by passing them to an entity of this filter with `field` set to `video_id`.
+
+Note, that history is kept in memory, so it will not be persisted between
+restarts.
+
+
+#### Entity configuration options:
+* `name`: name of specific entity. Used to reference it in `Chains` section. Must be unique within a plugin. Required.
+##### 
+* `field`: field name to use for comparison. Default value is `hash`.
+* `history_size`: how many old records should be kept in memory. Default value is `10000`.
+
+---
+
+### `gmail` - Check for new mails using Gmail simple interface [deprecated]
+
+Simple html interface was removed from Gmail since January 2024.
+R.I.P.
+
+
+#### Plugin configuration options:
+* `db_path`: path to sqlite database file keeping history of old records of this monitor.
+Might specify a path to a directory containing the file (with trailing slash)
+or direct path to the file itself (without a slash). If special value `:memory:` is used,
+database is kept in memory and not stored on disk at all, providing a clean database on every startup. Default value is `:memory:`.
+
+
+
+#### Entity configuration options:
+* `name`: name of specific entity. Used to reference it in `Chains` section. Must be unique within a plugin. Required.
+* `cookies_file`: . Required.
+##### 
+* `update_interval`: . Default value is `900`.
+* `headers`: custom HTTP headers as pairs "key": value". "Set-Cookie" header will be ignored, use `cookies_file` option instead. Default value is `"Accept-Language": "en-US,en;q=0.9"`.
+* `adjust_update_interval`: change delay before next update based on response headers. This setting doesn't affect timeouts after failed requests. Default value is `true`.
+* `quiet_start`: throw away new records on the first update after application startup. Default value is `false`.
+* `quiet_first_time`: throw away new records produced on first update of given url. Default value is `true`.
+
+---
+
 ### `nitter` - Monitor for Nitter instances
 
 Monitors recent tweets, retweets and replies of Twitter user
 by scraping and parsing data from a Nitter instance.
 
-Examples of supported urls:
+Examples of supported url:
 
 - `https://nitter.net/username`
 - `https://nitter.net/username/with_replies`
 
-Some instances might not be happy about getting automated scraping. Make sure
-to use a reasonable `update_interval` and keep an eye out for 4XX and 5XX responses
+Some instances might not be happy getting automated scraping. Make sure
+to use reasonable `update_interval` and keep eyes on 4XX and 5XX responses
 in log, as they might indicate server is under high load or refuses to
 communicate.
 
-Nitter has a built-in RSS feed, though not all instances enable it, so it
+Nitter has built in RSS feed, though not all instances enable it, so it
 can also be monitored with `generic_rss` plugin instead of this one.
 
 Twitter Spaces appears on user feed as normal tweets with text only
 containing a single link similar to `https://x.com/i/spaces/2FsjOybqEbnzR`.
 It therefore can be picked up by using a regular full-text `match` filter.
 
 
 #### Plugin configuration options:
-* `db_path`: path to the sqlite database file keeping history of old records of this monitor.
+* `db_path`: path to sqlite database file keeping history of old records of this monitor.
 Might specify a path to a directory containing the file (with trailing slash)
-or a direct path to the file itself (without a slash). If special value `:memory:` is used,
-database is kept in memory and not stored on disk at all, providing a clean database on every startup. Default value is `db/`.
+or direct path to the file itself (without a slash). If special value `:memory:` is used,
+database is kept in memory and not stored on disk at all, providing a clean database on every startup. Default value is `:memory:`.
 
 
 
 #### Entity configuration options:
-* `name`: name of a specific entity. Used to reference it in `chains` section. Must be unique within a plugin. Required.
+* `name`: name of specific entity. Used to reference it in `Chains` section. Must be unique within a plugin. Required.
 * `url`: url that should be monitored. Required.
 ##### 
 * `update_interval`: How often the monitored url will be checked, in seconds. Default value is `1800`.
-* `cookies_file`: path to a text file containing cookies in Netscape format. Not required.
+* `cookies_file`: path to text file containing cookies in Netscape format. Not required.
 * `headers`: custom HTTP headers as pairs "key": value". "Set-Cookie" header will be ignored, use `cookies_file` option instead. Default value is `"Accept-Language": "en-US,en;q=0.9"`.
 * `adjust_update_interval`: change delay before next update based on response headers. This setting doesn't affect timeouts after failed requests. Default value is `true`.
 * `quiet_start`: throw away new records on the first update after application startup. Default value is `false`.
 * `quiet_first_time`: throw away new records produced on first update of given url. Default value is `true`.
 * `max_continuation_depth`: when updating feed with pagination support, only continue for this many pages. Default value is `10`.
 * `next_page_delay`: when updating feed with pagination support, wait this much before loading next page. Default value is `1`.
 * `allow_discontinuity`: when updating feed with pagination support, if this setting is enabled and error happens when loading a page, records from already parsed pages will not be dropped. It will allow update of the feed to finish, but older records from deeper pages will then never be parsed on consecutive updates. Default value is `false`.
-* `fetch_until_the_end_of_feed_mode`: when updating feed with pagination support, enables special mode, which makes a monitor try loading and parsing all pages until the end, even if they have been already parsed. Designed for purpose of archiving entire feed content. Default value is `false`.
+* `fetch_until_the_end_of_feed_mode`: when updating feed with pagination support, enables special mode, which makes monitor try loading and parsing all pages until the end, even if they have been already parsed. Designed for purpose of archiving entire feed content. Default value is `false`.
 
 
 #### Produced records types:
 
 
 <details markdown="block">
   <summary>NitterRecord</summary>
@@ -177,15 +523,103 @@
 
 
 * `retweet_header`: text line saying this is a retweet. 
 * `reply_header`: text line saying this tweet is a reply. 
 * `url`: tweet url. 
 * `author`: user's visible name. 
 * `username`: user's handle. 
-* `avatar_url`: link to the picture used as the user's avatar. 
+* `avatar_url`: link to the picture used as user's avatar. 
+* `published`: tweet timestamp. 
+* `text`: tweet text with stripped formatting. 
+* `html`: tweet text as raw html. 
+* `attachments`: list of links to attached images or video thumbnails. 
+* `quote`: Nested NitterRecord containing tweet being quited. 
+
+</details>
+
+---
+
+### `filter.nitter.pick` - Pick `NitterRecord` with specified properties
+
+Lets through `NitterRecord` if it matches any of specified criteria.
+All records from other sources pass through without filtering.
+
+
+#### Entity configuration options:
+* `name`: name of specific entity. Used to reference it in `Chains` section. Must be unique within a plugin. Required.
+##### 
+* `retweet`: match retweets. Default value is `false`.
+* `reply`: match replies. Default value is `false`.
+* `quote`: match quotes. Default value is `false`.
+* `regular_tweet`: match regular tweets, that are not a retweet, reply or quote. Default value is `false`.
+* `author`: match if given string is a part of the name of the author of the tweet. Not required.
+* `username`: match if given string is a part of tweet author's username (without the "@" symbol). Not required.
+
+
+#### Produced records types:
+
+
+<details markdown="block">
+  <summary>NitterRecord</summary>
+
+Single post as parsed from Nitter instance
+
+Depending on the tweet type (regular, retweet, reply, quote) some fields might be empty
+
+
+* `retweet_header`: text line saying this is a retweet. 
+* `reply_header`: text line saying this tweet is a reply. 
+* `url`: tweet url. 
+* `author`: user's visible name. 
+* `username`: user's handle. 
+* `avatar_url`: link to the picture used as user's avatar. 
+* `published`: tweet timestamp. 
+* `text`: tweet text with stripped formatting. 
+* `html`: tweet text as raw html. 
+* `attachments`: list of links to attached images or video thumbnails. 
+* `quote`: Nested NitterRecord containing tweet being quited. 
+
+</details>
+
+---
+
+### `filter.nitter.drop` - Drop `NitterRecord` without specified properties.
+
+Lets through `NitterRecord` if it doesn't match all of the specified criteria.
+All records from other sources pass through without filtering.
+
+
+#### Entity configuration options:
+* `name`: name of specific entity. Used to reference it in `Chains` section. Must be unique within a plugin. Required.
+##### 
+* `retweet`: match retweets. Default value is `false`.
+* `reply`: match replies. Default value is `false`.
+* `quote`: match quotes. Default value is `false`.
+* `regular_tweet`: match regular tweets, that are not a retweet, reply or quote. Default value is `false`.
+* `author`: match if given string is a part of the name of the author of the tweet. Not required.
+* `username`: match if given string is a part of tweet author's username (without the "@" symbol). Not required.
+
+
+#### Produced records types:
+
+
+<details markdown="block">
+  <summary>NitterRecord</summary>
+
+Single post as parsed from Nitter instance
+
+Depending on the tweet type (regular, retweet, reply, quote) some fields might be empty
+
+
+* `retweet_header`: text line saying this is a retweet. 
+* `reply_header`: text line saying this tweet is a reply. 
+* `url`: tweet url. 
+* `author`: user's visible name. 
+* `username`: user's handle. 
+* `avatar_url`: link to the picture used as user's avatar. 
 * `published`: tweet timestamp. 
 * `text`: tweet text with stripped formatting. 
 * `html`: tweet text as raw html. 
 * `attachments`: list of links to attached images or video thumbnails. 
 * `quote`: Nested NitterRecord containing tweet being quited. 
 
 </details>
@@ -193,42 +627,42 @@
 ---
 
 ### `generic_rss` - RSS feed monitor
 
 Monitors RSS feed for new entries. Will attempt to adjust
 update interval based on HTTP response headers.
 
-Depending on a specific feed format, fields names and content
+Depending on specific feed format, fields names and content
 might vary greatly. Commonly present standardized fields are
 `url`, `title` and `author`, though they might be empty
 in some feeds.
 
-Before defining a command to be executed for records of a newly
-added feed it is recommended to inspect the feed entity content by
+Before defining a command to be executed for records of newly
+set feed it is recommended to inspect feed entity content by
 forwarding records in a file in JSON format using `to_file` plugin.
 
-Normally feeds have some kind of value to uniquely identify
-feed entries, but in case there is none, parser will attempt
+Normally feeds have some kind of value to unique identify
+feed entries, but in case there is none parser will attempt
 to create one by combining `link` and `title` or `summary` fields.
 
 
 #### Plugin configuration options:
-* `db_path`: path to the sqlite database file keeping history of old records of this monitor.
+* `db_path`: path to sqlite database file keeping history of old records of this monitor.
 Might specify a path to a directory containing the file (with trailing slash)
-or a direct path to the file itself (without a slash). If special value `:memory:` is used,
-database is kept in memory and not stored on disk at all, providing a clean database on every startup. Default value is `db/`.
+or direct path to the file itself (without a slash). If special value `:memory:` is used,
+database is kept in memory and not stored on disk at all, providing a clean database on every startup. Default value is `:memory:`.
 
 
 
 #### Entity configuration options:
-* `name`: name of a specific entity. Used to reference it in `chains` section. Must be unique within a plugin. Required.
+* `name`: name of specific entity. Used to reference it in `Chains` section. Must be unique within a plugin. Required.
 * `update_interval`: how often the monitored source should be checked for new content, in seconds. Required.
 * `url`: url that should be monitored. Required.
 ##### 
-* `cookies_file`: path to a text file containing cookies in Netscape format. Not required.
+* `cookies_file`: path to text file containing cookies in Netscape format. Not required.
 * `headers`: custom HTTP headers as pairs "key": value". "Set-Cookie" header will be ignored, use `cookies_file` option instead. Default value is `"Accept-Language": "en-US,en;q=0.9"`.
 * `adjust_update_interval`: change delay before next update based on response headers. This setting doesn't affect timeouts after failed requests. Default value is `true`.
 * `quiet_start`: throw away new records on the first update after application startup. Default value is `false`.
 * `quiet_first_time`: throw away new records produced on first update of given url. Default value is `true`.
 
 
 #### Produced records types:
@@ -251,105 +685,101 @@
 
 </details>
 
 ---
 
 ### `twitcast` - Monitor for twitcasting.tv
 
-Monitors twitcasting.tv user with a given id, produces a record when it goes live.
+Monitors twitcasting.tv user with given id, produces record when it goes live.
 For user `https://twitcasting.tv/c:username` user id would be `c:username`.
 
-Streams on Twitcasting might be set to be visible only for members of a specific group.
+Streams on Twitcasting might be set to be visible only for members of specific group.
 For monitoring such streams it is necessarily to provide login cookies of
-an account being a member of the group. Password-protected and age-restricted streams
+account being member of the group. Password-protected and age-restricted streams
 do not require that.
 
-Rate limits for the endpoint used to check if user is live are likely relatively high,
+Rate limits for endpoint used to check if user is live are likely relatively high,
 but it is better to keep `update_interval` big enough for combined amount of updates
 for all monitored users to not exceed one request per second.
 
 
 #### Entity configuration options:
-* `name`: name of a specific entity. Used to reference it in `chains` section. Must be unique within a plugin. Required.
+* `name`: name of specific entity. Used to reference it in `Chains` section. Must be unique within a plugin. Required.
 * `user_id`: user id that should be monitored. Required.
 ##### 
-* `update_interval`: how often the user will be checked for being live, in seconds. Default value is `60`.
-* `cookies_file`: path to a text file containing cookies in Netscape format. Not required.
+* `update_interval`: how often user will be checked for being live, in seconds. Default value is `60`.
+* `cookies_file`: path to text file containing cookies in Netscape format. Not required.
 * `headers`: custom HTTP headers as pairs "key": value". "Set-Cookie" header will be ignored, use `cookies_file` option instead. Default value is `"Accept-Language": "en-US,en;q=0.9"`.
 
 
 #### Produced records types:
 
 
 <details markdown="block">
   <summary>TwitcastRecord</summary>
 
-Represents an event of a user going live on Twitcasting
+Represents even of user going live on Twitcasting
 
 
-* `user_id`: unique part of the channel url. 
-* `movie_id`: unique id for the current livestream. 
+* `user_id`: unique part of channel url. 
+* `movie_id`: unique id for current livestream. 
 * `url`: user (channel) url. 
 * `movie_url`: current livestream url. 
 * `title`: livestream title. 
-* `thumbnail_url`: link to the stream thumbnail. 
 
 </details>
 
 ---
 
 ### `twitch` - Monitor for twitch.tv
 
-Monitors twitch.tv user with given username, produces a record when it goes live.
+Monitors twitch.tv user with given username, produces record when it goes live.
 For user `https://www.twitch.tv/username` username would be `username`.
 
 
 #### Entity configuration options:
-* `name`: name of a specific entity. Used to reference it in `chains` section. Must be unique within a plugin. Required.
-* `username`: Twitch username of a monitored channel. Required.
+* `name`: name of specific entity. Used to reference it in `Chains` section. Must be unique within a plugin. Required.
+* `username`: Twitch username of monitored channel. Required.
 ##### 
-* `update_interval`: how often the user will be checked for being live, in seconds. Default value is `300`.
-* `cookies_file`: path to a text file containing cookies in Netscape format. Not required.
+* `update_interval`: how often user will be checked for being live, in seconds. Default value is `300`.
+* `cookies_file`: path to text file containing cookies in Netscape format. Not required.
 * `headers`: custom HTTP headers as pairs "key": value". "Set-Cookie" header will be ignored, use `cookies_file` option instead. Default value is `"Accept-Language": "en-US,en;q=0.9"`.
 * `adjust_update_interval`: change delay before next update based on response headers. This setting doesn't affect timeouts after failed requests. Default value is `true`.
 
 
 #### Produced records types:
 
 
 <details markdown="block">
   <summary>TwitchRecord</summary>
 
-Represents event of a user going live on Twitch
+Represents even of user going live on Twitch
 
 
 * `url`: channel url. 
 * `username`: username value from configuration entity. 
 * `title`: stream title. 
-* `start`: timestamp of the stream start. 
-* `avatar_url`: link to the user's avatar. 
-* `game`: game name, if present. 
 
 </details>
 
 ---
 
 ### `get_url` - Monitor web page text
 
-Download contents of web page at `url` and emit it as a `TextRecord`
-if it has changed since the last update. Intended for working with simple
+Download content of web page at `url` and emit it as a `TextRecord`
+if it has changed since last update. Intended for working with simple
 text endpoints.
 
 
 #### Entity configuration options:
-* `name`: name of a specific entity. Used to reference it in `chains` section. Must be unique within a plugin. Required.
+* `name`: name of specific entity. Used to reference it in `Chains` section. Must be unique within a plugin. Required.
 * `update_interval`: how often the monitored source should be checked for new content, in seconds. Required.
 * `url`: url to monitor. Required.
 ##### 
-* `cookies_file`: path to a text file containing cookies in Netscape format. Not required.
+* `cookies_file`: path to text file containing cookies in Netscape format. Not required.
 * `headers`: custom HTTP headers as pairs "key": value". "Set-Cookie" header will be ignored, use `cookies_file` option instead. Default value is `"Accept-Language": "en-US,en;q=0.9"`.
 * `adjust_update_interval`: change delay before next update based on response headers. This setting doesn't affect timeouts after failed requests. Default value is `true`.
 
 
 #### Produced records types:
 
 
@@ -361,81 +791,102 @@
 
 * `text`: content of the record. 
 
 </details>
 
 ---
 
+### `xmpp` - Send record as a Jabber message
+
+Converts records to text representation and sends them as messages
+to specified recipients. Sends each record in separate message,
+does not impose any limits on frequency or size of messages, leaving
+it to server side.
+
+
+#### Plugin configuration options:
+* `xmpp_username`: JID of the account to be used to send messages, resource included. Required.
+* `xmpp_pass`: password of the account to be used to send messages. Required.
+
+
+
+#### Entity configuration options:
+* `name`: name of specific entity. Used to reference it in `Chains` section. Must be unique within a plugin. Required.
+* `jid`: JID to send message to. Required.
+##### 
+* `timezone`: takes timezone name from <https://en.wikipedia.org/wiki/List_of_tz_database_time_zones> or OS settings if omitted, converts record fields containing date and time to this timezone. Not required.
+
+---
+
 ### `rss` - Youtube channel RSS feed monitor
 
 Monitors channel for new uploads and livestreams using RSS feed
 generated by Youtube. Requires old channel id format. In order to obtain
 RSS feed url for a given channel, use "View Source" on a channel page
 and search for "rss".
 
-Example of a supported url:
+Example of supported url:
 
 - `https://www.youtube.com/feeds/videos.xml?channel_id=UCK0V3b23uJyU4N8eR_BR0QA`
 
-RSS feed is smaller and faster to parse compared to an HTML channel page,
+RSS feed is smaller and faster to parse compared to HTML channel page,
 but by design only shows updates of a single channel and doesn't support
 authentication and therefore unable to show member-only streams.
 
-Scheduled date for upcoming streams is not present in the feed itself, so it
-is obtained by fetching and parsing video page the first time it appears in
+Scheduled date for upcoming streams is not present in feed itself, so it
+is obtained by fetching and parsing video page first time it appears in
 the feed. It then gets updated until stream goes live, unless `track_reschedule`
 option is disabled.
 
 No matter how often the url gets fetched, content of the feed only gets
 changed once every 15 minutes, so setting `update_interval` lower than that
 value is not recommended. This monitor will attempt to calculate time of the
 next update from HTTP headers and schedule next request right after it. Use
 `adjust_update_interval` to disable this behavior.
 
 
 #### Plugin configuration options:
-* `db_path`: path to the sqlite database file keeping history of old records of this monitor.
+* `db_path`: path to sqlite database file keeping history of old records of this monitor.
 Might specify a path to a directory containing the file (with trailing slash)
-or a direct path to the file itself (without a slash). If special value `:memory:` is used,
-database is kept in memory and not stored on disk at all, providing a clean database on every startup. Default value is `db/`.
+or direct path to the file itself (without a slash). If special value `:memory:` is used,
+database is kept in memory and not stored on disk at all, providing a clean database on every startup. Default value is `:memory:`.
 
 
 
 #### Entity configuration options:
-* `name`: name of a specific entity. Used to reference it in `chains` section. Must be unique within a plugin. Required.
+* `name`: name of specific entity. Used to reference it in `Chains` section. Must be unique within a plugin. Required.
 * `url`: url that should be monitored. Required.
 ##### 
 * `update_interval`: How often the feed should be updated, in seconds. Default value is `900`.
-* `cookies_file`: path to a text file containing cookies in Netscape format. Not required.
+* `cookies_file`: path to text file containing cookies in Netscape format. Not required.
 * `headers`: custom HTTP headers as pairs "key": value". "Set-Cookie" header will be ignored, use `cookies_file` option instead. Default value is `"Accept-Language": "en-US,en;q=0.9"`.
 * `adjust_update_interval`: change delay before next update based on response headers. This setting doesn't affect timeouts after failed requests. Default value is `true`.
 * `quiet_start`: throw away new records on the first update after application startup. Default value is `false`.
 * `quiet_first_time`: throw away new records produced on first update of given url. Default value is `true`.
-* `track_reschedule`: keep track of scheduled time of upcoming streams, emit record again if it is changed to an earlier date. Default value is `false`.
+* `track_reschedule`: Keep track of scheduled time of upcoming streams, emit record again if it changed to earlier date. Default value is `true`.
 
 
 #### Produced records types:
 
 
 <details markdown="block">
   <summary>YoutubeFeedRecord</summary>
 
-Youtube video or livestream parsed from a channel's RSS feed
+Youtube video or livestream parsed from channel RSS feed
 
 
 * `url`: link to the video. 
-* `title`: title of the video at the time of parsing. 
-* `published`: published value of the feed item, usually the time when the video was uploaded or the livestream frame was set up. 
-* `updated`: updated value of the feed item. If different from `published`, might indicate either a change to video title, thumbnail or description, or a change in video status, for example livestream ending. 
-* `thumbnail_url`: link to the video thumbnail. 
-* `author`: author's name, as shown on the channel icon. 
-* `video_id`: short string identifying the video on Youtube. Part of the video url. 
-* `summary`: video's description. 
+* `title`: title of the video at time of parsing. 
+* `published`: published value of the feed item, usually the time when video was uploaded or livestream frame was set up. 
+* `updated`: updated value of the feed item. If different from `published` might indicate either a change to video title, thumbnail or description, or change in video status, for example livestream ending. 
+* `author`: author name, as shown on channel icon. 
+* `video_id`: short string identifying video on Youtube. Part of video url. 
+* `summary`: video description. 
 * `views`: current number of views. Is zero for upcoming and ongoing livestreams. 
-* `scheduled`: scheduled time for an upcoming livestream to start at, otherwise absent. 
+* `scheduled`: for upcoming livestream is a time it is scheduled to go live at, otherwise absent. 
 
 </details>
 
 ---
 
 ### `community` - Youtube community page monitor
 
@@ -446,87 +897,87 @@
 Examples of supported url:
 
 - `https://www.youtube.com/@ChannelName/community`
 - `https://www.youtube.com/channel/UCK0V3b23uJyU4N8eR_BR0QA/community`
 
 
 #### Plugin configuration options:
-* `db_path`: path to the sqlite database file keeping history of old records of this monitor.
+* `db_path`: path to sqlite database file keeping history of old records of this monitor.
 Might specify a path to a directory containing the file (with trailing slash)
-or a direct path to the file itself (without a slash). If special value `:memory:` is used,
-database is kept in memory and not stored on disk at all, providing a clean database on every startup. Default value is `db/`.
+or direct path to the file itself (without a slash). If special value `:memory:` is used,
+database is kept in memory and not stored on disk at all, providing a clean database on every startup. Default value is `:memory:`.
 
 
 
 #### Entity configuration options:
-* `name`: name of a specific entity. Used to reference it in `chains` section. Must be unique within a plugin. Required.
-* `url`: url of the community page of the channel. Required.
+* `name`: name of specific entity. Used to reference it in `Chains` section. Must be unique within a plugin. Required.
+* `url`: url of community page of the channel. Required.
 ##### 
-* `update_interval`: how often the community page will be checked for new posts. Default value is `1800`.
-* `cookies_file`: path to a text file containing cookies in Netscape format. Not required.
+* `update_interval`: how often community page will be checked for new posts. Default value is `1800`.
+* `cookies_file`: path to text file containing cookies in Netscape format. Not required.
 * `headers`: custom HTTP headers as pairs "key": value". "Set-Cookie" header will be ignored, use `cookies_file` option instead. Default value is `"Accept-Language": "en-US,en;q=0.9"`.
 * `adjust_update_interval`: change delay before next update based on response headers. This setting doesn't affect timeouts after failed requests. Default value is `true`.
 * `quiet_start`: throw away new records on the first update after application startup. Default value is `false`.
 * `quiet_first_time`: throw away new records produced on first update of given url. Default value is `true`.
 * `max_continuation_depth`: when updating feed with pagination support, only continue for this many pages. Default value is `10`.
 * `next_page_delay`: when updating feed with pagination support, wait this much before loading next page. Default value is `1`.
 * `allow_discontinuity`: when updating feed with pagination support, if this setting is enabled and error happens when loading a page, records from already parsed pages will not be dropped. It will allow update of the feed to finish, but older records from deeper pages will then never be parsed on consecutive updates. Default value is `false`.
-* `fetch_until_the_end_of_feed_mode`: when updating feed with pagination support, enables special mode, which makes a monitor try loading and parsing all pages until the end, even if they have been already parsed. Designed for purpose of archiving entire feed content. Default value is `false`.
+* `fetch_until_the_end_of_feed_mode`: when updating feed with pagination support, enables special mode, which makes monitor try loading and parsing all pages until the end, even if they have been already parsed. Designed for purpose of archiving entire feed content. Default value is `false`.
 
 
 #### Produced records types:
 
 
 <details markdown="block">
   <summary>CommunityPostRecord</summary>
 
 Youtube community post content
 
 
 * `channel_id`: channel ID in old format. 
 * `post_id`: unique id of the post. 
-* `author`: author's channel name. 
-* `avatar_url`: link to the avatar of the channel. 
+* `author`: author channel name. 
+* `avatar_url`: link to avatar of the channel. 
 * `vote_count`: current number of upvotes. 
-* `sponsor_only`: indicates whether the post is member-only. 
+* `sponsor_only`: indicates weather the post is member-only. 
 * `published_text`: localized text saying how long ago the video was uploaded. 
-* `full_text`: post contents as plaintext. 
+* `full_text`: post content as plaintext. 
 * `attachments`: list of links to attached images or video thumbnails. 
-* `video_id`: if the post links to youtube video will contain video id, otherwise absent. 
+* `video_id`: if post links to youtube video will have video id, otherwise absent. 
 * `original_post`: for reposts contains original post content, otherwise absent. 
 
 </details>
 
 
 <details markdown="block">
   <summary>SharedCommunityPostRecord</summary>
 
 Youtube community post that is itself a repost of another post
 
 
 * `channel_id`: channel ID in old format. 
 * `post_id`: unique id of the post. 
-* `author`: author's channel name. 
-* `avatar_url`: link to the avatar of the channel. 
+* `author`: author channel name. 
+* `avatar_url`: link to avatar of the channel. 
 * `published_text`: localized text saying how long ago the video was uploaded. 
 * `full_text`: post content. 
 * `original_post`: not present in shared post. 
 
 </details>
 
 ---
 
 ### `channel` - Youtube channel monitor
 
 Monitors Youtube url listing videos, such as channels main page,
 videos and streams tab of a channel, as well as playlists, and,
 with login cookies, subscriptions feed or the main page.
 
-Due to small differences in presentation in aforementioned
-sources, same video might have slightly different appearance when
+Due to small differences in presentation aforementioned sources
+have, same video might have slightly different appearance when
 parsed from different urls. For example, video parsed from main
 page or subscriptions feed will not have full description text.
 
 Examples of supported url:
 
 - `https://www.youtube.com/@ChannelName`
 - `https://www.youtube.com/@ChannelName/videos`
@@ -534,408 +985,71 @@
 - `https://www.youtube.com/channel/UCK0V3b23uJyU4N8eR_BR0QA/`
 - `https://www.youtube.com/playlist?list=PLWGY3fcU-ZeQmBfoJ6SmT8v2zV8NEhrB2`
 - `https://www.youtube.com/feed/subscriptions` (providing cookies is necessarily)
 
 Unlike `rss` monitor, with login cookies it can see videos and streams
 with limited access (such as member-only).
 
-While monitoring a single channel is less efficient, using this monitor with
+While monitoring a single channel is less efficient, both
+bandwidth- and computational-wise, using this monitor with
 subscriptions feed url on a dedicated account is a recommended way
 to monitor a high amount (hundreds) of channels, as it only requires
 loading a single page to check all of them for updates.
 
-When main page of a channel (https://www.youtube.com/@ChannelName) is viewed
-in logged in state, it might contain "For you" block, which content might
-vary with subsequent updates. As a result, monitoring this url might occasionally
-produce records with old videos that got showed in this block. If monitoring
-without a cookies file is not an option, use a combination of "Videos" and "Streams"
-tabs instead.
-
 
 #### Plugin configuration options:
-* `db_path`: path to the sqlite database file keeping history of old records of this monitor.
+* `db_path`: path to sqlite database file keeping history of old records of this monitor.
 Might specify a path to a directory containing the file (with trailing slash)
-or a direct path to the file itself (without a slash). If special value `:memory:` is used,
-database is kept in memory and not stored on disk at all, providing a clean database on every startup. Default value is `db/`.
+or direct path to the file itself (without a slash). If special value `:memory:` is used,
+database is kept in memory and not stored on disk at all, providing a clean database on every startup. Default value is `:memory:`.
 
 
 
 #### Entity configuration options:
-* `name`: name of a specific entity. Used to reference it in `chains` section. Must be unique within a plugin. Required.
+* `name`: name of specific entity. Used to reference it in `Chains` section. Must be unique within a plugin. Required.
 * `url`: url that should be monitored. Required.
 ##### 
 * `update_interval`: . Default value is `1800`.
-* `cookies_file`: path to a text file containing cookies in Netscape format. Not required.
+* `cookies_file`: path to text file containing cookies in Netscape format. Not required.
 * `headers`: custom HTTP headers as pairs "key": value". "Set-Cookie" header will be ignored, use `cookies_file` option instead. Default value is `"Accept-Language": "en-US,en;q=0.9"`.
 * `adjust_update_interval`: change delay before next update based on response headers. This setting doesn't affect timeouts after failed requests. Default value is `true`.
 * `quiet_start`: throw away new records on the first update after application startup. Default value is `false`.
 * `quiet_first_time`: throw away new records produced on first update of given url. Default value is `true`.
 * `max_continuation_depth`: when updating feed with pagination support, only continue for this many pages. Default value is `10`.
 * `next_page_delay`: when updating feed with pagination support, wait this much before loading next page. Default value is `1`.
 * `allow_discontinuity`: when updating feed with pagination support, if this setting is enabled and error happens when loading a page, records from already parsed pages will not be dropped. It will allow update of the feed to finish, but older records from deeper pages will then never be parsed on consecutive updates. Default value is `false`.
-* `fetch_until_the_end_of_feed_mode`: when updating feed with pagination support, enables special mode, which makes a monitor try loading and parsing all pages until the end, even if they have been already parsed. Designed for purpose of archiving entire feed content. Default value is `false`.
+* `fetch_until_the_end_of_feed_mode`: when updating feed with pagination support, enables special mode, which makes monitor try loading and parsing all pages until the end, even if they have been already parsed. Designed for purpose of archiving entire feed content. Default value is `false`.
 
 
 #### Produced records types:
 
 
 <details markdown="block">
   <summary>YoutubeVideoRecord</summary>
 
 Youtube video or livestream listed among others on Youtube page
 
-Produced by parsing a channels main page, videos and streams tab,
+Produced by parsing channels main page, videos and streams tab,
 as well as playlists, and, with login cookies, subscriptions feed.
 
 
 * `video_id`: short string identifying video on Youtube. Part of video url. 
-* `url`: link to the video, uses `https://www.youtube.com/watch?v=<video_id>` format. 
-* `title`: title of the video at the time of parsing. 
-* `summary`: snippet of the video description. Not always available. 
+* `url`: link to video, uses `https://www.youtube.com/watch?v=<video_id>` format. 
+* `title`: title of the video at time of parsing. 
+* `summary`: snippet of video description. Not always available. 
 * `scheduled`: scheduled date for upcoming stream or premiere. 
 * `author`: channel name. 
-* `avatar_url`: link to the avatar of the channel. Not always available. 
-* `thumbnail_url`: link to the video thumbnail. 
+* `avatar_url`: link to avatar of the channel. Not always available. 
 * `channel_link`: link to the channel uploading the video. 
 * `channel_id`: channel ID in old format (such as `UCK0V3b23uJyU4N8eR_BR0QA`). 
 * `published_text`: localized text saying how long ago the video was uploaded. 
 * `length`: text showing the video duration (hh:mm:ss). 
 * `is_upcoming`: indicates that video is an upcoming livestream or premiere. 
 * `is_live`: indicates that the video is a livestream or premiere that is currently live. 
-* `is_member_only`: indicated that the video is limited to members of the channel. Note that the video status might be changed at any time. 
-
-</details>
-
----
-
-### `prechat` - Youtube livechat monitor
-
-Monitor chat of a Youtube livestream and produce a record
-for each chat message. Though it is capable of processing
-chat on an ongoing stream and chat replay on a stream VOD,
-the main purpose is to monitor and preserve chat of upcoming
-livestreams.
-
-Some features, such as polls, are not supported.
-
-
-#### Plugin configuration options:
-* `db_path`: path to the sqlite database file keeping history of old records of this monitor.
-Might specify a path to a directory containing the file (with trailing slash)
-or a direct path to the file itself (without a slash). If special value `:memory:` is used,
-database is kept in memory and not stored on disk at all, providing a clean database on every startup. Default value is `db/`.
-
-
-
-#### Entity configuration options:
-* `name`: name of a specific entity. Used to reference it in `chains` section. Must be unique within a plugin. Required.
-* `url`: url of a video frame with a chat. Required.
-##### 
-* `cookies_file`: path to a text file containing cookies in Netscape format. Not required.
-* `headers`: custom HTTP headers as pairs "key": value". "Set-Cookie" header will be ignored, use `cookies_file` option instead. Default value is `"Accept-Language": "en-US,en;q=0.9"`.
-* `quiet_start`: throw away new records on the first update after application startup. Default value is `false`.
-* `quiet_first_time`: throw away new records produced on first update of given url. Default value is `true`.
-
-
-#### Produced records types:
-
-
-<details markdown="block">
-  <summary>YoutubeChatRecord</summary>
-
-Youtube chat message
-
-
-* `author`: message author's name. 
-* `channel`: message author's channel url. 
-* `badges`: localized list of message author's badges (owner, moderator, member, verified and so on). 
-* `timestamp`: timestamp of when the message was sent. 
-* `text`: message content as plaintext. 
-* `amount`: for superchats, string specifying amount and currency, otherwise empty. 
-* `banner_header`: used for special objects in chat, such as pinned messages. 
-* `message_header`: . 
-* `sticker`: supersticker name if the message is a supersticker, otherwise empty. 
-* `color`: message header color (RGB integer), if present. 
-* `video_id`: video_id of the video chat message was sent to. 
-* `video_title`: title of the video chat message was sent to. 
-* `video_author`: name of the channel where the video chat message was sent to is published. 
-* `uid`: unique id of the message. 
-* `action`: internal name of message type. Used for debug purposes. 
-* `renderer`: internal name of message format. Used for debug purposes. 
-
-</details>
-
-
-## Filters:
-
-
-### `filter.noop` - Pass everything through
-
-Lets all incoming records pass through unchanged, effectively
-doing nothing with them. As any other filter it has entities,
-so it can be used as a merging point to gather records from
-multiple chains and process them in a single place.
-
-
-#### Entity configuration options:
-* `name`: name of a specific entity. Used to reference it in `chains` section. Must be unique within a plugin. Required.
-
----
-
-### `filter.void` - Drop everything
-
-Does not produce anything, dropping all incoming records.
-Can be used to stuff multiple chains in one if the need ever arises.
-
-
-#### Entity configuration options:
-* `name`: name of a specific entity. Used to reference it in `chains` section. Must be unique within a plugin. Required.
-
----
-
-### `filter.match` - Keep records with specific words
-
-This filter lets through records that have one of the values
-defined by `patterns` list found in any (or specified) field of the record.
-
-
-#### Entity configuration options:
-* `name`: name of a specific entity. Used to reference it in `chains` section. Must be unique within a plugin. Required.
-* `patterns`: list of strings to search for in the record. Required.
-##### 
-* `fields`: field names to search the patterns in. If not specified, all fields are checked. Not required.
-
----
-
-### `filter.exclude` - Drop records with specific words
-
-This filter lets through records that have none of the values
-defined by `patterns` list found in any (or specified) field of the record.
-
-
-#### Entity configuration options:
-* `name`: name of a specific entity. Used to reference it in `chains` section. Must be unique within a plugin. Required.
-* `patterns`: list of strings to search for in the record. Required.
-##### 
-* `fields`: field names to search the patterns in. If not specified, all fields are checked. Not required.
-
----
-
-### `filter.event` - Filter for records with "Event" type
-
-Only lets through Events and not normal Records. Can be used to
-set up notifications on events (such as errors) from, for example,
-`execute` plugin within the same chain that uses it, by separating
-them from regular records.
-
-
-#### Entity configuration options:
-* `name`: name of a specific entity. Used to reference it in `chains` section. Must be unique within a plugin. Required.
-##### 
-* `event_types`: list of event types. See descriptions of plugins producing events for possible values. Not required.
-
-
-#### Produced records types:
-
-
-<details markdown="block">
-  <summary>Event</summary>
-
-Record produced by an internal event (usually error) inside the plugin
-
-
-* `event_type`: text describing the nature of event, can be used to filter classes of events, such as errors. 
-* `text`: text describing specific even details. 
-
-</details>
-
----
-
-### `filter.type` - Filter for records of specific type
-
-Only lets through records of specified types, such as `Event` or `YoutubeVideoRecord`.
-
-
-#### Entity configuration options:
-* `name`: name of a specific entity. Used to reference it in `chains` section. Must be unique within a plugin. Required.
-* `types`: list of records class names, such as "Record" and "Event" . Required.
-##### 
-* `exact_match`: whether match should check for exact record type or look in entire records hierarchy up to Record. Default value is `false`.
-
----
-
-### `filter.json` - Format record as JSON
-
-Takes record and produces a new `TextRecord` rendering fields of the
-original record in JSON format, with option for pretty-print.
-
-
-#### Entity configuration options:
-* `name`: name of a specific entity. Used to reference it in `chains` section. Must be unique within a plugin. Required.
-##### 
-* `prettify`: whether output should be multiline and indented or a single line. Default value is `false`.
-
-
-#### Produced records types:
-
-
-<details markdown="block">
-  <summary>TextRecord</summary>
-
-Simplest record, containing only a single text field
-
-
-* `text`: content of the record. 
-
-</details>
-
----
-
-### `filter.format` - Format record as text
-
-Takes a record and produces a new `TextRecord` by taking `template` string
-and replacing "{placeholder}" with value of `placeholder` field of the
-current record, where `placeholder` is any field the record might have.
-If one of the placeholders is not a field of a specific record, it will be
-replaced with a value defined in `missing` parameter if it is specified,
-otherwise it will be left intact.
-
-
-#### Entity configuration options:
-* `name`: name of a specific entity. Used to reference it in `chains` section. Must be unique within a plugin. Required.
-* `template`: template string with placeholders that will be filled with corresponding values from current record. Required.
-##### 
-* `missing`: if specified, will be used to fill template placeholders that do not have corresponding fields in current record. Not required.
-
-
-#### Produced records types:
-
-
-<details markdown="block">
-  <summary>TextRecord</summary>
-
-Simplest record, containing only a single text field
-
-
-* `text`: content of the record. 
-
-</details>
-
----
-
-### `filter.deduplicate` - Drop already seen records
-
-Checks if the `field` field value of the current record has already been
-present in one of the previous records and only let it through otherwise.
-
-`field` might be either a record field name or one of `hash` or `as_json`
-for sha1 and fulltext comparison. If `field` is not present in the current
-record, it will be passed through as if it's new.
-
-This filter will work with records of any type, as long as they have defined
-field (all records have `hash` and `as_json`). For example, it is possible
-to ensure no multiple records for a single video will be produced
-in a chain, that gather records from Youtube channel and Youtube RSS monitors,
-by passing them to an entity of this filter with `field` set to `video_id`.
-
-Note, that history is kept in memory, so it will not be persisted between
-restarts.
-
-
-#### Entity configuration options:
-* `name`: name of a specific entity. Used to reference it in `chains` section. Must be unique within a plugin. Required.
-##### 
-* `field`: field name to use for comparison. Default value is `hash`.
-* `history_size`: how many old records should be kept in memory. Default value is `10000`.
-
----
-
-### `filter.nitter.pick` - Pick `NitterRecord` with specified properties
-
-Lets through `NitterRecord` if it matches any of specified criteria.
-All records from other sources pass through without filtering.
-
-
-#### Entity configuration options:
-* `name`: name of a specific entity. Used to reference it in `chains` section. Must be unique within a plugin. Required.
-##### 
-* `retweet`: match retweets. Default value is `false`.
-* `reply`: match replies. Default value is `false`.
-* `quote`: match quotes. Default value is `false`.
-* `regular_tweet`: match regular tweets that are not a retweet, reply or quote. Default value is `false`.
-* `author`: match if a given string is a part of the name of the author of the tweet. Not required.
-* `username`: match if a given string is a part of tweet author's username (without the "@" symbol). Not required.
-
-
-#### Produced records types:
-
-
-<details markdown="block">
-  <summary>NitterRecord</summary>
-
-Single post as parsed from Nitter instance
-
-Depending on the tweet type (regular, retweet, reply, quote) some fields might be empty
-
-
-* `retweet_header`: text line saying this is a retweet. 
-* `reply_header`: text line saying this tweet is a reply. 
-* `url`: tweet url. 
-* `author`: user's visible name. 
-* `username`: user's handle. 
-* `avatar_url`: link to the picture used as the user's avatar. 
-* `published`: tweet timestamp. 
-* `text`: tweet text with stripped formatting. 
-* `html`: tweet text as raw html. 
-* `attachments`: list of links to attached images or video thumbnails. 
-* `quote`: Nested NitterRecord containing tweet being quited. 
-
-</details>
-
----
-
-### `filter.nitter.drop` - Drop `NitterRecord` without specified properties.
-
-Lets through `NitterRecord` if it doesn't match all of the specified criteria.
-All records from other sources pass through without filtering.
-
-
-#### Entity configuration options:
-* `name`: name of a specific entity. Used to reference it in `chains` section. Must be unique within a plugin. Required.
-##### 
-* `retweet`: match retweets. Default value is `false`.
-* `reply`: match replies. Default value is `false`.
-* `quote`: match quotes. Default value is `false`.
-* `regular_tweet`: match regular tweets that are not a retweet, reply or quote. Default value is `false`.
-* `author`: match if a given string is a part of the name of the author of the tweet. Not required.
-* `username`: match if a given string is a part of tweet author's username (without the "@" symbol). Not required.
-
-
-#### Produced records types:
-
-
-<details markdown="block">
-  <summary>NitterRecord</summary>
-
-Single post as parsed from Nitter instance
-
-Depending on the tweet type (regular, retweet, reply, quote) some fields might be empty
-
-
-* `retweet_header`: text line saying this is a retweet. 
-* `reply_header`: text line saying this tweet is a reply. 
-* `url`: tweet url. 
-* `author`: user's visible name. 
-* `username`: user's handle. 
-* `avatar_url`: link to the picture used as the user's avatar. 
-* `published`: tweet timestamp. 
-* `text`: tweet text with stripped formatting. 
-* `html`: tweet text as raw html. 
-* `attachments`: list of links to attached images or video thumbnails. 
-* `quote`: Nested NitterRecord containing tweet being quited. 
+* `is_member_only`: indicated that the video is limited to members of the channel. Note that video status might be changed at any time. 
 
 </details>
 
 ---
 
 ### `filter.channel` - Pick `YoutubeVideoRecord` with specified properties
 
@@ -943,267 +1057,100 @@
 All records from other sources pass through without filtering.
 
 If multiple settings are set to `true`, they all should match. Use multiple
 entities if picking records with any of multiple properties is required.
 
 
 #### Entity configuration options:
-* `name`: name of a specific entity. Used to reference it in `chains` section. Must be unique within a plugin. Required.
+* `name`: name of specific entity. Used to reference it in `Chains` section. Must be unique within a plugin. Required.
 ##### 
-* `upcoming`: to pass the filter a record should be either upcoming livestream or scheduled premiere. Default value is `false`.
-* `live`: to pass the filter a record should be an ongoing livestream. Default value is `false`.
-* `member_only`: to pass the filter a record should be marked as member-only. Default value is `false`.
+* `upcoming`: to pass filter record should be either upcoming livestream or scheduled premiere. Default value is `true`.
+* `live`: to pass filter record should be an ongoing livestream. Default value is `false`.
+* `member_only`: to pass filter record should be marked as member-only. Default value is `false`.
 
 
 #### Produced records types:
 
 
 <details markdown="block">
   <summary>YoutubeVideoRecord</summary>
 
 Youtube video or livestream listed among others on Youtube page
 
-Produced by parsing a channels main page, videos and streams tab,
+Produced by parsing channels main page, videos and streams tab,
 as well as playlists, and, with login cookies, subscriptions feed.
 
 
 * `video_id`: short string identifying video on Youtube. Part of video url. 
-* `url`: link to the video, uses `https://www.youtube.com/watch?v=<video_id>` format. 
-* `title`: title of the video at the time of parsing. 
-* `summary`: snippet of the video description. Not always available. 
+* `url`: link to video, uses `https://www.youtube.com/watch?v=<video_id>` format. 
+* `title`: title of the video at time of parsing. 
+* `summary`: snippet of video description. Not always available. 
 * `scheduled`: scheduled date for upcoming stream or premiere. 
 * `author`: channel name. 
-* `avatar_url`: link to the avatar of the channel. Not always available. 
-* `thumbnail_url`: link to the video thumbnail. 
+* `avatar_url`: link to avatar of the channel. Not always available. 
 * `channel_link`: link to the channel uploading the video. 
 * `channel_id`: channel ID in old format (such as `UCK0V3b23uJyU4N8eR_BR0QA`). 
 * `published_text`: localized text saying how long ago the video was uploaded. 
 * `length`: text showing the video duration (hh:mm:ss). 
 * `is_upcoming`: indicates that video is an upcoming livestream or premiere. 
 * `is_live`: indicates that the video is a livestream or premiere that is currently live. 
-* `is_member_only`: indicated that the video is limited to members of the channel. Note that the video status might be changed at any time. 
+* `is_member_only`: indicated that the video is limited to members of the channel. Note that video status might be changed at any time. 
 
 </details>
 
-
-## Actions:
-
-
-### `discord.hook` - Send record to Discord using webhook
-
-To generate webhook url follow instructions in "Making a Webhook" section of
-<https://support.discord.com/hc/en-us/articles/228383668-Intro-to-Webhooks>
-
-Some record types support rich formatting when sent to Discord, such as
-showing the author's avatar and links to attached images. Youtube videos will
-show thumbnail, however embedding video itself is not supported.
-
-Records coming within six seconds one after another will be batched together into a single message.
-When too many records are received at once, they will be sent with delays to conform to Discord
-rate limits. Records deemed to be too long to fit in a Discord message
-[length limits](https://discord.com/developers/docs/resources/channel#create-message-jsonform-params)
-will be dropped with a warning.
-
-
-#### Entity configuration options:
-* `name`: name of a specific entity. Used to reference it in `chains` section. Must be unique within a plugin. Required.
-* `url`: webhook url. Required.
-##### 
-* `consume_record`: whether record should be consumed or passed down the chain after processing. Disabling it allows chaining multiple Actions. Default value is `true`.
-* `timezone`: takes timezone name from <https://en.wikipedia.org/wiki/List_of_tz_database_time_zones> (or OS settings if omitted), converts record fields containing date and time to this timezone. Not required.
-
 ---
 
-### `execute` - Run pre-defined shell command
-
-Take `command` string, replace keywords provided in `placeholders` with corresponding fields
-of currently processed record. For example, if `command` is set to
-
-    "yt-dlp {url}"`
-
-and currently processed record comes from Youtube RSS feed and has `url` field value
-`https://www.youtube.com/watch?v=L692Sxz3thw`, then with default `placeholders`
-resulting command will be
-
-    yt-dlp https://www.youtube.com/watch?v=L692Sxz3thw
-
-Note that placeholders do not have to be wrapped in `{}` and can, in fact, be any
-arbitrary text strings. However, placeholders are replaced by corresponding values
-one after another, so using piece of text that might come up in record field might
-produce unexpected results.
-
-`command` string is not treated as raw shell command. Instead, it is split into list
- of elements, where first element specifies the program executable, and the rest
- specify the arguments. It is therefore not possible to use shell features such as pipes
- or execute multiple commands in one line.
-
-Make sure the executable the command uses (`yt-dlp` in this case) is installed and
-can be run from the working directory by current user. It is advised to confirm that
-the command can be executed manually and it finishes without errors before automating it.
-
-For each entity, a separate working directory can be configured. Output is shown
-in the same window by default, but can be redirected to a file, with either static
-or autogenerated name.
-
-Produces Events at startup and successful or erroneous termination of the executed command
-if corresponding entity settings are enabled. They can be used to send Discord
-or Jabber notifications or execute another command when it happens.
-
-Processed record itself can also be passed down the chain if the command failed,
-providing a way to try a different one as a fallback. For example, record with
-Youtube url could be first handled by `ytarchive` and passed to `yt-dlp` if
-it happens to fail due to video link not being a livestream.
-
-
-#### Entity configuration options:
-* `name`: name of a specific entity. Used to reference it in `chains` section. Must be unique within a plugin. Required.
-* `command`: shell command to be executed on every received record. Supports placeholders that will be replaced with currently processed record fields values. Required.
-##### 
-* `consume_record`: whether record should be consumed or passed down the chain after processing. Disabling it allows chaining multiple Actions. Default value is `true`.
-* `working_dir`: path to the directory where command will be executed. If not set current working directory is used. Supports templating with {...}. Not required.
-* `log_dir`: write executed process output to a file in this directory if set. If it is not set, output will not be redirected to file. Not required.
-* `log_filename`: filename to write executed process output to. If not defined, it is generated automatically based on command and entity name. Not required.
-* `placeholders`: parts of `command` string that should be replaced with processed record fields, defined as mapping `'placeholder': 'record field name'`. Default value is `"{url}": "url", "{title}": "title", "{text}": "text"`.
-* `static_placeholders`: parts of `command` string that will be replaced with provided values, defined as mapping `'placeholder': 'replacement string'`. Intended to allow reusing same `command` template for multiple entities. Not required.
-* `forward_failed`: emit currently processed record down the chain if the subprocess returned non-zero exit code. Can be used to define fallback command in case this one fails. Default value is `false`.
-* `report_failed`: emit Event with type "error" if the subprocess returned non-zero exit code or raised exception. Default value is `true`.
-* `report_finished`: emit Event with type "finished" if the subprocess returned zero as exit code. Default value is `false`.
-* `report_started`: emit Event with type "started" before starting a subprocess. Default value is `false`.
-
-
-#### Produced records types:
-
-
-<details markdown="block">
-  <summary>Event</summary>
-
-Record produced by an internal event (usually error) inside the plugin
-
-
-* `event_type`: text describing the nature of event, can be used to filter classes of events, such as errors. 
-* `text`: text describing specific even details. 
-
-</details>
-
----
-
-### `to_file` - Write record to a text file
+### `prechat` - Youtube livechat monitor
 
-Takes a record coming from a Chain, converts it to text representation,
-and writes to a file in given directory. When a file already exists,
-new records can be appended to the end of the file or overwrite it.
+Monitor chat of Youtube livestream and produce a record
+for each chat message. Though it is capable of processing
+a chat on ongoing stream and chat replay on a stream VOD,
+the main purpose is to monitor and preserve chat of upcoming
+livestreams.
 
-Output file name can be static or generated dynamically based on the template
-filled with values from the record fields: every occurrence of `{text}`
-in filename will be replaced with the value of the `text` field of processed
-record, if the record has one.
+Some features, such as polls, are not supported.
 
-Allows writing the record as human-readable text representation or as names and
-values of the record fields in json format. For custom format template, pass the record
-through `filter.format` plugin prior to this one.
 
-Produces `Event` with `error` type if writing to target file fails.
+#### Plugin configuration options:
+* `db_path`: path to sqlite database file keeping history of old records of this monitor.
+Might specify a path to a directory containing the file (with trailing slash)
+or direct path to the file itself (without a slash). If special value `:memory:` is used,
+database is kept in memory and not stored on disk at all, providing a clean database on every startup. Default value is `:memory:`.
 
-Note discrepancy between default value of `encoding` setting between `from_file`
-and `to_file` plugins. Former is expected to be able to read files produced by
-different software and therefore relies on system-wide settings. It would make
-sense to do the same in the latter, but it would introduce possibility of failing
-to write records containing text with Unicode codepoints that cannot be represented
-using system-wide encoding.
 
 
 #### Entity configuration options:
-* `name`: name of a specific entity. Used to reference it in `chains` section. Must be unique within a plugin. Required.
-* `filename`: name of the output file. Supports templating with {...}. Required.
+* `name`: name of specific entity. Used to reference it in `Chains` section. Must be unique within a plugin. Required.
+* `url`: . Required.
 ##### 
-* `consume_record`: whether record should be consumed or passed down the chain after processing. Disabling it allows chaining multiple Actions. Default value is `true`.
-* `path`: directory where output file should be created. Default is current directory. Supports templating with {...}. Not required.
-* `encoding`: output file encoding. Default value is `utf8`.
-* `output_format`: one of `str`, `repr`, `json`, `pretty_json`, `hash`. Default value is `text`.
-* `overwrite`: whether file should be overwritten in if it already exists. Default value is `true`.
-* `append`: if true, new record will be written at the end of the file without overwriting already present lines. Default value is `true`.
-* `prefix`: string that will be appended before the record text. Can be used to separate records from each other or for simple templating. Not required.
-* `postfix`: string that will be appended after the record text. Not required.
+* `update_interval`: . Default value is `20`.
+* `cookies_file`: path to text file containing cookies in Netscape format. Not required.
+* `headers`: custom HTTP headers as pairs "key": value". "Set-Cookie" header will be ignored, use `cookies_file` option instead. Default value is `"Accept-Language": "en-US,en;q=0.9"`.
+* `quiet_start`: throw away new records on the first update after application startup. Default value is `false`.
+* `quiet_first_time`: throw away new records produced on first update of given url. Default value is `true`.
 
 
 #### Produced records types:
 
 
 <details markdown="block">
-  <summary>Event</summary>
+  <summary>YoutubeChatRecord</summary>
 
-Record produced by an internal event (usually error) inside the plugin
+Youtube chat message
 
 
-* `event_type`: text describing the nature of event, can be used to filter classes of events, such as errors. 
-* `text`: text describing specific even details. 
+* `author`: name of the message author. 
+* `channel`: message author channel url. 
+* `badges`: localized list of message author badges (owner, moderator, member, verified and so on). 
+* `timestamp`: time when message was sent. 
+* `text`: message content as plaintext. 
+* `amount`: for superchats, string specifying amount and currency, otherwise empty. 
+* `banner_header`: used for special objects in chat, such as pinned messages. 
+* `message_header`: . 
+* `sticker`: supersticker name if message is a supersticker, otherwise empty. 
+* `uid`: unique id of the message. 
+* `action`: internal name of message type. Used for debug purposes. 
+* `renderer`: internal name of message format. Used for debug purposes. 
 
 </details>
 
 ---
-
-### `download` - Download a file
-
-Take an url from a field of a processed record with a name specified in `url_field`
-and download it as a file to specified location.
-The field must be present in the record and  must contain a valid url with a scheme
-(such as "https") or a list of such urls.
-
-Primarily designed for downloading images attached to a post, or thumbnails.
-Does not support resuming interrupted downloads or detecting that this exact file is
-already stored at target location without downloading it again.
-
-File extension and name are inferred from HTTP headers and path part of the url,
-unless provided explicitly with `extension` and `filename` parameters.
-Since final file name is determined as a part of the download process, the file
-is initially stored under a temporary name (currently an SHA1 of the url) in the
-download directory, and then renamed to target filename.
-
-If a file with given name already exists, depending on an `overwrite` setting a new file will either
-overwrite it or get stored under different name, generated by combining
-the base name with a number added as part of `rename_suffix`.
-If, however, an exact copy of the new file is found among the files in target directory
-sharing the base name, the new file will be deleted, giving preference to the existing copy.
-
-
-#### Plugin configuration options:
-* `max_concurrent_downloads`: limit for simultaneously active download tasks among all entities. Note that each entity will still process records sequentially regardless of this setting. Default value is `1`.
-* `partial_file_suffix`: appended to a name of the file that is not yet completely downloaded. Default value is `.part`.
-
-
-
-#### Entity configuration options:
-* `name`: name of a specific entity. Used to reference it in `chains` section. Must be unique within a plugin. Required.
-* `url_field`: field in the incoming record containing url of file to be downloaded. Required.
-* `path`: directory where downloaded file should be created. Supports templating with {...}. Required.
-##### 
-* `consume_record`: whether record should be consumed or passed down the chain after processing. Disabling it allows chaining multiple Actions. Default value is `true`.
-* `cookies_file`: path to a text file containing cookies in Netscape format. Not required.
-* `headers`: custom HTTP headers as pairs "key": value". "Set-Cookie" header will be ignored, use `cookies_file` option instead. Not required.
-* `filename`: name downloaded file should be stored under. If not provided will be inferred from HTTP headers or download url. Supports templating with {...}. Not required.
-* `extension`: normally file extension will be inferred from HTTP headers. This option allows to overwrite it. Not required.
-* `overwrite`: whether file should be overwritten in if it already exists. If set to false will cause suffix with a number be added to the newly downloaded file name. Default value is `false`.
-* `rename_suffix`: when overwriting is disabled, this suffix is attached to the base filename with the "{i}" part replaced with a number. Must contain "{i}" exactly once. Default value is ` [{i}]`.
-
----
-
-### `xmpp` - Send records as Jabber messages
-
-Converts records to a text representation and sends them as messages
-to specified recipients. Sends each record in a separate message,
-does not impose any limits on frequency or size of messages, leaving
-it to server side.
-
-
-#### Plugin configuration options:
-* `xmpp_username`: JID of the account to be used to send messages, including resource. Required.
-* `xmpp_pass`: password of the account to be used to send messages. Required.
-
-
-
-#### Entity configuration options:
-* `name`: name of a specific entity. Used to reference it in `chains` section. Must be unique within a plugin. Required.
-* `jid`: JID to send message to. Required.
-##### 
-* `consume_record`: whether record should be consumed or passed down the chain after processing. Disabling it allows chaining multiple Actions. Default value is `true`.
-* `timezone`: takes timezone name from <https://en.wikipedia.org/wiki/List_of_tz_database_time_zones> or OS settings if omitted, converts record fields containing date and time to this timezone. Not required.
-
```

### Comparing `avtdl-0.9.14.3/README.md` & `avtdl-0.9.9/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -9,33 +9,33 @@
     * [Features overview](#features-overview)
     * [Installation](#installation)
     * [Running](#running)
     * [Configuration](#configuration)
       * [Configuration file syntax](#configuration-file-syntax)
       * [Configuration file terminology](#configuration-file-terminology)
       * [Configuration file format](#configuration-file-format)
-        * [settings](#settings)
-        * [actors](#actors)
-        * [chains](#chains)
+        * [Settings](#settings)
+        * [Actors](#actors)
+        * [Chains](#chains)
       * [Examples](#examples)
+        * [Download livestreams from youtube channel](#download-livestreams-from-youtube-channel)
+        * [Save community posts to files](#save-community-posts-to-files)
+        * [Send posts from Nitter instance to Discord](#send-posts-from-nitter-instance-to-discord)
       * [Common options](#common-options)
         * [`update_interval`](#updateinterval)
         * [`cookies_file`](#cookiesfile)
         * [`headers`](#headers)
         * [`timezone`](#timezone)
         * [`fetch_until_the_end_of_feed_mode`](#fetchuntiltheendoffeedmode)
-        * [`quiet_first_time` and `quiet_start`](#quietfirsttime-and-quietstart)
         * [Formatting templates](#formatting-templates)
-        * [Providing path to a file or a directory](#providing-path-to-a-file-or-a-directory)
-      * [Troubleshooting](#troubleshooting)
-    * [Tools commonly used for downloading livestreams](#tools-commonly-used-for-downloading-livestreams)
-      * [Youtube](#youtube)
-      * [Twitcasting](#twitcasting)
-      * [FC2](#fc2)
-      * [Youtube community posts](#youtube-community-posts)
+      * [Tools commonly used for downloading livestreams](#tools-commonly-used-for-downloading-livestreams)
+        * [Youtube](#youtube)
+        * [Twitcasting](#twitcasting)
+        * [FC2](#fc2)
+        * [Youtube community posts](#youtube-community-posts)
 <!-- TOC -->
 
 ---
 
 ### Features overview
 
 Some of the supported features include:
@@ -52,40 +52,38 @@
 
 ### Installation
 
 Python version 3.9 or higher is required.
 
 Installing from git repository:
 
-```bash
-git clone https://github.com/15532th/avtdl.git
-cd avtdl
-pip3 install -r requirements.txt
-```
+- clone or download and unpack the repository
+- (optionally) initialize and activate virtual environment
+- inside the avtdl directory run `pip3 install -r requirements.txt`
 
 Installing from PyPI:
 
-```bash
-pip3 install avtdl
-```
+- (optionally) initialize and activate virtual environment
+- execute `pip3 install avtdl`
 
 Prebuilt executable:
 
-Available on [Releases](https://github.com/15532th/avtdl/releases) page ([latest](https://github.com/15532th/avtdl/releases/latest)) as a single executable or as a zip-archive of the app directory (recommended).
-
+    Not yet available  
 
 ### Running
 
-Depending on the installation method and OS, application might be invoked as `avtdl [options]`, `python3 avtdl.py [options]` or `py avtdl.py [options]`
+If installed from git, use `python3 avtdl.py [options]` inside the project directory.
 
-After installing, proceed with writing configuration file, as described in [Configuration](#configuration) section. [example.config.yml](example.config.yml) can be used as a starting point.
+Use `avtdl [options]` if installed from PyPI.
+
+After installing, proceed with writing configuration file, as described in [Configuration](#configuration) section.
 
 By default, configuration file is named `config.yml` and located in current working directory. Current directory is also used as default location to create folders for persistent storage and logs, unless redefined in configuration file.
 
-To specify a different config file, use `avtdl --config path/to/config.yml` option. Run `avtdl --help` for full list of options.
+To specify different config file, use `avtdl --config path/to/config.yml` option. Run `avtdl --help` for full list of options.
 
 ### Configuration
 
 #### Configuration file syntax
 
 Currently, configuration is performed with a configuration file that uses [YAML](https://yaml.org) format. It only uses basic features, but anything PyYAML can parse should work.
 
@@ -95,88 +93,86 @@
 
 It is not always required, but is strongly recommended to enclose every value in a sequence or mapping with single or double quotes to avoid ambiguity. Syntax validation is part of config file parsing, and error message will be produced if the file syntax is wrong. If the message is unclear, try pasting configuration file text in any online YAML validator.
 
 #### Configuration file terminology
 
 `Record` is an entity that represents a certain event, such as a new video getting published or a channel going live. It is internally represented as a set of `key: value` pairs, but also typically has a predefined human-friendly string representation used to send it over notification channel. What specific fields record has depends on where it was produced. For example, `record` about a new Youtube video will contain video title and url among other fields.
 
-There is also a special kind of records, `events`, that are generated by plugins themselves, not by data from external source.
-
 Features, such as monitoring RSS feeds or sending XMPP messages, are contained inside `plugins`. Plugins are grouped into three types:
 
 - `monitors` - periodically check something for new content and produce `records` for each new entity
 - `filters` - take `record` as input and then either produce the same `record` as output or drop it, based on a condition, such as presence of certain keywords
 - `actions` - take `record` as input and act on it. Examples of `action` would be sending Discord or Jabber notification or running `yt-dlp` with the url field of the `record` as argument.
 
 For each of the plugins, `entities` are unified sets of settings describing a single element a plugin works with. For RSS feeds monitor, one entity would be defined for every feed it is supposed to check, providing feed url and how often it should be checked for updates.
 
-`chains` combine `entities` of different plugins in sequences, where `records` produced by `monitors` flow through zero or more `filters` to `actors`.
+`Chains` combine `entities` of different plugins in sequences, where `records` produced by `monitors` flow through zero or more `filters` to `actors`.
 
 #### Configuration file format
 
 Configuration file contains three top level sections:
 
 ```yaml
-settings:
+Settings:
     # <application-wide setting>
 
-actors:
+Actors:
     # <plugins with entities they contain>
 
-chains:
+Chains:
     # <sequences of entities names>
 ```
 
 Each section is explained in details below.
 
-##### settings
+##### Settings
 
 This section contains some application settings and can be fully omitted if default values of options are acceptable.
 
 These options mostly regulate logging to a file. To set a log level for console output use command line options instead.
 
 - `log_directory` - path to a directory where application will write log file
 - `logfile_size` - size of a single log file in bytes. After reaching this size the file will be replaced by a new one. Only last 10 files are kept inside the log directory
 - `logfile_level` - how detailed the output to log file is. Can be "DEBUG", "INFO", "WARNING" or "ERROR". It is recommended to keep log file loglevel set to "DEBUG" and only set console output to higher level.
 - `loglevel_override` - allows to overwrite loglevel of a specific logger. Used to prevent a single talkative logger from filling up the log file. Each log line is preceded by log level and logger name. For example, line `[DEBUG  ] [actor.channel.db] successfully connected to sqlite database at ":memory:"` is produced by logger `actor.channel.db` on `DEBUG` level
 
-Example of `settings` section with all default values:
+Example of `Settings` section with all default values:
 
 ```yaml
-settings:
+Settings:
   log_directory: "logs"
   logfile_size: "1000000"
   logfile_level: "DEBUG"
   loglevel_override: 
     bus: "INFO"
     chain: "INFO"
     actor.request: "INFO"
 ```
 
-##### actors
+##### Actors
 
 This section must contain plugin names from [Description and configuration of available plugins](PLUGINS.md). Each of them has the following structure:
 
 ```yaml
-actors:
+Actors:
   <plugin_name>:
     config:
       # <plugin-specific configuration>
     defaults:
       # <options whose values are the same for all entities>
     entities:
       # <list of key-value pairs defining this plugin entities>
 ```
 
-Each plugin section contains three subsections: `config`, `defaults` and `entities`. Specific format is different for each plugin, see [Description and configuration of available plugins](PLUGINS.md) for details. Many plugins don't have `config` section, and `defaults` sections is not mandatory and can be omitted. If field description mentions a default value, it means the field could be omitted from the config section and the default value would be used instead. Fields without defaults are mandatory. If the section ends up not having any values (common for `config` section), it must be omitted.
+Each plugin section contains three subsections: `config`, `defaults` and `entities`. Specific format is different for each plugin, see  [Description and configuration of available plugins](PLUGINS.md) for details. Many plugins don't have `config` section, and `defaults` sections is not mandatory and can be omitted. If field description mentiones a default value, it means the field could be omitted from the config section and the default value would be used instead. Fields without defaults are mandatory. If the section ends up not having any values (common for `config` section), it must be omitted.
 
-Here is an example of `actors` configuration section with a few plugins. Refer to sections in [Description and configuration of available plugins](PLUGINS.md) corresponding to plugin names for detailed explanations on the options.
+Here is an example of `Actors` configuration section with a few plugins. Refer to sections in  [Description and configuration of available plugins](PLUGINS.md) corresponding to plugin names for detailed explanations on the options.
 
 ```yaml
-actors:
+Actors:
 
   rss:  # Youtube channel monitor
     defaults:
         update_interval: 3600 # how often the feed will be checked for updates, in seconds
     entities:
       - name: "One Example Channel"
         url: "https://www.youtube.com/feeds/videos.xml?channel_id=UCK0V3b23uJyU4N8eR_BR0QA"
@@ -194,203 +190,135 @@
     entities:
       - name: "karaoke"
         patterns:
           - "karaoke"
           - "sing"
 
   discord.hook:  # send Discord message using webhook
-    entities:
-      - name: "notifications"
-        url: "https://discord.com/api/webhooks/1176072251045217473/N-tDdv_iIZnUl6I67GcWqmO0GlNDgCBRYTYf2Z-lfUsLk0HcvvK-i0thuPXiigXcB6h6"
+    - name: "notifications"
+      url: "https://discord.com/api/webhooks/1176072251045217473/N-tDdv_iIZnUl6I67GcWqmO0GlNDgCBRYTYf2Z-lfUsLk0HcvvK-i0thuPXiigXcB6h6"
 ```
 
-It features four plugins: two for monitoring data sources (`rss` and `community`), one for matching against patterns (`filter.match`), and one more for sending notifications (`discord.hook`). Note how each entry in `entities` list has a `name` parameter: it will be later used in `chains` section to refer to a specific entity of a plugin.
+It features four plugins: two for monitoring data sources (`rss` and `community`), one for matching against patterns (`filter.match`), and one more for sending notifications (`discord.hook`). Note how each entry in `entities` list has a `name` parameter: it will be later used in `Chains` section to refer to a specific entity of a plugin.
 `rss` plugin's `entities` section sets it to monitor two Youtube channels RSS feeds, with default `update_interval` value for both of them overwritten in `defaults`. `community` plugin shows an example of plugin-wide option `db_path` in `config` section, explicitly setting persistent storage location.
 
-##### chains
+##### Chains
 
-As explained in the [Configuration file terminology](#configuration-file-terminology) section, plugins can be divided into three types: `monitors`, `filters` and `actions`. A `monitor` can only produce new records. A `filter` consumes records and decides to either output them or not based on its settings. An `action` only consumes `records`, but can produce `events`, for example in case of an error.
-
-A chain groups entities from plugins in the `actors` section in a sequence, where `records` from `monitors` get through `filters` and trigger `actions`. Each entity is identified by a combination of a plugin name and the entity `name` property. General `chains` section structure is:
+A chain groups entities from plugins in the `Actors` section in a sequence, where `records` from one or more `monitors` get through `filters` and trigger `actions`. Each entity is identified by a combination of a plugin name and the entity `name` property. General `Chains` section structure is:
 
 ```yaml
-chains:
+Chains:
   <arbitrary chain name>:
     - <plugin name>:
       - <entity name>
       - <another entity name>
     - <another plugin name>:
       - <entity name>
 ```
 
 Example, following this structure:
 
 ```yaml
-chains:
+Chains:
   "new streams notifications":
     - rss:
       - "One Example Channel"
       - "Another Example Channel"
     - discord.hook:
        - "notifications"
 ```
 
 In this example a single `chain` named "new streams notifications" declares that all records produced by two entities of the `rss` monitor are forwarded into the `discord.hook` entity to be sent as a messages into a Discord channel.
-According to the configuration in the `actors` section defined [before](#actors), `rss` plugin will check RSS feeds of the two Youtube channels every 3600 seconds. When a new video is uploaded, a new entry appears in the RSS feed, leading to a new `record` being generated on the next update. Due to the `rss` plugin entities being listed in the `chain`, it then gets fed into the `discord.hook` "notifications" entity, which in turn will convert the `record` into a fitting representation and send it to Discord by making a request to a webhook url.
-
-***
-
-Even though `actions` do not forward `records` they received down the chain, they might produce `events` when a certain event happens while processing a record. For example, `execute` plugin might produce an `event` with "error" type if the shell command it was set to execute failed. `Events` are treated as normal `records` and can be passed through `filters` to other `actors`.
-
-```yaml
-chains:
-  "download and notify":
-    - rss:
-        - "Example Channel"
-    - execute:
-        - "run ytarchive"
-    - xmpp:
-        - "notifications"
-```
-
-Records from the `rss` feed will be consumed by `execute` plugin entity and won't make it to `xmpp`, but if the command defined in "run ytarchive" failed, a message about it is passed to "notifications" as `event`.
-
-***
-
-Note, that all plugin entities are stateful, in a sense that if a certain entity of specific plugin is used in multiple chains, _all_ instances will produce all records consumed by _any_ of them.
-
-In its simplest form, a `chain` includes one monitor, zero or more `filters` and ends with an `action`. It is possible to list multiple `monitors` sequentially in one `chain`:
-
-```yaml
-chains:
-  "multiplatform streams notifications":
-    - rss:
-      - "Example Channel 1"
-    - twitch:
-      - "Example Channel 2"
-    - discord.hook:
-        - "notifications"
-```
+According to the configuration in the `Actors` section, `rss` plugin will check RSS feeds of the two Youtube channels every 3600 seconds. When a new video is uploaded, a new entry appears in the RSS feed, leading to a new `record` being generated on the next update. Due to the `rss` plugin entities being listed in the `chain`, it then gets fed into the `discord.hook` "notifications" entity, which in turn will convert the `record` into a fitting representation and send it to Discord by making a request to a webhook url.
 
-When a `monitor` located in the middle of a chain receives a `record` as input, it will be passed down the chain unchanged. In the example above records from the `rss` monitor will fall through `twitch`, ending in `discord.hook`, along with records from `twitch` itself.
+#### Examples
 
-However, if aforementioned entity "Example Channel 1" of the `twitch` plugin is also used in another chain to run a command, next entity will receive not only records from "Example Channel 2" on `twitch`, but also anything produced by "Example Channel 1" of the `rss` plugin.
+##### Download livestreams from youtube channel
 
-<details>
-  <summary>Like this (click to expand):</summary>
+Monitor two Youtube channels (`@ChannelName` and `@AnotherChannelName`) with default update interval of 30 minutes, send new publications urls to `ytarchive`, run in dedicated directories.
 
 ```yaml
-chains:
-  "multiplatform streams notifications":
-    - rss:
-        - "Example Channel 1"
-    - twitch:
-        - "Example Channel 2"
-    - discord.hook:
-        - "notifications"
+Actors:
+  channel:
+    entities:
+      - name: "ChannelName"
+        url: "https://www.youtube.com/@ChannelName"
+      - name: "AnotherChannelName"
+        url: "https://www.youtube.com/@AnotherChannelName"
+
+  execute:
+    default:
+      command: "ytarchive --threads 3 --wait {url} best"
+    entities:
+      - name: "ChannelName"
+        working_dir: "archive/livestreams/channelname/"
+      - name: "AnotherChannelName"
+        working_dir: "archive/livestreams/anotherchannelname/"
 
-  "twitch download":
-    - twitch:
-      - "Example Channel 2"
+Chains:
+  "archive ChannelName":
+    - channel:
+        - "ChannelName"
     - execute:
-      # receives records from both twitch and rss feed monitors
-      - "streamlink for Example Channel 2"
-```
-
-</details>
-
-**To avoid unexpected chains interconnections, it is generally advised to only place monitors at the beginning of a chain, and only use any `filter` entity in a single place.**
-
-***
-
-One exception to this rule would be using a `filter.noop` (or any other filter's) entity as a way to merge records produced by multiple monitors into a single processing chain.
-
-In the following example records from Youtube and Twitch monitors are fed into "multiplexor" entity of `noop` filter, which simply passes all records through unchanged. Output of the "multiplexor" then passed to `discord.hook` "notifications" entity after some (possible complex) filtering and preprocessing.
-
-```yaml
-chains:
-
-  "from youtube":
-    - rss:
-        - "Example Channel"
-        - "Another Example Channel"
-    - filter.noop:
-        - "multiplexor"
-
-  "from twitch":
-    - twitch:
-        - "Example Channel"
-    - filter.noop:
-        - "multiplexor"
-
-  "to discord":
-    - filter.noop:
-        - "multiplexor"
-    - filter.exclude:
-        - "notifications blacklist"
-    - filter.channel:
-        - "livestreams notifications"
-    - discord.hook:
-        - "notifications"
+        - "ChannelName"
+  "archive AnotherChannelName":
+    - channel:
+        - "AnotherChannelName"
+    - execute:
+        - "AnotherChannelName"
 ```
 
-***
+##### Save community posts to files
 
-If a plugin in a `chain` lists multiple entities, all of them will receive records from previous one, and all of them will generate records based on it.
+Monitor community page of `@ChannelName` and save each new post as a text file, using post id as a name. Uses cookies to access member-only posts.
 
 ```yaml
-chains:
-  "interesting streams notifications":
-    - rss:
-      - "Example Channel"
-    - filter.match:
-      - "sing"
-      - "game"
-      - "talk"
-    - xmpp:
-      - "notifications"
-```
+Actors:
+  community:
+    entities:
+      - name: "ChannelName"
+        url: "https://www.youtube.com/@ChannelName/community"
+        cookies_file: cookies.txt
 
-When two entities of such plugin let the same record through, it will effectively be duplicated, coming down the chain twice. To mitigate it, either give each entity its own `chain`, or use `filter.deduplicate` plugin to drop repeating `records` before passing it to the `action`:
+  to_file:
+    entities:
+      - name: "ChannelName"
+        path: "archive/community/channelname/"
+        filename: "{post_id}.txt"
 
-```yaml
-chains:
-  "interesting streams notifications":
-    - rss:
-      - "Example Channel"
-    - filter.match:
-      - "sing"
-      - "game"
-      - "talk"
-    - filter.deduplicate:
-        - "interesting streams in Example Channel"
-    - xmpp:
-      - "notifications"
+Chains:
+  "community posts on ChannelName":
+    - community:
+        - "ChannelName"
+    - to_file:
+        - "ChannelName"
 ```
 
-***
+##### Send posts from Nitter instance to Discord
 
-It is also possible for multiple entities to produce duplicate records simply because they monitor the same source. In the example below records from "subscriptions feed" might be already seen by "Example Channel". Then one of them will be dropped on `filter.deduplicate`.
+Monitor `@UserName` posts by parsing `nitter.net` once every two hours, send messages to Discord channel using webhook.
 
 ```yaml
-chains:
-  "interesting streams notifications":
-    - channel:
-        - "Example Channel"
-        - "subscriptions feed"
-    - filter.deduplicate:
-        - "youtube notifications"
-    - xmpp:
-        - "notifications"
-```
+Actors:
+  nitter:
+    - name: "UserName"
+      url: "https://nitter.net/username/with_replies"
+      update_interval: 7200
 
-#### Examples
+  discord.hook:
+    - name: "my server"
+      url: "https://discord.com/api/webhooks/..."
 
-Example configuration file [example.config.yml](example.config.yml) contains a combination of a few common workflows and can be used as starting point.
-[EXAMPLES.md](EXAMPLES.md) lists a few independent configuration files, highlighting usage of specific plugin or plugins combination.
+Chains:
+  "repost UserName":
+    - nitter:
+        - "UserName"
+    - discord.hook:
+        - "my server"
+```
 
 #### Common options
 
 Main description of plugins configuration is provided in [Description and configuration of available plugins](PLUGINS.md), this section aims to explain some nuances of several options used in multiple plugins without overloading each plugin description.
 
 ##### `update_interval`
 
@@ -419,15 +347,15 @@
 ##### `headers`
 
 Allows to specify HTTP headers that will be sent with every update request. Example of the intended use would be specifying preferred language with the [Accept-Language](https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/Accept-Language) header. Headers sent to a specific page by browser can be found by inspecting request in Network tab of Developer tools of the browser.
 
 Headers are specified in `"key": "value"` format. This example ensures locale-dependant elements of Youtube community post, such as published date, are presented in English regardless of IP address geolocation:
 
 ```yaml
-actors:
+Actors:
 
   community:
     defaults:
       headers:
         "Accept-Language": "en-US,en;q=0.9"
       entities:
         ...
@@ -443,141 +371,87 @@
 
 ##### `fetch_until_the_end_of_feed_mode`
 
 Intended for one time use, to allow loading, for example, an entire playlist or all available posts on a community tab on Youtube channel for archiving purposes. 
 
 Normally, when updating a community tab or a user page on Nitter instance, plugin will stop after encountering posts that have already been seen on previous updates or when maximum depth is reached. If this option is enabled, the plugin will try to load all pages available on first update and will continue trying until it succeeds at least once. After that it is recommended to delete this option from the config to avoid unnecessarily load on server on the app restart.
 
-##### `quiet_first_time` and `quiet_start`
-
-When content of a newly added feed is loaded and parsed for the first time, it might contain hundreds of new entries. Option `quiet_first_time` tells a monitor to throw them away to avoid causing a torrent of notifications on initial update of the feed. On consequent updates these entries will be considered already processed.
-
-It means that after a feed url is added to the monitor, it will only generate records when feed gets new entries that came in after the moment of first update on startup.
-
-The `quiet_start` option does the same on every startup, discarding entities that were added to the feed while the application wasn't running.
-
 ##### Formatting templates
 
 Allows populating a predefined text string with values of current record fields. Used for making dynamic strings, i.e. output file name, or to change the text representation of the record with help of the `filter.format` plugin.
 
 Formatting is performed by taking any text enclosed in `{}` and, if it contains a name of field of the currently processed record, replacing it with the value of the field.
 
 For example, the following config snippet uses a template to output each processed record to a separate file, with the record's `post_id` field used as the file name.
 
 ```yaml
-actors:
+Actors:
+  [...]
+
   to_file:
     entities:
       - name: "ChannelName"
         path: "archive/community/channelname/"
         filename: "{post_id}.txt"
 ```
 
 Note how this makes this plugin entity only suitable for processing records coming from the `community` plugin, since only that plugin uses this field. If currently processed record does not have this field, it will not be replaced with anything, and the resulting file name will be quite literally `{post_id}.txt`. If this happens, debug message is produced in log. Some field names are used by multiple plugins, one notable example being the `url` field, which usually contains the url of a new livestream, video or post.
 
-When a template is used as a file name or as a path to a directory, field values will have characters that are not allowed to be used in filenames replaced with underscore. Final string length and characters are not checked for compliance with OS restrictions, however.
-
-##### Providing path to a file or a directory
-
-Both absolute and relative paths can be used, with relative being resolved in a current working directory `avtdl` is run from. It is possible to use either `/` and `\\` as directory separator regardless of OS, but note that latter must be used twice. Shell variables and aliases, such as `~`, are not expanded, and full path must be provided instead.
-
-
-
-#### Troubleshooting
-
-When loading and parsing configuration file, `avtdl` will check the structure and parameters and report everything it finds wrong. Location of the error is presented as a semicolon-separated list of sections from the top one to most nested. For example, running it with unedited `example.config.yml` will produce the following output:
-
-    [ERROR  ] [avtdl] Failed to process configuration file, following errors occurred: 
-        error parsing "cookies.txt" in config section actors: channel: entities: 0: cookies_file: Path does not point to a file
-        error parsing "cookies.txt" in config section actors: community: entities: 0: cookies_file: Path does not point to a file
 
-It means that `cookies_file` parameters of first entity of both `channel` and `community` plugins specify path to a file that doesn't exist and therefore cannot be loaded and parsed as cookies file.
-
-Even if configuration file is valid and loads successfully, it still might be configured in a way causing application to fail or not produce desired results. Some obviously wrong settings, as well as any runtime errors deemed serious enough, such as network connection problems, will be reported with `[WARNING ]` or `[ERROR  ]` loglevels. Issues of lower severity are reported on `[DEBUG  ]` level along with debug messages providing context of what was happening around the moment. By default, they are not shown in console unless application is run with `--debug` argument, but are written in log file, as defined in `settings` section of the configuration file.
-
-### Tools commonly used for downloading livestreams
+#### Tools commonly used for downloading livestreams
 
 Before automating the download process it is a good idea to try doing it manually first and ensure everything is working properly. This section provides an overview of some tools that can be used for archiving livestreams, including those offering monitoring in addition to downloading that can be used as single-purpose alternatives to avtdl.
 
 Old versions of these tools (as well as avtdl itself) might sometimes not be able to work due to breaking changes on the site side, so in case of problems it is worth checking that the most recent version is used.
 
 Only a brief description is offered here. Refer to each tool's documentation for a full list of available options and adjust suggested command lines to fit specific use cases.
 
 All mentioned tools support customization of the output name format and can download limited access streams if an authorization cookies file is provided.
 
-#### Youtube
+##### Youtube
 
 [ytarchive](https://github.com/Kethsar/ytarchive) is a tool for downloading upcoming and ongoing livestreams. Checks scheduled date and waits for upcoming livestream, can monitor channel for livestreams and download them as they start. Typical command would be
 
-    ytarchive --threads 4 --add-metadata --thumbnail --wait --merge {url} best
-
-Running `ytarchive` without an url, specifying the `--wait` key or selecting the livestream quality will cause it to prompt for user input asking to provide missing details, which works in interactive environment but would wait forever if happened in automated job, so caution should be applied to provide all necessary info in command string. Quality can be specified as a slash-delimited list, and it is generally advised to always add `best` at the end: `1080p/1080p60/best`.
-
-<details>
-  <summary>Commonly used options (click to expand):</summary>
-
-- `--add-metadata` - writes stream info, such as title, description, channel name and date to output file metadata
-- `--cookies "path/to/file.txt"` - file with Youtube login cookies, allows downloading member-only streams
-- `--threads "number"` - run multiple download threads in parallel. Use if download is falling behind the live edge. Usually 2 or 3 threads is enough for a livestream
-- `--thumbnail` - embed the stream thumbnail as a video preview
-- `--wait` and `--merge` are used to avoid prompting for user input
-
-</details>
-
-`ytarchive` depends on [ffmpeg](https://www.ffmpeg.org/download.html) for merging video and audio in output file and for embedding thumbnail and metadata, so it should be installed or provided as an executable.
+    ytarchive --threads 4 --add-metadata --thumbnail --wait {url} best
 
 [yt-dlp](https://github.com/yt-dlp/yt-dlp) can be used to download Youtube videos, playlists or entire channel content. Might not work well with livestreams.
 
     yt-dlp --add-metadata --embed-thumbnail --embed-chapters --embed-subs {url}
 
-`yt-dlp` also requires [ffmpeg](https://www.ffmpeg.org/download.html) for many functions, but might work without it for simple download.
-
-<details>
-  <summary>Commonly used options (click to expand):</summary>
-
-- `--add-metadata` - writes stream info, such as title, description, channel name and date to output file metadata
-- `--cookies "path/to/file.txt"` - file with Youtube login cookies, allows downloading member-only streams
-- `--download-archive archive.txt` - writes video id of successfully downloaded streams into `archive.txt` file, marking them as processed to skip on consequential runs. Commonly used to download only new videos from a playlist or a channel even if already downloaded ones were moved
-- `--embed-thumbnail` - embed the stream thumbnail as a video preview
-- `--embed-subs --write-subs --sub-langs "live_chat, en"` - deals with subtitles and livechat. `--write-subs` stores them as a separate files (`vtt` for subtitles and `json` for livechat), `--embed-subs` will additionally put subtitles (but not a chat) in output video file
-- `--format` - allows to select quality and codecs. See [docs](https://github.com/yt-dlp/yt-dlp#format-selection) for examples
-- `-o` - format of the output file name ([docs](https://github.com/yt-dlp/yt-dlp#output-template)). One particularly useful feature is ability to limit maximum value of specific placeholder in order to prevent total filename length exceeding filesystem limit (typically 255 symbols or bytes). For example, format template `-o "[%(upload_date)s] %(title).200B - %(id)s.%(ext)s"` will ensure video title gets trimmed to 200 bytes regardles of how many characters it takes
-</details>
-
 Youtube livestreams are often encoded with `AVC1` codec, but stream archive would usually also have format encoded in `VP9` available, providing similar quality with much lower size after a certain time, usually a few hours after the stream end. 
 
 To keep long-term archive size small while ensuring a recording will still be present if the stream archive is not available, it is possible to use a combination of ytarchive (controlled by avtdl or standalone) to obtain the stream recording immediately and yt-dlp managed by a scheduler on daily basis to collect processed versions. To ensure yt-dlp won't try to download a livestream before it gets converted to `VP9`, exact quality code can be specified as the video format:
 
     yt-dlp --add-metadata --embed-thumbnail --embed-chapters --embed-subs --write-subs --sub-langs "live_chat, en" --merge-output-format mkv --download-archive archive.txt --format 303+251/248+251 {url}
 
 This way yt-dlp will skip ongoing and newly finished livestreams, leaving them to ytarchive, and download `VP9` format when it becomes available on the next day.
 
 To archive an entire channel, both uploads and livestreams, run yt-dlp with a channel url instead of a specific video or playlist:
 
-    yt-dlp --add-metadata --embed-thumbnail --embed-chapters --embed-subs --write-subs --sub-langs "live_chat, en" --merge-output-format mkv --download-archive archive.txt --format 303+251/248+251/bestvideo*+bestaudio/best -o "[%(upload_date)s] %(title).200B - %(id)s.%(ext)s" https://www.youtube.com/@ChannelName
+    yt-dlp --add-metadata --embed-thumbnail --embed-chapters --embed-subs --write-subs --sub-langs "live_chat, en" --merge-output-format mkv --download-archive archive.txt --format 303+251/248+251/bestvideo*+bestaudio/best -o "[%(upload_date)s] %(title)s - %(id)s.%(ext)s" https://www.youtube.com/@ChannelName
 
-#### Twitcasting
+##### Twitcasting
 
 To download an archive use [yt-dlp](https://github.com/yt-dlp/yt-dlp).
 
 Livestreams on Twitcasting are particularly sensitive to network connection latency, and the recording file might often end up missing fragments if connection is not good enough or the server is under high load. Using lower quality might help.
 
 Ongoing livestreams also can be downloaded with [yt-dlp](https://github.com/yt-dlp/yt-dlp). When specifying quality other than `best`, note that not every quality code is available on every stream, and it is better to always add `best` as a fallback option. 
 
     yt-dlp -f 220k/best https://twitcasting.tv/c:username
 
 Another tool for downloading livestreams is [TwcLazer](https://github.com/HoloArchivists/TwcLazer). It uses different download method compared to yt-dlp, so one might serve as alternative to another when something breaks due to changes on server side.
 
-#### FC2
+##### FC2
 
 [fc2-live-dl](https://github.com/HoloArchivists/fc2-live-dl) can be used for downloading ongoing FC2 streams. Default options are good for most cases:
 
     fc2-live-dl {url}
 
 Comes with [autofc2](https://github.com/HoloArchivists/fc2-live-dl#autofc2) script, that allows to continuously monitor a channel and download a stream as it goes live. Uses configuration file in JSON format, but file structure is simple and an example config is provided. Paste config file content in any online JSON validator to check it for possible formatting errors.
 
 Note, that FC2 only allows a single window with particular livestream, and opening channel that is currently being downloaded in a browser will result in error and is likely to interrupt download.
 
-#### Youtube community posts
+##### Youtube community posts
 
 avtdl supports saving community post text in a file natively, but as an alternative, this fork of [youtube-community-tab](https://github.com/HoloArchivists/youtube-community-tab) might be used. It comes with `ytct.py` script that allows to download either a specific post by direct link or all new posts on a channel. Posts are stored in JSON format, which can be rendered to human-readable text files with third party [ytct-convert.py](https://gist.github.com/15532th/111c8b32e5d82112379703f3eab51e49) script.
```

### Comparing `avtdl-0.9.14.3/avtdl/avtdl.py` & `avtdl-0.9.9/avtdl/avtdl.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,118 +1,129 @@
 #!/usr/bin/env python3
 
 import argparse
 import asyncio
 import logging
 import os
-from asyncio import AbstractEventLoop
 from pathlib import Path
-from typing import Any, Dict, Tuple
 
 import yaml
+from pydantic import ValidationError
 
-from avtdl.core.chain import Chain
-from avtdl.core.config import ConfigParser, ConfigurationError, config_sancheck
-from avtdl.core.info import generate_plugins_description, generate_version_string
-from avtdl.core.interfaces import Actor
+from avtdl.core.config import ConfigParser
+from avtdl.core.info import generate_plugins_description
 from avtdl.core.loggers import set_logging_format, silence_library_loggers
-from avtdl.core.plugins import UnknownPluginError
-from avtdl.core.utils import monitor_tasks, read_file
+from avtdl.core.utils import read_file
 
 
-def load_config(path: Path) -> Any:
+def load_config(path: Path):
+    if not os.path.exists(path):
+        print('Configuration file {} does not exist'.format(path))
+        raise SystemExit
     try:
-        if not os.path.exists(path):
-            raise ValueError('Configuration file {} does not exist'.format(path))
         config_text = read_file(path)
         config = yaml.load(config_text, Loader=yaml.FullLoader)
     except Exception as e:
         print('Failed to parse configuration file:')
         print(e)
         raise SystemExit from e
     return config
 
 
-def parse_config(conf) -> Tuple[Dict[str, Actor], Dict[str, Chain]]:
+def parse_config(conf):
     try:
         actors, chains = ConfigParser.parse(conf)
-    except (ConfigurationError, UnknownPluginError) as e:
+    except ValidationError as e:
         logging.error(e)
         raise SystemExit from e
     except Exception as e:
         logging.exception(e)
         raise SystemExit from e
     return actors, chains
 
 
-def handler(loop: AbstractEventLoop, context: Dict[str, Any]) -> None:
+def handler(loop, context):
     logging.exception(f'unhandled exception in event loop:', exc_info=context.get('exception'))
     loop.default_exception_handler(context)
 
 
-async def install_handler() -> None:
+async def run(runnables):
     loop = asyncio.get_running_loop()
     loop.set_exception_handler(handler)
     loop.slow_callback_duration = 100
 
+    tasks = []
+    for runnable in runnables:
+        task = asyncio.create_task(runnable.run(), name=runnable.__class__.__name__)
+        tasks.append(task)
+    while True:
+        done, pending = await asyncio.wait(tasks, return_when=asyncio.FIRST_EXCEPTION)
+        for task in done:
+            if not task.done():
+                continue
+            if task.exception() is not None:
+                logging.warning(f'task {task.get_name()} has terminated with exception', exc_info=task.exception())
+        if not pending:
+            break
+        tasks = pending
+    logging.info('all tasks are finished in the main loop')
+
 
-async def run(args: argparse.Namespace) -> None:
+def start(args):
     conf = load_config(args.config)
     actors, chains = parse_config(conf)
-    config_sancheck(actors, chains)
 
-    await install_handler()
-    tasks = []
-    for runnable in actors.values():
-        task = asyncio.create_task(runnable.run(), name=runnable.__class__.__name__)
-        tasks.append(task)
-    await monitor_tasks(tasks)
+    for chain_name, chain_instance in chains.items():
+        for actor_name, entities in chain_instance.conf:
+            actor = actors.get(actor_name)
+            if actor is None:
+                logging.warning(f'chain "{chain_name}" references actor "{actor_name}, absent in "Actors" section. It might be a typo in the chain configuration')
+                continue
+            orphans = set(entities) - actor.entities.keys()
+            for orphan in orphans:
+                logging.warning(f'chain "{chain_name}" references "{actor_name}: {orphan}", but actor "{actor_name}" has no "{orphan}" entity. It might be a typo in the chain conf configuration')
 
+    asyncio.run(run(actors.values()), debug=True)
 
-def make_docs(args: argparse.Namespace) -> None:
+
+def make_docs(args):
     output = args.plugins_doc
-    doc = generate_plugins_description(output.suffix == '.html')
+    doc = generate_plugins_description(output.suffix == 'html')
     try:
         with open(output, 'wt', encoding='utf8') as fp:
             fp.write(doc)
     except OSError as e:
         logging.error(f'failed to write documentation file "{output}": {e}')
         raise SystemExit from e
+    
 
-
-def main() -> None:
+def main():
     description = '''Tool for monitoring rss feeds and other sources and running commands for new entries'''
     parser = argparse.ArgumentParser(description=description)
     help_v = 'set loglevel to DEBUG'
     parser.add_argument('-d', '--debug', action='store_true', default=False, help=help_v)
-    help_v = 'print version and exit'
-    parser.add_argument('-v', '--version', action='store_true', default=False, help=help_v)
+    help_v = 'set loglevel to INFO'
+    parser.add_argument('-v', '--verbose', action='store_true', default=False, help=help_v)
     help_c = 'specify path to configuration file to use instead of default'
     parser.add_argument('-c', '--config', type=Path, default='config.yml', help=help_c)
     help_h = 'write plugins documentation in given file and exit. Documentation format is deduced by file extension: html document for ".html", markdown otherwise'
     parser.add_argument('-p', '--plugins-doc', type=Path, required=False, help=help_h)
     args = parser.parse_args()
 
     if args.debug:
         log_level = logging.DEBUG
-    else:
+    elif args.verbose:
         log_level = logging.INFO
+    else:
+        log_level = logging.WARNING
 
     set_logging_format(log_level)
     silence_library_loggers()
 
-    try:
-        if args.version:
-            print(generate_version_string())
-        elif args.plugins_doc is not None:
-            make_docs(args)
-        else:
-            asyncio.run(run(args), debug=True)
-    except KeyboardInterrupt:
-        if args.debug:
-            logging.exception('Interrupted, exiting... Printing stacktrace for debugging purpose:')
-        else:
-            logging.info('Interrupted, exiting...')
+    if args.plugins_doc is not None:
+        make_docs(args)
+    else:
+        start(args)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `avtdl-0.9.14.3/avtdl/core/chain.py` & `avtdl-0.9.9/avtdl/core/chain.py`

 * *Files identical despite different names*

### Comparing `avtdl-0.9.14.3/avtdl/core/config.py` & `avtdl-0.9.9/avtdl/core/config.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,31 +1,28 @@
-import logging
 from functools import wraps
 from pathlib import Path
 from typing import Any, Dict, Generic, List, Tuple, Type, TypeVar
 
-from pydantic import BaseModel, ConfigDict, ValidationError, create_model
+from pydantic import BaseModel, ValidationError, create_model
 
 from avtdl.core.chain import Chain, ChainConfigSection
 from avtdl.core.loggers import LogLevel, override_loglevel, set_file_logger
 from avtdl.core.plugins import Plugins
 
 
 class ConfigurationError(Exception):
     '''Generic exception raised if parsing config failed'''
 
 def format_validation_error(e: ValidationError) -> str:
     msg = 'Failed to process configuration file, following errors occurred: '
     errors = []
     for err in e.errors():
-        user_input = str(err['input'])
-        user_input = user_input if len(user_input) < 85 else user_input[:50] + ' [...] ' + user_input[-30:]
         location = ': '.join(str(l) for l in err['loc'])
-        error = 'error parsing "{}" in config section {}: {}'
-        errors.append(error.format(user_input, location, err['msg']))
+        error = 'error parsing "{}" in config section "{}": {}'
+        errors.append(error.format(err['input'], location, err['msg']))
     return '\n    '.join([msg] + errors)
 
 def try_parsing(func):
     @wraps(func)
     def wrapper(*args, **kwargs):
         try:
             return func(*args, **kwargs)
@@ -47,19 +44,17 @@
 
 class ActorConfigSection(BaseModel):
     config: dict = {}
     defaults: dict = {}
     entities: List[dict]
 
 class Config(BaseModel):
-    model_config = ConfigDict(extra='forbid')
-
-    settings: SettingsSection = SettingsSection()
-    actors: Dict[str, ActorConfigSection]
-    chains: Dict[str, ChainConfigSection]
+    Settings: SettingsSection = SettingsSection()
+    Actors: Dict[str, ActorConfigSection]
+    Chains: Dict[str, ChainConfigSection]
 
 
 TConfig = TypeVar('TConfig')
 TEntity = TypeVar('TEntity')
 
 class SpecificActorConfigSection(BaseModel, Generic[TConfig, TEntity]):
     config: TConfig
@@ -96,25 +91,25 @@
 
 class ConfigParser:
 
     @staticmethod
     def flatten_config(config: Config) -> Config:
         conf = config.model_dump()
         actors_section: Dict[str, ActorConfigSection] = {}
-        for name, section in config.actors.items():
+        for name, section in config.Actors.items():
             actors_section[name] = ActorParser.flatten_actor_section(name, section)
-        conf['actors'] = actors_section
+        conf['Actors'] = actors_section
         return Config(**conf)
 
     @staticmethod
     def load_models(config: Config) -> Type['SpecificConfig']:
-        actors_model = ActorParser.load_actors_plugins_model(config.actors)
+        actors_model = ActorParser.load_actors_plugins_model(config.Actors)
         SpecificConfigModel = create_model('SpecificConfig',
-                                     actors=(actors_model, ...),
-                                     chains=(Dict[str, ChainConfigSection], ...)
+                                     Actors=(actors_model, ...),
+                                     Chains=(Dict[str, ChainConfigSection], ...)
                                      )
         return SpecificConfigModel
 
     @classmethod
     def create_chains(cls, chains_section: Dict[str, ChainConfigSection]) -> Dict[str, Chain]:
         chains = {}
         for name, chain_config in chains_section.items():
@@ -123,34 +118,21 @@
 
     @classmethod
     @try_parsing
     def parse(cls, conf) -> Tuple[Dict[str, Any], Dict[str, Chain]]:
         # do basic structural validation of config file
         config = Config(**conf)
 
-        configure_loggers(config.settings)
-        Plugins.load(config.settings.plugins_directory)
+        configure_loggers(config.Settings)
+        Plugins.load(config.Settings.plugins_directory)
 
         # after that entities transformation and specific plugins validation can be safely performed
         flatted_conf = cls.flatten_config(config)
         SpecificConfig = cls.load_models(config)
         specific_config = SpecificConfig(**flatted_conf.model_dump())
 
-        actors = ActorParser.create_actors(specific_config.actors)
-        chains = ConfigParser.create_chains(specific_config.chains)
+        actors = ActorParser.create_actors(specific_config.Actors)
+        chains = ConfigParser.create_chains(specific_config.Chains)
 
         return actors, chains
 
 
-def config_sancheck(actors, chains):
-    """check for possible non-fatal misconfiguration and issue a warning"""
-    for chain_name, chain_instance in chains.items():
-        for actor_name, entities in chain_instance.conf:
-            actor = actors.get(actor_name)
-            if actor is None:
-                logging.warning(
-                    f'chain "{chain_name}" references actor "{actor_name}, absent in "Actors" section. It might be a typo in the chain configuration')
-                continue
-            orphans = set(entities) - actor.entities.keys()
-            for orphan in orphans:
-                logging.warning(
-                    f'chain "{chain_name}" references "{actor_name}: {orphan}", but actor "{actor_name}" has no "{orphan}" entity. It might be a typo in the chain conf configuration')
```

### Comparing `avtdl-0.9.14.3/avtdl/core/db.py` & `avtdl-0.9.9/avtdl/core/db.py`

 * *Files identical despite different names*

### Comparing `avtdl-0.9.14.3/avtdl/core/interfaces.py` & `avtdl-0.9.9/avtdl/core/interfaces.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,26 +3,21 @@
 import logging
 from abc import ABC, abstractmethod
 from collections import defaultdict
 from hashlib import sha1
 from textwrap import shorten
 from typing import Callable, Dict, List, Optional, Sequence, Tuple, Union
 
-from pydantic import BaseModel, ConfigDict, Field
+from pydantic import BaseModel
 
 MAX_REPR_LEN = 60
 
 class Record(BaseModel):
     '''Data entry, passed around from Monitors to Actions through Filters'''
 
-    model_config = ConfigDict(use_attribute_docstrings=True)
-
-    origin: Optional[str] = Field(default=None, exclude=True)
-    """semicolon-separated names of actor and entity record originated from"""
-
     @abstractmethod
     def __str__(self) -> str:
         '''Text representation of the record to be sent in a message, written to a file etc.'''
 
     @abstractmethod
     def __repr__(self) -> str:
         '''Short text representation of the record to be printed in logs'''
@@ -128,123 +123,74 @@
         except ValueError:
             self.logger.error(f'failed to split message topic "{topic}"')
             raise
         return actor, entity
 
 
 class ActorConfig(BaseModel):
-    model_config = ConfigDict(use_attribute_docstrings=True)
     name: str
 
 class ActorEntity(BaseModel):
-    model_config = ConfigDict(use_attribute_docstrings=True)
-
     name: str
-    """name of a specific entity. Used to reference it in `chains` section. Must be unique within a plugin"""
+    """name of a specific entity. Used to reference it in `Chains` section. Must be unique within a plugin"""
 
 class Actor(ABC):
-    model_config = ConfigDict(use_attribute_docstrings=True)
 
     def __init__(self, conf: ActorConfig, entities: Sequence[ActorEntity]):
         self.conf = conf
         self.logger = logging.getLogger(f'actor').getChild(conf.name)
         self.bus = MessageBus()
         self.entities: Dict[str, ActorEntity] = {entity.name: entity for entity in entities}
 
         for entity_name in self.entities:
             topic = self.bus.incoming_topic_for(self.conf.name, entity_name)
             self.bus.sub(topic, self._handle)
 
-    def __repr__(self):
-        text = f'{self.__class__.__name__}({list(self.entities)})'
-        return shorten(text, MAX_REPR_LEN)
-
     def _handle(self, topic: str, record: Record) -> None:
         _, entity_name = self.bus.split_message_topic(topic)
-        if entity_name not in self.entities:
+        if not entity_name in self.entities:
             logging.warning(f'received record on topic {topic}, but have no entity with name {entity_name} configured, dropping record {record!r}')
             return
         entity = self.entities[entity_name]
         try:
-            self.handle_record(entity, record)
+            self.handle(entity, record)
         except Exception:
             self.logger.exception(f'{self.conf.name}.{entity_name}: error while processing record "{record!r}"')
 
     @abstractmethod
-    def handle_record(self, entity: ActorEntity, record: Record) -> None:
+    def handle(self, entity: ActorEntity, record: Record) -> None:
         '''Perform an action on record if entity in self.entities'''
 
     def on_record(self, entity: ActorEntity, record: Record):
         '''Implementation should call it for every new Record it produces'''
         topic = self.bus.outgoing_topic_for(self.conf.name, entity.name)
         self.bus.pub(topic, record)
 
+    def __repr__(self):
+        return f'{self.__class__.__name__}({list(self.entities)})'
+
     async def run(self):
         '''Will be run as asyncio task once everything is set up'''
         return
 
 
-class MonitorEntity(ActorEntity):
-    pass
-
-
-class Monitor(Actor, ABC):
-
-    def __init__(self, conf: ActorConfig, entities: Sequence[MonitorEntity]):
-        super().__init__(conf, entities)
-
-    def handle_record(self, entity: MonitorEntity, record: Record) -> None:
-        # For convenience’s sake monitors pass incoming records down the chain.
-        # It allows using multiple monitors in a single chain, one after another
-        self.on_record(entity, record)
-
-    def on_record(self, entity: ActorEntity, record: Record):
-        '''Implementation should call it for every new Record it produces'''
-        origin = f'{self.conf.name}:{entity.name}'
-        if record.origin == origin:
-            self.logger.warning(f'[{entity.name}] received incoming record produced by self, which indicates loop in a chain, dropping: "{record!r}".\nCheck config for chains, passing records to each other in a loop.')
-            return
-        if record.origin is None:
-            record.origin = origin
-        super().on_record(entity, record)
-
 class FilterEntity(ActorEntity):
     pass
 
-
 class Filter(Actor):
 
     def __init__(self, conf: ActorConfig, entities: Sequence[FilterEntity]):
         super().__init__(conf, entities)
         self.logger = logging.getLogger(f'filters.{self.conf.name}')
 
-    def handle_record(self, entity: FilterEntity, record: Record):
+    def handle(self, entity: FilterEntity, record: Record):
         filtered = self.match(entity, record)
         if filtered is not None:
             self.on_record(entity, filtered)
         else:
-            self.logger.debug(f'[{entity.name}] record dropped: "{record!r}"')
+            self.logger.debug(f'record "{record!r}" dropped on filter {entity!r}')
 
     @abstractmethod
     def match(self, entity: FilterEntity, record: Record) -> Optional[Record]:
         '''Take a record and return it if it matches some condition
         or otherwise process it, else return None'''
 
-
-class ActionEntity(ActorEntity):
-    consume_record: bool = True
-    """whether record should be consumed or passed down the chain after processing. Disabling it allows chaining multiple Actions"""
-
-
-class Action(Actor, ABC):
-
-    def __init__(self, conf: ActorConfig, entities: Sequence[ActionEntity]):
-        super().__init__(conf, entities)
-
-    def handle_record(self, entity: ActionEntity, record: Record) -> None:
-        self.handle(entity, record)
-        if not entity.consume_record:
-            self.on_record(entity, record)
-
-    @abstractmethod
-    def handle(self, entity: ActionEntity, record: Record):
-        '''Method for implementation to process incoming record'''
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `avtdl-0.9.14.3/avtdl/core/loggers.py` & `avtdl-0.9.9/avtdl/core/loggers.py`

 * *Files identical despite different names*

### Comparing `avtdl-0.9.14.3/avtdl/core/monitors.py` & `avtdl-0.9.9/avtdl/core/monitors.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,64 +6,47 @@
 from pathlib import Path
 from typing import Any, Dict, List, Mapping, Optional, Sequence, Tuple, Union
 
 import aiohttp
 from pydantic import Field, FilePath, field_validator, model_validator
 
 from avtdl.core.db import BaseRecordDB
-from avtdl.core.interfaces import ActorConfig, Monitor, MonitorEntity, Record
-from avtdl.core.utils import Delay, check_dir, convert_cookiejar, get_cache_ttl, get_retry_after, load_cookies, \
-    monitor_tasks, show_diff
+from avtdl.core.interfaces import Actor, ActorConfig, ActorEntity, Record
+from avtdl.core.utils import Delay, check_dir, convert_cookiejar, get_cache_ttl, get_retry_after, load_cookies, show_diff
 
 HIGHEST_UPDATE_INTERVAL = 4 * 3600
 
-
-class TaskMonitorEntity(MonitorEntity):
+class TaskMonitorEntity(ActorEntity):
     update_interval: float
     """how often the monitored source should be checked for new content, in seconds"""
 
 
-class BaseTaskMonitor(Monitor):
+class BaseTaskMonitor(Actor):
 
     def __init__(self, conf: ActorConfig, entities: Sequence[TaskMonitorEntity]):
         super().__init__(conf, entities)
-        self.tasks: Dict[str, Optional[asyncio.Task]] = {}
+        self.tasks: Dict[str, asyncio.Task] = {}
 
-    async def run(self):
-        startup_tasks = await self.start_cyclic_tasks()
-        # keep an eye on possible exceptions in startup process
-        self.tasks['startup_tasks_monitor'] = asyncio.create_task(monitor_tasks(startup_tasks), name='startup_tasks_monitor')
+    def handle(self, entity: ActorEntity, record: Record) -> None:
+        self.on_record(entity, record)
 
-        # check for entities tasks
-        while True:
-            for name, task in self.tasks.items():
-                if task is None:
-                    continue
-                if not task.done():
-                    continue
-                if task.exception() is not None:
-                    self.logger.error(f'[{name}] task {task.get_name()} has terminated with exception', exc_info=task.exception())
-                else:
-                    self.logger.debug(f'[{name}] task {task.get_name()} has finished normally')
-                self.tasks[name] = None
-            await asyncio.sleep(1)
+    async def run(self):
+        # start cyclic tasks
+        await self.start_cyclic_tasks()
+        # and wait forever
+        await asyncio.Future()
 
-    async def start_cyclic_tasks(self) -> Sequence[asyncio.Task]:
+    async def start_cyclic_tasks(self):
         by_entity_interval = defaultdict(list)
         for entity in self.entities.values():
             by_entity_interval[entity.update_interval].append(entity)
-        by_group_interval = defaultdict(list)
-        for interval, entities in by_entity_interval.items():
-            by_group_interval[interval / len(entities)].extend(entities)
-        startup_tasks = []
+        by_group_interval = {interval / len(entities): entities for interval, entities in by_entity_interval.items()}
         for interval in sorted(by_group_interval.keys()):
             entities = by_group_interval[interval]
-            task = asyncio.create_task(self.start_tasks_for(entities, interval), name=f'start_cyclic_tasks_{interval}')
-            startup_tasks.append(task)
-        return startup_tasks
+            asyncio.create_task(self.start_tasks_for(entities, interval))
 
     async def start_tasks_for(self, entities, interval):
         logger = self.logger.parent.getChild('scheduler').getChild(self.conf.name)
         if len(entities) == 0:
             logger.debug(f'called with no entities and {interval} interval')
             return
         names = ', '.join([f'{self.conf.name}.{entity.name}' for entity in entities])
@@ -113,25 +96,14 @@
     base_update_interval: float = Field(exclude=True, default=60)
     """internal variable to persist state between updates. Used to keep update_interval while timeout after update error is active"""
     last_modified: Optional[str] = Field(exclude=True, default=None)
     """internal variable to persist state between updates. Used to keep Last-Modified header value"""
     etag: Optional[str] = Field(exclude=True, default=None)
     """internal variable to persist state between updates. Used to keep Etag header value"""
 
-    @field_validator('cookies_file')
-    @classmethod
-    def check_cookies(cls, path: Optional[Path]):
-        if path is None:
-            return None
-        try:
-            load_cookies(path, raise_on_error=True)
-        except Exception as e:
-            raise ValueError(f'{e}') from e
-        return path
-
     def model_post_init(self, __context: Any) -> None:
         self.base_update_interval = self.update_interval
 
 
 class HttpTaskMonitor(BaseTaskMonitor):
     '''Maintain and provide for records aiohttp.ClientSession objects
     grouped by HttpTaskMonitorEntity.cookies_path, which means entities that use
@@ -180,15 +152,15 @@
                     logger.debug(f'[{entity.name}] got Retry-After header with value {raw_header}')
                     entity.update_interval = max(float(retry_after), HIGHEST_UPDATE_INTERVAL)
                     logger.warning(f'[{entity.name}] update interval set to {entity.update_interval} seconds for {url} as requested by response headers')
                     return None
             else:
                 logger.warning(f'[{entity.name}] error while fetching {url}: {e.__class__.__name__} {e}')
 
-            update_interval = int(max(Delay.get_next(entity.update_interval), entity.update_interval))
+            update_interval = int(Delay.get_next(entity.update_interval))
             if entity.update_interval != update_interval:
                 entity.update_interval = update_interval
                 logger.warning(f'[{entity.name}] update interval set to {entity.update_interval} seconds for {url}')
             return None
 
         if response.status == 304:
             logger.debug(f'[{entity.name}] got {response.status} ({response.reason}) from {url}')
@@ -267,15 +239,15 @@
 
     def get_size(self, feed_name: Optional[str] = None) -> int:
         '''return number of records, total or for specified feed, are stored in db'''
         return super().get_size(feed_name)
 
 
 class BaseFeedMonitorConfig(ActorConfig):
-    db_path: Union[Path, str] = Field(default='db/', validate_default=True)
+    db_path: Union[Path, str] = 'db/'
     """path to the sqlite database file keeping history of old records of this monitor.
     Might specify a path to a directory containing the file (with trailing slash)
     or a direct path to the file itself (without a slash). If special value `:memory:` is used,
     database is kept in memory and not stored on disk at all, providing a clean database on every startup"""
 
     @field_validator('db_path')
     @classmethod
@@ -463,17 +435,15 @@
             self.logger.info(
                 f'[{entity.name}] "fetch_until_the_end_of_feed_mode" setting is enabled, will keep loading through already seen pages until the end. Disable it in config after it succeeds once')
 
         current_page = 1
         while True:
             if continuation_context is None:
                 self.logger.debug(f'[{entity.name}] no continuation link on {current_page - 1} page, end of feed reached')
-                if entity.fetch_until_the_end_of_feed_mode:
-                    self.logger.info(f'[{entity.name}] reached the end of the feed at {current_page - 1} page, fetch_until_the_end_of_feed_mode can be disabled now')
-                    entity.fetch_until_the_end_of_feed_mode = False
+                entity.fetch_until_the_end_of_feed_mode = False
                 break
             if not entity.fetch_until_the_end_of_feed_mode:
                 if current_page > entity.max_continuation_depth:
                     self.logger.info(
                         f'[{entity.name}] reached continuation limit of {entity.max_continuation_depth}, aborting update')
                     break
                 if not all(self.record_is_new(record, entity) for record in current_page_records):
@@ -487,14 +457,13 @@
                     # when unable to load _all_ new records, return at least current progress
                     break
                 else:
                     # when unable to load _all_ new records, throw away all already parsed and return nothing
                     # to not cause discontinuity in stored data
                     return []
             records.extend(current_page_records)
-            self.logger.debug(f'[{entity.name}] while parsing page {current_page} got {len(current_page_records)} records')
 
             current_page += 1
             await asyncio.sleep(entity.next_page_delay)
 
         records = records[::-1]
         return records
```

### Comparing `avtdl-0.9.14.3/avtdl/core/plugins.py` & `avtdl-0.9.9/avtdl/core/plugins.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 import importlib.util
 import logging
 from enum import Enum
 from pathlib import Path
 from typing import Any, Callable, Dict
 
 
-class UnknownPluginError(KeyError):
-    """Raised if plugin with given name is not registered"""
-
 class Plugins:
     class kind(Enum):
         ACTOR = 'actor'
         ACTOR_CONFIG = 'actor_config'
         ACTOR_ENTITY = 'actor_entity'
         ASSOCIATED_RECORD = 'associated_record'
 
@@ -28,15 +25,15 @@
             cls.known[kind][name] = factory
 
     @classmethod
     def _get(cls, name: str, kind: kind):
         instance = cls.known[kind].get(name)
         if instance is None:
             known = ', '.join(cls.known[kind].keys())
-            raise UnknownPluginError(f'"{name}" is not registered as {kind.value} plugin. Known {kind.value} plugins are {known}')
+            raise KeyError(f'"{name}" is not registered as {kind.value} plugin. Known {kind.value} plugins are {known}')
         return instance
 
     @classmethod
     def get_actor_factories(cls, name):
         actor_factory = cls._get(name, cls.kind.ACTOR)
         config_factory = cls._get(name, cls.kind.ACTOR_CONFIG)
         entity_factory = cls._get(name, cls.kind.ACTOR_ENTITY)
```

### Comparing `avtdl-0.9.14.3/avtdl/core/utils.py` & `avtdl-0.9.9/avtdl/core/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,34 +1,32 @@
 import asyncio
 import datetime
-import hashlib
 import http
 import json
 import logging
 import os
 import re
 from collections import OrderedDict
 from email.utils import mktime_tz, parsedate_to_datetime
 from enum import Enum
 from http import cookiejar
 from math import log2
 from pathlib import Path
 from textwrap import shorten
 from time import perf_counter_ns
-from typing import Any, Callable, Dict, Hashable, Iterable, List, Optional, Union
+from typing import Any, Callable, Dict, Hashable, List, Optional, Union
 
 import aiohttp
 import lxml.html
 import multidict
 
 from avtdl.core.interfaces import Record
 
 
 def load_cookies(path: Optional[Path], raise_on_error: bool = False) -> Optional[cookiejar.CookieJar]:
-    """load cookies from a text file in Netscape format"""
     logger = logging.getLogger('cookies')
     if path is None:
         return None
     cookie_jar = cookiejar.MozillaCookieJar(path)
     try:
         cookie_jar.load(ignore_discard=True, ignore_expires=True)
         logger.info(f"Successfully loaded cookies from {path}")
@@ -40,49 +38,44 @@
     except (cookiejar.LoadError, OSError) as e:
         if raise_on_error:
             raise
         logger.exception(f'Failed to load cookies from {path}: {e}')
         return None
     return cookie_jar
 
-
 def convert_cookiejar(cookie_jar: cookiejar.CookieJar) -> aiohttp.CookieJar:
-    """convert cookie jar produced by stdlib to format used by aiohttp"""
-    cookies = http.cookies.BaseCookie()
+    cookies = http.cookies.SimpleCookie()
     for cookie in cookie_jar:
         name = cookie.name
         cookies[name] = cookie.value
         cookies[name]['domain'] = cookie.domain
         cookies[name]['path'] = cookie.path
         cookies[name]['expires'] = str(cookie.expires)
         cookies[name]['secure'] = cookie.secure
         cookies[name]['version'] = str(cookie.version)
         cookies[name]['comment'] = cookie.comment
-    new_jar = aiohttp.CookieJar(quote_cookie=False)
+    new_jar = aiohttp.CookieJar()
     new_jar.update_cookies(cookies)
     return new_jar
 
-
 def get_cache_ttl(headers: multidict.CIMultiDictProxy) -> Optional[int]:
-    """
-    check for Expires and Cache-Control headers, return integer representing
-    how many seconds is left until resource is outdated, if they are present
-    and was parsed successfully
-    """
+    '''Check for Expires and Cache-Control headers,
+    return integer representing how many seconds is
+    left until resource is outdated'''
 
     def get_expires_from_cache_control(headers) -> Optional[datetime.datetime]:
         try:
             cache_control = headers.get('Cache-control')
             max_age = re.search('max-age=(\d+)', cache_control)
             max_age_value = datetime.timedelta(seconds=int(max_age))
 
             last_modified = headers.get('Last-Modified')
             last_modified_value = parsedate_to_datetime(last_modified)
 
-            expires = last_modified_value + max_age_value
+            expires  = last_modified_value + max_age_value
             return expires
         except (TypeError, ValueError):
             return None
 
     def get_expires_from_expires_header(headers) -> Optional[datetime.datetime]:
         try:
             expires_header = headers.get('Expires')
@@ -100,18 +93,16 @@
     now = datetime.datetime.now(tz=datetime.timezone.utc)
     delta = (expires - now).total_seconds()
     if delta < 0:
         return None
 
     return int(delta)
 
-
 def get_retry_after(headers: multidict.CIMultiDictProxy) -> Optional[int]:
-    """return parsed value of Retry-After header, if present"""
-    retry_after = headers.get('Retry-After')
+    retry_after =  headers.get('Retry-After')
     if retry_after is None:
         return None
     try:
         return int(retry_after)
     except ValueError:
         pass
     try:
@@ -122,106 +113,69 @@
             return delay
     except (TypeError, ValueError):
         pass
     return None
 
 
 def check_dir(path: Path, create=True) -> bool:
-    """check if directory exists and writable, create if asked"""
+    '''check if directory exists and writable, create if asked'''
     if path.is_dir() and os.access(path, mode=os.W_OK):
         return True
     elif create:
         logging.warning(f'directory {path} does not exists, creating')
         try:
-            path.mkdir(parents=True, exist_ok=True)
+            os.mkdir(path)
             return True
         except OSError as e:
             logging.warning(f'failed to create directory at {path}: {e}')
             return False
     else:
         return False
 
-
 def make_datetime(items) -> datetime.datetime:
-    """take 10-tuple and return datetime object with UTC timezone"""
+    '''take 10-tuple and return datetime object with UTC timezone'''
     if len(items) == 9:
-        items = *items, None
+       items = *items, None
     if len(items) != 10:
         raise ValueError(f'Expected tuple with 10 elements, got {len(items)}')
     timestamp = mktime_tz(items)
     return datetime.datetime.fromtimestamp(timestamp, tz=datetime.timezone.utc)
 
-
-def parse_timestamp_us(timestamp: Union[str, int, None], ) -> Optional[datetime.datetime]:
-    return parse_timestamp(timestamp, 6)
-
-
-def parse_timestamp_ms(timestamp: Union[str, int, None], ) -> Optional[datetime.datetime]:
-    return parse_timestamp(timestamp, 3)
-
-
-def parse_timestamp(timestamp: Union[str, int, None], fraction: int) -> Optional[datetime.datetime]:
-    """parse UNIX timestamp as datetime.datetime"""
-    if timestamp is None:
-        return None
-    try:
-        ts = int(timestamp)
-        dt = datetime.datetime.fromtimestamp(int(ts / 10**fraction), tz=datetime.timezone.utc)
-        return dt
-    except Exception:
-        return None
-
-
 def show_diff(dict1: Dict[str, Any], dict2: Dict[str, Any]) -> str:
-    """pretty-print keys which values in dict1 and dict2 are different"""
     keys = {*dict1.keys(), *dict2.keys()}
     diff = []
     for k in keys:
         v1 = str(dict1.get(k, ''))
         repr_v1 = shorten(v1, 60)
         v2 = str(dict2.get(k, ''))
         repr_v2 = shorten(v2, 60)
         if v1 != v2:
             diff.append(f'[{k[:12]:12}]: {repr_v2:60} |->| {repr_v1:60}')
     return '\n'.join(diff)
 
 
-async def monitor_tasks(tasks: Iterable[asyncio.Task]) -> None:
-    """given list of running tasks, wait for them and report any unhandled exceptions"""
-    while True:
-        done, pending = await asyncio.wait(tasks, return_when=asyncio.FIRST_EXCEPTION)
-        for task in done:
-            if not task.done():
-                continue
-            if task.exception() is not None:
-                logging.error(f'task {task.get_name()} has terminated with exception', exc_info=task.exception())
-        if not pending:
-            break
-        tasks = list(pending)
-
-
 async def request_raw(url: str, session: Optional[aiohttp.ClientSession], logger: Optional[logging.Logger] = None,
-                      method: str = 'GET', params: Optional[Any] = None, data: Optional[Any] = None,
-                      headers: Optional[Dict[str, Any]] = None, retry_times: int = 1, retry_delay: float = 1,
-                      retry_multiplier: int = 1,
-                      raise_errors: bool = False) -> Optional[aiohttp.ClientResponse]:
+                  method: str = 'GET', params: Optional[Any] = None, data: Optional[Any] = None,
+                  headers: Optional[Dict[str, Any]] = None, retry_times: int = 1, retry_delay: float = 1,
+                  retry_multiplier: int = 1,
+                  raise_errors: bool = False) -> Optional[aiohttp.ClientResponse]:
     logger = logger if logger else logging.getLogger('request')
     current_retry_delay = retry_delay
     for attempt in range(0, retry_times + 1):
         last_attempt = attempt == retry_times
         try:
             if session is not None:
                 if session.headers is not None and headers is not None:
                     headers.update(session.headers)
                 async with session.request(method=method, url=url, headers=headers, params=params, data=data) as response:
                     response.raise_for_status()
                     _ = await response.text()
                     return response
             else:
-                async with aiohttp.request(method=method, url=url, headers=headers, params=params, data=data) as response:
+                async with aiohttp.request(method=method, url=url, headers=headers) as response:
                     response.raise_for_status()
                     _ = await response.text()
                     return response
 
         except Exception as e:
             logger.warning(f'error when requesting {url}: {e}')
             if not last_attempt:
@@ -231,98 +185,87 @@
                 continue
             elif raise_errors:
                 raise
             else:
                 return None
     return None
 
-
 async def request(url: str, session: Optional[aiohttp.ClientSession] = None, logger: Optional[logging.Logger] = None,
-                  method: str = 'GET', params: Optional[Any] = None, data: Optional[Any] = None,
-                  headers: Optional[Dict[str, Any]] = None, retry_times: int = 1, retry_delay: float = 1,
-                  retry_multiplier: int = 1,
-                  raise_errors: bool = False) -> Optional[str]:
+                      method: str = 'GET', params: Optional[Any] = None, data: Optional[Any] = None,
+                      headers: Optional[Dict[str, Any]] = None, retry_times: int = 1, retry_delay: float = 1,
+                      retry_multiplier: int = 1,
+                      raise_errors: bool = False) -> Optional[str]:
     logger = logger if logger else logging.getLogger('request')
     response = await request_raw(url, session, logger, method, params, data, headers, retry_times, retry_delay, retry_multiplier, raise_errors)
     if response is None:
         return None
     if response.status >= 300:
         # presuming that there is no point in retrying 3xx and aiohttp will follow redirects transparently
         logger.debug(f'got {response.status} ({response.reason}) from {url}')
         return None
     return await response.text()
 
-
 async def request_json(url: str, session: Optional[aiohttp.ClientSession], logger: Optional[logging.Logger] = None,
-                       method: str = 'GET', params: Optional[Any] = None, data: Optional[Any] = None,
-                       headers: Optional[Dict[str, Any]] = None, retry_times: int = 1, retry_delay: float = 1,
-                       retry_multiplier: int = 1,
-                       raise_errors: bool = False) -> Optional[Any]:
+                  method: str = 'GET', params: Optional[Any] = None, data: Optional[Any] = None,
+                  headers: Optional[Dict[str, Any]] = None, retry_times: int = 1, retry_delay: float = 1,
+                  retry_multiplier: int = 1,
+                  raise_errors: bool = False) -> Optional[Any]:
     logger = logger if logger else logging.getLogger('request_json')
     text = await request(url, session, logger, method, params, data, headers, retry_times, retry_delay, retry_multiplier, raise_errors)
     if text is None:
         return None
     try:
-        parsed = json.loads(text)
-        return parsed
+         parsed = json.loads(text)
+         return parsed
     except json.JSONDecodeError as e:
         logger.debug(f'error parsing response from {url}: {e}. Raw response data: "{text}"')
         if raise_errors:
             raise
         else:
             return None
 
 
 class Delay:
-    """Provide method to calculate next delay for exponential backoff based on S-shaped curve"""
+    '''Provide method to calculate next delay for exponential backoff based on S-shaped curve'''
 
-    A: float = 4600  # upper asymptote
-    k: float = 0.88  # curve growth rate
-    x0: float = 8  # x value corresponding to midpoint of the curve
+    A: float = 4600 # upper asymptote
+    k: float = 0.88 # curve growth rate
+    x0: float = 8 # x value corresponding to midpoint of the curve
 
     @classmethod
     def _sigmoid(cls, x: float) -> float:
         y = cls.A / (1 + 2 ** (-cls.k * (x - cls.x0)))
         return y
 
     @classmethod
     def _inv_sigmoid(cls, y: float) -> float:
-        if y <= 0:
-            return 0
         # raises ValueError if y >= cls.A
         x = cls.x0 - log2((cls.A - y) / y) / cls.k
         return x
 
     @classmethod
     def get_next(cls, current: float) -> float:
-        """
-        Find current value on S-shaped curve and return a next one
-
-        Returns 0 if input is not higher than 0,
-        returns cls.A if input higher than cls.A.
-        """
+        '''Find current value on S-shaped curve and return a next one'''
         try:
             current_step = cls._inv_sigmoid(current)
         except ValueError:
             current_step = current
         next_step = current_step + 1
         next_delay = cls._sigmoid(next_step)
         return next_delay
 
 
 def timeit(func: Callable) -> Callable:
-    """measure time "func()" call takes, print it in log"""
-    def timer(*args, **kwargs) -> Any:
-        begin = perf_counter_ns()
-        result = func(*args, **kwargs)
-        duration = perf_counter_ns() - begin
-        logging.warning(f'{func.__name__}: {duration / 10 ** 6:10}')
-        return result
-
-    return timer
+  def timer(*args, **kwargs) -> Any:
+      begin = perf_counter_ns()
+      result = func(*args, **kwargs)
+      duration = perf_counter_ns() - begin
+      logging.warning(f'{func.__name__}: {duration/10**6:10}')
+      return result
+  return timer
 
 
 class LRUCache:
 
     def __init__(self, max_size: int = 100):
         if max_size <= 0:
             raise ValueError('Maximum cache size must be a positive integer')
@@ -361,65 +304,51 @@
     return find_matching_field(record, text) is not None
 
 
 def sanitize_filename(name: str) -> str:
     """Replace symbols not allowed in file names on NTFS with underscores"""
     return re.sub(r'[\\/:*?"<>|]', "_", name)
 
-
 class OutputFormat(str, Enum):
     str = 'text'
     repr = 'short'
     json = 'json'
     pretty_json = 'pretty_json'
     hash = 'hash'
 
 
 class Fmt:
     """Helper class to interpolate format string from config using data from Record"""
 
     @classmethod
-    def format(cls, fmt: str, record: Record, missing: Optional[str] = None, sanitize: bool = False) -> str:
+    def format(cls, fmt: str, record: Record, missing: Optional[str] = None) -> str:
         """Take string with placeholders like {field} and replace them with record fields"""
         logger = logging.getLogger().getChild('format')
         result = fmt
         record_as_dict = record.model_dump()
-        placeholders: List[str] = re.findall(r'({[^{}\\]+})', fmt)
+        placeholders: List[str] = re.findall(r'(?:[^\\]|^)({[^{}\\]+})', fmt)
         if not placeholders:
             logger.debug(f'format string "{fmt}" has no placeholders, it will be the same for all records')
         for placeholder in placeholders:
             field = placeholder.strip('{}')
             value = record_as_dict.get(field)
             if value is not None:
                 if isinstance(value, datetime.datetime):
-                    value = cls.date(value)
+                    value = value.strftime('%Y-%m-%d %H:%M')
                 else:
                     value = str(value)
-                    if sanitize:
-                        value = sanitize_filename(value)
                 result = result.replace(placeholder, value)
             else:
                 if missing is not None:
                     result = result.replace(placeholder, missing)
                 else:
                     logger.warning(f'placeholder "{placeholder}" used by format string "{fmt}" is not a field of {record.__class__.__name__} ({record!r}), resulting command is unlikely to be valid')
         return result
 
     @classmethod
-    def format_path(cls, path: Union[str, Path], record: Record, missing: Optional[str] = None) -> Path:
-        """Take string with placeholders and replace them with record fields, but strip them from bad symbols"""
-        fmt = str(path)
-        formatted_path = cls.format(fmt, record, missing, sanitize=True)
-        return Path(formatted_path)
-
-    @classmethod
-    def date(cls, dt: datetime.datetime) -> str:
-        return dt.strftime('%Y-%m-%d %H:%M')
-
-    @classmethod
     def save_as(cls, record: Record, output_format: OutputFormat = OutputFormat.str) -> str:
         """Take a record and convert in to string as text/json or sha1"""
         if output_format == OutputFormat.str:
             return str(record)
         if output_format == OutputFormat.repr:
             return repr(record)
         if output_format == OutputFormat.json:
@@ -427,26 +356,16 @@
         if output_format == OutputFormat.pretty_json:
             return record.as_json(2)
         if output_format == OutputFormat.hash:
             return record.hash()
 
 
 def html_to_text(html: str) -> str:
-    """take html fragment, try to parse it and extract text values using lxml"""
     try:
         root = lxml.html.fromstring(html)
-
-        # text_content() skips <img> content altogether
-        # walk tree manually and for images containing links
-        # add them to text representation
-        for elem in root.iter():
-            if elem.tag == 'img':
-                image_link = elem.get('src')
-                if image_link is not None:
-                    elem.text = f'\n{image_link}\n'
         text = root.text_content()
         return text
     except Exception as e:
         logger = logging.getLogger('html_to_text')
         logger.warning(e)
         return html
 
@@ -464,18 +383,7 @@
             text = fp.read()
             return text
         except UnicodeDecodeError:
             pass
     with open(path, encoding='utf8') as fp:
         text = fp.read()
         return text
-
-
-def sha1(text: str) -> str:
-    return hashlib.sha1(text.encode()).digest().hex()
-
-
-def get_cookie_value(jar: aiohttp.CookieJar, key: str) -> Optional[str]:
-    for morsel in jar:
-        if morsel.key == key:
-            return morsel.value
-    return None
```

### Comparing `avtdl-0.9.14.3/avtdl/plugins/discord/webhook.py` & `avtdl-0.9.9/avtdl/plugins/discord/webhook.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,17 +6,16 @@
 from typing import Any, List, Optional, Sequence, Tuple
 
 import aiohttp
 import dateutil
 import multidict
 from pydantic import Field, field_validator
 
-from avtdl.core.interfaces import Action, ActionEntity, ActorConfig, Record
+from avtdl.core.interfaces import Actor, ActorConfig, ActorEntity, Record
 from avtdl.core.plugins import Plugins
-from avtdl.core.utils import monitor_tasks
 
 EMBEDS_PER_MESSAGE = 10
 EMBED_TITLE_MAX_LENGTH = 256
 EMBED_DESCRIPTION_MAX_LENGTH = 4096
 
 
 class DiscordWebhook:
@@ -46,58 +45,50 @@
                 while len(to_be_sent) < EMBEDS_PER_MESSAGE:
                     record = await asyncio.wait_for(self.send_query.get(), 60/EMBEDS_PER_MESSAGE)
                     to_be_sent.append(record)
             except asyncio.TimeoutError:
                 pass
             if len(to_be_sent) == 0:
                 continue
-            try:
-                message, pending_records = MessageFormatter.format(to_be_sent)
-                self.logger.debug(f'[{self.name}] out of {len(to_be_sent)} records {len(pending_records)} are left pending')
-            except Exception as e:
-                self.logger.exception(f'error happened while formatting message: {e}\nRaw records list: "{to_be_sent}"')
-                to_be_sent = []
-                continue
+            message, pending_records = MessageFormatter.format(to_be_sent)
             try:
                 limits_ok = MessageFormatter.check_limits(message)
             except Exception as e:
-                self.logger.exception(f'error checking content length limits for message: {e}\nRaw message: "{message}"')
+                self.logger.debug(f'error checking content length limits for message: {e}\nRaw message: "{message}"')
                 continue
             if not limits_ok:
                 self.logger.warning(f'[{self.name}] prepared message exceeded Discord length limits. Records will be discarded')
                 self.logger.debug(f'[{self.name}] message content:\n{message}')
                 to_be_sent = pending_records
                 continue
             try:
                 response = await self.session.post(self.hook_url, json=message)
                 text = await response.text()
-            except (OSError, asyncio.TimeoutError, aiohttp.ClientConnectionError) as e:
-                self.logger.warning(f'[{self.name}] error while sending message with Discord webhook: {e or type(e)}, saving for the next try')
+            except OSError as e:
+                self.logger.warning(f'[{self.name}] error while sending message with Discord webhook: {e}')
                 until_next_try = 60
                 continue  # implicitly saving messages in to_be_sent until the next try
             except Exception as e:
-                self.logger.exception(f'[{self.name}] error while sending message with Discord webhook: {e or type(e)}')
+                self.logger.exception(f'[{self.name}] error while sending message with Discord webhook: {e}')
                 self.logger.debug(f'raw message text:\n{message}')
-                to_be_sent = pending_records # discard unsent messages as they might have been the cause of error
+                to_be_sent = pending_records
                 until_next_try = 60
                 continue
             try:
                 response.raise_for_status()
             except aiohttp.ClientResponseError as e:
                 self.logger.warning(f'got {response.status} ({response.reason}) from {self.hook_url}')
                 if e.status == 400:
                     self.logger.warning(f'[{self.name}] message got rejected with {response.status} ({response.reason}), dropping it')
                     self.logger.debug(f'[{self.name}] response headers: {response.headers}')
                     self.logger.debug(f'[{self.name}] raw request body: {json.dumps(message)}')
                 elif e.status in  [404, 403]:
                     self.logger.warning(f'[{self.name}] got {e.status} from webhook, interrupting operations. Check if webhook url is still valid: {self.hook_url}')
                     break
             # if message got send successfully discard records except these that didn't fit into message
-            if len(pending_records) > 0:
-                self.logger.debug(f'carrying {len(pending_records)} pending records to the next loop')
             to_be_sent = pending_records
             until_next_try = self.get_next_delay(response.headers)
 
     def get_next_delay(self, headers: multidict.CIMultiDictProxy):
         if 'Retry-After' in headers:
             delay = headers.get('Retry-After', 0)
             self.logger.debug(f'Retry-After header is set to {delay}')
@@ -173,15 +164,15 @@
             TITLE = 256
             DESCRIPTION = 4096
             FOOTER_TEXT = 2048
 
         total_length = 0
         embeds = message.get('embeds', [])
         for embed in embeds:
-            author_name = len(embed.get('author', {}).get('name', '') or '')
+            author_name = len(embed.get('author', {}).get('name', ''))
             title = len(embed.get('title') or '')
             description = len(embed.get('description') or '')
             footer_text = len((embed.get('footer') or {}).get('text') or '')
             if author_name > Limits.AUTHOR_NAME:
                 return False
             if title > Limits.TITLE:
                 return False
@@ -198,15 +189,15 @@
 
 @Plugins.register('discord.hook', Plugins.kind.ACTOR_CONFIG)
 class DiscordHookConfig(ActorConfig):
     pass
 
 
 @Plugins.register('discord.hook', Plugins.kind.ACTOR_ENTITY)
-class DiscordHookEntity(ActionEntity):
+class DiscordHookEntity(ActorEntity):
     url: str
     """webhook url"""
     timezone: Optional[str] = None # https://en.wikipedia.org/wiki/List_of_tz_database_time_zones
     """takes timezone name from <https://en.wikipedia.org/wiki/List_of_tz_database_time_zones> (or OS settings if omitted), converts record fields containing date and time to this timezone"""
     hook: Optional[Any] = Field(exclude=True, default=None)
     """internal variable to persist state between update calls, holds DiscordWebhook object for this entity"""
 
@@ -215,15 +206,15 @@
     def check_timezone(cls, timezone: str) -> datetime.timezone:
         tz = dateutil.tz.gettz(timezone)
         if tz is None:
             raise ValueError(f'Unknown timezone: {timezone}')
         return tz
 
 @Plugins.register('discord.hook', Plugins.kind.ACTOR)
-class DiscordHook(Action):
+class DiscordHook(Actor):
     """
     Send record to Discord using webhook
 
     To generate webhook url follow instructions in "Making a Webhook" section of
     <https://support.discord.com/hc/en-us/articles/228383668-Intro-to-Webhooks>
 
     Some record types support rich formatting when sent to Discord, such as
@@ -244,12 +235,9 @@
 
     def handle(self, entity: DiscordHookEntity, record: Record):
         if entity.hook is None:
             return
         entity.hook.to_be_sent(record.as_timezone(entity.timezone))
 
     async def run(self):
-        tasks = []
-        for entity in self.entities.values():
-            task = asyncio.create_task(entity.hook.run(), name=f'{self.conf.name}:{entity.name}')
-            tasks.append(task)
-        await monitor_tasks(tasks)
+        tasks = [asyncio.create_task(entity.hook.run()) for entity in self.entities.values()]
+        await asyncio.wait(tasks)
```

### Comparing `avtdl-0.9.14.3/avtdl/plugins/execute/run_command.py` & `avtdl-0.9.9/avtdl/plugins/execute/run_command.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,30 +5,30 @@
 from pathlib import Path
 from typing import Dict, List, Optional, Sequence
 
 from pydantic import field_validator
 
 from avtdl.core import utils
 from avtdl.core.config import Plugins
-from avtdl.core.interfaces import Action, ActionEntity, ActorConfig, Event, EventType, Record
+from avtdl.core.interfaces import Actor, ActorConfig, ActorEntity, Event, EventType, Record
 from avtdl.core.utils import Fmt, check_dir, sanitize_filename
 
 Plugins.register('execute', Plugins.kind.ASSOCIATED_RECORD)(Event)
 
 
 @Plugins.register('execute', Plugins.kind.ACTOR_CONFIG)
 class CommandConfig(ActorConfig):
     pass
 
 @Plugins.register('execute', Plugins.kind.ACTOR_ENTITY)
-class CommandEntity(ActionEntity):
+class CommandEntity(ActorEntity):
     command: str
     """shell command to be executed on every received record. Supports placeholders that will be replaced with currently processed record fields values"""
     working_dir: Optional[Path] = None
-    """path to the directory where command will be executed. If not set current working directory is used. Supports templating with {...}"""
+    """path to the directory where command will be executed. If not set current working directory is used"""
     log_dir: Optional[Path] = None
     """write executed process output to a file in this directory if set. If it is not set, output will not be redirected to file"""
     log_filename: Optional[str] = None
     """filename to write executed process output to. If not defined, it is generated automatically based on command and entity name"""
     placeholders: Dict[str, str] = {'{url}': 'url', '{title}': 'title', '{text}': 'text'}
     """parts of `command` string that should be replaced with processed record fields, defined as mapping `'placeholder': 'record field name'`"""
     static_placeholders: Dict[str, str] = {}
@@ -38,34 +38,28 @@
     report_failed: bool = True
     """emit Event with type "error" if the subprocess returned non-zero exit code or raised exception"""
     report_finished: bool = False
     """emit Event with type "finished" if the subprocess returned zero as exit code"""
     report_started: bool = False
     """emit Event with type "started" before starting a subprocess"""
 
-    @field_validator('log_dir')
+    @field_validator('working_dir', 'log_dir')
     @classmethod
     def check_dir(cls, path: Optional[Path]):
         if path is None:
             return path
         ok = utils.check_dir(path)
         if ok:
             return path
         else:
             raise ValueError(f'check path "{path}" exists and is a writeable directory')
 
-    @field_validator('command')
-    @classmethod
-    def split_args(cls, command: str):
-        _ = shlex.split(command) # might raise ValueError
-        return command
-
 
 @Plugins.register('execute', Plugins.kind.ACTOR)
-class Command(Action):
+class Command(Actor):
     """
     Run pre-defined shell command
 
     Take `command` string, replace keywords provided in `placeholders` with corresponding fields
     of currently processed record. For example, if `command` is set to
 
         "yt-dlp {url}"`
@@ -77,19 +71,14 @@
         yt-dlp https://www.youtube.com/watch?v=L692Sxz3thw
 
     Note that placeholders do not have to be wrapped in `{}` and can, in fact, be any
     arbitrary text strings. However, placeholders are replaced by corresponding values
     one after another, so using piece of text that might come up in record field might
     produce unexpected results.
 
-    `command` string is not treated as raw shell command. Instead, it is split into list
-     of elements, where first element specifies the program executable, and the rest
-     specify the arguments. It is therefore not possible to use shell features such as pipes
-     or execute multiple commands in one line.
-
     Make sure the executable the command uses (`yt-dlp` in this case) is installed and
     can be run from the working directory by current user. It is advised to confirm that
     the command can be executed manually and it finishes without errors before automating it.
 
     For each entity, a separate working directory can be configured. Output is shown
     in the same window by default, but can be redirected to a file, with either static
     or autogenerated name.
@@ -124,16 +113,15 @@
             for placeholder, static_value in entity.static_placeholders.items():
                 new_arg = new_arg.replace(placeholder, static_value)
             for placeholder, field in entity.placeholders.items():
                 value = record_as_dict.get(field)
                 if value is not None:
                     new_arg = new_arg.replace(placeholder, value)
                 else:
-                    if placeholder in arg:
-                        self.logger.warning(f'[{entity.name}] configured placeholder "{field}" is not a field of {record.__class__.__name__} ({record!r}), resulting command is unlikely to be valid')
+                    self.logger.warning(f'[{entity.name}] configured placeholder "{field}" is not a field of {record.__class__.__name__} ({record!r}), resulting command is unlikely to be valid')
             new_args.append(new_arg)
         return new_args
 
     @staticmethod
     def shell_for(args: List[str]) -> str:
         return ' '.join(args)
 
@@ -141,31 +129,30 @@
         record_hash = record.hash()
         task_id = f'Task for {entity.name}: on record {record!r} ({record_hash}) executing "{command_line}"'
         return task_id
 
     def add(self, entity: CommandEntity, record: Record):
         args = self.args_for(entity, record)
         if entity.working_dir is None:
-            working_dir = Path.cwd()
-            self.logger.info(f'[{entity.name}] working directory is not specified, using current directory instead: {working_dir}')
+            entity.working_dir = Path.cwd()
+            self.logger.info(f'[{entity.name}] working directory is not specified, using current directory instead: {entity.working_dir}')
         else:
-            working_dir = Fmt.format_path(entity.working_dir, record)
-            ok = check_dir(working_dir)
+            ok = check_dir(entity.working_dir)
             if not ok:
-                self.logger.warning(f'[{entity.name}] check if working directory "{working_dir}" exists and is a writeable directory')
+                self.logger.warning(f'[{entity.name}] check if working directory "{entity.working_dir}" exists and is a writeable directory')
 
         command_line = self.shell_for(args)
         task_id = self._generate_task_id(entity, record, command_line)
         if task_id in self.running_commands:
             msg = f'[{entity.name}] command "{command_line}" for record {record!r} is already running, will not call again'
             self.logger.info(msg)
             return
         self.logger.debug(f'[{entity.name}] executing command "{command_line}" for record {record!r}')
-        task = self.run_subprocess(args, task_id, working_dir, entity, record)
-        self.running_commands[task_id] = asyncio.get_event_loop().create_task(task, name=f'{self.conf.name}:{entity.name}:{task_id}')
+        task = self.run_subprocess(args, task_id, entity, record)
+        self.running_commands[task_id] = asyncio.get_event_loop().create_task(task)
 
     def _get_output_file(self, entity: CommandEntity, record: Record, task_id: str) -> Optional[Path]:
         if entity.log_dir is None:
             return None
         ok = check_dir(entity.log_dir)
         if not ok:
             self.logger.warning(f'[{entity.name}] check if directory specified in "output_dir" value "{entity.log_dir}" exists and is a writeable directory')
@@ -177,34 +164,34 @@
             timestamp = datetime.datetime.now().strftime('%Y-%m-%d_%H-%M-%S.%f')
             command_pre_hash = sha1(task_id.encode())
             command_hash = command_pre_hash.hexdigest()
             filename = f'command_{entity.name}_{timestamp}_{command_hash[:6]}_stdout.log'
         filename = sanitize_filename(filename)
         return entity.log_dir / filename
 
-    async def run_subprocess(self, args: List[str], task_id: str, working_dir: Path, entity: CommandEntity, record: Record):
+    async def run_subprocess(self, args: List[str], task_id: str, entity: CommandEntity, record: Record):
         command_line = self.shell_for(args)
         self.logger.info(f'[{entity.name}] executing command {command_line}')
         if entity.report_started:
             event = Event(event_type=EventType.started, text=f'Running command: {command_line}')
             self.on_record(entity, event)
         stdout_path = self._get_output_file(entity, record, task_id)
         try:
             stdout = open(stdout_path, 'at') if stdout_path is not None else None
         except OSError as e:
-            self.logger.warning(f'[{entity.name}] failed to open file {stdout_path}: {e}. Command output will not be written')
+            self.logger.warning(f'[{entity.name}] failed to open file {stdout_path}, command output will not be written')
             stdout = None
         try:
             if stdout is None:
-                process = await asyncio.create_subprocess_exec(*args, cwd=working_dir)
+                process = await asyncio.create_subprocess_exec(*args, cwd=entity.working_dir)
             else:
                 with stdout:
-                    stdout.write(f'# [{self.conf.name}.{entity.name}] > {command_line}\n')
+                    stdout.write(f'# [{self.conf.name}.{entity.name}] > {entity.command}\n')
                     stdout.flush()
-                    process = await asyncio.create_subprocess_exec(*args, cwd=working_dir, stdout=stdout, stderr=asyncio.subprocess.STDOUT)
+                    process = await asyncio.create_subprocess_exec(*args, cwd=entity.working_dir, stdout=stdout, stderr=asyncio.subprocess.STDOUT)
         except Exception as e:
             self.logger.warning(f'[{entity.name}] failed to execute command "{command_line}": {e}')
             if entity.report_failed:
                 event = Event(event_type=EventType.error, text=f'[{entity.name}] failed to execute command: {command_line}')
                 self.on_record(entity, event)
             if entity.forward_failed:
                 self.on_record(entity, record)
```

### Comparing `avtdl-0.9.14.3/avtdl/plugins/fc2/fc2.py` & `avtdl-0.9.9/avtdl/plugins/fc2/fc2.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,19 @@
-import datetime
 import json
 from json import JSONDecodeError
 from textwrap import shorten
 from typing import Optional, Sequence
 
 import aiohttp
 import pydantic
 from pydantic import Field
 
 from avtdl.core.config import Plugins
 from avtdl.core.interfaces import ActorConfig, MAX_REPR_LEN, Record
 from avtdl.core.monitors import HttpTaskMonitor, HttpTaskMonitorEntity
-from avtdl.core.utils import Fmt, parse_timestamp_ms
 
 
 @Plugins.register('fc2', Plugins.kind.ASSOCIATED_RECORD)
 class FC2Record(Record):
     """Represents event of a stream going live on FC2"""
     name: str = ''
     """name of the config entity for this user"""
@@ -23,39 +21,35 @@
     """url of the user stream"""
     user_id: str
     """unique for the given user/channel part of the stream url"""
     title: str
     """stream title"""
     info: str
     """stream description"""
-    start: Optional[datetime.datetime]
-    """time of the stream start"""
-    start_timestamp: str
-    """UNIX timestamp of the stream start"""
+    start: str
+    """timestamp of the stream start"""
     avatar_url: str
     """link to the user's avatar"""
     login_only: bool
     """whether logging in is required to view current livestream"""
 
     def __str__(self):
-        since = '\nsince ' + Fmt.date(self.start) if self.start else ''
-        return f'{self.url}\n{self.title}{since}'
+        return f'{self.url}\n{self.title}'
 
     def __repr__(self):
         title = shorten(self.title, MAX_REPR_LEN)
-        return f'FC2Record(user_id={self.user_id}, start={self.start_timestamp}, title={title})'
+        return f'FC2Record(user_id={self.user_id}, start={self.start}, title={title})'
 
     def discord_embed(self) -> dict:
         return {
             'title': self.title,
             'description': self.url,
             'color': None,
             'author': {'name': self.name, 'url': self.url, 'icon_url': self.avatar_url},
-            'timestamp': self.start.isoformat() if self.start else None,
-            'footer': {'text': self.info},
+            'footer': self.info,
             'fields': []
         }
 
 
 @Plugins.register('fc2', Plugins.kind.ACTOR_CONFIG)
 class FC2MonitorConfig(ActorConfig):
     pass
@@ -97,19 +91,18 @@
         try:
             record = self.parse_metadata(data)
             if record is None:
                 return None
         except (KeyError, TypeError, JSONDecodeError, pydantic.ValidationError) as e:
             self.logger.warning(f'FC2Monitor for {entity.name}: failed to parse channel info. Raw response: {data}')
             return None
-        if record.start_timestamp == entity.latest_live_start:
+        if record.start == entity.latest_live_start:
             self.logger.debug(f'FC2Monitor for {entity.name}: user {entity.user_id} is live since {entity.latest_live_start}, but record was already created')
             return None
-        self.logger.debug(f'FC2Monitor for {entity.name}: user {entity.user_id} is live since {record.start_timestamp}, producing record')
-        entity.latest_live_start = record.start_timestamp
+        entity.latest_live_start = record.start
         record.name = entity.name
         return record
 
     async def get_metadata(self, entity: FC2MonitorEntity, session: aiohttp.ClientSession) -> Optional[str]:
         url = 'https://live.fc2.com/api/memberApi.php'
         data = {'channel': 1, 'streamid': entity.user_id}
         text = await self.request(url, entity, session, method='POST', data=data)
@@ -118,25 +111,23 @@
     @staticmethod
     def parse_metadata(raw_data: str) -> Optional[FC2Record]:
         data = json.loads(raw_data)
         data = data['data']['channel_data']
         is_live = data['is_publish']
         if not is_live:
             return None
-        start_timestamp = str(data['start'])
-        start = parse_timestamp_ms(start_timestamp)
+        start = str(data['start'])
         title = data['title']
         info = data['info']
         avatar_url = data['image']
         login_only = data['login_only']
 
         channel_id = str(data['channelid'])
         channel_url = f'https://live.fc2.com/{channel_id}/'
 
         return FC2Record(url=channel_url,
                          title=title,
                          user_id=channel_id,
-                         start_timestamp=start_timestamp,
                          start=start,
                          info=info,
                          avatar_url=avatar_url,
                          login_only=login_only)
```

### Comparing `avtdl-0.9.14.3/avtdl/plugins/file/text_file.py` & `avtdl-0.9.9/avtdl/plugins/file/text_file.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 
 import os
 from pathlib import Path
 from typing import List, Optional, Sequence
 
 from pydantic import Field, field_validator
 
+from avtdl.core import utils
 from avtdl.core.config import Plugins
-from avtdl.core.interfaces import Action, ActionEntity, ActorConfig, Event, EventType, Record, \
-    TextRecord
+from avtdl.core.interfaces import Actor, ActorConfig, ActorEntity, Event, EventType, Record, TextRecord
 from avtdl.core.monitors import HIGHEST_UPDATE_INTERVAL, TaskMonitor, TaskMonitorEntity
-from avtdl.core.utils import Fmt, OutputFormat, check_dir, read_file, sanitize_filename
+from avtdl.core.utils import Fmt, OutputFormat, read_file, sanitize_filename
 
 Plugins.register('from_file', Plugins.kind.ASSOCIATED_RECORD)(TextRecord)
 
 
 @Plugins.register('from_file', Plugins.kind.ACTOR_CONFIG)
 class FileMonitorConfig(ActorConfig):
     pass
@@ -31,28 +31,17 @@
     update_interval: float = 60
     """how often the monitored file should be checked, in seconds"""
     mtime: float = Field(exclude=True, default=-1)
     """internal variable to persist state between updates. Used to check if the file has changed"""
     base_update_interval: float = Field(exclude=True, default=60)
     """internal variable to persist state between updates. Used to restore configured update interval after delay on network request error"""
 
-    @field_validator('path')
-    @classmethod
-    def check_length(cls, path: Path) -> Path:
-        try:
-            if path.is_dir():
-                raise ValueError(f'path is a directory: "{path}"')
-            if path.exists():
-                with open(path, 'rb') as _:
-                    pass
-        except OSError as e:
-            raise ValueError(f'{e}')
-        return path
 
     def __post_init__(self):
+        self.path = Path(self.path)
         self.base_update_interval = self.update_interval
 
 
 @Plugins.register('from_file', Plugins.kind.ACTOR)
 class FileMonitor(TaskMonitor):
     """
     Monitor content of a text file
@@ -104,51 +93,58 @@
         if self.exists(entity):
             text = read_file(entity.path)
             if entity.split_lines:
                 lines = text.split('\n')
             else:
                 lines = [text]
             for line in lines:
-                text = line.strip()
-                if text:
-                    record = TextRecord(text=text)
-                    records.append(record)
+                record = TextRecord(text=line.strip())
+                records.append(record)
         return records
 
 
 Plugins.register('to_file', Plugins.kind.ASSOCIATED_RECORD)(Event)
 
 
 @Plugins.register('to_file', Plugins.kind.ACTOR_CONFIG)
 class FileActionConfig(ActorConfig):
     pass
 
 
 @Plugins.register('to_file', Plugins.kind.ACTOR_ENTITY)
-class FileActionEntity(ActionEntity):
+class FileActionEntity(ActorEntity):
     path: Optional[Path] = None
-    """directory where output file should be created. Default is current directory. Supports templating with {...}"""
+    """directory where output file should be created. Default is current directory"""
     filename: str
-    """name of the output file. Supports templating with {...}"""
+    """name of the output file. Supports templating with `{...}`"""
     encoding: Optional[str] = 'utf8'
     """output file encoding"""
     output_format: OutputFormat = Field(default=OutputFormat.str, description='one of `' + "`, `".join(OutputFormat.__members__) + '`')
     """should record be written in output file as plain text or json"""
     overwrite: bool = True
     """whether file should be overwritten in if it already exists"""
     append: bool = True
     """if true, new record will be written at the end of the file without overwriting already present lines"""
     prefix: str = ''
     """string that will be appended before the record text. Can be used to separate records from each other or for simple templating"""
     postfix: str = '\n'
     """string that will be appended after the record text"""
 
+    @field_validator('path')
+    @classmethod
+    def check_dir(cls, path: Optional[Path]) -> Path:
+        if path is None:
+            return Path.cwd()
+        if utils.check_dir(path):
+            return path
+        raise ValueError(f'check if provided path points to a writeable directory')
+
 
 @Plugins.register('to_file', Plugins.kind.ACTOR)
-class FileAction(Action):
+class FileAction(Actor):
     """
     Write record to a text file
 
     Takes a record coming from a Chain, converts it to text representation,
     and writes to a file in given directory. When a file already exists,
     new records can be appended to the end of the file or overwrite it.
 
@@ -173,25 +169,15 @@
 
     def handle(self, entity: FileActionEntity, record: Record):
         filename = Fmt.format(entity.filename, record)
         filename = sanitize_filename(filename)
         if entity.path is None:
             path = Path.cwd().joinpath(filename)
         else:
-            path = Fmt.format_path(entity.path, record)
-            ok = check_dir(path)
-            if not ok:
-                self.logger.warning(f'[{entity.name}] check "{path}" is a valid and writeable directory')
-                return
-            path = path.joinpath(filename)
-        try:
-            path.exists()
-        except OSError as e:
-            self.logger.warning(f'[{entity.name}] failed to process record: {e}')
-            return
+            path = Path(entity.path).joinpath(filename)
         if path.exists() and not entity.overwrite:
             self.logger.debug(f'[{entity.name}] file {path} already exists, not overwriting')
             return
         mode = 'at' if entity.append else 'wt'
         try:
             text = entity.prefix + Fmt.save_as(record, entity.output_format) + entity.postfix
             with open(path, mode, encoding=entity.encoding) as fp:
```

### Comparing `avtdl-0.9.14.3/avtdl/plugins/filters/filters.py` & `avtdl-0.9.9/avtdl/plugins/filters/filters.py`

 * *Files identical despite different names*

### Comparing `avtdl-0.9.14.3/avtdl/plugins/nitter/nitter.py` & `avtdl-0.9.9/avtdl/plugins/nitter/nitter.py`

 * *Files identical despite different names*

### Comparing `avtdl-0.9.14.3/avtdl/plugins/rss/generic_rss.py` & `avtdl-0.9.9/avtdl/plugins/rss/generic_rss.py`

 * *Files 4% similar despite different names*

```diff
@@ -179,9 +179,8 @@
             except KeyError as e:
                 self.logger.warning(f'rss parser failed to construct record from rss entry {entry}: missing  necessarily field {e}')
                 continue
             except ValidationError as e:
                 self.logger.warning(f'rss parser failed to construct record from rss entry {entry}: {e}')
                 continue
             records.append(record)
-        records = records[::-1]  # records are ordered from new to old in the feed, reorder in chronological order
         return records
```

### Comparing `avtdl-0.9.14.3/avtdl/plugins/twitcast/twitcast_monitor.py` & `avtdl-0.9.9/avtdl/plugins/twitcast/twitcast_monitor.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,34 +18,22 @@
     """unique id for the current livestream"""
     url: str
     """user (channel) url"""
     movie_url: str
     """current livestream url"""
     title: str
     """livestream title"""
-    thumbnail_url: str
-    """link to the stream thumbnail"""
 
     def __str__(self):
         return f'{self.url}\n{self.title} ({self.movie_id})'
 
     def __repr__(self):
         title = shorten(self.title, MAX_REPR_LEN)
         return f'TwitcastRecord(user_id={self.user_id}, movie_id={self.movie_id}, title="{title}")'
 
-    def discord_embed(self) -> dict:
-        return {
-            'title': self.movie_url,
-            'description': None,
-            'color': None,
-            'author': {'name': self.user_id, 'url': self.url},
-            'image': {'url': self.thumbnail_url},
-            'fields': []
-        }
-
 @Plugins.register('twitcast', Plugins.kind.ACTOR_ENTITY)
 class TwitcastMonitorEntity(HttpTaskMonitorEntity):
     user_id: str
     """user id that should be monitored"""
     update_interval: float = 60
     """how often the user will be checked for being live, in seconds"""
     adjust_update_interval: bool = Field(exclude=True, default=True)
@@ -88,22 +76,20 @@
         movie_id = await self.get_movie_id(entity, session)
         if movie_id is None:
             self.logger.warning(f'[{entity.name}] failed to get movie id, will report this record again if it was a temporary error, will never report new records if it is permanent')
             movie_id = 'movie id is unknown'
         if movie_id == entity.most_recent_movie:
             self.logger.debug(f'[{entity.name}] user {entity.user_id} is live with movie {entity.most_recent_movie}, but record was already created')
             return None
-        self.logger.debug(f'[{entity.name}] user {entity.user_id} is live with movie {movie_id}, producing record')
         entity.most_recent_movie = movie_id
 
-        channel_url = f'https://twitcasting.tv/{entity.user_id}'
+        channel_url = f'https://twitcasting.tv/{entity.user_id}/'
         movie_url = f'{channel_url}/movie/{movie_id}'
-        thumbnail_url = f'{channel_url}/thumb/{movie_id}'
         title = f'{entity.name} is live on Twitcasting'
-        record = TwitcastRecord(url=channel_url, user_id=entity.user_id, movie_id=movie_id, movie_url=movie_url, title=title, thumbnail_url=thumbnail_url)
+        record = TwitcastRecord(url=channel_url, user_id=entity.user_id, movie_id=movie_id, movie_url=movie_url, title=title)
         return record
 
     async def is_live(self, entity: TwitcastMonitorEntity, session: aiohttp.ClientSession) -> bool:
         url = f"https://twitcasting.tv/userajax.php?c=islive&u={entity.user_id}"
         text = await self.request(url, entity, session)
         if text is None:
             self.logger.warning(f'[{entity.name}] failed to check if channel {entity.user_id} is live')
```

### Comparing `avtdl-0.9.14.3/avtdl/plugins/twitch/twitch.py` & `avtdl-0.9.9/avtdl/plugins/twitch/twitch.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,12 @@
-import datetime
 import json
 from textwrap import shorten
 from typing import Optional, Sequence
 
 import aiohttp
-from dateutil import parser as dateutil_parser
 from pydantic import Field
 
 from avtdl.core.config import Plugins
 from avtdl.core.interfaces import ActorConfig, MAX_REPR_LEN, Record
 from avtdl.core.monitors import HttpTaskMonitor, HttpTaskMonitorEntity
 
 
@@ -17,39 +15,22 @@
     """Represents event of a user going live on Twitch"""
     url: str
     """channel url"""
     username: str
     """username value from configuration entity"""
     title: str
     """stream title"""
-    start: datetime.datetime
-    """timestamp of the stream start"""
-    avatar_url: str
-    """link to the user's avatar"""
-    game: Optional[str] = None
-    """game name, if present"""
 
     def __str__(self):
         return f'{self.url}\n{self.title}'
 
     def __repr__(self):
         title = shorten(self.title, MAX_REPR_LEN)
         return f'TwitchRecord(username={self.username}, title="{title}")'
 
-    def discord_embed(self) -> dict:
-        return {
-            'title': self.title,
-            'description': self.url,
-            'color': None,
-            'author': {'name': self.username, 'url': self.url, 'icon_url': self.avatar_url},
-            'timestamp': self.start.isoformat(),
-            'footer': {'text': self.game},
-            'fields': []
-        }
-
 
 @Plugins.register('twitch', Plugins.kind.ACTOR_ENTITY)
 class TwitchMonitorEntity(HttpTaskMonitorEntity):
     username: str
     """Twitch username of a monitored channel"""
     update_interval: int = 300
     """how often the user will be checked for being live, in seconds"""
@@ -75,37 +56,30 @@
         return [record] if record else []
 
     async def check_channel(self, entity: TwitchMonitorEntity, session: aiohttp.ClientSession) -> Optional[TwitchRecord]:
         response = await self._get_channel_status(entity, session)
         if response is None:
             return None
         try:
-            info = response[0]['data']['user']
-            avatar_url = info['profileImageURL']
-            title = info['lastBroadcast']['title']
-            stream_info = info['stream']
-            if stream_info is None:
-                self.logger.debug(f'[{entity.name}] user {entity.username} is not live')
-                return None
-            stream_id = stream_info['id']
-            start_text = stream_info['createdAt']
-            start = dateutil_parser.parse(start_text)
-            game_info = stream_info.get('game') or {}
-            game = game_info.get('name', None)
+            stream_info = response[0]['data']['user']['stream']
+            title = response[0]['data']['user']['lastBroadcast']['title']
+            stream_id = response[0]['data']['user']['lastBroadcast']['id']
         except (TypeError, IndexError, KeyError) as e:
             self.logger.debug(f'[{entity.name}] failed to parse response: {type(e)} {e}. Raw response: {response}')
             return None
+        if stream_info is None:
+            self.logger.debug(f'[{entity.name}] user {entity.username} is not live')
+            return None
         if stream_id == entity.most_recent_stream:
             self.logger.debug(f'[{entity.name}] user {entity.username} is live with stream {entity.most_recent_stream}, but record was already created')
             return None
-        self.logger.debug(f'[{entity.name}] user {entity.username} is live with stream {stream_id}, producing record')
         entity.most_recent_stream = stream_id
 
         channel_url = f'https://twitch.tv/{entity.username}/'
-        record = TwitchRecord(url=channel_url, username=entity.username, title=title, avatar_url=avatar_url, start=start, game=game)
+        record = TwitchRecord(url=channel_url, username=entity.username, title=title)
         return record
 
     @staticmethod
     def _prepare_body(username: str) -> str:
         body = [{
             'operationName': 'StreamMetadata',
             'variables': {'channelLogin': username},
```

### Comparing `avtdl-0.9.14.3/avtdl/plugins/url/url.py` & `avtdl-0.9.9/avtdl/plugins/url/url.py`

 * *Files identical despite different names*

### Comparing `avtdl-0.9.14.3/avtdl/plugins/xmpp/msg2jbr_aioxmpp.py` & `avtdl-0.9.9/avtdl/plugins/xmpp/msg2jbr_aioxmpp.py`

 * *Files identical despite different names*

### Comparing `avtdl-0.9.14.3/avtdl/plugins/xmpp/msg2jbr_slixmpp.py` & `avtdl-0.9.9/avtdl/plugins/xmpp/msg2jbr_slixmpp.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,82 +1,74 @@
 import asyncio
 import logging
 from dataclasses import dataclass
-from typing import Callable, Optional
+from typing import List, Optional
 
 import slixmpp
 
 ON_ERROR_RETRY_DELAY = 60
 DISCONNECT_AFTER_DONE_DELAY = 30
 
-
 @dataclass
 class Line:
     recipient: str
     message: str
 
-
 class MSG2JBR:
-    def __init__(self, username: str, passwd: str, logger: Optional[logging.Logger] = None):
+    def __init__(self, username, passwd, logger=None):
         self.user = username
         self.passwd = passwd
         self.logger = logger or logging.getLogger('msg2jbr')
         # JabberClient gets initialized in async run() instead of __init__
         # to make sure it uses same event loop as run() instead of making its own,
         # making it possible to await JabberClient.disconnected there
         self.jabber: Optional[JabberClient] = None
 
-    def to_be_send(self, recipient: str, message: str) -> None:
+    def to_be_send(self, recipient, message):
         if self.jabber is None:
             self.logger.debug(f'not running yet, message discarded: (to: {recipient}) "{message[:50]}"')
             return
         line = Line(recipient, message)
         self.jabber.send_query.put_nowait(line)
 
-    async def run(self) -> None:
+    async def run(self):
         self.jabber = JabberClient(self.user, self.passwd, self.logger.getChild('slixmpp'))
         while True:
             pending = self.jabber.send_query.qsize()
-            if pending > 0:
+            if  pending > 0:
                 self.logger.debug(f'connecting to send {pending} pending messages')
                 self.jabber.connect()
                 try:
                     await asyncio.wait_for(self.jabber.disconnected, DISCONNECT_AFTER_DONE_DELAY * 10)
                 except asyncio.TimeoutError:
-                    self.logger.warning(f'sending messages takes too long, aborting to retry later')
+                    logging.warning(f'sending messages takes too long, aborting wait to retry later')
                 else:
                     self.logger.debug(f'done sending messages, disconnected')
             if self.jabber.fatal_error is not None:
                 self.logger.warning(f'{self.jabber.fatal_error}, terminating')
                 break
             pending = self.jabber.send_query.qsize()
             if pending > 0:
                 self.logger.debug(f'{pending} messages left after disconnect, delaying next attempt')
                 await asyncio.sleep(ON_ERROR_RETRY_DELAY)
             await asyncio.sleep(1)
 
-
 class JabberClient(slixmpp.ClientXMPP):  # type: ignore
 
-    def __init__(self, username: str, passwd: str, logger: Optional[logging.Logger] = None) -> None:
+    def __init__(self, username, passwd, logger=None):
         super().__init__(username, passwd)
         self.logger = logger or logging.getLogger('slixmppClient')
         self.send_query: asyncio.Queue = asyncio.Queue()
         self.fatal_error: Optional[str] = None
         self.add_event_handler('session_start', self.send_pending)
         self.add_event_handler('failed_all_auth', self.on_bad_auth)
         self.add_error_handlers()
-        self.now_sending = False
 
-    async def send_pending(self, _) -> None:
+    async def send_pending(self, _):
         self.logger.debug('got session_start event')
-        if self.now_sending:
-            self.logger.warning(f'session_start handler got called but now_sending={self.now_sending}, aborting')
-            return
-        self.now_sending = True
         try:
             self.send_presence()
             await self.get_roster()
             while True:
                 line: Line = await asyncio.wait_for(self.send_query.get(), DISCONNECT_AFTER_DONE_DELAY)
                 recipient = slixmpp.JID(line.recipient)  # type: ignore
                 self.send_message(mto=recipient, mbody=line.message, mtype='chat')
@@ -84,29 +76,27 @@
                 if self.send_query.empty():
                     self.logger.debug('put all pending messages in internal queue, waiting a bit for new ones')
         except asyncio.TimeoutError:
             self.logger.debug('disconnecting')
             await self.disconnect()
         except Exception as e:
             self.logger.exception(f'got error while sending messages: {e}')
-        finally:
-            self.now_sending = False
 
-    def on_bad_auth(self, _) -> None:
+    def on_bad_auth(self, _):
         self.fatal_error = f'authentication failed for {self.boundjid.bare}'
 
-    def add_error_handlers(self) -> None:
+    def add_error_handlers(self):
         error_messages = {'connection_failed': 'failed to connect',
                           'reconnect_delay': 'next connection attempt in',
                           'stream_error': 'stream error',
                           'killed': 'XML stream got aborted',
                           'message_error': 'got error message from jabber server',
                           'message': 'got message',
                           }
         for event, message in error_messages.items():
             self.add_event_handler(event, self.make_error_handler(message))
 
-    def make_error_handler(self, message: str) -> Callable:
+    def make_error_handler(self, message):
         def error_handler(event):
             msg = f'{message}: {event}' if event else f'{message}'
             self.logger.debug(msg)
         return error_handler
```

### Comparing `avtdl-0.9.14.3/avtdl/plugins/xmpp/send_jabber.py` & `avtdl-0.9.9/avtdl/plugins/xmpp/send_jabber.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import logging
 from typing import Optional, Sequence
 
 import dateutil
 from pydantic import field_validator
 
 from avtdl.core.config import Plugins
-from avtdl.core.interfaces import Action, ActionEntity, ActorConfig, Record
+from avtdl.core.interfaces import Actor, ActorConfig, ActorEntity, Record
 
 try:
     from avtdl.plugins.xmpp.msg2jbr_slixmpp import MSG2JBR
 except ImportError:
     try:
         from avtdl.plugins.xmpp.msg2jbr_aioxmpp import MSG2JBR
     except ImportError:
@@ -18,35 +18,35 @@
         logging.error(msg)
         raise ImportError(msg, name=__name__)
 
 
 @Plugins.register('xmpp', Plugins.kind.ACTOR_CONFIG)
 class JabberConfig(ActorConfig):
     xmpp_username: str
-    """JID of the account to be used to send messages, including resource"""
+    """JID of the account to be used to send messages, resource included"""
     xmpp_pass: str
     """password of the account to be used to send messages"""
 
 @Plugins.register('xmpp', Plugins.kind.ACTOR_ENTITY)
-class JabberEntity(ActionEntity):
+class JabberEntity(ActorEntity):
     jid: str
     """JID to send message to"""
     timezone: Optional[str] = None
     """takes timezone name from <https://en.wikipedia.org/wiki/List_of_tz_database_time_zones> or OS settings if omitted, converts record fields containing date and time to this timezone"""
 
     @field_validator('timezone')
     @classmethod
     def check_timezone(cls, timezone: str) -> datetime.timezone:
         tz = dateutil.tz.gettz(timezone)
         if tz is None:
             raise ValueError(f'Unknown timezone: {timezone}')
         return tz
 
 @Plugins.register('xmpp', Plugins.kind.ACTOR)
-class SendJabber(Action):
+class SendJabber(Actor):
     """
     Send records as Jabber messages
 
     Converts records to a text representation and sends them as messages
     to specified recipients. Sends each record in a separate message,
     does not impose any limits on frequency or size of messages, leaving
     it to server side.
```

### Comparing `avtdl-0.9.14.3/avtdl/plugins/youtube/common.py` & `avtdl-0.9.9/avtdl/plugins/youtube/common.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,17 +10,16 @@
 from json import JSONDecodeError
 from typing import Any, Dict, List, Optional, Tuple, Union
 from urllib.parse import parse_qs, unquote, urlparse
 
 import aiohttp
 import lxml.html
 from jsonpath import JSONPath
-from pydantic import BaseModel
 
-from avtdl.core.utils import get_cookie_value, request, request_raw
+from avtdl.core.utils import request, request_raw
 
 
 def find_all(data: Union[dict, list], jsonpath: str, cache={}) -> list:
     if jsonpath not in cache:
         cache[jsonpath] = JSONPath(jsonpath)
     parser = cache[jsonpath]
     return parser.parse(data)
@@ -113,53 +112,45 @@
 
 def get_innertube_context(page: str) -> Optional[dict]:
     anchor = '"INNERTUBE_CONTEXT":'
     _, context = extract_keys(page, [], anchor)
     return context
 
 
-def get_session_index(page: dict) -> str:
-    session_index = find_one(page, '$..responseContext..sessionIndex')
-    session_index = '' if session_index is None else str(session_index)
-    return session_index
-
-
 def get_utc_offset() -> int:
     offset = datetime.datetime.now(datetime.timezone.utc).astimezone().utcoffset()
     if offset is None:
         # should never happen since astimezone() returns tz-aware object
         return 0
     return offset // datetime.timedelta(minutes=1)
 
 
-class NextPageContext(BaseModel):
-    """Values from first or current page required to request next continuation page"""
-    innertube_context: Optional[dict]
-    session_index: str
-    continuation_token: Optional[str] = None
+def get_cookie_value(jar: aiohttp.CookieJar, key: str) -> Optional[str]:
+    for morsel in jar:
+        if morsel.key == key:
+            return morsel.value
+    return None
 
 
 CLIENT_VERSION = '2.20231023.04.02'
 
-def prepare_next_page_request(innertube_context: Optional[dict], continuation_token, cookies=None, session_index: str = '') -> Tuple[str, dict, dict]:
+def prepare_next_page_request(innertube_context: dict, continuation_token, cookies=None) -> Tuple[str, dict, dict]:
     BROWSE_ENDPOINT = 'https://www.youtube.com/youtubei/v1/browse?key=AIzaSyAO_FJ2SlqU8Q4STEHLGCilw_Y9_11qcW8'
     cookies = cookies or {}
-    innertube_context = innertube_context or {}
 
+    session_index = find_one(innertube_context, '$..sessionIndex') or ''
     visitor_data = find_one(innertube_context, '$..visitorData') or ''
     client_version = find_one(innertube_context, '$..clientVersion') or CLIENT_VERSION
     hl = find_one(innertube_context, '$..hl') or 'en'
     timezone = find_one(innertube_context, '$..timeZone') or ''
-    original_url = find_one(innertube_context, '$.client.originalUrl') or 'https://youtube.com'
 
     headers = {
         'X-Goog-AuthUser': session_index,
         'X-Origin': 'https://www.youtube.com',
         'X-Youtube-Client-Name': '1',
-        'X-Youtube-Client-Version': client_version,
         'Content-Type': 'application/json'
     }
     sapisid = get_cookie_value(cookies, 'SAPISID')
     if sapisid is not None:
         headers['Authorization'] = get_auth_header(sapisid)
 
     post_body = {
@@ -169,15 +160,14 @@
                 'clientVersion': client_version,
                 'visitorData': visitor_data,
                 'hl': hl,
                 # only reason timeZone might be present is "PREF" cookie being set in cookies file
                 'timeZone': timezone,
                 # Disabled until it gets better testing:
                 # 'utcOffsetMinutes': get_utc_offset() if not timezone else ''
-                'originalUrl': original_url
             }
         },
         'continuation': continuation_token
     }
     return BROWSE_ENDPOINT, headers, post_body
```

### Comparing `avtdl-0.9.14.3/avtdl/plugins/youtube/community_info.py` & `avtdl-0.9.9/avtdl/plugins/youtube/community_info.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import List, Optional, Union
 
 from pydantic import BaseModel
 
-from avtdl.plugins.youtube.common import find_all, find_one, parse_navigation_endpoint, thumbnail_url
+from avtdl.plugins.youtube.common import find_all, find_one, parse_navigation_endpoint
 
 
 class CommunityPostInfo(BaseModel):
     channel_id: str
     post_id: str
     author: str
     avatar_url: Optional[str] = None
@@ -31,19 +31,15 @@
         sponsor_only = find_one(post_renderer, '$.sponsorsOnlyBadge') is not None
         published_text = find_one(post_renderer, '$.publishedTimeText..text')
 
         text_runs = find_one(post_renderer, '$.contentText.runs') or []
         full_text = render_full_text(text_runs)
 
         attachments = find_all(post_renderer, '$.backstageAttachment..backstageImageRenderer.image.thumbnails.[-1:].url')
-        attachments = [link.split('=', 1)[0] + '=s0?imgmax=0' if 'fcrop' in link else link for link in attachments]
         video_id = find_one(post_renderer, '$.backstageAttachment..videoRenderer.videoId')
-        video_thumbnail =  thumbnail_url(video_id) if video_id else find_one(post_renderer, '$.backstageAttachment..videoRenderer.thumbnail.url')
-        if video_thumbnail is not None:
-            attachments.append(video_thumbnail)
 
         post = CommunityPostInfo(
             author=author,
             channel_id=channel_id,
             post_id=post_id,
             avatar_url=avatar_url,
             vote_count=vote_count,
```

### Comparing `avtdl-0.9.14.3/avtdl/plugins/youtube/feed_info.py` & `avtdl-0.9.9/avtdl/plugins/youtube/feed_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,57 +1,53 @@
 import datetime
 import re
 from typing import Optional, Tuple
 
 from pydantic import BaseModel, Field, ValidationError, field_validator
 
-from avtdl.plugins.youtube.common import extract_keys, find_all, find_one, get_continuation_token, thumbnail_url
+from avtdl.plugins.youtube.common import extract_keys, find_all, find_one, get_continuation_token
 
 
 class VideoRendererInfo(BaseModel):
     video_id: str
     url: str
     title: str
     summary: Optional[str] = Field(repr=False)
     scheduled: Optional[datetime.datetime] = None
     author: Optional[str]
     avatar_url: Optional[str] = None
-    thumbnail_url: Optional[str] = None
     channel_link: Optional[str] = None
     channel_id: Optional[str] = None
     published_text: Optional[str]
     length: Optional[str]
 
     is_upcoming: bool
     is_live: bool
     is_member_only: bool
 
-
 def get_video_renderers(page: str, anchor: str = 'var ytInitialData = ') -> Tuple[list, Optional[str], dict]:
     keys = ['gridVideoRenderer', 'videoRenderer', 'playlistVideoRenderer', 'continuationEndpoint']
     items, data = extract_keys(page, keys, anchor)
     continuation_token = get_continuation_token(items.pop('continuationEndpoint', {}))
     renderers = []
     for item in items.values():
         renderers.extend(item)
     return renderers, continuation_token, data
 
-
 def parse_scheduled(timestamp: Optional[str]) -> Optional[datetime.datetime]:
     if timestamp is None:
         return None
     try:
         timestamp_value = float(timestamp)
     except ValueError:
         return None
     scheduled = datetime.datetime.fromtimestamp(timestamp_value, tz=datetime.timezone.utc)
     return scheduled
 
-
-def get_author_fallback(item: dict) -> Optional[str]:
+def get_author_fallback(item:dict) -> Optional[str]:
     full_text = find_one(item, '$.title.accessibility..label')
     title_part = find_one(item, '$.title.runs..text')
     views_part = find_one(item, '$.viewCountText.simpleText')
     views_part_fallback = re.search('\d+\D+$', full_text) if full_text else None
     if not all((full_text, title_part, views_part or views_part_fallback)):
         return None
     start = full_text.find(title_part)
@@ -62,26 +58,26 @@
         end = views_part_fallback.start()
     else:
         end = -1
 
     if -1 in [start, end]:
         return None
     try:
-        author_text = full_text[start + len(title_part): end].split(':')[1].strip()
+        author_text = full_text[start + len(title_part) : end].split(':')[1].strip()
     except (IndexError, AttributeError):
         return None
     return author_text
 
 
 class AuthorInfo(BaseModel):
     name: str
     channel: str
     channel_id: str
     avatar_url: Optional[str] = None
-
+    
     @field_validator('channel')
     @classmethod
     def add_prefix(cls, channel: str) -> str:
         if channel.startswith('/'):
             return 'https://www.youtube.com' + channel
         else:
             return channel
@@ -98,79 +94,72 @@
     avatar_url = find_one(video_render, '$.channelThumbnailSupportedRenderers..thumbnails.[::-1].url')
 
     try:
         return AuthorInfo(name=author, channel=channel_link, channel_id=channel_id, avatar_url=avatar_url)
     except ValidationError:
         return None
 
-
 def parse_owner_info(page: dict) -> Optional[AuthorInfo]:
     owner_info_data = find_one(page, '$.header.c4TabbedHeaderRenderer')
     if owner_info_data is None:
         return None
     author = find_one(owner_info_data, '$.title')
     channel_link = find_one(owner_info_data, '$.navigationEndpoint.browseEndpoint.canonicalBaseUrl')
     channel_id = find_one(owner_info_data, '$.channelId')
     avatar_url = find_one(owner_info_data, '$.avatar.thumbnails.[::-1].url')
     try:
         return AuthorInfo(name=author, channel=channel_link, channel_id=channel_id, avatar_url=avatar_url)
     except ValidationError:
         return None
 
-
-def parse_video_renderer(item: dict, owner_info: Optional[AuthorInfo], raise_on_error: bool = False) -> Optional[
-    VideoRendererInfo]:
+def parse_video_renderer(item: dict, owner_info: Optional[AuthorInfo], raise_on_error: bool = False) -> Optional[VideoRendererInfo]:
     video_id = item.get('videoId')
     url = f'https://www.youtube.com/watch?v={video_id}'
     title = find_one(item, '$.title..text,simpleText')
     summary = find_one(item, '$.descriptionSnippet..text')
-    thumbnail = thumbnail_url(str(video_id)) or None
-
+    
     author_info = parse_author(item) or owner_info
     if author_info is None:
-        author_name = get_author_fallback(item)
+        author_name = get_author_fallback(item) 
         channel_link = channel_id = avatar_url = None
     else:
         author_name = author_info.name
         channel_link = author_info.channel
         channel_id = author_info.channel_id
         avatar_url = author_info.avatar_url
 
     scheduled_timestamp = find_one(item, '$.upcomingEventData.startTime')
     scheduled = parse_scheduled(scheduled_timestamp)
     published_text = find_one(item, '$.publishedTimeText.simpleText')
-    length = find_one(item, '$.lengthText.simpleText') or find_one(item,
-                                                                   '$..thumbnailOverlayTimeStatusRenderer.simpleText')
+    length = find_one(item, '$.lengthText.simpleText') or find_one(item, '$..thumbnailOverlayTimeStatusRenderer.simpleText')
 
     badges = find_all(item, '$.badges..style')
     is_member_only = 'BADGE_STYLE_TYPE_MEMBERS_ONLY' in badges
     is_live = 'BADGE_STYLE_TYPE_LIVE_NOW' in badges
     is_upcoming = scheduled is not None
 
     try:
         info = VideoRendererInfo(video_id=video_id,
                                  url=url,
                                  title=title,
                                  summary=summary,
                                  scheduled=scheduled,
                                  author=author_name,
                                  avatar_url=avatar_url,
-                                 thumbnail_url=thumbnail,
                                  channel_link=channel_link,
                                  channel_id=channel_id,
                                  published_text=published_text,
                                  length=length,
                                  is_live=is_live,
                                  is_upcoming=is_upcoming,
                                  is_member_only=is_member_only)
         return info
     except ValidationError:
         if raise_on_error:
             raise
         return None
 
-
 def handle_page(page: str) -> list:
     items, continuation, data = get_video_renderers(page)
     owner_info = parse_owner_info(data)
     info = [parse_video_renderer(x, owner_info) for x in items]
-    return info
+    return info
```

### Comparing `avtdl-0.9.14.3/avtdl/plugins/youtube/video_info.py` & `avtdl-0.9.9/avtdl/plugins/youtube/video_info.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,30 +7,25 @@
 from typing import Any, Dict, List, Optional
 
 import aiohttp
 from pydantic import BaseModel, Field
 
 
 class LoginRequiredError(ValueError):
-    '''Raised when video page returns no data aside
-    from {'playability_status': 'LOGIN_REQUIRED'},
-    which usually indicated video being private'''
-
+    '''Raised when video page returns no data aside from {'playability_status': 'LOGIN_REQUIRED'}, which usually indicated video being private'''
 
 class VideoErrorError(ValueError):
     '''Raised when video page returns {'playability_status': 'ERROR'}'''
 
-
 class VideoFormat(BaseModel):
     itag: int
     url: str = Field(repr=False)
     mime: str
     quality: str
 
-
 class VideoInfo(BaseModel):
     url: str
     title: str
     published: str
     uploaded: str
     author: str
     channel_id: str
@@ -55,113 +50,104 @@
 
 
 def get_video_page(url: str) -> str:
     with urllib.request.urlopen(url, timeout=15) as resp:
         data = resp.read()
         return data.decode('utf8')
 
-
 async def aget_video_page(url: str, session: Optional[aiohttp.ClientSession] = None) -> str:
     if session is None:
         async with aiohttp.request('GET', url) as response:
             text = await response.text()
     else:
         async with session.get(url) as response:
             text = await response.text()
     return text
 
-
 def get_initial_player_response(page: str) -> dict:
     try:
         return get_initial_response_fast(page)
     except (ValueError, JSONDecodeError):
         return get_initial_response_slow(page)
 
-
 def get_initial_response_fast(page: str) -> dict:
     re_initial_data = 'var ytInitialPlayerResponse = ([^;]*);'
     match = re.search(re_initial_data, page)
     if match is None:
         raise ValueError(f'Failed to find ytInitialPlayerResponse on the page')
     raw_data = match.groups()[0]
     data = json.loads(raw_data)
     return data
 
-
 def get_initial_response_slow(page: str) -> dict:
     anchor = 'var ytInitialPlayerResponse = {'
     pos_start = page.find(anchor)
     if pos_start == -1:
         raise ValueError(f'Failed to find ytInitialPlayerResponse on the page')
     pos_start += len(anchor) - 1
     position = pos_start
 
     re_parenthesses = re.compile('[{}]')
     parenthesses_values = defaultdict(int, {'{': 1, '}': -1})
     parentheses = 0
     while True:
         parentheses += parenthesses_values[page[position]]
         if parentheses == 0:
-            raw_data = page[pos_start:position + 1]
+            raw_data = page[pos_start:position+1]
             response = json.loads(raw_data)
             return response
         position_match = re_parenthesses.search(page, position + 1)
         try:
             position = position_match.start()
         except AttributeError:
             raise ValueError(f'Failed to find matching set of parentheses after ytInitialPlayerResponse')
 
-
 def get_embedded_player_response(page: str) -> dict:
     pos_start = page.find('{"embedded_player_response"')
     if pos_start == -1:
         raise ValueError(f'Failed to find embedded_player_response on page')
     parentheses = 1
-    for position in range(pos_start + 1, len(page)):
+    for position in range(pos_start+1, len(page)):
         if page[position] == '{':
             parentheses += 1
         if page[position] == '}':
             parentheses -= 1
         if parentheses == 0:
-            raw_data = page[pos_start:position + 1]
+            raw_data = page[pos_start:position+1]
             response_data = json.loads(raw_data).get('embedded_player_response', '')
             response = json.loads(response_data)
             return response
     else:
         raise ValueError(f'Failed to find closing parenthesis for embedded_player_response')
 
-
 def rename_keys(input_dict: Dict[str, Any], key_mapping: Dict[str, str]) -> Dict[str, Any]:
     output_dict = {}
     for data_key, input_key in key_mapping.items():
         value = input_dict.get(input_key)
         if value is not None:
             output_dict[data_key] = value
     return output_dict
 
-
 def parse_playability_status(player_response: dict) -> Dict[str, Any]:
     playability_status = player_response.get('playabilityStatus')
     if playability_status is None:
         return {}
 
     info = rename_keys(playability_status, {'playability_status': 'status', 'playability_reason': 'reason'})
 
     try:
-        date = playability_status["liveStreamability"]["liveStreamabilityRenderer"]["offlineSlate"][
-            "liveStreamOfflineSlateRenderer"]["scheduledStartTime"]
+        date = playability_status["liveStreamability"]["liveStreamabilityRenderer"]["offlineSlate"]["liveStreamOfflineSlateRenderer"]["scheduledStartTime"]
         date = datetime.datetime.fromtimestamp(int(date), tz=datetime.timezone.utc)
     except (KeyError, TypeError, ValueError):
         pass
     else:
         info['scheduled'] = date
 
     return info
 
-
 def parse_video_details(player_response: dict) -> Dict[str, Any]:
     video_details = player_response.get('videoDetails')
     if video_details is None:
         return {}
     key_mapping = {
         'title': 'title',
         'author': 'author',
@@ -172,15 +158,14 @@
         'length': 'lengthSeconds',
         'is_livestream': 'isLiveContent',
     }
     info = rename_keys(video_details, key_mapping)
     info['is_upcoming'] = video_details.get('isUpcoming', False)
     return info
 
-
 def parse_microformat(player_response: dict) -> Dict[str, Any]:
     microformat = player_response.get('microformat', {}).get('playerMicroformatRenderer')
     if microformat is None:
         return {}
     key_mapping = {
         'published': 'publishDate',
         'uploaded': 'uploadDate',
@@ -195,30 +180,29 @@
     if microformat.get('description') is not None:
         info['summary'] = microformat.get('description', {}).get('simpleText')
     info['is_adult'] = not microformat.get('isFamilySafe')
     info['is_livestream'] = microformat.get('liveBroadcastDetails') is not None
 
     live_details = microformat.get('liveBroadcastDetails')
     if live_details is not None:
-        if live_details.get('endTimestamp') is not None:  # live ended
+        if live_details.get('endTimestamp') is not None: # live ended
             info['live_start'] = live_details.get('startTimestamp')
             info['live_end'] = live_details.get('endTimestamp')
-        elif live_details.get('isLiveNow') == True:  # live is live
+        elif live_details.get('isLiveNow') == True: # live is live
             info['live_start'] = live_details.get('startTimestamp')
-        else:  # live is scheduled
+        else: # live is scheduled
             date = live_details.get('startTimestamp')
             try:
                 date = datetime.datetime.fromisoformat(date)
                 info['scheduled'] = date
             except (ValueError, TypeError):
                 pass
 
     return info
 
-
 def parse_video_formats(player_response: dict) -> List[VideoFormat]:
     formats = player_response.get('streamingData')
     if formats is None:
         return []
     formats_list = []
     formats_list.extend(formats.get('formats', []))
     formats_list.extend(formats.get('adaptiveFormats', []))
@@ -240,29 +224,51 @@
     info = {}
     info.update(parse_video_details(player_response))
     info.update(parse_microformat(player_response))
     info.update(parse_playability_status(player_response))
     info['formats'] = parse_video_formats(player_response)
     return info
 
-
 def parse_video_page(page: str, url: str) -> VideoInfo:
     response = get_initial_player_response(page)
     data = parse_player_response(response)
     data['url'] = url
     if data['playability_status'] == 'LOGIN_REQUIRED' and data.get('playability_reason') is None:
         raise LoginRequiredError(f'Video is likely private: {url}. Raw data: {data}')
     if data['playability_status'] == 'ERROR':
         raise VideoErrorError(f'Video was deleted or never existed: {url} . Raw data: {data}')
     info = VideoInfo(**data)
     return info
 
-
 def get_video_info(url: str) -> VideoInfo:
     page = get_video_page(url)
     return parse_video_page(page, url)
 
-
 async def aget_video_info(url: str, session: Optional[aiohttp.ClientSession] = None) -> VideoInfo:
     page = await aget_video_page(url, session)
     return parse_video_page(page, url)
 
+if __name__ == '__main__':
+    from pprint import pprint
+    urls = {
+        'past live': 'https://www.youtube.com/watch?v=4edZ1YcVnhE',
+        'future live': 'https://www.youtube.com/watch?v=rKMhl43RHo0',
+        'ongoing live': 'https://www.youtube.com/watch?v=rUxyKA_-grg',
+        'adult': 'https://www.youtube.com/watch?v=0UcBpNS8-P4',
+        'premium': 'https://www.youtube.com/watch?v=sY1tXDR-oBg',
+        'member only': 'https://www.youtube.com/watch?v=mcZ6dN_wGc8',
+        'unlisted': 'https://www.youtube.com/live/IJXKVtb3xuU?si=o0gUYiYGoWW5_ukt',
+        'not a live vod': 'https://www.youtube.com/watch?v=SdF0vjVj278',
+        'privated': 'https://www.youtube.com/watch?v=w_ivzW_ya-U',
+        'nonexistant': 'https://www.youtube.com/watch?v=mamamama',
+    }
+    for name, url in urls.items():
+        try:
+            info = get_video_info(url)
+            info.summary = '0'
+            info.formats = []
+        except Exception as e:
+            print(f'[****** {name} ********]')
+            print(f'{e!r}')
+        else:
+            print(f'[****** {name} ********]')
+            pprint(info.model_dump())
```

### Comparing `avtdl-0.9.14.3/avtdl/plugins/youtube/youtube_chat.py` & `avtdl-0.9.9/avtdl/plugins/youtube/youtube_chat.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,136 +1,124 @@
 import datetime
 import json
 import logging
 from textwrap import shorten
-from typing import Callable, Dict, List, Optional, Sequence, Tuple, Union
+from typing import Callable, Dict, List, Optional, Sequence, Tuple
 
 import aiohttp
-from pydantic import Field
+from pydantic import BaseModel, Field
 
 from avtdl.core import utils
 from avtdl.core.interfaces import MAX_REPR_LEN, Record
 from avtdl.core.monitors import BaseFeedMonitor, BaseFeedMonitorConfig, BaseFeedMonitorEntity
 from avtdl.core.plugins import Plugins
-from avtdl.core.utils import Delay, Fmt, parse_timestamp_us
 from avtdl.plugins.youtube import video_info
-from avtdl.plugins.youtube.common import NextPageContext, extract_keys, find_all, find_one, get_innertube_context, \
-    get_session_index, handle_consent, \
+from avtdl.plugins.youtube.common import extract_keys, find_all, find_one, get_innertube_context, handle_consent, \
     parse_navigation_endpoint, prepare_next_page_request
 
 
 @Plugins.register('prechat', Plugins.kind.ASSOCIATED_RECORD)
 class YoutubeChatRecord(Record):
     """Youtube chat message"""
     author: str
     """message author's name"""
     channel: str
     """message author's channel url"""
     badges: List[str]
     """localized list of message author's badges (owner, moderator, member, verified and so on)"""
-    timestamp: Union[datetime.datetime, int, None]
-    """timestamp of when the message was sent"""
+    timestamp: int
+    """timestamp (UNIX time) of when the message was sent"""
     text: Optional[str] = None
     """message content as plaintext"""
     amount: Optional[str] = None
     """for superchats, string specifying amount and currency, otherwise empty"""
     banner_header: Optional[str] = None
     """used for special objects in chat, such as pinned messages"""
     message_header: Optional[str] = None
     sticker: Optional[str] = None
     """supersticker name if the message is a supersticker, otherwise empty"""
-    color: Optional[int] = None
-    """message header color (RGB integer), if present"""
-
-    video_id: str = ''
-    """video_id of the video chat message was sent to"""
-    video_title: str = ''
-    """title of the video chat message was sent to"""
-    video_author: str = ''
-    """name of the channel where the video chat message was sent to is published"""
 
     uid: str
     """unique id of the message"""
     action: str
     """internal name of message type. Used for debug purposes"""
     renderer: str
     """internal name of message format. Used for debug purposes"""
 
+
     def _main_text(self) -> str:
         items = []
         if self.banner_header:
             items.append(f'{self.banner_header}:')
         if self.amount:
             items.append(f'{self.amount}:')
-        items.append(self._body_text())
+        items.extend(self._body_text())
         text = ' '.join(items)
         return text
 
-    def _body_text(self) -> str:
+    def _body_text(self):
         items = []
         if self.sticker:
             items.append(self.sticker)
         if self.message_header:
             items.append(self.message_header)
         if self.text:
             items.append(self.text)
         text = ' '.join(items)
         return text
 
+    def parse_timestamp(self) -> Optional[datetime.datetime]:
+        try:
+            ts = int(self.timestamp)
+            dt = datetime.datetime.fromtimestamp(int(ts/1000000), tz=datetime.timezone.utc)
+            return dt
+        except Exception:
+            return None
+
     def __str__(self):
-        timestamp = Fmt.date(self.timestamp)
-        badges = ', '.join(self.badges) if self.badges else ''
         text = self._main_text()
-        return f'{timestamp} {badges} [{self.author}] {text}'
+        return f'[{self.author}] {text}'
 
     def __repr__(self):
         text = shorten(self._main_text(), MAX_REPR_LEN)
         return f'[{self.action}: {self.renderer}] [{self.author}] {text}'
 
     def discord_embed(self) -> List[dict]:
-        dt = self.timestamp if isinstance(self.timestamp, datetime.datetime) else parse_timestamp_us(self.timestamp)
+        dt = self.parse_timestamp()
         timestamp = dt.isoformat() if dt is not None else None
         author = self.author
         if self.badges:
             author += ' [{}]'.format(', '.join(self.badges))
         if self.amount:
             author += f' [{self.amount}]'
         embed = {
             'title': self.banner_header,
             'description': self._body_text(),
             'url': None,
-            'color': self.color,
+            'color': None,
             'timestamp': timestamp,
             'author': {'name': author, 'url': self.channel},
             'fields': []
         }
         return [embed]
 
-
-class ChatPageContext(NextPageContext):
+class Context(BaseModel):
     innertube_context: Optional[dict] = None
-    session_index: str = ''
-    continuation_token: Optional[str] = None
-    is_replay: Optional[bool] = None
     continuation_url: Optional[str] = None
+    continuation_token: Optional[str] = None
     base_update_interval: float = 120
+    is_replay: Optional[bool] = None
     done: bool = False
-    video_author: str = ''
-    video_title: str = ''
-    video_id: str = ''
 
 @Plugins.register('prechat', Plugins.kind.ACTOR_ENTITY)
 class YoutubeChatMonitorEntity(BaseFeedMonitorEntity):
     url: str
-    """url of a video frame with a chat"""
-    update_interval: float = Field(exclude=True, default=20)
-    """unavailable for configuration since update interval is determined dynamically based on chat speed"""
+    update_interval: float = 20
     adjust_update_interval: bool = Field(exclude=True, default=False)
-    """unavailable for configuration since update interval is determined dynamically based on chat speed"""
-    context: ChatPageContext = Field(exclude=True, default=ChatPageContext())
+    context: Context = Field(exclude=True, default=Context())
 
 
 @Plugins.register('prechat', Plugins.kind.ACTOR_CONFIG)
 class YoutubeChatMonitorConfig(BaseFeedMonitorConfig):
     pass
 
 
@@ -148,93 +136,81 @@
     Some features, such as polls, are not supported.
     """
 
     def get_record_id(self, record: YoutubeChatRecord) -> str:
        return record.uid
 
     async def get_records(self, entity: YoutubeChatMonitorEntity, session: aiohttp.ClientSession) -> Sequence[YoutubeChatRecord]:
+        first_time = False
         if entity.context.done:
             return []
+        actions = {}
         if entity.context.continuation_token is None:
-            actions = await self._get_first(entity, session)
-            if actions:
-                self.logger.warning(f'[{entity.name}] got chat messages on the first update, this is not supposed to happen. Raw data: {actions}')
-        # _get_first(...) sets value of entity.context.continuation_token unless error happened
-        if entity.context.continuation_token is None:
-            return []
-
-        new_actions = await self._get_next(entity, session)
-        if new_actions is None:
-            records = []
-            new_update_interval = Delay.get_next(entity.update_interval)
-        else:
-            records = Parser().run_parsers(new_actions)
-            for record in records:
-                record.video_id = entity.context.video_id
-                record.video_author = entity.context.video_author
-                record.video_title = entity.context.video_title
+            actions.update(await self._get_first(entity, session))
+            first_time = True
+        if entity.context.continuation_token is not None:
+            actions.update(await self._get_next(entity, session))
+        records = Parser().run_parsers(actions)
+        if not first_time:
             new_update_interval = self._new_update_interval(entity, len(records))
-        # entity.update_interval gets updated by self.request()
-        # which doesn't expect anyone else to touch it
-        # in order to work together with it entity.base_update_interval
-        # is overwritten with current update interval, while original value
-        # is stored in entity.context.base_update_interval
-        entity.base_update_interval = entity.update_interval = new_update_interval
+            # if new_update_interval != entity.update_interval:
+            #     self.logger.debug(f'[{entity.name}] update interval changed from {entity.update_interval} to {new_update_interval}')
+            # entity.update_interval gets updated by self.request()
+            # which doesn't expect anyone else to touch it
+            # in order to work together with it entity.base_update_interval
+            # is overwritten with current update interval, while original value
+            # is stored in entity.context.base_update_interval
+            entity.base_update_interval = entity.update_interval = new_update_interval
         return records
 
     async def _get_first(self, entity: YoutubeChatMonitorEntity, session: aiohttp.ClientSession) -> Dict[str, list]:
         raw_page_text = await self.request(entity.url, entity, session)
         if raw_page_text is None:
             return {}
         raw_page_text = await handle_consent(raw_page_text, entity.url, session, self.logger)
         try:
             info = video_info.parse_video_page(raw_page_text, entity.url)
         except Exception as e:
             self.logger.warning(f'[{entity.name}] error parsing page {entity.url}: {e}')
             return {}
-        actions, continuation, initial_page = self._get_actions(raw_page_text, first_page=True)
-
-        innertube_context = get_innertube_context(raw_page_text)
-        session_index = get_session_index(initial_page)
-        entity.context = ChatPageContext(innertube_context=innertube_context, session_index=session_index, continuation_token=continuation)
         entity.context.is_replay = not (info.is_upcoming or (info.live_start is not None and info.live_end is None))
         entity.context.continuation_url = self._get_continuation_url(entity.context.is_replay)
+        actions, continuation, initial_data = self._get_actions(raw_page_text, first_page=True)
+        innertube_context = get_innertube_context(raw_page_text)
+        entity.context.innertube_context = innertube_context
+        entity.context.continuation_token = continuation
 
-        entity.context.video_id = info.video_id
-        entity.context.video_title = info.title
-        entity.context.video_author = info.author
-
-        message = find_one(initial_page, '$..conversationBar.conversationBarRenderer.availabilityMessage.messageRenderer.text')
+        message = find_one(initial_data, '$..conversationBar.conversationBarRenderer.availabilityMessage.messageRenderer.text')
         if message is not None:
             text = Parser.runs_to_text(message)
-            self.logger.info(f'[{entity.name}] {text}')
+            self.logger.debug(f'[{entity.name}] {text}')
 
         if continuation is None:
             self.logger.warning(f'[{entity.name}] first page has no continuation token. Video has no chat or an error occured while loading it')
             entity.context.done = True
         return actions
 
-    async def _get_next(self, entity: YoutubeChatMonitorEntity, session: aiohttp.ClientSession) -> Optional[Dict[str, list]]:
+    async def _get_next(self, entity: YoutubeChatMonitorEntity, session: aiohttp.ClientSession) -> Dict[str, list]:
         if entity.context.innertube_context is None:
             self.logger.warning(f'[{entity}] continuation token is present in an absence of initial data. This is a bug')
-            return None
+            return {}
         if entity.context.continuation_url is None:
             self.logger.warning(f'[{entity}] continuation token is present in an absence of continuation url. This is a bug')
-            return None
+            return {}
         _, headers, post_body = prepare_next_page_request(entity.context.innertube_context, entity.context.continuation_token)
         page = await utils.request(entity.context.continuation_url, session, self.logger, method='POST', headers=headers,
                                    data=json.dumps(post_body), retry_times=3, retry_multiplier=2,
                                    retry_delay=5)
         if page is None:
             entity.context.continuation_token = None
             self.logger.warning(f'[{entity.name}] downloading chat continuation for {entity.url} failed')
             if entity.context.is_replay:
                 entity.context.done = True
                 self.logger.info(f'[{entity.name}] giving up on downloading chat replay for {entity.url}')
-            return None
+            return {}
         actions, continuation, _ = self._get_actions(page)
         entity.context.continuation_token = continuation
         if continuation is None and entity.context.is_replay:
             self.logger.info(f'[{entity.name}] finished downloading chat replay')
             entity.context.done = True
         return actions
 
@@ -248,14 +224,15 @@
             self.logger.debug(f'[{entity.name}] speed: {new_records}/{entity.update_interval:.2f}={speed:.2f}, from {entity.update_interval:.2f} to {new_update_interval:.2f}')
             if new_update_interval < 60:
                 return new_update_interval
         return min(entity.update_interval * 1.2, entity.context.base_update_interval)
 
     def _get_continuation_url(self, replay: bool) -> str:
         if replay:
+            # loading chat replay is not implemented yet though
             return 'https://www.youtube.com/youtubei/v1/live_chat/get_live_chat_replay?key=AIzaSyAO_FJ2SlqU8Q4STEHLGCilw_Y9_11qcW8&prettyPrint=false'
         else:
             return 'https://www.youtube.com/youtubei/v1/live_chat/get_live_chat?key=AIzaSyAO_FJ2SlqU8Q4STEHLGCilw_Y9_11qcW8&prettyPrint=false'
 
     def _get_actions(self, page: str, first_page=False) -> Tuple[Dict[str, list], Optional[str], dict]:
         keys = list(Parser.known_actions)
         anchor = 'var ytInitialData = ' if first_page else ''
@@ -309,48 +286,38 @@
 
             text = run.get('text')
             if text is not None:
                 parts.append(text)
         message = ''.join(parts)
         return message
 
-    @classmethod
-    def parse_color(cls, color: int) -> Optional[int]:
-        """Take color as 0xAARRGGBB and return it as 0xRRGGBB"""
-        if not isinstance(color, int):
-            return None
-        return color & 0xFFFFFF
-
     def parse_chat_renderer(self, action_type: str, renderer_type: str, renderer: dict) -> YoutubeChatRecord:
         uid = renderer.get('id')
 
         text = self.runs_to_text(renderer.get('message', {}))
         author = renderer.get('authorName', {}).get('simpleText', '[no author]')
         channel_id = renderer.get('authorExternalChannelId') or find_one(renderer, '$..authorExternalChannelId')
         channel = f'https://www.youtube.com/channel/{channel_id}'
-        timestamp = renderer.get('timestampUsec') 
-        timestamp = parse_timestamp_us(timestamp)
+        timestamp = renderer.get('timestampUsec')
         badges = renderer.get('authorBadges', []) and find_all(renderer['authorBadges'], '$..label')
         amount = renderer.get('purchaseAmountText', {}).get('simpleText')
         header = renderer.get('headerSubtext')
         header_text = self.runs_to_text(header) if header else None
         sticker = find_one(renderer, '$.sticker.accessibility..label')
-        color = self.parse_color(find_one(renderer, '$.headerBackgroundColor,backgroundColor'))
         record = YoutubeChatRecord(uid=uid,
                                     action=action_type,
                                     renderer=renderer_type,
                                     author=author,
                                     channel=channel,
                                     timestamp=timestamp,
                                     badges=badges,
                                     text=text,
                                     amount=amount,
                                     message_header=header_text,
-                                    sticker=sticker,
-                                    color=color
+                                    sticker=sticker
                     )
         return record
 
     def parse_banner(self, action_type: str, renderer_type: str, renderer: dict) -> YoutubeChatRecord:
         header = find_one(renderer, '$..liveChatBannerHeaderRenderer.text') or {}
         header_text = self.runs_to_text(header)
         message = find_one(renderer, '$..liveChatTextMessageRenderer')
@@ -361,15 +328,14 @@
         return record
 
     def parse_gift_purchase(self, action_type: str, renderer_type: str, renderer: dict) -> YoutubeChatRecord:
         uid = renderer.get('id')
         channel_id = find_one(renderer, '$..authorExternalChannelId')
         channel = f'https://www.youtube.com/channel/{channel_id}'
         timestamp = renderer.get('timestampUsec')
-        timestamp = parse_timestamp_us(timestamp)
 
         author = find_one(renderer, '$..authorName.simpleText') or '[no author]'
         badges = find_all(renderer, '$..authorBadges..label')
         header = find_one(renderer, '$.primaryText')
         header_text = self.runs_to_text(header) if header else None
         record = YoutubeChatRecord(uid=uid,
                                    action=action_type,
```

### Comparing `avtdl-0.9.14.3/avtdl/plugins/youtube/youtube_community.py` & `avtdl-0.9.9/avtdl/plugins/youtube/youtube_community.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import json
-from typing import List, Optional, Sequence, Tuple, Union
+from typing import Any, List, Optional, Sequence, Tuple, Union
 
 import aiohttp
 
 from avtdl.core import utils
 from avtdl.core.interfaces import MAX_REPR_LEN, Record
 from avtdl.core.monitors import PagedFeedMonitor, PagedFeedMonitorConfig, PagedFeedMonitorEntity
 from avtdl.core.plugins import Plugins
-from avtdl.plugins.youtube.common import NextPageContext, get_continuation_token, get_initial_data, get_innertube_context, get_session_index, handle_consent, prepare_next_page_request, thumbnail_url, \
+from avtdl.plugins.youtube.common import get_continuation_token, get_initial_data, get_innertube_context, handle_consent, prepare_next_page_request, thumbnail_url, \
     video_url
 from avtdl.plugins.youtube.community_info import CommunityPostInfo, SharedCommunityPostInfo, get_posts_renderers, get_renderers, get_shared_posts_renderers
 
 
 @Plugins.register('community', Plugins.kind.ASSOCIATED_RECORD)
 class CommunityPostRecord(Record, CommunityPostInfo):
     """Youtube community post content"""
@@ -162,49 +162,46 @@
     - `https://www.youtube.com/@ChannelName/community`
     - `https://www.youtube.com/channel/UCK0V3b23uJyU4N8eR_BR0QA/community`
     """
 
     def get_record_id(self, record: CommunityPostRecord) -> str:
         return f'{record.channel_id}:{record.post_id}'
 
-    async def handle_first_page(self, entity: PagedFeedMonitorEntity, session: aiohttp.ClientSession) -> Tuple[Optional[Sequence[Record]], Optional[NextPageContext]]:
+    async def handle_first_page(self, entity: PagedFeedMonitorEntity, session: aiohttp.ClientSession) -> Tuple[Optional[Sequence[Record]], Optional[Any]]:
         raw_page_text = await self.request(entity.url, entity, session)
         if raw_page_text is None:
             return None, None
         raw_page_text = await handle_consent(raw_page_text, entity.url, session, self.logger)
         try:
             initial_page = get_initial_data(raw_page_text)
         except Exception as e:
             self.logger.exception(f'[{entity.name}] failed to get initial data from {entity.url}: {e}')
             return None, None
         records = self._parse_entries(initial_page)
-
         continuation_token = get_continuation_token(initial_page)
         innertube_context = get_innertube_context(raw_page_text)
-        session_index = get_session_index(initial_page)
-        ctx = NextPageContext(innertube_context=innertube_context, session_index=session_index, continuation_token=continuation_token)
 
-        return records, ctx
+        return records, (innertube_context, continuation_token)
 
-    async def handle_next_page(self, entity: PagedFeedMonitorEntity, session: aiohttp.ClientSession, context: Optional[NextPageContext]) -> Tuple[Optional[Sequence[Record]], Optional[NextPageContext]]:
-        if context is None or context.continuation_token is None:
+    async def handle_next_page(self, entity: PagedFeedMonitorEntity, session: aiohttp.ClientSession, context: Optional[Any]) -> Tuple[Optional[Sequence[Record]], Optional[Any]]:
+        innertube_context, continuation_token = context  # type: ignore
+        if continuation_token is None:
             self.logger.debug(f'[{entity.name}] no continuation for next page, done loading')
             return [], None
 
-        url, headers, post_body = prepare_next_page_request(context.innertube_context, context.continuation_token, session.cookie_jar, context.session_index)
+        url, headers, post_body = prepare_next_page_request(innertube_context, continuation_token, cookies=session.cookie_jar)
         current_page = await utils.request_json(url, session, self.logger, method='POST', headers=headers,
                                                 data=json.dumps(post_body), retry_times=3, retry_multiplier=2,
                                                 retry_delay=5)
         if current_page is None:
             self.logger.debug(f'[{entity.name}] failed to load next page, aborting')
             return None, None
         current_page_records = self._parse_entries(current_page) or []
-        context.continuation_token = get_continuation_token(current_page)
-        if context.continuation_token is None:
-            context = None
+        continuation_token = get_continuation_token(current_page)
+        context = (innertube_context, continuation_token) if continuation_token else None
         return current_page_records, context
 
     def _parse_entries(self, page: dict) -> List[Union[CommunityPostRecord, SharedCommunityPostRecord]]:
         renderers = get_renderers(page)
         records: List[Union[CommunityPostRecord, SharedCommunityPostRecord]] = []
         post_renderers = get_posts_renderers(renderers)
         for item in post_renderers:
```

### Comparing `avtdl-0.9.14.3/avtdl/plugins/youtube/youtube_feed.py` & `avtdl-0.9.9/avtdl/plugins/youtube/youtube_feed.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 import datetime
 import json
 from json import JSONDecodeError
-from typing import List, Optional, Sequence, Tuple
+from typing import Any, List, Optional, Sequence, Tuple
 
 import aiohttp
 from pydantic import Field, ValidationError
 
 from avtdl.core import utils
 from avtdl.core.interfaces import Filter, FilterEntity, Record
 from avtdl.core.monitors import PagedFeedMonitor, PagedFeedMonitorConfig, PagedFeedMonitorEntity
 from avtdl.core.plugins import Plugins
 from avtdl.plugins.filters.filters import EmptyFilterConfig
-from avtdl.plugins.youtube.common import NextPageContext, get_innertube_context, get_session_index, handle_consent, \
-    prepare_next_page_request
-from avtdl.plugins.youtube.feed_info import AuthorInfo, VideoRendererInfo, get_video_renderers, parse_owner_info, \
-    parse_video_renderer
+from avtdl.plugins.youtube.common import get_innertube_context, handle_consent, prepare_next_page_request, thumbnail_url
+from avtdl.plugins.youtube.feed_info import AuthorInfo, VideoRendererInfo, get_video_renderers, parse_owner_info, parse_video_renderer
 
 
 @Plugins.register('channel', Plugins.kind.ASSOCIATED_RECORD)
 @Plugins.register('filter.channel', Plugins.kind.ASSOCIATED_RECORD)
 class YoutubeVideoRecord(VideoRendererInfo, Record):
     """
     Youtube video or livestream listed among others on Youtube page
@@ -37,16 +35,14 @@
     """snippet of the video description. Not always available"""
     scheduled: Optional[datetime.datetime] = None
     """scheduled date for upcoming stream or premiere"""
     author: Optional[str]
     """channel name"""
     avatar_url: Optional[str] = None
     """link to the avatar of the channel. Not always available"""
-    thumbnail_url: Optional[str] = None
-    """link to the video thumbnail"""
     channel_link: Optional[str] = None
     """link to the channel uploading the video"""
     channel_id: Optional[str] = None
     """channel ID in old format (such as `UCK0V3b23uJyU4N8eR_BR0QA`)"""
     published_text: Optional[str]
     """localized text saying how long ago the video was uploaded"""
     length: Optional[str]
@@ -56,69 +52,58 @@
     """indicates that video is an upcoming livestream or premiere"""
     is_live: bool
     """indicates that the video is a livestream or premiere that is currently live"""
     is_member_only: bool
     """indicated that the video is limited to members of the channel. Note that the video status might be changed at any time"""
 
     def __str__(self):
-        last_line = ''
         scheduled = self.scheduled
         if scheduled:
-            last_line = '\nscheduled to {}'.format(scheduled.strftime('%Y-%m-%d %H:%M'))
-        elif self.is_live:
-            last_line = '\n[Live]'
-        if self.is_member_only:
-            last_line += ' [Member only]'
+            scheduled_time = '\nscheduled to {}'.format(scheduled.strftime('%Y-%m-%d %H:%M'))
+        else:
+            scheduled_time = ''
         template = '{}\n{}\npublished by {}'
-        return template.format(self.url, self.title, self.author) + last_line
+        return template.format(self.url, self.title, self.author) + scheduled_time
 
     def __repr__(self):
         template = '{:<8} [{}] {}'
         return template.format(self.author or 'Unknown author', self.video_id, self.title[:60])
 
     def discord_embed(self) -> dict:
         embed = {
             'title': self.title,
             # 'description': ,
             'url': self.url,
             'color': None,
             'author': {'name': self.author, 'url': self.channel_link, 'icon_url': self.avatar_url},
-            'image': {'url': self.thumbnail_url},
+            'image': {'url': thumbnail_url(self.video_id)},
             'fields': []
         }
         footer = ''
         if self.published_text:
             footer += self.published_text
         if self.length:
             embed['fields'].append({'name': f'[{self.length}]', 'value': '', 'inline': True})
         if self.scheduled is not None:
             scheduled = self.scheduled.strftime('%Y-%m-%d %H:%M')
             embed['fields'].append({'name': 'Scheduled:', 'value': scheduled, 'inline': True})
-        if self.is_live:
-            embed['fields'].append({'name': '[Live]', 'value': '', 'inline': True})
-        if self.is_member_only:
-            embed['fields'].append({'name': '[Member only]', 'value': '', 'inline': True})
         embed['footer'] = {'text': footer}
         return embed
 
 
 @Plugins.register('channel', Plugins.kind.ACTOR_CONFIG)
 class VideosMonitorConfig(PagedFeedMonitorConfig):
     pass
 
 
 @Plugins.register('channel', Plugins.kind.ACTOR_ENTITY)
 class VideosMonitorEntity(PagedFeedMonitorEntity):
     update_interval: float = 1800
 
 
-class FeedPageContext(NextPageContext):
-    owner_info: Optional[AuthorInfo]
-
-
 @Plugins.register('channel', Plugins.kind.ACTOR)
 class VideosMonitor(PagedFeedMonitor):
     """
     Youtube channel monitor
 
     Monitors Youtube url listing videos, such as channels main page,
     videos and streams tab of a channel, as well as playlists, and,
@@ -141,96 +126,72 @@
     Unlike `rss` monitor, with login cookies it can see videos and streams
     with limited access (such as member-only).
 
     While monitoring a single channel is less efficient, using this monitor with
     subscriptions feed url on a dedicated account is a recommended way
     to monitor a high amount (hundreds) of channels, as it only requires
     loading a single page to check all of them for updates.
-
-    When main page of a channel (https://www.youtube.com/@ChannelName) is viewed
-    in logged in state, it might contain "For you" block, which content might
-    vary with subsequent updates. As a result, monitoring this url might occasionally
-    produce records with old videos that got showed in this block. If monitoring
-    without a cookies file is not an option, use a combination of "Videos" and "Streams"
-    tabs instead.
     """
 
-    async def handle_first_page(self, entity: PagedFeedMonitorEntity, session: aiohttp.ClientSession) -> Tuple[Optional[Sequence[Record]], Optional[FeedPageContext]]:
+    async def handle_first_page(self, entity: PagedFeedMonitorEntity, session: aiohttp.ClientSession) -> Tuple[Optional[Sequence[Record]], Optional[Any]]:
         raw_page_text = await self.request(entity.url, entity, session)
         if raw_page_text is None:
             return None, None
         raw_page_text = await handle_consent(raw_page_text, entity.url, session, self.logger)
         video_renderers, continuation_token, page = get_video_renderers(raw_page_text)
-        if not video_renderers:
-            self.logger.debug(f'[{entity.name}] found no videos on first page of {entity.url}')
         owner_info = parse_owner_info(page)
         current_page_records = self._parse_entries(owner_info, video_renderers, entity)
         innertube_context = get_innertube_context(raw_page_text)
-        session_index = get_session_index(page)
-        context = FeedPageContext(innertube_context=innertube_context, session_index=session_index, continuation_token=continuation_token, owner_info=owner_info)
-        return current_page_records, context
+        return current_page_records, (innertube_context, owner_info, continuation_token)
 
-    async def handle_next_page(self, entity: PagedFeedMonitorEntity, session: aiohttp.ClientSession, context: Optional[FeedPageContext]) -> Tuple[Optional[Sequence[Record]], Optional[FeedPageContext]]:
-        if context is None or context.continuation_token is None:
+    async def handle_next_page(self, entity: PagedFeedMonitorEntity, session: aiohttp.ClientSession, context: Optional[Any]) -> Tuple[Optional[Sequence[Record]], Optional[Any]]:
+        innertube_context, owner_info, continuation_token = context  # type: ignore
+        if continuation_token is None:
             self.logger.debug(f'[{entity.name}] no continuation for next page, done loading')
             return [], None
 
-        url, headers, post_body = prepare_next_page_request(context.innertube_context, context.continuation_token, cookies=session.cookie_jar)
+        url, headers, post_body = prepare_next_page_request(innertube_context, continuation_token, cookies=session.cookie_jar)
         raw_page = await utils.request(url, session, self.logger, method='POST', headers=headers,
                                        data=json.dumps(post_body), retry_times=3, retry_multiplier=2,
                                        retry_delay=5)
         if raw_page is None:
             self.logger.debug(f'[{entity.name}] failed to load next page, aborting')
             return None, None
         video_renderers, continuation_token, page = get_video_renderers(raw_page, anchor='')
-
-        if not video_renderers:
-            self.logger.debug(f'[{entity.name}] found no videos when parsing continuation of {entity.url}')
-        current_page_records = self._parse_entries(context.owner_info, video_renderers, entity)
-
-        if continuation_token is not None:
-            context.continuation_token = continuation_token
-        else:
-            context = None
+        context = (innertube_context, owner_info, continuation_token) if continuation_token else None
+        current_page_records = self._parse_entries(owner_info, video_renderers, entity)
         return current_page_records, context
 
     def _parse_entries(self, owner_info: Optional[AuthorInfo], video_renderers: List[dict], entity: PagedFeedMonitorEntity) -> List[YoutubeVideoRecord]:
         records: List[YoutubeVideoRecord] = []
         for item in video_renderers:
             try:
                 info = parse_video_renderer(item, owner_info, raise_on_error=True)
                 record = YoutubeVideoRecord.model_validate(info.model_dump())
                 records.append(record)
             except (ValueError, JSONDecodeError, ValidationError) as e:
                 self.logger.warning(f'[{entity.name}] failed to parse video renderer on "{entity.url}": {type(e)}: {e}')
                 self.logger.debug(f'[{entity.name}] raw video renderer:\n{item}')
                 continue
+        if not records:
+            self.logger.warning(f'[{entity.name}] parsing page "{entity.url}" yielded no videos, check url and cookies')
         records = records[::-1] # records are ordered from old to new on page, reorder in chronological order
         return records
 
     def get_record_id(self, record: YoutubeVideoRecord) -> str:
         return record.video_id
 
-    def record_got_updated(self, record: YoutubeVideoRecord, entity: VideosMonitorEntity) -> bool:
-        excluded_fields = {'published_text'}
-        stored_record = self.load_record(record, entity)
-        if stored_record is None:
-            return False
-        record_dump = record.model_dump(exclude=excluded_fields)
-        stored_record_dump = stored_record.model_dump(exclude=excluded_fields)
-        return record_dump != stored_record_dump
-
 
 @Plugins.register('filter.channel', Plugins.kind.ACTOR_CONFIG)
 class ChannelFilterConfig(EmptyFilterConfig):
     pass
 
 @Plugins.register('filter.channel', Plugins.kind.ACTOR_ENTITY)
 class ChannelFilterEntity(FilterEntity):
-    upcoming: bool = False
+    upcoming: bool = True
     """to pass the filter a record should be either upcoming livestream or scheduled premiere"""
     live: bool = False
     """to pass the filter a record should be an ongoing livestream"""
     member_only: bool = False
     """to pass the filter a record should be marked as member-only"""
```

### Comparing `avtdl-0.9.14.3/avtdl/plugins/youtube/youtube_rss.py` & `avtdl-0.9.9/avtdl/plugins/youtube/youtube_rss.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,16 +27,14 @@
     """link to the video"""
     title: str
     """title of the video at the time of parsing"""
     published: datetime
     """published value of the feed item, usually the time when the video was uploaded or the livestream frame was set up"""
     updated: datetime
     """updated value of the feed item. If different from `published`, might indicate either a change to video title, thumbnail or description, or a change in video status, for example livestream ending"""
-    thumbnail_url: Optional[str] = None
-    """link to the video thumbnail"""
     author: str
     """author's name, as shown on the channel icon"""
     video_id: str
     """short string identifying the video on Youtube. Part of the video url"""
     summary: str
     """video's description"""
     views: Optional[int]
@@ -122,15 +120,15 @@
         return super().get_size(feed_name)
 
 
 @Plugins.register('rss', Plugins.kind.ACTOR_ENTITY)
 class FeedMonitorEntity(GenericRSSMonitorEntity):
     update_interval : float = 900
     """How often the feed should be updated, in seconds"""
-    track_reschedule: bool = False
+    track_reschedule: bool = True
     """keep track of scheduled time of upcoming streams, emit record again if it is changed to an earlier date"""
 
 @Plugins.register('rss', Plugins.kind.ACTOR_CONFIG)
 class FeedMonitorConfig(GenericRSSMonitorConfig):
     pass
 
 @Plugins.register('rss', Plugins.kind.ACTOR)
@@ -226,32 +224,25 @@
         for field in ['published', 'updated', 'scheduled']:
             value = latest_row[field]
             # handle db records with old format
             if isinstance(value, str):
                 latest_row[field] = datetime.fromisoformat(value)
         return YoutubeFeedRecord(**latest_row)
 
-    def _parse_entry(self, entry: feedparser.FeedParserDict) -> YoutubeFeedRecord:
+    @classmethod
+    def _parse_entry(cls, entry: feedparser.FeedParserDict) -> YoutubeFeedRecord:
         parsed = {}
         parsed['url'] = entry['link']
         parsed['title'] = entry['title']
         parsed['updated'] = utils.make_datetime(entry['updated_parsed'])
 
         parsed['published'] = utils.make_datetime(entry['published_parsed'])
         parsed['author'] = entry.get('author')
         parsed['summary'] = entry.get('summary')
-        video_id = entry.get('yt_videoid')
-        if video_id is not None:
-            parsed['video_id'] = video_id
-            parsed['thumbnail_url'] = thumbnail_url(video_id)
-        else:
-            parsed['video_id'] = None
-            parsed['thumbnail_url'] = None
-            self.logger.warning(f'[{entry.name}] got entry without video_id: {entry}')
-        """link to the video thumbnail"""
+        parsed['video_id'] = entry.get('yt_videoid', 'video_id missing')
         try:
             views = int(entry['media_statistics']['views'])
         except (ValueError, KeyError, TypeError):
             views = None
         parsed['views'] = views
         record = YoutubeFeedRecord(**parsed)
         return record
```

### Comparing `avtdl-0.9.14.3/avtdl.egg-info/PKG-INFO` & `avtdl-0.9.9/avtdl.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: avtdl
-Version: 0.9.14.3
+Version: 0.9.9
 Summary: Monitoring and automation tool for Youtube and other streaming platforms
 Author: 15532th
 Project-URL: Homepage, https://github.com/15532th/avtdl
 Project-URL: Documentation, https://github.com/15532th/avtdl
 Project-URL: Repository, https://github.com/15532th/avtdl.git
 Project-URL: Issues, https://github.com/15532th/avtdl/issues
 Classifier: Environment :: Console
@@ -23,15 +23,15 @@
 Requires-Dist: Markdown
 Requires-Dist: jsonpath-python==1.0.6
 
 ## avtdl
 
 Tool to monitor Youtube and some other streaming platforms for new streams and uploads and execute user-defined commands when it happens. It aims to provide a highly configurable environment for setting up automated archiving of new content with filtering and notification support. It does not try to provide downloading streams itself and instead relies on executing commonly used well-known solutions for the task, such as `yt-dlp`.
 
-Refer to [documentation](https://github.com/15532th/avtdl?tab=readme-ov-file#avtdl) for full list of available features and description of configuration process.
+Refer to documentation for full list of available features and description of configuration process.
 
 ### Features overview
 
 Some of the supported features include:
 
 - monitoring Youtube channels using RSS feed
 - monitoring Youtube channels, individual tabs of a channel or playlists by parsing html. With authorization cookies from Youtube account it's possible to get notifications for member-only and in any other way restricted streams and uploads, as well as to monitor the entire subscriptions feed
```

### Comparing `avtdl-0.9.14.3/avtdl.egg-info/SOURCES.txt` & `avtdl-0.9.9/avtdl.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,48 +1,43 @@
 .gitignore
 DESCRIPTION.md
-EXAMPLES.md
 LICENSE
 PLUGINS.md
 README.md
 avtdl.py
-example.config.yml
 pyproject.toml
 requirements.txt
-.github/workflows/publish-exe.yml
 .github/workflows/publish-pypi.yml
 avtdl/__init__.py
 avtdl/_version.py
 avtdl/avtdl.py
 avtdl.egg-info/PKG-INFO
 avtdl.egg-info/SOURCES.txt
 avtdl.egg-info/dependency_links.txt
 avtdl.egg-info/entry_points.txt
 avtdl.egg-info/requires.txt
 avtdl.egg-info/top_level.txt
 avtdl/core/__init__.py
 avtdl/core/chain.py
 avtdl/core/config.py
 avtdl/core/db.py
-avtdl/core/download.py
 avtdl/core/info.py
 avtdl/core/interfaces.py
 avtdl/core/loggers.py
 avtdl/core/monitors.py
 avtdl/core/plugins.py
 avtdl/core/utils.py
 avtdl/plugins/__init__.py
 avtdl/plugins/discord/__init__.py
 avtdl/plugins/discord/webhook.py
 avtdl/plugins/execute/__init__.py
 avtdl/plugins/execute/run_command.py
 avtdl/plugins/fc2/__init__.py
 avtdl/plugins/fc2/fc2.py
 avtdl/plugins/file/__init__.py
-avtdl/plugins/file/download.py
 avtdl/plugins/file/text_file.py
 avtdl/plugins/filters/__init__.py
 avtdl/plugins/filters/filters.py
 avtdl/plugins/nitter/__init__.py
 avtdl/plugins/nitter/nitter.py
 avtdl/plugins/rss/__init__.py
 avtdl/plugins/rss/generic_rss.py
```

### Comparing `avtdl-0.9.14.3/pyproject.toml` & `avtdl-0.9.9/pyproject.toml`

 * *Files identical despite different names*

