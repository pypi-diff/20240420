# Comparing `tmp/ytpb-2024.4.12.tar.gz` & `tmp/ytpb-2024.4.20.tar.gz`

## Comparing `ytpb-2024.4.12.tar` & `ytpb-2024.4.20.tar`

### file list

```diff
@@ -1,141 +1,141 @@
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 ytpb-2024.4.12/.gitattributes
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 ytpb-2024.4.12/.pre-commit-config.yaml
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 ytpb-2024.4.12/.readthedocs.yaml
--rw-r--r--   0        0        0     2934 2020-02-02 00:00:00.000000 ytpb-2024.4.12/CHANGELOG.rst
--rw-r--r--   0        0        0     2300 2020-02-02 00:00:00.000000 ytpb-2024.4.12/CONTRIBUTING.rst
--rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 ytpb-2024.4.12/Makefile
--rw-r--r--   0        0        0     2569 2020-02-02 00:00:00.000000 ytpb-2024.4.12/config.toml.example
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 ytpb-2024.4.12/docs/changelog.rst
--rw-r--r--   0        0        0    19723 2020-02-02 00:00:00.000000 ytpb-2024.4.12/docs/cli.rst
--rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 ytpb-2024.4.12/docs/conf.py
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 ytpb-2024.4.12/docs/contributing.rst
--rw-r--r--   0        0        0     3755 2020-02-02 00:00:00.000000 ytpb-2024.4.12/docs/cookbook.rst
--rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 ytpb-2024.4.12/docs/index.rst
--rw-r--r--   0        0        0     3160 2020-02-02 00:00:00.000000 ytpb-2024.4.12/docs/quick.rst
--rw-r--r--   0        0        0     8474 2020-02-02 00:00:00.000000 ytpb-2024.4.12/docs/reference.rst
--rw-r--r--   0        0        0     1373 2020-02-02 00:00:00.000000 ytpb-2024.4.12/docs/why.rst
--rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 ytpb-2024.4.12/docs/package/index.rst
--rw-r--r--   0        0        0     6811 2020-02-02 00:00:00.000000 ytpb-2024.4.12/docs/package/usage.rst
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 ytpb-2024.4.12/docs/package/api/index.rst
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 ytpb-2024.4.12/docs/package/api/ytpb.actions.rst
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ytpb-2024.4.12/docs/package/api/ytpb.cache.rst
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 ytpb-2024.4.12/docs/package/api/ytpb.download.rst
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 ytpb-2024.4.12/docs/package/api/ytpb.errors.rst
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 ytpb-2024.4.12/docs/package/api/ytpb.fetchers.rst
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 ytpb-2024.4.12/docs/package/api/ytpb.info.rst
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 ytpb-2024.4.12/docs/package/api/ytpb.locate.rst
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ytpb-2024.4.12/docs/package/api/ytpb.merge.rst
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 ytpb-2024.4.12/docs/package/api/ytpb.playback.rst
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 ytpb-2024.4.12/docs/package/api/ytpb.representations.rst
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 ytpb-2024.4.12/docs/package/api/ytpb.rst
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 ytpb-2024.4.12/docs/package/api/ytpb.segment.rst
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 ytpb-2024.4.12/docs/package/api/ytpb.streams.rst
--rw-r--r--   0        0        0     1552 2020-02-02 00:00:00.000000 ytpb-2024.4.12/etc/Containerfile
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ytpb-2024.4.12/notebooks/shared/.gitkeep
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 ytpb-2024.4.12/src/ytpb/__init__.py
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 ytpb-2024.4.12/src/ytpb/__main__.py
--rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 ytpb-2024.4.12/src/ytpb/api.py
--rw-r--r--   0        0        0     2690 2020-02-02 00:00:00.000000 ytpb-2024.4.12/src/ytpb/cache.py
--rw-r--r--   0        0        0     2341 2020-02-02 00:00:00.000000 ytpb-2024.4.12/src/ytpb/conditional.py
--rw-r--r--   0        0        0     6069 2020-02-02 00:00:00.000000 ytpb-2024.4.12/src/ytpb/config.py
--rw-r--r--   0        0        0     4834 2020-02-02 00:00:00.000000 ytpb-2024.4.12/src/ytpb/download.py
--rw-r--r--   0        0        0     1501 2020-02-02 00:00:00.000000 ytpb-2024.4.12/src/ytpb/errors.py
--rw-r--r--   0        0        0     6221 2020-02-02 00:00:00.000000 ytpb-2024.4.12/src/ytpb/fetchers.py
--rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 ytpb-2024.4.12/src/ytpb/ffmpeg.py
--rw-r--r--   0        0        0     3204 2020-02-02 00:00:00.000000 ytpb-2024.4.12/src/ytpb/info.py
--rw-r--r--   0        0        0    10576 2020-02-02 00:00:00.000000 ytpb-2024.4.12/src/ytpb/locate.py
--rw-r--r--   0        0        0    11224 2020-02-02 00:00:00.000000 ytpb-2024.4.12/src/ytpb/merge.py
--rw-r--r--   0        0        0    23882 2020-02-02 00:00:00.000000 ytpb-2024.4.12/src/ytpb/playback.py
--rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 ytpb-2024.4.12/src/ytpb/representations.py
--rw-r--r--   0        0        0     5395 2020-02-02 00:00:00.000000 ytpb-2024.4.12/src/ytpb/segment.py
--rw-r--r--   0        0        0     4886 2020-02-02 00:00:00.000000 ytpb-2024.4.12/src/ytpb/streams.py
--rw-r--r--   0        0        0     2389 2020-02-02 00:00:00.000000 ytpb-2024.4.12/src/ytpb/types.py
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 ytpb-2024.4.12/src/ytpb/actions/__init__.py
--rw-r--r--   0        0        0     3566 2020-02-02 00:00:00.000000 ytpb-2024.4.12/src/ytpb/actions/capture.py
--rw-r--r--   0        0        0     7418 2020-02-02 00:00:00.000000 ytpb-2024.4.12/src/ytpb/actions/compose.py
--rw-r--r--   0        0        0     7744 2020-02-02 00:00:00.000000 ytpb-2024.4.12/src/ytpb/actions/download.py
--rw-r--r--   0        0        0     4376 2020-02-02 00:00:00.000000 ytpb-2024.4.12/src/ytpb/cli/__init__.py
--rw-r--r--   0        0        0     9255 2020-02-02 00:00:00.000000 ytpb-2024.4.12/src/ytpb/cli/common.py
--rw-r--r--   0        0        0     4105 2020-02-02 00:00:00.000000 ytpb-2024.4.12/src/ytpb/cli/options.py
--rw-r--r--   0        0        0     7874 2020-02-02 00:00:00.000000 ytpb-2024.4.12/src/ytpb/cli/parameters.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ytpb-2024.4.12/src/ytpb/cli/commands/__init__.py
--rw-r--r--   0        0        0    17029 2020-02-02 00:00:00.000000 ytpb-2024.4.12/src/ytpb/cli/commands/capture.py
--rw-r--r--   0        0        0    14438 2020-02-02 00:00:00.000000 ytpb-2024.4.12/src/ytpb/cli/commands/download.py
--rw-r--r--   0        0        0    10345 2020-02-02 00:00:00.000000 ytpb-2024.4.12/src/ytpb/cli/commands/mpd.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ytpb-2024.4.12/src/ytpb/utils/__init__.py
--rw-r--r--   0        0        0     7961 2020-02-02 00:00:00.000000 ytpb-2024.4.12/src/ytpb/utils/date.py
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 ytpb-2024.4.12/src/ytpb/utils/other.py
--rw-r--r--   0        0        0     8625 2020-02-02 00:00:00.000000 ytpb-2024.4.12/src/ytpb/utils/path.py
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 ytpb-2024.4.12/src/ytpb/utils/remote.py
--rw-r--r--   0        0        0     2216 2020-02-02 00:00:00.000000 ytpb-2024.4.12/src/ytpb/utils/url.py
--rw-r--r--   0        0        0     9192 2020-02-02 00:00:00.000000 ytpb-2024.4.12/tests/conftest.py
--rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 ytpb-2024.4.12/tests/helpers.py
--rw-r--r--   0        0        0     2110 2020-02-02 00:00:00.000000 ytpb-2024.4.12/tests/test_cache.py
--rw-r--r--   0        0        0     1492 2020-02-02 00:00:00.000000 ytpb-2024.4.12/tests/test_download.py
--rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 ytpb-2024.4.12/tests/test_fetchers.py
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 ytpb-2024.4.12/tests/test_info.py
--rw-r--r--   0        0        0     7973 2020-02-02 00:00:00.000000 ytpb-2024.4.12/tests/test_locate.py
--rw-r--r--   0        0        0     9981 2020-02-02 00:00:00.000000 ytpb-2024.4.12/tests/test_merge.py
--rw-r--r--   0        0        0    11455 2020-02-02 00:00:00.000000 ytpb-2024.4.12/tests/test_playback.py
--rw-r--r--   0        0        0     4644 2020-02-02 00:00:00.000000 ytpb-2024.4.12/tests/test_playback_session.py
--rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 ytpb-2024.4.12/tests/test_representations.py
--rw-r--r--   0        0        0     2022 2020-02-02 00:00:00.000000 ytpb-2024.4.12/tests/test_segment.py
--rw-r--r--   0        0        0     2364 2020-02-02 00:00:00.000000 ytpb-2024.4.12/tests/test_streams.py
--rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 ytpb-2024.4.12/tests/test_types.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ytpb-2024.4.12/tests/actions/__init__.py
--rw-r--r--   0        0        0     8653 2020-02-02 00:00:00.000000 ytpb-2024.4.12/tests/actions/test_compose.py
--rw-r--r--   0        0        0     4857 2020-02-02 00:00:00.000000 ytpb-2024.4.12/tests/actions/test_download.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ytpb-2024.4.12/tests/cli/__init__.py
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 ytpb-2024.4.12/tests/cli/conftest.py
--rw-r--r--   0        0        0    39866 2020-02-02 00:00:00.000000 ytpb-2024.4.12/tests/cli/test_download_command.py
--rw-r--r--   0        0        0     4609 2020-02-02 00:00:00.000000 ytpb-2024.4.12/tests/cli/test_parameters.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ytpb-2024.4.12/tests/cli/capture/__init__.py
--rw-r--r--   0        0        0     4971 2020-02-02 00:00:00.000000 ytpb-2024.4.12/tests/cli/capture/test_frame_command.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ytpb-2024.4.12/tests/cli/mpd/__init__.py
--rw-r--r--   0        0        0     6849 2020-02-02 00:00:00.000000 ytpb-2024.4.12/tests/cli/mpd/test_compose_command.py
--rw-r--r--   0        0        0     4105 2020-02-02 00:00:00.000000 ytpb-2024.4.12/tests/cli/mpd/test_refresh_command.py
--rw-r--r--   0        0        0    56372 2020-02-02 00:00:00.000000 ytpb-2024.4.12/tests/data/info-1695928670.json
--rw-r--r--   0        0        0  2978627 2020-02-02 00:00:00.000000 ytpb-2024.4.12/tests/data/manifest-1695928670.mpd
--rw-r--r--   0        0        0   701494 2020-02-02 00:00:00.000000 ytpb-2024.4.12/tests/data/webpage-1695928670.html
--rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 ytpb-2024.4.12/tests/data/expected/test_compose_mpd[itag%20eq%20140-itag%20eq%20243%20or%20itag%20eq%20244].out
--rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 ytpb-2024.4.12/tests/data/expected/test_compose_mpd[itag%20eq%20140-none].out
--rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 ytpb-2024.4.12/tests/data/expected/test_compose_mpd[none-itag%20eq%20243%20or%20itag%20eq%20244].out
--rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 ytpb-2024.4.12/tests/data/expected/test_compose_mpd_with_no_streams.out
--rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 ytpb-2024.4.12/tests/data/expected/test_download_audio_and_or_video[itag%20eq%20140-itag%20eq%20244].out
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 ytpb-2024.4.12/tests/data/expected/test_download_audio_and_or_video[itag%20eq%20140-none].out
--rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 ytpb-2024.4.12/tests/data/expected/test_download_audio_and_or_video[none-itag%20eq%20244].out
--rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 ytpb-2024.4.12/tests/data/expected/test_download_within_interval[2023-03-25T23%3A33%3A55%2B00%2F2023-03-25T23%3A33%3A57%2B00-233355%2B00.mp4].out
--rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 ytpb-2024.4.12/tests/data/expected/test_download_within_interval[2023-03-25T23%3A33%3A55%2B00%2F7959121-233355%2B00.mp4].out
--rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 ytpb-2024.4.12/tests/data/expected/test_download_within_interval[2023-03-25T23%3A33%3A55%2B00%2FPT3S-233355%2B00.mp4].out
--rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 ytpb-2024.4.12/tests/data/expected/test_download_within_interval[7959120%2F2023-03-25T23%3A33%3A57%2B00-233354%2B00.mp4].out
--rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 ytpb-2024.4.12/tests/data/expected/test_download_within_interval[7959120%2F7959121-233354%2B00.mp4].out
--rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 ytpb-2024.4.12/tests/data/expected/test_download_within_interval[7959120%2FPT3S-233354%2B00.mp4].out
--rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 ytpb-2024.4.12/tests/data/expected/test_download_within_interval[PT3S%2F2023-03-25T23%3A33%3A58%2B00-233355%2B00.mp4].out
--rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 ytpb-2024.4.12/tests/data/expected/test_download_within_interval[PT3S%2F7959121-233355%2B00.mp4].out
--rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 ytpb-2024.4.12/tests/data/expected/test_dry_run_option.out
--rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 ytpb-2024.4.12/tests/data/expected/test_no_cut_option.out
--rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 ytpb-2024.4.12/tests/data/expected/test_no_merge_option.out
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 ytpb-2024.4.12/tests/data/expected/test_refresh_mpd.out
--rw-r--r--   0        0        0     2969 2020-02-02 00:00:00.000000 ytpb-2024.4.12/tests/data/gap-cases/gap-case-1-fixture.csv
--rw-r--r--   0        0        0     1263 2020-02-02 00:00:00.000000 ytpb-2024.4.12/tests/data/gap-cases/gap-case-2-fixture.csv
--rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 ytpb-2024.4.12/tests/data/gap-cases/gap-case-3-fixture.csv
--rw-r--r--   0        0        0    42603 2020-02-02 00:00:00.000000 ytpb-2024.4.12/tests/data/segments/7959120.i140.mp4
--rw-r--r--   0        0        0   172355 2020-02-02 00:00:00.000000 ytpb-2024.4.12/tests/data/segments/7959120.i244.webm
--rw-r--r--   0        0        0    42603 2020-02-02 00:00:00.000000 ytpb-2024.4.12/tests/data/segments/7959121.i140.mp4
--rw-r--r--   0        0        0   171647 2020-02-02 00:00:00.000000 ytpb-2024.4.12/tests/data/segments/7959121.i244.webm
--rw-r--r--   0        0        0    42602 2020-02-02 00:00:00.000000 ytpb-2024.4.12/tests/data/segments/7959122.i140.mp4
--rw-r--r--   0        0        0   173730 2020-02-02 00:00:00.000000 ytpb-2024.4.12/tests/data/segments/7959122.i244.webm
--rw-r--r--   0        0        0    42603 2020-02-02 00:00:00.000000 ytpb-2024.4.12/tests/data/segments/7959123.i140.mp4
--rw-r--r--   0        0        0   172126 2020-02-02 00:00:00.000000 ytpb-2024.4.12/tests/data/segments/7959123.i244.webm
--rw-r--r--   0        0        0    42602 2020-02-02 00:00:00.000000 ytpb-2024.4.12/tests/data/segments/7959203.i140.mp4
--rw-r--r--   0        0        0   172036 2020-02-02 00:00:00.000000 ytpb-2024.4.12/tests/data/segments/7959203.i244.webm
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ytpb-2024.4.12/tests/utils/__init__.py
--rw-r--r--   0        0        0     8435 2020-02-02 00:00:00.000000 ytpb-2024.4.12/tests/utils/test_date.py
--rw-r--r--   0        0        0     9081 2020-02-02 00:00:00.000000 ytpb-2024.4.12/tests/utils/test_path.py
--rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 ytpb-2024.4.12/tests/utils/test_remote.py
--rw-r--r--   0        0        0     1269 2020-02-02 00:00:00.000000 ytpb-2024.4.12/tests/utils/test_url.py
--rw-r--r--   0        0        0     3163 2020-02-02 00:00:00.000000 ytpb-2024.4.12/.gitignore
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 ytpb-2024.4.12/LICENSE
--rw-r--r--   0        0        0     3433 2020-02-02 00:00:00.000000 ytpb-2024.4.12/README.rst
--rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 ytpb-2024.4.12/pyproject.toml
--rw-r--r--   0        0        0     6245 2020-02-02 00:00:00.000000 ytpb-2024.4.12/PKG-INFO
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 ytpb-2024.4.20/.gitattributes
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 ytpb-2024.4.20/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 ytpb-2024.4.20/.readthedocs.yaml
+-rw-r--r--   0        0        0     3427 2020-02-02 00:00:00.000000 ytpb-2024.4.20/CHANGELOG.rst
+-rw-r--r--   0        0        0     2300 2020-02-02 00:00:00.000000 ytpb-2024.4.20/CONTRIBUTING.rst
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 ytpb-2024.4.20/Makefile
+-rw-r--r--   0        0        0     2569 2020-02-02 00:00:00.000000 ytpb-2024.4.20/config.toml.example
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 ytpb-2024.4.20/docs/changelog.rst
+-rw-r--r--   0        0        0    22920 2020-02-02 00:00:00.000000 ytpb-2024.4.20/docs/cli.rst
+-rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 ytpb-2024.4.20/docs/conf.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 ytpb-2024.4.20/docs/contributing.rst
+-rw-r--r--   0        0        0     3755 2020-02-02 00:00:00.000000 ytpb-2024.4.20/docs/cookbook.rst
+-rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 ytpb-2024.4.20/docs/index.rst
+-rw-r--r--   0        0        0     3160 2020-02-02 00:00:00.000000 ytpb-2024.4.20/docs/quick.rst
+-rw-r--r--   0        0        0     8474 2020-02-02 00:00:00.000000 ytpb-2024.4.20/docs/reference.rst
+-rw-r--r--   0        0        0     1373 2020-02-02 00:00:00.000000 ytpb-2024.4.20/docs/why.rst
+-rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 ytpb-2024.4.20/docs/package/index.rst
+-rw-r--r--   0        0        0     6811 2020-02-02 00:00:00.000000 ytpb-2024.4.20/docs/package/usage.rst
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 ytpb-2024.4.20/docs/package/api/index.rst
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 ytpb-2024.4.20/docs/package/api/ytpb.actions.rst
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ytpb-2024.4.20/docs/package/api/ytpb.cache.rst
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 ytpb-2024.4.20/docs/package/api/ytpb.download.rst
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 ytpb-2024.4.20/docs/package/api/ytpb.errors.rst
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 ytpb-2024.4.20/docs/package/api/ytpb.fetchers.rst
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 ytpb-2024.4.20/docs/package/api/ytpb.info.rst
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 ytpb-2024.4.20/docs/package/api/ytpb.locate.rst
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ytpb-2024.4.20/docs/package/api/ytpb.merge.rst
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 ytpb-2024.4.20/docs/package/api/ytpb.playback.rst
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 ytpb-2024.4.20/docs/package/api/ytpb.representations.rst
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 ytpb-2024.4.20/docs/package/api/ytpb.rst
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 ytpb-2024.4.20/docs/package/api/ytpb.segment.rst
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 ytpb-2024.4.20/docs/package/api/ytpb.streams.rst
+-rw-r--r--   0        0        0     1552 2020-02-02 00:00:00.000000 ytpb-2024.4.20/etc/Containerfile
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ytpb-2024.4.20/notebooks/shared/.gitkeep
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 ytpb-2024.4.20/src/ytpb/__init__.py
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 ytpb-2024.4.20/src/ytpb/__main__.py
+-rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 ytpb-2024.4.20/src/ytpb/api.py
+-rw-r--r--   0        0        0     2690 2020-02-02 00:00:00.000000 ytpb-2024.4.20/src/ytpb/cache.py
+-rw-r--r--   0        0        0     2341 2020-02-02 00:00:00.000000 ytpb-2024.4.20/src/ytpb/conditional.py
+-rw-r--r--   0        0        0     6069 2020-02-02 00:00:00.000000 ytpb-2024.4.20/src/ytpb/config.py
+-rw-r--r--   0        0        0     4834 2020-02-02 00:00:00.000000 ytpb-2024.4.20/src/ytpb/download.py
+-rw-r--r--   0        0        0     1501 2020-02-02 00:00:00.000000 ytpb-2024.4.20/src/ytpb/errors.py
+-rw-r--r--   0        0        0     6221 2020-02-02 00:00:00.000000 ytpb-2024.4.20/src/ytpb/fetchers.py
+-rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 ytpb-2024.4.20/src/ytpb/ffmpeg.py
+-rw-r--r--   0        0        0     3204 2020-02-02 00:00:00.000000 ytpb-2024.4.20/src/ytpb/info.py
+-rw-r--r--   0        0        0    10576 2020-02-02 00:00:00.000000 ytpb-2024.4.20/src/ytpb/locate.py
+-rw-r--r--   0        0        0    13146 2020-02-02 00:00:00.000000 ytpb-2024.4.20/src/ytpb/merge.py
+-rw-r--r--   0        0        0    23882 2020-02-02 00:00:00.000000 ytpb-2024.4.20/src/ytpb/playback.py
+-rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 ytpb-2024.4.20/src/ytpb/representations.py
+-rw-r--r--   0        0        0     5395 2020-02-02 00:00:00.000000 ytpb-2024.4.20/src/ytpb/segment.py
+-rw-r--r--   0        0        0     4886 2020-02-02 00:00:00.000000 ytpb-2024.4.20/src/ytpb/streams.py
+-rw-r--r--   0        0        0     2389 2020-02-02 00:00:00.000000 ytpb-2024.4.20/src/ytpb/types.py
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 ytpb-2024.4.20/src/ytpb/actions/__init__.py
+-rw-r--r--   0        0        0     3566 2020-02-02 00:00:00.000000 ytpb-2024.4.20/src/ytpb/actions/capture.py
+-rw-r--r--   0        0        0     7418 2020-02-02 00:00:00.000000 ytpb-2024.4.20/src/ytpb/actions/compose.py
+-rw-r--r--   0        0        0     7744 2020-02-02 00:00:00.000000 ytpb-2024.4.20/src/ytpb/actions/download.py
+-rw-r--r--   0        0        0     4376 2020-02-02 00:00:00.000000 ytpb-2024.4.20/src/ytpb/cli/__init__.py
+-rw-r--r--   0        0        0     9255 2020-02-02 00:00:00.000000 ytpb-2024.4.20/src/ytpb/cli/common.py
+-rw-r--r--   0        0        0     4105 2020-02-02 00:00:00.000000 ytpb-2024.4.20/src/ytpb/cli/options.py
+-rw-r--r--   0        0        0     7874 2020-02-02 00:00:00.000000 ytpb-2024.4.20/src/ytpb/cli/parameters.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ytpb-2024.4.20/src/ytpb/cli/commands/__init__.py
+-rw-r--r--   0        0        0    17029 2020-02-02 00:00:00.000000 ytpb-2024.4.20/src/ytpb/cli/commands/capture.py
+-rw-r--r--   0        0        0    15726 2020-02-02 00:00:00.000000 ytpb-2024.4.20/src/ytpb/cli/commands/download.py
+-rw-r--r--   0        0        0    10345 2020-02-02 00:00:00.000000 ytpb-2024.4.20/src/ytpb/cli/commands/mpd.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ytpb-2024.4.20/src/ytpb/utils/__init__.py
+-rw-r--r--   0        0        0     7961 2020-02-02 00:00:00.000000 ytpb-2024.4.20/src/ytpb/utils/date.py
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 ytpb-2024.4.20/src/ytpb/utils/other.py
+-rw-r--r--   0        0        0     8625 2020-02-02 00:00:00.000000 ytpb-2024.4.20/src/ytpb/utils/path.py
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 ytpb-2024.4.20/src/ytpb/utils/remote.py
+-rw-r--r--   0        0        0     2216 2020-02-02 00:00:00.000000 ytpb-2024.4.20/src/ytpb/utils/url.py
+-rw-r--r--   0        0        0     9192 2020-02-02 00:00:00.000000 ytpb-2024.4.20/tests/conftest.py
+-rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 ytpb-2024.4.20/tests/helpers.py
+-rw-r--r--   0        0        0     2110 2020-02-02 00:00:00.000000 ytpb-2024.4.20/tests/test_cache.py
+-rw-r--r--   0        0        0     1492 2020-02-02 00:00:00.000000 ytpb-2024.4.20/tests/test_download.py
+-rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 ytpb-2024.4.20/tests/test_fetchers.py
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 ytpb-2024.4.20/tests/test_info.py
+-rw-r--r--   0        0        0     7973 2020-02-02 00:00:00.000000 ytpb-2024.4.20/tests/test_locate.py
+-rw-r--r--   0        0        0     9981 2020-02-02 00:00:00.000000 ytpb-2024.4.20/tests/test_merge.py
+-rw-r--r--   0        0        0    11455 2020-02-02 00:00:00.000000 ytpb-2024.4.20/tests/test_playback.py
+-rw-r--r--   0        0        0     4644 2020-02-02 00:00:00.000000 ytpb-2024.4.20/tests/test_playback_session.py
+-rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 ytpb-2024.4.20/tests/test_representations.py
+-rw-r--r--   0        0        0     2022 2020-02-02 00:00:00.000000 ytpb-2024.4.20/tests/test_segment.py
+-rw-r--r--   0        0        0     2364 2020-02-02 00:00:00.000000 ytpb-2024.4.20/tests/test_streams.py
+-rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 ytpb-2024.4.20/tests/test_types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ytpb-2024.4.20/tests/actions/__init__.py
+-rw-r--r--   0        0        0     8653 2020-02-02 00:00:00.000000 ytpb-2024.4.20/tests/actions/test_compose.py
+-rw-r--r--   0        0        0     4857 2020-02-02 00:00:00.000000 ytpb-2024.4.20/tests/actions/test_download.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ytpb-2024.4.20/tests/cli/__init__.py
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 ytpb-2024.4.20/tests/cli/conftest.py
+-rw-r--r--   0        0        0    43550 2020-02-02 00:00:00.000000 ytpb-2024.4.20/tests/cli/test_download_command.py
+-rw-r--r--   0        0        0     4609 2020-02-02 00:00:00.000000 ytpb-2024.4.20/tests/cli/test_parameters.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ytpb-2024.4.20/tests/cli/capture/__init__.py
+-rw-r--r--   0        0        0     4971 2020-02-02 00:00:00.000000 ytpb-2024.4.20/tests/cli/capture/test_frame_command.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ytpb-2024.4.20/tests/cli/mpd/__init__.py
+-rw-r--r--   0        0        0     6849 2020-02-02 00:00:00.000000 ytpb-2024.4.20/tests/cli/mpd/test_compose_command.py
+-rw-r--r--   0        0        0     4105 2020-02-02 00:00:00.000000 ytpb-2024.4.20/tests/cli/mpd/test_refresh_command.py
+-rw-r--r--   0        0        0    56372 2020-02-02 00:00:00.000000 ytpb-2024.4.20/tests/data/info-1695928670.json
+-rw-r--r--   0        0        0  2978627 2020-02-02 00:00:00.000000 ytpb-2024.4.20/tests/data/manifest-1695928670.mpd
+-rw-r--r--   0        0        0   701494 2020-02-02 00:00:00.000000 ytpb-2024.4.20/tests/data/webpage-1695928670.html
+-rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 ytpb-2024.4.20/tests/data/expected/test_compose_mpd[itag%20eq%20140-itag%20eq%20243%20or%20itag%20eq%20244].out
+-rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 ytpb-2024.4.20/tests/data/expected/test_compose_mpd[itag%20eq%20140-none].out
+-rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 ytpb-2024.4.20/tests/data/expected/test_compose_mpd[none-itag%20eq%20243%20or%20itag%20eq%20244].out
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 ytpb-2024.4.20/tests/data/expected/test_compose_mpd_with_no_streams.out
+-rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 ytpb-2024.4.20/tests/data/expected/test_download_audio_and_or_video[itag%20eq%20140-itag%20eq%20244].out
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 ytpb-2024.4.20/tests/data/expected/test_download_audio_and_or_video[itag%20eq%20140-none].out
+-rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 ytpb-2024.4.20/tests/data/expected/test_download_audio_and_or_video[none-itag%20eq%20244].out
+-rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 ytpb-2024.4.20/tests/data/expected/test_download_within_interval[2023-03-25T23%3A33%3A55%2B00%2F2023-03-25T23%3A33%3A57%2B00-233355%2B00.mp4].out
+-rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 ytpb-2024.4.20/tests/data/expected/test_download_within_interval[2023-03-25T23%3A33%3A55%2B00%2F7959121-233355%2B00.mp4].out
+-rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 ytpb-2024.4.20/tests/data/expected/test_download_within_interval[2023-03-25T23%3A33%3A55%2B00%2FPT3S-233355%2B00.mp4].out
+-rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 ytpb-2024.4.20/tests/data/expected/test_download_within_interval[7959120%2F2023-03-25T23%3A33%3A57%2B00-233354%2B00.mp4].out
+-rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 ytpb-2024.4.20/tests/data/expected/test_download_within_interval[7959120%2F7959121-233354%2B00.mp4].out
+-rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 ytpb-2024.4.20/tests/data/expected/test_download_within_interval[7959120%2FPT3S-233354%2B00.mp4].out
+-rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 ytpb-2024.4.20/tests/data/expected/test_download_within_interval[PT3S%2F2023-03-25T23%3A33%3A58%2B00-233355%2B00.mp4].out
+-rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 ytpb-2024.4.20/tests/data/expected/test_download_within_interval[PT3S%2F7959121-233355%2B00.mp4].out
+-rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 ytpb-2024.4.20/tests/data/expected/test_dry_run_option.out
+-rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 ytpb-2024.4.20/tests/data/expected/test_no_cut_option.out
+-rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 ytpb-2024.4.20/tests/data/expected/test_no_merge_option.out
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 ytpb-2024.4.20/tests/data/expected/test_refresh_mpd.out
+-rw-r--r--   0        0        0     2969 2020-02-02 00:00:00.000000 ytpb-2024.4.20/tests/data/gap-cases/gap-case-1-fixture.csv
+-rw-r--r--   0        0        0     1263 2020-02-02 00:00:00.000000 ytpb-2024.4.20/tests/data/gap-cases/gap-case-2-fixture.csv
+-rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 ytpb-2024.4.20/tests/data/gap-cases/gap-case-3-fixture.csv
+-rw-r--r--   0        0        0    42603 2020-02-02 00:00:00.000000 ytpb-2024.4.20/tests/data/segments/7959120.i140.mp4
+-rw-r--r--   0        0        0   172355 2020-02-02 00:00:00.000000 ytpb-2024.4.20/tests/data/segments/7959120.i244.webm
+-rw-r--r--   0        0        0    42603 2020-02-02 00:00:00.000000 ytpb-2024.4.20/tests/data/segments/7959121.i140.mp4
+-rw-r--r--   0        0        0   171647 2020-02-02 00:00:00.000000 ytpb-2024.4.20/tests/data/segments/7959121.i244.webm
+-rw-r--r--   0        0        0    42602 2020-02-02 00:00:00.000000 ytpb-2024.4.20/tests/data/segments/7959122.i140.mp4
+-rw-r--r--   0        0        0   173730 2020-02-02 00:00:00.000000 ytpb-2024.4.20/tests/data/segments/7959122.i244.webm
+-rw-r--r--   0        0        0    42603 2020-02-02 00:00:00.000000 ytpb-2024.4.20/tests/data/segments/7959123.i140.mp4
+-rw-r--r--   0        0        0   172126 2020-02-02 00:00:00.000000 ytpb-2024.4.20/tests/data/segments/7959123.i244.webm
+-rw-r--r--   0        0        0    42602 2020-02-02 00:00:00.000000 ytpb-2024.4.20/tests/data/segments/7959203.i140.mp4
+-rw-r--r--   0        0        0   172036 2020-02-02 00:00:00.000000 ytpb-2024.4.20/tests/data/segments/7959203.i244.webm
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ytpb-2024.4.20/tests/utils/__init__.py
+-rw-r--r--   0        0        0     8435 2020-02-02 00:00:00.000000 ytpb-2024.4.20/tests/utils/test_date.py
+-rw-r--r--   0        0        0     9081 2020-02-02 00:00:00.000000 ytpb-2024.4.20/tests/utils/test_path.py
+-rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 ytpb-2024.4.20/tests/utils/test_remote.py
+-rw-r--r--   0        0        0     1269 2020-02-02 00:00:00.000000 ytpb-2024.4.20/tests/utils/test_url.py
+-rw-r--r--   0        0        0     3163 2020-02-02 00:00:00.000000 ytpb-2024.4.20/.gitignore
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 ytpb-2024.4.20/LICENSE
+-rw-r--r--   0        0        0     3535 2020-02-02 00:00:00.000000 ytpb-2024.4.20/README.rst
+-rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 ytpb-2024.4.20/pyproject.toml
+-rw-r--r--   0        0        0     6347 2020-02-02 00:00:00.000000 ytpb-2024.4.20/PKG-INFO
```

### Comparing `ytpb-2024.4.12/CHANGELOG.rst` & `ytpb-2024.4.20/CHANGELOG.rst`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,23 @@
 Changelog
 #########
 
 Versions follow `Calendar Versioning`_ with the ``YYYY.M.D`` scheme.
 
 .. _Calendar Versioning: https://calver.org
 
+`2024.4.20`_
+************
+
+- Fix wrong frame rate values of the video-only merged files when boundary
+  segments are cut and encoded with H.264 (`e1120bf
+  <https://github.com/xymaxim/ytpb/commit/e1120bf4514333ff3ac5d4eac862ccb6a9d5f606>`__)
+- Add metadata tags with basic and rewind information to merged files (`aa7adf1
+  <https://github.com/xymaxim/ytpb/commit/aa7adf1580e5a83c9abaa76f2836b9a0570cc4ba>`__)
+  
 `2024.4.12`_
 ************
 
 - Add the `Python package
   <https://ytpb.readthedocs.io/en/latest/package/index.html>`__ page with the
   basic usage and API reference
 - Add the ``--version`` CLI option to show version number
@@ -68,12 +77,13 @@
 `2024.3.9`_
 ***********
 
 - Add the CHANGELOG file and documentation page
 - Change the first segment locating step: don't limit it to two jumps (`#8
   <https://github.com/xymaxim/ytpb/pull/8>`__)
 
+.. _2024.4.20: https://github.com/xymaxim/ytpb/compare/v2024.4.12..v2024.4.20  
 .. _2024.4.12: https://github.com/xymaxim/ytpb/compare/v2024.3.27..v2024.4.12
 .. _2024.3.27: https://github.com/xymaxim/ytpb/compare/v2024.3.16..v2024.3.27
 .. _2024.3.16: https://github.com/xymaxim/ytpb/compare/v2024.3.13..v2024.3.16
 .. _2024.3.13: https://github.com/xymaxim/ytpb/compare/v2024.3.9..v2024.3.13
 .. _2024.3.9: https://github.com/xymaxim/ytpb/compare/v2024.3.7..v2024.3.9
```

### Comparing `ytpb-2024.4.12/CONTRIBUTING.rst` & `ytpb-2024.4.20/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `ytpb-2024.4.12/config.toml.example` & `ytpb-2024.4.20/config.toml.example`

 * *Files identical despite different names*

### Comparing `ytpb-2024.4.12/docs/cli.rst` & `ytpb-2024.4.20/docs/cli.rst`

 * *Files 8% similar despite different names*

```diff
@@ -11,67 +11,75 @@
 
 Overview
 ********
 
 Synopsis
 ========
 
+The general synopsis of ``ytpb`` commands is as follows::
+
+  ytpb [GLOBAL_OPTIONS] COMMAND [SUBCOMMAND] [OPTIONS] [ARGS]...
+
 Commands
 --------
 
 .. code:: man
 
-  Usage: ytpb [OPTIONS] COMMAND [ARGS]...
+   Usage: ytpb [OPTIONS] COMMAND [ARGS]...
 
-  Global options:
-    --no-config    Do not load any configuration files.
-    --config PATH  Specifies a path to a configuration file.
-    --debug        Enable verbose output for debugging.
-
-  Other options:
-    --help         Show this message and exit.
-
-  Top-level commands:
-    download  Download excerpts.
-    capture   Capture a single or many frames.
-    mpd       Compose MPEG-DASH manifests.
+   A playback for YouTube live streams
+
+   Global options:
+     --no-config    Do not load any configuration files.
+     --config PATH  Specifies a path to a configuration file.
+     --report       Dump all output to a file. It implies --debug.
+     --debug        Enable verbose output for debugging.
+     -q, --quiet    Supress all normal output.
+
+   Other options:
+     -V, --version  Show the version and exit.
+     --help         Show this message and exit.
+
+   Top-level commands:
+     download  Download excerpts.
+     capture   Capture a single or many frames.
+     mpd       Compose MPEG-DASH manifests.
 
 Subcommands
 -----------
 
 *capture*
 ^^^^^^^^^
 
 .. code:: man
 
-  Usage: ytpb capture [OPTIONS] COMMAND [ARGS]...
+   Usage: ytpb capture [OPTIONS] COMMAND [ARGS]...
 
-    Capture a single or many frames.
+     Capture a single or many frames.
 
-  Options:
-    --help  Show this message and exit.
+   Options:
+     --help  Show this message and exit.
 
-  Commands:
-    frame      Capture a single frame.
-    timelapse  Capture time-lapse frames.
+   Commands:
+     frame      Capture a single frame.
+     timelapse  Capture time-lapse frames.
 
 *mpd*
 ^^^^^
 
 .. code:: man
 
-  Usage: ytpb mpd [OPTIONS] COMMAND [ARGS]...
-
-  Options:
-    --help  Show this message and exit.
+   Usage: ytpb mpd [OPTIONS] COMMAND [ARGS]...
 
-  Commands:
-    compose  Compose an MPEG-DASH manifest.
-    refresh  Refresh a composed MPEG-DASH manifest.
+   Options:
+     --help  Show this message and exit.
 
+   Commands:
+     compose  Compose an MPEG-DASH manifest.
+     refresh  Refresh a composed MPEG-DASH manifest.
 
 Getting help
 ============
 
 To show a list of available options, type ``--help`` after commands or
 subcommands: ::
 
@@ -498,14 +506,49 @@
 	  # 20240102T102000+00
 	  styles = "basic,complete,hh"
 
 	  # 20240102T1020Z
           # 20240102T1220+02
 	  styles = "basic,reduced,z"
 
+Writing metadata tags
+=====================
+
+By default, metadata tags will be added to the output file by the ``ytpb
+download`` command.  Use the ``--no-metadata`` option to disable it.
+
+.. table:: Metadata tags overview
+
+   +---------------------------+-------------------------------+---------------------------------------------+
+   | Tag                       | Description                   |                   Example                   |
+   +===========================+===============================+=============================================+
+   | ``title``                 | Video's title                 | Stream Title                                |
+   +---------------------------+-------------------------------+---------------------------------------------+
+   | ``author``                | Video's channel name          | Author or Channel Name                      |
+   +---------------------------+-------------------------------+---------------------------------------------+
+   | ``comment``               | YouTube video URL             | https://www.youtube.com/watch?v=abcdefgh123 |
+   +---------------------------+-------------------------------+---------------------------------------------+
+   | ``input_start_time``      | Input start time              | 1700000000.000000                           |
+   +---------------------------+-------------------------------+---------------------------------------------+
+   | ``input_end_time``        | Input end time                | 1700000030.000000                           |
+   +---------------------------+-------------------------------+---------------------------------------------+
+   | ``actual_start_time``     | Actual start time             | 1700000000.000000                           |
+   +---------------------------+-------------------------------+---------------------------------------------+
+   | ``actual_start_time``     | Actual end time               | 1700000030.000000                           |
+   +---------------------------+-------------------------------+---------------------------------------------+
+   | ``start_sequence_number`` | Start segment sequence number | 0                                           |
+   +---------------------------+-------------------------------+---------------------------------------------+
+   | ``end_sequence_number``   | End segment sequence number   | 1001                                        |
+   +---------------------------+-------------------------------+---------------------------------------------+
+
+The input and actual time values (represented as seconds since the epoch) are
+expected to be different in only two cases: if the boundary (start and end)
+points fall in gaps or the ``--no-cut`` option is requested. In the opposite
+cases, after accurate cut, they're supposed to be identical.
+
 Configuring
 ***********
 
 The configuration provides the way to set up default values of the command
 options and change other settings via configuration files. It's optional, and
 the default, built-in settings are used.
```

### Comparing `ytpb-2024.4.12/docs/conf.py` & `ytpb-2024.4.20/docs/conf.py`

 * *Files identical despite different names*

### Comparing `ytpb-2024.4.12/docs/cookbook.rst` & `ytpb-2024.4.20/docs/cookbook.rst`

 * *Files identical despite different names*

### Comparing `ytpb-2024.4.12/docs/quick.rst` & `ytpb-2024.4.20/docs/quick.rst`

 * *Files identical despite different names*

### Comparing `ytpb-2024.4.12/docs/reference.rst` & `ytpb-2024.4.20/docs/reference.rst`

 * *Files identical despite different names*

### Comparing `ytpb-2024.4.12/docs/why.rst` & `ytpb-2024.4.20/docs/why.rst`

 * *Files identical despite different names*

### Comparing `ytpb-2024.4.12/docs/package/index.rst` & `ytpb-2024.4.20/docs/package/index.rst`

 * *Files identical despite different names*

### Comparing `ytpb-2024.4.12/docs/package/usage.rst` & `ytpb-2024.4.20/docs/package/usage.rst`

 * *Files identical despite different names*

### Comparing `ytpb-2024.4.12/etc/Containerfile` & `ytpb-2024.4.20/etc/Containerfile`

 * *Files identical despite different names*

### Comparing `ytpb-2024.4.12/src/ytpb/api.py` & `ytpb-2024.4.20/src/ytpb/api.py`

 * *Files identical despite different names*

### Comparing `ytpb-2024.4.12/src/ytpb/cache.py` & `ytpb-2024.4.20/src/ytpb/cache.py`

 * *Files identical despite different names*

### Comparing `ytpb-2024.4.12/src/ytpb/conditional.py` & `ytpb-2024.4.20/src/ytpb/conditional.py`

 * *Files identical despite different names*

### Comparing `ytpb-2024.4.12/src/ytpb/config.py` & `ytpb-2024.4.20/src/ytpb/config.py`

 * *Files identical despite different names*

### Comparing `ytpb-2024.4.12/src/ytpb/download.py` & `ytpb-2024.4.20/src/ytpb/download.py`

 * *Files identical despite different names*

### Comparing `ytpb-2024.4.12/src/ytpb/errors.py` & `ytpb-2024.4.20/src/ytpb/errors.py`

 * *Files identical despite different names*

### Comparing `ytpb-2024.4.12/src/ytpb/fetchers.py` & `ytpb-2024.4.20/src/ytpb/fetchers.py`

 * *Files identical despite different names*

### Comparing `ytpb-2024.4.12/src/ytpb/ffmpeg.py` & `ytpb-2024.4.20/src/ytpb/ffmpeg.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,25 +7,24 @@
 
 from ytpb.errors import FFmpegRunError
 
 logger = structlog.get_logger(__name__)
 
 
 def run_ffmpeg(
-    args: str | list[str], **subprocess_kwargs: Any
+    args: str | list[str | Path], **subprocess_kwargs: Any
 ) -> subprocess.CompletedProcess:
     command = ["ffmpeg", "-v", "error", "-hide_banner", "-y"]
-
     if isinstance(args, str):
         command.extend(shlex.split(args))
     else:
         command.extend(args)
 
+    logger.debug(" ".join([str(x) for x in command]))
     cp = subprocess.run(command, **subprocess_kwargs)
-
     try:
         cp.check_returncode()
     except subprocess.CalledProcessError as e:
         logger.error("There was a problem running FFmpeg command.")
         raise FFmpegRunError from e
 
     return cp
@@ -42,16 +41,18 @@
         command.extend(args)
     command.append(input_path)
 
     cp = subprocess.run(command, **subprocess_kwargs)
     return cp
 
 
-def ffprobe_show_entries(input_path: Path, entries_to_show: str) -> str:
-    command_args = f"-show_entries {entries_to_show} -of default=nw=1:nk=1"
+def ffprobe_show_entries(
+    input_path: Path, entries_to_show: str, of: str = "default=nw=1:nk=1"
+) -> str:
+    command_args = f"-show_entries {entries_to_show} -of {of}"
     cp = run_ffprobe(input_path, command_args, capture_output=True, check=True)
     output = cp.stdout.decode().rstrip("\n")
     return output
 
 
 def ffmpeg_stream_copy(input_path: Path, output_path: Path):
     subprocess_kwargs = {"capture_output": True, "check": True}
```

### Comparing `ytpb-2024.4.12/src/ytpb/info.py` & `ytpb-2024.4.20/src/ytpb/info.py`

 * *Files identical despite different names*

### Comparing `ytpb-2024.4.12/src/ytpb/locate.py` & `ytpb-2024.4.20/src/ytpb/locate.py`

 * *Files identical despite different names*

### Comparing `ytpb-2024.4.12/src/ytpb/merge.py` & `ytpb-2024.4.20/src/ytpb/merge.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Merge and cut media segments.
 
 Note:
     The current implementation of segment merging is not optimal in terms of
-    disk space, as it requires triple the amount of the total size of
-    segments. Should be changed to use different techniques, without the need
-    for intermediate files.
+    disk space, as it requires triple the amount of the total size of segments
+    if cutting is requested (by default). Should be changed to use different
+    techniques, without the need for intermediate files.
 """
 
 import functools
 import os
 import shlex
 from pathlib import Path
 from typing import Any
@@ -28,87 +28,104 @@
 def get_nth_or_none(iterable, n: int) -> Any | None:
     if not iterable:
         return None
     return iterable[n]
 
 
 def mux_and_cut_boundary_segment(
-    audio_segment_path: Path, video_segment_path: Path, output_path: Path, **cut_kwargs
+    audio_segment_path: Path,
+    video_segment_path: Path,
+    output_path: Path,
+    video_codec: str | None = None,
+    **cut_kwargs,
 ) -> None:
     """Muxes and cuts a boundary segment.
 
     Args:
         audio_segment_path: A path to an audio segment.
         video_segment_path: A path to a video segment.
         output_path: An output path of the muxed segment.
+        video_codec: A video codec name.
         cut_kwargs: Cut keyword arguments: ``cut_at_start`` and ``cut_at_end``.
     """
 
     def prepare_ffmpeg_input_options(
         segment_path: Path, cut_at_start: float = 0, cut_at_end: float = 0
     ):
         assert cut_at_start or cut_at_end
         if cut_at_start > 0:
-            return ["-ss", f"{cut_at_start}s", "-i", segment_path]
+            return ["-ss", f"{cut_at_start:.6f}s", "-i", segment_path]
         elif cut_at_end > 0:
-            return ["-i", segment_path, "-to", f"{cut_at_end}s"]
+            return ["-i", segment_path, "-to", f"{cut_at_end:.6f}s"]
         else:
             return ["-i", segment_path]
 
     if not {"cut_at_start", "cut_at_end"} > cut_kwargs.keys():
         raise ValueError(
             "only cut_at_start or cut_at_end keyword argument is accepted in cut_kwargs"
         )
 
+    if video_segment_path and video_codec is None:
+        video_codec = ffmpeg.ffprobe_show_entries(
+            video_segment_path, "stream=codec_name"
+        )
+
     ffmpeg_input_options = []
     ffmpeg_codecs_options = []
 
     should_cut = bool(
         cut_kwargs.get("cut_at_start", 0) or cut_kwargs.get("cut_at_end", 0)
     )
     if should_cut is False:
         if video_segment_path:
-            ffmpeg_input_options += ["-i", str(video_segment_path)]
+            ffmpeg_input_options += ["-i", video_segment_path]
         if audio_segment_path:
-            ffmpeg_input_options += ["-i", str(audio_segment_path)]
-        ffmpeg.run_ffmpeg(ffmpeg_input_options + ["-c", "copy", str(output_path)])
+            ffmpeg_input_options += ["-i", audio_segment_path]
+        ffmpeg.run_ffmpeg(ffmpeg_input_options + ["-c", "copy", output_path])
     else:
         if video_segment_path:
             ffmpeg_input_options += prepare_ffmpeg_input_options(
                 video_segment_path, **cut_kwargs
             )
 
-            video_codec_name = ffmpeg.ffprobe_show_entries(
-                video_segment_path, "stream=codec_name"
-            )
-
             user_encoding_settings = os.environ.get(
-                f"YTPB_{video_codec_name.upper()}_ENCODING_SETTINGS", None
+                f"YTPB_{video_codec.upper()}_ENCODING_SETTINGS", None
             )
             if user_encoding_settings:
                 ffmpeg_codecs_options += ["-c:v"] + shlex.split(user_encoding_settings)
             else:
                 try:
                     ffmpeg_codecs_options += ["-c:v"] + shlex.split(
-                        DEFAULT_VIDEO_ENCODING_SETTINGS[video_codec_name]
+                        DEFAULT_VIDEO_ENCODING_SETTINGS[video_codec]
                     )
                 except KeyError:
                     raise ValueError(
                         "No encoding settings are availabe for"
-                        f"'{video_codec_name}' video codec"
+                        f"'{video_codec}' video codec"
                     )
 
         if audio_segment_path:
             ffmpeg_input_options += prepare_ffmpeg_input_options(
                 audio_segment_path, **cut_kwargs
             )
             ffmpeg_codecs_options += ["-c:a", "copy"]
 
+        additional_options: list[str] = []
+        if video_segment_path and video_codec == "h264":
+            # Ensure to have the same tbn values after re-encoding of segments
+            # and their concatenation (see the merge_segments() function).
+            additional_options += ["-video_track_timescale", "1k"]
+
         ffmpeg.run_ffmpeg(
-            ffmpeg_input_options + ffmpeg_codecs_options + [str(output_path)]
+            [
+                *ffmpeg_input_options,
+                *additional_options,
+                *ffmpeg_codecs_options,
+                output_path,
+            ]
         )
 
 
 def _compose_concat_file(segment_paths, temp_directory, suffix: str = ""):
     if suffix:
         concat_file_path = Path(temp_directory, f"concat_{suffix}")
     else:
@@ -141,14 +158,15 @@
     audio_segment_paths: list[Path] | None = None,
     video_segment_paths: list[Path] | None = None,
     output_directory: str | Path | None = None,
     output_stem: str | Path | None = None,
     temp_directory: str | Path | None = None,
     cut_at_start: float = 0,
     cut_at_end: float = 0,
+    metadata_tags: dict[str, str] = None,
     cleanup: bool = True,
 ) -> Path:
     """Merges and cuts media segments.
 
     The ``cut_at_start`` and ``cut_at_end`` arguments define the values to be
     passed to FFmpeg: ``-ss <cut_at_start>s`` and ``-to <cut_at_end>s``,
     respectively.
@@ -157,14 +175,15 @@
         audio_segment_paths: Paths to audio segments.
         video_segment_paths: Paths to video segments.
         output_directory: Where to output the merged file.
         output_stem: An output stem of the merged file.
         temp_directory: Where to store intermediate files.
         cut_at_start: An offset (in seconds) to cut at start.
         cut_at_end: An offset (in seconds) to cut at end.
+        metadata_tags: Metadata tags to write to the merged file.
         cleanup: Whether to cleanup intermediate files.
 
     Returns:
         A path of the merged file.
     """
     merge_segments.paths_to_cleanup = []
 
@@ -185,14 +204,20 @@
 
     if output_directory:
         output_directory = Path(output_directory)
     else:
         output_directory = Path.cwd()
     output_path = output_directory / f"{output_stem}{output_extension}"
 
+    metadata_options: list[str] = []
+    if metadata_tags:
+        metadata_options = ["-movflags", "use_metadata_tags", "-map_metadata", "0"]
+        for k, v in metadata_tags.items():
+            metadata_options.extend(["-metadata", f"{k}={v}"])
+
     safe_concat_options = ["-safe", "0", "-f", "concat"]
 
     should_cut = bool(cut_at_start or cut_at_end)
     if should_cut is False:
         no_cut_concat_options = []
         if video_segment_paths:
             concat_file_path = _compose_concat_file(
@@ -202,67 +227,80 @@
             no_cut_concat_options += safe_concat_options + ["-i", concat_file_path]
         if audio_segment_paths:
             concat_file_path = _compose_concat_file(
                 audio_segment_paths, temp_directory, suffix="audio"
             )
             merge_segments.paths_to_cleanup.append(concat_file_path)
             no_cut_concat_options += safe_concat_options + ["-i", concat_file_path]
-        ffmpeg.run_ffmpeg(no_cut_concat_options + ["-c", "copy", output_path])
+        ffmpeg.run_ffmpeg(
+            [*no_cut_concat_options, "-c", "copy", *metadata_options, output_path]
+        )
     else:
         num_of_segments = len(audio_segment_paths or video_segment_paths)
 
         start_audio_segment_path = get_nth_or_none(audio_segment_paths, 0)
         start_video_segment_path = get_nth_or_none(video_segment_paths, 0)
 
         end_audio_segment_path = get_nth_or_none(audio_segment_paths, -1)
         end_video_segment_path = get_nth_or_none(video_segment_paths, -1)
 
+        video_codec: str | None = None
+        if video_segment_paths:
+            video_codec = ffmpeg.ffprobe_show_entries(
+                video_segment_paths[0], "stream=codec_name"
+            )
+
         if num_of_segments == 1:
             segment_trimmed_path = Path(temp_directory, "a.a" + output_extension)
             mux_and_cut_boundary_segment(
                 start_audio_segment_path,
                 start_video_segment_path,
                 segment_trimmed_path,
+                video_codec,
                 cut_at_start=cut_at_start,
             )
             parts_to_merge = [segment_trimmed_path]
         elif num_of_segments == 2:
             start_trimmed_path = Path(temp_directory, "ab.a" + output_extension)
             mux_and_cut_boundary_segment(
                 start_audio_segment_path,
                 start_video_segment_path,
                 start_trimmed_path,
+                video_codec,
                 cut_at_start=cut_at_start,
             )
 
             end_trimmed_path = start_trimmed_path.with_stem("ab.b")
             mux_and_cut_boundary_segment(
                 end_audio_segment_path,
                 end_video_segment_path,
                 end_trimmed_path,
+                video_codec,
                 cut_at_end=cut_at_end,
             )
 
             parts_to_merge = [start_trimmed_path, end_trimmed_path]
         else:
             start_trimmed_path = Path(temp_directory, "abc.a" + output_extension)
             mux_and_cut_boundary_segment(
                 start_audio_segment_path,
                 start_video_segment_path,
                 start_trimmed_path,
+                video_codec,
                 cut_at_start=cut_at_start,
             )
 
             middle_concatenated_path = start_trimmed_path.with_stem("abc.b")
 
             end_trimmed_path = start_trimmed_path.with_stem("abc.c")
             mux_and_cut_boundary_segment(
                 end_audio_segment_path,
                 end_video_segment_path,
                 end_trimmed_path,
+                video_codec,
                 cut_at_end=cut_at_end,
             )
 
             bounds_slice = slice(1, -1)
             concat_filter_options = []
 
             if video_segment_paths:
@@ -279,34 +317,58 @@
                     audio_segment_paths[bounds_slice],
                     temp_directory,
                     suffix="audio",
                 )
                 concat_filter_options += safe_concat_options + ["-i", concat_file_path]
                 merge_segments.paths_to_cleanup.append(concat_file_path)
 
+            additional_options: list[str] = []
+            if video_segment_paths and video_codec == "h264":
+                additional_options += ["-video_track_timescale", "1k"]
+
             ffmpeg.run_ffmpeg(
-                concat_filter_options + ["-c", "copy", middle_concatenated_path],
+                [
+                    *concat_filter_options,
+                    *additional_options,
+                    "-c",
+                    "copy",
+                    middle_concatenated_path,
+                ],
                 capture_output=True,
                 check=True,
             )
 
             parts_to_merge = [
                 start_trimmed_path,
                 middle_concatenated_path,
                 end_trimmed_path,
             ]
 
         merge_segments.paths_to_cleanup.extend(parts_to_merge)
 
         if num_of_segments == 1:
             ffmpeg.run_ffmpeg(
-                ["-i", str(parts_to_merge[0]), "-c", "copy", str(output_path)]
+                [
+                    "-i",
+                    parts_to_merge[0],
+                    "-c",
+                    "copy",
+                    *metadata_options,
+                    output_path,
+                ]
             )
         else:
             concat_file_path = _compose_concat_file(parts_to_merge, temp_directory)
             ffmpeg.run_ffmpeg(
-                safe_concat_options
-                + ["-i", str(concat_file_path), "-c", "copy", str(output_path)]
+                [
+                    *safe_concat_options,
+                    "-i",
+                    concat_file_path,
+                    "-c",
+                    "copy",
+                    *metadata_options,
+                    output_path,
+                ]
             )
             merge_segments.paths_to_cleanup.append(concat_file_path)
 
     return output_path
```

### Comparing `ytpb-2024.4.12/src/ytpb/playback.py` & `ytpb-2024.4.20/src/ytpb/playback.py`

 * *Files identical despite different names*

### Comparing `ytpb-2024.4.12/src/ytpb/representations.py` & `ytpb-2024.4.20/src/ytpb/representations.py`

 * *Files identical despite different names*

### Comparing `ytpb-2024.4.12/src/ytpb/segment.py` & `ytpb-2024.4.20/src/ytpb/segment.py`

 * *Files identical despite different names*

### Comparing `ytpb-2024.4.12/src/ytpb/streams.py` & `ytpb-2024.4.20/src/ytpb/streams.py`

 * *Files identical despite different names*

### Comparing `ytpb-2024.4.12/src/ytpb/types.py` & `ytpb-2024.4.20/src/ytpb/types.py`

 * *Files identical despite different names*

### Comparing `ytpb-2024.4.12/src/ytpb/actions/capture.py` & `ytpb-2024.4.20/src/ytpb/actions/capture.py`

 * *Files identical despite different names*

### Comparing `ytpb-2024.4.12/src/ytpb/actions/compose.py` & `ytpb-2024.4.20/src/ytpb/actions/compose.py`

 * *Files identical despite different names*

### Comparing `ytpb-2024.4.12/src/ytpb/actions/download.py` & `ytpb-2024.4.20/src/ytpb/actions/download.py`

 * *Files identical despite different names*

### Comparing `ytpb-2024.4.12/src/ytpb/cli/__init__.py` & `ytpb-2024.4.20/src/ytpb/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `ytpb-2024.4.12/src/ytpb/cli/common.py` & `ytpb-2024.4.20/src/ytpb/cli/common.py`

 * *Files identical despite different names*

### Comparing `ytpb-2024.4.12/src/ytpb/cli/options.py` & `ytpb-2024.4.20/src/ytpb/cli/options.py`

 * *Files identical despite different names*

### Comparing `ytpb-2024.4.12/src/ytpb/cli/parameters.py` & `ytpb-2024.4.20/src/ytpb/cli/parameters.py`

 * *Files identical despite different names*

### Comparing `ytpb-2024.4.12/src/ytpb/cli/commands/capture.py` & `ytpb-2024.4.20/src/ytpb/cli/commands/capture.py`

 * *Files identical despite different names*

### Comparing `ytpb-2024.4.12/src/ytpb/cli/commands/download.py` & `ytpb-2024.4.20/src/ytpb/cli/commands/download.py`

 * *Files 4% similar despite different names*

```diff
@@ -119,14 +119,15 @@
 @click.option(
     "-X",
     "--dry-run",
     is_flag=True,
     help="Run without downloading.",
 )
 @yt_dlp_option
+@click.option("--no-metadata", is_flag=True, help="Do not write metadata tags.")
 @click.option("--no-cut", is_flag=True, help="Do not perform excerpt cutting.")
 @click.option(
     "--no-merge",
     is_flag=True,
     help="Only download segments, without merging. This implies '--no-cleanup'.",
 )
 @no_cleanup_option
@@ -142,14 +143,15 @@
     preview: bool,
     dump_base_urls: bool,
     dump_segment_urls: bool,
     output_path: Path,
     from_manifest: Path,
     dry_run: bool,
     yt_dlp: bool,
+    no_metadata: bool,
     no_cut: bool,
     no_merge: bool,
     no_cleanup: bool,
     force_update_cache: bool,
     no_cache: bool,
     stream_url: str,
 ) -> int:
@@ -393,22 +395,47 @@
                     audio_and_video_segment_paths = downloaded_segment_paths
 
             if no_cut:
                 click.echo("2. Merging segments (no cut requested)... ", nl=False)
             else:
                 click.echo("2. Merging segments (may take a while)... ", nl=False)
 
+            metadata_tags: dict[str, str] = {}
+            if not no_metadata:
+                convert_timestamp_to_string = lambda timestamp: f"{timestamp:.6f}"
+                metadata_tags = {
+                    "title": playback.info.title,
+                    "author": playback.info.author,
+                    "comment": playback.video_url,
+                    "actual_start_time": convert_timestamp_to_string(
+                        actual_date_interval.start.timestamp()
+                    ),
+                    "actual_end_time": convert_timestamp_to_string(
+                        actual_date_interval.end.timestamp()
+                    ),
+                    "input_start_time": convert_timestamp_to_string(
+                        requested_date_interval.start.timestamp()
+                    ),
+                    "input_end_time": convert_timestamp_to_string(
+                        requested_date_interval.end.timestamp()
+                    ),
+                    "start_sequence_number": rewind_interval.start.sequence,
+                    "end_sequence_number": rewind_interval.end.sequence,
+                }
+
             merged_path = merge_segments(
                 audio_and_video_segment_paths[0],
                 audio_and_video_segment_paths[1],
                 output_directory=final_output_path.parent,
                 output_stem=final_output_path.name,
                 temp_directory=playback.get_temp_directory(),
+                metadata_tags=metadata_tags,
                 **cut_kwargs,
             )
+
             click.echo("done.\n")
 
             try:
                 saved_to_path_value = f"{merged_path.relative_to(Path.cwd())}"
             except ValueError:
                 saved_to_path_value = merged_path
             click.echo(f"Success! Saved to '{saved_to_path_value}'.")
```

### Comparing `ytpb-2024.4.12/src/ytpb/cli/commands/mpd.py` & `ytpb-2024.4.20/src/ytpb/cli/commands/mpd.py`

 * *Files identical despite different names*

### Comparing `ytpb-2024.4.12/src/ytpb/utils/date.py` & `ytpb-2024.4.20/src/ytpb/utils/date.py`

 * *Files identical despite different names*

### Comparing `ytpb-2024.4.12/src/ytpb/utils/other.py` & `ytpb-2024.4.20/src/ytpb/utils/other.py`

 * *Files identical despite different names*

### Comparing `ytpb-2024.4.12/src/ytpb/utils/path.py` & `ytpb-2024.4.20/src/ytpb/utils/path.py`

 * *Files identical despite different names*

### Comparing `ytpb-2024.4.12/src/ytpb/utils/remote.py` & `ytpb-2024.4.20/src/ytpb/utils/remote.py`

 * *Files identical despite different names*

### Comparing `ytpb-2024.4.12/src/ytpb/utils/url.py` & `ytpb-2024.4.20/src/ytpb/utils/url.py`

 * *Files identical despite different names*

### Comparing `ytpb-2024.4.12/tests/conftest.py` & `ytpb-2024.4.20/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ytpb-2024.4.12/tests/helpers.py` & `ytpb-2024.4.20/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `ytpb-2024.4.12/tests/test_cache.py` & `ytpb-2024.4.20/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `ytpb-2024.4.12/tests/test_download.py` & `ytpb-2024.4.20/tests/test_download.py`

 * *Files identical despite different names*

### Comparing `ytpb-2024.4.12/tests/test_fetchers.py` & `ytpb-2024.4.20/tests/test_fetchers.py`

 * *Files identical despite different names*

### Comparing `ytpb-2024.4.12/tests/test_locate.py` & `ytpb-2024.4.20/tests/test_locate.py`

 * *Files identical despite different names*

### Comparing `ytpb-2024.4.12/tests/test_merge.py` & `ytpb-2024.4.20/tests/test_merge.py`

 * *Files identical despite different names*

### Comparing `ytpb-2024.4.12/tests/test_playback.py` & `ytpb-2024.4.20/tests/test_playback.py`

 * *Files identical despite different names*

### Comparing `ytpb-2024.4.12/tests/test_playback_session.py` & `ytpb-2024.4.20/tests/test_playback_session.py`

 * *Files identical despite different names*

### Comparing `ytpb-2024.4.12/tests/test_representations.py` & `ytpb-2024.4.20/tests/test_representations.py`

 * *Files identical despite different names*

### Comparing `ytpb-2024.4.12/tests/test_segment.py` & `ytpb-2024.4.20/tests/test_segment.py`

 * *Files identical despite different names*

### Comparing `ytpb-2024.4.12/tests/test_streams.py` & `ytpb-2024.4.20/tests/test_streams.py`

 * *Files identical despite different names*

### Comparing `ytpb-2024.4.12/tests/test_types.py` & `ytpb-2024.4.20/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `ytpb-2024.4.12/tests/actions/test_compose.py` & `ytpb-2024.4.20/tests/actions/test_compose.py`

 * *Files identical despite different names*

### Comparing `ytpb-2024.4.12/tests/actions/test_download.py` & `ytpb-2024.4.20/tests/actions/test_download.py`

 * *Files identical despite different names*

### Comparing `ytpb-2024.4.12/tests/cli/conftest.py` & `ytpb-2024.4.20/tests/cli/conftest.py`

 * *Files identical despite different names*

### Comparing `ytpb-2024.4.12/tests/cli/test_download_command.py` & `ytpb-2024.4.20/tests/cli/test_download_command.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 
 import toml
 from freezegun import freeze_time
 
 from helpers import assert_approx_duration
 
 from ytpb.config import DEFAULT_CONFIG
+from ytpb.ffmpeg import ffprobe_show_entries
 
 
 @pytest.mark.parametrize(
     "interval,output_subpath",
     [
         # Segments and corresponding ingestion start dates:
         #             7959120       21       22
@@ -1375,7 +1376,112 @@
         )
 
     assert result.exit_code == 0
     assert result.output == (
         f"{audio_base_url.rstrip('/')}/sq/[7959120-7959121]\n"
         f"{video_base_url.rstrip('/')}/sq/[7959120-7959121]\n"
     )
+
+
+@freeze_time("2023-03-26T00:00:00+00:00")
+def test_metadata_tags_with_cutting(
+    ytpb_cli_invoke: Callable,
+    add_responses_callback_for_reference_base_url: Callable,
+    add_responses_callback_for_segment_urls: Callable,
+    fake_info_fetcher: MagicMock,
+    stream_url: str,
+    audio_base_url: str,
+    tmp_path: Path,
+    expected_out,
+) -> None:
+    # Given:
+    add_responses_callback_for_reference_base_url()
+    add_responses_callback_for_segment_urls(
+        urljoin(audio_base_url, r"sq/\w+"),
+    )
+
+    # When:
+    with patch("ytpb.cli.common.YtpbInfoFetcher") as mock_fetcher:
+        mock_fetcher.return_value = fake_info_fetcher
+        result = ytpb_cli_invoke(
+            [
+                "--no-config",
+                "download",
+                "--no-cache",
+                "--interval",
+                "2023-03-25T23:33:55+00/2023-03-25T23:33:57+00",
+                "-af",
+                "itag eq 140",
+                "-vf",
+                "none",
+                stream_url,
+            ],
+            catch_exceptions=False,
+            standalone_mode=False,
+        )
+
+    # Then:
+    format_tags = ffprobe_show_entries(
+        tmp_path / "Webcam-Zurich-HB_20230325T233355+00.mp4", "format_tags", "default"
+    )
+    assert "TAG:title=Webcam Zürich HB" in format_tags
+    assert "TAG:author=David Gubler" in format_tags
+    assert f"TAG:comment={stream_url}" in format_tags
+    assert "TAG:input_start_time=1679787235.000000" in format_tags
+    assert "TAG:input_end_time=1679787237.000000" in format_tags
+    assert "TAG:actual_start_time=1679787235.000000" in format_tags
+    assert "TAG:actual_end_time=1679787237.000000" in format_tags
+    assert "TAG:start_sequence_number=7959120" in format_tags
+    assert "TAG:end_sequence_number=7959121" in format_tags
+
+
+@freeze_time("2023-03-26T00:00:00+00:00")
+def test_metadata_tags_without_cutting(
+    ytpb_cli_invoke: Callable,
+    add_responses_callback_for_reference_base_url: Callable,
+    add_responses_callback_for_segment_urls: Callable,
+    fake_info_fetcher: MagicMock,
+    stream_url: str,
+    audio_base_url: str,
+    tmp_path: Path,
+    expected_out,
+) -> None:
+    # Given:
+    add_responses_callback_for_reference_base_url()
+    add_responses_callback_for_segment_urls(
+        urljoin(audio_base_url, r"sq/\w+"),
+    )
+
+    # When:
+    with patch("ytpb.cli.common.YtpbInfoFetcher") as mock_fetcher:
+        mock_fetcher.return_value = fake_info_fetcher
+        result = ytpb_cli_invoke(
+            [
+                "--no-config",
+                "download",
+                "--no-cache",
+                "--interval",
+                "2023-03-25T23:33:55+00/2023-03-25T23:33:57+00",
+                "--no-cut",
+                "-af",
+                "itag eq 140",
+                "-vf",
+                "none",
+                stream_url,
+            ],
+            catch_exceptions=False,
+            standalone_mode=False,
+        )
+
+    # Then:
+    format_tags = ffprobe_show_entries(
+        tmp_path / "Webcam-Zurich-HB_20230325T233355+00.mp4", "format_tags", "default"
+    )
+    assert "TAG:title=Webcam Zürich HB" in format_tags
+    assert "TAG:author=David Gubler" in format_tags
+    assert f"TAG:comment={stream_url}" in format_tags
+    assert "TAG:input_start_time=1679787235.000000" in format_tags
+    assert "TAG:input_end_time=1679787237.000000" in format_tags
+    assert "TAG:actual_start_time=1679787234.491176" in format_tags
+    assert "TAG:actual_end_time=1679787238.486826" in format_tags
+    assert "TAG:start_sequence_number=7959120" in format_tags
+    assert "TAG:end_sequence_number=7959121" in format_tags
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `ytpb-2024.4.12/tests/cli/test_parameters.py` & `ytpb-2024.4.20/tests/cli/test_parameters.py`

 * *Files identical despite different names*

### Comparing `ytpb-2024.4.12/tests/cli/capture/test_frame_command.py` & `ytpb-2024.4.20/tests/cli/capture/test_frame_command.py`

 * *Files identical despite different names*

### Comparing `ytpb-2024.4.12/tests/cli/mpd/test_compose_command.py` & `ytpb-2024.4.20/tests/cli/mpd/test_compose_command.py`

 * *Files identical despite different names*

### Comparing `ytpb-2024.4.12/tests/cli/mpd/test_refresh_command.py` & `ytpb-2024.4.20/tests/cli/mpd/test_refresh_command.py`

 * *Files identical despite different names*

### Comparing `ytpb-2024.4.12/tests/data/info-1695928670.json` & `ytpb-2024.4.20/tests/data/info-1695928670.json`

 * *Files identical despite different names*

### Comparing `ytpb-2024.4.12/tests/data/manifest-1695928670.mpd` & `ytpb-2024.4.20/tests/data/manifest-1695928670.mpd`

 * *Files identical despite different names*

### Comparing `ytpb-2024.4.12/tests/data/webpage-1695928670.html` & `ytpb-2024.4.20/tests/data/webpage-1695928670.html`

 * *Files identical despite different names*

### Comparing `ytpb-2024.4.12/tests/data/expected/test_compose_mpd[itag%20eq%20140-itag%20eq%20243%20or%20itag%20eq%20244].out` & `ytpb-2024.4.20/tests/data/expected/test_compose_mpd[itag%20eq%20140-itag%20eq%20243%20or%20itag%20eq%20244].out`

 * *Files identical despite different names*

### Comparing `ytpb-2024.4.12/tests/data/expected/test_compose_mpd[itag%20eq%20140-none].out` & `ytpb-2024.4.20/tests/data/expected/test_compose_mpd[itag%20eq%20140-none].out`

 * *Files identical despite different names*

### Comparing `ytpb-2024.4.12/tests/data/expected/test_compose_mpd[none-itag%20eq%20243%20or%20itag%20eq%20244].out` & `ytpb-2024.4.20/tests/data/expected/test_compose_mpd[none-itag%20eq%20243%20or%20itag%20eq%20244].out`

 * *Files identical despite different names*

### Comparing `ytpb-2024.4.12/tests/data/expected/test_download_audio_and_or_video[itag%20eq%20140-itag%20eq%20244].out` & `ytpb-2024.4.20/tests/data/expected/test_download_audio_and_or_video[itag%20eq%20140-itag%20eq%20244].out`

 * *Files identical despite different names*

### Comparing `ytpb-2024.4.12/tests/data/expected/test_download_audio_and_or_video[itag%20eq%20140-none].out` & `ytpb-2024.4.20/tests/data/expected/test_download_audio_and_or_video[itag%20eq%20140-none].out`

 * *Files identical despite different names*

### Comparing `ytpb-2024.4.12/tests/data/expected/test_download_audio_and_or_video[none-itag%20eq%20244].out` & `ytpb-2024.4.20/tests/data/expected/test_download_audio_and_or_video[none-itag%20eq%20244].out`

 * *Files identical despite different names*

### Comparing `ytpb-2024.4.12/tests/data/expected/test_download_within_interval[2023-03-25T23%3A33%3A55%2B00%2F2023-03-25T23%3A33%3A57%2B00-233355%2B00.mp4].out` & `ytpb-2024.4.20/tests/data/expected/test_download_within_interval[2023-03-25T23%3A33%3A55%2B00%2F2023-03-25T23%3A33%3A57%2B00-233355%2B00.mp4].out`

 * *Files identical despite different names*

### Comparing `ytpb-2024.4.12/tests/data/expected/test_download_within_interval[2023-03-25T23%3A33%3A55%2B00%2F7959121-233355%2B00.mp4].out` & `ytpb-2024.4.20/tests/data/expected/test_download_within_interval[2023-03-25T23%3A33%3A55%2B00%2F7959121-233355%2B00.mp4].out`

 * *Files identical despite different names*

### Comparing `ytpb-2024.4.12/tests/data/expected/test_download_within_interval[2023-03-25T23%3A33%3A55%2B00%2FPT3S-233355%2B00.mp4].out` & `ytpb-2024.4.20/tests/data/expected/test_download_within_interval[2023-03-25T23%3A33%3A55%2B00%2FPT3S-233355%2B00.mp4].out`

 * *Files identical despite different names*

### Comparing `ytpb-2024.4.12/tests/data/expected/test_download_within_interval[7959120%2F2023-03-25T23%3A33%3A57%2B00-233354%2B00.mp4].out` & `ytpb-2024.4.20/tests/data/expected/test_download_within_interval[7959120%2F2023-03-25T23%3A33%3A57%2B00-233354%2B00.mp4].out`

 * *Files identical despite different names*

### Comparing `ytpb-2024.4.12/tests/data/expected/test_download_within_interval[7959120%2F7959121-233354%2B00.mp4].out` & `ytpb-2024.4.20/tests/data/expected/test_download_within_interval[7959120%2F7959121-233354%2B00.mp4].out`

 * *Files identical despite different names*

### Comparing `ytpb-2024.4.12/tests/data/expected/test_download_within_interval[7959120%2FPT3S-233354%2B00.mp4].out` & `ytpb-2024.4.20/tests/data/expected/test_download_within_interval[7959120%2FPT3S-233354%2B00.mp4].out`

 * *Files identical despite different names*

### Comparing `ytpb-2024.4.12/tests/data/expected/test_download_within_interval[PT3S%2F2023-03-25T23%3A33%3A58%2B00-233355%2B00.mp4].out` & `ytpb-2024.4.20/tests/data/expected/test_download_within_interval[PT3S%2F2023-03-25T23%3A33%3A58%2B00-233355%2B00.mp4].out`

 * *Files identical despite different names*

### Comparing `ytpb-2024.4.12/tests/data/expected/test_download_within_interval[PT3S%2F7959121-233355%2B00.mp4].out` & `ytpb-2024.4.20/tests/data/expected/test_download_within_interval[PT3S%2F7959121-233355%2B00.mp4].out`

 * *Files identical despite different names*

### Comparing `ytpb-2024.4.12/tests/data/expected/test_no_cut_option.out` & `ytpb-2024.4.20/tests/data/expected/test_no_cut_option.out`

 * *Files identical despite different names*

### Comparing `ytpb-2024.4.12/tests/data/expected/test_no_merge_option.out` & `ytpb-2024.4.20/tests/data/expected/test_no_merge_option.out`

 * *Files identical despite different names*

### Comparing `ytpb-2024.4.12/tests/data/gap-cases/gap-case-1-fixture.csv` & `ytpb-2024.4.20/tests/data/gap-cases/gap-case-1-fixture.csv`

 * *Files identical despite different names*

### Comparing `ytpb-2024.4.12/tests/data/gap-cases/gap-case-2-fixture.csv` & `ytpb-2024.4.20/tests/data/gap-cases/gap-case-2-fixture.csv`

 * *Files identical despite different names*

### Comparing `ytpb-2024.4.12/tests/data/gap-cases/gap-case-3-fixture.csv` & `ytpb-2024.4.20/tests/data/gap-cases/gap-case-3-fixture.csv`

 * *Files identical despite different names*

### Comparing `ytpb-2024.4.12/tests/data/segments/7959120.i140.mp4` & `ytpb-2024.4.20/tests/data/segments/7959120.i140.mp4`

 * *Files identical despite different names*

### Comparing `ytpb-2024.4.12/tests/data/segments/7959120.i244.webm` & `ytpb-2024.4.20/tests/data/segments/7959120.i244.webm`

 * *Files identical despite different names*

### Comparing `ytpb-2024.4.12/tests/data/segments/7959121.i140.mp4` & `ytpb-2024.4.20/tests/data/segments/7959121.i140.mp4`

 * *Files identical despite different names*

### Comparing `ytpb-2024.4.12/tests/data/segments/7959121.i244.webm` & `ytpb-2024.4.20/tests/data/segments/7959121.i244.webm`

 * *Files identical despite different names*

### Comparing `ytpb-2024.4.12/tests/data/segments/7959122.i140.mp4` & `ytpb-2024.4.20/tests/data/segments/7959122.i140.mp4`

 * *Files identical despite different names*

### Comparing `ytpb-2024.4.12/tests/data/segments/7959122.i244.webm` & `ytpb-2024.4.20/tests/data/segments/7959122.i244.webm`

 * *Files identical despite different names*

### Comparing `ytpb-2024.4.12/tests/data/segments/7959123.i140.mp4` & `ytpb-2024.4.20/tests/data/segments/7959123.i140.mp4`

 * *Files identical despite different names*

### Comparing `ytpb-2024.4.12/tests/data/segments/7959123.i244.webm` & `ytpb-2024.4.20/tests/data/segments/7959123.i244.webm`

 * *Files identical despite different names*

### Comparing `ytpb-2024.4.12/tests/data/segments/7959203.i140.mp4` & `ytpb-2024.4.20/tests/data/segments/7959203.i140.mp4`

 * *Files identical despite different names*

### Comparing `ytpb-2024.4.12/tests/data/segments/7959203.i244.webm` & `ytpb-2024.4.20/tests/data/segments/7959203.i244.webm`

 * *Files identical despite different names*

### Comparing `ytpb-2024.4.12/tests/utils/test_date.py` & `ytpb-2024.4.20/tests/utils/test_date.py`

 * *Files identical despite different names*

### Comparing `ytpb-2024.4.12/tests/utils/test_path.py` & `ytpb-2024.4.20/tests/utils/test_path.py`

 * *Files identical despite different names*

### Comparing `ytpb-2024.4.12/tests/utils/test_remote.py` & `ytpb-2024.4.20/tests/utils/test_remote.py`

 * *Files identical despite different names*

### Comparing `ytpb-2024.4.12/tests/utils/test_url.py` & `ytpb-2024.4.20/tests/utils/test_url.py`

 * *Files identical despite different names*

### Comparing `ytpb-2024.4.12/.gitignore` & `ytpb-2024.4.20/.gitignore`

 * *Files identical despite different names*

### Comparing `ytpb-2024.4.12/LICENSE` & `ytpb-2024.4.20/LICENSE`

 * *Files identical despite different names*

### Comparing `ytpb-2024.4.12/README.rst` & `ytpb-2024.4.20/README.rst`

 * *Files 20% similar despite different names*

```diff
@@ -46,22 +46,22 @@
 
   - Compose DASH manifests to play it in your favorite player
   - Transcode/download excerpts into local files with FFmpeg
 
 - Capture a single frame or create time-lapse images
 - Makes use of yt-dlp to reliably extract information about videos (optionally)
 
-Demo
-****
+Demos
+*****
 
-.. image:: https://asciinema.org/a/645203.svg
-   :target: https://asciinema.org/a/645203
-   :alt: Asciinema
-
-*A demo of ytpb usage, showing downloading a live stream excerpt.*
+- Downloading a live stream excerpt (`link <https://asciinema.org/a/653861>`__)
+- Composing an MPEG-DASH MPD and transcoding it to MP4 (`link
+  <https://asciinema.org/a/653865>`__)
+- Creating a time-lapse of a live stream excerpt (`link
+  <https://asciinema.org/a/653869>`__)
 
 Install
 *******
 
 Ytpb requires Python 3.11 or higher. The recommended way is to use `pipx
 <https://pypa.github.io/pipx/>`_: ::
```

### Comparing `ytpb-2024.4.12/pyproject.toml` & `ytpb-2024.4.20/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [ "hatchling", "hatch-vcs" ]
 build-backend = "hatchling.build"
 
 [project]
 name = "ytpb"
 description = "A playback for YouTube live streams"
 readme = "README.rst"
-version = "2024.4.12"
+version = "2024.4.20"
 authors = [ { name = "Maxim Stolyarchuk" } ]
 keywords = [ "youtube" ]
 classifiers = [
   "Development Status :: 4 - Beta",
   "Environment :: Console",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3.11",
```

### Comparing `ytpb-2024.4.12/PKG-INFO` & `ytpb-2024.4.20/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ytpb
-Version: 2024.4.12
+Version: 2024.4.20
 Summary: A playback for YouTube live streams
 Project-URL: Source, https://github.com/xymaxim/ytpb
 Project-URL: Documentation, https://ytpb.readthedocs.io
 Author: Maxim Stolyarchuk
 License: MIT License
         
         Copyright (c) 2024 Maxim Stolyarchuk
@@ -112,22 +112,22 @@
 
   - Compose DASH manifests to play it in your favorite player
   - Transcode/download excerpts into local files with FFmpeg
 
 - Capture a single frame or create time-lapse images
 - Makes use of yt-dlp to reliably extract information about videos (optionally)
 
-Demo
-****
+Demos
+*****
 
-.. image:: https://asciinema.org/a/645203.svg
-   :target: https://asciinema.org/a/645203
-   :alt: Asciinema
-
-*A demo of ytpb usage, showing downloading a live stream excerpt.*
+- Downloading a live stream excerpt (`link <https://asciinema.org/a/653861>`__)
+- Composing an MPEG-DASH MPD and transcoding it to MP4 (`link
+  <https://asciinema.org/a/653865>`__)
+- Creating a time-lapse of a live stream excerpt (`link
+  <https://asciinema.org/a/653869>`__)
 
 Install
 *******
 
 Ytpb requires Python 3.11 or higher. The recommended way is to use `pipx
 <https://pypa.github.io/pipx/>`_: ::
```

