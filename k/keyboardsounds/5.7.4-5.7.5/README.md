# Comparing `tmp/keyboardsounds-5.7.4.tar.gz` & `tmp/keyboardsounds-5.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keyboardsounds-5.7.4.tar", last modified: Tue Apr 16 06:56:36 2024, max compression
+gzip compressed data, was "keyboardsounds-5.7.5.tar", last modified: Fri Apr 19 22:39:56 2024, max compression
```

## Comparing `keyboardsounds-5.7.4.tar` & `keyboardsounds-5.7.5.tar`

### file list

```diff
@@ -1,163 +1,163 @@
-drwxrwxrwx   0        0        0        0 2024-04-16 06:56:36.983391 keyboardsounds-5.7.4/
--rw-rw-rw-   0        0        0     1095 2024-04-16 05:39:56.000000 keyboardsounds-5.7.4/LICENSE
--rw-rw-rw-   0        0        0    12969 2024-04-16 06:56:36.982390 keyboardsounds-5.7.4/PKG-INFO
--rw-rw-rw-   0        0        0    12279 2024-04-16 05:39:56.000000 keyboardsounds-5.7.4/README.md
-drwxrwxrwx   0        0        0        0 2024-04-16 06:56:36.665671 keyboardsounds-5.7.4/keyboardsounds/
--rw-rw-rw-   0        0        0     5020 2024-04-16 05:39:56.000000 keyboardsounds-5.7.4/keyboardsounds/app_detector.py
--rw-rw-rw-   0        0        0     6278 2024-04-16 05:39:56.000000 keyboardsounds-5.7.4/keyboardsounds/app_rules.py
--rw-rw-rw-   0        0        0    10174 2024-04-16 05:39:56.000000 keyboardsounds-5.7.4/keyboardsounds/audio_manager.py
--rw-rw-rw-   0        0        0     4601 2024-04-16 05:39:56.000000 keyboardsounds-5.7.4/keyboardsounds/daemon.py
--rw-rw-rw-   0        0        0    10220 2024-04-16 05:39:56.000000 keyboardsounds-5.7.4/keyboardsounds/daemon_manager.py
-drwxrwxrwx   0        0        0        0 2024-04-16 06:56:36.678672 keyboardsounds-5.7.4/keyboardsounds/external_api/
--rw-rw-rw-   0        0        0     1987 2024-04-16 05:39:56.000000 keyboardsounds-5.7.4/keyboardsounds/external_api/__connection_handler.py
--rw-rw-rw-   0        0        0     1826 2024-04-16 05:39:56.000000 keyboardsounds-5.7.4/keyboardsounds/external_api/__external_api.py
--rw-rw-rw-   0        0        0       68 2024-04-16 05:39:56.000000 keyboardsounds-5.7.4/keyboardsounds/external_api/__init__.py
--rw-rw-rw-   0        0        0    12278 2024-04-16 05:39:56.000000 keyboardsounds-5.7.4/keyboardsounds/main.py
--rw-rw-rw-   0        0        0      185 2024-04-16 05:39:56.000000 keyboardsounds-5.7.4/keyboardsounds/path_resolver.py
--rw-rw-rw-   0        0        0     3331 2024-04-16 05:39:56.000000 keyboardsounds-5.7.4/keyboardsounds/profile.py
--rw-rw-rw-   0        0        0    18692 2024-04-16 05:39:56.000000 keyboardsounds-5.7.4/keyboardsounds/profile_builder.py
--rw-rw-rw-   0        0        0     8946 2024-04-16 05:39:56.000000 keyboardsounds-5.7.4/keyboardsounds/profile_validation.py
-drwxrwxrwx   0        0        0        0 2024-04-16 06:56:36.656162 keyboardsounds-5.7.4/keyboardsounds/profiles/
-drwxrwxrwx   0        0        0        0 2024-04-16 06:56:36.713672 keyboardsounds-5.7.4/keyboardsounds/profiles/alpaca/
--rw-rw-rw-   0        0        0     1107 2024-04-16 05:39:56.000000 keyboardsounds-5.7.4/keyboardsounds/profiles/alpaca/LICENSE
--rw-rw-rw-   0        0        0     2506 2024-04-16 05:39:56.000000 keyboardsounds-5.7.4/keyboardsounds/profiles/alpaca/press_back.mp3
--rw-rw-rw-   0        0        0     2506 2024-04-16 05:39:56.000000 keyboardsounds-5.7.4/keyboardsounds/profiles/alpaca/press_enter.mp3
--rw-rw-rw-   0        0        0     2088 2024-04-16 05:39:56.000000 keyboardsounds-5.7.4/keyboardsounds/profiles/alpaca/press_key1.mp3
--rw-rw-rw-   0        0        0     2088 2024-04-16 05:39:56.000000 keyboardsounds-5.7.4/keyboardsounds/profiles/alpaca/press_key2.mp3
--rw-rw-rw-   0        0        0     2088 2024-04-16 05:39:56.000000 keyboardsounds-5.7.4/keyboardsounds/profiles/alpaca/press_key3.mp3
--rw-rw-rw-   0        0        0     2088 2024-04-16 05:39:56.000000 keyboardsounds-5.7.4/keyboardsounds/profiles/alpaca/press_key4.mp3
--rw-rw-rw-   0        0        0     2088 2024-04-16 05:39:56.000000 keyboardsounds-5.7.4/keyboardsounds/profiles/alpaca/press_key5.mp3
--rw-rw-rw-   0        0        0     2506 2024-04-16 05:39:56.000000 keyboardsounds-5.7.4/keyboardsounds/profiles/alpaca/press_space.mp3
--rw-rw-rw-   0        0        0     1028 2024-04-16 05:39:56.000000 keyboardsounds-5.7.4/keyboardsounds/profiles/alpaca/profile.yaml
--rw-rw-rw-   0        0        0     2088 2024-04-16 05:39:56.000000 keyboardsounds-5.7.4/keyboardsounds/profiles/alpaca/release_back.mp3
--rw-rw-rw-   0        0        0     2088 2024-04-16 05:39:56.000000 keyboardsounds-5.7.4/keyboardsounds/profiles/alpaca/release_enter.mp3
--rw-rw-rw-   0        0        0     2088 2024-04-16 05:39:56.000000 keyboardsounds-5.7.4/keyboardsounds/profiles/alpaca/release_key.mp3
--rw-rw-rw-   0        0        0     2088 2024-04-16 05:39:56.000000 keyboardsounds-5.7.4/keyboardsounds/profiles/alpaca/release_space.mp3
-drwxrwxrwx   0        0        0        0 2024-04-16 06:56:36.746754 keyboardsounds-5.7.4/keyboardsounds/profiles/gateron-black-ink/
--rw-rw-rw-   0        0        0     1107 2024-04-16 05:39:56.000000 keyboardsounds-5.7.4/keyboardsounds/profiles/gateron-black-ink/LICENSE
--rw-rw-rw-   0        0        0     2088 2024-04-16 05:39:56.000000 keyboardsounds-5.7.4/keyboardsounds/profiles/gateron-black-ink/press_back.mp3
--rw-rw-rw-   0        0        0     2088 2024-04-16 05:39:56.000000 keyboardsounds-5.7.4/keyboardsounds/profiles/gateron-black-ink/press_enter.mp3
--rw-rw-rw-   0        0        0     2088 2024-04-16 05:39:56.000000 keyboardsounds-5.7.4/keyboardsounds/profiles/gateron-black-ink/press_key1.mp3
--rw-rw-rw-   0        0        0     2088 2024-04-16 05:39:56.000000 keyboardsounds-5.7.4/keyboardsounds/profiles/gateron-black-ink/press_key2.mp3
--rw-rw-rw-   0        0        0     2088 2024-04-16 05:39:56.000000 keyboardsounds-5.7.4/keyboardsounds/profiles/gateron-black-ink/press_key3.mp3
--rw-rw-rw-   0        0        0     2088 2024-04-16 05:39:56.000000 keyboardsounds-5.7.4/keyboardsounds/profiles/gateron-black-ink/press_key4.mp3
--rw-rw-rw-   0        0        0     2088 2024-04-16 05:39:56.000000 keyboardsounds-5.7.4/keyboardsounds/profiles/gateron-black-ink/press_key5.mp3
--rw-rw-rw-   0        0        0     2088 2024-04-16 05:39:56.000000 keyboardsounds-5.7.4/keyboardsounds/profiles/gateron-black-ink/press_space.mp3
--rw-rw-rw-   0        0        0     1040 2024-04-16 05:39:56.000000 keyboardsounds-5.7.4/keyboardsounds/profiles/gateron-black-ink/profile.yaml
--rw-rw-rw-   0        0        0     2506 2024-04-16 05:39:56.000000 keyboardsounds-5.7.4/keyboardsounds/profiles/gateron-black-ink/release_back.mp3
--rw-rw-rw-   0        0        0     2088 2024-04-16 05:39:56.000000 keyboardsounds-5.7.4/keyboardsounds/profiles/gateron-black-ink/release_enter.mp3
--rw-rw-rw-   0        0        0     2088 2024-04-16 05:39:56.000000 keyboardsounds-5.7.4/keyboardsounds/profiles/gateron-black-ink/release_key.mp3
--rw-rw-rw-   0        0        0     2088 2024-04-16 05:39:56.000000 keyboardsounds-5.7.4/keyboardsounds/profiles/gateron-black-ink/release_space.mp3
-drwxrwxrwx   0        0        0        0 2024-04-16 06:56:36.782307 keyboardsounds-5.7.4/keyboardsounds/profiles/gateron-red-ink/
--rw-rw-rw-   0        0        0     1107 2024-04-16 05:39:56.000000 keyboardsounds-5.7.4/keyboardsounds/profiles/gateron-red-ink/LICENSE
--rw-rw-rw-   0        0        0     2088 2024-04-16 05:39:56.000000 keyboardsounds-5.7.4/keyboardsounds/profiles/gateron-red-ink/press_back.mp3
--rw-rw-rw-   0        0        0     2924 2024-04-16 05:39:56.000000 keyboardsounds-5.7.4/keyboardsounds/profiles/gateron-red-ink/press_enter.mp3
--rw-rw-rw-   0        0        0     2506 2024-04-16 05:39:56.000000 keyboardsounds-5.7.4/keyboardsounds/profiles/gateron-red-ink/press_key1.mp3
--rw-rw-rw-   0        0        0     2506 2024-04-16 05:39:56.000000 keyboardsounds-5.7.4/keyboardsounds/profiles/gateron-red-ink/press_key2.mp3
--rw-rw-rw-   0        0        0     2506 2024-04-16 05:39:56.000000 keyboardsounds-5.7.4/keyboardsounds/profiles/gateron-red-ink/press_key3.mp3
--rw-rw-rw-   0        0        0     2506 2024-04-16 05:39:56.000000 keyboardsounds-5.7.4/keyboardsounds/profiles/gateron-red-ink/press_key4.mp3
--rw-rw-rw-   0        0        0     2506 2024-04-16 05:39:56.000000 keyboardsounds-5.7.4/keyboardsounds/profiles/gateron-red-ink/press_key5.mp3
--rw-rw-rw-   0        0        0     2506 2024-04-16 05:39:56.000000 keyboardsounds-5.7.4/keyboardsounds/profiles/gateron-red-ink/press_space.mp3
--rw-rw-rw-   0        0        0     1036 2024-04-16 05:39:56.000000 keyboardsounds-5.7.4/keyboardsounds/profiles/gateron-red-ink/profile.yaml
--rw-rw-rw-   0        0        0     2088 2024-04-16 05:39:56.000000 keyboardsounds-5.7.4/keyboardsounds/profiles/gateron-red-ink/release_back.mp3
--rw-rw-rw-   0        0        0     2088 2024-04-16 05:39:56.000000 keyboardsounds-5.7.4/keyboardsounds/profiles/gateron-red-ink/release_enter.mp3
--rw-rw-rw-   0        0        0     2088 2024-04-16 05:39:56.000000 keyboardsounds-5.7.4/keyboardsounds/profiles/gateron-red-ink/release_key.mp3
--rw-rw-rw-   0        0        0     2088 2024-04-16 05:39:56.000000 keyboardsounds-5.7.4/keyboardsounds/profiles/gateron-red-ink/release_space.mp3
-drwxrwxrwx   0        0        0        0 2024-04-16 06:56:36.816561 keyboardsounds-5.7.4/keyboardsounds/profiles/holy-panda/
--rw-rw-rw-   0        0        0     1107 2024-04-16 05:39:56.000000 keyboardsounds-5.7.4/keyboardsounds/profiles/holy-panda/LICENSE
--rw-rw-rw-   0        0        0     2088 2024-04-16 05:39:56.000000 keyboardsounds-5.7.4/keyboardsounds/profiles/holy-panda/press_back.mp3
--rw-rw-rw-   0        0        0     2088 2024-04-16 05:39:56.000000 keyboardsounds-5.7.4/keyboardsounds/profiles/holy-panda/press_enter.mp3
--rw-rw-rw-   0        0        0     2088 2024-04-16 05:39:56.000000 keyboardsounds-5.7.4/keyboardsounds/profiles/holy-panda/press_key1.mp3
--rw-rw-rw-   0        0        0     2088 2024-04-16 05:39:56.000000 keyboardsounds-5.7.4/keyboardsounds/profiles/holy-panda/press_key2.mp3
--rw-rw-rw-   0        0        0     2088 2024-04-16 05:39:56.000000 keyboardsounds-5.7.4/keyboardsounds/profiles/holy-panda/press_key3.mp3
--rw-rw-rw-   0        0        0     2088 2024-04-16 05:39:56.000000 keyboardsounds-5.7.4/keyboardsounds/profiles/holy-panda/press_key4.mp3
--rw-rw-rw-   0        0        0     2088 2024-04-16 05:39:56.000000 keyboardsounds-5.7.4/keyboardsounds/profiles/holy-panda/press_key5.mp3
--rw-rw-rw-   0        0        0     5850 2024-04-16 05:39:56.000000 keyboardsounds-5.7.4/keyboardsounds/profiles/holy-panda/press_space.mp3
--rw-rw-rw-   0        0        0     1026 2024-04-16 05:39:56.000000 keyboardsounds-5.7.4/keyboardsounds/profiles/holy-panda/profile.yaml
--rw-rw-rw-   0        0        0     1670 2024-04-16 05:39:56.000000 keyboardsounds-5.7.4/keyboardsounds/profiles/holy-panda/release_back.mp3
--rw-rw-rw-   0        0        0     1252 2024-04-16 05:39:56.000000 keyboardsounds-5.7.4/keyboardsounds/profiles/holy-panda/release_enter.mp3
--rw-rw-rw-   0        0        0     2088 2024-04-16 05:39:56.000000 keyboardsounds-5.7.4/keyboardsounds/profiles/holy-panda/release_key.mp3
--rw-rw-rw-   0        0        0     1252 2024-04-16 05:39:56.000000 keyboardsounds-5.7.4/keyboardsounds/profiles/holy-panda/release_space.mp3
-drwxrwxrwx   0        0        0        0 2024-04-16 06:56:36.818560 keyboardsounds-5.7.4/keyboardsounds/profiles/ios/
--rw-rw-rw-   0        0        0   740450 2024-04-16 05:39:56.000000 keyboardsounds-5.7.4/keyboardsounds/profiles/ios/ios-video-recording.mp4
--rw-rw-rw-   0        0        0      668 2024-04-16 05:39:56.000000 keyboardsounds-5.7.4/keyboardsounds/profiles/ios/profile.yaml
-drwxrwxrwx   0        0        0        0 2024-04-16 06:56:36.850568 keyboardsounds-5.7.4/keyboardsounds/profiles/mx-black/
--rw-rw-rw-   0        0        0     1107 2024-04-16 05:39:56.000000 keyboardsounds-5.7.4/keyboardsounds/profiles/mx-black/LICENSE
--rw-rw-rw-   0        0        0     2088 2024-04-16 05:39:56.000000 keyboardsounds-5.7.4/keyboardsounds/profiles/mx-black/press_back.mp3
--rw-rw-rw-   0        0        0     2506 2024-04-16 05:39:56.000000 keyboardsounds-5.7.4/keyboardsounds/profiles/mx-black/press_enter.mp3
--rw-rw-rw-   0        0        0     2088 2024-04-16 05:39:56.000000 keyboardsounds-5.7.4/keyboardsounds/profiles/mx-black/press_key1.mp3
--rw-rw-rw-   0        0        0     2088 2024-04-16 05:39:56.000000 keyboardsounds-5.7.4/keyboardsounds/profiles/mx-black/press_key2.mp3
--rw-rw-rw-   0        0        0     2088 2024-04-16 05:39:56.000000 keyboardsounds-5.7.4/keyboardsounds/profiles/mx-black/press_key3.mp3
--rw-rw-rw-   0        0        0     2088 2024-04-16 05:39:56.000000 keyboardsounds-5.7.4/keyboardsounds/profiles/mx-black/press_key4.mp3
--rw-rw-rw-   0        0        0     2088 2024-04-16 05:39:56.000000 keyboardsounds-5.7.4/keyboardsounds/profiles/mx-black/press_key5.mp3
--rw-rw-rw-   0        0        0     2506 2024-04-16 05:39:56.000000 keyboardsounds-5.7.4/keyboardsounds/profiles/mx-black/press_space.mp3
--rw-rw-rw-   0        0        0     1029 2024-04-16 05:39:56.000000 keyboardsounds-5.7.4/keyboardsounds/profiles/mx-black/profile.yaml
--rw-rw-rw-   0        0        0     2088 2024-04-16 05:39:56.000000 keyboardsounds-5.7.4/keyboardsounds/profiles/mx-black/release_back.mp3
--rw-rw-rw-   0        0        0     2088 2024-04-16 05:39:56.000000 keyboardsounds-5.7.4/keyboardsounds/profiles/mx-black/release_enter.mp3
--rw-rw-rw-   0        0        0     1670 2024-04-16 05:39:56.000000 keyboardsounds-5.7.4/keyboardsounds/profiles/mx-black/release_key.mp3
--rw-rw-rw-   0        0        0     2506 2024-04-16 05:39:56.000000 keyboardsounds-5.7.4/keyboardsounds/profiles/mx-black/release_space.mp3
-drwxrwxrwx   0        0        0        0 2024-04-16 06:56:36.868076 keyboardsounds-5.7.4/keyboardsounds/profiles/mx-blue/
--rw-rw-rw-   0        0        0     1107 2024-04-16 05:39:56.000000 keyboardsounds-5.7.4/keyboardsounds/profiles/mx-blue/LICENSE
--rw-rw-rw-   0        0        0     2088 2024-04-16 05:39:56.000000 keyboardsounds-5.7.4/keyboardsounds/profiles/mx-blue/press_key1.mp3
--rw-rw-rw-   0        0        0     2088 2024-04-16 05:39:56.000000 keyboardsounds-5.7.4/keyboardsounds/profiles/mx-blue/press_key2.mp3
--rw-rw-rw-   0        0        0     2088 2024-04-16 05:39:56.000000 keyboardsounds-5.7.4/keyboardsounds/profiles/mx-blue/press_key3.mp3
--rw-rw-rw-   0        0        0     2088 2024-04-16 05:39:56.000000 keyboardsounds-5.7.4/keyboardsounds/profiles/mx-blue/press_key4.mp3
--rw-rw-rw-   0        0        0     2088 2024-04-16 05:39:56.000000 keyboardsounds-5.7.4/keyboardsounds/profiles/mx-blue/press_key5.mp3
--rw-rw-rw-   0        0        0      530 2024-04-16 05:39:56.000000 keyboardsounds-5.7.4/keyboardsounds/profiles/mx-blue/profile.yaml
--rw-rw-rw-   0        0        0     1670 2024-04-16 05:39:56.000000 keyboardsounds-5.7.4/keyboardsounds/profiles/mx-blue/release.mp3
-drwxrwxrwx   0        0        0        0 2024-04-16 06:56:36.902077 keyboardsounds-5.7.4/keyboardsounds/profiles/mx-brown/
--rw-rw-rw-   0        0        0     1107 2024-04-16 05:39:56.000000 keyboardsounds-5.7.4/keyboardsounds/profiles/mx-brown/LICENSE
--rw-rw-rw-   0        0        0     2506 2024-04-16 05:39:56.000000 keyboardsounds-5.7.4/keyboardsounds/profiles/mx-brown/press_back.mp3
--rw-rw-rw-   0        0        0     2506 2024-04-16 05:39:56.000000 keyboardsounds-5.7.4/keyboardsounds/profiles/mx-brown/press_enter.mp3
--rw-rw-rw-   0        0        0     2506 2024-04-16 05:39:56.000000 keyboardsounds-5.7.4/keyboardsounds/profiles/mx-brown/press_key1.mp3
--rw-rw-rw-   0        0        0     2506 2024-04-16 05:39:56.000000 keyboardsounds-5.7.4/keyboardsounds/profiles/mx-brown/press_key2.mp3
--rw-rw-rw-   0        0        0     2506 2024-04-16 05:39:56.000000 keyboardsounds-5.7.4/keyboardsounds/profiles/mx-brown/press_key3.mp3
--rw-rw-rw-   0        0        0     2506 2024-04-16 05:39:56.000000 keyboardsounds-5.7.4/keyboardsounds/profiles/mx-brown/press_key4.mp3
--rw-rw-rw-   0        0        0     2506 2024-04-16 05:39:56.000000 keyboardsounds-5.7.4/keyboardsounds/profiles/mx-brown/press_key5.mp3
--rw-rw-rw-   0        0        0     1670 2024-04-16 05:39:56.000000 keyboardsounds-5.7.4/keyboardsounds/profiles/mx-brown/press_space.mp3
--rw-rw-rw-   0        0        0     1029 2024-04-16 05:39:56.000000 keyboardsounds-5.7.4/keyboardsounds/profiles/mx-brown/profile.yaml
--rw-rw-rw-   0        0        0     2088 2024-04-16 05:39:56.000000 keyboardsounds-5.7.4/keyboardsounds/profiles/mx-brown/release_back.mp3
--rw-rw-rw-   0        0        0     4596 2024-04-16 05:39:56.000000 keyboardsounds-5.7.4/keyboardsounds/profiles/mx-brown/release_enter.mp3
--rw-rw-rw-   0        0        0     2088 2024-04-16 05:39:56.000000 keyboardsounds-5.7.4/keyboardsounds/profiles/mx-brown/release_key.mp3
--rw-rw-rw-   0        0        0     1670 2024-04-16 05:39:56.000000 keyboardsounds-5.7.4/keyboardsounds/profiles/mx-brown/release_space.mp3
-drwxrwxrwx   0        0        0        0 2024-04-16 06:56:36.923075 keyboardsounds-5.7.4/keyboardsounds/profiles/mx-speed-silver/
--rw-rw-rw-   0        0        0    28336 2024-04-16 05:39:56.000000 keyboardsounds-5.7.4/keyboardsounds/profiles/mx-speed-silver/mx-speed-silver-1.wav
--rw-rw-rw-   0        0        0    34328 2024-04-16 05:39:56.000000 keyboardsounds-5.7.4/keyboardsounds/profiles/mx-speed-silver/mx-speed-silver-2.wav
--rw-rw-rw-   0        0        0    31488 2024-04-16 05:39:56.000000 keyboardsounds-5.7.4/keyboardsounds/profiles/mx-speed-silver/mx-speed-silver-3.wav
--rw-rw-rw-   0        0        0    31176 2024-04-16 05:39:56.000000 keyboardsounds-5.7.4/keyboardsounds/profiles/mx-speed-silver/mx-speed-silver-4.wav
--rw-rw-rw-   0        0        0    32228 2024-04-16 05:39:56.000000 keyboardsounds-5.7.4/keyboardsounds/profiles/mx-speed-silver/mx-speed-silver-5.wav
--rw-rw-rw-   0        0        0    32016 2024-04-16 05:39:56.000000 keyboardsounds-5.7.4/keyboardsounds/profiles/mx-speed-silver/mx-speed-silver-6.wav
--rw-rw-rw-   0        0        0      514 2024-04-16 05:39:56.000000 keyboardsounds-5.7.4/keyboardsounds/profiles/mx-speed-silver/profile.yaml
-drwxrwxrwx   0        0        0        0 2024-04-16 06:56:36.963102 keyboardsounds-5.7.4/keyboardsounds/profiles/telios-v2/
--rw-rw-rw-   0        0        0    28076 2024-04-16 05:39:56.000000 keyboardsounds-5.7.4/keyboardsounds/profiles/telios-v2/back.wav
--rw-rw-rw-   0        0        0    31916 2024-04-16 05:39:56.000000 keyboardsounds-5.7.4/keyboardsounds/profiles/telios-v2/caps.wav
--rw-rw-rw-   0        0        0    32812 2024-04-16 05:39:56.000000 keyboardsounds-5.7.4/keyboardsounds/profiles/telios-v2/ctrl.wav
--rw-rw-rw-   0        0        0    22316 2024-04-16 05:39:56.000000 keyboardsounds-5.7.4/keyboardsounds/profiles/telios-v2/ent.wav
--rw-rw-rw-   0        0        0    42540 2024-04-16 05:39:56.000000 keyboardsounds-5.7.4/keyboardsounds/profiles/telios-v2/key1.wav
--rw-rw-rw-   0        0        0    26316 2024-04-16 05:39:56.000000 keyboardsounds-5.7.4/keyboardsounds/profiles/telios-v2/key2.wav
--rw-rw-rw-   0        0        0    25516 2024-04-16 05:39:56.000000 keyboardsounds-5.7.4/keyboardsounds/profiles/telios-v2/key3.wav
--rw-rw-rw-   0        0        0    25612 2024-04-16 05:39:56.000000 keyboardsounds-5.7.4/keyboardsounds/profiles/telios-v2/key4.wav
--rw-rw-rw-   0        0        0    28300 2024-04-16 05:39:56.000000 keyboardsounds-5.7.4/keyboardsounds/profiles/telios-v2/key5.wav
--rw-rw-rw-   0        0        0    26860 2024-04-16 05:39:56.000000 keyboardsounds-5.7.4/keyboardsounds/profiles/telios-v2/key6.wav
--rw-rw-rw-   0        0        0      982 2024-04-16 05:39:56.000000 keyboardsounds-5.7.4/keyboardsounds/profiles/telios-v2/profile.yaml
--rw-rw-rw-   0        0        0    23596 2024-04-16 05:39:56.000000 keyboardsounds-5.7.4/keyboardsounds/profiles/telios-v2/shift.wav
--rw-rw-rw-   0        0        0    23212 2024-04-16 05:39:56.000000 keyboardsounds-5.7.4/keyboardsounds/profiles/telios-v2/space.wav
--rw-rw-rw-   0        0        0    38060 2024-04-16 05:39:56.000000 keyboardsounds-5.7.4/keyboardsounds/profiles/telios-v2/tab.wav
-drwxrwxrwx   0        0        0        0 2024-04-16 06:56:36.981391 keyboardsounds-5.7.4/keyboardsounds/profiles/typewriter/
--rw-rw-rw-   0        0        0    60204 2024-04-16 05:39:56.000000 keyboardsounds-5.7.4/keyboardsounds/profiles/typewriter/delete.wav
--rw-rw-rw-   0        0        0   146204 2024-04-16 05:39:56.000000 keyboardsounds-5.7.4/keyboardsounds/profiles/typewriter/enter.wav
--rw-rw-rw-   0        0        0    32664 2024-04-16 05:39:56.000000 keyboardsounds-5.7.4/keyboardsounds/profiles/typewriter/key.wav
--rw-rw-rw-   0        0        0    31588 2024-04-16 05:39:56.000000 keyboardsounds-5.7.4/keyboardsounds/profiles/typewriter/key2.wav
--rw-rw-rw-   0        0        0      610 2024-04-16 05:39:56.000000 keyboardsounds-5.7.4/keyboardsounds/profiles/typewriter/profile.yaml
--rw-rw-rw-   0        0        0    35788 2024-04-16 05:39:56.000000 keyboardsounds-5.7.4/keyboardsounds/profiles/typewriter/space.wav
--rw-rw-rw-   0        0        0       61 2024-04-16 05:39:56.000000 keyboardsounds-5.7.4/keyboardsounds/root.py
-drwxrwxrwx   0        0        0        0 2024-04-16 06:56:36.982390 keyboardsounds-5.7.4/keyboardsounds.egg-info/
--rw-rw-rw-   0        0        0    12969 2024-04-16 06:56:36.000000 keyboardsounds-5.7.4/keyboardsounds.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     6760 2024-04-16 06:56:36.000000 keyboardsounds-5.7.4/keyboardsounds.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-16 06:56:36.000000 keyboardsounds-5.7.4/keyboardsounds.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       91 2024-04-16 06:56:36.000000 keyboardsounds-5.7.4/keyboardsounds.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       76 2024-04-16 06:56:36.000000 keyboardsounds-5.7.4/keyboardsounds.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-04-16 06:56:36.000000 keyboardsounds-5.7.4/keyboardsounds.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      727 2024-04-16 06:45:10.000000 keyboardsounds-5.7.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-16 06:56:36.983391 keyboardsounds-5.7.4/setup.cfg
--rw-rw-rw-   0        0        0     1145 2024-04-16 06:55:03.000000 keyboardsounds-5.7.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-19 22:39:56.802567 keyboardsounds-5.7.5/
+-rw-rw-rw-   0        0        0     1095 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/LICENSE
+-rw-rw-rw-   0        0        0    13713 2024-04-19 22:39:56.801569 keyboardsounds-5.7.5/PKG-INFO
+-rw-rw-rw-   0        0        0    13023 2024-04-19 22:39:41.000000 keyboardsounds-5.7.5/README.md
+drwxrwxrwx   0        0        0        0 2024-04-19 22:39:56.687371 keyboardsounds-5.7.5/keyboardsounds/
+-rw-rw-rw-   0        0        0     5020 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/app_detector.py
+-rw-rw-rw-   0        0        0     6278 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/app_rules.py
+-rw-rw-rw-   0        0        0    10174 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/audio_manager.py
+-rw-rw-rw-   0        0        0     4601 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/daemon.py
+-rw-rw-rw-   0        0        0    10220 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/daemon_manager.py
+drwxrwxrwx   0        0        0        0 2024-04-19 22:39:56.700430 keyboardsounds-5.7.5/keyboardsounds/external_api/
+-rw-rw-rw-   0        0        0     1987 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/external_api/__connection_handler.py
+-rw-rw-rw-   0        0        0     1826 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/external_api/__external_api.py
+-rw-rw-rw-   0        0        0       68 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/external_api/__init__.py
+-rw-rw-rw-   0        0        0    14375 2024-04-19 22:39:41.000000 keyboardsounds-5.7.5/keyboardsounds/main.py
+-rw-rw-rw-   0        0        0      185 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/path_resolver.py
+-rw-rw-rw-   0        0        0     6304 2024-04-19 22:39:41.000000 keyboardsounds-5.7.5/keyboardsounds/profile.py
+-rw-rw-rw-   0        0        0    18692 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profile_builder.py
+-rw-rw-rw-   0        0        0     8946 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profile_validation.py
+drwxrwxrwx   0        0        0        0 2024-04-19 22:39:56.677359 keyboardsounds-5.7.5/keyboardsounds/profiles/
+drwxrwxrwx   0        0        0        0 2024-04-19 22:39:56.714609 keyboardsounds-5.7.5/keyboardsounds/profiles/alpaca/
+-rw-rw-rw-   0        0        0     1107 2024-04-19 22:33:46.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/alpaca/LICENSE
+-rw-rw-rw-   0        0        0     2506 2024-04-19 22:25:39.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/alpaca/press_back.mp3
+-rw-rw-rw-   0        0        0     2506 2024-04-19 22:25:39.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/alpaca/press_enter.mp3
+-rw-rw-rw-   0        0        0     2088 2024-04-19 22:25:39.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/alpaca/press_key1.mp3
+-rw-rw-rw-   0        0        0     2088 2024-04-19 22:25:39.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/alpaca/press_key2.mp3
+-rw-rw-rw-   0        0        0     2088 2024-04-19 22:25:39.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/alpaca/press_key3.mp3
+-rw-rw-rw-   0        0        0     2088 2024-04-19 22:25:39.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/alpaca/press_key4.mp3
+-rw-rw-rw-   0        0        0     2088 2024-04-19 22:25:39.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/alpaca/press_key5.mp3
+-rw-rw-rw-   0        0        0     2506 2024-04-19 22:25:39.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/alpaca/press_space.mp3
+-rw-rw-rw-   0        0        0     1028 2024-04-19 22:33:46.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/alpaca/profile.yaml
+-rw-rw-rw-   0        0        0     2088 2024-04-19 22:25:39.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/alpaca/release_back.mp3
+-rw-rw-rw-   0        0        0     2088 2024-04-19 22:25:39.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/alpaca/release_enter.mp3
+-rw-rw-rw-   0        0        0     2088 2024-04-19 22:25:39.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/alpaca/release_key.mp3
+-rw-rw-rw-   0        0        0     2088 2024-04-19 22:25:39.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/alpaca/release_space.mp3
+drwxrwxrwx   0        0        0        0 2024-04-19 22:39:56.725121 keyboardsounds-5.7.5/keyboardsounds/profiles/gateron-black-ink/
+-rw-rw-rw-   0        0        0     1107 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/gateron-black-ink/LICENSE
+-rw-rw-rw-   0        0        0     2088 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/gateron-black-ink/press_back.mp3
+-rw-rw-rw-   0        0        0     2088 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/gateron-black-ink/press_enter.mp3
+-rw-rw-rw-   0        0        0     2088 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/gateron-black-ink/press_key1.mp3
+-rw-rw-rw-   0        0        0     2088 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/gateron-black-ink/press_key2.mp3
+-rw-rw-rw-   0        0        0     2088 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/gateron-black-ink/press_key3.mp3
+-rw-rw-rw-   0        0        0     2088 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/gateron-black-ink/press_key4.mp3
+-rw-rw-rw-   0        0        0     2088 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/gateron-black-ink/press_key5.mp3
+-rw-rw-rw-   0        0        0     2088 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/gateron-black-ink/press_space.mp3
+-rw-rw-rw-   0        0        0     1040 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/gateron-black-ink/profile.yaml
+-rw-rw-rw-   0        0        0     2506 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/gateron-black-ink/release_back.mp3
+-rw-rw-rw-   0        0        0     2088 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/gateron-black-ink/release_enter.mp3
+-rw-rw-rw-   0        0        0     2088 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/gateron-black-ink/release_key.mp3
+-rw-rw-rw-   0        0        0     2088 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/gateron-black-ink/release_space.mp3
+drwxrwxrwx   0        0        0        0 2024-04-19 22:39:56.735386 keyboardsounds-5.7.5/keyboardsounds/profiles/gateron-red-ink/
+-rw-rw-rw-   0        0        0     1107 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/gateron-red-ink/LICENSE
+-rw-rw-rw-   0        0        0     2088 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/gateron-red-ink/press_back.mp3
+-rw-rw-rw-   0        0        0     2924 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/gateron-red-ink/press_enter.mp3
+-rw-rw-rw-   0        0        0     2506 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/gateron-red-ink/press_key1.mp3
+-rw-rw-rw-   0        0        0     2506 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/gateron-red-ink/press_key2.mp3
+-rw-rw-rw-   0        0        0     2506 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/gateron-red-ink/press_key3.mp3
+-rw-rw-rw-   0        0        0     2506 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/gateron-red-ink/press_key4.mp3
+-rw-rw-rw-   0        0        0     2506 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/gateron-red-ink/press_key5.mp3
+-rw-rw-rw-   0        0        0     2506 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/gateron-red-ink/press_space.mp3
+-rw-rw-rw-   0        0        0     1036 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/gateron-red-ink/profile.yaml
+-rw-rw-rw-   0        0        0     2088 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/gateron-red-ink/release_back.mp3
+-rw-rw-rw-   0        0        0     2088 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/gateron-red-ink/release_enter.mp3
+-rw-rw-rw-   0        0        0     2088 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/gateron-red-ink/release_key.mp3
+-rw-rw-rw-   0        0        0     2088 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/gateron-red-ink/release_space.mp3
+drwxrwxrwx   0        0        0        0 2024-04-19 22:39:56.745417 keyboardsounds-5.7.5/keyboardsounds/profiles/holy-panda/
+-rw-rw-rw-   0        0        0     1107 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/holy-panda/LICENSE
+-rw-rw-rw-   0        0        0     2088 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/holy-panda/press_back.mp3
+-rw-rw-rw-   0        0        0     2088 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/holy-panda/press_enter.mp3
+-rw-rw-rw-   0        0        0     2088 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/holy-panda/press_key1.mp3
+-rw-rw-rw-   0        0        0     2088 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/holy-panda/press_key2.mp3
+-rw-rw-rw-   0        0        0     2088 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/holy-panda/press_key3.mp3
+-rw-rw-rw-   0        0        0     2088 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/holy-panda/press_key4.mp3
+-rw-rw-rw-   0        0        0     2088 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/holy-panda/press_key5.mp3
+-rw-rw-rw-   0        0        0     5850 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/holy-panda/press_space.mp3
+-rw-rw-rw-   0        0        0     1026 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/holy-panda/profile.yaml
+-rw-rw-rw-   0        0        0     1670 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/holy-panda/release_back.mp3
+-rw-rw-rw-   0        0        0     1252 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/holy-panda/release_enter.mp3
+-rw-rw-rw-   0        0        0     2088 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/holy-panda/release_key.mp3
+-rw-rw-rw-   0        0        0     1252 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/holy-panda/release_space.mp3
+drwxrwxrwx   0        0        0        0 2024-04-19 22:39:56.747417 keyboardsounds-5.7.5/keyboardsounds/profiles/ios/
+-rw-rw-rw-   0        0        0   740450 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/ios/ios-video-recording.mp4
+-rw-rw-rw-   0        0        0      668 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/ios/profile.yaml
+drwxrwxrwx   0        0        0        0 2024-04-19 22:39:56.759982 keyboardsounds-5.7.5/keyboardsounds/profiles/mx-black/
+-rw-rw-rw-   0        0        0     1107 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/mx-black/LICENSE
+-rw-rw-rw-   0        0        0     2088 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/mx-black/press_back.mp3
+-rw-rw-rw-   0        0        0     2506 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/mx-black/press_enter.mp3
+-rw-rw-rw-   0        0        0     2088 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/mx-black/press_key1.mp3
+-rw-rw-rw-   0        0        0     2088 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/mx-black/press_key2.mp3
+-rw-rw-rw-   0        0        0     2088 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/mx-black/press_key3.mp3
+-rw-rw-rw-   0        0        0     2088 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/mx-black/press_key4.mp3
+-rw-rw-rw-   0        0        0     2088 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/mx-black/press_key5.mp3
+-rw-rw-rw-   0        0        0     2506 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/mx-black/press_space.mp3
+-rw-rw-rw-   0        0        0     1029 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/mx-black/profile.yaml
+-rw-rw-rw-   0        0        0     2088 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/mx-black/release_back.mp3
+-rw-rw-rw-   0        0        0     2088 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/mx-black/release_enter.mp3
+-rw-rw-rw-   0        0        0     1670 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/mx-black/release_key.mp3
+-rw-rw-rw-   0        0        0     2506 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/mx-black/release_space.mp3
+drwxrwxrwx   0        0        0        0 2024-04-19 22:39:56.767486 keyboardsounds-5.7.5/keyboardsounds/profiles/mx-blue/
+-rw-rw-rw-   0        0        0     1107 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/mx-blue/LICENSE
+-rw-rw-rw-   0        0        0     2088 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/mx-blue/press_key1.mp3
+-rw-rw-rw-   0        0        0     2088 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/mx-blue/press_key2.mp3
+-rw-rw-rw-   0        0        0     2088 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/mx-blue/press_key3.mp3
+-rw-rw-rw-   0        0        0     2088 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/mx-blue/press_key4.mp3
+-rw-rw-rw-   0        0        0     2088 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/mx-blue/press_key5.mp3
+-rw-rw-rw-   0        0        0      530 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/mx-blue/profile.yaml
+-rw-rw-rw-   0        0        0     1670 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/mx-blue/release.mp3
+drwxrwxrwx   0        0        0        0 2024-04-19 22:39:56.778540 keyboardsounds-5.7.5/keyboardsounds/profiles/mx-brown/
+-rw-rw-rw-   0        0        0     1107 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/mx-brown/LICENSE
+-rw-rw-rw-   0        0        0     2506 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/mx-brown/press_back.mp3
+-rw-rw-rw-   0        0        0     2506 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/mx-brown/press_enter.mp3
+-rw-rw-rw-   0        0        0     2506 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/mx-brown/press_key1.mp3
+-rw-rw-rw-   0        0        0     2506 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/mx-brown/press_key2.mp3
+-rw-rw-rw-   0        0        0     2506 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/mx-brown/press_key3.mp3
+-rw-rw-rw-   0        0        0     2506 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/mx-brown/press_key4.mp3
+-rw-rw-rw-   0        0        0     2506 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/mx-brown/press_key5.mp3
+-rw-rw-rw-   0        0        0     1670 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/mx-brown/press_space.mp3
+-rw-rw-rw-   0        0        0     1029 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/mx-brown/profile.yaml
+-rw-rw-rw-   0        0        0     2088 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/mx-brown/release_back.mp3
+-rw-rw-rw-   0        0        0     4596 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/mx-brown/release_enter.mp3
+-rw-rw-rw-   0        0        0     2088 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/mx-brown/release_key.mp3
+-rw-rw-rw-   0        0        0     1670 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/mx-brown/release_space.mp3
+drwxrwxrwx   0        0        0        0 2024-04-19 22:39:56.783539 keyboardsounds-5.7.5/keyboardsounds/profiles/mx-speed-silver/
+-rw-rw-rw-   0        0        0    28336 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/mx-speed-silver/mx-speed-silver-1.wav
+-rw-rw-rw-   0        0        0    34328 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/mx-speed-silver/mx-speed-silver-2.wav
+-rw-rw-rw-   0        0        0    31488 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/mx-speed-silver/mx-speed-silver-3.wav
+-rw-rw-rw-   0        0        0    31176 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/mx-speed-silver/mx-speed-silver-4.wav
+-rw-rw-rw-   0        0        0    32228 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/mx-speed-silver/mx-speed-silver-5.wav
+-rw-rw-rw-   0        0        0    32016 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/mx-speed-silver/mx-speed-silver-6.wav
+-rw-rw-rw-   0        0        0      514 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/mx-speed-silver/profile.yaml
+drwxrwxrwx   0        0        0        0 2024-04-19 22:39:56.795050 keyboardsounds-5.7.5/keyboardsounds/profiles/telios-v2/
+-rw-rw-rw-   0        0        0    28076 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/telios-v2/back.wav
+-rw-rw-rw-   0        0        0    31916 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/telios-v2/caps.wav
+-rw-rw-rw-   0        0        0    32812 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/telios-v2/ctrl.wav
+-rw-rw-rw-   0        0        0    22316 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/telios-v2/ent.wav
+-rw-rw-rw-   0        0        0    42540 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/telios-v2/key1.wav
+-rw-rw-rw-   0        0        0    26316 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/telios-v2/key2.wav
+-rw-rw-rw-   0        0        0    25516 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/telios-v2/key3.wav
+-rw-rw-rw-   0        0        0    25612 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/telios-v2/key4.wav
+-rw-rw-rw-   0        0        0    28300 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/telios-v2/key5.wav
+-rw-rw-rw-   0        0        0    26860 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/telios-v2/key6.wav
+-rw-rw-rw-   0        0        0      982 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/telios-v2/profile.yaml
+-rw-rw-rw-   0        0        0    23596 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/telios-v2/shift.wav
+-rw-rw-rw-   0        0        0    23212 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/telios-v2/space.wav
+-rw-rw-rw-   0        0        0    38060 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/telios-v2/tab.wav
+drwxrwxrwx   0        0        0        0 2024-04-19 22:39:56.799571 keyboardsounds-5.7.5/keyboardsounds/profiles/typewriter/
+-rw-rw-rw-   0        0        0    60204 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/typewriter/delete.wav
+-rw-rw-rw-   0        0        0   146204 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/typewriter/enter.wav
+-rw-rw-rw-   0        0        0    32664 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/typewriter/key.wav
+-rw-rw-rw-   0        0        0    31588 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/typewriter/key2.wav
+-rw-rw-rw-   0        0        0      610 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/typewriter/profile.yaml
+-rw-rw-rw-   0        0        0    35788 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/typewriter/space.wav
+-rw-rw-rw-   0        0        0       61 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/root.py
+drwxrwxrwx   0        0        0        0 2024-04-19 22:39:56.800571 keyboardsounds-5.7.5/keyboardsounds.egg-info/
+-rw-rw-rw-   0        0        0    13713 2024-04-19 22:39:56.000000 keyboardsounds-5.7.5/keyboardsounds.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     6760 2024-04-19 22:39:56.000000 keyboardsounds-5.7.5/keyboardsounds.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-19 22:39:56.000000 keyboardsounds-5.7.5/keyboardsounds.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       91 2024-04-19 22:39:56.000000 keyboardsounds-5.7.5/keyboardsounds.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       76 2024-04-19 22:39:56.000000 keyboardsounds-5.7.5/keyboardsounds.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-04-19 22:39:56.000000 keyboardsounds-5.7.5/keyboardsounds.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      727 2024-04-19 22:39:41.000000 keyboardsounds-5.7.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-19 22:39:56.802567 keyboardsounds-5.7.5/setup.cfg
+-rw-rw-rw-   0        0        0     1146 2024-04-19 22:39:41.000000 keyboardsounds-5.7.5/setup.py
```

### Comparing `keyboardsounds-5.7.4/LICENSE` & `keyboardsounds-5.7.5/LICENSE`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.4/PKG-INFO` & `keyboardsounds-5.7.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keyboardsounds
-Version: 5.7.4
+Version: 5.7.5
 Summary: Adds the ability to play sounds while typing on any system.
 Author: Nathan Fiscaletti
 Author-email: Nathan Fiscaletti <nate.fiscaletti@gmail.com>
 Project-URL: Homepage, https://github.com/nathan-fiscaletti/keyboardsounds
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -83,30 +83,31 @@
 
 usage: <keyboardsounds|kbs> <action> [params]
 
   manage daemon:
 
     <keyboardsounds|kbs> start [-v <volume>] [-p <profile>]
     <keyboardsounds|kbs> stop
-    <keyboardsounds|kbs> status
+    <keyboardsounds|kbs> status [-s]
 
   manage profiles:
 
     <keyboardsounds|kbs> <ap|add-profile> -z <zipfile>
     <keyboardsounds|kbs> <rp|remove-profile> -n <profile>
-    <keyboardsounds|kbs> <lp|list-profiles>
+    <keyboardsounds|kbs> <lp|list-profiles> [-s] [--remote]
+    <keyboardsounds|kbs> <dp|download-profile> -n <profile>
     <keyboardsounds|kbs> <bp|build-profile> -d <sound_dir> -o <zip_file>
 
   manage rules:
 
     <keyboardsounds|kbs> <ar|add-rule> -r <rule> -a <app>
     <keyboardsounds|kbs> <rr|remove-rule> -a <app>
-    <keyboardsounds|kbs> <lr|list-rules>
+    <keyboardsounds|kbs> <lr|list-rules> [-s]
     <keyboardsounds|kbs> <sr|set-global-rule> -r <rule>
-    <keyboardsounds|kbs> <gr|get-global-rule>
+    <keyboardsounds|kbs> <gr|get-global-rule> [-s]
 
   other:
 
     <keyboardsounds|kbs> [--version|-V]
 
 
 positional arguments:
@@ -114,16 +115,18 @@
 
 options:
   -h, --help            show this help message and exit
   -v volume, --volume volume
                         volume of the sound effects (0-100), default 100
   -p profile, --profile profile
                         sound profile to use, default 'ios'
+  -s, --short           consolidate output to a single line of json for scripting
   -n name, --name name  name of the profile remove
   -z file, --zip file   path to the zip file containing the profile to add
+  --remote              used with the list-profiles action to list remote profiles
   -V, --version         show program's version number and exit
   -d directory, --directory directory
                         path to the directory containing the sounds to use for the profile
   -o file, --output file
                         path to the zip file to create
   -a app, --app app     absolute path to the application to add the rule for
   -r rule, --rule rule  rule to apply. must be one of 'enable', 'disable', or 'exclusive'
@@ -206,30 +209,42 @@
 
 ```bash
 $ kbs get-global-rule
 ```
 
 ### Manage Profiles
 
-**Add a new profile to the application.**
+**List downloadable profiles.**
 
 ```bash
-$ kbs add-profile -z ./my-profile.zip
+$ kbs list-profiles --remote
 ```
 
-**Removes a profile from the application.**
+**Lists the currently installed profiles.**
 
 ```bash
-$ kbs remove-profile -n myprofile
+$ kbs list-profiles
 ```
 
-**Lists the currently loaded profiles.**
+**Download a profile.**
 
 ```bash
-$ kbs list-profiles
+$ kbs download-profile -n myprofile
+```
+
+**Add a new profile to the application.**
+
+```bash
+$ kbs add-profile -z ./my-profile.zip
+```
+
+**Removes a profile from the application.**
+
+```bash
+$ kbs remove-profile -n myprofile
 ```
 
 ## Custom Profiles
 
 This application supports custom profiles in which you can provide your own WAV or MP3 files to be used for the different keys pressed.
 
 ### Creating a Profile
@@ -239,14 +254,22 @@
 3. Follow the example format below to fill the file in.
 4. Combine the files into a ZIP file. The files must be at the root of the zip file.
 
 You can then load this profile into the application using the `add-profile` action.
 
 > Note: Alternately you can use the `build-profile` action for an environment with built in validation when creating a new profile.
 
+### Adding a profile to the official repository
+
+If you have created a profile that you think others would enjoy, you can submit it to the official repository. To do this, you will need to create a pull request.
+
+1. Fork the repository.
+2. Add your profile to the `profiles` directory.
+3. Create a pull request.
+
 ### Example Profile
 
 ```yaml
 # General information about your profile, this includes
 # name, author and description.
 #
 # You are only required to provide the "name" field.
```

### Comparing `keyboardsounds-5.7.4/README.md` & `keyboardsounds-5.7.5/keyboardsounds.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,26 @@
+Metadata-Version: 2.1
+Name: keyboardsounds
+Version: 5.7.5
+Summary: Adds the ability to play sounds while typing on any system.
+Author: Nathan Fiscaletti
+Author-email: Nathan Fiscaletti <nate.fiscaletti@gmail.com>
+Project-URL: Homepage, https://github.com/nathan-fiscaletti/keyboardsounds
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: pygame==2.5.2
+Requires-Dist: pynput==1.7.6
+Requires-Dist: psutil==5.9.4
+Requires-Dist: imageio-ffmpeg==0.4.6
+Requires-Dist: pyyaml==6.0
+
 # Keyboard Sounds
 
 [![Sponsor Me!](https://img.shields.io/badge/%F0%9F%92%B8-Sponsor%20Me!-blue)](https://github.com/sponsors/nathan-fiscaletti)
 [![PyPI version](https://badge.fury.io/py/keyboardsounds.svg)](https://badge.fury.io/py/keyboardsounds)
 [![GitHub license](https://img.shields.io/github/license/nathan-fiscaletti/keyboardsounds.svg)](https://github.com/nathan-fiscaletti/keyboardsounds/blob/master/LICENSE)
 [![Downloads](https://static.pepy.tech/badge/keyboardsounds)](https://pepy.tech/project/keyboardsounds)
 [![Downloads](https://static.pepy.tech/badge/keyboardsounds/month)](https://pepy.tech/project/keyboardsounds)
@@ -64,30 +83,31 @@
 
 usage: <keyboardsounds|kbs> <action> [params]
 
   manage daemon:
 
     <keyboardsounds|kbs> start [-v <volume>] [-p <profile>]
     <keyboardsounds|kbs> stop
-    <keyboardsounds|kbs> status
+    <keyboardsounds|kbs> status [-s]
 
   manage profiles:
 
     <keyboardsounds|kbs> <ap|add-profile> -z <zipfile>
     <keyboardsounds|kbs> <rp|remove-profile> -n <profile>
-    <keyboardsounds|kbs> <lp|list-profiles>
+    <keyboardsounds|kbs> <lp|list-profiles> [-s] [--remote]
+    <keyboardsounds|kbs> <dp|download-profile> -n <profile>
     <keyboardsounds|kbs> <bp|build-profile> -d <sound_dir> -o <zip_file>
 
   manage rules:
 
     <keyboardsounds|kbs> <ar|add-rule> -r <rule> -a <app>
     <keyboardsounds|kbs> <rr|remove-rule> -a <app>
-    <keyboardsounds|kbs> <lr|list-rules>
+    <keyboardsounds|kbs> <lr|list-rules> [-s]
     <keyboardsounds|kbs> <sr|set-global-rule> -r <rule>
-    <keyboardsounds|kbs> <gr|get-global-rule>
+    <keyboardsounds|kbs> <gr|get-global-rule> [-s]
 
   other:
 
     <keyboardsounds|kbs> [--version|-V]
 
 
 positional arguments:
@@ -95,16 +115,18 @@
 
 options:
   -h, --help            show this help message and exit
   -v volume, --volume volume
                         volume of the sound effects (0-100), default 100
   -p profile, --profile profile
                         sound profile to use, default 'ios'
+  -s, --short           consolidate output to a single line of json for scripting
   -n name, --name name  name of the profile remove
   -z file, --zip file   path to the zip file containing the profile to add
+  --remote              used with the list-profiles action to list remote profiles
   -V, --version         show program's version number and exit
   -d directory, --directory directory
                         path to the directory containing the sounds to use for the profile
   -o file, --output file
                         path to the zip file to create
   -a app, --app app     absolute path to the application to add the rule for
   -r rule, --rule rule  rule to apply. must be one of 'enable', 'disable', or 'exclusive'
@@ -187,30 +209,42 @@
 
 ```bash
 $ kbs get-global-rule
 ```
 
 ### Manage Profiles
 
-**Add a new profile to the application.**
+**List downloadable profiles.**
 
 ```bash
-$ kbs add-profile -z ./my-profile.zip
+$ kbs list-profiles --remote
 ```
 
-**Removes a profile from the application.**
+**Lists the currently installed profiles.**
 
 ```bash
-$ kbs remove-profile -n myprofile
+$ kbs list-profiles
 ```
 
-**Lists the currently loaded profiles.**
+**Download a profile.**
 
 ```bash
-$ kbs list-profiles
+$ kbs download-profile -n myprofile
+```
+
+**Add a new profile to the application.**
+
+```bash
+$ kbs add-profile -z ./my-profile.zip
+```
+
+**Removes a profile from the application.**
+
+```bash
+$ kbs remove-profile -n myprofile
 ```
 
 ## Custom Profiles
 
 This application supports custom profiles in which you can provide your own WAV or MP3 files to be used for the different keys pressed.
 
 ### Creating a Profile
@@ -220,14 +254,22 @@
 3. Follow the example format below to fill the file in.
 4. Combine the files into a ZIP file. The files must be at the root of the zip file.
 
 You can then load this profile into the application using the `add-profile` action.
 
 > Note: Alternately you can use the `build-profile` action for an environment with built in validation when creating a new profile.
 
+### Adding a profile to the official repository
+
+If you have created a profile that you think others would enjoy, you can submit it to the official repository. To do this, you will need to create a pull request.
+
+1. Fork the repository.
+2. Add your profile to the `profiles` directory.
+3. Create a pull request.
+
 ### Example Profile
 
 ```yaml
 # General information about your profile, this includes
 # name, author and description.
 #
 # You are only required to provide the "name" field.
```

### Comparing `keyboardsounds-5.7.4/keyboardsounds/app_detector.py` & `keyboardsounds-5.7.5/keyboardsounds/app_detector.py`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.4/keyboardsounds/app_rules.py` & `keyboardsounds-5.7.5/keyboardsounds/app_rules.py`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.4/keyboardsounds/audio_manager.py` & `keyboardsounds-5.7.5/keyboardsounds/audio_manager.py`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.4/keyboardsounds/daemon.py` & `keyboardsounds-5.7.5/keyboardsounds/daemon.py`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.4/keyboardsounds/daemon_manager.py` & `keyboardsounds-5.7.5/keyboardsounds/daemon_manager.py`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.4/keyboardsounds/external_api/__connection_handler.py` & `keyboardsounds-5.7.5/keyboardsounds/external_api/__connection_handler.py`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.4/keyboardsounds/external_api/__external_api.py` & `keyboardsounds-5.7.5/keyboardsounds/external_api/__external_api.py`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.4/keyboardsounds/main.py` & `keyboardsounds-5.7.5/keyboardsounds/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -61,15 +61,16 @@
             f"  manage daemon:{os.linesep * 2}"
             f"    %(prog)s start [-v <volume>] [-p <profile>]{os.linesep}"
             f"    %(prog)s stop{os.linesep}"
             f"    %(prog)s status [-s]{os.linesep * 2}"
             f"  manage profiles:{os.linesep * 2}"
             f"    %(prog)s <ap|add-profile> -z <zipfile>{os.linesep}"
             f"    %(prog)s <rp|remove-profile> -n <profile>{os.linesep}"
-            f"    %(prog)s <lp|list-profiles> [-s]{os.linesep}"
+            f"    %(prog)s <lp|list-profiles> [-s] [--remote]{os.linesep}"
+            f"    %(prog)s <dp|download-profile> -n <profile>{os.linesep}"
             f"    %(prog)s <bp|build-profile> -d <sound_dir> -o <zip_file>{os.linesep * 2}"
         )
         + win_messages
         + (f"  other:{os.linesep * 2}" f"    %(prog)s [--version|-V]{os.linesep}")
     )
 
     parser = argparse.ArgumentParser(
@@ -100,15 +101,15 @@
     )
 
     # Status Action
     parser.add_argument(
         "-s",
         "--short",
         action="store_true",
-        help="consolidate output to a single line for scripting",
+        help="consolidate output to a single line of json for scripting",
     )
 
     # Profiles
     parser.add_argument(
         "-n",
         "--name",
         type=str,
@@ -120,14 +121,19 @@
         "-z",
         "--zip",
         type=str,
         default=None,
         metavar="file",
         help="path to the zip file containing the profile to add",
     )
+    parser.add_argument(
+        "--remote",
+        action="store_true",
+        help="used with the list-profiles action to list remote profiles",
+    )
     parser.add_argument("-V", "--version", action="version", version=version_number)
 
     # Profile Builder
     parser.add_argument(
         "-d",
         "--directory",
         type=str,
@@ -194,59 +200,103 @@
     elif args.action == "remove-profile" or args.action == "rp":
         if args.name is None:
             print("Please specify a name for the profile to remove.")
             return
         Profile.remove_profile(args.name)
         return
     elif args.action == "list-profiles" or args.action == "lp":
-        profiles = [profile.metadata() for profile in Profile.list()]
+        if args.remote:
+            profiles = Profile.list_remote_profiles()
 
-        if args.short:
-            print(
-                json.dumps(
-                    [
-                        {
-                            "name": profile["name"],
-                            "author": profile["author"],
-                            "description": profile["description"],
-                        }
-                        for profile in profiles
-                    ]
+            if args.short:
+                print(json.dumps(profiles))
+                return
+            else:
+                print(f"{os.linesep} Fetching remote profiles...{os.linesep}")
+
+                names = [profile["name"] for profile in profiles]
+                names.append("Name")
+                authors = [profile["author"] for profile in profiles]
+                authors.append("Author")
+                name_len = len(max(names, key=len))
+                auth_len = len(max(authors, key=len))
+
+                print(f" Downloadable profiles{os.linesep}")
+                print(
+                    f" {'Name'.ljust(name_len)} | {'Author'.ljust(auth_len)} | Description"
                 )
-            )
-            return
+                print(f" {'-' * name_len} | {'-' * auth_len} | -----------")
+                for profile in profiles:
+                    print(
+                        f" {profile['name'].ljust(name_len)} | {profile['author'].ljust(auth_len)} | {profile['description']}"
+                    )
+                print(os.linesep)
+        else:
+            profiles = [profile.metadata() for profile in Profile.list()]
+
+            if args.short:
+                print(
+                    json.dumps(
+                        [
+                            {
+                                "name": profile["name"],
+                                "author": profile["author"],
+                                "description": profile["description"],
+                            }
+                            for profile in profiles
+                        ]
+                    )
+                )
+                return
 
-        names = [profile["name"] for profile in profiles]
-        names.append("Name")
-        authors = [profile["author"] for profile in profiles]
-        authors.append("Author")
-        name_len = len(max(names, key=len))
-        auth_len = len(max(authors, key=len))
-
-        print(f"{os.linesep} Available profiles{os.linesep}")
-        print(f" {'Name'.ljust(name_len)} | {'Author'.ljust(auth_len)} | Description")
-        print(f" {'-' * name_len} | {'-' * auth_len} | -----------")
-        for profile in profiles:
+            names = [profile["name"] for profile in profiles]
+            names.append("Name")
+            authors = [profile["author"] for profile in profiles]
+            authors.append("Author")
+            name_len = len(max(names, key=len))
+            auth_len = len(max(authors, key=len))
+
+            print(f"{os.linesep} Available profiles{os.linesep}")
             print(
-                f" {profile['name'].ljust(name_len)} | {profile['author'].ljust(auth_len)} | {profile['description']}"
+                f" {'Name'.ljust(name_len)} | {'Author'.ljust(auth_len)} | Description"
             )
-        print(os.linesep)
-        return
+            print(f" {'-' * name_len} | {'-' * auth_len} | -----------")
+            for profile in profiles:
+                print(
+                    f" {profile['name'].ljust(name_len)} | {profile['author'].ljust(auth_len)} | {profile['description']}"
+                )
+            print(os.linesep)
+            return
     elif args.action == "build-profile" or args.action == "bp":
         if args.directory is None:
             print(
                 "Please specify a directory containing the sounds to use for the profile."
             )
             return
         if args.output is None:
             print("Please specify a zip file to create.")
             return
 
         builder = CliProfileBuilder(args.directory, args.output)
         builder.start()
+    elif args.action == "download-profile" or args.action == "dp":
+        if args.name is None:
+            print("Please specify a name for the remote profile to download.")
+            return
+
+        existing = Profile.list()
+        for profile in existing:
+            if profile.metadata()["name"] == args.name:
+                print(f"Profile '{args.name}' already exists.")
+                return
+
+        try:
+            Profile.download_profile(args.name)
+        except Exception as e:
+            print(e)
 
     # Rules are only available on windows
     elif WIN32 and (args.action == "list-rules" or args.action == "lr"):
         rules = get_rules()
 
         if args.short:
             print(
```

### Comparing `keyboardsounds-5.7.4/keyboardsounds/profile_builder.py` & `keyboardsounds-5.7.5/keyboardsounds/profile_builder.py`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.4/keyboardsounds/profile_validation.py` & `keyboardsounds-5.7.5/keyboardsounds/profile_validation.py`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.4/keyboardsounds/profiles/alpaca/LICENSE` & `keyboardsounds-5.7.5/keyboardsounds/profiles/alpaca/LICENSE`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.4/keyboardsounds/profiles/alpaca/press_back.mp3` & `keyboardsounds-5.7.5/keyboardsounds/profiles/alpaca/press_back.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.4/keyboardsounds/profiles/alpaca/press_enter.mp3` & `keyboardsounds-5.7.5/keyboardsounds/profiles/alpaca/press_enter.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.4/keyboardsounds/profiles/alpaca/press_key1.mp3` & `keyboardsounds-5.7.5/keyboardsounds/profiles/alpaca/press_key1.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.4/keyboardsounds/profiles/alpaca/press_key2.mp3` & `keyboardsounds-5.7.5/keyboardsounds/profiles/alpaca/press_key2.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.4/keyboardsounds/profiles/alpaca/press_key3.mp3` & `keyboardsounds-5.7.5/keyboardsounds/profiles/alpaca/press_key3.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.4/keyboardsounds/profiles/alpaca/press_key4.mp3` & `keyboardsounds-5.7.5/keyboardsounds/profiles/alpaca/press_key4.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.4/keyboardsounds/profiles/alpaca/press_key5.mp3` & `keyboardsounds-5.7.5/keyboardsounds/profiles/alpaca/press_key5.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.4/keyboardsounds/profiles/alpaca/press_space.mp3` & `keyboardsounds-5.7.5/keyboardsounds/profiles/alpaca/press_space.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.4/keyboardsounds/profiles/alpaca/profile.yaml` & `keyboardsounds-5.7.5/keyboardsounds/profiles/alpaca/profile.yaml`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.4/keyboardsounds/profiles/alpaca/release_back.mp3` & `keyboardsounds-5.7.5/keyboardsounds/profiles/alpaca/release_back.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.4/keyboardsounds/profiles/alpaca/release_enter.mp3` & `keyboardsounds-5.7.5/keyboardsounds/profiles/alpaca/release_enter.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.4/keyboardsounds/profiles/alpaca/release_key.mp3` & `keyboardsounds-5.7.5/keyboardsounds/profiles/alpaca/release_key.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.4/keyboardsounds/profiles/alpaca/release_space.mp3` & `keyboardsounds-5.7.5/keyboardsounds/profiles/alpaca/release_space.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.4/keyboardsounds/profiles/gateron-black-ink/LICENSE` & `keyboardsounds-5.7.5/keyboardsounds/profiles/gateron-black-ink/LICENSE`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.4/keyboardsounds/profiles/gateron-black-ink/press_back.mp3` & `keyboardsounds-5.7.5/keyboardsounds/profiles/gateron-black-ink/press_back.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.4/keyboardsounds/profiles/gateron-black-ink/press_enter.mp3` & `keyboardsounds-5.7.5/keyboardsounds/profiles/gateron-black-ink/press_enter.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.4/keyboardsounds/profiles/gateron-black-ink/press_key1.mp3` & `keyboardsounds-5.7.5/keyboardsounds/profiles/gateron-black-ink/press_key1.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.4/keyboardsounds/profiles/gateron-black-ink/press_key2.mp3` & `keyboardsounds-5.7.5/keyboardsounds/profiles/gateron-black-ink/press_key2.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.4/keyboardsounds/profiles/gateron-black-ink/press_key3.mp3` & `keyboardsounds-5.7.5/keyboardsounds/profiles/gateron-black-ink/press_key3.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.4/keyboardsounds/profiles/gateron-black-ink/press_key4.mp3` & `keyboardsounds-5.7.5/keyboardsounds/profiles/gateron-black-ink/press_key4.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.4/keyboardsounds/profiles/gateron-black-ink/press_key5.mp3` & `keyboardsounds-5.7.5/keyboardsounds/profiles/gateron-black-ink/press_key5.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.4/keyboardsounds/profiles/gateron-black-ink/press_space.mp3` & `keyboardsounds-5.7.5/keyboardsounds/profiles/gateron-black-ink/press_space.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.4/keyboardsounds/profiles/gateron-black-ink/profile.yaml` & `keyboardsounds-5.7.5/keyboardsounds/profiles/gateron-black-ink/profile.yaml`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.4/keyboardsounds/profiles/gateron-black-ink/release_back.mp3` & `keyboardsounds-5.7.5/keyboardsounds/profiles/gateron-black-ink/release_back.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.4/keyboardsounds/profiles/gateron-black-ink/release_enter.mp3` & `keyboardsounds-5.7.5/keyboardsounds/profiles/gateron-black-ink/release_enter.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.4/keyboardsounds/profiles/gateron-black-ink/release_key.mp3` & `keyboardsounds-5.7.5/keyboardsounds/profiles/gateron-black-ink/release_key.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.4/keyboardsounds/profiles/gateron-black-ink/release_space.mp3` & `keyboardsounds-5.7.5/keyboardsounds/profiles/gateron-black-ink/release_space.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.4/keyboardsounds/profiles/gateron-red-ink/LICENSE` & `keyboardsounds-5.7.5/keyboardsounds/profiles/gateron-red-ink/LICENSE`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.4/keyboardsounds/profiles/gateron-red-ink/press_back.mp3` & `keyboardsounds-5.7.5/keyboardsounds/profiles/gateron-red-ink/press_back.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.4/keyboardsounds/profiles/gateron-red-ink/press_enter.mp3` & `keyboardsounds-5.7.5/keyboardsounds/profiles/gateron-red-ink/press_enter.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.4/keyboardsounds/profiles/gateron-red-ink/press_key1.mp3` & `keyboardsounds-5.7.5/keyboardsounds/profiles/gateron-red-ink/press_key1.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.4/keyboardsounds/profiles/gateron-red-ink/press_key2.mp3` & `keyboardsounds-5.7.5/keyboardsounds/profiles/gateron-red-ink/press_key2.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.4/keyboardsounds/profiles/gateron-red-ink/press_key3.mp3` & `keyboardsounds-5.7.5/keyboardsounds/profiles/gateron-red-ink/press_key3.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.4/keyboardsounds/profiles/gateron-red-ink/press_key4.mp3` & `keyboardsounds-5.7.5/keyboardsounds/profiles/gateron-red-ink/press_key4.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.4/keyboardsounds/profiles/gateron-red-ink/press_key5.mp3` & `keyboardsounds-5.7.5/keyboardsounds/profiles/gateron-red-ink/press_key5.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.4/keyboardsounds/profiles/gateron-red-ink/press_space.mp3` & `keyboardsounds-5.7.5/keyboardsounds/profiles/gateron-red-ink/press_space.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.4/keyboardsounds/profiles/gateron-red-ink/profile.yaml` & `keyboardsounds-5.7.5/keyboardsounds/profiles/gateron-red-ink/profile.yaml`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.4/keyboardsounds/profiles/gateron-red-ink/release_back.mp3` & `keyboardsounds-5.7.5/keyboardsounds/profiles/gateron-red-ink/release_back.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.4/keyboardsounds/profiles/gateron-red-ink/release_enter.mp3` & `keyboardsounds-5.7.5/keyboardsounds/profiles/gateron-red-ink/release_enter.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.4/keyboardsounds/profiles/gateron-red-ink/release_key.mp3` & `keyboardsounds-5.7.5/keyboardsounds/profiles/gateron-red-ink/release_key.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.4/keyboardsounds/profiles/gateron-red-ink/release_space.mp3` & `keyboardsounds-5.7.5/keyboardsounds/profiles/gateron-red-ink/release_space.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.4/keyboardsounds/profiles/holy-panda/LICENSE` & `keyboardsounds-5.7.5/keyboardsounds/profiles/holy-panda/LICENSE`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.4/keyboardsounds/profiles/holy-panda/press_back.mp3` & `keyboardsounds-5.7.5/keyboardsounds/profiles/holy-panda/press_back.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.4/keyboardsounds/profiles/holy-panda/press_enter.mp3` & `keyboardsounds-5.7.5/keyboardsounds/profiles/holy-panda/press_enter.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.4/keyboardsounds/profiles/holy-panda/press_key1.mp3` & `keyboardsounds-5.7.5/keyboardsounds/profiles/holy-panda/press_key1.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.4/keyboardsounds/profiles/holy-panda/press_key2.mp3` & `keyboardsounds-5.7.5/keyboardsounds/profiles/holy-panda/press_key2.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.4/keyboardsounds/profiles/holy-panda/press_key3.mp3` & `keyboardsounds-5.7.5/keyboardsounds/profiles/holy-panda/press_key3.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.4/keyboardsounds/profiles/holy-panda/press_key4.mp3` & `keyboardsounds-5.7.5/keyboardsounds/profiles/holy-panda/press_key4.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.4/keyboardsounds/profiles/holy-panda/press_key5.mp3` & `keyboardsounds-5.7.5/keyboardsounds/profiles/holy-panda/press_key5.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.4/keyboardsounds/profiles/holy-panda/press_space.mp3` & `keyboardsounds-5.7.5/keyboardsounds/profiles/holy-panda/press_space.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.4/keyboardsounds/profiles/holy-panda/profile.yaml` & `keyboardsounds-5.7.5/keyboardsounds/profiles/holy-panda/profile.yaml`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.4/keyboardsounds/profiles/holy-panda/release_back.mp3` & `keyboardsounds-5.7.5/keyboardsounds/profiles/holy-panda/release_back.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.4/keyboardsounds/profiles/holy-panda/release_enter.mp3` & `keyboardsounds-5.7.5/keyboardsounds/profiles/holy-panda/release_enter.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.4/keyboardsounds/profiles/holy-panda/release_key.mp3` & `keyboardsounds-5.7.5/keyboardsounds/profiles/holy-panda/release_key.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.4/keyboardsounds/profiles/holy-panda/release_space.mp3` & `keyboardsounds-5.7.5/keyboardsounds/profiles/holy-panda/release_space.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.4/keyboardsounds/profiles/ios/ios-video-recording.mp4` & `keyboardsounds-5.7.5/keyboardsounds/profiles/ios/ios-video-recording.mp4`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.4/keyboardsounds/profiles/ios/profile.yaml` & `keyboardsounds-5.7.5/keyboardsounds/profiles/ios/profile.yaml`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.4/keyboardsounds/profiles/mx-black/LICENSE` & `keyboardsounds-5.7.5/keyboardsounds/profiles/mx-black/LICENSE`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.4/keyboardsounds/profiles/mx-black/press_back.mp3` & `keyboardsounds-5.7.5/keyboardsounds/profiles/mx-black/press_back.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.4/keyboardsounds/profiles/mx-black/press_enter.mp3` & `keyboardsounds-5.7.5/keyboardsounds/profiles/mx-black/press_enter.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.4/keyboardsounds/profiles/mx-black/press_key1.mp3` & `keyboardsounds-5.7.5/keyboardsounds/profiles/mx-black/press_key1.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.4/keyboardsounds/profiles/mx-black/press_key2.mp3` & `keyboardsounds-5.7.5/keyboardsounds/profiles/mx-black/press_key2.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.4/keyboardsounds/profiles/mx-black/press_key3.mp3` & `keyboardsounds-5.7.5/keyboardsounds/profiles/mx-black/press_key3.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.4/keyboardsounds/profiles/mx-black/press_key4.mp3` & `keyboardsounds-5.7.5/keyboardsounds/profiles/mx-black/press_key4.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.4/keyboardsounds/profiles/mx-black/press_key5.mp3` & `keyboardsounds-5.7.5/keyboardsounds/profiles/mx-black/press_key5.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.4/keyboardsounds/profiles/mx-black/press_space.mp3` & `keyboardsounds-5.7.5/keyboardsounds/profiles/mx-black/press_space.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.4/keyboardsounds/profiles/mx-black/profile.yaml` & `keyboardsounds-5.7.5/keyboardsounds/profiles/mx-black/profile.yaml`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.4/keyboardsounds/profiles/mx-black/release_back.mp3` & `keyboardsounds-5.7.5/keyboardsounds/profiles/mx-black/release_back.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.4/keyboardsounds/profiles/mx-black/release_enter.mp3` & `keyboardsounds-5.7.5/keyboardsounds/profiles/mx-black/release_enter.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.4/keyboardsounds/profiles/mx-black/release_key.mp3` & `keyboardsounds-5.7.5/keyboardsounds/profiles/mx-black/release_key.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.4/keyboardsounds/profiles/mx-black/release_space.mp3` & `keyboardsounds-5.7.5/keyboardsounds/profiles/mx-black/release_space.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.4/keyboardsounds/profiles/mx-blue/LICENSE` & `keyboardsounds-5.7.5/keyboardsounds/profiles/mx-blue/LICENSE`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.4/keyboardsounds/profiles/mx-blue/press_key1.mp3` & `keyboardsounds-5.7.5/keyboardsounds/profiles/mx-blue/press_key1.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.4/keyboardsounds/profiles/mx-blue/press_key2.mp3` & `keyboardsounds-5.7.5/keyboardsounds/profiles/mx-blue/press_key2.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.4/keyboardsounds/profiles/mx-blue/press_key3.mp3` & `keyboardsounds-5.7.5/keyboardsounds/profiles/mx-blue/press_key3.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.4/keyboardsounds/profiles/mx-blue/press_key4.mp3` & `keyboardsounds-5.7.5/keyboardsounds/profiles/mx-blue/press_key4.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.4/keyboardsounds/profiles/mx-blue/press_key5.mp3` & `keyboardsounds-5.7.5/keyboardsounds/profiles/mx-blue/press_key5.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.4/keyboardsounds/profiles/mx-blue/profile.yaml` & `keyboardsounds-5.7.5/keyboardsounds/profiles/mx-blue/profile.yaml`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.4/keyboardsounds/profiles/mx-blue/release.mp3` & `keyboardsounds-5.7.5/keyboardsounds/profiles/mx-blue/release.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.4/keyboardsounds/profiles/mx-brown/LICENSE` & `keyboardsounds-5.7.5/keyboardsounds/profiles/mx-brown/LICENSE`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.4/keyboardsounds/profiles/mx-brown/press_back.mp3` & `keyboardsounds-5.7.5/keyboardsounds/profiles/mx-brown/press_back.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.4/keyboardsounds/profiles/mx-brown/press_enter.mp3` & `keyboardsounds-5.7.5/keyboardsounds/profiles/mx-brown/press_enter.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.4/keyboardsounds/profiles/mx-brown/press_key1.mp3` & `keyboardsounds-5.7.5/keyboardsounds/profiles/mx-brown/press_key1.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.4/keyboardsounds/profiles/mx-brown/press_key2.mp3` & `keyboardsounds-5.7.5/keyboardsounds/profiles/mx-brown/press_key2.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.4/keyboardsounds/profiles/mx-brown/press_key3.mp3` & `keyboardsounds-5.7.5/keyboardsounds/profiles/mx-brown/press_key3.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.4/keyboardsounds/profiles/mx-brown/press_key4.mp3` & `keyboardsounds-5.7.5/keyboardsounds/profiles/mx-brown/press_key4.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.4/keyboardsounds/profiles/mx-brown/press_key5.mp3` & `keyboardsounds-5.7.5/keyboardsounds/profiles/mx-brown/press_key5.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.4/keyboardsounds/profiles/mx-brown/press_space.mp3` & `keyboardsounds-5.7.5/keyboardsounds/profiles/mx-brown/press_space.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.4/keyboardsounds/profiles/mx-brown/profile.yaml` & `keyboardsounds-5.7.5/keyboardsounds/profiles/mx-brown/profile.yaml`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.4/keyboardsounds/profiles/mx-brown/release_back.mp3` & `keyboardsounds-5.7.5/keyboardsounds/profiles/mx-brown/release_back.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.4/keyboardsounds/profiles/mx-brown/release_enter.mp3` & `keyboardsounds-5.7.5/keyboardsounds/profiles/mx-brown/release_enter.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.4/keyboardsounds/profiles/mx-brown/release_key.mp3` & `keyboardsounds-5.7.5/keyboardsounds/profiles/mx-brown/release_key.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.4/keyboardsounds/profiles/mx-brown/release_space.mp3` & `keyboardsounds-5.7.5/keyboardsounds/profiles/mx-brown/release_space.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.4/keyboardsounds/profiles/mx-speed-silver/mx-speed-silver-1.wav` & `keyboardsounds-5.7.5/keyboardsounds/profiles/mx-speed-silver/mx-speed-silver-1.wav`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.4/keyboardsounds/profiles/mx-speed-silver/mx-speed-silver-2.wav` & `keyboardsounds-5.7.5/keyboardsounds/profiles/mx-speed-silver/mx-speed-silver-2.wav`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.4/keyboardsounds/profiles/mx-speed-silver/mx-speed-silver-3.wav` & `keyboardsounds-5.7.5/keyboardsounds/profiles/mx-speed-silver/mx-speed-silver-3.wav`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.4/keyboardsounds/profiles/mx-speed-silver/mx-speed-silver-4.wav` & `keyboardsounds-5.7.5/keyboardsounds/profiles/mx-speed-silver/mx-speed-silver-4.wav`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.4/keyboardsounds/profiles/mx-speed-silver/mx-speed-silver-5.wav` & `keyboardsounds-5.7.5/keyboardsounds/profiles/mx-speed-silver/mx-speed-silver-5.wav`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.4/keyboardsounds/profiles/mx-speed-silver/mx-speed-silver-6.wav` & `keyboardsounds-5.7.5/keyboardsounds/profiles/mx-speed-silver/mx-speed-silver-6.wav`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.4/keyboardsounds/profiles/mx-speed-silver/profile.yaml` & `keyboardsounds-5.7.5/keyboardsounds/profiles/mx-speed-silver/profile.yaml`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.4/keyboardsounds/profiles/telios-v2/back.wav` & `keyboardsounds-5.7.5/keyboardsounds/profiles/telios-v2/back.wav`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.4/keyboardsounds/profiles/telios-v2/caps.wav` & `keyboardsounds-5.7.5/keyboardsounds/profiles/telios-v2/caps.wav`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.4/keyboardsounds/profiles/telios-v2/ctrl.wav` & `keyboardsounds-5.7.5/keyboardsounds/profiles/telios-v2/ctrl.wav`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.4/keyboardsounds/profiles/telios-v2/ent.wav` & `keyboardsounds-5.7.5/keyboardsounds/profiles/telios-v2/ent.wav`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.4/keyboardsounds/profiles/telios-v2/key1.wav` & `keyboardsounds-5.7.5/keyboardsounds/profiles/telios-v2/key1.wav`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.4/keyboardsounds/profiles/telios-v2/key2.wav` & `keyboardsounds-5.7.5/keyboardsounds/profiles/telios-v2/key2.wav`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.4/keyboardsounds/profiles/telios-v2/key3.wav` & `keyboardsounds-5.7.5/keyboardsounds/profiles/telios-v2/key3.wav`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.4/keyboardsounds/profiles/telios-v2/key4.wav` & `keyboardsounds-5.7.5/keyboardsounds/profiles/telios-v2/key4.wav`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.4/keyboardsounds/profiles/telios-v2/key5.wav` & `keyboardsounds-5.7.5/keyboardsounds/profiles/telios-v2/key5.wav`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.4/keyboardsounds/profiles/telios-v2/key6.wav` & `keyboardsounds-5.7.5/keyboardsounds/profiles/telios-v2/key6.wav`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.4/keyboardsounds/profiles/telios-v2/profile.yaml` & `keyboardsounds-5.7.5/keyboardsounds/profiles/telios-v2/profile.yaml`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.4/keyboardsounds/profiles/telios-v2/shift.wav` & `keyboardsounds-5.7.5/keyboardsounds/profiles/telios-v2/shift.wav`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.4/keyboardsounds/profiles/telios-v2/space.wav` & `keyboardsounds-5.7.5/keyboardsounds/profiles/telios-v2/space.wav`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.4/keyboardsounds/profiles/telios-v2/tab.wav` & `keyboardsounds-5.7.5/keyboardsounds/profiles/telios-v2/tab.wav`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.4/keyboardsounds/profiles/typewriter/delete.wav` & `keyboardsounds-5.7.5/keyboardsounds/profiles/typewriter/delete.wav`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.4/keyboardsounds/profiles/typewriter/enter.wav` & `keyboardsounds-5.7.5/keyboardsounds/profiles/typewriter/enter.wav`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.4/keyboardsounds/profiles/typewriter/key.wav` & `keyboardsounds-5.7.5/keyboardsounds/profiles/typewriter/key.wav`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.4/keyboardsounds/profiles/typewriter/key2.wav` & `keyboardsounds-5.7.5/keyboardsounds/profiles/typewriter/key2.wav`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.4/keyboardsounds/profiles/typewriter/profile.yaml` & `keyboardsounds-5.7.5/keyboardsounds/profiles/typewriter/profile.yaml`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.4/keyboardsounds/profiles/typewriter/space.wav` & `keyboardsounds-5.7.5/keyboardsounds/profiles/typewriter/space.wav`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.4/keyboardsounds.egg-info/PKG-INFO` & `keyboardsounds-5.7.5/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,7 @@
-Metadata-Version: 2.1
-Name: keyboardsounds
-Version: 5.7.4
-Summary: Adds the ability to play sounds while typing on any system.
-Author: Nathan Fiscaletti
-Author-email: Nathan Fiscaletti <nate.fiscaletti@gmail.com>
-Project-URL: Homepage, https://github.com/nathan-fiscaletti/keyboardsounds
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: pygame==2.5.2
-Requires-Dist: pynput==1.7.6
-Requires-Dist: psutil==5.9.4
-Requires-Dist: imageio-ffmpeg==0.4.6
-Requires-Dist: pyyaml==6.0
-
 # Keyboard Sounds
 
 [![Sponsor Me!](https://img.shields.io/badge/%F0%9F%92%B8-Sponsor%20Me!-blue)](https://github.com/sponsors/nathan-fiscaletti)
 [![PyPI version](https://badge.fury.io/py/keyboardsounds.svg)](https://badge.fury.io/py/keyboardsounds)
 [![GitHub license](https://img.shields.io/github/license/nathan-fiscaletti/keyboardsounds.svg)](https://github.com/nathan-fiscaletti/keyboardsounds/blob/master/LICENSE)
 [![Downloads](https://static.pepy.tech/badge/keyboardsounds)](https://pepy.tech/project/keyboardsounds)
 [![Downloads](https://static.pepy.tech/badge/keyboardsounds/month)](https://pepy.tech/project/keyboardsounds)
@@ -83,30 +64,31 @@
 
 usage: <keyboardsounds|kbs> <action> [params]
 
   manage daemon:
 
     <keyboardsounds|kbs> start [-v <volume>] [-p <profile>]
     <keyboardsounds|kbs> stop
-    <keyboardsounds|kbs> status
+    <keyboardsounds|kbs> status [-s]
 
   manage profiles:
 
     <keyboardsounds|kbs> <ap|add-profile> -z <zipfile>
     <keyboardsounds|kbs> <rp|remove-profile> -n <profile>
-    <keyboardsounds|kbs> <lp|list-profiles>
+    <keyboardsounds|kbs> <lp|list-profiles> [-s] [--remote]
+    <keyboardsounds|kbs> <dp|download-profile> -n <profile>
     <keyboardsounds|kbs> <bp|build-profile> -d <sound_dir> -o <zip_file>
 
   manage rules:
 
     <keyboardsounds|kbs> <ar|add-rule> -r <rule> -a <app>
     <keyboardsounds|kbs> <rr|remove-rule> -a <app>
-    <keyboardsounds|kbs> <lr|list-rules>
+    <keyboardsounds|kbs> <lr|list-rules> [-s]
     <keyboardsounds|kbs> <sr|set-global-rule> -r <rule>
-    <keyboardsounds|kbs> <gr|get-global-rule>
+    <keyboardsounds|kbs> <gr|get-global-rule> [-s]
 
   other:
 
     <keyboardsounds|kbs> [--version|-V]
 
 
 positional arguments:
@@ -114,16 +96,18 @@
 
 options:
   -h, --help            show this help message and exit
   -v volume, --volume volume
                         volume of the sound effects (0-100), default 100
   -p profile, --profile profile
                         sound profile to use, default 'ios'
+  -s, --short           consolidate output to a single line of json for scripting
   -n name, --name name  name of the profile remove
   -z file, --zip file   path to the zip file containing the profile to add
+  --remote              used with the list-profiles action to list remote profiles
   -V, --version         show program's version number and exit
   -d directory, --directory directory
                         path to the directory containing the sounds to use for the profile
   -o file, --output file
                         path to the zip file to create
   -a app, --app app     absolute path to the application to add the rule for
   -r rule, --rule rule  rule to apply. must be one of 'enable', 'disable', or 'exclusive'
@@ -206,30 +190,42 @@
 
 ```bash
 $ kbs get-global-rule
 ```
 
 ### Manage Profiles
 
-**Add a new profile to the application.**
+**List downloadable profiles.**
 
 ```bash
-$ kbs add-profile -z ./my-profile.zip
+$ kbs list-profiles --remote
 ```
 
-**Removes a profile from the application.**
+**Lists the currently installed profiles.**
 
 ```bash
-$ kbs remove-profile -n myprofile
+$ kbs list-profiles
 ```
 
-**Lists the currently loaded profiles.**
+**Download a profile.**
 
 ```bash
-$ kbs list-profiles
+$ kbs download-profile -n myprofile
+```
+
+**Add a new profile to the application.**
+
+```bash
+$ kbs add-profile -z ./my-profile.zip
+```
+
+**Removes a profile from the application.**
+
+```bash
+$ kbs remove-profile -n myprofile
 ```
 
 ## Custom Profiles
 
 This application supports custom profiles in which you can provide your own WAV or MP3 files to be used for the different keys pressed.
 
 ### Creating a Profile
@@ -239,14 +235,22 @@
 3. Follow the example format below to fill the file in.
 4. Combine the files into a ZIP file. The files must be at the root of the zip file.
 
 You can then load this profile into the application using the `add-profile` action.
 
 > Note: Alternately you can use the `build-profile` action for an environment with built in validation when creating a new profile.
 
+### Adding a profile to the official repository
+
+If you have created a profile that you think others would enjoy, you can submit it to the official repository. To do this, you will need to create a pull request.
+
+1. Fork the repository.
+2. Add your profile to the `profiles` directory.
+3. Create a pull request.
+
 ### Example Profile
 
 ```yaml
 # General information about your profile, this includes
 # name, author and description.
 #
 # You are only required to provide the "name" field.
```

### Comparing `keyboardsounds-5.7.4/keyboardsounds.egg-info/SOURCES.txt` & `keyboardsounds-5.7.5/keyboardsounds.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.4/pyproject.toml` & `keyboardsounds-5.7.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "keyboardsounds"
-version = "5.7.4"
+version = "5.7.5"
 authors = [
   { name="Nathan Fiscaletti", email="nate.fiscaletti@gmail.com" },
 ]
 description = "Adds the ability to play sounds while typing on any system."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `keyboardsounds-5.7.4/setup.py` & `keyboardsounds-5.7.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from setuptools import setup
 
 setup(
     name="keyboardsounds",
-    version="5.7.4",
+    version="5.7.5",
     description="Adds the ability to play sounds while typing on any system.",
     author="Nathan Fiscaletti",
     author_email="nate.fiscaletti@gmail.com",
     packages=["keyboardsounds"],
     install_requires=[
         "pygame==2.5.2",
         "pynput==1.7.6",
         "psutil==5.9.4",
         "imageio-ffmpeg==0.4.6",
-        "pyyaml==6.0"
+        "pyyaml==6.0",
     ],
     package_data={
         "keyboardsounds": [
             "profiles/alpaca/*",
             "profiles/gateron-black-ink/*",
             "profiles/gateron-red-ink/*",
             "profiles/holy-panda/*",
```

