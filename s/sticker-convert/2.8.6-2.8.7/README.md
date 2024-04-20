# Comparing `tmp/sticker_convert-2.8.6.tar.gz` & `tmp/sticker_convert-2.8.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sticker_convert-2.8.6.tar", last modified: Thu Apr 18 14:31:42 2024, max compression
+gzip compressed data, was "sticker_convert-2.8.7.tar", last modified: Sat Apr 20 06:55:05 2024, max compression
```

## Comparing `sticker_convert-2.8.6.tar` & `sticker_convert-2.8.7.tar`

### file list

```diff
@@ -1,144 +1,144 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:31:42.120024 sticker_convert-2.8.6/
--rw-r--r--   0 runner    (1001) docker     (127)    18092 2024-04-18 14:31:35.000000 sticker_convert-2.8.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-18 14:31:35.000000 sticker_convert-2.8.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    49921 2024-04-18 14:31:42.120024 sticker_convert-2.8.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    27424 2024-04-18 14:31:35.000000 sticker_convert-2.8.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-04-18 14:31:35.000000 sticker_convert-2.8.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-18 14:31:35.000000 sticker_convert-2.8.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 14:31:42.120024 sticker_convert-2.8.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:31:42.096024 sticker_convert-2.8.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:31:42.100024 sticker_convert-2.8.6/src/sticker_convert/
--rwxr-xr-x   0 runner    (1001) docker     (127)      102 2024-04-18 14:31:35.000000 sticker_convert-2.8.6/src/sticker_convert/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      463 2024-04-18 14:31:35.000000 sticker_convert-2.8.6/src/sticker_convert/__main__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    18621 2024-04-18 14:31:35.000000 sticker_convert-2.8.6/src/sticker_convert/cli.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    37353 2024-04-18 14:31:35.000000 sticker_convert-2.8.6/src/sticker_convert/converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-04-18 14:31:35.000000 sticker_convert-2.8.6/src/sticker_convert/definitions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:31:42.100024 sticker_convert-2.8.6/src/sticker_convert/downloaders/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 14:31:35.000000 sticker_convert-2.8.6/src/sticker_convert/downloaders/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3980 2024-04-18 14:31:35.000000 sticker_convert-2.8.6/src/sticker_convert/downloaders/download_base.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8516 2024-04-18 14:31:35.000000 sticker_convert-2.8.6/src/sticker_convert/downloaders/download_kakao.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    17853 2024-04-18 14:31:35.000000 sticker_convert-2.8.6/src/sticker_convert/downloaders/download_line.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3063 2024-04-18 14:31:35.000000 sticker_convert-2.8.6/src/sticker_convert/downloaders/download_signal.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4614 2024-04-18 14:31:35.000000 sticker_convert-2.8.6/src/sticker_convert/downloaders/download_telegram.py
--rw-r--r--   0 runner    (1001) docker     (127)     3090 2024-04-18 14:31:35.000000 sticker_convert-2.8.6/src/sticker_convert/downloaders/download_viber.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    30707 2024-04-18 14:31:35.000000 sticker_convert-2.8.6/src/sticker_convert/gui.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:31:42.104024 sticker_convert-2.8.6/src/sticker_convert/gui_components/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 14:31:35.000000 sticker_convert-2.8.6/src/sticker_convert/gui_components/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:31:42.104024 sticker_convert-2.8.6/src/sticker_convert/gui_components/frames/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 14:31:35.000000 sticker_convert-2.8.6/src/sticker_convert/gui_components/frames/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7257 2024-04-18 14:31:35.000000 sticker_convert-2.8.6/src/sticker_convert/gui_components/frames/comp_frame.py
--rw-r--r--   0 runner    (1001) docker     (127)     4316 2024-04-18 14:31:35.000000 sticker_convert-2.8.6/src/sticker_convert/gui_components/frames/config_frame.py
--rw-r--r--   0 runner    (1001) docker     (127)      835 2024-04-18 14:31:35.000000 sticker_convert-2.8.6/src/sticker_convert/gui_components/frames/control_frame.py
--rw-r--r--   0 runner    (1001) docker     (127)     6499 2024-04-18 14:31:35.000000 sticker_convert-2.8.6/src/sticker_convert/gui_components/frames/cred_frame.py
--rw-r--r--   0 runner    (1001) docker     (127)     5040 2024-04-18 14:31:35.000000 sticker_convert-2.8.6/src/sticker_convert/gui_components/frames/input_frame.py
--rw-r--r--   0 runner    (1001) docker     (127)     4260 2024-04-18 14:31:35.000000 sticker_convert-2.8.6/src/sticker_convert/gui_components/frames/output_frame.py
--rw-r--r--   0 runner    (1001) docker     (127)     4915 2024-04-18 14:31:35.000000 sticker_convert-2.8.6/src/sticker_convert/gui_components/frames/progress_frame.py
--rw-r--r--   0 runner    (1001) docker     (127)      721 2024-04-18 14:31:35.000000 sticker_convert-2.8.6/src/sticker_convert/gui_components/frames/right_clicker.py
--rw-r--r--   0 runner    (1001) docker     (127)     3431 2024-04-18 14:31:35.000000 sticker_convert-2.8.6/src/sticker_convert/gui_components/gui_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:31:42.104024 sticker_convert-2.8.6/src/sticker_convert/gui_components/windows/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 14:31:35.000000 sticker_convert-2.8.6/src/sticker_convert/gui_components/windows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    31688 2024-04-18 14:31:35.000000 sticker_convert-2.8.6/src/sticker_convert/gui_components/windows/advanced_compression_window.py
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-18 14:31:35.000000 sticker_convert-2.8.6/src/sticker_convert/gui_components/windows/base_window.py
--rw-r--r--   0 runner    (1001) docker     (127)     7115 2024-04-18 14:31:35.000000 sticker_convert-2.8.6/src/sticker_convert/gui_components/windows/kakao_get_auth_window.py
--rw-r--r--   0 runner    (1001) docker     (127)     3375 2024-04-18 14:31:35.000000 sticker_convert-2.8.6/src/sticker_convert/gui_components/windows/line_get_auth_window.py
--rw-r--r--   0 runner    (1001) docker     (127)     4584 2024-04-18 14:31:35.000000 sticker_convert-2.8.6/src/sticker_convert/gui_components/windows/signal_get_auth_window.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:31:42.104024 sticker_convert-2.8.6/src/sticker_convert/ios-message-stickers-template/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:31:42.104024 sticker_convert-2.8.6/src/sticker_convert/ios-message-stickers-template/.github/
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-18 14:31:35.000000 sticker_convert-2.8.6/src/sticker_convert/ios-message-stickers-template/.github/FUNDING.yml
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-18 14:31:35.000000 sticker_convert-2.8.6/src/sticker_convert/ios-message-stickers-template/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-04-18 14:31:35.000000 sticker_convert-2.8.6/src/sticker_convert/ios-message-stickers-template/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:31:42.104024 sticker_convert-2.8.6/src/sticker_convert/ios-message-stickers-template/stickers/
--rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-04-18 14:31:35.000000 sticker_convert-2.8.6/src/sticker_convert/ios-message-stickers-template/stickers/Info.plist
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:31:42.104024 sticker_convert-2.8.6/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/
--rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-04-18 14:31:35.000000 sticker_convert-2.8.6/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Info.plist
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:31:42.104024 sticker_convert-2.8.6/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-18 14:31:35.000000 sticker_convert-2.8.6/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/Contents.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:31:42.104024 sticker_convert-2.8.6/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/Sticker Pack.stickerpack/
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-18 14:31:35.000000 sticker_convert-2.8.6/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/Sticker Pack.stickerpack/Contents.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:31:42.104024 sticker_convert-2.8.6/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/Sticker Pack.stickerpack/Sticker 1.sticker/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-18 14:31:35.000000 sticker_convert-2.8.6/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/Sticker Pack.stickerpack/Sticker 1.sticker/Contents.json
--rw-r--r--   0 runner    (1001) docker     (127)     7462 2024-04-18 14:31:35.000000 sticker_convert-2.8.6/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/Sticker Pack.stickerpack/Sticker 1.sticker/Sticker 1.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:31:42.104024 sticker_convert-2.8.6/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/Sticker Pack.stickerpack/Sticker 2.sticker/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-18 14:31:35.000000 sticker_convert-2.8.6/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/Sticker Pack.stickerpack/Sticker 2.sticker/Contents.json
--rw-r--r--   0 runner    (1001) docker     (127)     2521 2024-04-18 14:31:35.000000 sticker_convert-2.8.6/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/Sticker Pack.stickerpack/Sticker 2.sticker/Sticker 2.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:31:42.104024 sticker_convert-2.8.6/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/Sticker Pack.stickerpack/Sticker 3.sticker/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-18 14:31:35.000000 sticker_convert-2.8.6/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/Sticker Pack.stickerpack/Sticker 3.sticker/Contents.json
--rw-r--r--   0 runner    (1001) docker     (127)     7643 2024-04-18 14:31:35.000000 sticker_convert-2.8.6/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/Sticker Pack.stickerpack/Sticker 3.sticker/Sticker 3.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:31:42.108024 sticker_convert-2.8.6/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/
--rw-r--r--   0 runner    (1001) docker     (127)    11136 2024-04-18 14:31:35.000000 sticker_convert-2.8.6/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/App-Store-1024x1024pt.png
--rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-04-18 14:31:35.000000 sticker_convert-2.8.6/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Contents.json
--rw-r--r--   0 runner    (1001) docker     (127)     9504 2024-04-18 14:31:35.000000 sticker_convert-2.8.6/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages-App-Store-1024x768pt.png
--rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-04-18 14:31:35.000000 sticker_convert-2.8.6/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages-iPad-67x50pt@2x.png
--rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-04-18 14:31:35.000000 sticker_convert-2.8.6/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages-iPad-Pro-74x55pt@2x.png
--rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-04-18 14:31:35.000000 sticker_convert-2.8.6/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages-iPhone-60x45pt@2x.png
--rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-04-18 14:31:35.000000 sticker_convert-2.8.6/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages-iPhone-60x45pt@3x.png
--rw-r--r--   0 runner    (1001) docker     (127)      549 2024-04-18 14:31:35.000000 sticker_convert-2.8.6/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages27x20pt@2x.png
--rw-r--r--   0 runner    (1001) docker     (127)      763 2024-04-18 14:31:35.000000 sticker_convert-2.8.6/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages27x20pt@3x.png
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-18 14:31:35.000000 sticker_convert-2.8.6/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages32x24pt@2x.png
--rw-r--r--   0 runner    (1001) docker     (127)      858 2024-04-18 14:31:35.000000 sticker_convert-2.8.6/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages32x24pt@3x.png
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-18 14:31:35.000000 sticker_convert-2.8.6/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/iPad-Settings-29pt@2x.png
--rw-r--r--   0 runner    (1001) docker     (127)      863 2024-04-18 14:31:35.000000 sticker_convert-2.8.6/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/iPhone-Settings-29pt@3x.png
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-18 14:31:35.000000 sticker_convert-2.8.6/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/iPhone-settings-29pt@2x.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:31:42.108024 sticker_convert-2.8.6/src/sticker_convert/ios-message-stickers-template/stickers.xcodeproj/
--rw-r--r--   0 runner    (1001) docker     (127)    13282 2024-04-18 14:31:35.000000 sticker_convert-2.8.6/src/sticker_convert/ios-message-stickers-template/stickers.xcodeproj/project.pbxproj
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:31:42.108024 sticker_convert-2.8.6/src/sticker_convert/ios-message-stickers-template/stickers.xcodeproj/project.xcworkspace/
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-18 14:31:35.000000 sticker_convert-2.8.6/src/sticker_convert/ios-message-stickers-template/stickers.xcodeproj/project.xcworkspace/contents.xcworkspacedata
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:31:42.108024 sticker_convert-2.8.6/src/sticker_convert/ios-message-stickers-template/stickers.xcodeproj/project.xcworkspace/xcshareddata/
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-18 14:31:35.000000 sticker_convert-2.8.6/src/sticker_convert/ios-message-stickers-template/stickers.xcodeproj/project.xcworkspace/xcshareddata/IDEWorkspaceChecks.plist
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:31:42.096024 sticker_convert-2.8.6/src/sticker_convert/ios-message-stickers-template/stickers.xcodeproj/project.xcworkspace/xcuserdata/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:31:42.108024 sticker_convert-2.8.6/src/sticker_convert/ios-message-stickers-template/stickers.xcodeproj/project.xcworkspace/xcuserdata/niklaspeterson.xcuserdatad/
--rw-r--r--   0 runner    (1001) docker     (127)    21835 2024-04-18 14:31:35.000000 sticker_convert-2.8.6/src/sticker_convert/ios-message-stickers-template/stickers.xcodeproj/project.xcworkspace/xcuserdata/niklaspeterson.xcuserdatad/UserInterfaceState.xcuserstate
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:31:42.096024 sticker_convert-2.8.6/src/sticker_convert/ios-message-stickers-template/stickers.xcodeproj/xcuserdata/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:31:42.096024 sticker_convert-2.8.6/src/sticker_convert/ios-message-stickers-template/stickers.xcodeproj/xcuserdata/niklaspeterson.xcuserdatad/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:31:42.108024 sticker_convert-2.8.6/src/sticker_convert/ios-message-stickers-template/stickers.xcodeproj/xcuserdata/niklaspeterson.xcuserdatad/xcschemes/
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-18 14:31:35.000000 sticker_convert-2.8.6/src/sticker_convert/ios-message-stickers-template/stickers.xcodeproj/xcuserdata/niklaspeterson.xcuserdatad/xcschemes/xcschememanagement.plist
--rwxr-xr-x   0 runner    (1001) docker     (127)    25775 2024-04-18 14:31:35.000000 sticker_convert-2.8.6/src/sticker_convert/job.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7732 2024-04-18 14:31:35.000000 sticker_convert-2.8.6/src/sticker_convert/job_option.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:31:42.120024 sticker_convert-2.8.6/src/sticker_convert/resources/
--rwxr-xr-x   0 runner    (1001) docker     (127) 10353636 2024-04-18 14:31:36.000000 sticker_convert-2.8.6/src/sticker_convert/resources/NotoColorEmoji.ttf
--rwxr-xr-x   0 runner    (1001) docker     (127)     5404 2024-04-18 14:31:36.000000 sticker_convert-2.8.6/src/sticker_convert/resources/appicon.icns
--rwxr-xr-x   0 runner    (1001) docker     (127)    38078 2024-04-18 14:31:36.000000 sticker_convert-2.8.6/src/sticker_convert/resources/appicon.ico
--rwxr-xr-x   0 runner    (1001) docker     (127)     5265 2024-04-18 14:31:36.000000 sticker_convert-2.8.6/src/sticker_convert/resources/appicon.png
--rwxr-xr-x   0 runner    (1001) docker     (127)    12156 2024-04-18 14:31:36.000000 sticker_convert-2.8.6/src/sticker_convert/resources/compression.json
--rw-r--r--   0 runner    (1001) docker     (127)   413367 2024-04-18 14:31:36.000000 sticker_convert-2.8.6/src/sticker_convert/resources/emoji.json
--rw-r--r--   0 runner    (1001) docker     (127)     6541 2024-04-18 14:31:36.000000 sticker_convert-2.8.6/src/sticker_convert/resources/help.json
--rw-r--r--   0 runner    (1001) docker     (127)     2658 2024-04-18 14:31:36.000000 sticker_convert-2.8.6/src/sticker_convert/resources/input.json
--rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-04-18 14:31:36.000000 sticker_convert-2.8.6/src/sticker_convert/resources/output.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:31:42.120024 sticker_convert-2.8.6/src/sticker_convert/uploaders/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 14:31:36.000000 sticker_convert-2.8.6/src/sticker_convert/uploaders/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6021 2024-04-18 14:31:36.000000 sticker_convert-2.8.6/src/sticker_convert/uploaders/compress_wastickers.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1203 2024-04-18 14:31:36.000000 sticker_convert-2.8.6/src/sticker_convert/uploaders/upload_base.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6396 2024-04-18 14:31:36.000000 sticker_convert-2.8.6/src/sticker_convert/uploaders/upload_signal.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    15695 2024-04-18 14:31:36.000000 sticker_convert-2.8.6/src/sticker_convert/uploaders/upload_telegram.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    11254 2024-04-18 14:31:36.000000 sticker_convert-2.8.6/src/sticker_convert/uploaders/xcode_imessage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:31:42.120024 sticker_convert-2.8.6/src/sticker_convert/utils/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:31:42.120024 sticker_convert-2.8.6/src/sticker_convert/utils/auth/
--rwxr-xr-x   0 runner    (1001) docker     (127)     9829 2024-04-18 14:31:36.000000 sticker_convert-2.8.6/src/sticker_convert/utils/auth/get_kakao_auth.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2196 2024-04-18 14:31:36.000000 sticker_convert-2.8.6/src/sticker_convert/utils/auth/get_line_auth.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4925 2024-04-18 14:31:36.000000 sticker_convert-2.8.6/src/sticker_convert/utils/auth/get_signal_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     6061 2024-04-18 14:31:36.000000 sticker_convert-2.8.6/src/sticker_convert/utils/callback.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:31:42.120024 sticker_convert-2.8.6/src/sticker_convert/utils/files/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1047 2024-04-18 14:31:36.000000 sticker_convert-2.8.6/src/sticker_convert/utils/files/cache_store.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      541 2024-04-18 14:31:36.000000 sticker_convert-2.8.6/src/sticker_convert/utils/files/json_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-04-18 14:31:36.000000 sticker_convert-2.8.6/src/sticker_convert/utils/files/json_resources_loader.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    10088 2024-04-18 14:31:36.000000 sticker_convert-2.8.6/src/sticker_convert/utils/files/metadata_handler.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1743 2024-04-18 14:31:36.000000 sticker_convert-2.8.6/src/sticker_convert/utils/files/run_bin.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2156 2024-04-18 14:31:36.000000 sticker_convert-2.8.6/src/sticker_convert/utils/files/sanitize_filename.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:31:42.120024 sticker_convert-2.8.6/src/sticker_convert/utils/media/
--rwxr-xr-x   0 runner    (1001) docker     (127)     3657 2024-04-18 14:31:36.000000 sticker_convert-2.8.6/src/sticker_convert/utils/media/apple_png_normalize.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    15562 2024-04-18 14:31:36.000000 sticker_convert-2.8.6/src/sticker_convert/utils/media/codec_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     1947 2024-04-18 14:31:36.000000 sticker_convert-2.8.6/src/sticker_convert/utils/media/decrypt_kakao.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5732 2024-04-18 14:31:36.000000 sticker_convert-2.8.6/src/sticker_convert/utils/media/format_verify.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      840 2024-04-18 14:31:36.000000 sticker_convert-2.8.6/src/sticker_convert/utils/url_detect.py
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-18 14:31:36.000000 sticker_convert-2.8.6/src/sticker_convert/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:31:42.120024 sticker_convert-2.8.6/src/sticker_convert.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    49921 2024-04-18 14:31:42.000000 sticker_convert-2.8.6/src/sticker_convert.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7834 2024-04-18 14:31:42.000000 sticker_convert-2.8.6/src/sticker_convert.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 14:31:42.000000 sticker_convert-2.8.6/src/sticker_convert.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-18 14:31:42.000000 sticker_convert-2.8.6/src/sticker_convert.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-18 14:31:42.000000 sticker_convert-2.8.6/src/sticker_convert.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-18 14:31:42.000000 sticker_convert-2.8.6/src/sticker_convert.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:31:42.120024 sticker_convert-2.8.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2782 2024-04-18 14:31:36.000000 sticker_convert-2.8.6/tests/test_compression.py
--rw-r--r--   0 runner    (1001) docker     (127)    14721 2024-04-18 14:31:36.000000 sticker_convert-2.8.6/tests/test_download.py
--rw-r--r--   0 runner    (1001) docker     (127)     6148 2024-04-18 14:31:36.000000 sticker_convert-2.8.6/tests/test_export.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 06:55:05.780997 sticker_convert-2.8.7/
+-rw-r--r--   0 runner    (1001) docker     (127)    18092 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    50061 2024-04-20 06:55:05.780997 sticker_convert-2.8.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    27559 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2080 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 06:55:05.780997 sticker_convert-2.8.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 06:55:05.748997 sticker_convert-2.8.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 06:55:05.752997 sticker_convert-2.8.7/src/sticker_convert/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      102 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      463 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/__main__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    18621 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/cli.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    37357 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/definitions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 06:55:05.752997 sticker_convert-2.8.7/src/sticker_convert/downloaders/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/downloaders/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3980 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/downloaders/download_base.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8516 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/downloaders/download_kakao.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    17853 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/downloaders/download_line.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3063 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/downloaders/download_signal.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4614 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/downloaders/download_telegram.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3090 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/downloaders/download_viber.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    30707 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/gui.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 06:55:05.752997 sticker_convert-2.8.7/src/sticker_convert/gui_components/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/gui_components/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 06:55:05.756997 sticker_convert-2.8.7/src/sticker_convert/gui_components/frames/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/gui_components/frames/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7257 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/gui_components/frames/comp_frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4316 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/gui_components/frames/config_frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/gui_components/frames/control_frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6499 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/gui_components/frames/cred_frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5040 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/gui_components/frames/input_frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4260 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/gui_components/frames/output_frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4915 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/gui_components/frames/progress_frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/gui_components/frames/right_clicker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3431 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/gui_components/gui_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 06:55:05.756997 sticker_convert-2.8.7/src/sticker_convert/gui_components/windows/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/gui_components/windows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31964 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/gui_components/windows/advanced_compression_window.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/gui_components/windows/base_window.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7115 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/gui_components/windows/kakao_get_auth_window.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3375 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/gui_components/windows/line_get_auth_window.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4584 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/gui_components/windows/signal_get_auth_window.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 06:55:05.756997 sticker_convert-2.8.7/src/sticker_convert/ios-message-stickers-template/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 06:55:05.756997 sticker_convert-2.8.7/src/sticker_convert/ios-message-stickers-template/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/ios-message-stickers-template/.github/FUNDING.yml
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/ios-message-stickers-template/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/ios-message-stickers-template/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 06:55:05.756997 sticker_convert-2.8.7/src/sticker_convert/ios-message-stickers-template/stickers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/ios-message-stickers-template/stickers/Info.plist
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 06:55:05.756997 sticker_convert-2.8.7/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Info.plist
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 06:55:05.756997 sticker_convert-2.8.7/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/Contents.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 06:55:05.756997 sticker_convert-2.8.7/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/Sticker Pack.stickerpack/
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/Sticker Pack.stickerpack/Contents.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 06:55:05.756997 sticker_convert-2.8.7/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/Sticker Pack.stickerpack/Sticker 1.sticker/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/Sticker Pack.stickerpack/Sticker 1.sticker/Contents.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7462 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/Sticker Pack.stickerpack/Sticker 1.sticker/Sticker 1.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 06:55:05.756997 sticker_convert-2.8.7/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/Sticker Pack.stickerpack/Sticker 2.sticker/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/Sticker Pack.stickerpack/Sticker 2.sticker/Contents.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2521 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/Sticker Pack.stickerpack/Sticker 2.sticker/Sticker 2.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 06:55:05.756997 sticker_convert-2.8.7/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/Sticker Pack.stickerpack/Sticker 3.sticker/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/Sticker Pack.stickerpack/Sticker 3.sticker/Contents.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7643 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/Sticker Pack.stickerpack/Sticker 3.sticker/Sticker 3.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 06:55:05.760997 sticker_convert-2.8.7/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/
+-rw-r--r--   0 runner    (1001) docker     (127)    11136 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/App-Store-1024x1024pt.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Contents.json
+-rw-r--r--   0 runner    (1001) docker     (127)     9504 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages-App-Store-1024x768pt.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages-iPad-67x50pt@2x.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages-iPad-Pro-74x55pt@2x.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages-iPhone-60x45pt@2x.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages-iPhone-60x45pt@3x.png
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages27x20pt@2x.png
+-rw-r--r--   0 runner    (1001) docker     (127)      763 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages27x20pt@3x.png
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages32x24pt@2x.png
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages32x24pt@3x.png
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/iPad-Settings-29pt@2x.png
+-rw-r--r--   0 runner    (1001) docker     (127)      863 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/iPhone-Settings-29pt@3x.png
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/iPhone-settings-29pt@2x.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 06:55:05.760997 sticker_convert-2.8.7/src/sticker_convert/ios-message-stickers-template/stickers.xcodeproj/
+-rw-r--r--   0 runner    (1001) docker     (127)    13282 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/ios-message-stickers-template/stickers.xcodeproj/project.pbxproj
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 06:55:05.760997 sticker_convert-2.8.7/src/sticker_convert/ios-message-stickers-template/stickers.xcodeproj/project.xcworkspace/
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/ios-message-stickers-template/stickers.xcodeproj/project.xcworkspace/contents.xcworkspacedata
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 06:55:05.760997 sticker_convert-2.8.7/src/sticker_convert/ios-message-stickers-template/stickers.xcodeproj/project.xcworkspace/xcshareddata/
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/ios-message-stickers-template/stickers.xcodeproj/project.xcworkspace/xcshareddata/IDEWorkspaceChecks.plist
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 06:55:05.748997 sticker_convert-2.8.7/src/sticker_convert/ios-message-stickers-template/stickers.xcodeproj/project.xcworkspace/xcuserdata/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 06:55:05.760997 sticker_convert-2.8.7/src/sticker_convert/ios-message-stickers-template/stickers.xcodeproj/project.xcworkspace/xcuserdata/niklaspeterson.xcuserdatad/
+-rw-r--r--   0 runner    (1001) docker     (127)    21835 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/ios-message-stickers-template/stickers.xcodeproj/project.xcworkspace/xcuserdata/niklaspeterson.xcuserdatad/UserInterfaceState.xcuserstate
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 06:55:05.748997 sticker_convert-2.8.7/src/sticker_convert/ios-message-stickers-template/stickers.xcodeproj/xcuserdata/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 06:55:05.748997 sticker_convert-2.8.7/src/sticker_convert/ios-message-stickers-template/stickers.xcodeproj/xcuserdata/niklaspeterson.xcuserdatad/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 06:55:05.760997 sticker_convert-2.8.7/src/sticker_convert/ios-message-stickers-template/stickers.xcodeproj/xcuserdata/niklaspeterson.xcuserdatad/xcschemes/
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/ios-message-stickers-template/stickers.xcodeproj/xcuserdata/niklaspeterson.xcuserdatad/xcschemes/xcschememanagement.plist
+-rwxr-xr-x   0 runner    (1001) docker     (127)    25775 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/job.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7732 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/job_option.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 06:55:05.776997 sticker_convert-2.8.7/src/sticker_convert/resources/
+-rwxr-xr-x   0 runner    (1001) docker     (127) 10353636 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/resources/NotoColorEmoji.ttf
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5404 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/resources/appicon.icns
+-rwxr-xr-x   0 runner    (1001) docker     (127)    38078 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/resources/appicon.ico
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5265 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/resources/appicon.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12156 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/resources/compression.json
+-rw-r--r--   0 runner    (1001) docker     (127)   413367 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/resources/emoji.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6575 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/resources/help.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2665 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/resources/input.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/resources/output.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 06:55:05.776997 sticker_convert-2.8.7/src/sticker_convert/uploaders/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/uploaders/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6021 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/uploaders/compress_wastickers.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1203 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/uploaders/upload_base.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6396 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/uploaders/upload_signal.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    15695 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/uploaders/upload_telegram.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    11254 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/uploaders/xcode_imessage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 06:55:05.776997 sticker_convert-2.8.7/src/sticker_convert/utils/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 06:55:05.776997 sticker_convert-2.8.7/src/sticker_convert/utils/auth/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9829 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/utils/auth/get_kakao_auth.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2196 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/utils/auth/get_line_auth.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4925 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/utils/auth/get_signal_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6061 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/utils/callback.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 06:55:05.776997 sticker_convert-2.8.7/src/sticker_convert/utils/files/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1047 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/utils/files/cache_store.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      541 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/utils/files/json_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/utils/files/json_resources_loader.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10100 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/utils/files/metadata_handler.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1743 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/utils/files/run_bin.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2156 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/utils/files/sanitize_filename.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 06:55:05.776997 sticker_convert-2.8.7/src/sticker_convert/utils/media/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3657 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/utils/media/apple_png_normalize.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    15562 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/utils/media/codec_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1947 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/utils/media/decrypt_kakao.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5732 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/utils/media/format_verify.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      840 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/utils/url_detect.py
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/src/sticker_convert/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 06:55:05.780997 sticker_convert-2.8.7/src/sticker_convert.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    50061 2024-04-20 06:55:05.000000 sticker_convert-2.8.7/src/sticker_convert.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7834 2024-04-20 06:55:05.000000 sticker_convert-2.8.7/src/sticker_convert.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 06:55:05.000000 sticker_convert-2.8.7/src/sticker_convert.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-20 06:55:05.000000 sticker_convert-2.8.7/src/sticker_convert.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-20 06:55:05.000000 sticker_convert-2.8.7/src/sticker_convert.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-20 06:55:05.000000 sticker_convert-2.8.7/src/sticker_convert.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 06:55:05.780997 sticker_convert-2.8.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2782 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/tests/test_compression.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14721 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/tests/test_download.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6148 2024-04-20 06:55:00.000000 sticker_convert-2.8.7/tests/test_export.py
```

### Comparing `sticker_convert-2.8.6/LICENSE` & `sticker_convert-2.8.7/LICENSE`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.6/PKG-INFO` & `sticker_convert-2.8.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: sticker-convert
-Version: 2.8.6
-Summary: Convert (animated) stickers to/from WhatsApp, Telegram, Signal, Line, Kakao, iMessage. Written in Python.
+Version: 2.8.7
+Summary: Convert (animated) stickers to/from WhatsApp, Telegram, Signal, Line, Kakao, Viber, iMessage. Written in Python.
 Author-email: laggykiller <chaudominic2@gmail.com>
 Maintainer-email: laggykiller <chaudominic2@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 2, June 1991
         
          Copyright (C) 1989, 1991 Free Software Foundation, Inc.,
          51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA
@@ -582,16 +582,16 @@
                         Between -1 and positive infinity. Power lower = More importance of the parameter, try harder to keep higher and not sacrifice.
   --duration-min DURATION_MIN
                         Set minimum output duration in miliseconds.
   --duration-max DURATION_MAX
                         Set maximum output duration in miliseconds.
   --padding-percent PADDING_PERCENT
                         Set percentage of space used as padding.
-  --bg-color BG_COLOR   Set custom background color.
-                        Example: 00ff00 for green.
+  --bg-color BG_COLOR   Set custom background color in rrggbbaa format.
+                        Example: 00ff00 for green with alpha 0.
                         If this is not set, background color would be auto set to black if image is bright, or white if image is dark.
                         Note: The color should not be visible if output format supports transparency.
   --vid-size-max VID_SIZE_MAX
                         Set maximum file size limit for animated stickers.
   --img-size-max IMG_SIZE_MAX
                         Set maximum file size limit for static stickers.
   --vid-format VID_FORMAT
@@ -764,14 +764,15 @@
 
 ### Platform-specific guides (e.g. Getting credentials)
 - [Signal](docs/guide_signal.md)
 - [Telegram](docs/guide_telegram.md)
 - [WhatsApp](docs/guide_whatsapp.md)
 - [Line](docs/guide_line.md)
 - [Kakao](docs/guide_kakao.md)
+- [Viber](docs/guide_viber.md)
 - [iMessage](docs/guide_imessage.md)
 
 ### Conversion is slow
 Try the following tips:
 - Increase number of processes (`--processes`)
     - Increasing over default value can actually be slower though
 - Decrease number of steps (`--steps`)
@@ -821,11 +822,12 @@
 ## Credits
 - Information about Signal and Telegram stickers: https://github.com/teynav/signalApngSticker
 - Information about Line and Kakao stickers: https://github.com/star-39/moe-sticker-bot
 - Information about Line stickers: https://github.com/doubleplusc/Line-sticker-downloader
 - Information about Kakao animated stickers: https://gist.github.com/chitacan/9802668
 - Downloading and decrypting Kakao animated stickers: https://github.com/blluv/KakaoTalkEmoticonDownloader
 - Application icon taken from [Icons8](https://icons8.com/)
+- Banner generated from [GitHub Socialify](https://socialify.git.ci/)
 
 ## DISCLAIMER
 - The author of this repo is NOT affiliated with Signal, Telegram, WhatsApp, Line, Kakao or Sticker Maker.
 - The author of this repo is NOT repsonsible for any legal consequences and loss incurred from using this repo.
```

### Comparing `sticker_convert-2.8.6/README.md` & `sticker_convert-2.8.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -195,16 +195,16 @@
                         Between -1 and positive infinity. Power lower = More importance of the parameter, try harder to keep higher and not sacrifice.
   --duration-min DURATION_MIN
                         Set minimum output duration in miliseconds.
   --duration-max DURATION_MAX
                         Set maximum output duration in miliseconds.
   --padding-percent PADDING_PERCENT
                         Set percentage of space used as padding.
-  --bg-color BG_COLOR   Set custom background color.
-                        Example: 00ff00 for green.
+  --bg-color BG_COLOR   Set custom background color in rrggbbaa format.
+                        Example: 00ff00 for green with alpha 0.
                         If this is not set, background color would be auto set to black if image is bright, or white if image is dark.
                         Note: The color should not be visible if output format supports transparency.
   --vid-size-max VID_SIZE_MAX
                         Set maximum file size limit for animated stickers.
   --img-size-max IMG_SIZE_MAX
                         Set maximum file size limit for static stickers.
   --vid-format VID_FORMAT
@@ -377,14 +377,15 @@
 
 ### Platform-specific guides (e.g. Getting credentials)
 - [Signal](docs/guide_signal.md)
 - [Telegram](docs/guide_telegram.md)
 - [WhatsApp](docs/guide_whatsapp.md)
 - [Line](docs/guide_line.md)
 - [Kakao](docs/guide_kakao.md)
+- [Viber](docs/guide_viber.md)
 - [iMessage](docs/guide_imessage.md)
 
 ### Conversion is slow
 Try the following tips:
 - Increase number of processes (`--processes`)
     - Increasing over default value can actually be slower though
 - Decrease number of steps (`--steps`)
@@ -434,11 +435,12 @@
 ## Credits
 - Information about Signal and Telegram stickers: https://github.com/teynav/signalApngSticker
 - Information about Line and Kakao stickers: https://github.com/star-39/moe-sticker-bot
 - Information about Line stickers: https://github.com/doubleplusc/Line-sticker-downloader
 - Information about Kakao animated stickers: https://gist.github.com/chitacan/9802668
 - Downloading and decrypting Kakao animated stickers: https://github.com/blluv/KakaoTalkEmoticonDownloader
 - Application icon taken from [Icons8](https://icons8.com/)
+- Banner generated from [GitHub Socialify](https://socialify.git.ci/)
 
 ## DISCLAIMER
 - The author of this repo is NOT affiliated with Signal, Telegram, WhatsApp, Line, Kakao or Sticker Maker.
 - The author of this repo is NOT repsonsible for any legal consequences and loss incurred from using this repo.
```

### Comparing `sticker_convert-2.8.6/pyproject.toml` & `sticker_convert-2.8.7/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "sticker-convert"
-description = "Convert (animated) stickers to/from WhatsApp, Telegram, Signal, Line, Kakao, iMessage. Written in Python."
+description = "Convert (animated) stickers to/from WhatsApp, Telegram, Signal, Line, Kakao, Viber, iMessage. Written in Python."
 readme = "README.md"
 requires-python = ">=3.8"
 license = {file = "LICENSE"}
 keywords = ["telegram", "line", "tgs", "whatsapp", "kakao", "signal", "imessage", "wastickers", "viber"]
 authors = [
   {name = "laggykiller", email = "chaudominic2@gmail.com" } # Optional
 ]
```

### Comparing `sticker_convert-2.8.6/src/sticker_convert/cli.py` & `sticker_convert-2.8.7/src/sticker_convert/cli.py`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.6/src/sticker_convert/converter.py` & `sticker_convert-2.8.7/src/sticker_convert/converter.py`

 * *Files 0% similar despite different names*

```diff
@@ -182,16 +182,16 @@
         self.res_h: Optional[int] = None
         self.quality: Optional[int] = None
         self.fps: Optional[Fraction] = None
         self.color: Optional[int] = None
 
         self.bg_color: Optional[Tuple[int, int, int, int]] = None
         if self.opt_comp.bg_color:
-            r, g, b = bytes.fromhex(self.opt_comp.bg_color)
-            self.bg_color = (r, g, b, 0)
+            r, g, b, a = bytes.fromhex(self.opt_comp.bg_color)
+            self.bg_color = (r, g, b, a)
 
         self.tmp_f: BytesIO = BytesIO()
         self.result: Optional[bytes] = None
         self.result_size: int = 0
         self.result_step: Optional[int] = None
 
         self.apngasm = None
@@ -224,15 +224,15 @@
         step_upper = self.opt_comp.steps
 
         if self.codec_info_orig.is_animated is True:
             self.size_max = self.opt_comp.size_max_vid
         else:
             self.size_max = self.opt_comp.size_max_img
 
-        if self.size_max is None:
+        if self.size_max in (None, 0):
             # No limit to size, create the best quality result
             step_current = 0
         else:
             step_current = int(rounding((step_lower + step_upper) / 2))
 
         self.frames_import()
         while True:
@@ -800,14 +800,15 @@
         else:
             extra_kwargs["optimize"] = True
 
         if self.out_f.suffix == ".gif":
             # GIF can only have one alpha color
             # Change lowest alpha to alpha=0
             # Only keep alpha=0 and alpha=255, nothing in between
+            extra_kwargs["format"] = "GIF"
             frames_processed = np.array(self.frames_processed)
             alpha = frames_processed[:, :, :, 3]
             alpha_min = np.min(alpha)  # type: ignore
             if alpha_min < 255:
                 alpha[alpha > alpha_min] = 255
                 alpha[alpha == alpha_min] = 0
 
@@ -816,15 +817,14 @@
                 extra_kwargs["disposal"] = 2
                 im_out = [self.quantize(Image.fromarray(i)) for i in frames_processed]  # type: ignore
             else:
                 im_out = [
                     self.quantize(Image.fromarray(i).convert("RGB")).convert("RGB")  # type: ignore
                     for i in frames_processed
                 ]
-                extra_kwargs["format"] = "GIF"
         elif self.out_f.suffix == ".webp":
             im_out = [Image.fromarray(i) for i in self.frames_processed]  # type: ignore
             extra_kwargs["format"] = "WebP"
             extra_kwargs["minimize_size"] = True
             extra_kwargs["method"] = 6
         else:
             raise RuntimeError(f"Invalid format {self.out_f.suffix}")
```

### Comparing `sticker_convert-2.8.6/src/sticker_convert/definitions.py` & `sticker_convert-2.8.7/src/sticker_convert/definitions.py`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.6/src/sticker_convert/downloaders/download_base.py` & `sticker_convert-2.8.7/src/sticker_convert/downloaders/download_base.py`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.6/src/sticker_convert/downloaders/download_kakao.py` & `sticker_convert-2.8.7/src/sticker_convert/downloaders/download_kakao.py`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.6/src/sticker_convert/downloaders/download_line.py` & `sticker_convert-2.8.7/src/sticker_convert/downloaders/download_line.py`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.6/src/sticker_convert/downloaders/download_signal.py` & `sticker_convert-2.8.7/src/sticker_convert/downloaders/download_signal.py`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.6/src/sticker_convert/downloaders/download_telegram.py` & `sticker_convert-2.8.7/src/sticker_convert/downloaders/download_telegram.py`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.6/src/sticker_convert/downloaders/download_viber.py` & `sticker_convert-2.8.7/src/sticker_convert/downloaders/download_viber.py`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.6/src/sticker_convert/gui.py` & `sticker_convert-2.8.7/src/sticker_convert/gui.py`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.6/src/sticker_convert/gui_components/frames/comp_frame.py` & `sticker_convert-2.8.7/src/sticker_convert/gui_components/frames/comp_frame.py`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.6/src/sticker_convert/gui_components/frames/config_frame.py` & `sticker_convert-2.8.7/src/sticker_convert/gui_components/frames/config_frame.py`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.6/src/sticker_convert/gui_components/frames/control_frame.py` & `sticker_convert-2.8.7/src/sticker_convert/gui_components/frames/control_frame.py`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.6/src/sticker_convert/gui_components/frames/cred_frame.py` & `sticker_convert-2.8.7/src/sticker_convert/gui_components/frames/cred_frame.py`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.6/src/sticker_convert/gui_components/frames/input_frame.py` & `sticker_convert-2.8.7/src/sticker_convert/gui_components/frames/input_frame.py`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.6/src/sticker_convert/gui_components/frames/output_frame.py` & `sticker_convert-2.8.7/src/sticker_convert/gui_components/frames/output_frame.py`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.6/src/sticker_convert/gui_components/frames/progress_frame.py` & `sticker_convert-2.8.7/src/sticker_convert/gui_components/frames/progress_frame.py`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.6/src/sticker_convert/gui_components/frames/right_clicker.py` & `sticker_convert-2.8.7/src/sticker_convert/gui_components/frames/right_clicker.py`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.6/src/sticker_convert/gui_components/gui_utils.py` & `sticker_convert-2.8.7/src/sticker_convert/gui_components/gui_utils.py`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.6/src/sticker_convert/gui_components/windows/advanced_compression_window.py` & `sticker_convert-2.8.7/src/sticker_convert/gui_components/windows/advanced_compression_window.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 #!/usr/bin/env python3
 from __future__ import annotations
 
+import re
 from functools import partial
 from tkinter import colorchooser
 from typing import Any, List, Tuple
 
 from PIL import Image, ImageDraw, ImageTk
 from ttkbootstrap import Button, Canvas, Checkbutton, Entry, Frame, Label, LabelFrame, OptionMenu, Scrollbar, StringVar  # type: ignore
 
@@ -576,17 +577,25 @@
             state = "disabled"
         else:
             state = "normal"
 
         self.fake_vid_cbox.config(state=state)
 
     def cb_bg_color(self, *_: Any) -> None:
-        color = colorchooser.askcolor(title="Choose color")[1]
+        color_init = "#" + self.gui.bg_color_var.get()[:6]
+        color_init = (
+            color_init if re.search(r"^#(?:[0-9a-fA-F]{3}){1,2}$", color_init) else None
+        )
+        color = colorchooser.askcolor(
+            title="Choose color",
+            color=color_init,
+            parent=self,
+        )[1]
         if color:
-            self.gui.bg_color_var.set(color.replace("#", ""))
+            self.gui.bg_color_var.set(color.replace("#", "") + "00")
         self.lift()
         self.attributes("-topmost", True)  # type: ignore
         self.attributes("-topmost", False)  # type: ignore
 
     def cb_bound_to_mousewheel(self, event: Any) -> None:
         for i in self.mousewheel:
             self.emoji_canvas.bind_all(i, self.cb_on_mousewheel)
```

### Comparing `sticker_convert-2.8.6/src/sticker_convert/gui_components/windows/base_window.py` & `sticker_convert-2.8.7/src/sticker_convert/gui_components/windows/base_window.py`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.6/src/sticker_convert/gui_components/windows/kakao_get_auth_window.py` & `sticker_convert-2.8.7/src/sticker_convert/gui_components/windows/kakao_get_auth_window.py`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.6/src/sticker_convert/gui_components/windows/line_get_auth_window.py` & `sticker_convert-2.8.7/src/sticker_convert/gui_components/windows/line_get_auth_window.py`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.6/src/sticker_convert/gui_components/windows/signal_get_auth_window.py` & `sticker_convert-2.8.7/src/sticker_convert/gui_components/windows/signal_get_auth_window.py`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.6/src/sticker_convert/ios-message-stickers-template/stickers/Info.plist` & `sticker_convert-2.8.7/src/sticker_convert/ios-message-stickers-template/stickers/Info.plist`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.6/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Info.plist` & `sticker_convert-2.8.7/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Info.plist`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.6/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/Sticker Pack.stickerpack/Sticker 1.sticker/Sticker 1.png` & `sticker_convert-2.8.7/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/Sticker Pack.stickerpack/Sticker 1.sticker/Sticker 1.png`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.6/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/Sticker Pack.stickerpack/Sticker 2.sticker/Sticker 2.png` & `sticker_convert-2.8.7/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/Sticker Pack.stickerpack/Sticker 2.sticker/Sticker 2.png`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.6/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/Sticker Pack.stickerpack/Sticker 3.sticker/Sticker 3.png` & `sticker_convert-2.8.7/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/Sticker Pack.stickerpack/Sticker 3.sticker/Sticker 3.png`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.6/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/App-Store-1024x1024pt.png` & `sticker_convert-2.8.7/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/App-Store-1024x1024pt.png`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.6/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Contents.json` & `sticker_convert-2.8.7/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Contents.json`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.6/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages-App-Store-1024x768pt.png` & `sticker_convert-2.8.7/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages-App-Store-1024x768pt.png`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.6/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages-iPad-67x50pt@2x.png` & `sticker_convert-2.8.7/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages-iPad-67x50pt@2x.png`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.6/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages-iPad-Pro-74x55pt@2x.png` & `sticker_convert-2.8.7/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages-iPad-Pro-74x55pt@2x.png`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.6/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages-iPhone-60x45pt@2x.png` & `sticker_convert-2.8.7/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages-iPhone-60x45pt@2x.png`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.6/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages-iPhone-60x45pt@3x.png` & `sticker_convert-2.8.7/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages-iPhone-60x45pt@3x.png`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.6/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages27x20pt@2x.png` & `sticker_convert-2.8.7/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages27x20pt@2x.png`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.6/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages27x20pt@3x.png` & `sticker_convert-2.8.7/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages27x20pt@3x.png`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.6/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages32x24pt@2x.png` & `sticker_convert-2.8.7/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages32x24pt@2x.png`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.6/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages32x24pt@3x.png` & `sticker_convert-2.8.7/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages32x24pt@3x.png`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.6/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/iPad-Settings-29pt@2x.png` & `sticker_convert-2.8.7/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/iPad-Settings-29pt@2x.png`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.6/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/iPhone-Settings-29pt@3x.png` & `sticker_convert-2.8.7/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/iPhone-Settings-29pt@3x.png`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.6/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/iPhone-settings-29pt@2x.png` & `sticker_convert-2.8.7/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/iPhone-settings-29pt@2x.png`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.6/src/sticker_convert/ios-message-stickers-template/stickers.xcodeproj/project.pbxproj` & `sticker_convert-2.8.7/src/sticker_convert/ios-message-stickers-template/stickers.xcodeproj/project.pbxproj`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.6/src/sticker_convert/ios-message-stickers-template/stickers.xcodeproj/project.xcworkspace/xcuserdata/niklaspeterson.xcuserdatad/UserInterfaceState.xcuserstate` & `sticker_convert-2.8.7/src/sticker_convert/ios-message-stickers-template/stickers.xcodeproj/project.xcworkspace/xcuserdata/niklaspeterson.xcuserdatad/UserInterfaceState.xcuserstate`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.6/src/sticker_convert/job.py` & `sticker_convert-2.8.7/src/sticker_convert/job.py`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.6/src/sticker_convert/job_option.py` & `sticker_convert-2.8.7/src/sticker_convert/job_option.py`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.6/src/sticker_convert/resources/NotoColorEmoji.ttf` & `sticker_convert-2.8.7/src/sticker_convert/resources/NotoColorEmoji.ttf`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.6/src/sticker_convert/resources/appicon.icns` & `sticker_convert-2.8.7/src/sticker_convert/resources/appicon.icns`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.6/src/sticker_convert/resources/appicon.ico` & `sticker_convert-2.8.7/src/sticker_convert/resources/appicon.ico`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.6/src/sticker_convert/resources/appicon.png` & `sticker_convert-2.8.7/src/sticker_convert/resources/appicon.png`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.6/src/sticker_convert/resources/compression.json` & `sticker_convert-2.8.7/src/sticker_convert/resources/compression.json`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.6/src/sticker_convert/resources/emoji.json` & `sticker_convert-2.8.7/src/sticker_convert/resources/emoji.json`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.6/src/sticker_convert/resources/help.json` & `sticker_convert-2.8.7/src/sticker_convert/resources/help.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.99875%*

 * *Differences: {"'comp'": "{'bg_color': 'Set custom background color in rrggbbaa format.\\nExample: 00ff0000 for "*

 * *           'green with alpha 0.\\nIf this is not set, background color would be auto set to black '*

 * *           'if image is bright, or white if image is dark.\\nNote: The color should not be visible '*

 * *           "if output format supports transparency.'}"}*

```diff
@@ -1,10 +1,10 @@
 {
     "comp": {
-        "bg_color": "Set custom background color.\nExample: 00ff00 for green.\nIf this is not set, background color would be auto set to black if image is bright, or white if image is dark.\nNote: The color should not be visible if output format supports transparency.",
+        "bg_color": "Set custom background color in rrggbbaa format.\nExample: 00ff0000 for green with alpha 0.\nIf this is not set, background color would be auto set to black if image is bright, or white if image is dark.\nNote: The color should not be visible if output format supports transparency.",
         "cache_dir": "Set custom cache directory.\nUseful for debugging, or speed up conversion if cache_dir is on RAM disk.",
         "color": "Reduce size by limiting number of colors.\nMakes image 'blocky'. >256 will disable this.\nApplies to png and apng only.\nColor higher = More colors but larger size.",
         "color_max": "Set maximum number of colors (For converting to apng and apng only).",
         "color_min": "Set minimum number of colors (For converting to apng and apng only).",
         "color_power": "Between -1 and positive infinity. Power lower = More importance of the parameter, try harder to keep higher and not sacrifice.",
         "default_emoji": "Set the default emoji for uploading Signal and Telegram sticker packs.",
         "duration": "Change playback speed if outside of duration limit.\nDuration set in miliseconds.\n0 will disable limit.",
```

### Comparing `sticker_convert-2.8.6/src/sticker_convert/resources/input.json` & `sticker_convert-2.8.7/src/sticker_convert/resources/input.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9928571428571429%*

 * *Differences: {"'auto'": "{'example': 'Supported input sources: Signal, Telegram, Line, Kakao, Viber'}"}*

```diff
@@ -1,11 +1,11 @@
 {
     "auto": {
         "address_lbls": "URL address",
-        "example": "Supported input sources: Signal, Telegram, Line, Kakao",
+        "example": "Supported input sources: Signal, Telegram, Line, Kakao, Viber",
         "full_name": "Download (Auto detect)",
         "help": "Auto detect URL type and download",
         "metadata_provides": {
             "author": false,
             "title": false
         }
     },
```

### Comparing `sticker_convert-2.8.6/src/sticker_convert/resources/output.json` & `sticker_convert-2.8.7/src/sticker_convert/resources/output.json`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.6/src/sticker_convert/uploaders/compress_wastickers.py` & `sticker_convert-2.8.7/src/sticker_convert/uploaders/compress_wastickers.py`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.6/src/sticker_convert/uploaders/upload_base.py` & `sticker_convert-2.8.7/src/sticker_convert/uploaders/upload_base.py`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.6/src/sticker_convert/uploaders/upload_signal.py` & `sticker_convert-2.8.7/src/sticker_convert/uploaders/upload_signal.py`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.6/src/sticker_convert/uploaders/upload_telegram.py` & `sticker_convert-2.8.7/src/sticker_convert/uploaders/upload_telegram.py`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.6/src/sticker_convert/uploaders/xcode_imessage.py` & `sticker_convert-2.8.7/src/sticker_convert/uploaders/xcode_imessage.py`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.6/src/sticker_convert/utils/auth/get_kakao_auth.py` & `sticker_convert-2.8.7/src/sticker_convert/utils/auth/get_kakao_auth.py`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.6/src/sticker_convert/utils/auth/get_line_auth.py` & `sticker_convert-2.8.7/src/sticker_convert/utils/auth/get_line_auth.py`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.6/src/sticker_convert/utils/auth/get_signal_auth.py` & `sticker_convert-2.8.7/src/sticker_convert/utils/auth/get_signal_auth.py`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.6/src/sticker_convert/utils/callback.py` & `sticker_convert-2.8.7/src/sticker_convert/utils/callback.py`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.6/src/sticker_convert/utils/files/cache_store.py` & `sticker_convert-2.8.7/src/sticker_convert/utils/files/cache_store.py`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.6/src/sticker_convert/utils/files/json_manager.py` & `sticker_convert-2.8.7/src/sticker_convert/utils/files/json_manager.py`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.6/src/sticker_convert/utils/files/json_resources_loader.py` & `sticker_convert-2.8.7/src/sticker_convert/utils/files/json_resources_loader.py`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.6/src/sticker_convert/utils/files/metadata_handler.py` & `sticker_convert-2.8.7/src/sticker_convert/utils/files/metadata_handler.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,14 +20,15 @@
     ".mp4",
     ".mkv",
     ".mov",
     ".webm",
     ".webp",
     ".avi",
     ".m4a",
+    ".mp3",
     ".wastickers",
 )
 RELATED_NAME = (
     "title.txt",
     "author.txt",
     "emoji.txt",
     "export-result.txt",
```

### Comparing `sticker_convert-2.8.6/src/sticker_convert/utils/files/run_bin.py` & `sticker_convert-2.8.7/src/sticker_convert/utils/files/run_bin.py`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.6/src/sticker_convert/utils/files/sanitize_filename.py` & `sticker_convert-2.8.7/src/sticker_convert/utils/files/sanitize_filename.py`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.6/src/sticker_convert/utils/media/apple_png_normalize.py` & `sticker_convert-2.8.7/src/sticker_convert/utils/media/apple_png_normalize.py`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.6/src/sticker_convert/utils/media/codec_info.py` & `sticker_convert-2.8.7/src/sticker_convert/utils/media/codec_info.py`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.6/src/sticker_convert/utils/media/decrypt_kakao.py` & `sticker_convert-2.8.7/src/sticker_convert/utils/media/decrypt_kakao.py`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.6/src/sticker_convert/utils/media/format_verify.py` & `sticker_convert-2.8.7/src/sticker_convert/utils/media/format_verify.py`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.6/src/sticker_convert/utils/url_detect.py` & `sticker_convert-2.8.7/src/sticker_convert/utils/url_detect.py`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.6/src/sticker_convert.egg-info/PKG-INFO` & `sticker_convert-2.8.7/src/sticker_convert.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: sticker-convert
-Version: 2.8.6
-Summary: Convert (animated) stickers to/from WhatsApp, Telegram, Signal, Line, Kakao, iMessage. Written in Python.
+Version: 2.8.7
+Summary: Convert (animated) stickers to/from WhatsApp, Telegram, Signal, Line, Kakao, Viber, iMessage. Written in Python.
 Author-email: laggykiller <chaudominic2@gmail.com>
 Maintainer-email: laggykiller <chaudominic2@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 2, June 1991
         
          Copyright (C) 1989, 1991 Free Software Foundation, Inc.,
          51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA
@@ -582,16 +582,16 @@
                         Between -1 and positive infinity. Power lower = More importance of the parameter, try harder to keep higher and not sacrifice.
   --duration-min DURATION_MIN
                         Set minimum output duration in miliseconds.
   --duration-max DURATION_MAX
                         Set maximum output duration in miliseconds.
   --padding-percent PADDING_PERCENT
                         Set percentage of space used as padding.
-  --bg-color BG_COLOR   Set custom background color.
-                        Example: 00ff00 for green.
+  --bg-color BG_COLOR   Set custom background color in rrggbbaa format.
+                        Example: 00ff00 for green with alpha 0.
                         If this is not set, background color would be auto set to black if image is bright, or white if image is dark.
                         Note: The color should not be visible if output format supports transparency.
   --vid-size-max VID_SIZE_MAX
                         Set maximum file size limit for animated stickers.
   --img-size-max IMG_SIZE_MAX
                         Set maximum file size limit for static stickers.
   --vid-format VID_FORMAT
@@ -764,14 +764,15 @@
 
 ### Platform-specific guides (e.g. Getting credentials)
 - [Signal](docs/guide_signal.md)
 - [Telegram](docs/guide_telegram.md)
 - [WhatsApp](docs/guide_whatsapp.md)
 - [Line](docs/guide_line.md)
 - [Kakao](docs/guide_kakao.md)
+- [Viber](docs/guide_viber.md)
 - [iMessage](docs/guide_imessage.md)
 
 ### Conversion is slow
 Try the following tips:
 - Increase number of processes (`--processes`)
     - Increasing over default value can actually be slower though
 - Decrease number of steps (`--steps`)
@@ -821,11 +822,12 @@
 ## Credits
 - Information about Signal and Telegram stickers: https://github.com/teynav/signalApngSticker
 - Information about Line and Kakao stickers: https://github.com/star-39/moe-sticker-bot
 - Information about Line stickers: https://github.com/doubleplusc/Line-sticker-downloader
 - Information about Kakao animated stickers: https://gist.github.com/chitacan/9802668
 - Downloading and decrypting Kakao animated stickers: https://github.com/blluv/KakaoTalkEmoticonDownloader
 - Application icon taken from [Icons8](https://icons8.com/)
+- Banner generated from [GitHub Socialify](https://socialify.git.ci/)
 
 ## DISCLAIMER
 - The author of this repo is NOT affiliated with Signal, Telegram, WhatsApp, Line, Kakao or Sticker Maker.
 - The author of this repo is NOT repsonsible for any legal consequences and loss incurred from using this repo.
```

### Comparing `sticker_convert-2.8.6/src/sticker_convert.egg-info/SOURCES.txt` & `sticker_convert-2.8.7/src/sticker_convert.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.6/tests/test_compression.py` & `sticker_convert-2.8.7/tests/test_compression.py`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.6/tests/test_download.py` & `sticker_convert-2.8.7/tests/test_download.py`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.6/tests/test_export.py` & `sticker_convert-2.8.7/tests/test_export.py`

 * *Files identical despite different names*

