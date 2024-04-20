# Comparing `tmp/xklb-2.6.7.tar.gz` & `tmp/xklb-2.6.9.tar.gz`

## Comparing `xklb-2.6.7.tar` & `xklb-2.6.9.tar`

### file list

```diff
@@ -1,124 +1,132 @@
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 xklb-2.6.7/.gitattributes
--rw-r--r--   0        0        0   202498 2020-02-02 00:00:00.000000 xklb-2.6.7/pdm.lock
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 xklb-2.6.7/.github/FUNDING.yml
--rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 xklb-2.6.7/.github/LICENSE
--rw-r--r--   0        0        0     1727 2020-02-02 00:00:00.000000 xklb-2.6.7/.github/Windows.md
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 xklb-2.6.7/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 xklb-2.6.7/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 xklb-2.6.7/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0    10282 2020-02-02 00:00:00.000000 xklb-2.6.7/.github/examples/art.avif
--rw-r--r--   0        0        0    17854 2020-02-02 00:00:00.000000 xklb-2.6.7/.github/examples/extract.svg
--rw-r--r--   0        0        0    13463 2020-02-02 00:00:00.000000 xklb-2.6.7/.github/examples/tubeadd.svg
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 xklb-2.6.7/.github/workflows/green.yaml
--rw-r--r--   0        0        0     1724 2020-02-02 00:00:00.000000 xklb-2.6.7/.github/workflows/push.yaml
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/__init__.py
--rw-r--r--   0        0        0    18761 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/db_media.py
--rw-r--r--   0        0        0     8190 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/db_playlists.py
--rw-r--r--   0        0        0    12781 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/dl_extract.py
--rw-r--r--   0        0        0    15664 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/fs_extract.py
--rw-r--r--   0        0        0     8076 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/gdl_backend.py
--rw-r--r--   0        0        0     3230 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/gdl_extract.py
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/history.py
--rw-r--r--   0        0        0     5622 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/hn_extract.py
--rw-r--r--   0        0        0    13595 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/lb.py
--rw-r--r--   0        0        0    19486 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/play_actions.py
--rw-r--r--   0        0        0     7206 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/post_actions.py
--rw-r--r--   0        0        0    13926 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/readme.py
--rw-r--r--   0        0        0    13125 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/reddit_extract.py
--rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/rss_extract.py
--rw-r--r--   0        0        0     6208 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/search.py
--rw-r--r--   0        0        0     6463 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/site_extract.py
--rw-r--r--   0        0        0     5890 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/tabs_actions.py
--rw-r--r--   0        0        0     5722 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/tabs_extract.py
--rw-r--r--   0        0        0    20308 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/tube_backend.py
--rw-r--r--   0        0        0     4059 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/tube_extract.py
--rw-r--r--   0        0        0   118259 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/usage.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/data/__init__.py
--rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/data/imagemagick_errors.py
--rw-r--r--   0        0        0    17127 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/data/wordbank.py
--rw-r--r--   0        0        0     7204 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/data/yt_dlp_errors.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/media/__init__.py
--rw-r--r--   0        0        0     9140 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/media/av.py
--rw-r--r--   0        0        0     7460 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/media/books.py
--rw-r--r--   0        0        0    20852 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/media/dedupe.py
--rw-r--r--   0        0        0     6806 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/media/media_check.py
--rw-r--r--   0        0        0    23467 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/media/media_player.py
--rw-r--r--   0        0        0    10390 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/media/media_printer.py
--rw-r--r--   0        0        0     4597 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/media/subtitle.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/scratch/__init__.py
--rw-r--r--   0        0        0     6159 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/scratch/javguru.py
--rw-r--r--   0        0        0     1897 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/scratch/javtiful.py
--rw-r--r--   0        0        0     8327 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/scratch/mam_search.py
--rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/scratch/mam_slots.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/scripts/__init__.py
--rw-r--r--   0        0        0     1282 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/scripts/add_row.py
--rw-r--r--   0        0        0     7057 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/scripts/big_dirs.py
--rw-r--r--   0        0        0    11608 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/scripts/block.py
--rw-r--r--   0        0        0     2717 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/scripts/christen.py
--rw-r--r--   0        0        0    13461 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/scripts/cluster_sort.py
--rw-r--r--   0        0        0     1957 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/scripts/copy_play_counts.py
--rw-r--r--   0        0        0    13814 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/scripts/dedupe_czkawka.py
--rw-r--r--   0        0        0     4049 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/scripts/dedupe_db.py
--rw-r--r--   0        0        0     4903 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/scripts/disk_usage.py
--rw-r--r--   0        0        0     3627 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/scripts/download_status.py
--rw-r--r--   0        0        0     7498 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/scripts/eda.py
--rw-r--r--   0        0        0     1361 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/scripts/export_text.py
--rw-r--r--   0        0        0     6810 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/scripts/history.py
--rw-r--r--   0        0        0     4437 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/scripts/incremental_diff.py
--rw-r--r--   0        0        0    10811 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/scripts/links_db.py
--rw-r--r--   0        0        0     8241 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/scripts/mcda.py
--rw-r--r--   0        0        0     3522 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/scripts/merge_dbs.py
--rw-r--r--   0        0        0     7811 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/scripts/merge_folders.py
--rw-r--r--   0        0        0     3695 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/scripts/merge_online_local.py
--rw-r--r--   0        0        0     7501 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/scripts/move_list.py
--rw-r--r--   0        0        0     6658 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/scripts/open_links.py
--rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/scripts/optimize_db.py
--rw-r--r--   0        0        0     1997 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/scripts/places_import.py
--rw-r--r--   0        0        0     9778 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/scripts/playback_control.py
--rw-r--r--   0        0        0     5638 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/scripts/playlists.py
--rw-r--r--   0        0        0     7478 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/scripts/process_ffmpeg.py
--rw-r--r--   0        0        0     2885 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/scripts/process_image.py
--rw-r--r--   0        0        0     5559 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/scripts/redownload.py
--rw-r--r--   0        0        0     2906 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/scripts/rel_mv.py
--rw-r--r--   0        0        0     3634 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/scripts/sample_compare.py
--rw-r--r--   0        0        0     2693 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/scripts/sample_hash.py
--rw-r--r--   0        0        0    11711 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/scripts/scatter.py
--rw-r--r--   0        0        0     2583 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/scripts/search_db.py
--rw-r--r--   0        0        0     2378 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/scripts/streaming_tab_loader.py
--rw-r--r--   0        0        0     9864 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/scripts/web_add.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/scripts/mining/__init__.py
--rw-r--r--   0        0        0     6607 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/scripts/mining/extract_links.py
--rw-r--r--   0        0        0     3486 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/scripts/mining/extract_text.py
--rw-r--r--   0        0        0     1886 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/scripts/mining/markdown_links.py
--rw-r--r--   0        0        0     1848 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/scripts/mining/mpv_watchlater.py
--rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/scripts/mining/nouns.py
--rw-r--r--   0        0        0     2032 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/scripts/mining/pushshift.py
--rw-r--r--   0        0        0     2172 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/scripts/mining/reddit_selftext.py
--rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/scripts/mining/substack.py
--rw-r--r--   0        0        0     5733 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/scripts/mining/tildes.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/utils/__init__.py
--rw-r--r--   0        0        0     6202 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/utils/arg_utils.py
--rw-r--r--   0        0        0    17780 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/utils/arggroups.py
--rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/utils/argparse_utils.py
--rw-r--r--   0        0        0    10529 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/utils/consts.py
--rw-r--r--   0        0        0    11248 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/utils/db_utils.py
--rw-r--r--   0        0        0     3793 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/utils/devices.py
--rw-r--r--   0        0        0    15276 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/utils/file_utils.py
--rw-r--r--   0        0        0     6208 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/utils/gui.py
--rw-r--r--   0        0        0     4574 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/utils/iterables.py
--rw-r--r--   0        0        0     2051 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/utils/log_utils.py
--rw-r--r--   0        0        0     2237 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/utils/mpv_utils.py
--rw-r--r--   0        0        0     4023 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/utils/nums.py
--rw-r--r--   0        0        0     3714 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/utils/objects.py
--rw-r--r--   0        0        0     3326 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/utils/path_utils.py
--rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/utils/pd_utils.py
--rw-r--r--   0        0        0     7418 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/utils/printing.py
--rw-r--r--   0        0        0     7051 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/utils/processes.py
--rw-r--r--   0        0        0     8306 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/utils/sql_utils.py
--rw-r--r--   0        0        0     6170 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/utils/strings.py
--rw-r--r--   0        0        0    22132 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/utils/web.py
--rw-r--r--   0        0        0     8385 2020-02-02 00:00:00.000000 xklb-2.6.7/xklb/assets/kotobago.png
--rw-r--r--   0        0        0     1504 2020-02-02 00:00:00.000000 xklb-2.6.7/.gitignore
--rw-r--r--   0        0        0     3111 2020-02-02 00:00:00.000000 xklb-2.6.7/pyproject.toml
--rw-r--r--   0        0        0   158475 2020-02-02 00:00:00.000000 xklb-2.6.7/.github/README.md
--rw-r--r--   0        0        0   162236 2020-02-02 00:00:00.000000 xklb-2.6.7/PKG-INFO
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 xklb-2.6.9/.gitattributes
+-rw-r--r--   0        0        0   202498 2020-02-02 00:00:00.000000 xklb-2.6.9/pdm.lock
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 xklb-2.6.9/.github/FUNDING.yml
+-rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 xklb-2.6.9/.github/LICENSE
+-rw-r--r--   0        0        0     1727 2020-02-02 00:00:00.000000 xklb-2.6.9/.github/Windows.md
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 xklb-2.6.9/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 xklb-2.6.9/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 xklb-2.6.9/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0    10282 2020-02-02 00:00:00.000000 xklb-2.6.9/.github/examples/art.avif
+-rw-r--r--   0        0        0    17854 2020-02-02 00:00:00.000000 xklb-2.6.9/.github/examples/extract.svg
+-rw-r--r--   0        0        0    13463 2020-02-02 00:00:00.000000 xklb-2.6.9/.github/examples/tubeadd.svg
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 xklb-2.6.9/.github/workflows/green.yaml
+-rw-r--r--   0        0        0     1724 2020-02-02 00:00:00.000000 xklb-2.6.9/.github/workflows/push.yaml
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/__init__.py
+-rw-r--r--   0        0        0    18758 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/db_media.py
+-rw-r--r--   0        0        0     8190 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/db_playlists.py
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/history.py
+-rw-r--r--   0        0        0    13707 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/lb.py
+-rw-r--r--   0        0        0    10415 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/media_printer.py
+-rw-r--r--   0        0        0    13927 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/readme.py
+-rw-r--r--   0        0        0   119411 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/usage.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/createdb/__init__.py
+-rw-r--r--   0        0        0     9170 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/createdb/av.py
+-rw-r--r--   0        0        0    23196 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/createdb/fs_add.py
+-rw-r--r--   0        0        0     3277 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/createdb/gallery_add.py
+-rw-r--r--   0        0        0     8076 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/createdb/gallery_backend.py
+-rw-r--r--   0        0        0     5623 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/createdb/hn_add.py
+-rw-r--r--   0        0        0    10801 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/createdb/links_add.py
+-rw-r--r--   0        0        0     1997 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/createdb/places_import.py
+-rw-r--r--   0        0        0    13129 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/createdb/reddit_add.py
+-rw-r--r--   0        0        0     1282 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/createdb/row_add.py
+-rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/createdb/rss_add.py
+-rw-r--r--   0        0        0     6464 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/createdb/site_add.py
+-rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/createdb/substack.py
+-rw-r--r--   0        0        0     4597 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/createdb/subtitle.py
+-rw-r--r--   0        0        0     5724 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/createdb/tabs_add.py
+-rw-r--r--   0        0        0     5733 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/createdb/tildes.py
+-rw-r--r--   0        0        0     4090 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/createdb/tube_add.py
+-rw-r--r--   0        0        0    20339 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/createdb/tube_backend.py
+-rw-r--r--   0        0        0     9862 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/createdb/web_add.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/data/__init__.py
+-rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/data/imagemagick_errors.py
+-rw-r--r--   0        0        0    17127 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/data/wordbank.py
+-rw-r--r--   0        0        0     7204 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/data/yt_dlp_errors.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/editdb/__init__.py
+-rw-r--r--   0        0        0     4049 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/editdb/dedupe_db.py
+-rw-r--r--   0        0        0    20728 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/editdb/dedupe_media.py
+-rw-r--r--   0        0        0     3673 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/editdb/merge_online_local.py
+-rw-r--r--   0        0        0     1848 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/editdb/mpv_watchlater.py
+-rw-r--r--   0        0        0     2037 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/editdb/pushshift.py
+-rw-r--r--   0        0        0     2172 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/editdb/reddit_selftext.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/files/__init__.py
+-rw-r--r--   0        0        0     3632 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/files/sample_compare.py
+-rw-r--r--   0        0        0     2693 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/files/sample_hash.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/folders/__init__.py
+-rw-r--r--   0        0        0     7811 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/folders/merge_folders.py
+-rw-r--r--   0        0        0     7501 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/folders/move_list.py
+-rw-r--r--   0        0        0     2906 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/folders/rel_mv.py
+-rw-r--r--   0        0        0    11711 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/folders/scatter.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/fsdb/__init__.py
+-rw-r--r--   0        0        0     7036 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/fsdb/big_dirs.py
+-rw-r--r--   0        0        0     2717 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/fsdb/christen.py
+-rw-r--r--   0        0        0     4882 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/fsdb/disk_usage.py
+-rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/fsdb/mount_stats.py
+-rw-r--r--   0        0        0     2583 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/fsdb/search_db.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/mediadb/__init__.py
+-rw-r--r--   0        0        0    11633 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/mediadb/block.py
+-rw-r--r--   0        0        0    12796 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/mediadb/download.py
+-rw-r--r--   0        0        0     3650 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/mediadb/download_status.py
+-rw-r--r--   0        0        0     6765 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/mediadb/history.py
+-rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/mediadb/optimize_db.py
+-rw-r--r--   0        0        0     5616 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/mediadb/playlists.py
+-rw-r--r--   0        0        0     5537 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/mediadb/redownload.py
+-rw-r--r--   0        0        0     6159 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/mediadb/search.py
+-rw-r--r--   0        0        0     6806 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/mediafiles/media_check.py
+-rw-r--r--   0        0        0     7478 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/mediafiles/process_ffmpeg.py
+-rw-r--r--   0        0        0     2885 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/mediafiles/process_image.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/misc/__init__.py
+-rw-r--r--   0        0        0    13764 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/misc/dedupe_czkawka.py
+-rw-r--r--   0        0        0     1361 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/misc/export_text.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/multidb/__init__.py
+-rw-r--r--   0        0        0     1954 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/multidb/copy_play_counts.py
+-rw-r--r--   0        0        0     3522 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/multidb/merge_dbs.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/playback/__init__.py
+-rw-r--r--   0        0        0     6633 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/playback/links_open.py
+-rw-r--r--   0        0        0    23498 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/playback/media_player.py
+-rw-r--r--   0        0        0    19535 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/playback/play_actions.py
+-rw-r--r--   0        0        0     9779 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/playback/playback_control.py
+-rw-r--r--   0        0        0     7206 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/playback/post_actions.py
+-rw-r--r--   0        0        0     2381 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/playback/surf.py
+-rw-r--r--   0        0        0     5826 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/playback/tabs_open.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/scratch/__init__.py
+-rw-r--r--   0        0        0     6164 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/scratch/javguru.py
+-rw-r--r--   0        0        0     1902 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/scratch/javtiful.py
+-rw-r--r--   0        0        0     8327 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/scratch/mam_search.py
+-rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/scratch/mam_slots.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/tablefiles/__init__.py
+-rw-r--r--   0        0        0     7498 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/tablefiles/eda.py
+-rw-r--r--   0        0        0     4437 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/tablefiles/incremental_diff.py
+-rw-r--r--   0        0        0     8241 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/tablefiles/mcda.py
+-rw-r--r--   0        0        0    13464 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/text/cluster_sort.py
+-rw-r--r--   0        0        0     6607 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/text/extract_links.py
+-rw-r--r--   0        0        0     3486 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/text/extract_text.py
+-rw-r--r--   0        0        0     1935 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/text/markdown_links.py
+-rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/text/nouns.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/utils/__init__.py
+-rw-r--r--   0        0        0     6202 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/utils/arg_utils.py
+-rw-r--r--   0        0        0    16906 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/utils/arggroups.py
+-rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/utils/argparse_utils.py
+-rw-r--r--   0        0        0    10555 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/utils/consts.py
+-rw-r--r--   0        0        0    11248 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/utils/db_utils.py
+-rw-r--r--   0        0        0     3252 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/utils/devices.py
+-rw-r--r--   0        0        0    15276 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/utils/file_utils.py
+-rw-r--r--   0        0        0     6208 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/utils/gui.py
+-rw-r--r--   0        0        0     4574 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/utils/iterables.py
+-rw-r--r--   0        0        0     2051 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/utils/log_utils.py
+-rw-r--r--   0        0        0     2237 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/utils/mpv_utils.py
+-rw-r--r--   0        0        0     4023 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/utils/nums.py
+-rw-r--r--   0        0        0     3714 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/utils/objects.py
+-rw-r--r--   0        0        0     3326 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/utils/path_utils.py
+-rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/utils/pd_utils.py
+-rw-r--r--   0        0        0     7418 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/utils/printing.py
+-rw-r--r--   0        0        0     7051 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/utils/processes.py
+-rw-r--r--   0        0        0     8306 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/utils/sql_utils.py
+-rw-r--r--   0        0        0     6170 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/utils/strings.py
+-rw-r--r--   0        0        0    22132 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/utils/web.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/assets/__init__.py
+-rw-r--r--   0        0        0     8385 2020-02-02 00:00:00.000000 xklb-2.6.9/xklb/assets/kotobago.png
+-rw-r--r--   0        0        0     1504 2020-02-02 00:00:00.000000 xklb-2.6.9/.gitignore
+-rw-r--r--   0        0        0     3111 2020-02-02 00:00:00.000000 xklb-2.6.9/pyproject.toml
+-rw-r--r--   0        0        0   159958 2020-02-02 00:00:00.000000 xklb-2.6.9/.github/README.md
+-rw-r--r--   0        0        0   163719 2020-02-02 00:00:00.000000 xklb-2.6.9/PKG-INFO
```

### Comparing `xklb-2.6.7/pdm.lock` & `xklb-2.6.9/pdm.lock`

 * *Files identical despite different names*

### Comparing `xklb-2.6.7/.github/LICENSE` & `xklb-2.6.9/.github/LICENSE`

 * *Files identical despite different names*

### Comparing `xklb-2.6.7/.github/Windows.md` & `xklb-2.6.9/.github/Windows.md`

 * *Files identical despite different names*

### Comparing `xklb-2.6.7/.github/examples/art.avif` & `xklb-2.6.9/.github/examples/art.avif`

 * *Files identical despite different names*

### Comparing `xklb-2.6.7/.github/examples/extract.svg` & `xklb-2.6.9/.github/examples/extract.svg`

 * *Files identical despite different names*

### Comparing `xklb-2.6.7/.github/examples/tubeadd.svg` & `xklb-2.6.9/.github/examples/tubeadd.svg`

 * *Files identical despite different names*

### Comparing `xklb-2.6.7/.github/workflows/push.yaml` & `xklb-2.6.9/.github/workflows/push.yaml`

 * *Files identical despite different names*

### Comparing `xklb-2.6.7/xklb/db_media.py` & `xklb-2.6.9/xklb/db_media.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import argparse, os, sqlite3
 from collections.abc import Collection
 from datetime import datetime
 from pathlib import Path
 
 from dateutil import parser
 
-from xklb import fs_extract
+from xklb.createdb import fs_add
 from xklb.utils import consts, db_utils, iterables, nums, objects, processes, strings
 from xklb.utils.consts import DBType
 from xklb.utils.log_utils import log
 
 
 def exists(args, path) -> bool:
     m_columns = db_utils.columns(args, "media")
@@ -244,17 +244,17 @@
             profile=args.profile,
             scan_subtitles=args.profile == DBType.video,
             ocr=False,
             speech_recognition=False,
             delete_unplayable=False,
             check_corrupt=False,
         )
-        fs_tags = fs_extract.extract_metadata(fs_args, local_path)
+        fs_tags = fs_add.extract_metadata(fs_args, local_path)
         fs_tags = objects.dict_filter_bool(fs_tags, keep_0=False) or {}
-        fs_extract.clean_up_temp_dirs()
+        fs_add.clean_up_temp_dirs()
     else:
         fs_tags = {"time_modified": consts.now()}
 
     if not info:  # not downloaded or already downloaded
         info = {"path": webpath}
 
     consolidated_entry = consolidate(info) or {}
```

### Comparing `xklb-2.6.7/xklb/db_playlists.py` & `xklb-2.6.9/xklb/db_playlists.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.7/xklb/dl_extract.py` & `xklb-2.6.9/xklb/mediadb/download.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import argparse, os, sys
 
-from xklb import db_media, gdl_backend, tube_backend, usage
-from xklb.media import media_printer
+from xklb import db_media, media_printer, usage
+from xklb.createdb import gallery_backend, tube_backend
 from xklb.utils import (
     arg_utils,
     arggroups,
     argparse_utils,
     consts,
     db_utils,
     iterables,
@@ -283,15 +283,15 @@
     for m in media:
         if args.blocklist_rules and sql_utils.is_blocked_dict_like_sql(m, args.blocklist_rules):
             mark_download_attempt(args, [m["path"]])
             continue
 
         if args.safe:
             if (args.profile in (DBType.audio, DBType.video) and not tube_backend.is_supported(m["path"])) or (
-                args.profile in (DBType.image) and not gdl_backend.is_supported(args, m["path"])
+                args.profile in (DBType.image) and not gallery_backend.is_supported(args, m["path"])
             ):
                 log.info("[%s]: Skipping unsupported URL (safe_mode)", m["path"])
                 mark_download_attempt(args, [m["path"]])
                 continue
 
         # check if download already attempted recently by another process
         previous_time_attempted = m.get("time_modified") or consts.APPLICATION_START  # 0 is nullified
@@ -325,15 +325,15 @@
 
         try:
             log.debug(m)
 
             if args.profile in (DBType.audio, DBType.video):
                 tube_backend.download(args, m)
             elif args.profile == DBType.image:
-                gdl_backend.download(args, m)
+                gallery_backend.download(args, m)
             elif args.profile == DBType.filesystem:
                 local_path = web.download_url(m["path"], output_prefix=args.prefix)
                 db_media.download_add(args, m["path"], m, local_path)
             else:
                 raise NotImplementedError
         except Exception:
             print("db:", args.database)
```

### Comparing `xklb-2.6.7/xklb/fs_extract.py` & `xklb-2.6.9/xklb/misc/dedupe_czkawka.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,433 +1,383 @@
-import argparse, json, math, os, sys
-from concurrent.futures import ProcessPoolExecutor, ThreadPoolExecutor
-from functools import partial
-from multiprocessing import TimeoutError as mp_TimeoutError
+import argparse, difflib, os, re, shlex, shutil, subprocess, sys, time
+from concurrent.futures import ThreadPoolExecutor
 from pathlib import Path
-from shutil import which
-from timeit import default_timer as timer
 
-from xklb import db_media, db_playlists, usage
-from xklb.media import av, books
-from xklb.scripts import playlists, process_ffmpeg, process_image, sample_hash
-from xklb.utils import arg_utils, arggroups, consts, db_utils, file_utils, iterables, nums, objects, path_utils
-from xklb.utils.consts import SC, DBType
+import humanize
+from screeninfo import get_monitors
+
+from xklb import usage
+from xklb.playback import media_player, post_actions
+from xklb.utils import arggroups, consts, devices, file_utils, iterables, mpv_utils, processes
 from xklb.utils.log_utils import log
 
+left_mpv_socket = str(Path(consts.TEMP_SCRIPT_DIR) / f"mpv_socket_{consts.random_string()}")
+right_mpv_socket = str(Path(consts.TEMP_SCRIPT_DIR) / f"mpv_socket_{consts.random_string()}")
+
 
-def parse_args(action, usage):
-    parser = argparse.ArgumentParser(prog="library " + action, usage=usage)
-    arggroups.db_profiles(parser)
-    arggroups.capability_simulate(parser)
+def parse_args():
+    parser = argparse.ArgumentParser(usage.dedupe_czkawka)
+    arggroups.playback(parser)
+    arggroups.capability_clobber(parser)
+    arggroups.capability_delete(parser)
+    arggroups.post_actions(parser)
+    parser.set_defaults(start="15%", volume="70")
 
     parser.add_argument(
-        "--io-multiplier",
+        "--auto-select-min-ratio",
         type=float,
         default=1.0,
-        help="Especially useful for text, image, filesystem db types",
-    )
-    parser.add_argument("--ocr", "--OCR", action="store_true", help=argparse.SUPPRESS)
-    parser.add_argument("--speech-recognition", "--speech", action="store_true", help=argparse.SUPPRESS)
-    parser.add_argument("--scan-subtitles", "--scan-subtitle", action="store_true", help=argparse.SUPPRESS)
-
-    parser.add_argument("--hash", action="store_true")
-    parser.add_argument("--move")
-
-    parser.add_argument("--process", action="store_true", help=argparse.SUPPRESS)
-    arggroups.process_ffmpeg(parser)
-    parser.add_argument("--delete-unplayable", action="store_true")
-
-    parser.add_argument("--check-corrupt", "--check-corruption", action="store_true")
-    arggroups.media_check(parser)
-    parser.set_defaults(gap="0.10")
-
-    parser.add_argument(
-        "--force", "-f", action="store_true", help="Mark all subpath files as deleted if no files found"
+        help="Automatically select largest file if files have similar basenames. A sane value is in the range of 0.7~0.9",
     )
+    parser.add_argument("--all-keep", action="store_true")
+    parser.add_argument("--all-left", action="store_true")
+    parser.add_argument("--all-right", action="store_true")
+    parser.add_argument("--all-delete", action="store_true")
     arggroups.debug(parser)
 
-    arggroups.database(parser)
-    if action == SC.fsadd:
-        parser.add_argument("paths", nargs="+")
-    args = parser.parse_intermixed_args()
+    parser.add_argument("file_path", help="Path to the text file containing the file list.")
+    args = parser.parse_args()
+    return args
 
-    if not args.profiles:
-        args.profiles = [DBType.video]
 
-    if args.move:
-        args.move = str(Path(args.move).expanduser().resolve())
+def backup_and_read_file(file_path):
+    backup_filename = file_path + ".bak"
+    if not os.path.exists(backup_filename):
+        try:
+            shutil.copy2(file_path, backup_filename)
+        except Exception as e:
+            print(f"Failed to create backup file: {e}")
 
-    args.gap = nums.float_from_percent(args.gap)
-    if args.delete_corrupt:
-        args.delete_corrupt = nums.float_from_percent(args.delete_corrupt)
-    if args.full_scan_if_corrupt:
-        args.full_scan_if_corrupt = nums.float_from_percent(args.full_scan_if_corrupt)
+    with open(file_path) as file:
+        content = file.read()
+    return content
 
-    args.split_longer_than = nums.human_to_seconds(args.split_longer_than)
-    args.min_split_segment = nums.human_to_seconds(args.min_split_segment)
 
-    Path(args.database).touch()
-    args.db = db_utils.connect(args)
+def extract_dupe_groups(content):
+    first_newline_index = content.find("\n")
 
-    if hasattr(args, "paths"):
-        args.paths = iterables.conform(args.paths)
-    log.info(objects.dict_filter_bool(args.__dict__))
+    if first_newline_index != -1 and "similar friends" in content[:first_newline_index].strip().lower():
+        content = content[first_newline_index + 1 :]
 
-    if not which("ffprobe") and (DBType.audio in args.profiles or DBType.video in args.profiles):
-        log.error("ffmpeg is not installed. Install it with your package manager.")
-        raise SystemExit(3)
+    groups = re.split(r"(-+MESSAGES-+\n+)", content)[0].split("\n\n")
+    return groups
 
-    return args, parser
 
+def parse_czkawka_line(line):
+    image_pattern = r"^(.+) - (\d+x\d+) - (\d+(?:\.\d+)?|\d+) ([KMG]iB) - .+$"
+    video_pattern = r"^(.+) - (\d+(?:\.\d+)?|\d+) ([KMG]iB)$"
 
-def extract_metadata(mp_args, path) -> dict[str, int] | None:
-    try:
-        path.encode()
-    except UnicodeEncodeError:
-        log.error("Could not encode file path as UTF-8. Skipping %s", path)
-        return None
+    image_match = re.match(image_pattern, line)
+    if image_match:
+        path, resolution, size_value, size_unit = image_match.groups()
+        return path.strip(), float(size_value), size_unit
 
-    try:
-        stat = os.stat(path, follow_symlinks=False)
-    except FileNotFoundError:
-        return None
-    except OSError:
-        log.error(f"IOError: possible filesystem corruption; check dmesg. {path}")
-        return None
-    except Exception as e:
-        log.error(f"%s {path}", e)
-        return None
+    video_match = re.match(video_pattern, line)
+    if video_match:
+        path, size_value, size_unit = video_match.groups()
+        return path.strip(), float(size_value), size_unit
 
-    media = {
-        "path": path,
-        "size": stat.st_size,
-        "type": file_utils.mimetype(path),
-        "time_created": int(stat.st_ctime),
-        "time_modified": int(stat.st_mtime) or consts.now(),
-        "time_downloaded": consts.APPLICATION_START,
-        "time_deleted": 0,
-    }
+    raise ValueError("Could not detect file style")
 
-    ext = path.rsplit(".", 1)[-1].lower()
-    is_scan_all_files = getattr(mp_args, "scan_all_files", False)
 
-    if media["type"] == "directory":
+def extract_group_data(group_content):
+    paths_and_sizes = []
+    groups = group_content.split("\n")
+    if len(groups) < 2:
         return None
+    for match in groups:
+        if match == "":
+            continue
+
+        path, size_value, size_unit = parse_czkawka_line(match)
+        if size_unit == "GiB":
+            size_value *= 1024 * 1024 * 1024
+        elif size_unit == "MiB":
+            size_value *= 1024 * 1024
+        elif size_unit == "KiB":
+            size_value *= 1024
+        paths_and_sizes.append({"path": path, "size": size_value})
+    return paths_and_sizes
+
+
+def truncate_file_before_match(filename, match_string):
+    with open(filename) as file:
+        lines = file.readlines()
+    matching_lines = [i for i, line in enumerate(lines) if match_string in line]
+
+    if len(matching_lines) == 1:
+        line_index = matching_lines[0]
+        with open(filename, "w") as file:
+            file.write("".join(lines[line_index - 1 :]))
+        print(f"Progress saved. File truncated before the line containing: '{match_string}'")
+        remaining = sum(1 for s in lines[line_index - 1 :] if s == "\n") - 1
+        num_videos = sum(1 for s in lines[line_index - 1 :] if s != "\n") - 12
+        print(f"{remaining} groups (~{num_videos} videos) remain to check")
+    elif len(matching_lines) == 0:
+        print(f"Match not found in the file: '{match_string}'")
+    else:
+        print(f"Multiple matches found in the file for: '{match_string}'")
 
-    if not Path(path).exists():
-        return media
-
-    if objects.is_profile(mp_args, DBType.audio) and (ext in consts.AUDIO_ONLY_EXTENSIONS or is_scan_all_files):
-        media |= av.munge_av_tags(mp_args, path)
-    elif objects.is_profile(mp_args, DBType.video) and (ext in consts.VIDEO_EXTENSIONS or is_scan_all_files):
-        media |= av.munge_av_tags(mp_args, path)
-
-    if not Path(path).exists():  # av.munge_av_tags might delete if unplayable or corruption exceeds threshold
-        return media
-
-    text_exts = consts.TEXTRACT_EXTENSIONS
-    if mp_args.ocr:
-        text_exts |= consts.OCR_EXTENSIONS
-    if mp_args.speech_recognition:
-        text_exts |= consts.SPEECH_RECOGNITION_EXTENSIONS
-    if objects.is_profile(mp_args, DBType.text) and (ext in text_exts or is_scan_all_files):
-        try:
-            start = timer()
-            if any([mp_args.ocr, mp_args.speech_recognition]):
-                media |= books.munge_book_tags_slow(path)
-            else:
-                media |= books.munge_book_tags_fast(path)
-        except mp_TimeoutError:
-            log.warning(f"Timed out trying to read file. {path}")
-        else:
-            log.debug(f"{timer()-start} {path}")
-
-    if getattr(mp_args, "hash", False) and media["type"] != "directory" and media["size"] > 0:
-        media["hash"] = sample_hash.sample_hash_file(path)
 
-    if getattr(mp_args, "move", False) and not file_utils.is_file_open(path):
-        dest_path = bytes(Path(mp_args.move) / Path(path).relative_to(mp_args.playlist_path))
-        dest_path = path_utils.clean_path(dest_path)
-        file_utils.rename_move_file(path, dest_path, simulate=mp_args.simulate)
-        path = media["path"] = dest_path
-
-    if getattr(mp_args, "process", False):
-        if objects.is_profile(mp_args, DBType.audio) and Path(path).suffix not in [".opus", ".mka"]:
-            result = process_ffmpeg.process_path(
-                mp_args,
-                path,
-                split_longer_than=2160 if mp_args.split_longer_than is None and "audiobook" in path.lower() else None,
-            )
-            if result is None:
-                return None
-            path = media["path"] = str(result)
-        elif objects.is_profile(mp_args, DBType.video) and Path(path).suffix not in [".av1.mkv"]:
-            result = process_ffmpeg.process_path(mp_args, path)
-            if result is None:
-                return None
-            path = media["path"] = str(result)
-        elif objects.is_profile(mp_args, DBType.image) and Path(path).suffix not in [".avif", ".avifs"]:
-            result = process_image.process_path(mp_args, path)
-            if result is None:
-                return None
-            path = media["path"] = str(result)
-
-    return media
-
-
-def clean_up_temp_dirs():
-    temp_subs_path = Path(consts.SUB_TEMP_DIR)
-    if temp_subs_path.exists():
-        for p in temp_subs_path.glob("*.srt"):
-            p.unlink()
-
-
-def extract_chunk(args, media) -> None:
-    if objects.is_profile(args, DBType.image):
-        media = books.extract_image_metadata_chunk(media)
-
-    if args.scan_subtitles:
-        clean_up_temp_dirs()
-
-    captions = []
-    for d in media:
-        caption = {}
-        caption["path"] = d["path"]
-
-        caption["chapters"] = d.pop("chapters", None) or []
-        caption["subtitles"] = d.pop("subtitles", None) or []
-
-        tags = d.pop("tags", None) or ""
-        description = d.pop("description", None) or ""
-        if description:
-            tags += "\n" + description
-        if tags:
-            caption["captions_t0"] = {"time": 0, "text": tags}
-
-        captions.append(caption)
-
-    media = [{"playlists_id": args.playlists_id, **d} for d in media]
-    media = iterables.list_dict_filter_bool(media)
-    args.db["media"].insert_all(media, pk="id", alter=True, replace=True)
-
-    for d in captions:
-        media_id = args.db.pop("select id from media where path = ?", [d["path"]])
-        if len(d["chapters"]) > 0:
-            args.db["captions"].insert_all([{**d, "media_id": media_id} for d in d["chapters"]], alter=True)
-        if len(d["subtitles"]) > 0:
-            args.db["captions"].insert_all([{**d, "media_id": media_id} for d in d["subtitles"]], alter=True)
-        if d.get("caption_t0"):
-            args.db["captions"].insert({**d["caption_t0"], "media_id": media_id}, alter=True)
-
-
-def mark_media_undeleted(args, paths) -> int:
-    paths = iterables.conform(paths)
-
-    modified_row_count = 0
-    if paths:
-        df_chunked = iterables.chunks(paths, consts.SQLITE_PARAM_LIMIT)
-        for chunk_paths in df_chunked:
-            with args.db.conn:
-                cursor = args.db.conn.execute(
-                    """update media
-                    set time_deleted=0
-                    where path in ("""
-                    + ",".join(["?"] * len(chunk_paths))
-                    + ")",
-                    (*chunk_paths,),
-                )
-                modified_row_count += cursor.rowcount
-
-    return modified_row_count
-
-
-def find_new_files(args, path) -> list[str]:
-    if path.is_file():
-        scanned_set = {str(path)}
-    else:
-        for s in args.profiles:
-            if getattr(DBType, s, None) is None:
-                msg = f"fs_extract for profile {s}"
-                raise NotImplementedError(msg)
-
-        exts = args.ext
-        if not exts:
-            exts = set()
-            if args.scan_all_files or DBType.filesystem in args.profiles:
-                exts = None
-            else:
-                if DBType.audio in args.profiles:
-                    exts |= consts.AUDIO_ONLY_EXTENSIONS
-                if DBType.video in args.profiles:
-                    exts |= consts.VIDEO_EXTENSIONS
-
-                if DBType.image in args.profiles:
-                    exts |= consts.IMAGE_EXTENSIONS
-
-                if DBType.text in args.profiles:
-                    exts |= consts.TEXTRACT_EXTENSIONS
-                if args.ocr:
-                    exts |= consts.OCR_EXTENSIONS
-                if args.speech_recognition:
-                    exts |= consts.SPEECH_RECOGNITION_EXTENSIONS
+def side_by_side_mpv(args, left_side, right_side):
+    monitors = get_monitors()
+    if not monitors:
+        print("No connected displays found.")
+        return
 
-        if DBType.filesystem in args.profiles:
-            scanned_set = set.union(*file_utils.rglob(path))
-        else:
-            scanned_set = file_utils.rglob(path, exts)[0]
+    display = media_player.modify_display_size_for_taskbar(monitors[0])
+    mpv_width = display.width // 2
 
-    m_columns = db_utils.columns(args, "media")
+    if args.auto_seek:
+        from python_mpv_jsonipc import MPV
 
-    try:
-        deleted_set = {
-            d["path"]
-            for d in args.db.query(
-                f"""select path from media
-                where 1=1
-                    and time_deleted > 0
-                    and path like '{path}%'
-                    {'AND time_downloaded > 0' if 'time_downloaded' in m_columns else ''}
-                """,
-            )
+        mpv_kwargs = {
+            "save_position_on_quit": False,
+            "start": args.start,
         }
-    except Exception as e:
-        log.debug(e)
-    else:
-        undeleted_files = list(deleted_set.intersection(scanned_set))
-        undeleted_count = mark_media_undeleted(args, undeleted_files)
-        if undeleted_count > 0:
-            print(f"[{path}] Marking", undeleted_count, "metadata records as undeleted")
 
-    try:
-        existing_set = {
-            d["path"]
-            for d in args.db.query(
-                f"""select path from media
-                where 1=1
-                    and path like ?
-                    and coalesce(time_deleted, 0) = 0
-                    {'AND time_downloaded > 0' if 'time_downloaded' in m_columns else ''}
-                """,
-                [str(path) + "%"],
-            )
-        }
-    except Exception as e:
-        log.debug(e)
-        new_files = list(scanned_set)
+        left_mpv = MPV(ipc_socket=left_mpv_socket, geometry=f"{mpv_width}x{display.height}+0+0", **mpv_kwargs)
+        right_mpv = MPV(
+            ipc_socket=right_mpv_socket,
+            geometry=f"{mpv_width}x{display.height}+{mpv_width}+0",
+            **mpv_kwargs,
+        )
+
+        for x_mpv in (left_mpv, right_mpv):
+            x_mpv.volume = args.volume
+            x_mpv.command("script-message", "osc-visibility", "always")  # , "no-osd"
+
+            @x_mpv.on_key_press("k")
+            def keep_handler():
+                print("keep")
+
+            @x_mpv.on_key_press("d")
+            def delete_handler():
+                print("delete")
+
+        left_mpv.play(left_side)
+        right_mpv.play(right_side)
+
+        def right_quit_callback():
+            try:
+                left_mpv.command("quit")
+            except BrokenPipeError:
+                pass
+
+        left_mpv.quit_callback = right_mpv.terminate
+        right_mpv.quit_callback = right_quit_callback  # they can't both be the same
+
+        with ThreadPoolExecutor() as e:
+            e.submit(mpv_utils.auto_seek, left_mpv)
+            e.submit(mpv_utils.auto_seek, right_mpv, delay=0.4)
+
     else:
-        new_files = list(scanned_set - existing_set)
+        mpv_options = [
+            "--save-position-on-quit=no",
+            "--no-resume-playback",
+            "--image-display-duration=inf",
+            "--script-opts=osc-visibility=always",
+            f"--start={args.start}",
+            f"--volume={args.volume}",
+        ]
+
+        left_mpv_process = subprocess.Popen(
+            [
+                "mpv",
+                left_side,
+                f"--input-ipc-server={left_mpv_socket}",
+                f"--geometry={mpv_width}x{display.height}+0+0",
+                *mpv_options,
+            ],
+            stdout=subprocess.DEVNULL,
+            stderr=subprocess.DEVNULL,
+        )
+        right_mpv_process = subprocess.Popen(
+            [
+                "mpv",
+                right_side,
+                f"--input-ipc-server={right_mpv_socket}",
+                f"--geometry={mpv_width}x{display.height}+{mpv_width}+0",
+                *mpv_options,
+            ],
+            stdout=subprocess.DEVNULL,
+            stderr=subprocess.DEVNULL,
+        )
+
+        # if not all([Path(left_side).exists(), Path(right_side).exists()]):
+        #     return  # race condition
+
+        while True:  # Monitor the processes and terminate the other one when one finishes
+            if left_mpv_process.poll() is not None or right_mpv_process.poll() is not None:
+                break
+            time.sleep(0.1)
+
+        # Terminate the other process
+        if left_mpv_process.poll() is None:
+            left_mpv_process.terminate()
+        if right_mpv_process.poll() is None:
+            right_mpv_process.terminate()
+
+
+def mv_to_keep_folder(args, d) -> None:
+    keep_path = Path(args.keep_dir)
+    keep_path.mkdir(exist_ok=True)
 
-        deleted_files = list(existing_set - scanned_set)
-        if not scanned_set and len(deleted_files) >= len(existing_set) and not args.force:
-            print(f"[{path}] Path empty or device not mounted. Rerun with -f to mark all subpaths as deleted.")
-            return []  # if path not mounted or all files deleted
-        deleted_count = db_media.mark_media_deleted(args, deleted_files)
-        if deleted_count > 0:
-            print(f"[{path}] Marking", deleted_count, "orphaned metadata records as deleted")
-
-    new_files.sort(key=len, reverse=True)
-    return new_files
-
-
-def scan_path(args, path_str: str) -> int:
-    path = Path(path_str).expanduser().resolve()
-    if not path.exists():
-        print(f"[{path}] Path does not exist")
-        if args.force:
-            playlists.delete_playlists(args, [str(path)])
-        return 0
-
-    n_jobs = None
-    if args.verbose >= consts.LOG_DEBUG:
-        n_jobs = 1
-    elif args.io_multiplier != 1.0:
-        n_jobs = max(1, int(max(os.cpu_count() or 4, 4) * args.io_multiplier))
-
-    threadsafe = [DBType.audio, DBType.video, DBType.filesystem]
-
-    info = {
-        "extractor_key": "Local",
-        "extractor_config": objects.dict_filter_bool(
-            {k: v for k, v in args.__dict__.items() if k not in ["db", "database", "verbose", "force", "paths"]}
-        ),
-        "time_deleted": 0,
-    }
-    args.playlists_id = db_playlists.add(args, str(path), info, check_subpath=True)
-
-    print(f"[{path}] Building file list...")
-    new_files = find_new_files(args, path)
-    if new_files:
-        print(f"[{path}] Adding {len(new_files)} new media")
-        # log.debug(new_files)
-
-        if DBType.text in args.profiles:
-            batch_count = int(os.cpu_count() or 4)
-        elif DBType.image in args.profiles:
-            batch_count = consts.SQLITE_PARAM_LIMIT // 20
-        else:
-            batch_count = consts.SQLITE_PARAM_LIMIT // 100
-        chunks_count = math.ceil(len(new_files) / batch_count)
-        files_chunked = iterables.chunks(new_files, batch_count)
+    media_file = d["path"]
 
-        if all(s in threadsafe for s in args.profiles):
-            pool_fn = ThreadPoolExecutor
+    try:
+        new_path = shutil.move(media_file, keep_path)
+    except FileNotFoundError:
+        return
+    except shutil.Error as e:
+        if "already exists" not in str(e):
+            raise
+        p = Path(media_file)
+        new_path = Path(keep_path) / p.name
+
+        src_size = d["size"]
+        dst_size = new_path.stat().st_size
+        diff_size = humanize.naturalsize(src_size - dst_size, binary=True)
+
+        if src_size > dst_size:
+            print("Source is larger than destination", diff_size)
+        elif src_size < dst_size:
+            print("Source is smaller than destination", diff_size)
         else:
-            pool_fn = ProcessPoolExecutor
-
-        with pool_fn(n_jobs) as parallel:
-            for idx, chunk_paths in enumerate(files_chunked):
-                percent = ((batch_count * idx) + len(chunk_paths)) / len(new_files) * 100
-                print(f"[{path}] Extracting metadata {percent:3.1f}% (chunk {idx + 1} of {chunks_count})")
-
-                mp_args = argparse.Namespace(
-                    playlist_path=path, **{k: v for k, v in args.__dict__.items() if k not in {"db"}}
-                )
-                metadata = parallel.map(partial(extract_metadata, mp_args), chunk_paths)
-                metadata = list(filter(None, metadata))
-                extract_chunk(args, metadata)
-
-    return len(new_files)
-
-
-def extractor(args, paths) -> None:
-    new_files = 0
-    for path in paths:
-        new_files += scan_path(args, path)
-
-    log.info("Imported %s paths", new_files)
-
-    if not args.db["media"].detect_fts() or new_files > 100000:
-        db_utils.optimize(args)
-
-
-def fs_add(args=None) -> None:
-    if args:
-        sys.argv = ["lb", *args]
-
-    args, _parser = parse_args(SC.fsadd, usage.fsadd)
-    extractor(args, args.paths)
-
-
-def fs_update(args=None) -> None:
-    if args:
-        sys.argv = ["lb", *args]
-
-    args, parser = parse_args(SC.fsupdate, usage.fsupdate)
-
-    fs_playlists = list(
-        args.db.query(
-            f"""
-            SELECT *
-            FROM playlists
-            WHERE extractor_key = 'Local'
-            ORDER BY
-                length(path)-length(REPLACE(path, '{os.sep}', '')) desc
-                , path
-            """,
-        ),
-    )
-
-    for playlist in fs_playlists:
-        extractor_config = json.loads(playlist.get("extractor_config") or "{}")
-        args_env = arg_utils.override_config(parser, extractor_config, args)
-
-        extractor(args_env, [playlist["path"]])
+            print("Source and destination are the same size", humanize.naturalsize(src_size, binary=True))
+        if devices.confirm("Replace destination file?"):
+            file_utils.trash(args, new_path, detach=False)
+            new_path = shutil.move(media_file, keep_path)
+
+    log.info(f"{new_path}: new location")
+
+
+def group_and_delete(args, groups):
+    is_interactive = not any([args.all_keep, args.all_left, args.all_right, args.all_delete])
+
+    for group_content in groups:
+        if group_content == "":
+            continue
+
+        group = extract_group_data(group_content)
+        if group is None:
+            continue
+
+        def delete_dupe(d, detach=is_interactive):
+            file_utils.trash(args, d["path"], detach=detach)
+            log.info(f"{d['path']}: Deleted")
+
+        group.sort(key=lambda x: x["size"], reverse=True)
+        left = group[0]
+
+        dups = group[1:]
+        kept_dups = []
+        while len(dups) > 0:
+            right = dups.pop()
+
+            if right["path"] == left["path"]:
+                continue
+
+            if not os.path.exists(right["path"]):
+                log.debug(f"{right['path']}: not found")
+                continue
+
+            if not os.path.exists(left["path"]):
+                log.debug(f"{left['path']}: not found")
+                left = right
+                continue
+
+            print(left["path"], humanize.naturalsize(left["size"], binary=True))
+            print(right["path"], humanize.naturalsize(right["size"], binary=True))
+
+            if args.auto_select_min_ratio < 1.0:
+                similar_ratio = difflib.SequenceMatcher(
+                    None,
+                    os.path.basename(left["path"]),
+                    os.path.basename(right["path"]),
+                ).ratio()
+                if similar_ratio >= args.auto_select_min_ratio or any(
+                    s in left["path"] and s in right["path"] for s in ["Goldmines_Bollywood"]
+                ):
+                    delete_dupe(right)
+                continue
+
+            if not is_interactive:
+                if args.all_left:
+                    kept_dups.append(left)
+                    delete_dupe(right)
+                elif args.all_right:
+                    kept_dups.append(right)
+                    delete_dupe(left)
+                    left = right
+                elif args.all_delete:
+                    delete_dupe(left)
+                    delete_dupe(right)
+                continue
+
+            is_next_iter_not_last = len(dups) > 1
+
+            if args.override_player:
+                for path in (left["path"], right["path"]):
+                    player_process = processes.cmd(*shlex.split(args.override_player), path, strict=False)
+                    if player_process.returncode == 0:
+                        post_actions.post_act(
+                            args,
+                            path,
+                            media_len=len(dups),
+                            record_history=False,
+                            player_process=player_process,
+                            action="ASK_MOVE_OR_DELETE" if args.keep_dir else "ASK_DELETE",
+                        )
+                    else:
+                        truncate_file_before_match(args.file_path, left["path"])
+                        processes.player_exit(player_process)
+            else:
+                side_by_side_mpv(args, left["path"], right["path"])
+                while True:
+                    devices.clear_input()
+                    user_input = (
+                        input("Keep which files? (l Left/r Right/k Keep both/d Delete both) [default: l]: ")
+                        .strip()
+                        .lower()
+                    )
+                    if args.all_keep or user_input in ("k", "keep"):
+                        kept_dups.append(left)
+                        kept_dups.append(right)
+                        break
+                    elif args.all_left or user_input in ("l", "left", ""):
+                        kept_dups.append(left)
+                        delete_dupe(right, detach=is_next_iter_not_last)
+                        break
+                    elif args.all_right or user_input in ("r", "right"):
+                        kept_dups.append(right)
+                        delete_dupe(left, detach=is_next_iter_not_last)
+                        break
+                    elif args.all_delete or user_input in ("d", "delete"):
+                        delete_dupe(right, detach=is_next_iter_not_last)
+                        delete_dupe(left, detach=is_next_iter_not_last)
+                        break
+                    elif user_input in ("q", "quit"):
+                        truncate_file_before_match(args.file_path, left["path"])
+                        sys.exit(0)
+                    else:
+                        print("Invalid input. Please type 'left', 'right', 'keep', 'delete', or 'quit' and enter")
+
+            if len(dups) > 1:
+                left = dups.pop()
+            elif len(dups) == 1 and len(kept_dups) > 0:
+                left = kept_dups[-1]
+
+        if args.keep_dir:
+            for d in iterables.list_dict_unique(kept_dups, ["path"]):
+                if os.path.exists(d["path"]):
+                    mv_to_keep_folder(args, d)
+
+        print()
+
+
+def czkawka_dedupe():
+    args = parse_args()
+
+    content = backup_and_read_file(args.file_path)
+    groups = extract_dupe_groups(content)
+    group_and_delete(args, groups)
```

### Comparing `xklb-2.6.7/xklb/gdl_backend.py` & `xklb-2.6.9/xklb/createdb/gallery_backend.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.7/xklb/gdl_extract.py` & `xklb-2.6.9/xklb/createdb/gallery_add.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import argparse, sys
 from pathlib import Path
 
-from xklb import db_media, db_playlists, gdl_backend, usage
+from xklb import db_media, db_playlists, usage
+from xklb.createdb import gallery_backend
 from xklb.utils import arggroups, argparse_utils, consts, db_utils, iterables, objects, path_utils, processes
 from xklb.utils.consts import SC
 from xklb.utils.log_utils import log
 
 
 def parse_args(action, usage) -> argparse.Namespace:
     parser = argparse.ArgumentParser(
@@ -16,23 +17,23 @@
     arggroups.extractor(parser)
     arggroups.download(parser)
     parser.set_defaults(download_archive=str(Path("~/.local/share/gallerydl.sqlite3").expanduser().resolve()))
 
     arggroups.debug(parser)
 
     arggroups.database(parser)
-    if action == SC.galleryadd:
+    if action == SC.gallery_add:
         parser.add_argument(
             "playlists", nargs="*", default=argparse_utils.STDIN_DASH, action=argparse_utils.ArgparseArgsOrStdin
         )
 
     args = parser.parse_intermixed_args()
     args.action = action
 
-    if action == SC.galleryadd:
+    if action == SC.gallery_add:
         Path(args.database).touch()
     args.db = db_utils.connect(args)
 
     if hasattr(args, "playlists"):
         args.playlists = list({s.strip() for s in args.playlists})
         if not args.no_sanitize:
             args.playlists = [path_utils.sanitize_url(args, p) for p in args.playlists]
@@ -45,15 +46,15 @@
     return args
 
 
 def gallery_add(args=None) -> None:
     if args:
         sys.argv = ["galleryadd", *args]
 
-    args = parse_args(SC.galleryadd, usage=usage.galleryadd)
+    args = parse_args(SC.gallery_add, usage=usage.gallery_add)
 
     if args.insert_only:
         args.db["media"].insert_all(
             [{"path": p, "time_created": consts.APPLICATION_START} for p in args.playlists],
             alter=True,
             ignore=True,
             pk="path",
@@ -71,29 +72,29 @@
             known_playlists = db_media.get_paths(args)
 
         for path in args.playlists:
             if path in known_playlists:
                 log.info("[%s]: Already added. Skipping!", path)
                 continue
 
-            if args.safe and not gdl_backend.is_supported(args, path):
+            if args.safe and not gallery_backend.is_supported(args, path):
                 log.info("[%s]: Skipping unsupported playlist (safe_mode)", path)
                 continue
 
-            gdl_backend.get_playlist_metadata(args, path)
+            gallery_backend.get_playlist_metadata(args, path)
 
     if not args.db["media"].detect_fts():
         db_utils.optimize(args)
 
 
 def gallery_update(args=None) -> None:
     if args:
         sys.argv = ["galleryupdate", *args]
 
-    args = parse_args(SC.galleryupdate, usage=usage.galleryupdate)
+    args = parse_args(SC.gallery_update, usage=usage.gallery_update)
 
     gdl_playlists = db_playlists.get_all(
         args,
         sql_filters=["AND extractor_key NOT IN ('Local', 'reddit_praw_redditor', 'reddit_praw_subreddit')"],
     )
     for d in gdl_playlists:
-        gdl_backend.get_playlist_metadata(args, d["path"])
+        gallery_backend.get_playlist_metadata(args, d["path"])
```

### Comparing `xklb-2.6.7/xklb/history.py` & `xklb-2.6.9/xklb/history.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.7/xklb/hn_extract.py` & `xklb-2.6.9/xklb/createdb/hn_add.py`

 * *Files 0% similar despite different names*

```diff
@@ -99,15 +99,15 @@
             task.add_done_callback(background_tasks.discard)
 
         for _i in range(N):
             await sem.acquire()
 
 
 def hacker_news_add() -> None:
-    args = parse_args(prog="library hnadd", usage=usage.hnadd)
+    args = parse_args(prog="library hnadd", usage=usage.hn_add)
     try:
         import aiohttp
     except ModuleNotFoundError:
         log.error("aiohttp is required for hn_extract. Install with pip install aiohttp or pip install xklb[deluxe]")
         raise
 
     args.db.enable_wal()
```

### Comparing `xklb-2.6.7/xklb/lb.py` & `xklb-2.6.9/xklb/lb.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,34 +4,34 @@
 
 from xklb import __version__
 from xklb.utils import iterables
 from xklb.utils.log_utils import log
 
 progs = {
     "Create database subcommands": {
-        "fsadd": "Add local media",
-        "tubeadd": "Add online video media (yt-dlp)",
-        "webadd": "Add open-directory media",
-        "galleryadd": "Add online gallery media (gallery-dl)",
-        "tabsadd": "Create a tabs database; Add URLs",
+        "fs_add": "Add local media",
+        "tube_add": "Add online video media (yt-dlp)",
+        "web_add": "Add open-directory media",
+        "gallery_add": "Add online gallery media (gallery-dl)",
+        "tabs_add": "Create a tabs database; Add URLs",
         "links_add": "Create a link-scraping database",
-        "siteadd": "Auto-scrape website data to SQLITE",
-        "redditadd": "Create a reddit database; Add subreddits",
-        "pushshift": "Convert pushshift data to reddit.db format (stdin)",
-        "hnadd": "Create / Update a Hacker News database",
+        "site_add": "Auto-scrape website data to SQLITE",
+        "reddit_add": "Create a reddit database; Add subreddits",
+        "hn_add": "Create / Update a Hacker News database",
         "substack": "Backup substack articles",
         "tildes": "Backup tildes comments and topics",
         "places_import": "Import places of interest (POIs)",
-        "add_row": "Add arbitrary data to SQLITE",
+        "row_add": "Add arbitrary data to SQLITE",
     },
     "Text subcommands": {
         "cluster_sort": "Sort text and images by similarity",
         "extract_links": "Extract inner links from lists of web links",
         "extract_text": "Extract human text from lists of web links",
         "markdown_links": "Extract titles from lists of web links",
+        "nouns": "Unstructured text -> compound nouns (stdin)",
     },
     "Folder subcommands": {
         "merge_folders": "Merge two or more file trees",
         "relmv": "Move files preserving parent folder hierarchy",
         "mv_list": "Find specific folders to move to different disks",
         "scatter": "Scatter files between folders or disks",
     },
@@ -55,55 +55,55 @@
     },
     "Filesystem Database subcommands": {
         "christen": "Clean filenames",
         "disk_usage": "Show disk usage",
         "mount_stats": "Show some relative mount stats",
         "big_dirs": "Show large folders",
         "search_db": "Search a SQLITE database",
-        "optimize": "Re-optimize database",
     },
     "Media Database subcommands": {
-        "tabs": "Open your tabs for the day",
         "block": "Block a channel",
         "playlists": "List stored playlists",
         "download": "Download media",
         "download_status": "Show download status",
         "redownload": "Re-download deleted/lost media",
         "history": "Show some playback statistics",
         "search": "Search captions / subtitles",
+        "optimize": "Re-optimize database",
     },
     "Playback subcommands": {
         "watch": "Watch / Listen",
         "now": "Show what is currently playing",
         "next": "Play next file and optionally delete current file",
         "stop": "Stop all playback",
         "pause": "Pause all playback",
-        "open_links": "Open links from link dbs",
+        "tabs_open": "Open your tabs for the day",
+        "links_open": "Open links from link dbs",
         "surf": "Auto-load browser tabs in a streaming way (stdin)",
     },
     "Database enrichment subcommands": {
         "dedupe_db": "Dedupe SQLITE tables",
         "dedupe_media": "Dedupe similar media",
         "merge_online_local": "Merge online and local data",
         "mpv_watchlater": "Import mpv watchlater files to history",
         "reddit_selftext": "Copy selftext links to media table",
         "tabs_shuffle": "Randomize tabs.db a bit",
+        "pushshift": "Convert pushshift data to reddit.db format (stdin)",
     },
     "Update database subcommands": {
-        "fsupdate": "Update local media",
-        "tubeupdate": "Update online video media",
-        "webupdate": "Update open-directory media",
-        "galleryupdate": "Update online gallery media",
+        "fs_update": "Update local media",
+        "tube_update": "Update online video media",
+        "web_update": "Update open-directory media",
+        "gallery_update": "Update online gallery media",
         "links_update": "Update a link-scraping database",
-        "redditupdate": "Update reddit media",
+        "reddit_update": "Update reddit media",
     },
     "Misc subcommands": {
         "export_text": "Export HTML files from SQLite databases",
         "dedupe_czkawka": "Process czkawka diff output",
-        "nouns": "Unstructured text -> compound nouns (stdin)",
     },
 }
 
 
 def usage() -> str:
     subcommands_list = []
     for category, category_progs in progs.items():
@@ -166,86 +166,86 @@
 
         aliases += consecutive_prefixes(name) + iterables.conform([consecutive_prefixes(a) for a in aliases])
         subp = subparsers.add_parser(name, aliases=aliases, add_help=False)
 
         set_func(subp, module_name, function_name)
         return subp
 
-    add_parser(subparsers, "xklb.dl_extract.dl_download", ["dl", "download"])
-    add_parser(subparsers, "xklb.fs_extract.fs_add", ["x", "extract"])
-    add_parser(subparsers, "xklb.fs_extract.fs_update", ["xu"])
-    add_parser(subparsers, "xklb.gdl_extract.gallery_add", ["gdl-add", "ga"])
-    add_parser(subparsers, "xklb.gdl_extract.gallery_update", ["gdl-update", "gu"])
-    add_parser(subparsers, "xklb.hn_extract.hacker_news_add", ["hn-add"])
-    add_parser(subparsers, "xklb.media.dedupe.dedupe_media")
-    add_parser(subparsers, "xklb.media.media_check.media_check")
-    add_parser(subparsers, "xklb.play_actions.filesystem", ["fs", "open"])
-    add_parser(subparsers, "xklb.play_actions.listen", ["lt", "tubelisten", "tl"])
-    add_parser(subparsers, "xklb.play_actions.read", ["books", "docs"])
-    add_parser(subparsers, "xklb.play_actions.view", ["image", "see", "look"])
-    add_parser(subparsers, "xklb.play_actions.watch", ["wt", "tubewatch", "tw", "entries"])
-    add_parser(subparsers, "xklb.reddit_extract.reddit_add", ["ra"])
-    add_parser(subparsers, "xklb.reddit_extract.reddit_update", ["ru"])
-    add_parser(subparsers, "xklb.scripts.add_row.add_row")
-    add_parser(subparsers, "xklb.scripts.big_dirs.big_dirs", ["large-folders"])
-    add_parser(subparsers, "xklb.scripts.block.block")
-    add_parser(subparsers, "xklb.scripts.christen.christen")
-    add_parser(subparsers, "xklb.scripts.cluster_sort.cluster_sort", ["cs"])
-    add_parser(subparsers, "xklb.scripts.copy_play_counts.copy_play_counts")
-    add_parser(subparsers, "xklb.scripts.dedupe_czkawka.czkawka_dedupe", ["dedupe-czkawka"])
-    add_parser(subparsers, "xklb.scripts.dedupe_db.dedupe_db", ["dedupe-dbs"])
-    add_parser(subparsers, "xklb.scripts.disk_usage.disk_usage", ["du", "usage"])
-    add_parser(subparsers, "xklb.scripts.download_status.download_status", ["ds", "dl-status"])
-    add_parser(subparsers, "xklb.scripts.eda.eda", ["preview"])
-    add_parser(subparsers, "xklb.scripts.export_text.export_text")
-    add_parser(subparsers, "xklb.scripts.history.history", ["hi", "log"])
-    add_parser(subparsers, "xklb.scripts.incremental_diff.incremental_diff")
-    add_parser(subparsers, "xklb.scripts.links_db.links_add", ["links-db"])
-    add_parser(subparsers, "xklb.scripts.links_db.links_update")
-    add_parser(subparsers, "xklb.scripts.mcda.mcda", ["mcdm", "rank"])
-    add_parser(subparsers, "xklb.scripts.merge_dbs.merge_dbs", ["merge-db"])
-    add_parser(subparsers, "xklb.scripts.merge_folders.merge_folders", ["merge-folder", "mv"])
-    add_parser(subparsers, "xklb.scripts.merge_online_local.merge_online_local")
-    add_parser(subparsers, "xklb.scripts.mining.extract_links.extract_links", ["links", "links_extract"])
-    add_parser(subparsers, "xklb.scripts.mining.extract_text.extract_text", ["text", "text_extract"])
-    add_parser(subparsers, "xklb.scripts.mining.markdown_links.markdown_links", ["markdown-urls"])
-    add_parser(subparsers, "xklb.scripts.mining.mpv_watchlater.mpv_watchlater")
-    add_parser(subparsers, "xklb.scripts.mining.nouns.nouns", ["nouns"])
-    add_parser(subparsers, "xklb.scripts.mining.pushshift.pushshift_extract", ["pushshift"])
-    add_parser(subparsers, "xklb.scripts.mining.reddit_selftext.reddit_selftext")
-    add_parser(subparsers, "xklb.scripts.mining.substack.substack")
-    add_parser(subparsers, "xklb.scripts.mining.tildes.tildes")
-    add_parser(subparsers, "xklb.scripts.move_list.move_list", ["mv-list"])
-    add_parser(subparsers, "xklb.scripts.open_links.open_links", ["links-open"])
-    add_parser(subparsers, "xklb.scripts.optimize_db.optimize_db", ["optimize"])
-    add_parser(subparsers, "xklb.scripts.places_import.places_import")
-    add_parser(subparsers, "xklb.scripts.playback_control.playback_next", ["next"])
-    add_parser(subparsers, "xklb.scripts.playback_control.playback_now", ["now"])
-    add_parser(subparsers, "xklb.scripts.playback_control.playback_pause", ["pause", "play"])
-    add_parser(subparsers, "xklb.scripts.playback_control.playback_stop", ["stop"])
-    add_parser(subparsers, "xklb.scripts.playlists.playlists", ["pl", "folders"])
-    add_parser(subparsers, "xklb.scripts.process_ffmpeg.process_ffmpeg", ["process-video", "process-audio"])
-    add_parser(subparsers, "xklb.scripts.process_image.process_image")
-    add_parser(subparsers, "xklb.scripts.redownload.redownload", ["re-dl", "re-download"])
-    add_parser(subparsers, "xklb.scripts.rel_mv.rel_mv", ["relmv", "mv-rel", "mvrel"])
-    add_parser(subparsers, "xklb.scripts.sample_hash.sample_hash", ["hash", "hash-file"])
-    add_parser(subparsers, "xklb.scripts.sample_compare.sample_compare", ["cmp"])
-    add_parser(subparsers, "xklb.scripts.scatter.scatter")
-    add_parser(subparsers, "xklb.scripts.search_db.search_db", ["s", "sdb", "search-dbs"])
-    add_parser(subparsers, "xklb.scripts.streaming_tab_loader.streaming_tab_loader", ["surf"])
-    add_parser(subparsers, "xklb.scripts.web_add.web_add", ["web-dir-add"])
-    add_parser(subparsers, "xklb.scripts.web_update.web_update", ["web-dir-update"])
-    add_parser(subparsers, "xklb.search.search", ["sc", "search-captions"])
-    add_parser(subparsers, "xklb.site_extract.site_add", ["sa", "sql-site", "site-sql"])
-    add_parser(subparsers, "xklb.tabs_actions.tabs", ["tb"])
-    add_parser(subparsers, "xklb.tabs_extract.tabs_add")
-    add_parser(subparsers, "xklb.tabs_extract.tabs_shuffle")
-    add_parser(subparsers, "xklb.tube_extract.tube_add", ["ta", "dladd", "da"])
-    add_parser(subparsers, "xklb.tube_extract.tube_update", ["dlupdate", "tu"])
-    add_parser(subparsers, "xklb.utils.devices.mount_stats", ["mu", "mount-usage"])
+    add_parser(subparsers, "xklb.createdb.fs_add.fs_add", ["x", "extract"])
+    add_parser(subparsers, "xklb.createdb.fs_add.fs_update", ["xu"])
+    add_parser(subparsers, "xklb.createdb.gallery_add.gallery_add", ["gdl-add", "ga"])
+    add_parser(subparsers, "xklb.createdb.gallery_add.gallery_update", ["gdl-update", "gu"])
+    add_parser(subparsers, "xklb.createdb.hn_add.hacker_news_add", ["hn-add"])
+    add_parser(subparsers, "xklb.createdb.links_add.links_add", ["links-db"])
+    add_parser(subparsers, "xklb.createdb.links_add.links_update")
+    add_parser(subparsers, "xklb.createdb.places_import.places_import")
+    add_parser(subparsers, "xklb.createdb.reddit_add.reddit_add", ["ra"])
+    add_parser(subparsers, "xklb.createdb.reddit_add.reddit_update", ["ru"])
+    add_parser(subparsers, "xklb.createdb.row_add.row_add", ["add_row"])
+    add_parser(subparsers, "xklb.createdb.site_add.site_add", ["sa", "sql-site", "site-sql"])
+    add_parser(subparsers, "xklb.createdb.substack.substack")
+    add_parser(subparsers, "xklb.createdb.tabs_add.tabs_add")
+    add_parser(subparsers, "xklb.createdb.tabs_add.tabs_shuffle")
+    add_parser(subparsers, "xklb.createdb.tildes.tildes")
+    add_parser(subparsers, "xklb.createdb.tube_add.tube_add", ["ta", "dladd", "da"])
+    add_parser(subparsers, "xklb.createdb.tube_add.tube_update", ["dlupdate", "tu"])
+    add_parser(subparsers, "xklb.createdb.web_add.web_add", ["web-dir-add"])
+    add_parser(subparsers, "xklb.createdb.web_add.web_update", ["web-dir-update"])
+    add_parser(subparsers, "xklb.editdb.dedupe_db.dedupe_db", ["dedupe-dbs"])
+    add_parser(subparsers, "xklb.editdb.dedupe_media.dedupe_media")
+    add_parser(subparsers, "xklb.editdb.merge_online_local.merge_online_local")
+    add_parser(subparsers, "xklb.editdb.mpv_watchlater.mpv_watchlater")
+    add_parser(subparsers, "xklb.editdb.pushshift.pushshift_extract", ["pushshift"])
+    add_parser(subparsers, "xklb.editdb.reddit_selftext.reddit_selftext")
+    add_parser(subparsers, "xklb.files.sample_compare.sample_compare", ["cmp"])
+    add_parser(subparsers, "xklb.files.sample_hash.sample_hash", ["hash", "hash-file"])
+    add_parser(subparsers, "xklb.folders.merge_folders.merge_folders", ["merge-folder", "mv"])
+    add_parser(subparsers, "xklb.folders.move_list.move_list", ["mv-list"])
+    add_parser(subparsers, "xklb.folders.rel_mv.rel_mv", ["relmv", "mv-rel", "mvrel"])
+    add_parser(subparsers, "xklb.folders.scatter.scatter")
+    add_parser(subparsers, "xklb.fsdb.big_dirs.big_dirs", ["large-folders"])
+    add_parser(subparsers, "xklb.fsdb.christen.christen")
+    add_parser(subparsers, "xklb.fsdb.disk_usage.disk_usage", ["du", "usage"])
+    add_parser(subparsers, "xklb.fsdb.mount_stats.mount_stats", ["mu", "mount-usage"])
+    add_parser(subparsers, "xklb.fsdb.search_db.search_db", ["s", "sdb", "search-dbs"])
+    add_parser(subparsers, "xklb.mediadb.block.block")
+    add_parser(subparsers, "xklb.mediadb.download.dl_download", ["dl", "download"])
+    add_parser(subparsers, "xklb.mediadb.download_status.download_status", ["ds", "dl-status"])
+    add_parser(subparsers, "xklb.mediadb.history.history", ["hi", "log"])
+    add_parser(subparsers, "xklb.mediadb.optimize_db.optimize_db", ["optimize"])
+    add_parser(subparsers, "xklb.mediadb.playlists.playlists", ["pl", "folders"])
+    add_parser(subparsers, "xklb.mediadb.redownload.redownload", ["re-dl", "re-download"])
+    add_parser(subparsers, "xklb.mediadb.search.search", ["sc", "search-captions"])
+    add_parser(subparsers, "xklb.mediafiles.media_check.media_check")
+    add_parser(subparsers, "xklb.mediafiles.process_ffmpeg.process_ffmpeg", ["process-video", "process-audio"])
+    add_parser(subparsers, "xklb.mediafiles.process_image.process_image")
+    add_parser(subparsers, "xklb.misc.dedupe_czkawka.czkawka_dedupe", ["dedupe-czkawka"])
+    add_parser(subparsers, "xklb.misc.export_text.export_text")
+    add_parser(subparsers, "xklb.multidb.copy_play_counts.copy_play_counts")
+    add_parser(subparsers, "xklb.multidb.merge_dbs.merge_dbs", ["merge-db"])
+    add_parser(subparsers, "xklb.playback.links_open.links_open", ["open-links"])
+    add_parser(subparsers, "xklb.playback.play_actions.filesystem", ["fs", "open"])
+    add_parser(subparsers, "xklb.playback.play_actions.listen", ["lt", "tubelisten", "tl"])
+    add_parser(subparsers, "xklb.playback.play_actions.read", ["books", "docs"])
+    add_parser(subparsers, "xklb.playback.play_actions.view", ["image", "see", "look"])
+    add_parser(subparsers, "xklb.playback.play_actions.watch", ["wt", "tubewatch", "tw", "entries"])
+    add_parser(subparsers, "xklb.playback.playback_control.playback_next", ["next"])
+    add_parser(subparsers, "xklb.playback.playback_control.playback_now", ["now"])
+    add_parser(subparsers, "xklb.playback.playback_control.playback_pause", ["pause", "play"])
+    add_parser(subparsers, "xklb.playback.playback_control.playback_stop", ["stop"])
+    add_parser(subparsers, "xklb.playback.surf.streaming_tab_loader", ["surf"])
+    add_parser(subparsers, "xklb.playback.tabs_open.tabs_open", ["tb", "tabs", "open_tabs"])
+    add_parser(subparsers, "xklb.tablefiles.eda.eda", ["preview"])
+    add_parser(subparsers, "xklb.tablefiles.incremental_diff.incremental_diff")
+    add_parser(subparsers, "xklb.tablefiles.mcda.mcda", ["mcdm", "rank"])
+    add_parser(subparsers, "xklb.text.cluster_sort.cluster_sort", ["cs"])
+    add_parser(subparsers, "xklb.text.extract_links.extract_links", ["links", "links_extract"])
+    add_parser(subparsers, "xklb.text.extract_text.extract_text", ["text", "text_extract"])
+    add_parser(subparsers, "xklb.text.markdown_links.markdown_links", ["markdown-urls"])
+    add_parser(subparsers, "xklb.text.nouns.nouns", ["nouns"])
 
     parser.add_argument("--version", "-V", action="store_true")
 
     return parser
 
 
 def library(args=None) -> None:
```

### Comparing `xklb-2.6.7/xklb/play_actions.py` & `xklb-2.6.9/xklb/playback/play_actions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import argparse, os, shlex, sys
 from pathlib import Path
 
-from xklb import db_media, history, tube_backend, usage
-from xklb.media import media_player, media_printer
-from xklb.scripts import big_dirs, mcda
+from xklb import db_media, history, media_printer, usage
+from xklb.createdb import tube_backend
+from xklb.fsdb import big_dirs
+from xklb.playback import media_player
+from xklb.tablefiles import mcda
 from xklb.utils import arggroups, consts, db_utils, devices, file_utils, iterables, nums, objects, processes, sql_utils
 from xklb.utils.arg_utils import parse_args_limit, parse_args_sort
 from xklb.utils.consts import SC
 from xklb.utils.log_utils import Timer, log
 
 
 def parse_args(action, default_chromecast=None) -> argparse.Namespace:
@@ -476,15 +478,15 @@
                         media.append(media_keyed[key])
             log.debug("double for loop compare_block_strings: %s", t.elapsed())
 
     if args.play_in_order:
         media = db_media.natsort_media(args, media)
 
     if args.cluster_sort:
-        from xklb.scripts.cluster_sort import cluster_dicts
+        from xklb.text.cluster_sort import cluster_dicts
 
         media = cluster_dicts(args, media)
         log.debug("cluster-sort: %s", t.elapsed())
 
     if getattr(args, "refresh", False):
         marked = db_media.mark_media_deleted(args, [d["path"] for d in media if not Path(d["path"]).exists()])
         log.warning(f"Marked {marked} metadata records as deleted")
```

### Comparing `xklb-2.6.7/xklb/post_actions.py` & `xklb-2.6.9/xklb/playback/post_actions.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.7/xklb/readme.py` & `xklb-2.6.9/xklb/readme.py`

 * *Files 0% similar despite different names*

```diff
@@ -117,15 +117,15 @@
     library tubeadd my.db $(xclip -selection c)
 
 #### 1a. Get new videos for saved playlists
 
 Tubeupdate will go through the list of added playlists and fetch metadata for
 any videos not previously seen.
 
-    library tubeupdate tube.db
+    library tube-update tube.db
 
 ### 2. Watch / Listen from websites
 
     library watch maker.db
 
 To stop playing press Ctrl+C in either the terminal or mpv
```

### Comparing `xklb-2.6.7/xklb/reddit_extract.py` & `xklb-2.6.9/xklb/createdb/reddit_add.py`

 * *Files identical despite different names*

```diff
@@ -291,15 +291,15 @@
 skip_errors = (prawcore.exceptions.NotFound, prawcore.exceptions.Forbidden, prawcore.exceptions.Redirect)
 
 
 def reddit_add(args=None) -> None:
     if args:
         sys.argv = ["lb", *args]
 
-    args = parse_args("redditadd", usage=usage.redditadd)
+    args = parse_args("reddit_add", usage=usage.reddit_add)
 
     for path in args.paths:
         path = path.lower()
         subreddit_matches = consts.REGEX_SUBREDDIT.match(path)
         redditor_matches = consts.REGEX_REDDITOR.match(path)
         extractor_key = "reddit_praw"
         name = path
@@ -348,15 +348,15 @@
         db_utils.optimize(args)
 
 
 def reddit_update(args=None) -> None:
     if args:
         sys.argv = ["lb", *args]
 
-    args = parse_args("redditupdate", usage=usage.redditupdate)
+    args = parse_args("reddit-update", usage=usage.reddit_update)
     reddit_playlists = db_playlists.get_all(
         args,
         "extractor_key, path, extractor_playlist_id, extractor_config",
         sql_filters=['AND extractor_key in ("reddit_praw_subreddit","reddit_praw_redditor")'],
     )
 
     for playlist in reddit_playlists:
```

### Comparing `xklb-2.6.7/xklb/rss_extract.py` & `xklb-2.6.9/xklb/createdb/rss_add.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.7/xklb/search.py` & `xklb-2.6.9/xklb/mediadb/search.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import argparse, textwrap
 from copy import deepcopy
 from itertools import groupby
 
-from xklb import db_media, usage
-from xklb.media import media_player, media_printer
+from xklb import db_media, media_printer, usage
+from xklb.playback import media_player
 from xklb.utils import arg_utils, arggroups, consts, db_utils, iterables, objects, printing, processes
 from xklb.utils.log_utils import log
 
 
 def parse_args() -> argparse.Namespace:
     parser = argparse.ArgumentParser(prog="library search", usage=usage.search)
 
@@ -20,20 +20,19 @@
 
     parser.add_argument("--open", "--play", action="store_true", help=argparse.SUPPRESS)
     parser.add_argument("--overlap", type=int, default=8, help=argparse.SUPPRESS)
     parser.add_argument("--table", action="store_true")
 
     parser.set_defaults(print="p")
 
-    parser.add_argument("--action", default="search", help=argparse.SUPPRESS)
-
     arggroups.debug(parser)
     arggroups.database(parser)
     parser.add_argument("search", nargs="*")
     args = parser.parse_intermixed_args()
+    args.action = "search"
 
     args.include += args.search
 
     if args.cols:
         args.cols = list(iterables.flatten([s.split(",") for s in args.cols]))
 
     sort = [arg_utils.override_sort(s) for s in args.sort]
```

### Comparing `xklb-2.6.7/xklb/site_extract.py` & `xklb-2.6.9/xklb/createdb/site_add.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from xklb import usage
 from xklb.utils import arg_utils, arggroups, consts, db_utils, iterables, objects, web
 from xklb.utils.log_utils import log
 
 
 def parse_args() -> argparse.Namespace:
-    parser = argparse.ArgumentParser(prog="library site-add", usage=usage.siteadd)
+    parser = argparse.ArgumentParser(prog="library site-add", usage=usage.site_add)
     arggroups.selenium(parser)
     parser.set_defaults(selenium=True)
 
     parser.add_argument("--local-file", "--local-html", action="store_true", help="Treat paths as Local HTML files")
 
     arggroups.debug(parser)
     arggroups.database(parser)
```

### Comparing `xklb-2.6.7/xklb/tabs_actions.py` & `xklb-2.6.9/xklb/playback/tabs_open.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 import argparse, math, webbrowser
 from pathlib import Path
 from time import sleep
 
-from xklb import history, usage
-from xklb.media import media_printer
+from xklb import history, media_printer, usage
 from xklb.utils import arg_utils, arggroups, consts, db_utils, iterables, objects, processes
 from xklb.utils.log_utils import log
 
 
 def parse_args(action) -> argparse.Namespace:
     parser = argparse.ArgumentParser(
         prog="library tabs",
         formatter_class=argparse.ArgumentDefaultsHelpFormatter,
-        usage=usage.tabs,
+        usage=usage.tabs_open,
     )
 
     arggroups.sql_fs(parser)
     arggroups.debug(parser)
 
     arggroups.database(parser)
     parser.add_argument("search", nargs="*")
@@ -151,23 +150,16 @@
         log.debug(f"freq_count {freq_count} / num_days {num_days} = num_tabs {num_tabs}")
 
         filtered_media.extend([m for m in media if m["frequency"] == freq][:num_tabs])
 
     return filtered_media
 
 
-def open_tabs(args, media):
-    for m in media:
-        play(args, m)
-        if len(media) >= consts.MANY_LINKS:
-            sleep(0.3)
-
-
-def tabs() -> None:
-    args = parse_args(consts.SC.tabs)
+def tabs_open() -> None:
+    args = parse_args(consts.SC.tabs_open)
     history.create(args)
 
     query, bindings = construct_tabs_query(args)
 
     if args.print:
         media_printer.printer(args, query, bindings)
         return
@@ -175,8 +167,11 @@
     media = list(args.db.query(query, bindings))
     if not media:
         processes.no_media_found()
 
     counts = args.db.execute("select frequency, count(*) from media group by 1").fetchall()
     media = frequency_filter(counts, media)
 
-    open_tabs(args, media)
+    for m in media:
+        play(args, m)
+        if len(media) >= consts.MANY_LINKS:
+            sleep(0.3)
```

### Comparing `xklb-2.6.7/xklb/tabs_extract.py` & `xklb-2.6.9/xklb/createdb/tabs_add.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from xklb import db_media, history, usage
 from xklb.utils import arggroups, consts, db_utils, iterables, objects, path_utils, strings
 from xklb.utils.log_utils import log
 
 
 def parse_args() -> argparse.Namespace:
-    parser = argparse.ArgumentParser(prog="library tabsadd", usage=usage.tabsadd)
+    parser = argparse.ArgumentParser(prog="library tabs-add", usage=usage.tabs_add)
     arggroups.extractor(parser)
     arggroups.frequency(parser)
 
     parser.add_argument("--category", "-c", help=argparse.SUPPRESS)
     parser.add_argument("--allow-immediate", action="store_true")
     arggroups.debug(parser)
     arggroups.database(parser)
```

### Comparing `xklb-2.6.7/xklb/tube_backend.py` & `xklb-2.6.9/xklb/createdb/tube_backend.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,21 +2,22 @@
 from copy import deepcopy
 from pathlib import Path
 from pprint import pprint
 from subprocess import CalledProcessError
 from types import ModuleType
 
 from xklb import db_media, db_playlists
+from xklb.createdb import subtitle
 from xklb.data.yt_dlp_errors import (
     prefix_unrecoverable_errors,
     yt_meaningless_errors,
     yt_recoverable_errors,
     yt_unrecoverable_errors,
 )
-from xklb.media import media_check, subtitle
+from xklb.mediafiles import media_check
 from xklb.utils import consts, db_utils, iterables, objects, path_utils, printing, sql_utils, strings
 from xklb.utils.consts import DBType
 from xklb.utils.log_utils import Timer, log
 
 yt_dlp = None
 yt_archive = set()
 
@@ -168,15 +169,15 @@
             if not pl and not args.safe:
                 log.warning("Logging undownloadable media")
                 db_playlists.save_undownloadable(args, playlist_path)
 
         if added_media_count > count_before_extract:
             sys.stdout.write("\n")
 
-        if args.action == consts.SC.tubeupdate:
+        if args.action == consts.SC.tube_update:
             if added_media_count > count_before_extract:
                 db_playlists.decrease_update_delay(args, playlist_path)
             else:
                 db_playlists.increase_update_delay(args, playlist_path)
 
 
 def yt_subs_config(args):
```

### Comparing `xklb-2.6.7/xklb/tube_extract.py` & `xklb-2.6.9/xklb/createdb/tube_add.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import argparse, sys
 from pathlib import Path
 
-from xklb import db_media, db_playlists, tube_backend, usage
+from xklb import db_media, db_playlists, usage
+from xklb.createdb import tube_backend
 from xklb.utils import arggroups, argparse_utils, consts, db_utils, iterables, objects, path_utils, processes
 from xklb.utils.consts import SC
 from xklb.utils.log_utils import log
 
 
 def parse_args(action, usage) -> argparse.Namespace:
     parser = argparse.ArgumentParser(
@@ -17,23 +18,23 @@
     arggroups.download(parser)
     arggroups.download_subtitle(parser)
     parser.set_defaults(download_archive=str(Path("~/.local/share/yt_archive.txt").expanduser().resolve()))
 
     arggroups.debug(parser)
 
     arggroups.database(parser)
-    if action == SC.tubeadd:
+    if action == SC.tube_add:
         parser.add_argument(
             "playlists", nargs="*", default=argparse_utils.STDIN_DASH, action=argparse_utils.ArgparseArgsOrStdin
         )
 
     args = parser.parse_intermixed_args()
     args.action = action
 
-    if action == SC.tubeadd:
+    if action == SC.tube_add:
         Path(args.database).touch()
     args.db = db_utils.connect(args)
 
     if hasattr(args, "playlists"):
         args.playlists = list({s.strip() for s in args.playlists})
         if not args.no_sanitize:
             args.playlists = [path_utils.sanitize_url(args, p) for p in args.playlists]
@@ -45,15 +46,15 @@
     return args
 
 
 def tube_add(args=None) -> None:
     if args:
         sys.argv = ["tubeadd", *args]
 
-    args = parse_args(SC.tubeadd, usage=usage.tubeadd)
+    args = parse_args(SC.tube_add, usage=usage.tube_add)
 
     if args.insert_only:
         args.db["media"].insert_all(
             [
                 {
                     "path": p,
                     "time_created": consts.APPLICATION_START,
@@ -97,15 +98,15 @@
         db_utils.optimize(args)
 
 
 def tube_update(args=None) -> None:
     if args:
         sys.argv = ["tubeupdate", *args]
 
-    args = parse_args(SC.tubeupdate, usage=usage.tubeupdate)
+    args = parse_args(SC.tube_update, usage=usage.tube_update)
     tube_playlists = db_playlists.get_all(
         args,
         sql_filters=["AND extractor_key NOT IN ('Local', 'reddit_praw_redditor', 'reddit_praw_subreddit')"],
     )
     for d in tube_playlists:
         tube_backend.get_playlist_metadata(
             args,
```

### Comparing `xklb-2.6.7/xklb/usage.py` & `xklb-2.6.9/xklb/usage.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,15 +86,15 @@
         183 ArchiveOrg
         187 Documentary
         237 PBS
         243 BBC
         ...
 """
 
-fsadd = """library fsadd [(--video) | --audio | --image |  --text | --filesystem] DATABASE PATH ...
+fs_add = """library fs-add [(--video) | --audio | --image |  --text | --filesystem] DATABASE PATH ...
 
     The default database type is video:
         library fsadd tv.db ./tv/
         library fsadd --video tv.db ./tv/  # equivalent
 
     You can also create audio databases. Both audio and video use ffmpeg to read metadata:
         library fsadd --audio audio.db ./music/
@@ -135,27 +135,27 @@
 
     Move files on import
 
         library fsadd audio.db --move ~/library/ ./added_folder/
         This will run destination paths through `library christen` and move files relative to the added folder root
 """
 
-fsupdate = """library fsupdate DATABASE
+fs_update = """library fs-update DATABASE
 
     Update each path previously saved:
 
         library fsupdate video.db
 """
 
 places_import = """library places-import DATABASE PATH ...
 
     Load POIs from Google Maps Google Takeout
 """
 
-hnadd = """library hnadd [--oldest] DATABASE
+hn_add = """library hn-add [--oldest] DATABASE
 
     Fetch latest stories first:
 
         library hnadd hn.db -v
         Fetching 154873 items (33212696 to 33367569)
         Saving comment 33367568
         Saving comment 33367543
@@ -190,16 +190,14 @@
     Control playback:
         To stop playback press Ctrl-C in either the terminal or mpv
 
         Create global shortcuts in your desktop environment by sending commands to mpv_socket:
         echo 'playlist-next force' | socat - /tmp/mpv_socket
 
     Override the default player (mpv):
-        library does a lot of things to try to automatically use your preferred media player
-        but if it doesn't guess right you can make it explicit:
         library {action} --player "vlc --vlc-opts"
 
     Cast to chromecast groups:
         library {action} --cast --cast-to "Office pair"
         library {action} -ct "Office pair"  # equivalent
         If you don't know the exact name of your chromecast group run `catt scan`
 
@@ -564,15 +562,15 @@
 
 """
 
 
 watch = play("watch")
 
 
-redditadd = """library redditadd [--lookback N_DAYS] [--praw-site bot1] DATABASE URLS ...
+reddit_add = """library reddit-add [--lookback N_DAYS] [--praw-site bot1] DATABASE URLS ...
 
     Fetch data for redditors and reddits:
 
         library redditadd interesting.db https://old.reddit.com/r/coolgithubprojects/ https://old.reddit.com/user/Diastro
 
     If you have a file with a list of subreddits you can do this:
 
@@ -584,15 +582,15 @@
 
     Note that reddit's API is limited to 1000 posts and it usually doesn't go back very far historically.
     Also, it may be the case that reddit's API (praw) will stop working in the near future. For both of these problems
     my suggestion is to use pushshift data.
     You can find more info here: https://github.com/chapmanjacobd/reddit_mining#how-was-this-made
 """
 
-redditupdate = """library redditupdate [--audio | --video] [--lookback N_DAYS] [--praw-site bot1] DATABASE
+reddit_update = """library reddit-update [--audio | --video] [--lookback N_DAYS] [--praw-site bot1] DATABASE
 
     Fetch the latest posts for every subreddit/redditor saved in your database
 
         library redditupdate edu_subreddits.db
 """
 
 search = """library search DATABASE QUERY
@@ -814,15 +812,15 @@
         ╘═════════════╧══════════════════╧════════════════════╧══════════╛
 
     Simulate --safe flag
 
         library download-status video.db --safe
 """
 
-tabs = """library tabs DATABASE
+tabs_open = """library tabs-open DATABASE
 
     Tabs is meant to run **once per day**. Here is how you would configure it with `crontab`:
 
         45 9 * * * DISPLAY=:0 library tabs /home/my/tabs.db
 
     If things aren't working you can use `at` to simulate a similar environment as `cron`
 
@@ -881,15 +879,15 @@
         │ p/?sort=top&t=year                    │             │              │
         ├───────────────────────────────────────┼─────────────┼──────────────┤
         │ https://old.reddit.com/r/Cyberpunk/to │ yearly      │ Aug 29 2023  │
         │ p/?sort=top&t=year                    │             │              │
         ╘═══════════════════════════════════════╧═════════════╧══════════════╛
 """
 
-tabsadd = r"""library tabsadd [--frequency daily weekly (monthly) quarterly yearly] [--no-sanitize] DATABASE URLS ...
+tabs_add = r"""library tabs-add [--frequency daily weekly (monthly) quarterly yearly] [--no-sanitize] DATABASE URLS ...
 
     Adding one URL:
 
         library tabsadd -f daily tabs.db https://wiby.me/surprise/
 
         Depending on your shell you may need to escape the URL (add quotes)
 
@@ -912,15 +910,15 @@
     It may also be useful to shuffle monthly tabs, etc. You can accomplish this like so:
 
         library tabs-shuffle tabs.db -d  31 -f monthly
         library tabs-shuffle tabs.db -d  90 -f quarterly
         library tabs-shuffle tabs.db -d 365 -f yearly
 """
 
-tubeadd = r"""library tubeadd [--safe] [--extra] [--subs] [--auto-subs] DATABASE URLS ...
+tube_add = r"""library tube-add [--safe] [--extra] [--subs] [--auto-subs] DATABASE URLS ...
 
     Create a dl database / add links to an existing database
 
         library tubeadd dl.db https://www.youdl.com/c/BranchEducation/videos
 
     Add links from a line-delimited file
 
@@ -932,18 +930,18 @@
 
     Fetch extra metadata:
 
         By default tubeadd will quickly add media at the expense of less metadata.
         If you plan on using `library download` then it doesn't make sense to use `--extra`.
         Downloading will add the extra metadata automatically to the database.
         You can always fetch more metadata later via tubeupdate:
-        library tubeupdate tw.db --extra
+        library tube-update tw.db --extra
 """
 
-tubeupdate = """library tubeupdate [--audio | --video] DATABASE
+tube_update = """library tube-update [--audio | --video] DATABASE
 
     Fetch the latest videos for every playlist saved in your database
 
         library tubeupdate educational.db
 
     Fetch extra metadata:
 
@@ -953,24 +951,24 @@
         library tubeupdate educational.db --extra https://www.youtube.com/channel/UCBsEUcR-ezAuxB2WlfeENvA/videos
 
     Remove duplicate playlists:
 
         lb dedupe-db video.db playlists --bk extractor_playlist_id
 """
 
-galleryadd = """library galleryadd DATABASE URLS
+gallery_add = """library gallery-add DATABASE URLS
 
     Add gallery_dl URLs to download later or periodically update
 
     If you have many URLs use stdin
 
         cat ./my-favorite-manhwa.txt | library galleryadd your.db --insert-only -
 """
 
-galleryupdate = """library galleryupdate DATABASE URLS
+gallery_update = """library gallery-update DATABASE URLS
 
     Check previously saved gallery_dl URLs for new content
 """
 
 big_dirs = """library big-dirs DATABASE [--limit (4000)] [--depth (0)] [--sort-groups-by deleted | played] [--size=+5MB]
 
     See what folders take up space
@@ -1102,14 +1100,21 @@
         library dedupe-media video.db --duration --basename -u 'm1.size desc'  # sort such that large files are treated as originals and smaller files are deleted
 
     Dedupe online against local media
 
         library dedupe-media video.db / http
 """
 
+dedupe_czkawka = """library dedupe-czkawka [--volume VOLUME] [--auto-seek] [--ignore-errors] [--folder] [--folder-glob [FOLDER_GLOB]] [--replace] [--no-replace] [--override-trash OVERRIDE_TRASH] [--delete-files] [--gui]
+               [--auto-select-min-ratio AUTO_SELECT_MIN_RATIO] [--all-keep] [--all-left] [--all-right] [--all-delete] [--verbose]
+               czkawka_dupes_output_path
+
+    Choose which duplicate to keep by opening both side-by-side in mpv
+"""
+
 dedupe_db = """library dedupe-dbs DATABASE TABLE --bk BUSINESS_KEYS [--pk PRIMARY_KEYS] [--only-columns COLUMNS]
 
     Dedupe your database (not to be confused with the dedupe subcommand)
 
     It should not need to be said but *backup* your database before trying this tool!
 
     Dedupe-DB will help remove duplicate rows based on non-primary-key business keys
@@ -1150,15 +1155,15 @@
         library merge-dbs --pk id --only-tables subreddits reddit/81_New_Music.db audio.db
         library merge-dbs --only-new-rows --pk subreddit,path --only-tables reddit_posts reddit/81_New_Music.db audio.db -v
 
      To skip copying primary-keys from the source table(s) use --business-keys instead of --primary-keys
 
      Split DBs using --where
 
-         library merge-dbs --pk path specific-site.db big.db -v --only-new-rows -t media,playlists -w 'path like "https://specific-site%"'
+         library merge-dbs --pk path specific-site.db big.db -v --only-new-rows -t media,playlists -w 'path like "https://specific-site%%"'
 """
 
 merge_folders = """library merge-folders [--replace] [--no-replace] [--simulate] SOURCES ... DESTINATION
 
     Merge multiple folders with the same file tree into a single folder.
 
     https://github.com/chapmanjacobd/journal/blob/main/programming/linux/misconceptions.md#mv-src-vs-mv-src
@@ -1364,15 +1369,15 @@
         library scatter -m /mnt/d1:/mnt/d2 -l 100 -s 'time_modified desc' fs.db /
 
     Multi-device re-bin: empty out a disk (/mnt/d2) into many other disks (/mnt/d1, /mnt/d3, and /mnt/d4)
 
         library scatter fs.db -m /mnt/d1:/mnt/d3:/mnt/d4 /mnt/d2
 """
 
-open_links = """library open-links DATABASE [search] [--title] [--title-prefix TITLE_PREFIX]
+links_open = """library links-open DATABASE [search] [--title] [--title-prefix TITLE_PREFIX]
 
     Open links from a links db
 
         wget https://github.com/chapmanjacobd/library/raw/main/example_dbs/music.korea.ln.db
         library open-links music.korea.ln.db
 
     Only open links once
@@ -1669,15 +1674,15 @@
 extract_text = r"""library extract-text PATH ... [--skip-links]
 
     Sorting suggestions
 
         lb extract-text --skip-links --local-file (cb -t text/html | psub) | lb cs --groups | jq -r '.[] | .grouped_paths | "\n" + join("\n")'
 """
 
-siteadd = """library site-add DATABASE PATH ... [--auto-pager] [--poke] [--local-html] [--file FILE]
+site_add = """library site-add DATABASE PATH ... [--auto-pager] [--poke] [--local-html] [--file FILE]
 
     Extract data from website requests to a database
 
         library siteadd jobs.st.db --poke https://hk.jobsdb.com/hk/search-jobs/python/
 
     Run with `-vv` to see and interact with the browser
 """
@@ -1709,15 +1714,15 @@
     Calculate hashes for large files by reading only small segments of each file
 
         library sample-hash ./my_file.mkv
 
     The threads flag seems to be faster for rotational media but slower on SSDs
 """
 
-sample_compare = """library sample-hash [--threads 10] [--chunk-size BYTES] [--gap BYTES OR 0.0-1.0*FILESIZE] PATH ...
+sample_compare = """library sample-compare [--threads 10] [--chunk-size BYTES] [--gap BYTES OR 0.0-1.0*FILESIZE] PATH ...
 
     Convenience subcommand to compare multiple files using sample-hash
 """
 
 media_check = """library media-check [--chunk-size SECONDS] [--gap SECONDS OR 0.0-1.0*DURATION] [--delete-corrupt >0-100] [--full-scan] [--audio-scan] PATH ...
 
     Defaults to decode 0.5 second per 10%% of each file
@@ -1756,15 +1761,15 @@
     To scan a large folder use `fsadd`. I recommend something like this two-stage approach:
 
         library fsadd --delete-unplayable --check-corrupt --chunk-size 5%% tmp.db ./video/ ./folders/
         library media-check (library fs tmp.db -w 'corruption>15' -pf) --full-scan --delete-corrupt 25%%
 
     The above can now be done in one command via `--full-scan-if-corrupt`:
 
-        library fsadd --delete-unplayable --check-corrupt --chunk-size 5%% tmp.db ./video/ ./folders/ --full-scan-if-corrupt 15% --delete-corrupt 25%
+        library fsadd --delete-unplayable --check-corrupt --chunk-size 5%% tmp.db ./video/ ./folders/ --full-scan-if-corrupt 15%% --delete-corrupt 25%%
 
     Corruption stats
 
         library fs tmp.db -w 'corruption>15' -pa
         path         count  duration             avg_duration         size    avg_size
         ---------  -------  -------------------  --------------  ---------  ----------
         Aggregate      907  15 days and 9 hours  24 minutes      130.6 GiB   147.4 MiB
@@ -1784,15 +1789,15 @@
         [ 55.0 ..  64.0] [ 12] ∎∎
         [ 64.0 ..  73.0] [ 15] ∎∎
         [ 73.0 ..  82.0] [ 18] ∎∎∎
         [ 82.0 ..  91.0] [ 50] ∎∎∎∎∎∎∎∎
         [ 91.0 .. 100.0] [141] ∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎
 """
 
-webadd = """library web-add [(--filesystem) | --video | --audio | --image | --text] DATABASE URL ...
+web_add = """library web-add [(--filesystem) | --video | --audio | --image | --text] DATABASE URL ...
 
     Scan open directories
 
         library web-add open_dir.db --video http://1.1.1.1/
 
     Check download size of all videos matching some criteria
 
@@ -1833,24 +1838,44 @@
 
     Download checked videos
 
         library download --fs open_dir.db --prefix ~/d/dump/video/ -w 'id in (select media_id from history)'
 
 """
 
-webupdate = """library web-update DATABASE
+web_update = """library web-update DATABASE
 
     Update saved open directories
 
 """
 
-add_row = """library add-row DATABASE [--table-name TABLE_NAME]
+row_add = """library row-add DATABASE [--table-name TABLE_NAME]
 
     Add a row to sqlite
 
-        library add-row t.db --test_b 1 --test-a 2
+        library row-add t.db --test_b 1 --test-a 2
 
         ### media (1 rows)
         |   test_b |   test_a |
         |----------|----------|
         |        1 |        2 |
 """
+
+markdown_links = """usage: library markdown-links URL ... [--cookies COOKIES] [--cookies-from-browser BROWSER[+KEYRING][:PROFILE][::CONTAINER]] [--firefox] [--chrome] [--allow-insecure] [--scroll] [--manual] [--auto-pager] [--poke] [--file FILE]
+
+    Convert URLs into Markdown links with page titles filled in
+
+        $ lb markdown-links https://www.youtube.com/watch?v=IgZDDW-NXDE
+        [Work For Peace](https://www.youtube.com/watch?v=IgZDDW-NXDE)
+"""
+
+mount_stats = """library mount-stats MOUNTPOINT ...
+
+    Print relative use and free for multiple mount points
+"""
+
+nouns = """library nouns (stdin)
+
+    Extract compound nouns and phrases from unstructured mixed HTML plain text
+
+        xsv select text hn_comment_202210242109.csv | library nouns | sort | uniq -c | sort --numeric-sort
+"""
```

### Comparing `xklb-2.6.7/xklb/data/imagemagick_errors.py` & `xklb-2.6.9/xklb/data/imagemagick_errors.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.7/xklb/data/wordbank.py` & `xklb-2.6.9/xklb/data/wordbank.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.7/xklb/data/yt_dlp_errors.py` & `xklb-2.6.9/xklb/data/yt_dlp_errors.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.7/xklb/media/av.py` & `xklb-2.6.9/xklb/createdb/av.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from datetime import datetime
 from pathlib import Path
 
-from xklb.media import media_check, subtitle
+from xklb.createdb import subtitle
+from xklb.mediafiles import media_check
 from xklb.utils import consts, file_utils, iterables, nums, objects, processes, strings
 from xklb.utils.consts import DBType
 from xklb.utils.log_utils import log
 
 
 def get_subtitle_tags(path, streams, codec_types, scan_subtitles=False) -> dict:
     attachment_count = sum(1 for s in codec_types if s == "attachment")
```

### Comparing `xklb-2.6.7/xklb/media/dedupe.py` & `xklb-2.6.9/xklb/editdb/dedupe_media.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,25 +2,23 @@
 from collections import defaultdict
 from concurrent.futures import ThreadPoolExecutor
 from copy import deepcopy
 from pathlib import Path
 
 import humanize
 
-from xklb import db_media, usage
-from xklb.media import media_printer
-from xklb.scripts import sample_compare, sample_hash
+from xklb import db_media, media_printer, usage
+from xklb.files import sample_compare, sample_hash
 from xklb.utils import arggroups, consts, db_utils, devices, file_utils, iterables, objects, processes, strings
 from xklb.utils.consts import DBType
 from xklb.utils.log_utils import log
 
 
 def parse_args() -> argparse.Namespace:
     parser = argparse.ArgumentParser(prog="library dedupe-media", usage=usage.dedupe_media)
-
     arggroups.sql_fs(parser)
 
     profile = parser.add_mutually_exclusive_group()
     profile.add_argument(
         "--audio",
         action="store_const",
         dest="profile",
@@ -55,14 +53,15 @@
         dest="profile",
         const="fts",
         help=argparse.SUPPRESS,
     )
     profile.add_argument(
         "--filesystem",
         "--fs",
+        "--hash",
         action="store_const",
         dest="profile",
         const=DBType.filesystem,
         help="Dedupe filesystem database",
     )
     profile.add_argument(
         "--text",
@@ -80,15 +79,14 @@
         help=argparse.SUPPRESS,
         # "Dedupe image database",
     )
     profile.set_defaults(profile="audio")
 
     parser.set_defaults(limit="100")
 
-    parser.add_argument("--no-delete", "--soft-delete", "--mark-deleted", action="store_true")
     parser.add_argument("--dedupe-cmd", help=argparse.SUPPRESS)
     parser.add_argument("--force", "-f", action="store_true")
 
     parser.add_argument("--basename", action="store_true")
     parser.add_argument("--dirname", action="store_true")
     parser.add_argument(
         "--min-similarity-ratio",
@@ -100,15 +98,15 @@
     arggroups.debug(parser)
 
     arggroups.database(parser)
     parser.add_argument("paths", nargs="*")
     args = parser.parse_intermixed_args()
     args.db = db_utils.connect(args)
 
-    args.action = consts.SC.dedupe
+    args.action = consts.SC.dedupe_media
 
     args.sort = "\n        , ".join(filter(bool, args.sort))
     args.sort = args.sort.replace(",,", ",")
 
     args.filter_sql = []
     args.filter_bindings = {}
 
@@ -587,19 +585,20 @@
     duplicates_size = sum(filter(None, [d["duplicate_size"] for d in duplicates]))
     print(f"Approx. space savings: {humanize.naturalsize(duplicates_size // 2, binary=True)}")
 
     if duplicates and (args.force or devices.confirm("Delete duplicates?")):  # type: ignore
         log.info("Deleting...")
         for d in duplicates:
             path = d["duplicate_path"]
-            if not path.startswith("http") and not args.no_delete:
-                if args.dedupe_cmd:
-                    processes.cmd(
-                        *shlex.split(args.dedupe_cmd), d["duplicate_path"], d["keep_path"]
-                    )  # follows rmlint interface
-                else:
-                    file_utils.trash(args, path, detach=False)
+            if path.startswith("http"):
+                pass
+            elif args.dedupe_cmd:
+                processes.cmd(
+                    *shlex.split(args.dedupe_cmd), d["duplicate_path"], d["keep_path"]
+                )  # follows rmlint interface
+            else:
+                file_utils.trash(args, path, detach=False)
             db_media.mark_media_deleted(args, path)
 
 
 if __name__ == "__main__":
     dedupe_media()
```

### Comparing `xklb-2.6.7/xklb/media/media_check.py` & `xklb-2.6.9/xklb/mediafiles/media_check.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.7/xklb/media/media_player.py` & `xklb-2.6.9/xklb/playback/media_player.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,17 +4,16 @@
 from pathlib import Path
 from platform import system
 from random import randrange
 from shutil import which
 from time import sleep
 
 from xklb import db_media, history
-from xklb.media import subtitle
-from xklb.post_actions import post_act
-from xklb.scripts import playback_control
+from xklb.createdb import subtitle
+from xklb.playback import playback_control, post_actions
 from xklb.utils import consts, db_utils, devices, iterables, log_utils, mpv_utils, path_utils, processes
 from xklb.utils.consts import SC
 from xklb.utils.log_utils import log
 
 
 def watch_chromecast(args, m: dict, subtitles_file=None) -> subprocess.CompletedProcess | None:
     if "vlc" in m["player"]:
@@ -574,15 +573,15 @@
                     if m:
                         players.append(_create_window_player(args, window_geometry, m))
                 else:
                     log.debug("%s Check if still running", t_idx)
                     if m["process"].poll() is not None:
                         player_process = processes.Pclose(m["process"])
 
-                        post_act(
+                        post_actions.post_act(
                             args,
                             m["path"],
                             media_len=playlist.remaining,
                             geom_data=geom_data,
                             player_process=player_process,
                         )
 
@@ -637,28 +636,28 @@
 
     start_time = time.time()
     try:
         if args.chromecast:
             try:
                 chromecast_play(args, m)
                 t.reset()
-                post_act(args, m["original_path"], media_len=media_len)
+                post_actions.post_act(args, m["original_path"], media_len=media_len)
                 log.debug("player.post_act: %s", t.elapsed())
             except Exception:
                 if args.ignore_errors:
                     return
                 else:
                     raise
         elif args.auto_seek and Path(m["player"][0]).name in ["mpv", "mpv.com"]:
             mpv_jsonipc(args, m)
-            post_act(args, m["original_path"], media_len=media_len)
+            post_actions.post_act(args, m["original_path"], media_len=media_len)
         else:
             player_process = single_player(args, m)
             t.reset()
-            post_act(args, m["original_path"], media_len=media_len, player_process=player_process)
+            post_actions.post_act(args, m["original_path"], media_len=media_len, player_process=player_process)
             log.debug("player.post_act: %s", t.elapsed())
     finally:
         playhead = mpv_utils.get_playhead(
             args,
             m["original_path"],
             start_time,
             existing_playhead=m.get("playhead"),
```

### Comparing `xklb-2.6.7/xklb/media/media_printer.py` & `xklb-2.6.9/xklb/media_printer.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 from copy import deepcopy
 from io import StringIO
 from numbers import Number
 from pathlib import Path
 
 from tabulate import tabulate
 
-from xklb import db_media, history, post_actions
+from xklb import db_media, history
+from xklb.playback import post_actions
 from xklb.utils import consts, db_utils, iterables, printing, processes, sql_utils, strings
 from xklb.utils.consts import SC
 from xklb.utils.log_utils import log
 
 
 def filter_deleted(media):
     http_list = []
@@ -198,15 +199,15 @@
         if isinstance(v, (int, float)):
             return True
         return None
 
     media = iterables.list_dict_filter_bool(media)
 
     if "f" in print_args:
-        if len(media) <= 1000 and getattr(args, "action", "") not in [consts.SC.open_links]:
+        if len(media) <= 1000 and getattr(args, "action", "") not in [consts.SC.links_open]:
             media, deleted_paths = filter_deleted(media)
             db_media.mark_media_deleted(args, deleted_paths)
             if len(media) == 0:
                 raise FileNotFoundError
 
         if not cols:
             cols = ["path"]
```

### Comparing `xklb-2.6.7/xklb/media/subtitle.py` & `xklb-2.6.9/xklb/createdb/subtitle.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.7/xklb/scratch/javguru.py` & `xklb-2.6.9/xklb/scratch/javguru.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import argparse, time
 from pathlib import Path
 from urllib.parse import urljoin
 
-from xklb.media import media_check
+from xklb.mediafiles import media_check
 from xklb.utils import arggroups, file_utils, path_utils, processes, web
 
 
 def jav_guru() -> None:
     parser = argparse.ArgumentParser()
     parser.add_argument("--chrome", action="store_true")
     parser.add_argument("--small", action="store_true")
```

### Comparing `xklb-2.6.7/xklb/scratch/javtiful.py` & `xklb-2.6.9/xklb/scratch/javtiful.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import argparse, time
 from pathlib import Path
 
-from xklb.media import media_check
+from xklb.mediafiles import media_check
 from xklb.utils import arggroups, file_utils, path_utils, processes, web
 
 
 def javtiful() -> None:
     parser = argparse.ArgumentParser()
     parser.add_argument("--chrome", action="store_true")
     arggroups.debug(parser)
```

### Comparing `xklb-2.6.7/xklb/scratch/mam_search.py` & `xklb-2.6.9/xklb/scratch/mam_search.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.7/xklb/scratch/mam_slots.py` & `xklb-2.6.9/xklb/scratch/mam_slots.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.7/xklb/scripts/add_row.py` & `xklb-2.6.9/xklb/createdb/row_add.py`

 * *Files 10% similar despite different names*

```diff
@@ -28,16 +28,16 @@
 
     if len(values) > 0:
         kwargs[key] = get_val()
 
     return kwargs
 
 
-def add_row():
-    parser = argparse.ArgumentParser(description="Add arbitrary rows to a SQLITE db", usage=usage.add_row)
+def row_add():
+    parser = argparse.ArgumentParser(description="Add arbitrary rows to a SQLITE db", usage=usage.row_add)
     parser.add_argument("--table-name", "--table", "-t", default="media")
     arggroups.debug(parser)
 
     arggroups.database(parser)
     args, unknown_args = parser.parse_known_args()
 
     Path(args.database).touch()
```

### Comparing `xklb-2.6.7/xklb/scripts/big_dirs.py` & `xklb-2.6.9/xklb/fsdb/big_dirs.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import argparse, os
 from pathlib import Path
 
-from xklb import history, usage
-from xklb.media import media_printer
-from xklb.scripts import mcda
+from xklb import history, media_printer, usage
+from xklb.tablefiles import mcda
 from xklb.utils import arg_utils, arggroups, consts, db_utils, file_utils, nums, objects, sql_utils
 from xklb.utils.log_utils import log
 
 
 def parse_args() -> argparse.Namespace:
     parser = argparse.ArgumentParser(
         prog="library big_dirs",
@@ -35,15 +34,15 @@
     if args.sort_groups_by:
         args.sort_groups_by = arg_utils.parse_ambiguous_sort(args.sort_groups_by)
         args.sort_groups_by = ",".join(args.sort_groups_by)
 
     if args.size:
         args.size = sql_utils.parse_human_to_sql(nums.human_to_bytes, "size", args.size)
 
-    args.action = consts.SC.bigdirs
+    args.action = consts.SC.big_dirs
     log.info(objects.dict_filter_bool(args.__dict__))
     return args
 
 
 def group_files_by_folder(args, media) -> list[dict]:
     p_media = {}
     for m in media:
@@ -158,15 +157,15 @@
 
 def big_dirs() -> None:
     args = parse_args()
     history.create(args)
 
     media = get_table(args)
     if args.cluster_sort and len(media) > 2:
-        from xklb.scripts.cluster_sort import cluster_paths
+        from xklb.text.cluster_sort import cluster_paths
 
         groups = cluster_paths([d["path"] for d in media], n_clusters=getattr(args, "clusters", None))
         groups = sorted(groups, key=lambda d: (-len(d["grouped_paths"]), -len(d["common_prefix"])))
 
         media_keyed = {d["path"]: d for d in media}
         folders = [
             {
```

### Comparing `xklb-2.6.7/xklb/scripts/block.py` & `xklb-2.6.9/xklb/mediadb/block.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import argparse, sys
 
 import humanize
 
-from xklb import post_actions, tube_backend, usage
-from xklb.media import media_printer
+from xklb import media_printer, usage
+from xklb.createdb import tube_backend
+from xklb.playback import post_actions
 from xklb.utils import arggroups, consts, db_utils, devices, iterables, objects
 from xklb.utils.consts import SC
 from xklb.utils.log_utils import log
 
 
 def parse_args():
     parser = argparse.ArgumentParser(
@@ -240,15 +241,15 @@
                         )
 
         if not matching_media:
             unmatched_playlists.append(p)
             continue
 
         if args.cluster:
-            from xklb.scripts.cluster_sort import cluster_dicts
+            from xklb.text.cluster_sort import cluster_dicts
 
             matching_media = list(reversed(cluster_dicts(args, matching_media)))
 
         media_printer.media_printer(args, matching_media)
         if args.no_confirm or devices.confirm("Add to blocklist?"):
             add_to_blocklist(args, p)
         else:
```

### Comparing `xklb-2.6.7/xklb/scripts/christen.py` & `xklb-2.6.9/xklb/fsdb/christen.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.7/xklb/scripts/cluster_sort.py` & `xklb-2.6.9/xklb/text/cluster_sort.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import argparse, difflib, json, os.path, sys
 from collections import Counter
 from pathlib import Path
 
 from xklb import usage
 from xklb.data import wordbank
-from xklb.scripts import eda, mcda
+from xklb.tablefiles import eda, mcda
 from xklb.utils import arggroups, consts, db_utils, file_utils, iterables, nums, objects, printing, strings
 from xklb.utils.consts import DBType
 from xklb.utils.log_utils import Timer, log
 
 
 def parse_args() -> argparse.Namespace:
     parser = argparse.ArgumentParser(prog="library cluster-sort", usage=usage.cluster_sort)
```

### Comparing `xklb-2.6.7/xklb/scripts/copy_play_counts.py` & `xklb-2.6.9/xklb/multidb/copy_play_counts.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import argparse
 from pathlib import Path
 
 from xklb import history, usage
-from xklb.scripts.dedupe_db import dedupe_rows
+from xklb.editdb import dedupe_db
 from xklb.utils import arggroups, db_utils, objects
 from xklb.utils.log_utils import log
 
 
 def parse_args() -> argparse.Namespace:
     parser = argparse.ArgumentParser(prog="library copy-play-counts", usage=usage.copy_play_counts)
     parser.add_argument("--source-prefix", default="")
@@ -60,12 +60,12 @@
 
 
 def copy_play_counts() -> None:
     args = parse_args()
     history.create(args)
     for s_db in args.source_dbs:
         copy_play_count(args, s_db)
-    dedupe_rows(args, "history", ["id"], ["media_id", "time_played"])
+    dedupe_db.dedupe_rows(args, "history", ["id"], ["media_id", "time_played"])
 
 
 if __name__ == "__main__":
     copy_play_counts()
```

### Comparing `xklb-2.6.7/xklb/scripts/dedupe_czkawka.py` & `xklb-2.6.9/xklb/utils/file_utils.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,383 +1,481 @@
-import argparse, difflib, os, re, shlex, shutil, subprocess, sys, time
-from concurrent.futures import ThreadPoolExecutor
+import errno, mimetypes, os, shlex, shutil, tempfile, time
+from collections import Counter
+from collections.abc import Iterable
+from functools import wraps
+from io import StringIO
 from pathlib import Path
+from shutil import which
 
-import humanize
-from screeninfo import get_monitors
+import urllib3
 
-from xklb import post_actions
-from xklb.media import media_player
-from xklb.utils import arggroups, consts, devices, file_utils, iterables, mpv_utils, processes
+from xklb.utils import consts, file_utils, printing, processes, web
 from xklb.utils.log_utils import log
 
-left_mpv_socket = str(Path(consts.TEMP_SCRIPT_DIR) / f"mpv_socket_{consts.random_string()}")
-right_mpv_socket = str(Path(consts.TEMP_SCRIPT_DIR) / f"mpv_socket_{consts.random_string()}")
 
-
-def parse_args():
-    parser = argparse.ArgumentParser(description="Choose which duplicate to keep by opening both side-by-side in mpv")
-    arggroups.playback(parser)
-    arggroups.capability_clobber(parser)
-    arggroups.capability_delete(parser)
-    arggroups.post_actions(parser)
-    parser.set_defaults(start="15%", volume="70")
-
-    parser.add_argument(
-        "--auto-select-min-ratio",
-        type=float,
-        default=1.0,
-        help="Automatically select largest file if files have similar basenames. A sane value is in the range of 0.7~0.9",
+def scan_stats(files, filtered_files, folders):
+    return (
+        f"""Files: {len(files)}{f" [{len(filtered_files)} ignored]" if filtered_files else ''}"""
+        f" Folders: {len(folders)}"
     )
-    parser.add_argument("--all-keep", action="store_true")
-    parser.add_argument("--all-left", action="store_true")
-    parser.add_argument("--all-right", action="store_true")
-    parser.add_argument("--all-delete", action="store_true")
-    arggroups.debug(parser)
-
-    parser.add_argument("file_path", help="Path to the text file containing the file list.")
-    args = parser.parse_args()
-    return args
 
 
-def backup_and_read_file(file_path):
-    backup_filename = file_path + ".bak"
-    if not os.path.exists(backup_filename):
+def rglob(base_dir: str, extensions: None | Iterable[str] = None) -> tuple[set[str], set[str], set[str]]:
+    files = set()
+    filtered_files = set()
+    folders = set()
+    stack = [base_dir]
+    while stack:
+        current_dir = stack.pop()
         try:
-            shutil.copy2(file_path, backup_filename)
-        except Exception as e:
-            print(f"Failed to create backup file: {e}")
-
-    with open(file_path) as file:
-        content = file.read()
-    return content
-
-
-def extract_dupe_groups(content):
-    first_newline_index = content.find("\n")
-
-    if first_newline_index != -1 and "similar friends" in content[:first_newline_index].strip().lower():
-        content = content[first_newline_index + 1 :]
-
-    groups = re.split(r"(-+MESSAGES-+\n+)", content)[0].split("\n\n")
-    return groups
-
-
-def parse_czkawka_line(line):
-    image_pattern = r"^(.+) - (\d+x\d+) - (\d+(?:\.\d+)?|\d+) ([KMG]iB) - .+$"
-    video_pattern = r"^(.+) - (\d+(?:\.\d+)?|\d+) ([KMG]iB)$"
-
-    image_match = re.match(image_pattern, line)
-    if image_match:
-        path, resolution, size_value, size_unit = image_match.groups()
-        return path.strip(), float(size_value), size_unit
-
-    video_match = re.match(video_pattern, line)
-    if video_match:
-        path, size_value, size_unit = video_match.groups()
-        return path.strip(), float(size_value), size_unit
-
-    raise ValueError("Could not detect file style")
-
-
-def extract_group_data(group_content):
-    paths_and_sizes = []
-    groups = group_content.split("\n")
-    if len(groups) < 2:
-        return None
-    for match in groups:
-        if match == "":
-            continue
-
-        path, size_value, size_unit = parse_czkawka_line(match)
-        if size_unit == "GiB":
-            size_value *= 1024 * 1024 * 1024
-        elif size_unit == "MiB":
-            size_value *= 1024 * 1024
-        elif size_unit == "KiB":
-            size_value *= 1024
-        paths_and_sizes.append({"path": path, "size": size_value})
-    return paths_and_sizes
-
-
-def truncate_file_before_match(filename, match_string):
-    with open(filename) as file:
-        lines = file.readlines()
-    matching_lines = [i for i, line in enumerate(lines) if match_string in line]
-
-    if len(matching_lines) == 1:
-        line_index = matching_lines[0]
-        with open(filename, "w") as file:
-            file.write("".join(lines[line_index - 1 :]))
-        print(f"Progress saved. File truncated before the line containing: '{match_string}'")
-        remaining = sum(1 for s in lines[line_index - 1 :] if s == "\n") - 1
-        num_videos = sum(1 for s in lines[line_index - 1 :] if s != "\n") - 12
-        print(f"{remaining} groups (~{num_videos} videos) remain to check")
-    elif len(matching_lines) == 0:
-        print(f"Match not found in the file: '{match_string}'")
-    else:
-        print(f"Multiple matches found in the file for: '{match_string}'")
+            scanned_dir = os.scandir(current_dir)
+        except FileNotFoundError:
+            pass
+        else:
+            for entry in scanned_dir:
+                if entry.is_dir(follow_symlinks=False):
+                    folders.add(entry.path)
+                    stack.append(entry.path)
+                else:
+                    if extensions is None:
+                        files.add(entry.path)
+                    else:
+                        extension = entry.path.rsplit(".", 1)[-1].lower()
+                        if extension in extensions:
+                            files.add(entry.path)
+                        else:
+                            filtered_files.add(entry.path)
+
+            printing.print_overwrite(f"[{base_dir}] {scan_stats(files, filtered_files, folders)}")
+
+    print(f"\r[{base_dir}] {scan_stats(files, filtered_files, folders)}")
+
+    filtered_extensions = Counter(Path(s).suffix for s in filtered_files)
+    log.info("Filtered extensions: %s", filtered_extensions)
+
+    return files, filtered_files, folders
+
+
+def file_temp_copy(src) -> str:
+    fo_dest = tempfile.NamedTemporaryFile(delete=False)
+    with open(src, "r+b") as fo_src:
+        shutil.copyfileobj(fo_src, fo_dest)
+    fo_dest.seek(0)
+    fname = fo_dest.name
+    fo_dest.close()
+    return fname
+
+
+def trash(args, path: Path | str, detach=True) -> None:
+    if Path(path).exists():
+        trash_put = which(args.override_trash)
+        if trash_put is not None:
+            if not detach:
+                processes.cmd(trash_put, path, strict=False)
+                return
+            try:
+                processes.cmd_detach(trash_put, path)
+            except Exception:
+                processes.cmd(trash_put, path, strict=False)
+        else:
+            Path(path).unlink(missing_ok=True)
 
 
-def side_by_side_mpv(args, left_side, right_side):
-    monitors = get_monitors()
-    if not monitors:
-        print("No connected displays found.")
-        return
+def is_file_open(path):
+    if os.name == "nt":
+        try:
+            os.open(path, os.O_RDWR | os.O_EXCL)
+            return False
+        except OSError:
+            return True
+    else:
+        open_files = set()
+        for proc in os.listdir("/proc"):
+            try:
+                fd_dir = os.path.join("/proc", proc, "fd")
+                for fd in os.listdir(fd_dir):
+                    link = os.readlink(os.path.join(fd_dir, fd))
+                    if link.startswith("/") and link == path:
+                        open_files.add(link)
+            except OSError:
+                continue
+        return path in open_files
+
 
-    display = media_player.modify_display_size_for_taskbar(monitors[0])
-    mpv_width = display.width // 2
+def filter_file(path, sieve) -> None:
+    with open(path) as fr:
+        lines = fr.readlines()
+        with tempfile.NamedTemporaryFile(mode="w", delete=False) as temp:
+            temp.writelines(line for line in lines if line.rstrip() not in sieve)
+            temp.flush()
+            os.fsync(temp.fileno())
+    shutil.copy(temp.name, path)
+    Path(temp.name).unlink()
+
+
+def tempdir_unlink(pattern):
+    temp_dir = tempfile.gettempdir()
+    cutoff = time.time() - 15 * 60  # 15 minutes in seconds
+    for p in Path(temp_dir).glob(pattern):
+        try:
+            if p.stat().st_mtime < cutoff:
+                p.unlink(missing_ok=True)
+        except FileNotFoundError:  # glob->stat() racing
+            pass
+
+
+def resolve_absolute_path(s):
+    p = Path(s).expanduser()
+    if p.is_absolute():
+        p = p.resolve()
+        if p.exists():
+            return str(p)
+    return s  # relative path
+
+
+def resolve_absolute_paths(paths):
+    if paths is None:
+        return paths
+    return [resolve_absolute_path(s) for s in paths]
+
+
+def fast_glob(path_dir, limit=100):
+    files = []
+    with os.scandir(path_dir) as entries:
+        for entry in entries:
+            if entry.is_file():
+                files.append(entry.path)
+                if len(files) == limit:
+                    break
+    return sorted(files)
+
+
+def rename_move_file(source_file, destination_file, simulate=False):
+    if simulate:
+        print("mv", source_file, destination_file)
+    else:
+        try:
+            os.rename(source_file, destination_file)  # performance
+        except OSError as e:
+            if e.errno == errno.ENOENT:
+                try:
+                    os.makedirs(os.path.dirname(destination_file), exist_ok=True)
+                    os.rename(source_file, destination_file)  # try again
+                except OSError as e:
+                    if e.errno == errno.EXDEV:  # Cross-device
+                        shutil.move(source_file, destination_file)  # Fallback to shutil.move
+                    else:
+                        raise
+            elif e.errno == errno.EXDEV:  # Cross-device
+                shutil.move(source_file, destination_file)  # Fallback to shutil.move
+            else:
+                raise
 
-    if args.auto_seek:
-        from python_mpv_jsonipc import MPV
 
-        mpv_kwargs = {
-            "save_position_on_quit": False,
-            "start": args.start,
-        }
+def move_files(file_list):
+    for existing_path, new_path in file_list:
+        try:
+            os.rename(existing_path, new_path)
+        except Exception:
+            try:
+                parent_dir = os.path.dirname(new_path)
+                os.makedirs(parent_dir, exist_ok=True)
 
-        left_mpv = MPV(ipc_socket=left_mpv_socket, geometry=f"{mpv_width}x{display.height}+0+0", **mpv_kwargs)
-        right_mpv = MPV(
-            ipc_socket=right_mpv_socket,
-            geometry=f"{mpv_width}x{display.height}+{mpv_width}+0",
-            **mpv_kwargs,
+                shutil.move(existing_path, new_path)
+            except Exception:
+                log.exception("Could not move %s", existing_path)
+
+
+def move_files_bash(file_list):
+    move_sh = """#!/bin/sh
+existing_path=$1
+new_path=$2
+
+# Attempt to rename the file/directory
+mv -Tn "$existing_path" "$new_path" 2>/dev/null
+
+if [ $? -ne 0 ]; then
+    mkdir -p $(dirname "$new_path")
+    mv -Tn "$existing_path" "$new_path"
+fi
+"""
+    move_sh_path = Path(tempfile.mktemp(dir=consts.TEMP_SCRIPT_DIR, prefix="move_", suffix=".sh"))
+    move_sh_path.write_text(move_sh)
+    move_sh_path.chmod(move_sh_path.stat().st_mode | 0o100)
+
+    with tempfile.NamedTemporaryFile(mode="w", delete=False, suffix=".tsv") as temp:
+        temp.writelines(
+            f"{shlex.quote(existing_path)}\t{shlex.quote(new_path)}\n" for existing_path, new_path in file_list
         )
+        temp.flush()
+        os.fsync(temp.fileno())
 
-        for x_mpv in (left_mpv, right_mpv):
-            x_mpv.volume = args.volume
-            x_mpv.command("script-message", "osc-visibility", "always")  # , "no-osd"
-
-            @x_mpv.on_key_press("k")
-            def keep_handler():
-                print("keep")
-
-            @x_mpv.on_key_press("d")
-            def delete_handler():
-                print("delete")
+        print(f"""### Move {len(file_list)} files to new folders: ###""")
+        print(rf"PARALLEL_SHELL=sh parallel --colsep '\t' -a {temp.name} -j 20 {move_sh_path}")
 
-        left_mpv.play(left_side)
-        right_mpv.play(right_side)
 
-        def right_quit_callback():
-            try:
-                left_mpv.command("quit")
-            except BrokenPipeError:
-                pass
+def get_file_encoding(path):
+    import chardet
 
-        left_mpv.quit_callback = right_mpv.terminate
-        right_mpv.quit_callback = right_quit_callback  # they can't both be the same
+    if path.startswith("http"):
+        detector = chardet.UniversalDetector()
+        response = web.session.get(path, stream=True)
+        response.raw.decode_content = True
 
-        with ThreadPoolExecutor() as e:
-            e.submit(mpv_utils.auto_seek, left_mpv)
-            e.submit(mpv_utils.auto_seek, right_mpv, delay=0.4)
+        num_bytes = 0
+        for chunk in response.iter_content(chunk_size=16_384):
+            if num_bytes > 1048576:  # 1MiB
+                break
+            detector.feed(chunk)
+            if detector.done:
+                break
+            num_bytes += len(chunk)
+        detector.close()
 
+        encoding = detector.result["encoding"]
     else:
-        mpv_options = [
-            "--save-position-on-quit=no",
-            "--no-resume-playback",
-            "--image-display-duration=inf",
-            "--script-opts=osc-visibility=always",
-            f"--start={args.start}",
-            f"--volume={args.volume}",
-        ]
-
-        left_mpv_process = subprocess.Popen(
-            [
-                "mpv",
-                left_side,
-                f"--input-ipc-server={left_mpv_socket}",
-                f"--geometry={mpv_width}x{display.height}+0+0",
-                *mpv_options,
-            ],
-            stdout=subprocess.DEVNULL,
-            stderr=subprocess.DEVNULL,
-        )
-        right_mpv_process = subprocess.Popen(
-            [
-                "mpv",
-                right_side,
-                f"--input-ipc-server={right_mpv_socket}",
-                f"--geometry={mpv_width}x{display.height}+{mpv_width}+0",
-                *mpv_options,
-            ],
-            stdout=subprocess.DEVNULL,
-            stderr=subprocess.DEVNULL,
-        )
+        with open(path, "rb") as f:
+            sample = f.read(1048576)  # 1 MiB
 
-        # if not all([Path(left_side).exists(), Path(right_side).exists()]):
-        #     return  # race condition
+        encoding = chardet.detect(sample)["encoding"]
 
-        while True:  # Monitor the processes and terminate the other one when one finishes
-            if left_mpv_process.poll() is not None or right_mpv_process.poll() is not None:
-                break
-            time.sleep(0.1)
+    if encoding:
+        log.info(f"The encoding of {path} is likely: {encoding}")
+    return encoding
 
-        # Terminate the other process
-        if left_mpv_process.poll() is None:
-            left_mpv_process.terminate()
-        if right_mpv_process.poll() is None:
-            right_mpv_process.terminate()
 
+def head_foot_stream(url, head_len, foot_len):
+    import io
 
-def mv_to_keep_folder(args, d) -> None:
-    keep_path = Path(args.keep_dir)
-    keep_path.mkdir(exist_ok=True)
+    head_response = web.session.get(url, stream=True)
+    head_response.raw.decode_content = True
+    head_response.raise_for_status()
 
-    media_file = d["path"]
+    head_bytes = head_response.raw.read(head_len)
 
+    foot_response = web.session.get(url, stream=True, headers={"Range": f"bytes=-{foot_len}"})
+    foot_response.raw.decode_content = True
     try:
-        new_path = shutil.move(media_file, keep_path)
-    except FileNotFoundError:
-        return
-    except shutil.Error as e:
-        if "already exists" not in str(e):
-            raise
-        p = Path(media_file)
-        new_path = Path(keep_path) / p.name
-
-        src_size = d["size"]
-        dst_size = new_path.stat().st_size
-        diff_size = humanize.naturalsize(src_size - dst_size, binary=True)
-
-        if src_size > dst_size:
-            print("Source is larger than destination", diff_size)
-        elif src_size < dst_size:
-            print("Source is smaller than destination", diff_size)
-        else:
-            print("Source and destination are the same size", humanize.naturalsize(src_size, binary=True))
-        if devices.confirm("Replace destination file?"):
-            file_utils.trash(args, new_path, detach=False)
-            new_path = shutil.move(media_file, keep_path)
+        foot_bytes = foot_response.raw.read(foot_len)
+    except urllib3.exceptions.DecodeError:
+        foot_bytes = b""
 
-    log.info(f"{new_path}: new location")
+    stream = io.BytesIO(head_bytes + foot_bytes)
+    return stream
 
 
-def group_and_delete(args, groups):
-    is_interactive = not any([args.all_keep, args.all_left, args.all_right, args.all_delete])
+def mimetype(path):
+    import puremagic
 
-    for group_content in groups:
-        if group_content == "":
-            continue
+    p = Path(path)
 
-        group = extract_group_data(group_content)
-        if group is None:
-            continue
+    file_type = None
+    ext = puremagic.ext_from_filename(path)
+    if ext in (".zarr", ".zarr/"):
+        file_type = "Zarr"
+    elif p.is_dir():
+        file_type = "directory"
+    else:
+        file_type, encoding = mimetypes.guess_type(path, strict=False)
 
-        def delete_dupe(d, detach=is_interactive):
-            file_utils.trash(args, d["path"], detach=detach)
-            log.info(f"{d['path']}: Deleted")
+    if ext and file_type is None:
+        pandas_ext = {
+            ".dta": "Stata",
+            ".xlsx": "Excel",
+            ".xls": "Excel",
+            ".json": "JSON",
+            ".jsonl": "JSON Lines",
+            ".ndjson": "JSON Lines",
+            ".geojson": "GeoJSON",
+            ".geojsonl": "GeoJSON Lines",
+            ".ndgeojson": "GeoJSON Lines",
+            ".hdf": "HDF5",
+            ".feather": "Feather",
+            ".parquet": "Parquet",
+            ".sas7bdat": "SAS",
+            ".sav": "SPSS",
+            ".pkl": "Pickle",
+            ".orc": "ORC",
+        }
+        file_type = pandas_ext.get(ext)
 
-        group.sort(key=lambda x: x["size"], reverse=True)
-        left = group[0]
+    if file_type is None:
+        try:
+            if path.startswith("http"):
+                max_head = max([len(x.byte_match) + x.offset for x in puremagic.magic_header_array])
+                max_foot = max([len(x.byte_match) + abs(x.offset) for x in puremagic.magic_footer_array])
+                info = puremagic.magic_stream(head_foot_stream(path, max_head, max_foot), path)
+            else:
+                info = puremagic.magic_file(path)
+            log.debug(info)
+            file_type = info[0].name
+        except (puremagic.PureError, IndexError, ValueError):
+            if p.is_socket():
+                file_type = "socket"
+            elif p.is_fifo():
+                file_type = "fifo"
+            elif p.is_symlink():
+                file_type = "symlink"
+            elif p.is_block_device():
+                file_type = "block device"
+            elif p.is_char_device():
+                file_type = "char device"
+            try:
+                if Path(path).stat().st_size == 0:
+                    file_type = "empty file"
+            except Exception:
+                pass
 
-        dups = group[1:]
-        kept_dups = []
-        while len(dups) > 0:
-            right = dups.pop()
+        except FileNotFoundError:
+            return
 
-            if right["path"] == left["path"]:
-                continue
+    return file_type
 
-            if not os.path.exists(right["path"]):
-                log.debug(f"{right['path']}: not found")
-                continue
 
-            if not os.path.exists(left["path"]):
-                log.debug(f"{left['path']}: not found")
-                left = right
-                continue
+def retry_with_different_encodings(func):
+    @wraps(func)
+    def wrapper(*args, **kwargs):
+        try:
+            return func(*args, **kwargs)
+        except UnicodeDecodeError as exc:
+            original_exc = exc
+
+        likely_encodings = []
+        detected_encoding = get_file_encoding(args[0])
+        if detected_encoding:
+            likely_encodings.append(detected_encoding)
 
-            print(left["path"], humanize.naturalsize(left["size"], binary=True))
-            print(right["path"], humanize.naturalsize(right["size"], binary=True))
+        for encoding in likely_encodings + consts.COMMON_ENCODINGS:
+            try:
+                kwargs["encoding"] = encoding
+                return func(*args, **kwargs)
+            except UnicodeDecodeError:
+                pass
 
-            if args.auto_select_min_ratio < 1.0:
-                similar_ratio = difflib.SequenceMatcher(
-                    None,
-                    os.path.basename(left["path"]),
-                    os.path.basename(right["path"]),
-                ).ratio()
-                if similar_ratio >= args.auto_select_min_ratio or any(
-                    s in left["path"] and s in right["path"] for s in ["Goldmines_Bollywood"]
-                ):
-                    delete_dupe(right)
-                continue
+        raise original_exc  # If no encoding worked, raise the original exception
 
-            if not is_interactive:
-                if args.all_left:
-                    kept_dups.append(left)
-                    delete_dupe(right)
-                elif args.all_right:
-                    kept_dups.append(right)
-                    delete_dupe(left)
-                    left = right
-                elif args.all_delete:
-                    delete_dupe(left)
-                    delete_dupe(right)
-                continue
+    return wrapper
 
-            is_next_iter_not_last = len(dups) > 1
 
-            if args.override_player:
-                for path in (left["path"], right["path"]):
-                    player_process = processes.cmd(*shlex.split(args.override_player), path, strict=False)
-                    if player_process.returncode == 0:
-                        post_actions.post_act(
-                            args,
-                            path,
-                            media_len=len(dups),
-                            record_history=False,
-                            player_process=player_process,
-                            action="ASK_MOVE_OR_DELETE" if args.keep_dir else "ASK_DELETE",
-                        )
-                    else:
-                        truncate_file_before_match(args.file_path, left["path"])
-                        processes.player_exit(player_process)
-            else:
-                side_by_side_mpv(args, left["path"], right["path"])
-                while True:
-                    devices.clear_input()
-                    user_input = (
-                        input("Keep which files? (l Left/r Right/k Keep both/d Delete both) [default: l]: ")
-                        .strip()
-                        .lower()
-                    )
-                    if args.all_keep or user_input in ("k", "keep"):
-                        kept_dups.append(left)
-                        kept_dups.append(right)
-                        break
-                    elif args.all_left or user_input in ("l", "left", ""):
-                        kept_dups.append(left)
-                        delete_dupe(right, detach=is_next_iter_not_last)
-                        break
-                    elif args.all_right or user_input in ("r", "right"):
-                        kept_dups.append(right)
-                        delete_dupe(left, detach=is_next_iter_not_last)
-                        break
-                    elif args.all_delete or user_input in ("d", "delete"):
-                        delete_dupe(right, detach=is_next_iter_not_last)
-                        delete_dupe(left, detach=is_next_iter_not_last)
-                        break
-                    elif user_input in ("q", "quit"):
-                        truncate_file_before_match(args.file_path, left["path"])
-                        sys.exit(0)
-                    else:
-                        print("Invalid input. Please type 'left', 'right', 'keep', 'delete', or 'quit' and enter")
+@retry_with_different_encodings
+def read_file_to_dataframes(
+    path, table_name=None, table_index=None, start_row=None, end_row=None, order_by=None, encoding=None, mimetype=None
+):
+    import pandas as pd
+
+    if mimetype is None:
+        mimetype = file_utils.mimetype(path)
+    if mimetype is not None:
+        mimetype = mimetype.strip().lower()
+    log.info(mimetype)
 
-            if len(dups) > 1:
-                left = dups.pop()
-            elif len(dups) == 1 and len(kept_dups) > 0:
-                left = kept_dups[-1]
+    if mimetype is None:
+        msg = f"{path}: File type could not be determined. Pass in --filetype"
+        raise ValueError(msg)
 
-        if args.keep_dir:
-            for d in iterables.list_dict_unique(kept_dups, ["path"]):
-                if os.path.exists(d["path"]):
-                    mv_to_keep_folder(args, d)
+    if mimetype in ("sqlite", "sqlite3", "sqlite database file"):
+        import pandas as pd
+        from sqlite_utils import Database
 
-        print()
+        db = Database(path)
 
+        if table_name:
+            tables = [table_name]
+        else:
+            tables = [
+                s
+                for s in db.table_names() + db.view_names()
+                if not any(["_fts_" in s, s.endswith("_fts"), s.startswith("sqlite_")])
+            ]
+            if table_index:
+                tables = [table_index]
+
+        dfs = []
+        for table in tables:
+            df = pd.DataFrame(db[table].rows_where(offset=start_row, limit=end_row, order_by=order_by))
+            df.name = table
+            dfs.append(df)
+        db.close()
+    elif mimetype in (
+        "excel",
+        "application/vnd.ms-excel",
+        "excel spreadsheet subheader",
+        "application/vnd.openxmlformats-officedocument.spreadsheetml.sheet",
+    ):
+        excel_data = pd.read_excel(path, sheet_name=table_name or table_index, nrows=end_row, skiprows=start_row)
+        dfs = []
+        if isinstance(excel_data, pd.DataFrame):
+            worksheet_names = excel_data.index.levels[0]  # type: ignore
+            for name in worksheet_names:
+                df = excel_data.loc[name]
+                df.name = name
+                dfs.append(df)
+        else:
+            for worksheet_name, df in excel_data.items():
+                df.name = worksheet_name
+                dfs.append(df)
+    elif mimetype in (
+        "netcdf",
+        "application/x-netcdf",
+    ):
+        import xarray as xr  # type: ignore
+
+        ds = xr.open_dataset(path)
+        dfs = [ds.to_dataframe()]
+    elif mimetype in ("zarr",):
+        import xarray as xr  # type: ignore
+
+        ds = xr.open_zarr(path)
+        dfs = [ds.to_dataframe()]
+    elif mimetype in (
+        "hdf",
+        "application/x-hdf",
+    ):
+        dfs = [pd.read_hdf(path, start=start_row, stop=end_row)]
+    elif mimetype in (
+        "json",
+        "application/json",
+    ):
+        dfs = [pd.read_json(path, encoding=encoding)]
+    elif mimetype in ("jsonl", "json lines", "geojson lines"):
+        dfs = [pd.read_json(path, nrows=end_row, lines=True, encoding=encoding)]
+    elif mimetype in (
+        "csv",
+        "text/csv",
+    ):
+        dfs = [pd.read_csv(path, nrows=end_row, skiprows=start_row or 0, encoding=encoding)]
+    elif mimetype in (
+        "tsv",
+        "text/tsv",
+        "text/tab-separated-values",
+    ):
+        dfs = [pd.read_csv(path, delimiter="\t", nrows=end_row, skiprows=start_row or 0, encoding=encoding)]
+    elif mimetype in ("parq", "parquet", "application/parquet"):
+        dfs = [pd.read_parquet(path)]
+    elif mimetype in ("pkl", "pickle", "application/octet-stream"):
+        dfs = [pd.read_pickle(path)]
+    elif mimetype in (
+        "html",
+        "htm",
+        "text/html",
+        "html document",
+    ):
+        if path.startswith("http"):
+            path = StringIO(web.extract_html(path))
+        dfs = pd.read_html(path, skiprows=start_row, encoding=encoding)
+    elif mimetype in ("stata",):
+        dfs = [pd.read_stata(path)]
+    elif mimetype in ("feather",):
+        dfs = [pd.read_feather(path)]
+    elif mimetype in ("orc",):
+        dfs = [pd.read_orc(path)]
+    elif "xml" in mimetype:
+        dfs = [pd.read_xml(path, encoding=encoding or "utf-8")]
+    else:
+        msg = f"{path}: Unsupported file type: {mimetype}"
+        raise ValueError(msg)
 
-def czkawka_dedupe():
-    args = parse_args()
+    for table_index, df in enumerate(dfs):
+        if not hasattr(df, "name"):
+            df.name = str(table_index)
 
-    content = backup_and_read_file(args.file_path)
-    groups = extract_dupe_groups(content)
-    group_and_delete(args, groups)
+    return dfs
```

### Comparing `xklb-2.6.7/xklb/scripts/dedupe_db.py` & `xklb-2.6.9/xklb/editdb/dedupe_db.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.7/xklb/scripts/disk_usage.py` & `xklb-2.6.9/xklb/fsdb/disk_usage.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import argparse, os
 from pathlib import Path
 
-from xklb import usage
-from xklb.media import media_printer
+from xklb import media_printer, usage
 from xklb.utils import arggroups, consts, db_utils, file_utils, nums, objects, processes, sql_utils
 from xklb.utils.log_utils import log
 
 
 def parse_args() -> argparse.Namespace:
     parser = argparse.ArgumentParser(
         prog="library disk_usage",
@@ -36,15 +35,15 @@
 
     if args.sort_groups_by:
         args.sort_groups_by = " ".join(args.sort_groups_by)
 
     if args.size:
         args.size = sql_utils.parse_human_to_sql(nums.human_to_bytes, "size", args.size)
 
-    args.action = consts.SC.diskusage
+    args.action = consts.SC.disk_usage
     log.info(objects.dict_filter_bool(args.__dict__))
     return args
 
 
 def sort_by(args):
     if args.sort_groups_by:
         return lambda x: x.get(args.sort_groups_by) or 0
```

### Comparing `xklb-2.6.7/xklb/scripts/download_status.py` & `xklb-2.6.9/xklb/mediadb/download_status.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import argparse
 
-from xklb import dl_extract, tube_backend, usage
-from xklb.media import media_printer
+from xklb import media_printer, usage
+from xklb.createdb import tube_backend
+from xklb.mediadb import download
 from xklb.utils import arg_utils, arggroups, consts, db_utils, objects, sql_utils
 from xklb.utils.log_utils import log
 
 
 def parse_args() -> argparse.Namespace:
     parser = argparse.ArgumentParser(
         "library download-status",
@@ -32,15 +33,15 @@
     return args
 
 
 def download_status() -> None:
     args = parse_args()
     arg_utils.parse_args_sort(args)
 
-    query, bindings = dl_extract.construct_query(args)
+    query, bindings = download.construct_query(args)
 
     count_paths = ""
     if "time_modified" in query:
         if args.safe:
             args.db.register_function(tube_backend.is_supported, deterministic=True)
             count_paths += f", count(*) FILTER(WHERE cast(STRFTIME('%s', datetime( time_modified, 'unixepoch', '+{args.retry_delay}')) as int) >= STRFTIME('%s', datetime()) and is_supported(path)) failed_recently"
             count_paths += f", count(*) FILTER(WHERE time_modified>0 and cast(STRFTIME('%s', datetime( time_modified, 'unixepoch', '+{args.retry_delay}')) as int) < STRFTIME('%s', datetime()) and is_supported(path)) retry_queued"
```

### Comparing `xklb-2.6.7/xklb/scripts/eda.py` & `xklb-2.6.9/xklb/tablefiles/eda.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.7/xklb/scripts/export_text.py` & `xklb-2.6.9/xklb/misc/export_text.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.7/xklb/scripts/history.py` & `xklb-2.6.9/xklb/mediadb/history.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import argparse
 
-from xklb import usage
+from xklb import media_printer, usage
 from xklb.history import create
-from xklb.media import media_printer
 from xklb.utils import arggroups, consts, db_utils, objects, sql_utils, strings
 from xklb.utils.log_utils import log
 
 
 def parse_args() -> argparse.Namespace:
     parser = argparse.ArgumentParser(
         "library history",
@@ -21,15 +20,15 @@
     parser.add_argument(
         "facet",
         metavar="facet",
         type=str.lower,
         default="watched",
         const="watched",
         nargs="?",
-        help=f"One of: {', '.join(consts.time_facets)} (default: %(default)s)",
+        help=f"One of: {', '.join(consts.time_facets)}",
     )
     parser.add_argument("--hide-deleted", action="store_true")
     parser.add_argument("--played", "--opened", action="store_true")
 
     arggroups.debug(parser)
 
     arggroups.database(parser)
```

### Comparing `xklb-2.6.7/xklb/scripts/incremental_diff.py` & `xklb-2.6.9/xklb/tablefiles/incremental_diff.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.7/xklb/scripts/links_db.py` & `xklb-2.6.9/xklb/createdb/links_add.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import argparse, json, random, time
 from pathlib import Path
 from urllib.parse import parse_qs, urlencode, urlparse, urlunparse
 
 from xklb import db_media, db_playlists, usage
-from xklb.scripts.mining import extract_links
+from xklb.text import extract_links
 from xklb.utils import arg_utils, arggroups, consts, db_utils, objects, printing, strings, web
 from xklb.utils.log_utils import log
 
 
 def parse_args(**kwargs):
     parser = argparse.ArgumentParser(**kwargs)
     parser.add_argument("--category", "-c", help=argparse.SUPPRESS)
```

### Comparing `xklb-2.6.7/xklb/scripts/mcda.py` & `xklb-2.6.9/xklb/tablefiles/mcda.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.7/xklb/scripts/merge_dbs.py` & `xklb-2.6.9/xklb/multidb/merge_dbs.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.7/xklb/scripts/merge_folders.py` & `xklb-2.6.9/xklb/folders/merge_folders.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.7/xklb/scripts/merge_online_local.py` & `xklb-2.6.9/xklb/editdb/merge_online_local.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import argparse, os
 from copy import deepcopy
 
-from xklb import db_media, usage
-from xklb.media import media_printer
+from xklb import db_media, media_printer, usage
 from xklb.utils import arggroups, consts, db_utils, devices, objects
 from xklb.utils.log_utils import log
 
 
 def parse_args() -> argparse.Namespace:
     parser = argparse.ArgumentParser(prog="library merge-online-local", usage=usage.merge_online_local)
     parser.add_argument("--no-confirm", "--yes", "-y", action="store_true", help=argparse.SUPPRESS)
```

### Comparing `xklb-2.6.7/xklb/scripts/move_list.py` & `xklb-2.6.9/xklb/folders/move_list.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.7/xklb/scripts/open_links.py` & `xklb-2.6.9/xklb/playback/links_open.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 import argparse, shlex, webbrowser
 from pathlib import Path
 from time import sleep
 
-from xklb import db_media, history, usage
-from xklb.media import media_printer
+from xklb import db_media, history, media_printer, usage
 from xklb.utils import arg_utils, arggroups, consts, db_utils, iterables, objects, processes, web
 from xklb.utils.log_utils import log
 
 
 def parse_args() -> argparse.Namespace:
     parser = argparse.ArgumentParser(
         prog="library open-links",
         formatter_class=argparse.ArgumentDefaultsHelpFormatter,
-        usage=usage.open_links,
+        usage=usage.links_open,
     )
     arggroups.sql_fs(parser)
 
     parser.add_argument("--path", action="store_true")
     parser.add_argument("--title", action="store_true")
     parser.add_argument("--title-prefix", "--prefix", nargs="+", action="extend")
 
@@ -30,15 +29,15 @@
 
     parser.add_argument("--browser")
     arggroups.debug(parser)
 
     arggroups.database(parser)
     parser.add_argument("search", nargs="*")
     args = parser.parse_intermixed_args()
-    args.action = consts.SC.open_links
+    args.action = consts.SC.links_open
     args.defaults = []
 
     arg_utils.parse_args_limit(args)
 
     args.include += args.search
     if args.include == ["."]:
         args.include = [str(Path().cwd().resolve())]
@@ -175,26 +174,26 @@
 
         pan.extend([{**m, "url": url} for url in m_urls if url not in urls])
         urls |= m_urls
 
     return pan
 
 
-def open_links() -> None:
+def links_open() -> None:
     args = parse_args()
     history.create(args)
 
     query, bindings = construct_links_query(args)
     media = list(args.db.query(query, bindings))
 
     if args.related >= consts.RELATED:
         media = db_media.get_related_media(args, media[0])
 
     if args.cluster_sort:
-        from xklb.scripts.cluster_sort import cluster_dicts
+        from xklb.text.cluster_sort import cluster_dicts
 
         media = cluster_dicts(args, media)[: args.limit]
 
     media = make_souffle(args, media)
 
     if args.print:
         media_printer.media_printer(args, media)
```

### Comparing `xklb-2.6.7/xklb/scripts/optimize_db.py` & `xklb-2.6.9/xklb/mediadb/optimize_db.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.7/xklb/scripts/places_import.py` & `xklb-2.6.9/xklb/createdb/places_import.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.7/xklb/scripts/playback_control.py` & `xklb-2.6.9/xklb/playback/playback_control.py`

 * *Files 0% similar despite different names*

```diff
@@ -286,15 +286,15 @@
         catt_stop(args)
 
     Path(consts.CAST_NOW_PLAYING).unlink(missing_ok=True)
     Path(args.mpv_socket).unlink(missing_ok=True)
 
 
 def playback_pause() -> None:
-    args = parse_args("next")
+    args = parse_args("pause")
     playing = _now_playing(args)
 
     if playing["catt"]:
         catt_pause(args)
 
     if playing["mpv"]:
         args.mpv.command("cycle", "pause")
```

### Comparing `xklb-2.6.7/xklb/scripts/playlists.py` & `xklb-2.6.9/xklb/mediadb/playlists.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import argparse, os, sqlite3
 
-from xklb import usage
-from xklb.media import media_printer
+from xklb import media_printer, usage
 from xklb.utils import arggroups, consts, db_utils, objects
 from xklb.utils.log_utils import log
 
 
 def parse_args() -> argparse.Namespace:
     parser = argparse.ArgumentParser(
         "library playlists",
```

### Comparing `xklb-2.6.7/xklb/scripts/process_ffmpeg.py` & `xklb-2.6.9/xklb/mediafiles/process_ffmpeg.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.7/xklb/scripts/process_image.py` & `xklb-2.6.9/xklb/mediafiles/process_image.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.7/xklb/scripts/redownload.py` & `xklb-2.6.9/xklb/mediadb/redownload.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import argparse, json, tempfile
 from copy import deepcopy
 from pathlib import Path
 
-from xklb import usage
-from xklb.media import media_printer
+from xklb import media_printer, usage
 from xklb.utils import arggroups, consts, db_utils, devices, file_utils, iterables, objects
 from xklb.utils.log_utils import log
 
 
 def parse_args() -> argparse.Namespace:
     parser = argparse.ArgumentParser(
         prog="library redownload",
```

### Comparing `xklb-2.6.7/xklb/scripts/rel_mv.py` & `xklb-2.6.9/xklb/folders/rel_mv.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.7/xklb/scripts/sample_compare.py` & `xklb-2.6.9/xklb/files/sample_compare.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import argparse, hashlib
 from concurrent.futures import ThreadPoolExecutor
 from pathlib import Path
 
 from xklb import usage
-from xklb.scripts import sample_hash
+from xklb.files import sample_hash
 from xklb.utils import arggroups, nums, objects
 from xklb.utils.log_utils import log
 
 
 def full_hash_file(path):
     sha256_hash = hashlib.sha256()
```

### Comparing `xklb-2.6.7/xklb/scripts/sample_hash.py` & `xklb-2.6.9/xklb/files/sample_hash.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.7/xklb/scripts/scatter.py` & `xklb-2.6.9/xklb/folders/scatter.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.7/xklb/scripts/search_db.py` & `xklb-2.6.9/xklb/fsdb/search_db.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.7/xklb/scripts/streaming_tab_loader.py` & `xklb-2.6.9/xklb/playback/surf.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import argparse, logging, sys
 from time import sleep
 
 from xklb import usage
-from xklb.media import media_player
+from xklb.playback import media_player
 from xklb.utils import arggroups, db_utils, objects, processes
 from xklb.utils.log_utils import log
 
 
 def parse_args() -> argparse.Namespace:
     parser = argparse.ArgumentParser(
         prog="library surf",
```

### Comparing `xklb-2.6.7/xklb/scripts/web_add.py` & `xklb-2.6.9/xklb/createdb/web_add.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import argparse, json, random, sys, time
 from pathlib import Path
 from urllib.parse import urlparse
 
 from xklb import db_media, db_playlists, usage
-from xklb.media import av, books
-from xklb.scripts import sample_hash
-from xklb.scripts.mining import extract_links
+from xklb.createdb import av, fs_add
+from xklb.files import sample_hash
+from xklb.text import extract_links
 from xklb.utils import arg_utils, arggroups, consts, db_utils, file_utils, iterables, objects, printing, strings, web
 from xklb.utils.consts import SC, DBType
 from xklb.utils.log_utils import log
 
 
 def parse_args(**kwargs):
     parser = argparse.ArgumentParser(**kwargs)
@@ -162,18 +162,18 @@
             remote_path = m["path"]  # for temp file extraction
             if DBType.video in args.profiles and (extension in consts.VIDEO_EXTENSIONS or args.scan_all_files):
                 m |= av.munge_av_tags(args, m["path"])
             if DBType.audio in args.profiles and (extension in consts.AUDIO_ONLY_EXTENSIONS or args.scan_all_files):
                 m |= av.munge_av_tags(args, m["path"])
             if DBType.text in args.profiles and (extension in consts.TEXTRACT_EXTENSIONS or args.scan_all_files):
                 with web.PartialContent(m["path"]) as temp_file_path:
-                    m |= books.munge_book_tags_fast(temp_file_path)
+                    m |= fs_add.munge_book_tags_fast(temp_file_path)
             if DBType.image in args.profiles and (extension in consts.IMAGE_EXTENSIONS or args.scan_all_files):
                 with web.PartialContent(m["path"], max_size=32 * 1024) as temp_file_path:
-                    m |= books.extract_image_metadata_chunk([{"path": temp_file_path}])[0]
+                    m |= fs_add.extract_image_metadata_chunk([{"path": temp_file_path}])[0]
             m["path"] = remote_path  # restore from temp file extraction
 
         if media:
             add_media(args, media)
 
         printing.print_overwrite(
             f"Pages to scan {len(paths)} link scan: {new_media_count} new [{len(known_paths)} known]"
@@ -192,15 +192,15 @@
     db_playlists.add(args, str(path), info)
 
 
 def web_add(args=None) -> None:
     if args:
         sys.argv = ["lb", *args]
 
-    args, _parser = parse_args(prog=f"library {SC.webadd}", usage=usage.webadd)
+    args, _parser = parse_args(prog=f"library {SC.web_add}", usage=usage.web_add)
     web.requests_session(args)  # configure session
 
     if args.insert_only:
         media_new = set()
         media_known = set()
         for p in arg_utils.gen_paths(args):
             if db_media.exists(args, p):
@@ -226,15 +226,15 @@
         db_utils.optimize(args)
 
 
 def web_update(args=None) -> None:
     if args:
         sys.argv = ["lb", *args]
 
-    args, parser = parse_args(prog=f"library {SC.webupdate}", usage=usage.webupdate)
+    args, parser = parse_args(prog=f"library {SC.web_update}", usage=usage.web_update)
     web.requests_session(args)  # configure session
 
     web_playlists = db_playlists.get_all(
         args,
         sql_filters="extractor_key = 'WebFolder'",
         order_by="""length(path)-length(REPLACE(path, '/', '')) desc
         , random()
```

### Comparing `xklb-2.6.7/xklb/scripts/mining/extract_links.py` & `xklb-2.6.9/xklb/text/extract_links.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.7/xklb/scripts/mining/extract_text.py` & `xklb-2.6.9/xklb/text/extract_text.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.7/xklb/scripts/mining/markdown_links.py` & `xklb-2.6.9/xklb/text/markdown_links.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import argparse, urllib.parse
 
+from xklb import usage
 from xklb.utils import arg_utils, arggroups, web
 
 COMMON_SITE_TITLE_SUFFIXES = [
     " | Listen online for free on SoundCloud",
     " - YouTube",
 ]
 
@@ -19,15 +20,15 @@
     title = title.replace("?", " ")
     title = title.replace("#", ": ")
 
     return title.strip()
 
 
 def markdown_links():
-    parser = argparse.ArgumentParser()
+    parser = argparse.ArgumentParser(usage=usage.markdown_links)
     arggroups.requests(parser)
     arggroups.selenium(parser)
     arggroups.debug(parser)
 
     arggroups.paths_or_stdin(parser)
     args = parser.parse_args()
```

### Comparing `xklb-2.6.7/xklb/scripts/mining/mpv_watchlater.py` & `xklb-2.6.9/xklb/editdb/mpv_watchlater.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.7/xklb/scripts/mining/nouns.py` & `xklb-2.6.9/xklb/text/nouns.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,14 @@
-import sys
+import argparse, sys
 from html.parser import HTMLParser
 from io import StringIO
 
+from xklb import usage
 from xklb.data import wordbank
-from xklb.utils import printing
-
-"""
-extract compound nouns and phrases from unstructured mixed HTML plain text
-
-xsv select text hn_comment_202210242109.csv | library nouns | sort | uniq -c | sort --numeric-sort
-"""
+from xklb.utils import arggroups, printing
 
 
 class MLStripper(HTMLParser):
     def __init__(self) -> None:
         super().__init__()
         self.reset()
         self.strict = False
@@ -61,9 +56,13 @@
         )
 
     parts = line_processor.RE_NOUNS_SPLIT.split(txt)
     printer(parts)
 
 
 def nouns() -> None:
+    parser = argparse.ArgumentParser(usage.nouns)
+    arggroups.debug(parser)
+    args = parser.parse_args()
+
     for line in sys.stdin:
         line_processor(line)
```

### Comparing `xklb-2.6.7/xklb/scripts/mining/pushshift.py` & `xklb-2.6.9/xklb/editdb/pushshift.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import argparse, sys
 from pathlib import Path
 
 from xklb import usage
-from xklb.reddit_extract import slim_post_data
+from xklb.createdb.reddit_add import slim_post_data
 from xklb.utils import arggroups, db_utils, objects, printing
 from xklb.utils.log_utils import log
 
 try:
     import orjson
 except ModuleNotFoundError:
     import json as orjson
```

### Comparing `xklb-2.6.7/xklb/scripts/mining/reddit_selftext.py` & `xklb-2.6.9/xklb/editdb/reddit_selftext.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.7/xklb/scripts/mining/substack.py` & `xklb-2.6.9/xklb/createdb/substack.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.7/xklb/scripts/mining/tildes.py` & `xklb-2.6.9/xklb/createdb/tildes.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.7/xklb/utils/arg_utils.py` & `xklb-2.6.9/xklb/utils/arg_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -140,15 +140,15 @@
                 getattr(args, "upper", False),
             ],
         ):
             if args.action in (SC.listen, SC.watch, SC.read):
                 args.limit = consts.DEFAULT_PLAY_QUEUE
             elif args.action in (SC.view):
                 args.limit = consts.DEFAULT_PLAY_QUEUE * 4
-            elif args.action in (SC.open_links):
+            elif args.action in (SC.links_open):
                 args.limit = consts.MANY_LINKS - 1
             elif args.action in (SC.download):
                 args.limit = consts.DEFAULT_PLAY_QUEUE * 60
     elif args.limit.lower() in ("inf", "all"):
         args.limit = None
```

### Comparing `xklb-2.6.7/xklb/utils/arggroups.py` & `xklb-2.6.9/xklb/utils/arggroups.py`

 * *Files 20% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 
 def capability_delete(parser):
     parser.add_argument(
         "--override-trash", "--override-rm", "--trash-cmd", default="trash", help="Custom trash command"
     )
     parser.add_argument(
         "--delete-files",
-        "--delete-file",
         "--trash",
         "--rm",
         action="store_true",
         help="Delete files from filesystem",
     )
 
 
@@ -39,85 +38,85 @@
     parser.add_argument("--file", "-f", help="File with one URL per line")
     parser.add_argument(
         "paths", nargs="*", default=argparse_utils.STDIN_DASH, action=argparse_utils.ArgparseArgsOrStdin
     )
 
 
 def sql_fs(parser):
-    parser.add_argument("--print", "-p", default="", const="p", nargs="?", help=argparse.SUPPRESS)
+    parser.add_argument("--print", "-p", default="", const="p", nargs="?")
     parser.add_argument("--cols", "--col", nargs="*", help="Include specific column(s) when printing")
 
-    parser.add_argument("--limit", "--queue", "--count", "-n", "-L", "-l", help=argparse.SUPPRESS)
+    parser.add_argument("--limit", "--queue", "--count", "-n", "-L", "-l")
     parser.add_argument("--offset", help=argparse.SUPPRESS)
-    parser.add_argument("--sort", "-u", nargs="+", help=argparse.SUPPRESS)
-    parser.add_argument("--random", "-r", action="store_true", help=argparse.SUPPRESS)
+    parser.add_argument("--sort", "-u", nargs="+", default=[])
+    parser.add_argument("--random", "-r", action="store_true")
 
-    parser.add_argument("--where", "-w", nargs="+", action="extend", default=[], help=argparse.SUPPRESS)
-    parser.add_argument("--include", "--search", "-s", nargs="+", action="extend", default=[], help=argparse.SUPPRESS)
-    parser.add_argument("--exclude", "-E", nargs="+", action="extend", default=[], help=argparse.SUPPRESS)
+    parser.add_argument("--where", "-w", nargs="+", action="extend", default=[])
+    parser.add_argument("--include", "--search", "-s", nargs="+", action="extend", default=[])
+    parser.add_argument("--exclude", "-E", nargs="+", action="extend", default=[])
     parser.add_argument("--exact", action="store_true")
     parser.add_argument("--flexible-search", "--or", "--flex", action="store_true")
     parser.add_argument("--no-fts", action="store_true")
 
     parser.add_argument("--ext", "-e", default=[], action=argparse_utils.ArgparseList)
 
     parser.add_argument(
         "--size",
         "-S",
         action="append",
         help="Only include files of specific sizes (uses the same syntax as fd-find)",
     )
 
-    parser.add_argument("--created-within", help=argparse.SUPPRESS)
-    parser.add_argument("--created-before", help=argparse.SUPPRESS)
-    parser.add_argument("--changed-within", "--modified-within", help=argparse.SUPPRESS)
-    parser.add_argument("--changed-before", "--modified-before", help=argparse.SUPPRESS)
-    parser.add_argument("--deleted-within", help=argparse.SUPPRESS)
-    parser.add_argument("--deleted-before", help=argparse.SUPPRESS)
+    parser.add_argument("--created-within")
+    parser.add_argument("--created-before")
+    parser.add_argument("--changed-within", "--modified-within")
+    parser.add_argument("--changed-before", "--modified-before")
+    parser.add_argument("--deleted-within")
+    parser.add_argument("--deleted-before")
     parser.add_argument("--downloaded-within", help=argparse.SUPPRESS)
     parser.add_argument("--downloaded-before", help=argparse.SUPPRESS)
     parser.add_argument("--played-within", help=argparse.SUPPRESS)
     parser.add_argument("--played-before", help=argparse.SUPPRESS)
 
 
 def sql_media(parser):
-    parser.add_argument("--online-media-only", "--online", action="store_true", help=argparse.SUPPRESS)
-    parser.add_argument("--local-media-only", "--local", action="store_true", help=argparse.SUPPRESS)
+    parser.add_argument("--online-media-only", "--online", action="store_true")
+    parser.add_argument("--local-media-only", "--local", action="store_true")
 
-    parser.add_argument("--no-video", "-vn", action="store_true", help=argparse.SUPPRESS)
-    parser.add_argument("--no-audio", "-an", action="store_true", help=argparse.SUPPRESS)
+    parser.add_argument("--no-video", "-vn", action="store_true")
+    parser.add_argument("--no-audio", "-an", action="store_true")
     parser.add_argument(
         "--no-subtitles",
         "--no-subtitle",
         "--no-subs",
         "--nosubs",
         "-sn",
         action="store_true",
         help=argparse.SUPPRESS,
     )
-    parser.add_argument("--subtitles", "--subtitle", "-sy", action="store_true", help=argparse.SUPPRESS)
+    parser.add_argument("--subtitles", "--subtitle", "-sy", action="store_true")
 
-    parser.add_argument("--duration", "-d", action="append", help=argparse.SUPPRESS)
+    parser.add_argument("--duration", "-d", action="append")
     parser.add_argument("--duration-from-size", action="append", help=argparse.SUPPRESS)
 
-    parser.add_argument("--portrait", "-portrait", action="store_true", help=argparse.SUPPRESS)
+    parser.add_argument("--portrait", action="store_true")
 
 
 def playback(parser):
-    parser.add_argument("--crop", "--zoom", "--stretch", "--fit", "--fill", action="store_true", help=argparse.SUPPRESS)
-    parser.add_argument("--loop", action="store_true", help=argparse.SUPPRESS)
-    parser.add_argument("--pause", action="store_true", help=argparse.SUPPRESS)
-    parser.add_argument("--start", "-vs", help=argparse.SUPPRESS)
-    parser.add_argument("--end", "-ve", help=argparse.SUPPRESS)
+    parser.add_argument("--crop", "--zoom", "--stretch", "--fit", "--fill", action="store_true")
+    parser.add_argument("--loop", action="store_true")
+    parser.add_argument("--pause", action="store_true")
+    parser.add_argument("--start", "-vs")
+    parser.add_argument("--end", "-ve")
     parser.add_argument("--volume", type=float)
 
-    parser.add_argument("--mpv-socket", help=argparse.SUPPRESS)
+    parser.add_argument("--mpv-socket")
     parser.add_argument("--auto-seek", action="store_true")
 
-    parser.add_argument("--override-player", "--player", help=argparse.SUPPRESS)
+    parser.add_argument("--override-player", "--player")
     parser.add_argument(
         "--ignore-errors",
         "--ignoreerrors",
         "-i",
         action="store_true",
         help="After a playback error continue to the next track instead of exiting",
     )
@@ -131,33 +130,32 @@
         const=10,
         nargs="?",
         help="Experimental escape hatch to open a folder glob limited to x number of files",
     )
 
 
 def post_actions(parser):
-    parser.add_argument("--exit-code-confirm", action="store_true", help=argparse.SUPPRESS)
+    parser.add_argument("--exit-code-confirm", action="store_true")
     parser.add_argument("--gui", action="store_true")
-    parser.add_argument("--keep-dir", "--keepdir", help=argparse.SUPPRESS)
-    parser.add_argument("--post-action", "--action", "-k", default="keep", help=argparse.SUPPRESS)
+    parser.add_argument("--keep-dir", "--keepdir")
+    parser.add_argument("--post-action", "--action", "-k", default="keep")
 
 
 def multiple_playback(parser):
     parser.add_argument(
         "--multiple-playback",
         "-m",
         default=False,
         nargs="?",
         const=consts.DEFAULT_MULTIPLE_PLAYBACK,
         type=int,
-        help=argparse.SUPPRESS,
     )
-    parser.add_argument("--screen-name", help=argparse.SUPPRESS)
-    parser.add_argument("--hstack", action="store_true", help=argparse.SUPPRESS)
-    parser.add_argument("--vstack", action="store_true", help=argparse.SUPPRESS)
+    parser.add_argument("--screen-name")
+    parser.add_argument("--hstack", action="store_true")
+    parser.add_argument("--vstack", action="store_true")
 
 
 def extractor(parser):
     parser.add_argument("--no-sanitize", action="store_true", help="Don't sanitize some common URL parameters")
     parser.add_argument(
         "--insert-only", "--no-extract", "--skip-extract", action="store_true"
     )  # TODO: move to its own subcommand
@@ -199,15 +197,15 @@
     parser.add_argument(
         "--unique-only", action="store_true", help="Include only 'unique' lines (not including originals or duplicates)"
     )
     parser.add_argument("--exclude-unique", "--no-unique", action="store_true", help="Exclude 'unique' lines")
 
 
 def operation_related(parser):
-    parser.add_argument("--related", "-R", action="count", default=0, help=argparse.SUPPRESS)
+    parser.add_argument("--related", "-R", action="count", default=0)
 
 
 def capability_clobber(parser):
     parser.add_argument("--replace", "--clobber", action="store_true")
     parser.add_argument("--no-replace", "--no-clobber", action="store_true")
```

### Comparing `xklb-2.6.7/xklb/utils/argparse_utils.py` & `xklb-2.6.9/xklb/utils/argparse_utils.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.7/xklb/utils/consts.py` & `xklb-2.6.9/xklb/utils/consts.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,38 +87,38 @@
     video = "video"
     filesystem = "filesystem"
     text = "text"
     image = "image"
 
 
 class SC:
-    fsadd = "fs-add"
-    fsupdate = "fs-update"
+    fs_add = "fs-add"
+    fs_update = "fs-update"
     watch = "watch"
     listen = "listen"
     filesystem = "filesystem"
-    tubeadd = "tube-add"
-    tubeupdate = "tube-update"
-    galleryadd = "gallery-add"
-    galleryupdate = "gallery-update"
-    tabs = "tabs"
-    open_links = "open-links"
+    tube_add = "tube-add"
+    tube_update = "tube-update"
+    gallery_add = "gallery-add"
+    gallery_update = "gallery-update"
+    tabs_open = "tabs-open"
+    links_open = "links-open"
     read = "read"
     view = "view"
     download = "download"
     block = "block"
     playlists = "playlists"
     download_status = "download-status"
     search = "search"
     history = "history"
-    bigdirs = "big-dirs"
-    diskusage = "disk-usage"
-    dedupe = "dedupe"
-    webadd = "web-add"
-    webupdate = "web-update"
+    big_dirs = "big-dirs"
+    disk_usage = "disk-usage"
+    dedupe_media = "dedupe"
+    web_add = "web-add"
+    web_update = "web-update"
 
 
 def reddit_frequency(frequency) -> str:
     mapper = {
         "daily": "day",
         "weekly": "week",
         "monthly": "month",
```

### Comparing `xklb-2.6.7/xklb/utils/db_utils.py` & `xklb-2.6.9/xklb/utils/db_utils.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.7/xklb/utils/devices.py` & `xklb-2.6.9/xklb/utils/devices.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-import argparse, os, platform, random, shutil, sys
+import os, platform, random, shutil, sys
 
-from xklb.utils import arggroups
 from xklb.utils.log_utils import log
 
 
 def get_ip_of_chromecast(device_name) -> str:
     from pychromecast import discovery
 
     cast_infos, browser = discovery.discover_listed_chromecasts(friendly_names=[device_name])
@@ -103,25 +102,7 @@
         grand_total += total
         mount_space.append((src_mount, used, free, total))
 
     return [
         {"mount": mount, "used": used / total_used, "free": free / total_free, "total": total / grand_total}
         for mount, used, free, total in mount_space
     ]
-
-
-def mount_stats() -> None:
-    parser = argparse.ArgumentParser(add_help=False)
-    arggroups.debug(parser)
-
-    parser.add_argument("mounts", nargs="+")
-    args = parser.parse_args()
-
-    space = get_mount_stats(args.mounts)
-
-    print("Relative disk dependence:")
-    for d in space:
-        print(f"{d['mount']}: {'#' * int(d['used'] * 80)} {d['used']:.1%}")
-
-    print("\nRelative free space:")
-    for d in space:
-        print(f"{d['mount']}: {'#' * int(d['free'] * 80)} {d['free']:.1%}")
```

### Comparing `xklb-2.6.7/xklb/utils/gui.py` & `xklb-2.6.9/xklb/utils/gui.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.7/xklb/utils/iterables.py` & `xklb-2.6.9/xklb/utils/iterables.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.7/xklb/utils/log_utils.py` & `xklb-2.6.9/xklb/utils/log_utils.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.7/xklb/utils/mpv_utils.py` & `xklb-2.6.9/xklb/utils/mpv_utils.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.7/xklb/utils/nums.py` & `xklb-2.6.9/xklb/utils/nums.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.7/xklb/utils/objects.py` & `xklb-2.6.9/xklb/utils/objects.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.7/xklb/utils/path_utils.py` & `xklb-2.6.9/xklb/utils/path_utils.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.7/xklb/utils/pd_utils.py` & `xklb-2.6.9/xklb/utils/pd_utils.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.7/xklb/utils/printing.py` & `xklb-2.6.9/xklb/utils/printing.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.7/xklb/utils/processes.py` & `xklb-2.6.9/xklb/utils/processes.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.7/xklb/utils/sql_utils.py` & `xklb-2.6.9/xklb/utils/sql_utils.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.7/xklb/utils/strings.py` & `xklb-2.6.9/xklb/utils/strings.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.7/xklb/utils/web.py` & `xklb-2.6.9/xklb/utils/web.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.7/xklb/assets/kotobago.png` & `xklb-2.6.9/xklb/assets/kotobago.png`

 * *Files identical despite different names*

### Comparing `xklb-2.6.7/.gitignore` & `xklb-2.6.9/.gitignore`

 * *Files identical despite different names*

### Comparing `xklb-2.6.7/pyproject.toml` & `xklb-2.6.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `xklb-2.6.7/.github/README.md` & `xklb-2.6.9/.github/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -80,69 +80,69 @@
     library tubeadd my.db $(xclip -selection c)
 
 #### 1a. Get new videos for saved playlists
 
 Tubeupdate will go through the list of added playlists and fetch metadata for
 any videos not previously seen.
 
-    library tubeupdate tube.db
+    library tube-update tube.db
 
 ### 2. Watch / Listen from websites
 
     library watch maker.db
 
 To stop playing press Ctrl+C in either the terminal or mpv
 
 </details>
 
 <details><summary>List all subcommands</summary>
 
     $ library
-    xk media library subcommands (v2.6.007)
+    xk media library subcommands (v2.6.009)
 
     Create database subcommands:
-    ╭───────────────┬────────────────────────────────────────────────────╮
-    │ fsadd         │ Add local media                                    │
-    ├───────────────┼────────────────────────────────────────────────────┤
-    │ tubeadd       │ Add online video media (yt-dlp)                    │
-    ├───────────────┼────────────────────────────────────────────────────┤
-    │ webadd        │ Add open-directory media                           │
-    ├───────────────┼────────────────────────────────────────────────────┤
-    │ galleryadd    │ Add online gallery media (gallery-dl)              │
-    ├───────────────┼────────────────────────────────────────────────────┤
-    │ tabsadd       │ Create a tabs database; Add URLs                   │
-    ├───────────────┼────────────────────────────────────────────────────┤
-    │ links-add     │ Create a link-scraping database                    │
-    ├───────────────┼────────────────────────────────────────────────────┤
-    │ siteadd       │ Auto-scrape website data to SQLITE                 │
-    ├───────────────┼────────────────────────────────────────────────────┤
-    │ redditadd     │ Create a reddit database; Add subreddits           │
-    ├───────────────┼────────────────────────────────────────────────────┤
-    │ pushshift     │ Convert pushshift data to reddit.db format (stdin) │
-    ├───────────────┼────────────────────────────────────────────────────┤
-    │ hnadd         │ Create / Update a Hacker News database             │
-    ├───────────────┼────────────────────────────────────────────────────┤
-    │ substack      │ Backup substack articles                           │
-    ├───────────────┼────────────────────────────────────────────────────┤
-    │ tildes        │ Backup tildes comments and topics                  │
-    ├───────────────┼────────────────────────────────────────────────────┤
-    │ places-import │ Import places of interest (POIs)                   │
-    ├───────────────┼────────────────────────────────────────────────────┤
-    │ add-row       │ Add arbitrary data to SQLITE                       │
-    ╰───────────────┴────────────────────────────────────────────────────╯
+    ╭───────────────┬──────────────────────────────────────────╮
+    │ fs-add        │ Add local media                          │
+    ├───────────────┼──────────────────────────────────────────┤
+    │ tube-add      │ Add online video media (yt-dlp)          │
+    ├───────────────┼──────────────────────────────────────────┤
+    │ web-add       │ Add open-directory media                 │
+    ├───────────────┼──────────────────────────────────────────┤
+    │ gallery-add   │ Add online gallery media (gallery-dl)    │
+    ├───────────────┼──────────────────────────────────────────┤
+    │ tabs-add      │ Create a tabs database; Add URLs         │
+    ├───────────────┼──────────────────────────────────────────┤
+    │ links-add     │ Create a link-scraping database          │
+    ├───────────────┼──────────────────────────────────────────┤
+    │ site-add      │ Auto-scrape website data to SQLITE       │
+    ├───────────────┼──────────────────────────────────────────┤
+    │ reddit-add    │ Create a reddit database; Add subreddits │
+    ├───────────────┼──────────────────────────────────────────┤
+    │ hn-add        │ Create / Update a Hacker News database   │
+    ├───────────────┼──────────────────────────────────────────┤
+    │ substack      │ Backup substack articles                 │
+    ├───────────────┼──────────────────────────────────────────┤
+    │ tildes        │ Backup tildes comments and topics        │
+    ├───────────────┼──────────────────────────────────────────┤
+    │ places-import │ Import places of interest (POIs)         │
+    ├───────────────┼──────────────────────────────────────────┤
+    │ row-add       │ Add arbitrary data to SQLITE             │
+    ╰───────────────┴──────────────────────────────────────────╯
 
     Text subcommands:
     ╭────────────────┬─────────────────────────────────────────────╮
     │ cluster-sort   │ Sort text and images by similarity          │
     ├────────────────┼─────────────────────────────────────────────┤
     │ extract-links  │ Extract inner links from lists of web links │
     ├────────────────┼─────────────────────────────────────────────┤
     │ extract-text   │ Extract human text from lists of web links  │
     ├────────────────┼─────────────────────────────────────────────┤
     │ markdown-links │ Extract titles from lists of web links      │
+    ├────────────────┼─────────────────────────────────────────────┤
+    │ nouns          │ Unstructured text -> compound nouns (stdin) │
     ╰────────────────┴─────────────────────────────────────────────╯
 
     Folder subcommands:
     ╭───────────────┬──────────────────────────────────────────────────╮
     │ merge-folders │ Merge two or more file trees                     │
     ├───────────────┼──────────────────────────────────────────────────┤
     │ relmv         │ Move files preserving parent folder hierarchy    │
@@ -191,92 +191,92 @@
     │ disk-usage  │ Show disk usage                │
     ├─────────────┼────────────────────────────────┤
     │ mount-stats │ Show some relative mount stats │
     ├─────────────┼────────────────────────────────┤
     │ big-dirs    │ Show large folders             │
     ├─────────────┼────────────────────────────────┤
     │ search-db   │ Search a SQLITE database       │
-    ├─────────────┼────────────────────────────────┤
-    │ optimize    │ Re-optimize database           │
     ╰─────────────┴────────────────────────────────╯
 
     Media Database subcommands:
     ╭─────────────────┬────────────────────────────────╮
-    │ tabs            │ Open your tabs for the day     │
-    ├─────────────────┼────────────────────────────────┤
     │ block           │ Block a channel                │
     ├─────────────────┼────────────────────────────────┤
     │ playlists       │ List stored playlists          │
     ├─────────────────┼────────────────────────────────┤
     │ download        │ Download media                 │
     ├─────────────────┼────────────────────────────────┤
     │ download-status │ Show download status           │
     ├─────────────────┼────────────────────────────────┤
     │ redownload      │ Re-download deleted/lost media │
     ├─────────────────┼────────────────────────────────┤
     │ history         │ Show some playback statistics  │
     ├─────────────────┼────────────────────────────────┤
     │ search          │ Search captions / subtitles    │
+    ├─────────────────┼────────────────────────────────┤
+    │ optimize        │ Re-optimize database           │
     ╰─────────────────┴────────────────────────────────╯
 
     Playback subcommands:
     ╭────────────┬───────────────────────────────────────────────────╮
     │ watch      │ Watch / Listen                                    │
     ├────────────┼───────────────────────────────────────────────────┤
     │ now        │ Show what is currently playing                    │
     ├────────────┼───────────────────────────────────────────────────┤
     │ next       │ Play next file and optionally delete current file │
     ├────────────┼───────────────────────────────────────────────────┤
     │ stop       │ Stop all playback                                 │
     ├────────────┼───────────────────────────────────────────────────┤
     │ pause      │ Pause all playback                                │
     ├────────────┼───────────────────────────────────────────────────┤
-    │ open-links │ Open links from link dbs                          │
+    │ tabs-open  │ Open your tabs for the day                        │
+    ├────────────┼───────────────────────────────────────────────────┤
+    │ links-open │ Open links from link dbs                          │
     ├────────────┼───────────────────────────────────────────────────┤
     │ surf       │ Auto-load browser tabs in a streaming way (stdin) │
     ╰────────────┴───────────────────────────────────────────────────╯
 
     Database enrichment subcommands:
-    ╭────────────────────┬────────────────────────────────────────╮
-    │ dedupe-db          │ Dedupe SQLITE tables                   │
-    ├────────────────────┼────────────────────────────────────────┤
-    │ dedupe-media       │ Dedupe similar media                   │
-    ├────────────────────┼────────────────────────────────────────┤
-    │ merge-online-local │ Merge online and local data            │
-    ├────────────────────┼────────────────────────────────────────┤
-    │ mpv-watchlater     │ Import mpv watchlater files to history │
-    ├────────────────────┼────────────────────────────────────────┤
-    │ reddit-selftext    │ Copy selftext links to media table     │
-    ├────────────────────┼────────────────────────────────────────┤
-    │ tabs-shuffle       │ Randomize tabs.db a bit                │
-    ╰────────────────────┴────────────────────────────────────────╯
+    ╭────────────────────┬────────────────────────────────────────────────────╮
+    │ dedupe-db          │ Dedupe SQLITE tables                               │
+    ├────────────────────┼────────────────────────────────────────────────────┤
+    │ dedupe-media       │ Dedupe similar media                               │
+    ├────────────────────┼────────────────────────────────────────────────────┤
+    │ merge-online-local │ Merge online and local data                        │
+    ├────────────────────┼────────────────────────────────────────────────────┤
+    │ mpv-watchlater     │ Import mpv watchlater files to history             │
+    ├────────────────────┼────────────────────────────────────────────────────┤
+    │ reddit-selftext    │ Copy selftext links to media table                 │
+    ├────────────────────┼────────────────────────────────────────────────────┤
+    │ tabs-shuffle       │ Randomize tabs.db a bit                            │
+    ├────────────────────┼────────────────────────────────────────────────────┤
+    │ pushshift          │ Convert pushshift data to reddit.db format (stdin) │
+    ╰────────────────────┴────────────────────────────────────────────────────╯
 
     Update database subcommands:
-    ╭───────────────┬─────────────────────────────────╮
-    │ fsupdate      │ Update local media              │
-    ├───────────────┼─────────────────────────────────┤
-    │ tubeupdate    │ Update online video media       │
-    ├───────────────┼─────────────────────────────────┤
-    │ webupdate     │ Update open-directory media     │
-    ├───────────────┼─────────────────────────────────┤
-    │ galleryupdate │ Update online gallery media     │
-    ├───────────────┼─────────────────────────────────┤
-    │ links-update  │ Update a link-scraping database │
-    ├───────────────┼─────────────────────────────────┤
-    │ redditupdate  │ Update reddit media             │
-    ╰───────────────┴─────────────────────────────────╯
+    ╭────────────────┬─────────────────────────────────╮
+    │ fs-update      │ Update local media              │
+    ├────────────────┼─────────────────────────────────┤
+    │ tube-update    │ Update online video media       │
+    ├────────────────┼─────────────────────────────────┤
+    │ web-update     │ Update open-directory media     │
+    ├────────────────┼─────────────────────────────────┤
+    │ gallery-update │ Update online gallery media     │
+    ├────────────────┼─────────────────────────────────┤
+    │ links-update   │ Update a link-scraping database │
+    ├────────────────┼─────────────────────────────────┤
+    │ reddit-update  │ Update reddit media             │
+    ╰────────────────┴─────────────────────────────────╯
 
     Misc subcommands:
-    ╭────────────────┬─────────────────────────────────────────────╮
-    │ export-text    │ Export HTML files from SQLite databases     │
-    ├────────────────┼─────────────────────────────────────────────┤
-    │ dedupe-czkawka │ Process czkawka diff output                 │
-    ├────────────────┼─────────────────────────────────────────────┤
-    │ nouns          │ Unstructured text -> compound nouns (stdin) │
-    ╰────────────────┴─────────────────────────────────────────────╯
+    ╭────────────────┬─────────────────────────────────────────╮
+    │ export-text    │ Export HTML files from SQLite databases │
+    ├────────────────┼─────────────────────────────────────────┤
+    │ dedupe-czkawka │ Process czkawka diff output             │
+    ╰────────────────┴─────────────────────────────────────────╯
 
 
 </details>
 
 ## Examples
 
 ### Watch online media on your PC
@@ -511,20 +511,20 @@
 </details>
 
 ## Usage
 
 
 ### Create database subcommands
 
-###### fsadd
+###### fs-add
 
 <details><summary>Add local media</summary>
 
-    $ library fsadd -h
-    usage: library fsadd [(--video) | --audio | --image |  --text | --filesystem] DATABASE PATH ...
+    $ library fs-add -h
+    usage: library fs-add [(--video) | --audio | --image |  --text | --filesystem] DATABASE PATH ...
 
     The default database type is video:
         library fsadd tv.db ./tv/
         library fsadd --video tv.db ./tv/  # equivalent
 
     You can also create audio databases. Both audio and video use ffmpeg to read metadata:
         library fsadd --audio audio.db ./music/
@@ -567,20 +567,20 @@
 
         library fsadd audio.db --move ~/library/ ./added_folder/
         This will run destination paths through `library christen` and move files relative to the added folder root
 
 
 </details>
 
-###### tubeadd
+###### tube-add
 
 <details><summary>Add online video media (yt-dlp)</summary>
 
-    $ library tubeadd -h
-    usage: library tubeadd [--safe] [--extra] [--subs] [--auto-subs] DATABASE URLS ...
+    $ library tube-add -h
+    usage: library tube-add [--safe] [--extra] [--subs] [--auto-subs] DATABASE URLS ...
 
     Create a dl database / add links to an existing database
 
         library tubeadd dl.db https://www.youdl.com/c/BranchEducation/videos
 
     Add links from a line-delimited file
 
@@ -592,24 +592,24 @@
 
     Fetch extra metadata:
 
         By default tubeadd will quickly add media at the expense of less metadata.
         If you plan on using `library download` then it doesn't make sense to use `--extra`.
         Downloading will add the extra metadata automatically to the database.
         You can always fetch more metadata later via tubeupdate:
-        library tubeupdate tw.db --extra
+        library tube-update tw.db --extra
 
 
 </details>
 
-###### webadd
+###### web-add
 
 <details><summary>Add open-directory media</summary>
 
-    $ library webadd -h
+    $ library web-add -h
     usage: library web-add [(--filesystem) | --video | --audio | --image | --text] DATABASE URL ...
 
     Scan open directories
 
         library web-add open_dir.db --video http://1.1.1.1/
 
     Check download size of all videos matching some criteria
@@ -653,36 +653,36 @@
 
         library download --fs open_dir.db --prefix ~/d/dump/video/ -w 'id in (select media_id from history)'
 
 
 
 </details>
 
-###### galleryadd
+###### gallery-add
 
 <details><summary>Add online gallery media (gallery-dl)</summary>
 
-    $ library galleryadd -h
-    usage: library galleryadd DATABASE URLS
+    $ library gallery-add -h
+    usage: library gallery-add DATABASE URLS
 
     Add gallery_dl URLs to download later or periodically update
 
     If you have many URLs use stdin
 
         cat ./my-favorite-manhwa.txt | library galleryadd your.db --insert-only -
 
 
 </details>
 
-###### tabsadd
+###### tabs-add
 
 <details><summary>Create a tabs database; Add URLs</summary>
 
-    $ library tabsadd -h
-    usage: library tabsadd [--frequency daily weekly (monthly) quarterly yearly] [--no-sanitize] DATABASE URLS ...
+    $ library tabs-add -h
+    usage: library tabs-add [--frequency daily weekly (monthly) quarterly yearly] [--no-sanitize] DATABASE URLS ...
 
     Adding one URL:
 
         library tabsadd -f daily tabs.db https://wiby.me/surprise/
 
         Depending on your shell you may need to escape the URL (add quotes)
 
@@ -800,36 +800,36 @@
         library links-add --path-include viewtopic.php --cookies-from-browser firefox \
         --page-key start --page-start 0 --page-step 50 --fixed-pages 14 --stop-pages-no-match 1 \
         plab.db https://plab/forum/tracker.php?o=(string replace ' ' \n -- 1 4 7 10 15)&s=2&tm=-1&f=(string replace ' ' \n -- 1670 1768 60 1671 1644 1672 1111 508 555 1112 1718 1143 1717 1851 1713 1712 1775 1674 902 1675 36 1830 1803 1831 1741 1676 1677 1780 1110 1124 1784 1769 1793 1797 1804 1819 1825 1836 1842 1846 1857 1861 1867 1451 1788 1789 1792 1798 1805 1820 1826 1837 1843 1847 1856 1862 1868 284 1853 1823 1800 1801 1719 997 1818 1849 1711 1791 1762)
 
 
 </details>
 
-###### siteadd
+###### site-add
 
 <details><summary>Auto-scrape website data to SQLITE</summary>
 
-    $ library siteadd -h
+    $ library site-add -h
     usage: library site-add DATABASE PATH ... [--auto-pager] [--poke] [--local-html] [--file FILE]
 
     Extract data from website requests to a database
 
         library siteadd jobs.st.db --poke https://hk.jobsdb.com/hk/search-jobs/python/
 
     Run with `-vv` to see and interact with the browser
 
 
 </details>
 
-###### redditadd
+###### reddit-add
 
 <details><summary>Create a reddit database; Add subreddits</summary>
 
-    $ library redditadd -h
-    usage: library redditadd [--lookback N_DAYS] [--praw-site bot1] DATABASE URLS ...
+    $ library reddit-add -h
+    usage: library reddit-add [--lookback N_DAYS] [--praw-site bot1] DATABASE URLS ...
 
     Fetch data for redditors and reddits:
 
         library redditadd interesting.db https://old.reddit.com/r/coolgithubprojects/ https://old.reddit.com/user/Diastro
 
     If you have a file with a list of subreddits you can do this:
 
@@ -843,45 +843,20 @@
     Also, it may be the case that reddit's API (praw) will stop working in the near future. For both of these problems
     my suggestion is to use pushshift data.
     You can find more info here: https://github.com/chapmanjacobd/reddit_mining#how-was-this-made
 
 
 </details>
 
-###### pushshift
-
-<details><summary>Convert pushshift data to reddit.db format (stdin)</summary>
-
-    $ library pushshift -h
-    usage: library pushshift DATABASE < stdin
-
-    Download data (about 600GB jsonl.zst; 6TB uncompressed)
-
-        wget -e robots=off -r -k -A zst https://files.pushshift.io/reddit/submissions/
-
-    Load data from files via unzstd
-
-        unzstd --memory=2048MB --stdout RS_2005-07.zst | library pushshift pushshift.db
-
-    Or multiple (output is about 1.5TB SQLITE fts-searchable):
-
-        for f in psaw/files.pushshift.io/reddit/submissions/*.zst
-            echo "unzstd --memory=2048MB --stdout $f | library pushshift (basename $f).db"
-            library optimize (basename $f).db
-        end | parallel -j5
-
-
-</details>
-
-###### hnadd
+###### hn-add
 
 <details><summary>Create / Update a Hacker News database</summary>
 
-    $ library hnadd -h
-    usage: library hnadd [--oldest] DATABASE
+    $ library hn-add -h
+    usage: library hn-add [--oldest] DATABASE
 
     Fetch latest stories first:
 
         library hnadd hn.db -v
         Fetching 154873 items (33212696 to 33367569)
         Saving comment 33367568
         Saving comment 33367543
@@ -933,24 +908,24 @@
     usage: library places-import DATABASE PATH ...
 
     Load POIs from Google Maps Google Takeout
 
 
 </details>
 
-###### add-row
+###### row-add
 
 <details><summary>Add arbitrary data to SQLITE</summary>
 
-    $ library add-row -h
-    usage: library add-row DATABASE [--table-name TABLE_NAME]
+    $ library row-add -h
+    usage: library row-add DATABASE [--table-name TABLE_NAME]
 
     Add a row to sqlite
 
-        library add-row t.db --test_b 1 --test-a 2
+        library row-add t.db --test_b 1 --test-a 2
 
         ### media (1 rows)
         |   test_b |   test_a |
         |----------|----------|
         |        1 |        2 |
 
 
@@ -1041,14 +1016,43 @@
     Sorting suggestions
 
         lb extract-text --skip-links --local-file (cb -t text/html | psub) | lb cs --groups | jq -r '.[] | .grouped_paths | "\n" + join("\n")'
 
 
 </details>
 
+###### markdown-links
+
+<details><summary>Extract titles from lists of web links</summary>
+
+    $ library markdown-links -h
+    usage: usage: library markdown-links URL ... [--cookies COOKIES] [--cookies-from-browser BROWSER[+KEYRING][:PROFILE][::CONTAINER]] [--firefox] [--chrome] [--allow-insecure] [--scroll] [--manual] [--auto-pager] [--poke] [--file FILE]
+
+    Convert URLs into Markdown links with page titles filled in
+
+        $ lb markdown-links https://www.youtube.com/watch?v=IgZDDW-NXDE
+        [Work For Peace](https://www.youtube.com/watch?v=IgZDDW-NXDE)
+
+
+</details>
+
+###### nouns
+
+<details><summary>Unstructured text -> compound nouns (stdin)</summary>
+
+    $ library nouns -h
+    usage: library nouns (stdin)
+
+    Extract compound nouns and phrases from unstructured mixed HTML plain text
+
+        xsv select text hn_comment_202210242109.csv | library nouns | sort | uniq -c | sort --numeric-sort
+
+
+</details>
+
 ### Folder subcommands
 
 ###### merge-folders
 
 <details><summary>Merge two or more file trees</summary>
 
     $ library merge-folders -h
@@ -1254,15 +1258,15 @@
 </details>
 
 ###### sample-compare
 
 <details><summary>Compare files using sample-hash and other shortcuts</summary>
 
     $ library sample-compare -h
-    usage: library sample-hash [--threads 10] [--chunk-size BYTES] [--gap BYTES OR 0.0-1.0*FILESIZE] PATH ...
+    usage: library sample-compare [--threads 10] [--chunk-size BYTES] [--gap BYTES OR 0.0-1.0*FILESIZE] PATH ...
 
     Convenience subcommand to compare multiple files using sample-hash
 
 
 </details>
 
 ### Tabular data subcommands
@@ -1612,14 +1616,26 @@
         | /home/xk/github/xk/lb/__pypackages__/3.11/lib/jedi/third_party/typeshed/third_party/2and3/requests/packages/urllib3/packages/ssl_match_hostname/__init__.pyi        | 88 Bytes |
         | /home/xk/github/xk/lb/__pypackages__/3.11/lib/jedi/third_party/typeshed/third_party/2and3/requests/packages/urllib3/packages/ssl_match_hostname/_implementation.pyi | 81 Bytes |
 
 
 
 </details>
 
+###### mount-stats
+
+<details><summary>Show some relative mount stats</summary>
+
+    $ library mount-stats -h
+    usage: library mount-stats MOUNTPOINT ...
+
+    Print relative use and free for multiple mount points
+
+
+</details>
+
 ###### big-dirs
 
 <details><summary>Show large folders</summary>
 
     $ library big-dirs -h
     usage: library big-dirs DATABASE [--limit (4000)] [--depth (0)] [--sort-groups-by deleted | played] [--size=+5MB]
 
@@ -1649,104 +1665,16 @@
     usage: library search-db DATABASE TABLE SEARCH ... [--delete-rows]
 
     Search all columns in a SQLITE table. If the table does not exist, uses the table which startswith (if only one match)
 
 
 </details>
 
-###### optimize
-
-<details><summary>Re-optimize database</summary>
-
-    $ library optimize -h
-    usage: library optimize DATABASE [--force]
-
-    Optimize library databases
-
-    The force flag is usually unnecessary and it can take much longer
-
-
-</details>
-
 ### Media Database subcommands
 
-###### tabs
-
-<details><summary>Open your tabs for the day</summary>
-
-    $ library tabs -h
-    usage: library tabs DATABASE
-
-    Tabs is meant to run **once per day**. Here is how you would configure it with `crontab`:
-
-        45 9 * * * DISPLAY=:0 library tabs /home/my/tabs.db
-
-    If things aren't working you can use `at` to simulate a similar environment as `cron`
-
-        echo 'fish -c "export DISPLAY=:0 && library tabs /full/path/to/tabs.db"' | at NOW
-
-    You can also invoke tabs manually:
-
-        library tabs -L 1  # open one tab
-
-    Print URLs
-
-        library tabs -w "frequency='yearly'" -p
-        ╒════════════════════════════════════════════════════════════════╤═════════════╤══════════════╕
-        │ path                                                           │ frequency   │ time_valid   │
-        ╞════════════════════════════════════════════════════════════════╪═════════════╪══════════════╡
-        │ https://old.reddit.com/r/Autonomia/top/?sort=top&t=year        │ yearly      │ Dec 31 1970  │
-        ├────────────────────────────────────────────────────────────────┼─────────────┼──────────────┤
-        │ https://old.reddit.com/r/Cyberpunk/top/?sort=top&t=year        │ yearly      │ Dec 31 1970  │
-        ├────────────────────────────────────────────────────────────────┼─────────────┼──────────────┤
-        │ https://old.reddit.com/r/ExperiencedDevs/top/?sort=top&t=year  │ yearly      │ Dec 31 1970  │
-
-        ...
-
-        ╘════════════════════════════════════════════════════════════════╧═════════════╧══════════════╛
-
-    View how many yearly tabs you have:
-
-        library tabs -w "frequency='yearly'" -p a
-        ╒═══════════╤═════════╕
-        │ path      │   count │
-        ╞═══════════╪═════════╡
-        │ Aggregate │     134 │
-        ╘═══════════╧═════════╛
-
-    Delete URLs
-
-        library tabs -p -s cyber
-        ╒═══════════════════════════════════════╤═════════════╤══════════════╕
-        │ path                                  │ frequency   │ time_valid   │
-        ╞═══════════════════════════════════════╪═════════════╪══════════════╡
-        │ https://old.reddit.com/r/cyberDeck/to │ yearly      │ Dec 31 1970  │
-        │ p/?sort=top&t=year                    │             │              │
-        ├───────────────────────────────────────┼─────────────┼──────────────┤
-        │ https://old.reddit.com/r/Cyberpunk/to │ yearly      │ Aug 29 2023  │
-        │ p/?sort=top&t=year                    │             │              │
-        ├───────────────────────────────────────┼─────────────┼──────────────┤
-        │ https://www.reddit.com/r/cyberDeck/   │ yearly      │ Sep 05 2023  │
-        ╘═══════════════════════════════════════╧═════════════╧══════════════╛
-        library tabs -p -w "path='https://www.reddit.com/r/cyberDeck/'" --delete-rows
-        Removed 1 metadata records
-        library tabs -p -s cyber
-        ╒═══════════════════════════════════════╤═════════════╤══════════════╕
-        │ path                                  │ frequency   │ time_valid   │
-        ╞═══════════════════════════════════════╪═════════════╪══════════════╡
-        │ https://old.reddit.com/r/cyberDeck/to │ yearly      │ Dec 31 1970  │
-        │ p/?sort=top&t=year                    │             │              │
-        ├───────────────────────────────────────┼─────────────┼──────────────┤
-        │ https://old.reddit.com/r/Cyberpunk/to │ yearly      │ Aug 29 2023  │
-        │ p/?sort=top&t=year                    │             │              │
-        ╘═══════════════════════════════════════╧═════════════╧══════════════╛
-
-
-</details>
-
 ###### block
 
 <details><summary>Block a channel</summary>
 
     $ library block -h
     usage: library block DATABASE URLS ...
 
@@ -2140,14 +2068,28 @@
     Search and open file
 
         library search fts.db 'two words' --open
 
 
 </details>
 
+###### optimize
+
+<details><summary>Re-optimize database</summary>
+
+    $ library optimize -h
+    usage: library optimize DATABASE [--force]
+
+    Optimize library databases
+
+    The force flag is usually unnecessary and it can take much longer
+
+
+</details>
+
 ### Playback subcommands
 
 ###### watch
 
 <details><summary>Watch / Listen</summary>
 
     $ library watch -h
@@ -2156,16 +2098,14 @@
     Control playback:
         To stop playback press Ctrl-C in either the terminal or mpv
 
         Create global shortcuts in your desktop environment by sending commands to mpv_socket:
         echo 'playlist-next force' | socat - /tmp/mpv_socket
 
     Override the default player (mpv):
-        library does a lot of things to try to automatically use your preferred media player
-        but if it doesn't guess right you can make it explicit:
         library watch --player "vlc --vlc-opts"
 
     Cast to chromecast groups:
         library watch --cast --cast-to "Office pair"
         library watch -ct "Office pair"  # equivalent
         If you don't know the exact name of your chromecast group run `catt scan`
 
@@ -2528,20 +2468,94 @@
                 qdbus-qt5 org.kde.KWin /KWin reconfigure
             end
 
 
 
 </details>
 
-###### open-links
+###### tabs-open
+
+<details><summary>Open your tabs for the day</summary>
+
+    $ library tabs-open -h
+    usage: library tabs-open DATABASE
+
+    Tabs is meant to run **once per day**. Here is how you would configure it with `crontab`:
+
+        45 9 * * * DISPLAY=:0 library tabs /home/my/tabs.db
+
+    If things aren't working you can use `at` to simulate a similar environment as `cron`
+
+        echo 'fish -c "export DISPLAY=:0 && library tabs /full/path/to/tabs.db"' | at NOW
+
+    You can also invoke tabs manually:
+
+        library tabs -L 1  # open one tab
+
+    Print URLs
+
+        library tabs -w "frequency='yearly'" -p
+        ╒════════════════════════════════════════════════════════════════╤═════════════╤══════════════╕
+        │ path                                                           │ frequency   │ time_valid   │
+        ╞════════════════════════════════════════════════════════════════╪═════════════╪══════════════╡
+        │ https://old.reddit.com/r/Autonomia/top/?sort=top&t=year        │ yearly      │ Dec 31 1970  │
+        ├────────────────────────────────────────────────────────────────┼─────────────┼──────────────┤
+        │ https://old.reddit.com/r/Cyberpunk/top/?sort=top&t=year        │ yearly      │ Dec 31 1970  │
+        ├────────────────────────────────────────────────────────────────┼─────────────┼──────────────┤
+        │ https://old.reddit.com/r/ExperiencedDevs/top/?sort=top&t=year  │ yearly      │ Dec 31 1970  │
+
+        ...
+
+        ╘════════════════════════════════════════════════════════════════╧═════════════╧══════════════╛
+
+    View how many yearly tabs you have:
+
+        library tabs -w "frequency='yearly'" -p a
+        ╒═══════════╤═════════╕
+        │ path      │   count │
+        ╞═══════════╪═════════╡
+        │ Aggregate │     134 │
+        ╘═══════════╧═════════╛
+
+    Delete URLs
+
+        library tabs -p -s cyber
+        ╒═══════════════════════════════════════╤═════════════╤══════════════╕
+        │ path                                  │ frequency   │ time_valid   │
+        ╞═══════════════════════════════════════╪═════════════╪══════════════╡
+        │ https://old.reddit.com/r/cyberDeck/to │ yearly      │ Dec 31 1970  │
+        │ p/?sort=top&t=year                    │             │              │
+        ├───────────────────────────────────────┼─────────────┼──────────────┤
+        │ https://old.reddit.com/r/Cyberpunk/to │ yearly      │ Aug 29 2023  │
+        │ p/?sort=top&t=year                    │             │              │
+        ├───────────────────────────────────────┼─────────────┼──────────────┤
+        │ https://www.reddit.com/r/cyberDeck/   │ yearly      │ Sep 05 2023  │
+        ╘═══════════════════════════════════════╧═════════════╧══════════════╛
+        library tabs -p -w "path='https://www.reddit.com/r/cyberDeck/'" --delete-rows
+        Removed 1 metadata records
+        library tabs -p -s cyber
+        ╒═══════════════════════════════════════╤═════════════╤══════════════╕
+        │ path                                  │ frequency   │ time_valid   │
+        ╞═══════════════════════════════════════╪═════════════╪══════════════╡
+        │ https://old.reddit.com/r/cyberDeck/to │ yearly      │ Dec 31 1970  │
+        │ p/?sort=top&t=year                    │             │              │
+        ├───────────────────────────────────────┼─────────────┼──────────────┤
+        │ https://old.reddit.com/r/Cyberpunk/to │ yearly      │ Aug 29 2023  │
+        │ p/?sort=top&t=year                    │             │              │
+        ╘═══════════════════════════════════════╧═════════════╧══════════════╛
+
+
+</details>
+
+###### links-open
 
 <details><summary>Open links from link dbs</summary>
 
-    $ library open-links -h
-    usage: library open-links DATABASE [search] [--title] [--title-prefix TITLE_PREFIX]
+    $ library links-open -h
+    usage: library links-open DATABASE [search] [--title] [--title-prefix TITLE_PREFIX]
 
     Open links from a links db
 
         wget https://github.com/chapmanjacobd/library/raw/main/example_dbs/music.korea.ln.db
         library open-links music.korea.ln.db
 
     Only open links once
@@ -2698,36 +2712,61 @@
         library tabs-shuffle tabs.db -d  31 -f monthly
         library tabs-shuffle tabs.db -d  90 -f quarterly
         library tabs-shuffle tabs.db -d 365 -f yearly
 
 
 </details>
 
+###### pushshift
+
+<details><summary>Convert pushshift data to reddit.db format (stdin)</summary>
+
+    $ library pushshift -h
+    usage: library pushshift DATABASE < stdin
+
+    Download data (about 600GB jsonl.zst; 6TB uncompressed)
+
+        wget -e robots=off -r -k -A zst https://files.pushshift.io/reddit/submissions/
+
+    Load data from files via unzstd
+
+        unzstd --memory=2048MB --stdout RS_2005-07.zst | library pushshift pushshift.db
+
+    Or multiple (output is about 1.5TB SQLITE fts-searchable):
+
+        for f in psaw/files.pushshift.io/reddit/submissions/*.zst
+            echo "unzstd --memory=2048MB --stdout $f | library pushshift (basename $f).db"
+            library optimize (basename $f).db
+        end | parallel -j5
+
+
+</details>
+
 ### Update database subcommands
 
-###### fsupdate
+###### fs-update
 
 <details><summary>Update local media</summary>
 
-    $ library fsupdate -h
-    usage: library fsupdate DATABASE
+    $ library fs-update -h
+    usage: library fs-update DATABASE
 
     Update each path previously saved:
 
         library fsupdate video.db
 
 
 </details>
 
-###### tubeupdate
+###### tube-update
 
 <details><summary>Update online video media</summary>
 
-    $ library tubeupdate -h
-    usage: library tubeupdate [--audio | --video] DATABASE
+    $ library tube-update -h
+    usage: library tube-update [--audio | --video] DATABASE
 
     Fetch the latest videos for every playlist saved in your database
 
         library tubeupdate educational.db
 
     Fetch extra metadata:
 
@@ -2739,33 +2778,33 @@
     Remove duplicate playlists:
 
         lb dedupe-db video.db playlists --bk extractor_playlist_id
 
 
 </details>
 
-###### webupdate
+###### web-update
 
 <details><summary>Update open-directory media</summary>
 
-    $ library webupdate -h
+    $ library web-update -h
     usage: library web-update DATABASE
 
     Update saved open directories
 
 
 
 </details>
 
-###### galleryupdate
+###### gallery-update
 
 <details><summary>Update online gallery media</summary>
 
-    $ library galleryupdate -h
-    usage: library galleryupdate DATABASE URLS
+    $ library gallery-update -h
+    usage: library gallery-update DATABASE URLS
 
     Check previously saved gallery_dl URLs for new content
 
 
 </details>
 
 ###### links-update
@@ -2778,20 +2817,20 @@
     Fetch new links from each path previously saved
 
         library links-update links.db
 
 
 </details>
 
-###### redditupdate
+###### reddit-update
 
 <details><summary>Update reddit media</summary>
 
-    $ library redditupdate -h
-    usage: library redditupdate [--audio | --video] [--lookback N_DAYS] [--praw-site bot1] DATABASE
+    $ library reddit-update -h
+    usage: library reddit-update [--audio | --video] [--lookback N_DAYS] [--praw-site bot1] DATABASE
 
     Fetch the latest posts for every subreddit/redditor saved in your database
 
         library redditupdate edu_subreddits.db
 
 
 </details>
@@ -2806,14 +2845,28 @@
     usage: library export-text DATABASE
 
     Generate HTML files from SQLite databases
 
 
 </details>
 
+###### dedupe-czkawka
+
+<details><summary>Process czkawka diff output</summary>
+
+    $ library dedupe-czkawka -h
+    usage: library dedupe-czkawka [--volume VOLUME] [--auto-seek] [--ignore-errors] [--folder] [--folder-glob [FOLDER_GLOB]] [--replace] [--no-replace] [--override-trash OVERRIDE_TRASH] [--delete-files] [--gui]
+               [--auto-select-min-ratio AUTO_SELECT_MIN_RATIO] [--all-keep] [--all-left] [--all-right] [--all-delete] [--verbose]
+               czkawka_dupes_output_path
+
+    Choose which duplicate to keep by opening both side-by-side in mpv
+
+
+</details>
+
 
 <details><summary>Chicken mode</summary>
 
 
            ////////////////////////
           ////////////////////////|
          //////////////////////// |
```

### Comparing `xklb-2.6.7/PKG-INFO` & `xklb-2.6.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: xklb
-Version: 2.6.7
+Version: 2.6.9
 Summary: xk library
 Project-URL: documentation, https://github.com/chapmanjacobd/library#usage
 Project-URL: homepage, https://github.com/chapmanjacobd/library#readme
 Project-URL: repository, https://github.com/chapmanjacobd/library/
 Author-email: Jacob Chapman <7908073+chapmanjacobd@users.noreply.github.com>
 License: BSD 3-Clause No Nuclear License
         
@@ -168,69 +168,69 @@
     library tubeadd my.db $(xclip -selection c)
 
 #### 1a. Get new videos for saved playlists
 
 Tubeupdate will go through the list of added playlists and fetch metadata for
 any videos not previously seen.
 
-    library tubeupdate tube.db
+    library tube-update tube.db
 
 ### 2. Watch / Listen from websites
 
     library watch maker.db
 
 To stop playing press Ctrl+C in either the terminal or mpv
 
 </details>
 
 <details><summary>List all subcommands</summary>
 
     $ library
-    xk media library subcommands (v2.6.007)
+    xk media library subcommands (v2.6.009)
 
     Create database subcommands:
-    ╭───────────────┬────────────────────────────────────────────────────╮
-    │ fsadd         │ Add local media                                    │
-    ├───────────────┼────────────────────────────────────────────────────┤
-    │ tubeadd       │ Add online video media (yt-dlp)                    │
-    ├───────────────┼────────────────────────────────────────────────────┤
-    │ webadd        │ Add open-directory media                           │
-    ├───────────────┼────────────────────────────────────────────────────┤
-    │ galleryadd    │ Add online gallery media (gallery-dl)              │
-    ├───────────────┼────────────────────────────────────────────────────┤
-    │ tabsadd       │ Create a tabs database; Add URLs                   │
-    ├───────────────┼────────────────────────────────────────────────────┤
-    │ links-add     │ Create a link-scraping database                    │
-    ├───────────────┼────────────────────────────────────────────────────┤
-    │ siteadd       │ Auto-scrape website data to SQLITE                 │
-    ├───────────────┼────────────────────────────────────────────────────┤
-    │ redditadd     │ Create a reddit database; Add subreddits           │
-    ├───────────────┼────────────────────────────────────────────────────┤
-    │ pushshift     │ Convert pushshift data to reddit.db format (stdin) │
-    ├───────────────┼────────────────────────────────────────────────────┤
-    │ hnadd         │ Create / Update a Hacker News database             │
-    ├───────────────┼────────────────────────────────────────────────────┤
-    │ substack      │ Backup substack articles                           │
-    ├───────────────┼────────────────────────────────────────────────────┤
-    │ tildes        │ Backup tildes comments and topics                  │
-    ├───────────────┼────────────────────────────────────────────────────┤
-    │ places-import │ Import places of interest (POIs)                   │
-    ├───────────────┼────────────────────────────────────────────────────┤
-    │ add-row       │ Add arbitrary data to SQLITE                       │
-    ╰───────────────┴────────────────────────────────────────────────────╯
+    ╭───────────────┬──────────────────────────────────────────╮
+    │ fs-add        │ Add local media                          │
+    ├───────────────┼──────────────────────────────────────────┤
+    │ tube-add      │ Add online video media (yt-dlp)          │
+    ├───────────────┼──────────────────────────────────────────┤
+    │ web-add       │ Add open-directory media                 │
+    ├───────────────┼──────────────────────────────────────────┤
+    │ gallery-add   │ Add online gallery media (gallery-dl)    │
+    ├───────────────┼──────────────────────────────────────────┤
+    │ tabs-add      │ Create a tabs database; Add URLs         │
+    ├───────────────┼──────────────────────────────────────────┤
+    │ links-add     │ Create a link-scraping database          │
+    ├───────────────┼──────────────────────────────────────────┤
+    │ site-add      │ Auto-scrape website data to SQLITE       │
+    ├───────────────┼──────────────────────────────────────────┤
+    │ reddit-add    │ Create a reddit database; Add subreddits │
+    ├───────────────┼──────────────────────────────────────────┤
+    │ hn-add        │ Create / Update a Hacker News database   │
+    ├───────────────┼──────────────────────────────────────────┤
+    │ substack      │ Backup substack articles                 │
+    ├───────────────┼──────────────────────────────────────────┤
+    │ tildes        │ Backup tildes comments and topics        │
+    ├───────────────┼──────────────────────────────────────────┤
+    │ places-import │ Import places of interest (POIs)         │
+    ├───────────────┼──────────────────────────────────────────┤
+    │ row-add       │ Add arbitrary data to SQLITE             │
+    ╰───────────────┴──────────────────────────────────────────╯
 
     Text subcommands:
     ╭────────────────┬─────────────────────────────────────────────╮
     │ cluster-sort   │ Sort text and images by similarity          │
     ├────────────────┼─────────────────────────────────────────────┤
     │ extract-links  │ Extract inner links from lists of web links │
     ├────────────────┼─────────────────────────────────────────────┤
     │ extract-text   │ Extract human text from lists of web links  │
     ├────────────────┼─────────────────────────────────────────────┤
     │ markdown-links │ Extract titles from lists of web links      │
+    ├────────────────┼─────────────────────────────────────────────┤
+    │ nouns          │ Unstructured text -> compound nouns (stdin) │
     ╰────────────────┴─────────────────────────────────────────────╯
 
     Folder subcommands:
     ╭───────────────┬──────────────────────────────────────────────────╮
     │ merge-folders │ Merge two or more file trees                     │
     ├───────────────┼──────────────────────────────────────────────────┤
     │ relmv         │ Move files preserving parent folder hierarchy    │
@@ -279,92 +279,92 @@
     │ disk-usage  │ Show disk usage                │
     ├─────────────┼────────────────────────────────┤
     │ mount-stats │ Show some relative mount stats │
     ├─────────────┼────────────────────────────────┤
     │ big-dirs    │ Show large folders             │
     ├─────────────┼────────────────────────────────┤
     │ search-db   │ Search a SQLITE database       │
-    ├─────────────┼────────────────────────────────┤
-    │ optimize    │ Re-optimize database           │
     ╰─────────────┴────────────────────────────────╯
 
     Media Database subcommands:
     ╭─────────────────┬────────────────────────────────╮
-    │ tabs            │ Open your tabs for the day     │
-    ├─────────────────┼────────────────────────────────┤
     │ block           │ Block a channel                │
     ├─────────────────┼────────────────────────────────┤
     │ playlists       │ List stored playlists          │
     ├─────────────────┼────────────────────────────────┤
     │ download        │ Download media                 │
     ├─────────────────┼────────────────────────────────┤
     │ download-status │ Show download status           │
     ├─────────────────┼────────────────────────────────┤
     │ redownload      │ Re-download deleted/lost media │
     ├─────────────────┼────────────────────────────────┤
     │ history         │ Show some playback statistics  │
     ├─────────────────┼────────────────────────────────┤
     │ search          │ Search captions / subtitles    │
+    ├─────────────────┼────────────────────────────────┤
+    │ optimize        │ Re-optimize database           │
     ╰─────────────────┴────────────────────────────────╯
 
     Playback subcommands:
     ╭────────────┬───────────────────────────────────────────────────╮
     │ watch      │ Watch / Listen                                    │
     ├────────────┼───────────────────────────────────────────────────┤
     │ now        │ Show what is currently playing                    │
     ├────────────┼───────────────────────────────────────────────────┤
     │ next       │ Play next file and optionally delete current file │
     ├────────────┼───────────────────────────────────────────────────┤
     │ stop       │ Stop all playback                                 │
     ├────────────┼───────────────────────────────────────────────────┤
     │ pause      │ Pause all playback                                │
     ├────────────┼───────────────────────────────────────────────────┤
-    │ open-links │ Open links from link dbs                          │
+    │ tabs-open  │ Open your tabs for the day                        │
+    ├────────────┼───────────────────────────────────────────────────┤
+    │ links-open │ Open links from link dbs                          │
     ├────────────┼───────────────────────────────────────────────────┤
     │ surf       │ Auto-load browser tabs in a streaming way (stdin) │
     ╰────────────┴───────────────────────────────────────────────────╯
 
     Database enrichment subcommands:
-    ╭────────────────────┬────────────────────────────────────────╮
-    │ dedupe-db          │ Dedupe SQLITE tables                   │
-    ├────────────────────┼────────────────────────────────────────┤
-    │ dedupe-media       │ Dedupe similar media                   │
-    ├────────────────────┼────────────────────────────────────────┤
-    │ merge-online-local │ Merge online and local data            │
-    ├────────────────────┼────────────────────────────────────────┤
-    │ mpv-watchlater     │ Import mpv watchlater files to history │
-    ├────────────────────┼────────────────────────────────────────┤
-    │ reddit-selftext    │ Copy selftext links to media table     │
-    ├────────────────────┼────────────────────────────────────────┤
-    │ tabs-shuffle       │ Randomize tabs.db a bit                │
-    ╰────────────────────┴────────────────────────────────────────╯
+    ╭────────────────────┬────────────────────────────────────────────────────╮
+    │ dedupe-db          │ Dedupe SQLITE tables                               │
+    ├────────────────────┼────────────────────────────────────────────────────┤
+    │ dedupe-media       │ Dedupe similar media                               │
+    ├────────────────────┼────────────────────────────────────────────────────┤
+    │ merge-online-local │ Merge online and local data                        │
+    ├────────────────────┼────────────────────────────────────────────────────┤
+    │ mpv-watchlater     │ Import mpv watchlater files to history             │
+    ├────────────────────┼────────────────────────────────────────────────────┤
+    │ reddit-selftext    │ Copy selftext links to media table                 │
+    ├────────────────────┼────────────────────────────────────────────────────┤
+    │ tabs-shuffle       │ Randomize tabs.db a bit                            │
+    ├────────────────────┼────────────────────────────────────────────────────┤
+    │ pushshift          │ Convert pushshift data to reddit.db format (stdin) │
+    ╰────────────────────┴────────────────────────────────────────────────────╯
 
     Update database subcommands:
-    ╭───────────────┬─────────────────────────────────╮
-    │ fsupdate      │ Update local media              │
-    ├───────────────┼─────────────────────────────────┤
-    │ tubeupdate    │ Update online video media       │
-    ├───────────────┼─────────────────────────────────┤
-    │ webupdate     │ Update open-directory media     │
-    ├───────────────┼─────────────────────────────────┤
-    │ galleryupdate │ Update online gallery media     │
-    ├───────────────┼─────────────────────────────────┤
-    │ links-update  │ Update a link-scraping database │
-    ├───────────────┼─────────────────────────────────┤
-    │ redditupdate  │ Update reddit media             │
-    ╰───────────────┴─────────────────────────────────╯
+    ╭────────────────┬─────────────────────────────────╮
+    │ fs-update      │ Update local media              │
+    ├────────────────┼─────────────────────────────────┤
+    │ tube-update    │ Update online video media       │
+    ├────────────────┼─────────────────────────────────┤
+    │ web-update     │ Update open-directory media     │
+    ├────────────────┼─────────────────────────────────┤
+    │ gallery-update │ Update online gallery media     │
+    ├────────────────┼─────────────────────────────────┤
+    │ links-update   │ Update a link-scraping database │
+    ├────────────────┼─────────────────────────────────┤
+    │ reddit-update  │ Update reddit media             │
+    ╰────────────────┴─────────────────────────────────╯
 
     Misc subcommands:
-    ╭────────────────┬─────────────────────────────────────────────╮
-    │ export-text    │ Export HTML files from SQLite databases     │
-    ├────────────────┼─────────────────────────────────────────────┤
-    │ dedupe-czkawka │ Process czkawka diff output                 │
-    ├────────────────┼─────────────────────────────────────────────┤
-    │ nouns          │ Unstructured text -> compound nouns (stdin) │
-    ╰────────────────┴─────────────────────────────────────────────╯
+    ╭────────────────┬─────────────────────────────────────────╮
+    │ export-text    │ Export HTML files from SQLite databases │
+    ├────────────────┼─────────────────────────────────────────┤
+    │ dedupe-czkawka │ Process czkawka diff output             │
+    ╰────────────────┴─────────────────────────────────────────╯
 
 
 </details>
 
 ## Examples
 
 ### Watch online media on your PC
@@ -599,20 +599,20 @@
 </details>
 
 ## Usage
 
 
 ### Create database subcommands
 
-###### fsadd
+###### fs-add
 
 <details><summary>Add local media</summary>
 
-    $ library fsadd -h
-    usage: library fsadd [(--video) | --audio | --image |  --text | --filesystem] DATABASE PATH ...
+    $ library fs-add -h
+    usage: library fs-add [(--video) | --audio | --image |  --text | --filesystem] DATABASE PATH ...
 
     The default database type is video:
         library fsadd tv.db ./tv/
         library fsadd --video tv.db ./tv/  # equivalent
 
     You can also create audio databases. Both audio and video use ffmpeg to read metadata:
         library fsadd --audio audio.db ./music/
@@ -655,20 +655,20 @@
 
         library fsadd audio.db --move ~/library/ ./added_folder/
         This will run destination paths through `library christen` and move files relative to the added folder root
 
 
 </details>
 
-###### tubeadd
+###### tube-add
 
 <details><summary>Add online video media (yt-dlp)</summary>
 
-    $ library tubeadd -h
-    usage: library tubeadd [--safe] [--extra] [--subs] [--auto-subs] DATABASE URLS ...
+    $ library tube-add -h
+    usage: library tube-add [--safe] [--extra] [--subs] [--auto-subs] DATABASE URLS ...
 
     Create a dl database / add links to an existing database
 
         library tubeadd dl.db https://www.youdl.com/c/BranchEducation/videos
 
     Add links from a line-delimited file
 
@@ -680,24 +680,24 @@
 
     Fetch extra metadata:
 
         By default tubeadd will quickly add media at the expense of less metadata.
         If you plan on using `library download` then it doesn't make sense to use `--extra`.
         Downloading will add the extra metadata automatically to the database.
         You can always fetch more metadata later via tubeupdate:
-        library tubeupdate tw.db --extra
+        library tube-update tw.db --extra
 
 
 </details>
 
-###### webadd
+###### web-add
 
 <details><summary>Add open-directory media</summary>
 
-    $ library webadd -h
+    $ library web-add -h
     usage: library web-add [(--filesystem) | --video | --audio | --image | --text] DATABASE URL ...
 
     Scan open directories
 
         library web-add open_dir.db --video http://1.1.1.1/
 
     Check download size of all videos matching some criteria
@@ -741,36 +741,36 @@
 
         library download --fs open_dir.db --prefix ~/d/dump/video/ -w 'id in (select media_id from history)'
 
 
 
 </details>
 
-###### galleryadd
+###### gallery-add
 
 <details><summary>Add online gallery media (gallery-dl)</summary>
 
-    $ library galleryadd -h
-    usage: library galleryadd DATABASE URLS
+    $ library gallery-add -h
+    usage: library gallery-add DATABASE URLS
 
     Add gallery_dl URLs to download later or periodically update
 
     If you have many URLs use stdin
 
         cat ./my-favorite-manhwa.txt | library galleryadd your.db --insert-only -
 
 
 </details>
 
-###### tabsadd
+###### tabs-add
 
 <details><summary>Create a tabs database; Add URLs</summary>
 
-    $ library tabsadd -h
-    usage: library tabsadd [--frequency daily weekly (monthly) quarterly yearly] [--no-sanitize] DATABASE URLS ...
+    $ library tabs-add -h
+    usage: library tabs-add [--frequency daily weekly (monthly) quarterly yearly] [--no-sanitize] DATABASE URLS ...
 
     Adding one URL:
 
         library tabsadd -f daily tabs.db https://wiby.me/surprise/
 
         Depending on your shell you may need to escape the URL (add quotes)
 
@@ -888,36 +888,36 @@
         library links-add --path-include viewtopic.php --cookies-from-browser firefox \
         --page-key start --page-start 0 --page-step 50 --fixed-pages 14 --stop-pages-no-match 1 \
         plab.db https://plab/forum/tracker.php?o=(string replace ' ' \n -- 1 4 7 10 15)&s=2&tm=-1&f=(string replace ' ' \n -- 1670 1768 60 1671 1644 1672 1111 508 555 1112 1718 1143 1717 1851 1713 1712 1775 1674 902 1675 36 1830 1803 1831 1741 1676 1677 1780 1110 1124 1784 1769 1793 1797 1804 1819 1825 1836 1842 1846 1857 1861 1867 1451 1788 1789 1792 1798 1805 1820 1826 1837 1843 1847 1856 1862 1868 284 1853 1823 1800 1801 1719 997 1818 1849 1711 1791 1762)
 
 
 </details>
 
-###### siteadd
+###### site-add
 
 <details><summary>Auto-scrape website data to SQLITE</summary>
 
-    $ library siteadd -h
+    $ library site-add -h
     usage: library site-add DATABASE PATH ... [--auto-pager] [--poke] [--local-html] [--file FILE]
 
     Extract data from website requests to a database
 
         library siteadd jobs.st.db --poke https://hk.jobsdb.com/hk/search-jobs/python/
 
     Run with `-vv` to see and interact with the browser
 
 
 </details>
 
-###### redditadd
+###### reddit-add
 
 <details><summary>Create a reddit database; Add subreddits</summary>
 
-    $ library redditadd -h
-    usage: library redditadd [--lookback N_DAYS] [--praw-site bot1] DATABASE URLS ...
+    $ library reddit-add -h
+    usage: library reddit-add [--lookback N_DAYS] [--praw-site bot1] DATABASE URLS ...
 
     Fetch data for redditors and reddits:
 
         library redditadd interesting.db https://old.reddit.com/r/coolgithubprojects/ https://old.reddit.com/user/Diastro
 
     If you have a file with a list of subreddits you can do this:
 
@@ -931,45 +931,20 @@
     Also, it may be the case that reddit's API (praw) will stop working in the near future. For both of these problems
     my suggestion is to use pushshift data.
     You can find more info here: https://github.com/chapmanjacobd/reddit_mining#how-was-this-made
 
 
 </details>
 
-###### pushshift
-
-<details><summary>Convert pushshift data to reddit.db format (stdin)</summary>
-
-    $ library pushshift -h
-    usage: library pushshift DATABASE < stdin
-
-    Download data (about 600GB jsonl.zst; 6TB uncompressed)
-
-        wget -e robots=off -r -k -A zst https://files.pushshift.io/reddit/submissions/
-
-    Load data from files via unzstd
-
-        unzstd --memory=2048MB --stdout RS_2005-07.zst | library pushshift pushshift.db
-
-    Or multiple (output is about 1.5TB SQLITE fts-searchable):
-
-        for f in psaw/files.pushshift.io/reddit/submissions/*.zst
-            echo "unzstd --memory=2048MB --stdout $f | library pushshift (basename $f).db"
-            library optimize (basename $f).db
-        end | parallel -j5
-
-
-</details>
-
-###### hnadd
+###### hn-add
 
 <details><summary>Create / Update a Hacker News database</summary>
 
-    $ library hnadd -h
-    usage: library hnadd [--oldest] DATABASE
+    $ library hn-add -h
+    usage: library hn-add [--oldest] DATABASE
 
     Fetch latest stories first:
 
         library hnadd hn.db -v
         Fetching 154873 items (33212696 to 33367569)
         Saving comment 33367568
         Saving comment 33367543
@@ -1021,24 +996,24 @@
     usage: library places-import DATABASE PATH ...
 
     Load POIs from Google Maps Google Takeout
 
 
 </details>
 
-###### add-row
+###### row-add
 
 <details><summary>Add arbitrary data to SQLITE</summary>
 
-    $ library add-row -h
-    usage: library add-row DATABASE [--table-name TABLE_NAME]
+    $ library row-add -h
+    usage: library row-add DATABASE [--table-name TABLE_NAME]
 
     Add a row to sqlite
 
-        library add-row t.db --test_b 1 --test-a 2
+        library row-add t.db --test_b 1 --test-a 2
 
         ### media (1 rows)
         |   test_b |   test_a |
         |----------|----------|
         |        1 |        2 |
 
 
@@ -1129,14 +1104,43 @@
     Sorting suggestions
 
         lb extract-text --skip-links --local-file (cb -t text/html | psub) | lb cs --groups | jq -r '.[] | .grouped_paths | "\n" + join("\n")'
 
 
 </details>
 
+###### markdown-links
+
+<details><summary>Extract titles from lists of web links</summary>
+
+    $ library markdown-links -h
+    usage: usage: library markdown-links URL ... [--cookies COOKIES] [--cookies-from-browser BROWSER[+KEYRING][:PROFILE][::CONTAINER]] [--firefox] [--chrome] [--allow-insecure] [--scroll] [--manual] [--auto-pager] [--poke] [--file FILE]
+
+    Convert URLs into Markdown links with page titles filled in
+
+        $ lb markdown-links https://www.youtube.com/watch?v=IgZDDW-NXDE
+        [Work For Peace](https://www.youtube.com/watch?v=IgZDDW-NXDE)
+
+
+</details>
+
+###### nouns
+
+<details><summary>Unstructured text -> compound nouns (stdin)</summary>
+
+    $ library nouns -h
+    usage: library nouns (stdin)
+
+    Extract compound nouns and phrases from unstructured mixed HTML plain text
+
+        xsv select text hn_comment_202210242109.csv | library nouns | sort | uniq -c | sort --numeric-sort
+
+
+</details>
+
 ### Folder subcommands
 
 ###### merge-folders
 
 <details><summary>Merge two or more file trees</summary>
 
     $ library merge-folders -h
@@ -1342,15 +1346,15 @@
 </details>
 
 ###### sample-compare
 
 <details><summary>Compare files using sample-hash and other shortcuts</summary>
 
     $ library sample-compare -h
-    usage: library sample-hash [--threads 10] [--chunk-size BYTES] [--gap BYTES OR 0.0-1.0*FILESIZE] PATH ...
+    usage: library sample-compare [--threads 10] [--chunk-size BYTES] [--gap BYTES OR 0.0-1.0*FILESIZE] PATH ...
 
     Convenience subcommand to compare multiple files using sample-hash
 
 
 </details>
 
 ### Tabular data subcommands
@@ -1700,14 +1704,26 @@
         | /home/xk/github/xk/lb/__pypackages__/3.11/lib/jedi/third_party/typeshed/third_party/2and3/requests/packages/urllib3/packages/ssl_match_hostname/__init__.pyi        | 88 Bytes |
         | /home/xk/github/xk/lb/__pypackages__/3.11/lib/jedi/third_party/typeshed/third_party/2and3/requests/packages/urllib3/packages/ssl_match_hostname/_implementation.pyi | 81 Bytes |
 
 
 
 </details>
 
+###### mount-stats
+
+<details><summary>Show some relative mount stats</summary>
+
+    $ library mount-stats -h
+    usage: library mount-stats MOUNTPOINT ...
+
+    Print relative use and free for multiple mount points
+
+
+</details>
+
 ###### big-dirs
 
 <details><summary>Show large folders</summary>
 
     $ library big-dirs -h
     usage: library big-dirs DATABASE [--limit (4000)] [--depth (0)] [--sort-groups-by deleted | played] [--size=+5MB]
 
@@ -1737,104 +1753,16 @@
     usage: library search-db DATABASE TABLE SEARCH ... [--delete-rows]
 
     Search all columns in a SQLITE table. If the table does not exist, uses the table which startswith (if only one match)
 
 
 </details>
 
-###### optimize
-
-<details><summary>Re-optimize database</summary>
-
-    $ library optimize -h
-    usage: library optimize DATABASE [--force]
-
-    Optimize library databases
-
-    The force flag is usually unnecessary and it can take much longer
-
-
-</details>
-
 ### Media Database subcommands
 
-###### tabs
-
-<details><summary>Open your tabs for the day</summary>
-
-    $ library tabs -h
-    usage: library tabs DATABASE
-
-    Tabs is meant to run **once per day**. Here is how you would configure it with `crontab`:
-
-        45 9 * * * DISPLAY=:0 library tabs /home/my/tabs.db
-
-    If things aren't working you can use `at` to simulate a similar environment as `cron`
-
-        echo 'fish -c "export DISPLAY=:0 && library tabs /full/path/to/tabs.db"' | at NOW
-
-    You can also invoke tabs manually:
-
-        library tabs -L 1  # open one tab
-
-    Print URLs
-
-        library tabs -w "frequency='yearly'" -p
-        ╒════════════════════════════════════════════════════════════════╤═════════════╤══════════════╕
-        │ path                                                           │ frequency   │ time_valid   │
-        ╞════════════════════════════════════════════════════════════════╪═════════════╪══════════════╡
-        │ https://old.reddit.com/r/Autonomia/top/?sort=top&t=year        │ yearly      │ Dec 31 1970  │
-        ├────────────────────────────────────────────────────────────────┼─────────────┼──────────────┤
-        │ https://old.reddit.com/r/Cyberpunk/top/?sort=top&t=year        │ yearly      │ Dec 31 1970  │
-        ├────────────────────────────────────────────────────────────────┼─────────────┼──────────────┤
-        │ https://old.reddit.com/r/ExperiencedDevs/top/?sort=top&t=year  │ yearly      │ Dec 31 1970  │
-
-        ...
-
-        ╘════════════════════════════════════════════════════════════════╧═════════════╧══════════════╛
-
-    View how many yearly tabs you have:
-
-        library tabs -w "frequency='yearly'" -p a
-        ╒═══════════╤═════════╕
-        │ path      │   count │
-        ╞═══════════╪═════════╡
-        │ Aggregate │     134 │
-        ╘═══════════╧═════════╛
-
-    Delete URLs
-
-        library tabs -p -s cyber
-        ╒═══════════════════════════════════════╤═════════════╤══════════════╕
-        │ path                                  │ frequency   │ time_valid   │
-        ╞═══════════════════════════════════════╪═════════════╪══════════════╡
-        │ https://old.reddit.com/r/cyberDeck/to │ yearly      │ Dec 31 1970  │
-        │ p/?sort=top&t=year                    │             │              │
-        ├───────────────────────────────────────┼─────────────┼──────────────┤
-        │ https://old.reddit.com/r/Cyberpunk/to │ yearly      │ Aug 29 2023  │
-        │ p/?sort=top&t=year                    │             │              │
-        ├───────────────────────────────────────┼─────────────┼──────────────┤
-        │ https://www.reddit.com/r/cyberDeck/   │ yearly      │ Sep 05 2023  │
-        ╘═══════════════════════════════════════╧═════════════╧══════════════╛
-        library tabs -p -w "path='https://www.reddit.com/r/cyberDeck/'" --delete-rows
-        Removed 1 metadata records
-        library tabs -p -s cyber
-        ╒═══════════════════════════════════════╤═════════════╤══════════════╕
-        │ path                                  │ frequency   │ time_valid   │
-        ╞═══════════════════════════════════════╪═════════════╪══════════════╡
-        │ https://old.reddit.com/r/cyberDeck/to │ yearly      │ Dec 31 1970  │
-        │ p/?sort=top&t=year                    │             │              │
-        ├───────────────────────────────────────┼─────────────┼──────────────┤
-        │ https://old.reddit.com/r/Cyberpunk/to │ yearly      │ Aug 29 2023  │
-        │ p/?sort=top&t=year                    │             │              │
-        ╘═══════════════════════════════════════╧═════════════╧══════════════╛
-
-
-</details>
-
 ###### block
 
 <details><summary>Block a channel</summary>
 
     $ library block -h
     usage: library block DATABASE URLS ...
 
@@ -2228,14 +2156,28 @@
     Search and open file
 
         library search fts.db 'two words' --open
 
 
 </details>
 
+###### optimize
+
+<details><summary>Re-optimize database</summary>
+
+    $ library optimize -h
+    usage: library optimize DATABASE [--force]
+
+    Optimize library databases
+
+    The force flag is usually unnecessary and it can take much longer
+
+
+</details>
+
 ### Playback subcommands
 
 ###### watch
 
 <details><summary>Watch / Listen</summary>
 
     $ library watch -h
@@ -2244,16 +2186,14 @@
     Control playback:
         To stop playback press Ctrl-C in either the terminal or mpv
 
         Create global shortcuts in your desktop environment by sending commands to mpv_socket:
         echo 'playlist-next force' | socat - /tmp/mpv_socket
 
     Override the default player (mpv):
-        library does a lot of things to try to automatically use your preferred media player
-        but if it doesn't guess right you can make it explicit:
         library watch --player "vlc --vlc-opts"
 
     Cast to chromecast groups:
         library watch --cast --cast-to "Office pair"
         library watch -ct "Office pair"  # equivalent
         If you don't know the exact name of your chromecast group run `catt scan`
 
@@ -2616,20 +2556,94 @@
                 qdbus-qt5 org.kde.KWin /KWin reconfigure
             end
 
 
 
 </details>
 
-###### open-links
+###### tabs-open
+
+<details><summary>Open your tabs for the day</summary>
+
+    $ library tabs-open -h
+    usage: library tabs-open DATABASE
+
+    Tabs is meant to run **once per day**. Here is how you would configure it with `crontab`:
+
+        45 9 * * * DISPLAY=:0 library tabs /home/my/tabs.db
+
+    If things aren't working you can use `at` to simulate a similar environment as `cron`
+
+        echo 'fish -c "export DISPLAY=:0 && library tabs /full/path/to/tabs.db"' | at NOW
+
+    You can also invoke tabs manually:
+
+        library tabs -L 1  # open one tab
+
+    Print URLs
+
+        library tabs -w "frequency='yearly'" -p
+        ╒════════════════════════════════════════════════════════════════╤═════════════╤══════════════╕
+        │ path                                                           │ frequency   │ time_valid   │
+        ╞════════════════════════════════════════════════════════════════╪═════════════╪══════════════╡
+        │ https://old.reddit.com/r/Autonomia/top/?sort=top&t=year        │ yearly      │ Dec 31 1970  │
+        ├────────────────────────────────────────────────────────────────┼─────────────┼──────────────┤
+        │ https://old.reddit.com/r/Cyberpunk/top/?sort=top&t=year        │ yearly      │ Dec 31 1970  │
+        ├────────────────────────────────────────────────────────────────┼─────────────┼──────────────┤
+        │ https://old.reddit.com/r/ExperiencedDevs/top/?sort=top&t=year  │ yearly      │ Dec 31 1970  │
+
+        ...
+
+        ╘════════════════════════════════════════════════════════════════╧═════════════╧══════════════╛
+
+    View how many yearly tabs you have:
+
+        library tabs -w "frequency='yearly'" -p a
+        ╒═══════════╤═════════╕
+        │ path      │   count │
+        ╞═══════════╪═════════╡
+        │ Aggregate │     134 │
+        ╘═══════════╧═════════╛
+
+    Delete URLs
+
+        library tabs -p -s cyber
+        ╒═══════════════════════════════════════╤═════════════╤══════════════╕
+        │ path                                  │ frequency   │ time_valid   │
+        ╞═══════════════════════════════════════╪═════════════╪══════════════╡
+        │ https://old.reddit.com/r/cyberDeck/to │ yearly      │ Dec 31 1970  │
+        │ p/?sort=top&t=year                    │             │              │
+        ├───────────────────────────────────────┼─────────────┼──────────────┤
+        │ https://old.reddit.com/r/Cyberpunk/to │ yearly      │ Aug 29 2023  │
+        │ p/?sort=top&t=year                    │             │              │
+        ├───────────────────────────────────────┼─────────────┼──────────────┤
+        │ https://www.reddit.com/r/cyberDeck/   │ yearly      │ Sep 05 2023  │
+        ╘═══════════════════════════════════════╧═════════════╧══════════════╛
+        library tabs -p -w "path='https://www.reddit.com/r/cyberDeck/'" --delete-rows
+        Removed 1 metadata records
+        library tabs -p -s cyber
+        ╒═══════════════════════════════════════╤═════════════╤══════════════╕
+        │ path                                  │ frequency   │ time_valid   │
+        ╞═══════════════════════════════════════╪═════════════╪══════════════╡
+        │ https://old.reddit.com/r/cyberDeck/to │ yearly      │ Dec 31 1970  │
+        │ p/?sort=top&t=year                    │             │              │
+        ├───────────────────────────────────────┼─────────────┼──────────────┤
+        │ https://old.reddit.com/r/Cyberpunk/to │ yearly      │ Aug 29 2023  │
+        │ p/?sort=top&t=year                    │             │              │
+        ╘═══════════════════════════════════════╧═════════════╧══════════════╛
+
+
+</details>
+
+###### links-open
 
 <details><summary>Open links from link dbs</summary>
 
-    $ library open-links -h
-    usage: library open-links DATABASE [search] [--title] [--title-prefix TITLE_PREFIX]
+    $ library links-open -h
+    usage: library links-open DATABASE [search] [--title] [--title-prefix TITLE_PREFIX]
 
     Open links from a links db
 
         wget https://github.com/chapmanjacobd/library/raw/main/example_dbs/music.korea.ln.db
         library open-links music.korea.ln.db
 
     Only open links once
@@ -2786,36 +2800,61 @@
         library tabs-shuffle tabs.db -d  31 -f monthly
         library tabs-shuffle tabs.db -d  90 -f quarterly
         library tabs-shuffle tabs.db -d 365 -f yearly
 
 
 </details>
 
+###### pushshift
+
+<details><summary>Convert pushshift data to reddit.db format (stdin)</summary>
+
+    $ library pushshift -h
+    usage: library pushshift DATABASE < stdin
+
+    Download data (about 600GB jsonl.zst; 6TB uncompressed)
+
+        wget -e robots=off -r -k -A zst https://files.pushshift.io/reddit/submissions/
+
+    Load data from files via unzstd
+
+        unzstd --memory=2048MB --stdout RS_2005-07.zst | library pushshift pushshift.db
+
+    Or multiple (output is about 1.5TB SQLITE fts-searchable):
+
+        for f in psaw/files.pushshift.io/reddit/submissions/*.zst
+            echo "unzstd --memory=2048MB --stdout $f | library pushshift (basename $f).db"
+            library optimize (basename $f).db
+        end | parallel -j5
+
+
+</details>
+
 ### Update database subcommands
 
-###### fsupdate
+###### fs-update
 
 <details><summary>Update local media</summary>
 
-    $ library fsupdate -h
-    usage: library fsupdate DATABASE
+    $ library fs-update -h
+    usage: library fs-update DATABASE
 
     Update each path previously saved:
 
         library fsupdate video.db
 
 
 </details>
 
-###### tubeupdate
+###### tube-update
 
 <details><summary>Update online video media</summary>
 
-    $ library tubeupdate -h
-    usage: library tubeupdate [--audio | --video] DATABASE
+    $ library tube-update -h
+    usage: library tube-update [--audio | --video] DATABASE
 
     Fetch the latest videos for every playlist saved in your database
 
         library tubeupdate educational.db
 
     Fetch extra metadata:
 
@@ -2827,33 +2866,33 @@
     Remove duplicate playlists:
 
         lb dedupe-db video.db playlists --bk extractor_playlist_id
 
 
 </details>
 
-###### webupdate
+###### web-update
 
 <details><summary>Update open-directory media</summary>
 
-    $ library webupdate -h
+    $ library web-update -h
     usage: library web-update DATABASE
 
     Update saved open directories
 
 
 
 </details>
 
-###### galleryupdate
+###### gallery-update
 
 <details><summary>Update online gallery media</summary>
 
-    $ library galleryupdate -h
-    usage: library galleryupdate DATABASE URLS
+    $ library gallery-update -h
+    usage: library gallery-update DATABASE URLS
 
     Check previously saved gallery_dl URLs for new content
 
 
 </details>
 
 ###### links-update
@@ -2866,20 +2905,20 @@
     Fetch new links from each path previously saved
 
         library links-update links.db
 
 
 </details>
 
-###### redditupdate
+###### reddit-update
 
 <details><summary>Update reddit media</summary>
 
-    $ library redditupdate -h
-    usage: library redditupdate [--audio | --video] [--lookback N_DAYS] [--praw-site bot1] DATABASE
+    $ library reddit-update -h
+    usage: library reddit-update [--audio | --video] [--lookback N_DAYS] [--praw-site bot1] DATABASE
 
     Fetch the latest posts for every subreddit/redditor saved in your database
 
         library redditupdate edu_subreddits.db
 
 
 </details>
@@ -2894,14 +2933,28 @@
     usage: library export-text DATABASE
 
     Generate HTML files from SQLite databases
 
 
 </details>
 
+###### dedupe-czkawka
+
+<details><summary>Process czkawka diff output</summary>
+
+    $ library dedupe-czkawka -h
+    usage: library dedupe-czkawka [--volume VOLUME] [--auto-seek] [--ignore-errors] [--folder] [--folder-glob [FOLDER_GLOB]] [--replace] [--no-replace] [--override-trash OVERRIDE_TRASH] [--delete-files] [--gui]
+               [--auto-select-min-ratio AUTO_SELECT_MIN_RATIO] [--all-keep] [--all-left] [--all-right] [--all-delete] [--verbose]
+               czkawka_dupes_output_path
+
+    Choose which duplicate to keep by opening both side-by-side in mpv
+
+
+</details>
+
 
 <details><summary>Chicken mode</summary>
 
 
            ////////////////////////
           ////////////////////////|
          //////////////////////// |
```

