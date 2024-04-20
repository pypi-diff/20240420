# Comparing `tmp/TUIFIManager-3.3.5.tar.gz` & `tmp/TUIFIManager-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TUIFIManager-3.3.5.tar", last modified: Sat Sep  2 14:15:53 2023, max compression
+gzip compressed data, was "TUIFIManager-4.0.0.tar", last modified: Sat Apr 20 09:35:48 2024, max compression
```

## Comparing `TUIFIManager-3.3.5.tar` & `TUIFIManager-4.0.0.tar`

### file list

```diff
@@ -1,38 +1,39 @@
-drwxr-xr-x   0 xou       (1000) xou       (1000)        0 2023-09-02 14:15:53.498027 TUIFIManager-3.3.5/
--rw-r--r--   0 xou       (1000) xou       (1000)      132 2023-08-04 06:46:27.000000 TUIFIManager-3.3.5/.gitattributes
-drwxr-xr-x   0 xou       (1000) xou       (1000)        0 2023-09-02 14:15:53.488027 TUIFIManager-3.3.5/.github/
-drwxr-xr-x   0 xou       (1000) xou       (1000)        0 2023-09-02 14:15:53.494694 TUIFIManager-3.3.5/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 xou       (1000) xou       (1000)      437 2023-08-05 01:45:08.000000 TUIFIManager-3.3.5/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 xou       (1000) xou       (1000)      604 2023-08-05 01:47:30.000000 TUIFIManager-3.3.5/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 xou       (1000) xou       (1000)        0 2023-09-02 14:15:53.494694 TUIFIManager-3.3.5/.github/workflows/
--rw-r--r--   0 xou       (1000) xou       (1000)      652 2023-01-04 08:02:28.000000 TUIFIManager-3.3.5/.github/workflows/nox_ci.yml
--rw-r--r--   0 xou       (1000) xou       (1000)      605 2022-12-31 18:56:42.000000 TUIFIManager-3.3.5/.gitignore
--rw-r--r--   0 xou       (1000) xou       (1000)      464 2023-01-04 08:02:28.000000 TUIFIManager-3.3.5/.scrutinizer.yml
--rw-r--r--   0 xou       (1000) xou       (1000)      492 2023-01-04 08:02:28.000000 TUIFIManager-3.3.5/.sourcery.yaml
--rw-r--r--   0 xou       (1000) xou       (1000)     7729 2023-01-18 17:40:22.000000 TUIFIManager-3.3.5/CHANGELOG.md
--rw-r--r--   0 xou       (1000) xou       (1000)    35149 2023-01-18 17:33:41.000000 TUIFIManager-3.3.5/LICENSE
--rw-r--r--   0 xou       (1000) xou       (1000)     8823 2023-09-02 14:15:53.498027 TUIFIManager-3.3.5/PKG-INFO
--rw-r--r--   0 xou       (1000) xou       (1000)  1285986 2023-08-04 23:04:46.000000 TUIFIManager-3.3.5/Peek.gif
--rw-r--r--   0 xou       (1000) xou       (1000)     7725 2023-08-15 12:16:53.000000 TUIFIManager-3.3.5/README.md
--rw-r--r--   0 xou       (1000) xou       (1000)   246555 2022-12-31 18:56:42.000000 TUIFIManager-3.3.5/TUIFI.png
-drwxr-xr-x   0 xou       (1000) xou       (1000)        0 2023-09-02 14:15:53.494694 TUIFIManager-3.3.5/TUIFIManager/
--rw-r--r--   0 xou       (1000) xou       (1000)    29042 2023-08-07 15:10:23.000000 TUIFIManager-3.3.5/TUIFIManager/TUIFIProfile.py
--rw-r--r--   0 xou       (1000) xou       (1000)     6025 2023-08-08 06:39:14.000000 TUIFIManager-3.3.5/TUIFIManager/TUIFile.py
--rw-r--r--   0 xou       (1000) xou       (1000)     6460 2023-08-06 09:01:10.000000 TUIFIManager-3.3.5/TUIFIManager/TUIMenu.py
--rw-r--r--   0 xou       (1000) xou       (1000)    11402 2023-08-07 05:50:19.000000 TUIFIManager-3.3.5/TUIFIManager/TUItilities.py
--rw-r--r--   0 xou       (1000) xou       (1000)    61425 2023-09-02 14:13:01.000000 TUIFIManager-3.3.5/TUIFIManager/__init__.py
--rw-r--r--   0 xou       (1000) xou       (1000)     3109 2023-09-02 14:08:31.000000 TUIFIManager-3.3.5/TUIFIManager/__main__.py
-drwxr-xr-x   0 xou       (1000) xou       (1000)        0 2023-09-02 14:15:53.498027 TUIFIManager-3.3.5/TUIFIManager.egg-info/
--rw-r--r--   0 xou       (1000) xou       (1000)     8823 2023-09-02 14:15:53.000000 TUIFIManager-3.3.5/TUIFIManager.egg-info/PKG-INFO
--rw-r--r--   0 xou       (1000) xou       (1000)      671 2023-09-02 14:15:53.000000 TUIFIManager-3.3.5/TUIFIManager.egg-info/SOURCES.txt
--rw-r--r--   0 xou       (1000) xou       (1000)        1 2023-09-02 14:15:53.000000 TUIFIManager-3.3.5/TUIFIManager.egg-info/dependency_links.txt
--rw-r--r--   0 xou       (1000) xou       (1000)       53 2023-09-02 14:15:53.000000 TUIFIManager-3.3.5/TUIFIManager.egg-info/entry_points.txt
--rw-r--r--   0 xou       (1000) xou       (1000)       36 2023-09-02 14:15:53.000000 TUIFIManager-3.3.5/TUIFIManager.egg-info/requires.txt
--rw-r--r--   0 xou       (1000) xou       (1000)       13 2023-09-02 14:15:53.000000 TUIFIManager-3.3.5/TUIFIManager.egg-info/top_level.txt
--rw-r--r--   0 xou       (1000) xou       (1000)     1004 2023-08-04 06:46:27.000000 TUIFIManager-3.3.5/flake.lock
--rw-r--r--   0 xou       (1000) xou       (1000)      695 2023-08-04 06:46:27.000000 TUIFIManager-3.3.5/flake.nix
--rw-r--r--   0 xou       (1000) xou       (1000)      201 2023-01-04 08:02:28.000000 TUIFIManager-3.3.5/noxfile.py
--rw-r--r--   0 xou       (1000) xou       (1000)     1093 2023-09-02 14:11:11.000000 TUIFIManager-3.3.5/pyproject.toml
--rw-r--r--   0 xou       (1000) xou       (1000)       40 2023-01-04 08:02:28.000000 TUIFIManager-3.3.5/requirements.txt
--rw-r--r--   0 xou       (1000) xou       (1000)     1272 2023-09-02 14:15:53.498027 TUIFIManager-3.3.5/setup.cfg
--rw-r--r--   0 xou       (1000) xou       (1000)       69 2023-01-04 08:02:28.000000 TUIFIManager-3.3.5/setup.py
+drwxr-xr-x   0 xou       (1000) xou       (1000)        0 2024-04-20 09:35:48.899902 TUIFIManager-4.0.0/
+-rw-r--r--   0 xou       (1000) xou       (1000)      132 2023-10-01 12:46:14.000000 TUIFIManager-4.0.0/.gitattributes
+drwxr-xr-x   0 xou       (1000) xou       (1000)        0 2024-04-20 09:35:48.893235 TUIFIManager-4.0.0/.github/
+drwxr-xr-x   0 xou       (1000) xou       (1000)        0 2024-04-20 09:35:48.896569 TUIFIManager-4.0.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 xou       (1000) xou       (1000)      437 2023-10-01 12:46:14.000000 TUIFIManager-4.0.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 xou       (1000) xou       (1000)      604 2023-10-01 12:46:14.000000 TUIFIManager-4.0.0/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 xou       (1000) xou       (1000)        0 2024-04-20 09:35:48.896569 TUIFIManager-4.0.0/.github/workflows/
+-rw-r--r--   0 xou       (1000) xou       (1000)      652 2023-10-01 12:46:14.000000 TUIFIManager-4.0.0/.github/workflows/nox_ci.yml
+-rw-r--r--   0 xou       (1000) xou       (1000)      605 2023-10-01 12:46:14.000000 TUIFIManager-4.0.0/.gitignore
+-rw-r--r--   0 xou       (1000) xou       (1000)      464 2023-10-01 12:46:14.000000 TUIFIManager-4.0.0/.scrutinizer.yml
+-rw-r--r--   0 xou       (1000) xou       (1000)      492 2023-10-01 12:46:14.000000 TUIFIManager-4.0.0/.sourcery.yaml
+-rw-r--r--   0 xou       (1000) xou       (1000)     7729 2023-10-01 12:46:14.000000 TUIFIManager-4.0.0/CHANGELOG.md
+-rw-r--r--   0 xou       (1000) xou       (1000)    35149 2023-10-01 12:46:14.000000 TUIFIManager-4.0.0/LICENSE
+-rw-r--r--   0 xou       (1000) xou       (1000)    10650 2024-04-20 09:35:48.899902 TUIFIManager-4.0.0/PKG-INFO
+-rw-r--r--   0 xou       (1000) xou       (1000)  1632442 2024-04-19 15:58:04.000000 TUIFIManager-4.0.0/Peek.gif
+-rw-r--r--   0 xou       (1000) xou       (1000)     9552 2024-04-20 09:09:44.000000 TUIFIManager-4.0.0/README.md
+-rw-r--r--   0 xou       (1000) xou       (1000)   246555 2023-10-01 12:46:14.000000 TUIFIManager-4.0.0/TUIFI.png
+drwxr-xr-x   0 xou       (1000) xou       (1000)        0 2024-04-20 09:35:48.899902 TUIFIManager-4.0.0/TUIFIManager/
+-rw-r--r--   0 xou       (1000) xou       (1000)    31045 2024-04-20 08:55:24.000000 TUIFIManager-4.0.0/TUIFIManager/TUIFIProfile.py
+-rw-r--r--   0 xou       (1000) xou       (1000)     5509 2024-04-11 13:08:50.000000 TUIFIManager-4.0.0/TUIFIManager/TUIFile.py
+-rw-r--r--   0 xou       (1000) xou       (1000)     5044 2024-04-19 15:56:05.000000 TUIFIManager-4.0.0/TUIFIManager/TUIMenu.py
+-rw-r--r--   0 xou       (1000) xou       (1000)     8377 2024-04-19 15:58:04.000000 TUIFIManager-4.0.0/TUIFIManager/TUISynthXDND.py
+-rw-r--r--   0 xou       (1000) xou       (1000)    11793 2024-04-20 08:55:32.000000 TUIFIManager-4.0.0/TUIFIManager/TUItilities.py
+-rw-r--r--   0 xou       (1000) xou       (1000)    73488 2024-04-20 09:24:19.000000 TUIFIManager-4.0.0/TUIFIManager/__init__.py
+-rw-r--r--   0 xou       (1000) xou       (1000)     3109 2024-04-20 09:24:48.000000 TUIFIManager-4.0.0/TUIFIManager/__main__.py
+drwxr-xr-x   0 xou       (1000) xou       (1000)        0 2024-04-20 09:35:48.899902 TUIFIManager-4.0.0/TUIFIManager.egg-info/
+-rw-r--r--   0 xou       (1000) xou       (1000)    10650 2024-04-20 09:35:48.000000 TUIFIManager-4.0.0/TUIFIManager.egg-info/PKG-INFO
+-rw-r--r--   0 xou       (1000) xou       (1000)      700 2024-04-20 09:35:48.000000 TUIFIManager-4.0.0/TUIFIManager.egg-info/SOURCES.txt
+-rw-r--r--   0 xou       (1000) xou       (1000)        1 2024-04-20 09:35:48.000000 TUIFIManager-4.0.0/TUIFIManager.egg-info/dependency_links.txt
+-rw-r--r--   0 xou       (1000) xou       (1000)       53 2024-04-20 09:35:48.000000 TUIFIManager-4.0.0/TUIFIManager.egg-info/entry_points.txt
+-rw-r--r--   0 xou       (1000) xou       (1000)       36 2024-04-20 09:35:48.000000 TUIFIManager-4.0.0/TUIFIManager.egg-info/requires.txt
+-rw-r--r--   0 xou       (1000) xou       (1000)       13 2024-04-20 09:35:48.000000 TUIFIManager-4.0.0/TUIFIManager.egg-info/top_level.txt
+-rw-r--r--   0 xou       (1000) xou       (1000)     1497 2024-04-05 13:07:00.000000 TUIFIManager-4.0.0/flake.lock
+-rw-r--r--   0 xou       (1000) xou       (1000)     1713 2024-04-05 19:20:12.000000 TUIFIManager-4.0.0/flake.nix
+-rw-r--r--   0 xou       (1000) xou       (1000)      201 2023-10-01 12:46:14.000000 TUIFIManager-4.0.0/noxfile.py
+-rw-r--r--   0 xou       (1000) xou       (1000)     1093 2024-04-20 09:23:34.000000 TUIFIManager-4.0.0/pyproject.toml
+-rw-r--r--   0 xou       (1000) xou       (1000)       40 2024-04-05 13:07:00.000000 TUIFIManager-4.0.0/requirements.txt
+-rw-r--r--   0 xou       (1000) xou       (1000)     1272 2024-04-20 09:35:48.899902 TUIFIManager-4.0.0/setup.cfg
+-rw-r--r--   0 xou       (1000) xou       (1000)       69 2023-10-01 12:46:14.000000 TUIFIManager-4.0.0/setup.py
```

### Comparing `TUIFIManager-3.3.5/.github/ISSUE_TEMPLATE/feature_request.md` & `TUIFIManager-4.0.0/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `TUIFIManager-3.3.5/.github/workflows/nox_ci.yml` & `TUIFIManager-4.0.0/.github/workflows/nox_ci.yml`

 * *Files identical despite different names*

### Comparing `TUIFIManager-3.3.5/.gitignore` & `TUIFIManager-4.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `TUIFIManager-3.3.5/CHANGELOG.md` & `TUIFIManager-4.0.0/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `TUIFIManager-3.3.5/LICENSE` & `TUIFIManager-4.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `TUIFIManager-3.3.5/PKG-INFO` & `TUIFIManager-4.0.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,51 +1,32 @@
-Metadata-Version: 2.1
-Name: TUIFIManager
-Version: 3.3.5
-Summary: A cross-platform terminal-based termux-oriented file manager.
-Home-page: https://github.com/GiorgosXou/TUIFIManager
-Author: George Chousos
-Author-email: gxousos@gmail.com
-License: General Public License v3.0
-Project-URL: Github, https://github.com/GiorgosXou/TUIFIManager
-Keywords: file-manager,terminal,tui,ncurses,pdcurses,uni-curses,termux,vim,vim-motions,cross-platform
-Platform: unix
-Platform: linux
-Platform: osx
-Platform: cygwin
-Platform: windows
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: End Users/Desktop
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: POSIX
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 
 
 <div align="center">
 <h1>TUIFI Manager</h1>
 <p>
     <a href="https://github.com/GiorgosXou/TUIFIManager/pulse">
       <img src="https://img.shields.io/github/last-commit/GiorgosXou/TUIFIManager?color=%4dc71f&label=Last%20Commit&logo=github&style=flat-square"/>
     </a>
     <a href="https://github.com/GiorgosXou/TUIFIManager/blob/master/LICENSE">
       <img src="https://img.shields.io/github/license/GiorgosXou/TUIFIManager?label=License&logo=GNU&style=flat-square"/>
 	</a>
 </p>
 </div>
 
-A cross-platform terminal-based termux-oriented file manager *(and component)*, meant to be used with a [Uni-Curses](https://github.com/unicurses/unicurses) project or as is. This project is mainly an attempt to get more attention to the [Uni-Curses](https://github.com/unicurses/unicurses) project.
+A cross-platform terminal-based termux-oriented file manager *(and component)*, meant to be used with a [Uni-Curses](https://github.com/unicurses/unicurses) project or as is. This project is mainly an attempt to get more attention to the [Uni-Curses](https://github.com/unicurses/unicurses) project. 
+
+##
+<div align="center">
+<p>
+<img src="./Peek.gif">
+</p>
+<p>
+<sub>FONT: Cartograph CF</sub>
+</p>
+</div>
 
 
 # ⚙️ Installation
 ```terminal
 sudo pip3 install tuifimanager --upgrade
 ```
 ```terminal
@@ -57,51 +38,52 @@
 # 💥 Usage
 Run `tuifi` in your terminal to use it as is or import it in one of your [Uni-Curses](https://github.com/unicurses/unicurses) project as a component like:
 ```python
 from TUIFIManager import *
 ```
 for more details look into the `__main__.py`
 
-<img src="./Peek.gif">
-<sub>FONT: Cartograph CF</sub>
 
 # 📦 Features 
 ### • 📌 *Current:*
-- Supports most of the common mouse events so far
-- It is somewhat fully customizable?
+- [Supports X11 Drag&Drop from terminals](#-customization 'set `tuifi_synth_dnd` enviroment variable to `True`. `pip install pynput PySide6 python-xlib`...')
+- Supports most common mouse events 
 - Can be used as a component
-- Uses only ~30MB of RAM
+- Uses about [~30MB](## '80mb with synthetic xdnd') of RAM
+- Strong [C TUI backend](https://github.com/unicurses/unicurses 'Via Uni-Curses, a NCurses\\PDCurses wrapper')
 - It is pretty snappy <!-- Kinda lol -->
 - Supports [Termux](https://github.com/termux) 
 - Cross Platform 
 - and more
 
 ### • 🔮 *Desired:*
+- Macros
+- [Treeview](## 'Via a `WindowPad`')
 - Undo\Redo
-- tool-tips
-- Scroll bar
-- [Sixel support](https://github.com/GiorgosXou/TUIFIManager/issues/86)
+- Improved UI
 - Multiple tabs
-- Better performance
+- [Sixel support](https://github.com/GiorgosXou/TUIFIManager/issues/86#issuecomment-2016846146)
 - Effect on cutted Files
-- [Drop files into GUI apps](https://github.com/GiorgosXou/TUIFIManager/issues/21)
+- Multithread performance
 
 # ⌨️ Keybindings
 In `vim_mode` both normal and vim shortcuts work 
 | Normal      | vim_mode | Action                                        |
-|----         | ---- |:----                                          |
+|----         | ---- |----                                          |
 |`SHIFT + TAB`  |   |Moves selected file to the previous directory |
 |`KEY_BACKSPACE`| `J` |Opens\Goes to the previous directory          |
 |`ALT + DOWN`   |   |Opens\Closes the "right-click menu"           |
 |`KEY_HOME`     | `H`  |Navigates to the $HOME directory              |
 |`KEY_F5`       |   |Reload\Refresh current directory              |
+|`KEY_F3`       | `o`  |(descending) order-type switch|
+|`KEY_F1`       | `O`  |(ascending) order-type switch|
 |`CTRL + V`     | `p` |Pastes the Copied or Cuted files              |
 |`DEL`          | `CTRL+d`  |Deletes the selected files                    |
 |`CTRL + F`     | `i`  |Find Files *(if not auto_find_on_typing)*     |
-|`CTRL + O`     | `O`  |Open whole directory in editor                |
+|`CTRL + O`     |   |Open whole directory in editor                |
 |`CTRL + A`     |  |Select all files in current folder|
 |`CTRL + C`     | `yy`  |Copies the selected files                     |
 |`CTRL + K`     |   |Copies the selected files                     |
 |`CTRL + X`     | `c`  |Cuts the selected files                       |
 |`CTRL + R`     | `r` |Rename selected file                          | 
 |`CTRL + T`     | | Toggle hidden files|
 |`CTRL + N`     | `W` |Create new folder                             |
@@ -122,73 +104,115 @@
 |`CTRL + UP`  | Same as `CTRL + V`, Pastes the Copied or Cuted files                           |
 |`END`        | Deletes selected files                                                         |
 
 
 # 👨‍💻 Commands
 **(Default & Custom Comands)** - To perform a command under the normal-mode, you first have to press the space-bar and then type the command. Alternatively, use `vim_mode` or enable the `tuifi_auto_command_on_typing` env-variable *(notice: it disables `tuifi_auto_find_on_typing`)*. **The default commands can be seen below and can be found under the `~/.config/tuifi/cmds.conf` where you can add your custom ones too:**
 
-| Cmd | Type | Attributes | Label Comment|
+| Cmd | Type | Attributes | Label Information|
 |---|---|---|---|
 |`gt` | open | 'directory':'~/.config/tuifi'           | - tuifi -|
 |`gh` | open | 'directory':'~/'                        | - Home -|
 |`owv` | open | 'directory':None,'\_with':'vim'         |Opened With Vim|
 |`yat` | copy | 'pattern':'.+\.txt'                     ||
 |`yy` | copy | 'pattern':None                          ||
 
-There are also some "static" ones like the `m`+character which marks the current directory into the character, so you can navigate back to it by using \` or `;`+that_character 
+**Available Type-keywords:** `open`, `copy`, `cut`, [`find`](## 'Attributes: `filename`')
+
+**important note:** `o` is also used for ordering in `vim_mode`. In this case you can first press space-bar before proceeding with `owv` or with any other already reserved starting key, or just change it. 
+
+**Additionally** there are also some "static" ones like the `m`+character which marks the current directory into the character, so you can navigate back to it by using \` or `;`+that_character 
+
 
 
 # 📜 Documentation
 <sub>Work in progress 🛠️🏗 ...</sub>
 
 
 # 💭 Customization 
-*How do I enable vim_mode?*
+<details>
+<summary><i>How do I enable vim_mode?</i></summary>
+
 > Set `tuifi_vim_mode` enviroment variable to `True`
 
-*How do I change the default keys (besides commands)?*
-> This is not possible right now althought you could play around with the content of `toggle_vim_mode` function under `__init__.py`
+</details>
+<details>
+<summary><i>How do I enable synthetic XDND?</i></summary>
+
+> set `tuifi_synth_dnd` enviroment variable to `True`. `pip install pynput PySide6 python-xlib`. Know it's expirimental! You'll need to adapt to it slightly, **use it as: Drag&drop + click afterwords where you want the file to be dropped.** [See also](https://github.com/GiorgosXou/TUIFIManager/discussions/92) and [this issue](https://github.com/GiorgosXou/TUIFIManager/issues/21)
+
+</details>
+<details>
+<summary><i>How do I set the default editor?</i></summary>
 
-*How do I set the default editor?*
 > Set `tuifi_default_editor` enviroment variable to `vim` or whatever you prefer
 
-*How do I disable the auto-find-mode?*
+</details>
+<details>
+<summary><i>How do I disable the auto-find-mode?</i></summary>
+
 > You can just set `tuifi_auto_find_on_typing` enviroment variable to `False`
 
-*How do I change the scroll sensitivity?*
+</details>
+<details>
+<summary><i>How do I change the scroll sensitivity?</i></summary>
+
 > You can set either or both `tuifi_scroll_sensitivity`, `tuifi_ctrl_scroll_sensitivity` enviromental variables, to the disered number of characters per scroll action *(they default to 1 and 7)*
 
-How do I change the number of visible lines of filenames that are visible?
+</details>
+<details>
+<summary><i>How do I change the default keys (besides commands)?</i></summary>
+
+> This is not possible right now althought you could play around with the content of `toggle_vim_mode` function under `__init__.py`
+
+</details>
+<details>
+<summary><i>How do I change the number of visible lines of filenames that are visible?</i></summary>
+
 > You can set how mnay lines you want using `tuifi_visible_filename_lines` *(Defaults to 4)*
 
-*How do I change the default configuration path?*
+</details>
+<details>
+<summary><i>How do I change the default configuration path?</i></summary>
+
 > Set `tuifi_config_path` enviroment variable to whatever you prefer most
 
-*How do I toggle hidden files/folders?*
+</details>
+<details>
+<summary><i>How do I toggle hidden files/folders?</i></summary>
+
 > You can either `CTRL + T` or set `tuifi_show_hidden` enviroment variable to `True`
 
-*How do I change the default colors?*
+</details>
+<details>
+<summary><i>How do I change the default colors?</i></summary>
+
 > [look here for more informations](https://github.com/GiorgosXou/TUIFIManager/issues/38)
 
+</details>
+
 
 # 💗 Donation
 I do really need money to survive, I have no job, living in a basement, making things for free, because I love to.
 - [***Paypal Address***](https://www.paypal.com/donate/?hosted_button_id=QNQN23M55EJVS)
 - ***Monero Address:*** `897ehhSQJQpGF7tYDhQM51jiX7nnHmzuYAW4q8JGwJxu8JKXvaK6AivCzatuJxnifjZ2qy98ks2g2PhmTaYCMMta2Ga2LJx`
 
 <div align="center">
 <img src='./TUIFI.png'>
 </div>
 
 
 # 🫶 Special thanks to
+- [@KORBEN for this article](https://korben.info/gestionnaire-fichiers-terminal-tuifimanager-multiplateforme-leger-personnalisable.html)
 - [Bryan Lunduke for this article](https://lunduke.substack.com/p/tuifi-manager-a-file-manager-in-the)
 - [Brodie Robertson for this video](https://youtu.be/9laxdMKTZLA)
 - [r/linux community for their comments](https://www.reddit.com/r/linux/comments/zzf5rx)
 - [r/cyberDeck community for their comments](https://www.reddit.com/r/cyberDeck/comments/zttur0)
 - [r/commandline community for their comments](https://www.reddit.com/r/commandline/comments/zt30v9)
 
-# 🕳️ Help
-Any Idea with this issue https://github.com/unicurses/unicurses/issues/21 ?
+# 🕳️ Outro
+- Any Idea with this issue https://github.com/unicurses/unicurses/issues/21 ?
+- Btw I use TUIFI in a daily basis. As crazy as it might sound: It's my primary file manager.
+
```

#### html2text {}

```diff
@@ -1,53 +1,44 @@
-Metadata-Version: 2.1 Name: TUIFIManager Version: 3.3.5 Summary: A cross-
-platform terminal-based termux-oriented file manager. Home-page: https://
-github.com/GiorgosXou/TUIFIManager Author: George Chousos Author-email:
-gxousos@gmail.com License: General Public License v3.0 Project-URL: Github,
-https://github.com/GiorgosXou/TUIFIManager Keywords: file-
-manager,terminal,tui,ncurses,pdcurses,uni-curses,termux,vim,vim-motions,cross-
-platform Platform: unix Platform: linux Platform: osx Platform: cygwin
-Platform: windows Classifier: Intended Audience :: Developers Classifier:
-Intended Audience :: End Users/Desktop Classifier: License :: OSI Approved ::
-MIT License Classifier: Operating System :: MacOS :: MacOS X Classifier:
-Operating System :: Microsoft :: Windows Classifier: Operating System :: POSIX
-Classifier: Programming Language :: Python :: 3 :: Only Classifier: Programming
-Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10 Requires-Python: >=3.8
-Description-Content-Type: text/markdown License-File: LICENSE
                           ************ TTUUIIFFII MMaannaaggeerr ************
             _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_l_a_s_t_-_c_o_m_m_i_t_/_G_i_o_r_g_o_s_X_o_u_/
  _T_U_I_F_I_M_a_n_a_g_e_r_?_c_o_l_o_r_=_%_4_d_c_7_1_f_&_l_a_b_e_l_=_L_a_s_t_%_2_0_C_o_m_m_i_t_&_l_o_g_o_=_g_i_t_h_u_b_&_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]
               _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_l_i_c_e_n_s_e_/_G_i_o_r_g_o_s_X_o_u_/
             _T_U_I_F_I_M_a_n_a_g_e_r_?_l_a_b_e_l_=_L_i_c_e_n_s_e_&_l_o_g_o_=_G_N_U_&_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]
 A cross-platform terminal-based termux-oriented file manager *(and component)*,
 meant to be used with a [Uni-Curses](https://github.com/unicurses/unicurses)
 project or as is. This project is mainly an attempt to get more attention to
-the [Uni-Curses](https://github.com/unicurses/unicurses) project. # âï¸
-Installation ```terminal sudo pip3 install tuifimanager --upgrade ```
+the [Uni-Curses](https://github.com/unicurses/unicurses) project. ##
+                                 [./Peek.gif]
+                              FONT: Cartograph CF
+# âï¸ Installation ```terminal sudo pip3 install tuifimanager --upgrade ```
 ```terminal pip3 install TUIFIManager --upgrade ``` or just ^^^ if it works for
 you. *(eg. on termux?)* # ð¥ Usage Run `tuifi` in your terminal to use it as
 is or import it in one of your [Uni-Curses](https://github.com/unicurses/
 unicurses) project as a component like: ```python from TUIFIManager import *
-``` for more details look into the `__main__.py` [./Peek.gif]FONT: Cartograph
-CF # ð¦ Features ### â¢ ð *Current:* - Supports most of the common mouse
-events so far - It is somewhat fully customizable? - Can be used as a component
-- Uses only ~30MB of RAM - It is pretty snappy - Supports [Termux](https://
-github.com/termux) - Cross Platform - and more ### â¢ ð® *Desired:* -
-Undo\Redo - tool-tips - Scroll bar - [Sixel support](https://github.com/
-GiorgosXou/TUIFIManager/issues/86) - Multiple tabs - Better performance -
-Effect on cutted Files - [Drop files into GUI apps](https://github.com/
-GiorgosXou/TUIFIManager/issues/21) # â¨ï¸ Keybindings In `vim_mode` both
-normal and vim shortcuts work | Normal | vim_mode | Action | |---- | ---- |:---
-- | |`SHIFT + TAB` | |Moves selected file to the previous directory |
-|`KEY_BACKSPACE`| `J` |Opens\Goes to the previous directory | |`ALT + DOWN` |
-|Opens\Closes the "right-click menu" | |`KEY_HOME` | `H` |Navigates to the
-$HOME directory | |`KEY_F5` | |Reload\Refresh current directory | |`CTRL + V` |
-`p` |Pastes the Copied or Cuted files | |`DEL` | `CTRL+d` |Deletes the selected
+``` for more details look into the `__main__.py` # ð¦ Features ### â¢ ð
+*Current:* - [Supports X11 Drag&Drop from terminals](#-customization 'set
+`tuifi_synth_dnd` enviroment variable to `True`. `pip install pynput PySide6
+python-xlib`...') - Supports most common mouse events - Can be used as a
+component - Uses about [~30MB](## '80mb with synthetic xdnd') of RAM - Strong
+[C TUI backend](https://github.com/unicurses/unicurses 'Via Uni-Curses, a
+NCurses\\PDCurses wrapper') - It is pretty snappy - Supports [Termux](https://
+github.com/termux) - Cross Platform - and more ### â¢ ð® *Desired:* - Macros
+- [Treeview](## 'Via a `WindowPad`') - Undo\Redo - Improved UI - Multiple tabs
+- [Sixel support](https://github.com/GiorgosXou/TUIFIManager/issues/
+86#issuecomment-2016846146) - Effect on cutted Files - Multithread performance
+# â¨ï¸ Keybindings In `vim_mode` both normal and vim shortcuts work | Normal
+| vim_mode | Action | |---- | ---- |---- | |`SHIFT + TAB` | |Moves selected
+file to the previous directory | |`KEY_BACKSPACE`| `J` |Opens\Goes to the
+previous directory | |`ALT + DOWN` | |Opens\Closes the "right-click menu" |
+|`KEY_HOME` | `H` |Navigates to the $HOME directory | |`KEY_F5` |
+|Reload\Refresh current directory | |`KEY_F3` | `o` |(descending) order-type
+switch| |`KEY_F1` | `O` |(ascending) order-type switch| |`CTRL + V` | `p`
+|Pastes the Copied or Cuted files | |`DEL` | `CTRL+d` |Deletes the selected
 files | |`CTRL + F` | `i` |Find Files *(if not auto_find_on_typing)* | |`CTRL +
-O` | `O` |Open whole directory in editor | |`CTRL + A` | |Select all files in
+O` | |Open whole directory in editor | |`CTRL + A` | |Select all files in
 current folder| |`CTRL + C` | `yy` |Copies the selected files | |`CTRL + K` |
 |Copies the selected files | |`CTRL + X` | `c` |Cuts the selected files |
 |`CTRL + R` | `r` |Rename selected file | |`CTRL + T` | | Toggle hidden files|
 |`CTRL + N` | `W` |Create new folder | |`CTRL + W` | `w` |Create new file |
 |`ARROW KEYS` | `l` `k` `j` `h` |Navigates files | |`KEY_ENTER` | `K`|Opens
 files | |`CTRL + E` | `e` |Exit with `cd` | |`ESCAPE` | |Exit | **(*TIP:** ð
 use `ALT + CLICK` for multiple mouse selection if `SHIFT` not working)*
@@ -58,45 +49,57 @@
 the selected file(s) | |`CTRL + UP` | Same as `CTRL + V`, Pastes the Copied or
 Cuted files | |`END` | Deletes selected files | # ð¨âð» Commands **
 (Default & Custom Comands)** - To perform a command under the normal-mode, you
 first have to press the space-bar and then type the command. Alternatively, use
 `vim_mode` or enable the `tuifi_auto_command_on_typing` env-variable *(notice:
 it disables `tuifi_auto_find_on_typing`)*. **The default commands can be seen
 below and can be found under the `~/.config/tuifi/cmds.conf` where you can add
-your custom ones too:** | Cmd | Type | Attributes | Label Comment| |---|---|---
-|---| |`gt` | open | 'directory':'~/.config/tuifi' | - tuifi -| |`gh` | open |
-'directory':'~/' | - Home -| |`owv` | open | 'directory':None,'\_with':'vim'
-|Opened With Vim| |`yat` | copy | 'pattern':'.+\.txt' || |`yy` | copy |
-'pattern':None || There are also some "static" ones like the `m`+character
-which marks the current directory into the character, so you can navigate back
-to it by using \` or `;`+that_character # ð Documentation Work in progress
-ð ï¸ð ... # ð­ Customization *How do I enable vim_mode?* > Set
-`tuifi_vim_mode` enviroment variable to `True` *How do I change the default
-keys (besides commands)?* > This is not possible right now althought you could
-play around with the content of `toggle_vim_mode` function under `__init__.py`
-*How do I set the default editor?* > Set `tuifi_default_editor` enviroment
-variable to `vim` or whatever you prefer *How do I disable the auto-find-mode?*
-> You can just set `tuifi_auto_find_on_typing` enviroment variable to `False`
-*How do I change the scroll sensitivity?* > You can set either or both
+your custom ones too:** | Cmd | Type | Attributes | Label Information| |---|---
+|---|---| |`gt` | open | 'directory':'~/.config/tuifi' | - tuifi -| |`gh` |
+open | 'directory':'~/' | - Home -| |`owv` | open | 'directory':None,'\_with':
+'vim' |Opened With Vim| |`yat` | copy | 'pattern':'.+\.txt' || |`yy` | copy |
+'pattern':None || **Available Type-keywords:** `open`, `copy`, `cut`, [`find`]
+(## 'Attributes: `filename`') **important note:** `o` is also used for ordering
+in `vim_mode`. In this case you can first press space-bar before proceeding
+with `owv` or with any other already reserved starting key, or just change it.
+**Additionally** there are also some "static" ones like the `m`+character which
+marks the current directory into the character, so you can navigate back to it
+by using \` or `;`+that_character # ð Documentation Work in progress
+ð ï¸ð ... # ð­ Customization How do I enable vim_mode? > Set
+`tuifi_vim_mode` enviroment variable to `True` How do I enable synthetic XDND?
+> set `tuifi_synth_dnd` enviroment variable to `True`. `pip install pynput
+PySide6 python-xlib`. Know it's expirimental! You'll need to adapt to it
+slightly, **use it as: Drag&drop + click afterwords where you want the file to
+be dropped.** [See also](https://github.com/GiorgosXou/TUIFIManager/
+discussions/92) and [this issue](https://github.com/GiorgosXou/TUIFIManager/
+issues/21) How do I set the default editor? > Set `tuifi_default_editor`
+enviroment variable to `vim` or whatever you prefer How do I disable the auto-
+find-mode? > You can just set `tuifi_auto_find_on_typing` enviroment variable
+to `False` How do I change the scroll sensitivity? > You can set either or both
 `tuifi_scroll_sensitivity`, `tuifi_ctrl_scroll_sensitivity` enviromental
 variables, to the disered number of characters per scroll action *(they default
-to 1 and 7)* How do I change the number of visible lines of filenames that are
-visible? > You can set how mnay lines you want using
-`tuifi_visible_filename_lines` *(Defaults to 4)* *How do I change the default
-configuration path?* > Set `tuifi_config_path` enviroment variable to whatever
-you prefer most *How do I toggle hidden files/folders?* > You can either `CTRL
-+ T` or set `tuifi_show_hidden` enviroment variable to `True` *How do I change
-the default colors?* > [look here for more informations](https://github.com/
-GiorgosXou/TUIFIManager/issues/38) # ð Donation I do really need money to
-survive, I have no job, living in a basement, making things for free, because I
-love to. - [***Paypal Address***](https://www.paypal.com/donate/
+to 1 and 7)* How do I change the default keys (besides commands)? > This is not
+possible right now althought you could play around with the content of
+`toggle_vim_mode` function under `__init__.py` How do I change the number of
+visible lines of filenames that are visible? > You can set how mnay lines you
+want using `tuifi_visible_filename_lines` *(Defaults to 4)* How do I change the
+default configuration path? > Set `tuifi_config_path` enviroment variable to
+whatever you prefer most How do I toggle hidden files/folders? > You can either
+`CTRL + T` or set `tuifi_show_hidden` enviroment variable to `True` How do I
+change the default colors? > [look here for more informations](https://
+github.com/GiorgosXou/TUIFIManager/issues/38) # ð Donation I do really need
+money to survive, I have no job, living in a basement, making things for free,
+because I love to. - [***Paypal Address***](https://www.paypal.com/donate/
 ?hosted_button_id=QNQN23M55EJVS) - ***Monero Address:***
 `897ehhSQJQpGF7tYDhQM51jiX7nnHmzuYAW4q8JGwJxu8JKXvaK6AivCzatuJxnifjZ2qy98ks2g2PhmTaYCMMta2Ga2LJx`
                                  [./TUIFI.png]
-# ð«¶ Special thanks to - [Bryan Lunduke for this article](https://
+# ð«¶ Special thanks to - [@KORBEN for this article](https://korben.info/
+gestionnaire-fichiers-terminal-tuifimanager-multiplateforme-leger-
+personnalisable.html) - [Bryan Lunduke for this article](https://
 lunduke.substack.com/p/tuifi-manager-a-file-manager-in-the) - [Brodie Robertson
 for this video](https://youtu.be/9laxdMKTZLA) - [r/linux community for their
 comments](https://www.reddit.com/r/linux/comments/zzf5rx) - [r/cyberDeck
 community for their comments](https://www.reddit.com/r/cyberDeck/comments/
 zttur0) - [r/commandline community for their comments](https://www.reddit.com/
-r/commandline/comments/zt30v9) # ð³ï¸ Help Any Idea with this issue https://
-github.com/unicurses/unicurses/issues/21 ?
+r/commandline/comments/zt30v9) # ð³ï¸ Outro - Any Idea with this issue
+https://github.com/unicurses/unicurses/issues/21 ? - Btw I use TUIFI in a daily
+basis. As crazy as it might sound: It's my primary file manager.
```

### Comparing `TUIFIManager-3.3.5/TUIFI.png` & `TUIFIManager-4.0.0/TUIFI.png`

 * *Files identical despite different names*

### Comparing `TUIFIManager-3.3.5/TUIFIManager/TUIFIProfile.py` & `TUIFIManager-4.0.0/TUIFIManager/TUIFIProfile.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,26 @@
 TUIFIProfiles = { # TODO: ADD gitignore and etc. icons | TODO: open zip rar and etc. files on __init__.py as if they where kind of folders?
     ':folder':TUIFIProfile(( # TODO: change folder and empty_folder to something containing illegal characters because if someone names a hidden file that way, there will be a conflict 2022-12-19 09:16:13 PM
         ' █████▒⎫⎫ \n'
         ' █████▒▐┇ \n'
         ' █████▒▐┃ \n'
         ' ▀▀▀▀▀  ┘ '
     ),2),
+    ':folder_subfolder':TUIFIProfile((
+        ' █████░⎫⎫ \n'
+        ' █████░▐┇ \n'
+        ' █████░▐┃ \n'
+        ' ▀▀▀▀▀  ┘ '
+    ),2),
+    ':folder_single_file':TUIFIProfile((
+        ' █████░⎫⎫ \n'
+        ' █████░┇┃ \n'
+        ' █████░┃┃ \n'
+        ' ▀▀▀▀▀  ┘ '
+    ),2),
     ':empty_folder':TUIFIProfile((
         ' █████ ⎫⎫ \n'
         ' █████ ┇┇ \n'
         ' █████ ┃┃ \n'
         ' ▀▀▀▀▀  ┘ '
     ),2),
     ':file':TUIFIProfile((
@@ -119,14 +131,20 @@
 
     '/ino':TUIFIProfile((
         ' ┏┳┳┳━━━╮ \n'
         ' ┇ARDINO┃ \n'
         ' ┃━ ┗┛+┓┃ \n'
         ' ╰┻━━┻┻┻┛ '
     ),4, DEFAULT_EDITOR),
+    '/o':TUIFIProfile((
+        ' ┏━━━━━━┓ \n'
+        ' ┇ █▀▀█ ┃ \n'
+        ' ┃ █▄▄█ ┃ \n'
+        ' ┗━━━━━━┛ '
+    ),1, DEFAULT_OPENER),
     '/h':TUIFIProfile((
         ' ┏━━━━━━┓ \n'
         ' ┇ █▂▂█ ┃ \n'
         ' ┃ █▔▔█ ┃ \n'
         ' ┗━━━━━━┛ '
     ),2, DEFAULT_EDITOR),
     '/c':TUIFIProfile((
@@ -181,19 +199,37 @@
     '/vbs':TUIFIProfile((
         '▃ ▃ ▃▃  ▃▃\n'
         '█ █ █▃█ █▃\n'
         '▀▃▀ █▃▀ ▃█\n'
         '          '
     ),4, DEFAULT_EDITOR),
     '/apk':TUIFIProfile((
-        ' ▃  ▃▃ ▃ ▃\n'
-        '█▃█ ██ █▃▀\n'
-        '█ █ █  █ █\n'
-        '          '
+        ' ┏▅▅▅▅▅▅┓ \n'    # ' ▃  ▃▃ ▃ ▃\n'
+        ' ┇┏┓┏┓┒┒┇ \n'    # '█▃█ ██ █▃▀\n'
+        ' ┃┣┫┣┛┣┓┃ \n'    # '█ █ █  █ █\n'
+        ' ┗━━━━━━┛ '      # '          '
     ),5, DEFAULT_OPENER),
+    '/adb':TUIFIProfile((
+        ' ┏━━━┏━━┓ \n'
+        ' ┇┏┓┏┇┏┓┇ \n'
+        ' ┃┣┫┇┛┣┫┃ \n'
+        ' ┗━━┛━━━┛ '
+    ),4, DEFAULT_EDITOR),
+    '/ads':TUIFIProfile((
+        ' ┏━━━┏━━┓ \n'
+        ' ┇┏┓┏┇┏┓┇ \n'
+        ' ┃┣┫┇┛DS┃ \n'
+        ' ┗━━┛━━━┛ '
+    ),8, DEFAULT_EDITOR),
+    '/lisp':TUIFIProfile((
+        ' ╭┳━┳━━┓╮ \n'
+        ' │┣━┛┏━┓│ \n'
+        ' │┗━┛┏━┫│ \n'
+        ' ╰┗━━┻━┻╯ '
+    ),1, DEFAULT_EDITOR),
     '/vim':TUIFIProfile((
         ' ┏━━━━━┳┓ \n'
         ' ┃VI━━━┫┇ \n'
         ' ┃█▀▅▀▄┃┃ \n'
         ' ╰━━━━━┻┛ '
     ),5, DEFAULT_EDITOR),
     '/md':TUIFIProfile((
@@ -278,14 +314,20 @@
     ),1, DEFAULT_EDITOR),
     '/pyw':TUIFIProfile((
         ' ▃▃▃ ▃ ▃. \n'
         ' █▃█▒█▃█▒ \n'
         ' █▒.wW.█▒ \n'
         '          '
     ),1, DEFAULT_EDITOR),
+    '/tex':TUIFIProfile((
+        ' ┏┏┏┏━━━┓ \n'
+        ' ┃┃┏┓┳┏━┃ \n'
+        ' ┃┇┣┫┃EX┃ \n'
+        ' ┗━━━━━━┛ '
+    ),1, DEFAULT_EDITOR),
     '/txt':TUIFIProfile((
         ' ┏━━┓┓┓┓┓ \n'
         ' ┃┏┇┃☵☲┃┇ \n'
         ' ┃┇┛┃☲☵┃┃ \n'
         ' ┗━━┛━━┛┛ '
     ),1, DEFAULT_EDITOR),
     '/log':TUIFIProfile((
@@ -310,17 +352,17 @@
         ' ╭━━━━╮╮╮ \n'
         ' ┃SCS┃▅▅┃ \n'
         ' ┃┇▒▒┃S☲┃ \n'
         ' ┗━━━╯━━╯ '
     ),2, DEFAULT_EDITOR),
     '/pdf':TUIFIProfile((
         ' ╭━━━━╮━╮ \n'
-        ' ┃PDF┃==│ \n'
-        ' ┃┇▒█┃▒▒│ \n'
-        ' ┗━━━━━━╯ '
+        ' │PDF┃==│ \n'
+        ' │┇▒▓┃▒▒│ \n'
+        ' ╰━━━━━━╯ '
     ),3, DEFAULT_OPENER),
 
 
     '/stl':TUIFIProfile((
         ' ╭─╭┰─╮─╮ \n'
         ' │╭╰┸─╯╮│ \n'
         ' │╰.STL╯│ \n'
@@ -387,54 +429,54 @@
         ' │D│L┠│L│ \n'
         ' │▒│█┠│▒│ \n'
         ' ╰━╰━┹╰━╯ '
     ),2, DEFAULT_OPENER),
 
 
     '/rar':TUIFIProfile((
-        ' ▃▃RAR▃▃╮ \n'
+        ' ▃▃RAR▃▃┓ \n'
         ' ▒▒░ ░▒▒┃ \n'
         ' ▓▓░ ░▓▓┃ \n'
-        ' ▀▀░ ░▀▀┘ '
+        ' ▀▀───▀▀┛ '
     ),2, DEFAULT_OPENER),
     '/zip':TUIFIProfile((
-        ' ▃▃▃░░▃▃▃ \n'
-        ' ▒▒▒░░▒▒▒ \n'
-        ' ▓▓▓░░▓▓▓ \n'
-        ' ZIP░░▀▀▀ '
+        ' ▃▃▃┃┓▃▃▃ \n'
+        ' ▒▒▒┃┃▒▒▒ \n'
+        ' ▓▓▓┃┃▓▓▓ \n'
+        ' ZIP┗┃▀▀▀ '
     ),2, DEFAULT_OPENER),
     '/tar':TUIFIProfile((
-        ' ▃▃▃░░▃▃▃ \n'
-        ' ▒▒▒░░▒▒▒ \n'
-        ' ▓▓▓░░▓▓▓ \n'
-        ' TAR░░▀▀▀ '
+        ' ▃▃▃┏┓▃▃▃ \n'
+        ' ▒▒▒┣┫▒▒▒ \n'
+        ' ▓▓▓┣┫▓▓▓ \n'
+        ' TAR┗┛▀▀▀ '
     ),2, DEFAULT_OPENER),
     '/gz':TUIFIProfile((
-        ' ▃▃▃░░▃▃▃ \n'
-        ' ▒▒▒░░▒▒▒ \n'
-        ' ▓▓▓░░▓▓▓ \n'
-        ' GZ▀░░▀▀▀ '
+        ' ▃▃▃┏┓▃▃▃ \n'
+        ' ▒▒▒┃┃▒▒▒ \n'
+        ' ▓▓▓┃┃▓▓▓ \n'
+        ' GZ▀┗┛▀▀▀ '
     ),2, DEFAULT_OPENER),
     '/xz':TUIFIProfile((
-        ' ▃▃▃░░▃▃▃ \n'
-        ' ▒▒▒░░▒▒▒ \n'
-        ' ▓▓▓░░▓▓▓ \n'
-        ' XZ▀░░▀▀▀ '
+        ' ▃▃▃┏┓▃▃▃ \n'
+        ' ▒▒▒┃┃▒▒▒ \n'
+        ' ▓▓▓┃┃▓▓▓ \n'
+        ' XZ▀┗┛▀▀▀ '
     ),2, DEFAULT_OPENER),
     '/bz2':TUIFIProfile((
-        ' ▃▃▃░░▃▃▃ \n'
-        ' ▒▒▒░░▒▒▒ \n'
-        ' ▓▓▓░░▓▓▓ \n'
-        ' BZ2░░▀▀▀ '
+        ' ▃▃▃┏┓▃▃▃ \n'
+        ' ▒▒▒┃┃▒▒▒ \n'
+        ' ▓▓▓┃┃▓▓▓ \n'
+        ' BZ2┗┛▀▀▀ '
     ),2, DEFAULT_OPENER),
     '/zst':TUIFIProfile((
-        ' ▃▃▃░░▃▃▃ \n'
-        ' ▒▒▒░░▒▒▒ \n'
-        ' ▓▓▓░░▓▓▓ \n'
-        ' ZST░░▀▀▀ '
+        ' ▃▃▃┏┓▃▃▃ \n'
+        ' ▒▒▒┃┃▒▒▒ \n'
+        ' ▓▓▓┃┃▓▓▓ \n'
+        ' ZST┗┛▀▀▀ '
     ),2, DEFAULT_OPENER),
 
 
     '/gif':TUIFIProfile((
         ' ┍━━━┳┳┳┓ \n'
         ' │GIF:∵◖┇ \n'
         ' ┝┓░▃_▓▆┇ \n'
@@ -446,14 +488,22 @@
         ' ╭──────╮ \n'
         ' │TORENT│ \n'
         ' │░▓██▓░│ \n'
         ' ╰━━━━━━╯ '
     ),5, DEFAULT_OPENER),
 
 
+    '/desktop':TUIFIProfile((
+        ' ╭──────╮ \n'
+        ' │.:||[]│ \n'
+        ' │[][][]│ \n'
+        ' ╰━━━━━━╯ '
+    ),1, DEFAULT_OPENER),
+
+
     '/mp4':TUIFIProfile((
         ' ┏┳┳┳┳┳┳┓ \n'
         ' ┇MP4∴∵◖┇ \n'
         ' ┇_░▃_▓▆┇ \n'
         ' ┗┻┻┻┻┻┻┛ '
     ),2, DEFAULT_OPENER),
     '/mkv':TUIFIProfile((
@@ -531,83 +581,83 @@
         ' ┃▓█┣━╋━┫ \n'
         ' ┇EXE━┻━┫ \n'
         ' ╰━━┻━━━┛ '
     ),1, DEFAULT_OPENER),
 
 
     '/jpg':TUIFIProfile((
-        ' ┏━━━JPG╮ \n'
-        ' ┇*.∴:∵◖┃ \n'
-        ' ┣┓░▃┏▓▆┇ \n'
+        ' ┍━━━JPG╮ \n'
+        ' │*.∴:∵◖┃ \n'
+        ' ┝┓░▃┏▓▆┇ \n'
         ' ╰━━━━━━┛ '
     ),2, DEFAULT_OPENER),
     '/png':TUIFIProfile((
-        ' ┏━━━PNG╮ \n'
-        ' ┇*.∴:∵◖┃ \n'
-        ' ┣┓░▃┏▓▆┇ \n'
+        ' ┍━━━PNG╮ \n'
+        ' │*.∴:∵◖┃ \n'
+        ' ┝┓░▃┏▓▆┇ \n'
         ' ╰━━━━━━┛ '
     ),2, DEFAULT_OPENER),
     '/ico':TUIFIProfile((
-        ' ┏━━━ICO╮ \n'
-        ' ┇*.∴:∵◖┃ \n'
-        ' ┣┓░▃┏▓▆┇ \n'
+        ' ┍━━━ICO╮ \n'
+        ' │*.∴:∵◖┃ \n'
+        ' ┝┓░▃┏▓▆┇ \n'
         ' ╰━━━━━━┛ '
     ),2, DEFAULT_OPENER),
     '/jpeg':TUIFIProfile((
-        ' ┏━━JPEG╮ \n'
-        ' ┇*.∴:∵◖┃ \n'
-        ' ┣┓░▃┏▓▆┇ \n'
+        ' ┍━━JPEG╮ \n'
+        ' │*.∴:∵◖┃ \n'
+        ' ┝┓░▃┏▓▆┇ \n'
         ' ╰━━━━━━┛ '
     ),2, DEFAULT_OPENER),
     '/bmp':TUIFIProfile((
         ' ┏━━━BMP┓ \n'
         ' ┇*.∴:∵◖┃ \n'
         ' ┣┓░▃┏▓▆┇ \n'
         ' ┗━━━━━━┛ '
     ),2, DEFAULT_OPENER),
     '/webp':TUIFIProfile((
-        ' ┏━━WEBP╮ \n'
-        ' ┇*.∴:∵◖┃ \n'
-        ' ┣┓░▃┏▓▆┇ \n'
+        ' ┍━━WEBP╮ \n'
+        ' │*.∴:∵◖┃ \n'
+        ' ┝┓░▃┏▓▆┇ \n'
         ' ╰━━━━━━┛ '
     ),2, DEFAULT_OPENER),
     '/tiff':TUIFIProfile((
-        ' ┏━━TIFF╮ \n'
-        ' ┇*.∴:∵◖┃ \n'
-        ' ┣┓░▃┏▓▆┇ \n'
+        ' ┍━━TIFF╮ \n'
+        ' │*.∴:∵◖┃ \n'
+        ' ┝┓░▃┏▓▆┇ \n'
         ' ╰━━━━━━┛ '
     ),2, DEFAULT_OPENER),
     '/tif':TUIFIProfile((
-        ' ┏━━TIFF╮ \n'
-        ' ┇*.∴:∵◖┃ \n'
-        ' ┣┓░▃┏▓▆┇ \n'
+        ' ┍━━TIFF╮ \n'
+        ' │*.∴:∵◖┃ \n'
+        ' ┝┓░▃┏▓▆┇ \n'
         ' ╰━━━━━━┛ '
     ),2, DEFAULT_OPENER),
     '/tga':TUIFIProfile((
-        ' ┏━TARGA╮ \n'
-        ' ┇*.∴:∵◖┃ \n'
-        ' ┣┓░▃┏▓▆┇ \n'
+        ' ┍━TARGA╮ \n'
+        ' │*.∴:∵◖┃ \n'
+        ' ┝┓░▃┏▓▆┇ \n'
         ' ╰━━━━━━┛ '
     ),2, DEFAULT_OPENER),
     '/heif':TUIFIProfile((
-        ' ┏━━HEIF╮ \n'
-        ' ┇*.∴:∵◖┃ \n'
-        ' ┣┓░▃┏▓▆┇ \n'
+        ' ┍━━HEIF╮ \n'
+        ' │*.∴:∵◖┃ \n'
+        ' ┝┓░▃┏▓▆┇ \n'
         ' ╰━━━━━━┛ '
     ),2, DEFAULT_OPENER),
     '/heifs':TUIFIProfile((
-        ' ┏━━HEIF╮ \n'
-        ' ┇*.∴:∵◖┃ \n'
-        ' ┣┓░▃┏▓▆┇ \n'
+        ' ┍━━HEIF╮ \n'
+        ' │*.∴:∵◖┃ \n'
+        ' ┝┓░▃┏▓▆┇ \n'
         ' ╰━━━━━━┛ '
     ),2, DEFAULT_OPENER),
     '/heic':TUIFIProfile((
-        ' ┏━━HEIC╮ \n'
-        ' ┇*.∴:∵◖┃ \n'
-        ' ┣┓░▃┏▓▆┇ \n'
+        ' ┍━━HEIC╮ \n'
+        ' │*.∴:∵◖┃ \n'
+        ' ┝┓░▃┏▓▆┇ \n'
         ' ╰━━━━━━┛ '
     ),2, DEFAULT_OPENER),
 
 
     '/m4a':TUIFIProfile((  # 8 = Aqua, just like the waves
         ' ┏━━━━━━╮ \n'
         ' ┇.:.M4A┫ \n'
@@ -637,30 +687,37 @@
         ' ┇.:.AAC┫ \n'
         ' ╋┻╋┻╋┻━┇ \n'
         ' ┗━━━━━━┛ '
     ),8, DEFAULT_OPENER),
 
 
     '/psd':TUIFIProfile((
-        ' ┏▃▃▃▃▃▃┓ \n'
-        ' ┃█▂█▒▃▃┃ \n'
-        ' ┃█  ▃▃▒┃ \n'
+        ' ┏━━━━━━┓ \n'
+        ' ┇PHSHOP┃ \n'
+        ' ┣┓░▃┏▓▆┇ \n'
         ' ┗━━━━━━┛ '
     ),4, DEFAULT_OPENER),
 
+
+    '/sqlite3':TUIFIProfile((
+        ' ┏━━━━━━  \n'
+        ' ┃SQL┏▄ ┇ \n'
+        ' ┇█▓░┣┻▄┃ \n'
+        ' ┗━━ ▀  ┛ '
+    ),8, DEFAULT_EDITOR),
     '/mdf':TUIFIProfile((
         ' ┏━━━━━━  \n'
         ' ┃MDF┏▄ ┇ \n'
-        ' ┇█▓░┣┻▄┇ \n'
+        ' ┇█▓░┣┻▄┃ \n'
         ' ┗━━ ▀  ┛ '
     ),8, DEFAULT_EDITOR),
     '/db':TUIFIProfile((
         ' ┏━━┳━━━  \n'
-        ' ┃DB┃┏▄ ┇ \n'
-        ' ┇█▓░┣┻▄┇ \n'
+        ' ┃DB┇┏▄ ┇ \n'
+        ' ┇▓░ ┣┻▄┃ \n'
         ' ┗━━ ▀  ┛ '
     ),8, DEFAULT_EDITOR),
 
 
     '/tuifi':TUIFIProfile((
         '             \                                      [            \n'
         '              @                 ⟡                  ╢             \n'
@@ -735,7 +792,9 @@
         '⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠹⣿⠀⠀⠀⠀\n'
         '⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀ ⠀⠀⠀⠀⠁⠀⠀⠀'
     ),8)
 }
 DEFAULT_PROFILE   = TUIFIProfiles[':file']
 LINK_SYMBOL       = '↩'  # Potential:⤶ ⤾ ↲ ⎌ ☍ ⧉
 LINK_SYMBOL_COLOR = 1
+
+#TODO: Overide profiles from external file | I'll do it, don't do it!
```

### Comparing `TUIFIManager-3.3.5/TUIFIManager/TUItilities.py` & `TUIFIManager-4.0.0/TUIFIManager/TUItilities.py`

 * *Files 5% similar despite different names*

```diff
@@ -72,26 +72,45 @@
 
 class Parent:
     def __init__(self,win):
         self.win = win
         self.lines, self.columns = uc.getmaxyx(self.win)
 
 
+
+# # mapping function values 0-255 to 0-1000
+# C = lambda x: int((x - 0) * (1000 - 0) / (255 - 0) + 0)
+
 MY_COLOR_PAIRS = (
     (uc.COLOR_WHITE  ,uc.COLOR_BLACK  ),
     (uc.COLOR_YELLOW ,uc.COLOR_BLACK  ),
     (uc.COLOR_RED    ,uc.COLOR_BLACK  ),
     (uc.COLOR_BLUE   ,uc.COLOR_BLACK  ),
     (uc.COLOR_GREEN  ,uc.COLOR_BLACK  ),
     (uc.COLOR_BLACK  ,uc.COLOR_WHITE  ),
     (uc.COLOR_BLUE   ,uc.COLOR_WHITE  ),
     (uc.COLOR_CYAN   ,uc.COLOR_BLACK  ),
     (uc.COLOR_BLACK  ,uc.COLOR_YELLOW ),
 )
 
+# DIM_OFFSET    = len(MY_COLOR_PAIRS) +1
+# BRIGHT_OFFSET = len(MY_COLOR_PAIRS) *2 +1
+
+
+initialized = False # Initializing color pairs of (FOREGROUND, BACKGROUND) colors.
+def initialize_colors():
+    global initialized 
+    if initialized: return
+    # if MY_COLORS:
+    #     for i in range(0, len(MY_COLORS)):
+    #         uc.init_color(i+1, *MY_COLORS[i])
+    for i in range(0, len(MY_COLOR_PAIRS)): # if uc.pair_content(i) in ((0,0),(7,0)): # if it exists in some way already | also TODO: https://github.com/GiorgosXou/TUIFIManager/issues/48
+        uc.init_pair(i+1 , *MY_COLOR_PAIRS[i] )
+    initialized = True
+
 
 
 @dataclass
 class Border:
     left                : int = uc.ACS_VLINE
     right               : int = uc.ACS_VLINE
     top                 : int = uc.ACS_HLINE
@@ -116,32 +135,30 @@
 
     def update(self, win):
         self.clear(win)
         self.draw (win)
 
 
 
-class Component():
-    def __init__(self, win, y, x, height, width, anchor, is_focused=False, color_pair_offset=0, iheight=None, iwidth=None, warp=True, border:Border=None) -> None:
+class WindowPad():
+    def __init__(self, win=None, y=0, x=0, height=0, width=0, anchor=(False, False, False, False), is_focused=False, iheight=None, iwidth=None, warp=True, border:Border=None) -> None:
         self.pad               = uc.newpad(height, width)
         self.parent            = Parent(win or uc.stdscr)
         self.position          = Position (y, x)
         self.size              = Size(height, width, iheight or height, iwidth or width)
         self.anchor            = Anchor   (*anchor)
         self.is_focused        = is_focused
-        self.color_pair_offset = color_pair_offset
         self.warp              = warp
         self.border            = border # TODO: to check
-        if border: self.border.draw(self.pad)
-        for i in range(1, 10):                                            # Initializing color pairs of (FOREGROUND, BACKGROUND) colors.
-            if uc.pair_content(i+color_pair_offset) in ((0,0),(7,0)):     # if it exists in some way | also TODO: https://github.com/GiorgosXou/TUIFIManager/issues/48
-                uc.init_pair(i+color_pair_offset, *MY_COLOR_PAIRS[i-1] )
+        # if border: self.border.draw(self.pad)
+        initialize_colors()
 
 
     def refresh(self, redraw_parent=False):
+        if self.border: self.border.update(self.pad)
         if redraw_parent:
             uc.touchwin(self.parent.win) # Do i need this? YES
         uc.wrefresh(self.parent.win) # Do i need this? YES | IMPORTANT: wrefresh works only with windows, not pads also look at https://stackoverflow.com/a/35351060/11465149
         uc.prefresh(self.pad, self.position.iy, self.position.ix, self.position.y, self.position.x, self.position.y + self.size.height -1, self.position.x + self.size.width -1)
 
 
     @property #TODO: ADD descrition like use `self.position.x` instead if you don't want to redraw the `parent.win` immediately after
@@ -239,32 +256,32 @@
 
 
     def handle_events(self, event, redraw_parent=True):
         if event == uc.KEY_RESIZE: self.handle_resize(redraw_parent)
 
 
 
-class Label(Component):
+class Label(WindowPad): # TODO: make components a type of Drawables\components rather than a WindowPad
     __text     = ''
     style      = uc.A_NORMAL
     color_pair = 2
 
-    def __init__(self,y=0, x=0, height=1, width=45, anchor=(False, False, False, False), text='', color_pair_offset=0, win=None) -> None:
-        super().__init__(win, y, x, height, width, anchor, color_pair_offset)
+    def __init__(self,y=0, x=0, height=1, width=45, anchor=(False, False, False, False), text='', win=None) -> None:
+        super().__init__(win, y, x, height, width, anchor)
         self.text       = text
 
 
     @property
     def text(self): return self.__text
 
     @text.setter
     def text(self, text):
         self.__text = text
-        uc.mvwaddstr(self.pad,0,0, ' '*self.width, uc.color_pair(self.color_pair+self.color_pair_offset) | self.style )
-        uc.mvwaddstr(self.pad,0,0, text, uc.color_pair(self.color_pair+self.color_pair_offset) | self.style )
+        uc.mvwaddstr(self.pad,0,0, ' '*self.width, uc.color_pair(self.color_pair) | self.style )
+        uc.mvwaddstr(self.pad,0,0, text, uc.color_pair(self.color_pair) | self.style )
 
 
     def handle_resize(self, redraw_parent=True):
         super().handle_resize(redraw_parent)
         self.text = self.__text
```

### Comparing `TUIFIManager-3.3.5/TUIFIManager/__init__.py` & `TUIFIManager-4.0.0/TUIFIManager/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,26 +8,26 @@
 from         typing import Optional, Final
 from           time import time
 from             os import sep, access, W_OK
 from           math import log10
 from        os.path import basename
 from       .TUIMenu import TUIMenu
 from       .TUIFile import TUIFile
-from   .TUItilities import Component, Cd, Label, END_MOUSE, BEGIN_MOUSE, BEGIN_MOUSE, END_MOUSE, IS_WINDOWS, HOME_DIR, IS_TERMUX   
+from   .TUItilities import WindowPad, Cd, Label, END_MOUSE, BEGIN_MOUSE, BEGIN_MOUSE, END_MOUSE, IS_WINDOWS, HOME_DIR, IS_TERMUX
 from  .TUIFIProfile import TUIFIProfiles, DEFAULT_PROFILE , DEFAULT_WITH, DEFAULT_OPENER
 import   subprocess
 import    unicurses
 import       shutil
 import       signal
 import         json
 import          ast
 import           re
 import           os
 
-__version__: Final[str] = "3.3.5"
+__version__: Final[str] = "4.0.0"
 
 PADDING_LEFT   = 2
 PADDING_RIGHT  = 2
 PADDING_TOP    = 1
 PADDING_BOTTOM = 0
 
 SCROLL_SENSITIVITY      = int(os.getenv('tuifi_scroll_sensitivity'     , 1))
@@ -38,14 +38,22 @@
 CTRL_UP        = - CTRL_SCROLL_SENSITIVITY
 CTRL_DOWN      =   CTRL_SCROLL_SENSITIVITY
 
 CONFIG_PATH    = os.getenv('tuifi_config_path',f'{HOME_DIR}{sep}.config{sep}tuifi')
 STTY_EXISTS    = shutil.which('stty')
 INIT_DIRECTORY = os.getcwd()
 
+IS_DRAG_N_DROP = os.getenv('tuifi_synth_dnd') == 'True'
+if IS_DRAG_N_DROP: 
+    from   .TUISynthXDND  import SyntheticXDND
+    from   PySide6.QtCore import QUrl
+    import requests
+    import mimetypes
+    import base64
+
 
 def stty_a(key=None):  # whatever [...]
     if not STTY_EXISTS:
         return None
 
     if not key:
         return [s.strip() for s in subprocess.Popen("stty -a", shell=True, stdout=subprocess.PIPE).stdout.read().decode().split(';')[4:-3]] # risky? i've no idea.. thats why i've not done the same when "if key:"
@@ -53,15 +61,15 @@
     for sig in subprocess.Popen("stty -a", shell=True, stdout=subprocess.PIPE).stdout.read().decode().split(';'):
         if sig.endswith(key):
             return sig.split('=')[0].strip()
     return None
 
 
 
-class TUIFIManager(Component, Cd):  # TODO: I need to create a TUIWindowManager class where i will manage all the anchor, resizing and positional stuff for future components (something like Visual-Studio's c#/vb's Winform's behaviour)
+class TUIFIManager(WindowPad, Cd):  # TODO: I need to create a TUIWindowManager class where i will manage all the anchor, resizing and positional stuff for future components (something like Visual-Studio's c#/vb's Winform's behaviour)
     """
     parent     (       win      ): Parent windows in which the Filemanager-pad is hosted.
     pad        ( Window pointer ): The window/Pad where the manager is hosted.
     anchor     ((bool), optional): Anchor refers to the position the Manager window has relative to the edges of the parent one. [top, bottom, left, right]
     y          (int   , optional): y-axis position of pad. Defaults to 0.
     x          (int   , optional): x-axis position of pad. Defaults to 0.
     directory  (str   , optional): Initital directory. Defaults to HOME_DIR which is $HOME or $UserProfile
@@ -69,92 +77,125 @@
     sort_by    ([type], optional): [Not implemented yet]. Defaults to None.
     has_label  (bool  , optional): Creates a Label which displays informations about files
     draw_files (bool  , optional): "draws" files the moment of initialization (must unicurses.prefresh to show). Defaults to True.
     termux_touch_only      (bool, optional): if true: full touch, no mouse support else: full mouse half touch support. Defaults to True.
     auto_find_on_typing    (bool, optional): if true: when starting to type, automatically search else only if CTRL_F
     auto_command_on_typing (bool, optional): if true: when starting to type, automatically performs a command else only if space key is pressed
     vim_mode   (bool  , optional): If True: uses vim like keys to navigate. Defaults to False.
-    color_pair_offset   (int,  optional): Initializes\\Uses color-pairs from the offset an on | `unicurses.COLOR_PAIR(color_pair...+i)`
     is_focused (bool , optional): disables events
     cd         (bool , optional): cd or not to the current directory on exit (Doesn't support windows yet)
     show_hidden(bool , optional): Show hidden files (you can toggle them by using CTRL+H or use tuifi_show_hidden)
     """
 
     files              = []
-    pad                = None  # for now only pads
     directory          = sep
     __count_selected   = 0
     double_click_DELAY = 0.4
     vim_mode           = False
     info_label         = None
 
-    def __init__(self, y=0, x=0, height=30, width=45, anchor=(False,False,False,False), directory=HOME_DIR, suffixes=[], sort_by=None, has_label=True, win=None, draw_files=True, termux_touch_only=True, auto_find_on_typing=True, auto_cmd_on_typing=False, vim_mode=False, color_pair_offset=0, is_focused=False, cd=False, show_hidden=False):
+    def __init__(self, y=0, x=0, height=30, width=45, anchor=(False,False,False,False), directory=HOME_DIR, suffixes=[], sort_by=None, has_label=True, win=None, draw_files=True, termux_touch_only=True, auto_find_on_typing=True, auto_cmd_on_typing=False, vim_mode=False, is_focused=False, cd=False, show_hidden=False):
         if has_label:
             height -= 1
-            self.info_label       = Label(y+height, x, 1, width, (False,anchor[1],anchor[2],anchor[3]), '', color_pair_offset, win)
+            self.info_label       = Label(y+height, x, 1, width, (False,anchor[1],anchor[2],anchor[3]), f' TUIFIManager {__version__} | Powered by uni-curses', win)
             self.info_label.style = unicurses.A_REVERSE | unicurses.A_BOLD
 
-        super().__init__(win, y, x, height, width, anchor, is_focused, color_pair_offset)
+        super().__init__(win, y, x, height, width, anchor, is_focused)
+        self.__order_method      = sort_by
         self.suffixes            = suffixes
         self.draw_files          = draw_files
         self.termux_touch_only   = termux_touch_only
         self.auto_find_on_typing = os.getenv('tuifi_auto_find_on_typing'   , str(auto_find_on_typing)) == 'True' 
         self.auto_cmd_on_typing  = os.getenv('tuifi_auto_command_on_typing', str(auto_cmd_on_typing )) == 'True' 
         self.show_hidden         = os.getenv('tuifi_show_hidden'           , str(    show_hidden    )) == 'True' 
         self.perform_cd          = os.getenv('tuifi_cd_on_exit'            , str(         cd        )) == 'True' 
-        self.menu                = TUIMenu(color_pair_offset=color_pair_offset)
-
+        self.menu                = TUIMenu  (on_choice=self.on_menu_choice ,
+            items=[
+                'Open       │ ENTER' ,
+                'Cut        │ CTRL+X',
+                'Copy       │ CTRL+C',
+                'Paste      │ CTRL+V',
+                'Delete     │ DEL'   ,
+                'Rename     │ CTRL+R',
+                'Reload     │ KEY_F5',
+                'New File   │ CTRL+W',
+                'New Folder │ CTRL+N',
+                'Properties │'      ],
+        )
+        self.load_order  ()
         if directory:
             self.directory = os.path.normpath(directory)
-            self.load_files(directory, suffixes, sort_by)
+            self.load_files(directory, suffixes)
             if draw_files:
                 self.draw()
 
         self.load_markers       ()
         self.load_commands      ()
         self.__set_normal_events()
-        if stty_a('^C') or unicurses.OPERATING_SYSTEM == 'Windows': signal.signal(signal.SIGINT,self.copy) # https://docs.microsoft.com/en-us/windows/console/ctrl-c-and-ctrl-break-signals
+        if stty_a('^Z')               : signal.signal(signal.SIGTSTP, self.suspend_proccess)
+        if stty_a('^C') or IS_WINDOWS : signal.signal(signal.SIGINT , self.copy            ) # https://docs.microsoft.com/en-us/windows/console/ctrl-c-and-ctrl-break-signals
         if os.getenv('tuifi_vim_mode', str(vim_mode)) == 'True'   : self.toggle_vim_mode()
+        if IS_DRAG_N_DROP: self.drag_and_drop = SyntheticXDND(self.handle_gui_to_tui_dropped_file, self.__get_selected_files) #NOTE: https://stackoverflow.com/a/14829479/11465149
+
+
+    def suspend_proccess(self, signum, frame): # Kinda SuS but you know the deal...
+        print(END_MOUSE)
+        with self.suspend():
+            os.kill(os.getpid(), signal.SIGSTOP)
+        print(BEGIN_MOUSE)
+        unicurses.clear()
 
 
+    if IS_DRAG_N_DROP:
+        def __handle_garbage(self): self.__del__()
+
     def __del__(self):
         self.save_markers()
+        self.save_order  ()
 
 
     def __handle_focus_on_previour_dir(self, f, i):
         if self.__is_opening_previous_dir and f.name == self.basename:
             if not IS_TERMUX or not self.termux_touch_only:
                 self.__index_of_clicked_file = i
                 self.__clicked_file = f
+                self.__pre_pressed_file = f # https://github.com/GiorgosXou/TUIFIManager/issues/96
             self.scroll_to_file(f, not IS_TERMUX or not self.termux_touch_only)
             self.__is_opening_previous_dir = False
 
 
     def draw(self):
         unicurses.werase(self.pad)
         #self.refresh()
         if self.maxpLines < self.height:
             self.maxpLines = self.height
         unicurses.wresize(self.pad, self.maxpLines, self.width)
         for i,f in enumerate(self.files):
-            f.draw(self.pad, color_pair_offset=self.color_pair_offset)
+            f.draw(self.pad)
             self.__handle_focus_on_previour_dir(f,i)
 
 
     #def get_TUIFIProfile_by_key(self, key): # https://stackoverflow.com/a/2974082/11465149
         #return next((v for k, v in TUIFIProfiles.items() if (key == k) or (isinstance(k,tuple) and key in k)),FILE_profile)
 
 
     def get_profile(self, file_directory, new=False):
         if os.path.isdir(file_directory):
+            count = 0
             temp_profile = TUIFIProfiles.get(':empty_folder')
             for suffix in ['/', *self.suffixes] if self.suffixes else ['']: # TODO: Make sure there's no Potential Windows issue? 
-                if list(Path(file_directory + sep).glob('*'+suffix)):
-                    temp_profile = TUIFIProfiles.get(':folder')
-                    break
+                for f in Path(file_directory + sep).glob('*'+suffix): # thankfully is a generator
+                    count +=1
+                    if count == 2:
+                        return TUIFIProfiles.get(':folder')
+            if count == 1 : 
+                if os.path.isdir(f):
+                    return TUIFIProfiles.get(':folder_subfolder')
+                else:
+                    return TUIFIProfiles.get(':folder_single_file')
         else:
             file_extension = os.path.splitext(file_directory)[1]
             file_extension = f'/{file_extension[1:]}' if file_extension else basename(file_directory)
             temp_profile   = TUIFIProfiles.get(file_extension.lower(),DEFAULT_PROFILE) # ..[-1] = extension
         return temp_profile
 
 
@@ -216,48 +257,49 @@
         filename     = name
         file_        = TUIFile(filename, self.___y, self.___x, self.get_profile(self.directory + sep + name), is_link=is_link)
         self.files.append(file_)
         self.__set_coordinates(file_)
 
 
     basename = ''
-    def load_files(self, directory, suffixes=[], sort_by=None):  # DON'T load and then don't show :P
+    def load_files(self, directory, suffixes=[]):  # DON'T load and then don't show :P
         directory = os.path.realpath(os.path.normpath(directory))
         if not os.path.isdir(directory):
             raise FileNotFoundError(f'DirectoryNotFound: "{directory}"')
         if not suffixes:
             suffixes = self.suffixes
 
+        order = self.get_order_of(directory)
+        self.is_order_reversed = order[1]
         self.basename = basename(self.directory)
         self.directory = directory
         self.files = []
         self.__reset_coordinates()
         self.__load_file('..')
         os.chdir(directory)
-        for f in sorted(os.listdir(), key=None): # key=os.path.getctime): # os.listdir(directory):
+        for f in sorted(os.listdir(), key=order[0], reverse=order[1]): # key=os.path.getctime): # os.listdir(directory):
             if not self.__is_valid_file(f): continue
             self.__load_file(f)
 
         self.maxpLines = self.___y + self.y if self.__count == 0 else self.___y + self.__max_h + PADDING_TOP + PADDING_BOTTOM + self.y
-        if not self.is_in_find_mode: self.__set_label_text(f'[{len(self.files)-1:04}] {directory}') # just because i know that len is stored as variable,  that's why i don;t count them in for loop
         return self.files
 
 
     def resort(self): #draw_files=True # repeating code but nvm
         """In case of resize, call this function to resort/replace existing files to the new dimensions of pad
 
         Returns:
             list: self.files
         """
         unicurses.werase(self.pad)
 
         self.__reset_coordinates()
         for f in self.files:
             self.__set_coordinates(f, resize=True)
-            f.draw(self.pad,redraw_icon=True, color_pair_offset=self.color_pair_offset)
+            f.draw(self.pad,redraw_icon=True)
 
         #unicurses.wresize(self.pad, self.maxpLines, self.width) # because it works doesn't also mean that i should do it like that
 
         #if self.position.iy >= unicurses.getmaxy(self.pad) - self.height + self.y:
             #self.position.iy = unicurses.getmaxy(self.pad) - self.height
         #if self.height + self.position.iy > y:
         #    self.position.iy -= self.height + self.position.iy - y  # NOT SURE AT ALL BUT IT WORKS LOL, actually NOP ):(
@@ -270,15 +312,15 @@
     def reload(self,draw_files=True, keep_search_results=False):
         if not keep_search_results:
             self.__temp_find_filename = ''
         else:
             self.__keep_search_results = True
         self.position.iy                = 0
         self.__mouse_btn1_pressed_file  = None
-        self.__pre_clicked_file         = None
+        self.__pre_pressed_file         = None
         self.__clicked_file             = None
         self.__index_of_clicked_file    = None
         self.__pre_hov                  = None           
         self.__count_selected           = 0
         self.load_files(self.directory)
         self.__keep_search_results      = False
         if draw_files:
@@ -313,41 +355,42 @@
         else:
             dirs = [directory]
 
         if not dirs: return # Although not needed just in case for other DEFAULT_OPENERs
 
         print(END_MOUSE, end='\r')
         with self.suspend():
-            proc = subprocess.Popen([open_with, *dirs], shell=IS_WINDOWS)
+            proc = subprocess.Popen([open_with, *dirs], shell=IS_WINDOWS) # TODO: optional stdout=subprocess.DEVNULL when I'll add loading TUIFIProfiles from external file ?
             proc.wait()
         print(BEGIN_MOUSE, end='\r')
         self.__set_label_on_file_selection()
         return
 
 
     def __reset_open(self):
-        if self.vim_mode and self.escape_event_consumed and not self.is_in_command_mode: # SuS SuS SuS SuS SuS damn that's so Sus lol
+        if self.vim_mode and self.escape_event_consumed and not self.is_in_command_mode: # SuS SuS SuS SuS SuS damn that's so Sus lol | 2024-04-05 08:48:24 PM this was for keeping search/find/input mode after opening a folder but i didn't like it and removed it
             self.find()
         else:
-            self.is_in_find_mode       = False
-            self.escape_event_consumed = False
+            self.is_in_find_mode       = False # else content
+            self.escape_event_consumed = False # else content
         self.__change_escape_event_consumed = False
         self.is_in_command_mode      = False
         self.__temp_findname         = ''
         self.__temp_find_filename    = '' # Ahh..
         self.__clicked_file          = None
-        self.__pre_clicked_file      = None
+        self.__pre_pressed_file      = None
         self.__index_of_clicked_file = None
         self.__pre_hov               = None
         self.__count_selected        = 0
         self.position.iy             = 0
+        self.__order_method          = None
 
 
     __is_opening_previous_dir = False
-    def open(self, directory, suffixes=[], sort_by=None, _with=None):
+    def open(self, directory, suffixes=[], _with=None):
         """
         `open()` is `load_files()` + `draw()`
         """
         if directory is None or not directory:
             return None
 
         if isinstance(directory, TUIFile):
@@ -362,15 +405,16 @@
         multiple = self.__count_selected > 1
         if not os.path.isdir(directory) or multiple: # if there is at least one file that it is not a directory OR multiple selected files that they are whatever, then: ... (Now it makes sense why `not isdir`)
             prof = f'/{os.path.splitext(directory)[1][1:]}'
             open_with = TUIFIProfiles.get(prof, DEFAULT_PROFILE).open_with
             return self.__try_open_with(directory, open_with, multiple) # TODO: check if the multiple selected files are folders and open them in new tabs
 
         self.__reset_open()
-        self.load_files(directory, suffixes, sort_by)
+        self.load_files(directory, suffixes)
+        if not self.is_in_find_mode: self.__set_label_text(f'[{len(self.files)-1:04}]' + (' [▼] ' if self.is_order_reversed else ' [▲] ') + directory ) # just because i know that len is stored as variable,  that's why i don;t count them in for loop
         self.draw()
         return self.files
 
 
     def refresh(self):
         super().refresh()
         self.menu.refresh()
@@ -396,43 +440,148 @@
         if not return_enumerator:
             return None
         else:
             return None, None
 
 
     def deselect(self,tuifile=None):
-        if not tuifile and self.__count_selected == 1:
-            tuifile = self.__clicked_file
         if not tuifile:
+            if self.__count_selected == 1:
+                tuifile = self.__clicked_file
+            elif self.__count_selected == 0:
+                return
+        if not tuifile: # If after above condtion is still not tuifile:
             for f in self.files:
                 if f.is_selected:
                     f.is_selected = False
-                    f.draw(self.pad, color_pair_offset=self.color_pair_offset)
+                    f.draw(self.pad)
             self.__count_selected = 0 # i can just -= 1 and break it if 0 :P
         elif tuifile.is_selected:
             tuifile.is_selected = False
-            tuifile.draw(self.pad, color_pair_offset=self.color_pair_offset)
+            tuifile.draw(self.pad)
             self.__count_selected -=1
 
 
     def select(self, tuifile):
         if tuifile.is_selected:return
         self.__count_selected +=1
         #for y in range(tuifile.y, tuifile.y + tuifile.profile.height):
         #    mvwchgat(self.pad,y, tuifile.x, tuifile.profile.width,A_REVERSE,7)
         tuifile.is_selected = True
-        tuifile.draw(self.pad, color_pair_offset=self.color_pair_offset)
+        tuifile.draw(self.pad)
 
 
     def select_all_files(self):
         for f in self.files[1:]:
             self.select(f)
         self.__set_label_text(f'[{self.__count_selected}] Files selected')
 
 
+    if IS_DRAG_N_DROP:
+        headers = { # just in case
+            'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/103.0.5060.53 Safari/537.36', 
+            'X-Requested-With': 'XMLHttpRequest'
+        } 
+        def save(self, path, filename, data):
+            try:
+                path = os.path.join(path, filename)
+                f = open(path, 'wb')
+                f.write(data)
+                f.close()
+                # block from create_new()
+                self.__sub_handle_creation_of(filename, self.get_profile(path))
+                self.__set_label_text(f'SAVED: "{filename}"')
+                return True
+            except Exception as e:
+                self.__set_label_text(f"FAILED TO SAVE: { str(e) }")
+                return False
+
+
+        def get_available_filename(self,name):
+            tmp_name = name
+            i = 0
+            while os.path.isfile(self.directory + sep + tmp_name):
+                tmp_name = f'{i}_{name}'
+                i += 1
+            return tmp_name
+
+
+
+        def download(self, url, out_path): # downloading github images from comments or posts seems to have issues ... those https://private-user-images...
+            self.__set_label_text(f'DOWNLOADING: {url}')
+            try:
+                # self.__set_label_text(f'Downloading file ...')
+                r = requests.get(url, headers=self.headers) # , stream=True
+                # if r.headers.get('filename'):pass
+                filename = ''
+                extension = mimetypes.guess_extension(r.headers.get('content-type', '').split(';')[0]) # .split(';') is needed because there might be more after  https://stackoverflow.com/a/59575973/11465149
+                content = r.headers.get('Content-Disposition')
+                if content and not content.find('filename=') == -1:
+                    filename = content.split('filename=')[1].split(';')[0]
+                    if filename[0] in ('"', "'"):
+                        filename = filename[1:-1]
+                    if filename.strip() == '': # This happened with an image dropped from my stackoverflow profile (not the small ones)
+                        filename = 'download'
+                    if extension and filename.find('.') == -1: # hidden filenames without extension might be an issue\get-ignored :P
+                        filename = filename + extension
+                else:
+                    filename = basename(url).split("?")[0].split(".",1)
+                    if extension:
+                        filename = filename[0] + extension
+                    elif len(filename)>1:
+                        filename = filename[0] + "." + filename[1]
+                    else:
+                        filename = "download"
+
+                #TODO: if duplicate display a msg replace or something | or if duplicate check hashes and if the same ignore else ask?
+                filename = self.get_available_filename(filename)
+
+                return self.save(out_path, filename, r.content)
+            except Exception as e:
+                self.__set_label_text(f"FAILD TO DOWNLOAD: { str(e) }")
+                return False
+
+
+
+        def __get_selected_files(self): # I know it's not optimized at all, but ... anyways for now... I have a life too :P
+            if self.__count_selected > 1: # don't simplify the condition cause it doesn't count __pre_pressed_file as selected until it becomes clicked (if i remember well pre_clicked means pressed but not released)
+                f_list = []
+                for f in self.files:
+                    if f.is_selected:
+                        f_list.append(QUrl.fromLocalFile(self.directory + sep + f.name))
+                return f_list
+            elif self.__pre_pressed_file:
+                return [QUrl.fromLocalFile(self.directory + sep + self.__pre_pressed_file.name)]
+
+
+        def handle_gui_to_tui_dropped_file(self, file_url, type): #TODO: Custom user actions on link patterns: eg. clone git, save at folder xy, etc.
+            self.__set_label_text(f'DROPPED: {file_url}')
+            if type == 1:
+                self.__set_label_text("It's on the todo list :P") #TODO: handle files
+            elif type == 0:
+                self.download(file_url, self.directory + sep)
+            elif file_url.startswith('data:') and not file_url.find('base64') == -1:
+                extension = mimetypes.guess_extension(file_url.split(';')[0].split(':')[1])
+                filename = self.get_available_filename('download'+extension)
+                self.save(self.directory, filename, base64.b64decode(file_url[file_url.find('4')+1:])) # 4 is from base64
+            else:
+                self.__set_label_text(f'DROPPED UNHANDLED: {file_url}')
+
+                # r = requests.get(file_url) # , stream=True
+                # r.headers.get('filename')
+                # unicurses.mvwaddwstr(self.pad,0,0,f'is downloadable: {r.headers}')
+
+                # from urllib.request import urlopen 
+                # response = urlopen(file_url)
+                # filename = response.headers.get_filename()
+                # self.__set_label_text(f'{filename} <-----')
+                
+
+
+
     def scroll_pad(self, y):
         if self.position.iy <= 0 and y < 0:
             self.position.iy = 0
             return
         if self.position.iy >= unicurses.getmaxy(self.pad) - self.height  and y > 0:
             self.position.iy = unicurses.getmaxy(self.pad) - self.height
             return
@@ -440,19 +589,95 @@
 
 
     def exit_to_self_directory(self):
         if not IS_WINDOWS and not self.directory == INIT_DIRECTORY:
             self.cd(self.directory)
         print(END_MOUSE)
         unicurses.endwin()
+        if IS_DRAG_N_DROP: self.__handle_garbage()
         exit()
 
 
+    def load_order(self, path=CONFIG_PATH):
+        path = path + sep + 'ORDER.csv'
+        if not os.path.isfile(path) : return
+        tmp_order_methods = {
+            'getctime' : os.path.getctime,
+            'getsize ' : os.path.getsize ,
+            'getatime' : os.path.getatime,
+            'getmtime' : os.path.getmtime,
+            'none'     : None
+        }
+        with open(path, 'r') as file:
+            for d in file:
+                d = d.split(',')
+                self.ordered_dirs[d[0]] = (tmp_order_methods[d[1]], True if d[2][:-1] == 'True' else False) # -1 to remove newline
+
+
+    def save_order(self, path=CONFIG_PATH):
+        if not self.__ordered_dirs_need_saving: return # prevent unnecessary saving
+        with open(path + sep + 'ORDER.csv','w') as fp:
+            for k, v in self.ordered_dirs.items():
+                if os.path.isdir(k):
+                    fp.write(k + ',' + (v[0].__name__ if v[0] else 'none') + f',{v[1]}\n')
+
+
+    def get_order_of(self, directory):
+        tmp_ordered_dir = self.ordered_dirs.get(directory)
+        return (None, False) if not tmp_ordered_dir else tmp_ordered_dir
+
+
+    is_order_reversed = False
+    def ascend_order_switch(self, order_method=None):
+        if not self.is_order_reversed: order_method = self.__order_method
+        self.is_order_reversed = True
+        self.switch_order_method(order_method)
+
+
+    def descend_order_switch(self, order_method=None):
+        if self.is_order_reversed: order_method = self.__order_method
+        self.is_order_reversed = False
+        self.switch_order_method(order_method)
+
+
+    __ordered_dirs_need_saving = False
+    ordered_dirs = {}
+    def switch_order_method(self, order_method=None):
+        self.__ordered_dirs_need_saving = True
+        if order_method: 
+            self.__order_method = order_method
+            self.__set_label_text(('[▼] DESCENDING' if self.is_order_reversed else '[▲] ASCENDING') + ' ORDER')
+        elif self.__order_method == None:
+            self.__order_method = os.path.getctime
+            self.__set_label_text(('[▼]' if self.is_order_reversed else '[▲]') + '[ORDERED] BY CHANGE TIME')
+        elif self.__order_method == os.path.getctime: 
+            self.__order_method = os.path.getsize 
+            self.__set_label_text(('[▼]' if self.is_order_reversed else '[▲]') + '[ORDERED] BY SIZE')
+        elif self.__order_method == os.path.getsize:
+            self.__order_method = os.path.getatime
+            self.__set_label_text(('[▼]' if self.is_order_reversed else '[▲]') + '[ORDERED] BY ACCESS TIME')
+        elif self.__order_method == os.path.getatime:
+            self.__order_method = os.path.getmtime
+            self.__set_label_text(('[▼]' if self.is_order_reversed else '[▲]') + '[ORDERED] BY MODIFICATION TIME')
+        else:
+            self.__order_method = None # oreder default
+            self.__set_label_text(('[▼]' if self.is_order_reversed else '[▲]') + '[ORDERED] BY NAME')
+
+        if not self.is_order_reversed and self.__order_method == None: # prevent default mode to be saved 
+            if self.ordered_dirs.get(self.directory): del self.ordered_dirs[self.directory]
+        else:
+            self.ordered_dirs[self.directory] = (self.__order_method, self.is_order_reversed)
+
+        self.reload()
+
+
+
     is_on_select_mode          = False
     __mouse_btn1_pressed_file  = None
+    __pre_pressed_file         = None
     __pre_clicked_file         = None
     __clicked_file             = None
     __index_of_clicked_file    = None
     __start_time               = 0
     __temp__copied_files       = []
     __temp_dir_of_copied_files = ''
 
@@ -462,14 +687,16 @@
             unicurses.KEY_UP        : self.__perform_key_up             ,
             unicurses.KEY_DOWN      : self.__perform_key_down           ,
             unicurses.KEY_LEFT      : self.__perform_key_left           ,
             unicurses.KEY_RIGHT     : self.__perform_key_right          ,
             unicurses.KEY_BTAB      : self.__perform_key_btab           ,
             unicurses.KEY_DC        : self.delete                       ,
             unicurses.KEY_F(5)      : self.reload                       ,
+            unicurses.KEY_F(3)      : self.descend_order_switch         ,
+            unicurses.KEY_F(1)      : self.ascend_order_switch          ,
             unicurses.CTRL('A')     : self.select_all_files             ,
             unicurses.CTRL('T')     : self.toggle_hidden_files          ,
             unicurses.CTRL('R')     : self.rename                       ,
             unicurses.CTRL('C')     : self.copy                         ,
             unicurses.CTRL('K')     : self.copy                         ,
             unicurses.CTRL('X')     : self.cut                          ,
             unicurses.CTRL('V')     : self.paste                        ,
@@ -483,14 +710,15 @@
             10                      : self.__perform_key_enter          ,
             unicurses.KEY_BACKSPACE : self.__open_previous_dir          ,
             8                       : self.__open_previous_dir          , # https://superuser.com/questions/212874/why-is-backspace-often-represented-with-h | TODO: I might remove it 
             127                     : self.__open_previous_dir          ,
             263                     : self.__open_previous_dir          ,
             unicurses.KEY_RESIZE    : self.__handle_resize_event        ,
             32                      : self.command                      , # SPACEBAR
+            27                      : self.__handle_garbage if IS_DRAG_N_DROP else lambda *args : None #NOTE: https://stackoverflow.com/a/14829479/11465149
         }
 
     def toggle_vim_mode(self): # TODO: Use it in rename and find or something
         if self.vim_mode:
             self.vim_mode = False
             # TODO revert events Map
         else:
@@ -501,23 +729,23 @@
                 unicurses.CCHAR('k') : self.__perform_key_up             ,
                 unicurses.CCHAR('j') : self.__perform_key_down           ,
                 unicurses.CCHAR('h') : self.__perform_key_left           ,
                 unicurses.CCHAR('l') : self.__perform_key_right          ,
                 unicurses.CCHAR('r') : self.rename                       ,
                 unicurses.CCHAR('c') : self.cut                          ,
                 unicurses.CCHAR('p') : self.paste                        ,
-                unicurses.CCHAR('O') : self.__open_DEFAULT_WITH          ,
+                unicurses.CCHAR('o') : self.descend_order_switch         ,
+                unicurses.CCHAR('O') : self.ascend_order_switch          ,
                 unicurses.CCHAR('K') : self.__perform_key_enter          ,
                 unicurses.CCHAR('J') : self.__open_previous_dir          ,
                 unicurses.CCHAR('b') : self.__open_previous_dir          ,
                 unicurses.CCHAR('H') : partial(self.open      , HOME_DIR),
                 unicurses.CCHAR('w') : partial(self.create_new, 'file'  ),
                 unicurses.CCHAR('W') : partial(self.create_new, 'folder'),
                 unicurses.CCHAR('i') : self.find                         ,
-                unicurses.CCHAR('O') : self.__open_DEFAULT_WITH          , # https://stackoverflow.com/a/33966657/11465149
                 unicurses.CCHAR('e') : self.exit_to_self_directory       ,
                 unicurses.CTRL ('D') : self.delete                       ,
             }) # TODO Map  events
 
 
     def toggle_hidden_files(self):
         self.show_hidden = not self.show_hidden
@@ -645,45 +873,54 @@
         if not self.has_write_access(self.directory): return
         if len(self.__temp__copied_files) == 0 or not os.path.exists(self.__temp_dir_of_copied_files): return # u never no if the user deleted anything from other file manager this is also something i haven't consider for the rest of the things and [...]
         if self.__temp_dir_of_copied_files != self.directory: self.__copy_cut ()
         else                                                : self.__duplicate()
         self.reload(keep_search_results=True)
 
 
+    def resort_reset_select(self, i):
+        self.resort() # replaced -> self.reload(keep_search_results=True)
+        self.__index_of_clicked_file = i
+        self.__clicked_file          = self.files[i]
+        self.__pre_pressed_file      = self.files[i]
+        self.__pre_hov               = None           
+        self.select(self.__clicked_file)
+
+
+    def __delete_selected_file(self):
+        # checking under __delete_file too but nvm cause i have no time right now
+        if self.__clicked_file.name == '..': return 0
+        self.__delete_file(self.__clicked_file)
+        del self.files[self.__index_of_clicked_file]
+        return self.__index_of_clicked_file - 1
+
+
+    def __delete_multiple_selected_file(self):
+        i=0
+        while True:
+            if self.files[i].is_selected: # first file is never selected because it is the .. one
+                self.__delete_file(self.files[i])
+                del self.files[i]
+                i-=1
+                if self.__count_selected == 0:
+                    break
+            i+=1
+        return i
+
+
     def delete(self):
         """
         Deletes the selected file(s). | Not fully implemented yet
         """
         if not self.has_write_access(self.directory): return
         if self.__count_selected == 1 and self.__clicked_file :
-            # checking under __delete_file too but nvm cause i have no time right now
-            if self.__clicked_file.name != '..':
-                self.__delete_file(self.__clicked_file)
-                temp_i = self.__index_of_clicked_file - 1
-                self.reload(keep_search_results=True)
-                self.__index_of_clicked_file = temp_i
-                self.__clicked_file          = self.files[temp_i]
-                self.__pre_clicked_file      = None # hmm.. sus?
-                self.select(self.__clicked_file)
+            fi = self.__delete_selected_file()
         else: # if self.__count_selected > 1:  # Why do i even > 1 very sus
-            if self.__clicked_file:
-                temp_i = self.__index_of_clicked_file - self.__count_selected
-            else:
-                temp_i = 0 # VERY SUS BUT NVM NOW
-
-            for f in self.files:
-                if f.is_selected:
-                    self.__delete_file(f)
-                    if self.__count_selected == 0:
-                        self.reload(keep_search_results=True)
-                        self.__index_of_clicked_file = temp_i
-                        self.__clicked_file          = self.files[temp_i]
-                        self.__pre_clicked_file      = None # hmm.. sus
-                        self.select(self.__clicked_file)
-                        break
+            fi = self.__delete_multiple_selected_file()
+        self.resort_reset_select(fi)
 
 
     def load_markers(self, path=CONFIG_PATH):
         path = path + sep + 'MARKERS'
         if not os.path.isfile(path) : return
         with open(path, 'r') as file:
             self.markers = json.load(file)
@@ -710,17 +947,20 @@
     __temp_findname = ''
     def handle_find_events(self,event): # TODO: FIX SUFFIXES WHEN DELETING, find_file
         if event == 27:
             if self.vim_mode:
                 self.__change_escape_event_consumed = True
                 self.is_in_find_mode                = False
                 if self.__temp_findname != '': # When Escaping without searching anything
-                    i = 0 if len(self.files) == 1 else 1
-                    self.__index_of_clicked_file = i
-                    self.__clicked_file          = self.files[i]
+                    if len(self.files) == 1:  # if nothing is found (only folder ".." then reload at cancel)
+                        self.reload()
+                        self.__set_label_text('[NORMAL]')
+                        return False
+                    self.__index_of_clicked_file = 1
+                    self.__clicked_file          = self.files[1]
                 self.__set_label_text('[NORMAL]')
                 return False
             self.clear_find_results()
             return True
         elif event in (unicurses.KEY_BACKSPACE, 8, 127, 263):
             if len(self.__temp_findname) > 1:
                 self.__temp_findname = self.__temp_findname[:-1]
@@ -909,18 +1149,18 @@
         self.__set_label_text('[COMMAND]')
         self.is_in_command_mode    = True
         self.escape_event_consumed = True
         self.__temp_findname = '' # just ot make sure although it might not be need it
 
 
     def rename(self):
-        if self.__clicked_file:
+        if self.__clicked_file and not self.__clicked_file == self.files[0]:
             self.__set_label_text(f'[RENAMING] {self.__clicked_file.name}')
             self.escape_event_consumed = True
-            self.__clicked_file.draw_name(self.pad, self.__clicked_file.name, '', 0, unicurses.A_UNDERLINE, self.color_pair_offset)  # Yeah ok, whatever
+            self.__clicked_file.draw_name(self.pad, self.__clicked_file.name, '', 0, unicurses.A_UNDERLINE)  # Yeah ok, whatever
             self.__temp_name        = self.__clicked_file.name
             self.__temp_pre_name    = self.__temp_name
             self.__first_pass       = True
 
 
     escape_event_consumed          = False
     __first_pass                   = True
@@ -930,20 +1170,21 @@
     __temp_i                       = 0
     __illegal_filename_characters  = ('<', '>', ':',  '/', '\\', '|', '?', '*', '"')
     def handle_rename_events(self, event):  # At this momment i don't even care about optimizing anything... just kidding, you get the point, no free time | TODO: change event == ... to self.events.get(...)
         if event == unicurses.KEY_LEFT:
             if self.__temp_i != 0: self.__temp_i -= 1
         elif event == unicurses.KEY_RIGHT:
             if self.__temp_i != len(self.__temp_name): self.__temp_i += 1
-        elif event in (27, unicurses.KEY_ENTER, 10): # TODO: clicks to act as enter
+        elif event in (27, unicurses.KEY_ENTER, 10) or (event == unicurses.KEY_MOUSE and (self.get_mouse()[5] & unicurses.BUTTON1_PRESSED)) : # TODO: clicks to act as enter
             new_path_name                       = self.directory + sep + self.__temp_name
             self.__temp_i                       = 0
             self.__change_escape_event_consumed = True
             if  event != 27 and self.__temp_name.strip() != '' and not os.path.exists(new_path_name):
                 os.rename(self.directory + sep + self.__clicked_file.name, new_path_name)
+                self.__set_label_text(f'RENAMED: "{self.__clicked_file.name}" to "{self.__temp_name}"')
                 self.__clicked_file.name    = self.__temp_name
                 self.__clicked_file.profile = self.get_profile(new_path_name)
                 self.resort()
                 self.scroll_to_file(self.__clicked_file, True, True)
             else:
                 self.__temp_name = self.__clicked_file.name
         elif unicurses.RCCHAR(event) in self.__illegal_filename_characters or event == unicurses.KEY_MOUSE or unicurses.keyname(event) in ('kxOUT','kxIN'):
@@ -958,41 +1199,47 @@
         elif event == unicurses.KEY_END : self.__temp_i = len(self.__temp_name)
         elif self.__first_pass:
             self.__temp_name = unicurses.RCCHAR(event)
             self.__temp_i += 1
         else:
             self.__temp_name = self.__temp_name[:self.__temp_i] + unicurses.RCCHAR(event) + self.__temp_name[self.__temp_i:]
             self.__temp_i += 1
-        self.__clicked_file.draw_name(self.pad,self.__temp_name,self.__temp_pre_name, self.__temp_i, color_pair_offset=self.color_pair_offset)
+        self.__clicked_file.draw_name(self.pad,self.__temp_name,self.__temp_pre_name, self.__temp_i)
         self.__temp_pre_name = self.__temp_name
         self.__first_pass    = False
         #if event in (unicurses.KEY_BACKSPACE, 8, 127, 263):
         #    pass
 
 
+    def __sub_handle_creation_of(self, filename, profile):
+        self.deselect()
+        self.__clicked_file = TUIFile(filename, profile=profile)
+        self.__pre_pressed_file = self.__clicked_file # https://github.com/GiorgosXou/TUIFIManager/issues/98
+        self.__index_of_clicked_file = self.__index_of_clicked_file if self.__index_of_clicked_file else 1
+        self.files.insert(self.__index_of_clicked_file, self.__clicked_file) # condition added because if self.__index_of_clicked_file is None and create a file it fails
+        self.resort()
+        self.scroll_to_file(self.__clicked_file,True) # removed deselect=True thanks to `self.__index_of_clicked_file =...` but just in case I let this here
+
+
     def create_new(self,_type='folder'): # temporary implementation but nvm
         if not self.has_write_access(self.directory): return
         i, j = '', 0
         exists = os.path.isdir if _type == 'folder' else os.path.isfile
 
         while exists(self.directory + sep + 'New ' + _type + i):
             i = f' ({str(j)})'
             j += 1
         filename = f'New {_type}{i}'
         if _type == 'folder':
             os.mkdir(self.directory + sep + filename)
             _type = 'empty_folder'
         else                :
             open(self.directory + sep + filename, 'w').close()
-        self.deselect()
-        self.__clicked_file = TUIFile(filename, profile=TUIFIProfiles.get(f':{_type}'))
-        self.__index_of_clicked_file = 1
-        self.files.insert(1,self.__clicked_file)
-        self.resort()
-        self.scroll_to_file(self.__clicked_file,True,True)
+
+        self.__sub_handle_creation_of(filename, TUIFIProfiles.get(f':{_type}'))
         self.rename()
 
 
     def create_new_file  (self): self.create_new('file'  )
     def create_new_folder(self): self.create_new('folder')
 
     def __int_len(self, n): # https://stackoverflow.com/a/2189827/11465149
@@ -1008,30 +1255,28 @@
         self.info_label.text = f'[{len(self.files) - 1:04}] [{index}] {path[max(len(path) - self.info_label.width + offset, 0):]} {info}'
         # just because i know that len is stored as variable,  that's why i don;t count them in for loop
 
     def __open_clicked_file(self):
         return self.open(self.__clicked_file)
 
 
-    __menu_select_actions = {
-        'Open'      : __open_clicked_file           ,
-        'Cut'       : cut                           ,
-        'Delete'    : delete                        ,
-        'Copy'      : copy                          ,
-        'Paste'     : paste                         ,
-        'Rename'    : rename                        ,
-        'New File'  : create_new_file               ,
-        'New Folder': create_new_folder             ,
-        'Reload'    : reload                        ,
-    }
-    def __perform_menu_selected_action(self, action):
-        if not action : return False
-        action_func = self.__menu_select_actions.get(action)
-        if action_func: action_func(self) # don't change this, it has to return true even if no action_func() performed else it doesn't overide the events
-        return True
+    __menu_select_actions = (
+        __open_clicked_file           ,
+        cut                           ,
+        copy                          ,
+        paste                         ,
+        delete                        ,
+        rename                        ,
+        reload                        ,
+        create_new_file               ,
+        create_new_folder             ,
+        lambda *args : None 
+    )
+    def on_menu_choice(self, action):
+        self.__menu_select_actions[action](self)
 
 
     def __handle_termux_touch_events(self, bstate, y, x): # termux needs to implement CTRL + CLICK
         if not (bstate & unicurses.BUTTON1_CLICKED or bstate & unicurses.BUTTON1_PRESSED): return False
         self.__index_of_clicked_file, self.__clicked_file = self.get_tuifile_by_coordinates(y, x, return_enumerator=True)
         if not self.is_on_select_mode: self.deselect()
 
@@ -1051,32 +1296,32 @@
     __pre_hov  = None # TODO: clear the value when directory change at open
     def __handle_hover_mode(self, y, x):
         if not self.hover_mode: return
         tmp_id_of_hov_file, tmp_hov_file = self.get_tuifile_by_coordinates(y,x, return_enumerator=True)
         if tmp_hov_file and tmp_id_of_hov_file and not tmp_hov_file.is_selected: 
             self.__set_label_on_file_selection(tmp_id_of_hov_file,tmp_hov_file)
             # tmp_hov_file.is_selected = True
-            tmp_hov_file.draw_effect(self.pad, color_pair_offset=self.color_pair_offset, effect=0)
+            tmp_hov_file.draw_effect(self.pad, effect=0)
             if self.__pre_hov and self.__pre_hov != tmp_hov_file:
                 # self.__pre_hov.is_selected = False
-                self.__pre_hov.draw(self.pad, color_pair_offset=self.color_pair_offset)
+                self.__pre_hov.draw(self.pad)
             self.__pre_hov = tmp_hov_file
         elif self.__pre_hov:
-            self.__pre_hov.draw(self.pad, color_pair_offset=self.color_pair_offset)
+            self.__pre_hov.draw(self.pad)
             self.__pre_hov = None
 
 
 
     __index_of_alt_clicked_file     = None
     __index_of_pressed_file         = None
     def __handle_mouse_events(self, event): # I know it's a messy code ... lol
         if event != unicurses.KEY_MOUSE: return False
         in_range, id, x, y, z, bstate = self.get_mouse()
         if not IS_WINDOWS and not in_range: return True # TODO: https://github.com/GiorgosXou/TUIFIManager/issues/49
-        if self.__perform_menu_selected_action(self.menu.handle_mouse_events(id, x, y, z, bstate)): return True
+        if self.menu.handle_mouse_events(id, x, y, z, bstate): return True
         if self.__x != x or self.__y != y: self.hover_mode = True #hover mode
 
         if   not self.hover_mode and (bstate & unicurses.BUTTON4_PRESSED): self.scroll_pad(UP   if not bstate & unicurses.BUTTON_CTRL else CTRL_UP  )
         elif not self.hover_mode and (bstate & unicurses.BUTTON5_PRESSED): self.scroll_pad(DOWN if not bstate & unicurses.BUTTON_CTRL else CTRL_DOWN)
         elif not IS_TERMUX or not self.termux_touch_only: # because there are some times that long like presses might be translated to BUTTON1_PRESSED instead of CLICK
             self.__handle_hover_mode(y,x)
             if (bstate & unicurses.BUTTON1_RELEASED) or (bstate & unicurses.BUTTON3_RELEASED) or (unicurses.OPERATING_SYSTEM == 'Windows' and bstate & unicurses.BUTTON1_DOUBLE_CLICKED): # unicurses.OPERATING_SYSTEM == 'Windows' because issues with ncurses
@@ -1095,32 +1340,45 @@
                     if not ((bstate & unicurses.BUTTON3_RELEASED) and self.__count_selected > 1 and self.__clicked_file and self.__clicked_file.is_selected):
                         self.menu.delete()
                         self.deselect()
                     if bstate & unicurses.BUTTON3_RELEASED:
                         self.menu.create(y,x)
                     if self.__mouse_btn1_pressed_file and not self.__mouse_btn1_pressed_file.name == '..' and not self.__mouse_btn1_pressed_file.is_selected :
                         self.select(self.__mouse_btn1_pressed_file )
-                    if (((sumed_time < self.double_click_DELAY) and (bstate & unicurses.BUTTON1_RELEASED)) or bstate & unicurses.BUTTON1_DOUBLE_CLICKED) and self.__clicked_file: #and count == 2  :
+                    if (((sumed_time < self.double_click_DELAY) and (bstate & unicurses.BUTTON1_RELEASED) and (self.__pre_clicked_file == self.__clicked_file)) or bstate & unicurses.BUTTON1_DOUBLE_CLICKED) and self.__clicked_file: #and count == 2  :
                         self.open(self.__clicked_file)
-                elif self.__clicked_file and self.__mouse_btn1_pressed_file and not self.__mouse_btn1_pressed_file == self.__clicked_file: #and not self.__clicked_file.is_selected:
-                    if os.path.isdir(self.directory + sep + self.__clicked_file.name) and self.has_write_access(self.directory) and  self.has_write_access(self.directory + sep + self.__clicked_file.name):
-                        for f in self.files:
-                            if f.is_selected:
-                                shutil.move(self.directory + sep + f.name, self.directory + sep + self.__clicked_file.name + sep + f.name)
-                        self.__pre_clicked_file = None
-                        self.reload(keep_search_results=True)
+                elif self.__clicked_file and self.__mouse_btn1_pressed_file and not self.__mouse_btn1_pressed_file == self.__clicked_file and not self.__clicked_file.is_selected: # this `and not self.__clicked_file.is_selected:` was needed because __clicked_file isn't marked as selected until "drop event" ends | tldr prevents from dropping files into itself
+                    if os.path.isdir(self.directory + sep + self.__clicked_file.name) and self.has_write_access(self.directory) and self.has_write_access(self.directory + sep + self.__clicked_file.name):
+                        i=0 # taken from __delete_multiple_selected_file
+                        folder_index = None
+                        while True:
+                            if self.files[i].is_selected: # first file is never selected because it is the .. one
+                                fname = self.files[i].name
+                                shutil.move(self.directory + sep + fname, self.directory + sep + self.__clicked_file.name + sep + fname)
+                                self.__count_selected -=1
+                                del self.files[i]
+                                i-=1
+                                if self.__count_selected == 0 and not folder_index == None:
+                                    break
+                            elif self.files[i] == self.__clicked_file:
+                                folder_index = i
+                                if self.__count_selected == 0:
+                                    break
+                            i+=1
+                        self.resort_reset_select(folder_index)
 
+                self.__pre_clicked_file = self.__clicked_file
                 self.__start_time = time()
             elif (bstate & unicurses.BUTTON1_PRESSED) or (bstate & unicurses.BUTTON3_PRESSED):
                 self.__delay1 = time()
                 self.__index_of_pressed_file, self.__mouse_btn1_pressed_file = self.get_tuifile_by_coordinates(y, x, return_enumerator=True)
 
-                if not bstate & unicurses.BUTTON_CTRL and self.__pre_clicked_file and self.__pre_clicked_file.is_selected:#and summ > self.double_click_DELAY:
+                if not bstate & unicurses.BUTTON_CTRL and self.__pre_pressed_file and self.__pre_pressed_file.is_selected:#and summ > self.double_click_DELAY:
                     if self.__count_selected == 1:
-                        self.deselect(self.__pre_clicked_file)
+                        self.deselect(self.__pre_pressed_file)
                         self.menu.delete()
                 if bstate & unicurses.BUTTON_ALT or bstate & unicurses.BUTTON_SHIFT: 
                         self.deselect()
 
                 if self.__mouse_btn1_pressed_file and self.__mouse_btn1_pressed_file.name != '..':
                     if not self.__mouse_btn1_pressed_file.is_selected and not (bstate & unicurses.BUTTON3_PRESSED):
                         if (bstate & unicurses.BUTTON_ALT or bstate & unicurses.BUTTON_SHIFT) and self.__index_of_alt_clicked_file:
@@ -1129,15 +1387,15 @@
                             for f in self.files[start:end+1]: # __index_of_alt_clicked_file acts as the index of the pre-clicked file | that "+1" it's so weird....
                                 self.select(f)
                             # self.select(self.files[end])
                         self.select(self.__mouse_btn1_pressed_file)
                     elif bstate & unicurses.BUTTON_CTRL :#and summ > self.double_click_DELAY:
                         self.deselect(self.__mouse_btn1_pressed_file)
 
-                self.__pre_clicked_file = self.__mouse_btn1_pressed_file
+                self.__pre_pressed_file = self.__mouse_btn1_pressed_file
         else: self.__handle_termux_touch_events(bstate, y, x)
 
         self.__x, self.__y = x,y
         self.hover_mode = False
         return True
 
 
@@ -1217,15 +1475,15 @@
 
 
     def __change_index_of_clicked_file(self, index: int) -> None:
         self.deselect()
         self.__index_of_clicked_file   = index
         self.__clicked_file            = self.files[index]
         self.__mouse_btn1_pressed_file = self.__clicked_file
-        self.__pre_clicked_file        = self.__clicked_file
+        self.__pre_pressed_file        = self.__clicked_file
         self.scroll_to_file(self.__clicked_file, True)
         self.__set_label_on_file_selection()
 
 
     def __perform_key_up(self):
         if self.__reset_index_of_clicked_file(): return
         for i in range(self.__index_of_clicked_file, 0, -1):
@@ -1269,15 +1527,15 @@
         else               : self.menu.create(self.__clicked_file.y,self.__clicked_file.x +1)
         return True
 
 
     def handle_events(self, event): # wtf, ok .. works acceptably :P, TODO: REMOVE rrrrepeating code but nvm for now >:( xD  | UPDATE: WHAT HAVE I DONE, WHY SO MANY IF AND NOT JSUT A DIRCT WITH FUNCTIONS
         if event == 0 or not self.is_focused                                           : return  # https://github.com/GiorgosXou/TUIFIManager/issues/24
         if self.__is_escape_consumed(event)                                            : return
-        if self.__perform_menu_selected_action(self.menu.handle_keyboard_events(event)): return
+        if self.menu.handle_keyboard_events(event): return
 
         if unicurses.keyname(event) in ('kxOUT','kxIN') :return # https://github.com/GiorgosXou/TUIFIManager/issues/81
         if self.events.get(event, self.__return)() != True : return # Is this too bad of a practice? let me know
         if self.__handle_mouse_events          (event) : return
         if self.__handle_alt_down              (event) : return
         if self.__handle_termux_keyboard_events(event) : return
         if self.auto_cmd_on_typing and event != 27:
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `TUIFIManager-3.3.5/TUIFIManager/__main__.py` & `TUIFIManager-4.0.0/TUIFIManager/__main__.py`

 * *Files identical despite different names*

### Comparing `TUIFIManager-3.3.5/TUIFIManager.egg-info/PKG-INFO` & `TUIFIManager-4.0.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TUIFIManager
-Version: 3.3.5
+Version: 4.0.0
 Summary: A cross-platform terminal-based termux-oriented file manager.
 Home-page: https://github.com/GiorgosXou/TUIFIManager
 Author: George Chousos
 Author-email: gxousos@gmail.com
 License: General Public License v3.0
 Project-URL: Github, https://github.com/GiorgosXou/TUIFIManager
 Keywords: file-manager,terminal,tui,ncurses,pdcurses,uni-curses,termux,vim,vim-motions,cross-platform
@@ -37,15 +37,25 @@
     </a>
     <a href="https://github.com/GiorgosXou/TUIFIManager/blob/master/LICENSE">
       <img src="https://img.shields.io/github/license/GiorgosXou/TUIFIManager?label=License&logo=GNU&style=flat-square"/>
 	</a>
 </p>
 </div>
 
-A cross-platform terminal-based termux-oriented file manager *(and component)*, meant to be used with a [Uni-Curses](https://github.com/unicurses/unicurses) project or as is. This project is mainly an attempt to get more attention to the [Uni-Curses](https://github.com/unicurses/unicurses) project.
+A cross-platform terminal-based termux-oriented file manager *(and component)*, meant to be used with a [Uni-Curses](https://github.com/unicurses/unicurses) project or as is. This project is mainly an attempt to get more attention to the [Uni-Curses](https://github.com/unicurses/unicurses) project. 
+
+##
+<div align="center">
+<p>
+<img src="./Peek.gif">
+</p>
+<p>
+<sub>FONT: Cartograph CF</sub>
+</p>
+</div>
 
 
 # ⚙️ Installation
 ```terminal
 sudo pip3 install tuifimanager --upgrade
 ```
 ```terminal
@@ -57,51 +67,52 @@
 # 💥 Usage
 Run `tuifi` in your terminal to use it as is or import it in one of your [Uni-Curses](https://github.com/unicurses/unicurses) project as a component like:
 ```python
 from TUIFIManager import *
 ```
 for more details look into the `__main__.py`
 
-<img src="./Peek.gif">
-<sub>FONT: Cartograph CF</sub>
 
 # 📦 Features 
 ### • 📌 *Current:*
-- Supports most of the common mouse events so far
-- It is somewhat fully customizable?
+- [Supports X11 Drag&Drop from terminals](#-customization 'set `tuifi_synth_dnd` enviroment variable to `True`. `pip install pynput PySide6 python-xlib`...')
+- Supports most common mouse events 
 - Can be used as a component
-- Uses only ~30MB of RAM
+- Uses about [~30MB](## '80mb with synthetic xdnd') of RAM
+- Strong [C TUI backend](https://github.com/unicurses/unicurses 'Via Uni-Curses, a NCurses\\PDCurses wrapper')
 - It is pretty snappy <!-- Kinda lol -->
 - Supports [Termux](https://github.com/termux) 
 - Cross Platform 
 - and more
 
 ### • 🔮 *Desired:*
+- Macros
+- [Treeview](## 'Via a `WindowPad`')
 - Undo\Redo
-- tool-tips
-- Scroll bar
-- [Sixel support](https://github.com/GiorgosXou/TUIFIManager/issues/86)
+- Improved UI
 - Multiple tabs
-- Better performance
+- [Sixel support](https://github.com/GiorgosXou/TUIFIManager/issues/86#issuecomment-2016846146)
 - Effect on cutted Files
-- [Drop files into GUI apps](https://github.com/GiorgosXou/TUIFIManager/issues/21)
+- Multithread performance
 
 # ⌨️ Keybindings
 In `vim_mode` both normal and vim shortcuts work 
 | Normal      | vim_mode | Action                                        |
-|----         | ---- |:----                                          |
+|----         | ---- |----                                          |
 |`SHIFT + TAB`  |   |Moves selected file to the previous directory |
 |`KEY_BACKSPACE`| `J` |Opens\Goes to the previous directory          |
 |`ALT + DOWN`   |   |Opens\Closes the "right-click menu"           |
 |`KEY_HOME`     | `H`  |Navigates to the $HOME directory              |
 |`KEY_F5`       |   |Reload\Refresh current directory              |
+|`KEY_F3`       | `o`  |(descending) order-type switch|
+|`KEY_F1`       | `O`  |(ascending) order-type switch|
 |`CTRL + V`     | `p` |Pastes the Copied or Cuted files              |
 |`DEL`          | `CTRL+d`  |Deletes the selected files                    |
 |`CTRL + F`     | `i`  |Find Files *(if not auto_find_on_typing)*     |
-|`CTRL + O`     | `O`  |Open whole directory in editor                |
+|`CTRL + O`     |   |Open whole directory in editor                |
 |`CTRL + A`     |  |Select all files in current folder|
 |`CTRL + C`     | `yy`  |Copies the selected files                     |
 |`CTRL + K`     |   |Copies the selected files                     |
 |`CTRL + X`     | `c`  |Cuts the selected files                       |
 |`CTRL + R`     | `r` |Rename selected file                          | 
 |`CTRL + T`     | | Toggle hidden files|
 |`CTRL + N`     | `W` |Create new folder                             |
@@ -122,73 +133,115 @@
 |`CTRL + UP`  | Same as `CTRL + V`, Pastes the Copied or Cuted files                           |
 |`END`        | Deletes selected files                                                         |
 
 
 # 👨‍💻 Commands
 **(Default & Custom Comands)** - To perform a command under the normal-mode, you first have to press the space-bar and then type the command. Alternatively, use `vim_mode` or enable the `tuifi_auto_command_on_typing` env-variable *(notice: it disables `tuifi_auto_find_on_typing`)*. **The default commands can be seen below and can be found under the `~/.config/tuifi/cmds.conf` where you can add your custom ones too:**
 
-| Cmd | Type | Attributes | Label Comment|
+| Cmd | Type | Attributes | Label Information|
 |---|---|---|---|
 |`gt` | open | 'directory':'~/.config/tuifi'           | - tuifi -|
 |`gh` | open | 'directory':'~/'                        | - Home -|
 |`owv` | open | 'directory':None,'\_with':'vim'         |Opened With Vim|
 |`yat` | copy | 'pattern':'.+\.txt'                     ||
 |`yy` | copy | 'pattern':None                          ||
 
-There are also some "static" ones like the `m`+character which marks the current directory into the character, so you can navigate back to it by using \` or `;`+that_character 
+**Available Type-keywords:** `open`, `copy`, `cut`, [`find`](## 'Attributes: `filename`')
+
+**important note:** `o` is also used for ordering in `vim_mode`. In this case you can first press space-bar before proceeding with `owv` or with any other already reserved starting key, or just change it. 
+
+**Additionally** there are also some "static" ones like the `m`+character which marks the current directory into the character, so you can navigate back to it by using \` or `;`+that_character 
+
 
 
 # 📜 Documentation
 <sub>Work in progress 🛠️🏗 ...</sub>
 
 
 # 💭 Customization 
-*How do I enable vim_mode?*
+<details>
+<summary><i>How do I enable vim_mode?</i></summary>
+
 > Set `tuifi_vim_mode` enviroment variable to `True`
 
-*How do I change the default keys (besides commands)?*
-> This is not possible right now althought you could play around with the content of `toggle_vim_mode` function under `__init__.py`
+</details>
+<details>
+<summary><i>How do I enable synthetic XDND?</i></summary>
+
+> set `tuifi_synth_dnd` enviroment variable to `True`. `pip install pynput PySide6 python-xlib`. Know it's expirimental! You'll need to adapt to it slightly, **use it as: Drag&drop + click afterwords where you want the file to be dropped.** [See also](https://github.com/GiorgosXou/TUIFIManager/discussions/92) and [this issue](https://github.com/GiorgosXou/TUIFIManager/issues/21)
+
+</details>
+<details>
+<summary><i>How do I set the default editor?</i></summary>
 
-*How do I set the default editor?*
 > Set `tuifi_default_editor` enviroment variable to `vim` or whatever you prefer
 
-*How do I disable the auto-find-mode?*
+</details>
+<details>
+<summary><i>How do I disable the auto-find-mode?</i></summary>
+
 > You can just set `tuifi_auto_find_on_typing` enviroment variable to `False`
 
-*How do I change the scroll sensitivity?*
+</details>
+<details>
+<summary><i>How do I change the scroll sensitivity?</i></summary>
+
 > You can set either or both `tuifi_scroll_sensitivity`, `tuifi_ctrl_scroll_sensitivity` enviromental variables, to the disered number of characters per scroll action *(they default to 1 and 7)*
 
-How do I change the number of visible lines of filenames that are visible?
+</details>
+<details>
+<summary><i>How do I change the default keys (besides commands)?</i></summary>
+
+> This is not possible right now althought you could play around with the content of `toggle_vim_mode` function under `__init__.py`
+
+</details>
+<details>
+<summary><i>How do I change the number of visible lines of filenames that are visible?</i></summary>
+
 > You can set how mnay lines you want using `tuifi_visible_filename_lines` *(Defaults to 4)*
 
-*How do I change the default configuration path?*
+</details>
+<details>
+<summary><i>How do I change the default configuration path?</i></summary>
+
 > Set `tuifi_config_path` enviroment variable to whatever you prefer most
 
-*How do I toggle hidden files/folders?*
+</details>
+<details>
+<summary><i>How do I toggle hidden files/folders?</i></summary>
+
 > You can either `CTRL + T` or set `tuifi_show_hidden` enviroment variable to `True`
 
-*How do I change the default colors?*
+</details>
+<details>
+<summary><i>How do I change the default colors?</i></summary>
+
 > [look here for more informations](https://github.com/GiorgosXou/TUIFIManager/issues/38)
 
+</details>
+
 
 # 💗 Donation
 I do really need money to survive, I have no job, living in a basement, making things for free, because I love to.
 - [***Paypal Address***](https://www.paypal.com/donate/?hosted_button_id=QNQN23M55EJVS)
 - ***Monero Address:*** `897ehhSQJQpGF7tYDhQM51jiX7nnHmzuYAW4q8JGwJxu8JKXvaK6AivCzatuJxnifjZ2qy98ks2g2PhmTaYCMMta2Ga2LJx`
 
 <div align="center">
 <img src='./TUIFI.png'>
 </div>
 
 
 # 🫶 Special thanks to
+- [@KORBEN for this article](https://korben.info/gestionnaire-fichiers-terminal-tuifimanager-multiplateforme-leger-personnalisable.html)
 - [Bryan Lunduke for this article](https://lunduke.substack.com/p/tuifi-manager-a-file-manager-in-the)
 - [Brodie Robertson for this video](https://youtu.be/9laxdMKTZLA)
 - [r/linux community for their comments](https://www.reddit.com/r/linux/comments/zzf5rx)
 - [r/cyberDeck community for their comments](https://www.reddit.com/r/cyberDeck/comments/zttur0)
 - [r/commandline community for their comments](https://www.reddit.com/r/commandline/comments/zt30v9)
 
-# 🕳️ Help
-Any Idea with this issue https://github.com/unicurses/unicurses/issues/21 ?
+# 🕳️ Outro
+- Any Idea with this issue https://github.com/unicurses/unicurses/issues/21 ?
+- Btw I use TUIFI in a daily basis. As crazy as it might sound: It's my primary file manager.
+
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: TUIFIManager Version: 3.3.5 Summary: A cross-
+Metadata-Version: 2.1 Name: TUIFIManager Version: 4.0.0 Summary: A cross-
 platform terminal-based termux-oriented file manager. Home-page: https://
 github.com/GiorgosXou/TUIFIManager Author: George Chousos Author-email:
 gxousos@gmail.com License: General Public License v3.0 Project-URL: Github,
 https://github.com/GiorgosXou/TUIFIManager Keywords: file-
 manager,terminal,tui,ncurses,pdcurses,uni-curses,termux,vim,vim-motions,cross-
 platform Platform: unix Platform: linux Platform: osx Platform: cygwin
 Platform: windows Classifier: Intended Audience :: Developers Classifier:
@@ -17,37 +17,43 @@
             _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_l_a_s_t_-_c_o_m_m_i_t_/_G_i_o_r_g_o_s_X_o_u_/
  _T_U_I_F_I_M_a_n_a_g_e_r_?_c_o_l_o_r_=_%_4_d_c_7_1_f_&_l_a_b_e_l_=_L_a_s_t_%_2_0_C_o_m_m_i_t_&_l_o_g_o_=_g_i_t_h_u_b_&_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]
               _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_l_i_c_e_n_s_e_/_G_i_o_r_g_o_s_X_o_u_/
             _T_U_I_F_I_M_a_n_a_g_e_r_?_l_a_b_e_l_=_L_i_c_e_n_s_e_&_l_o_g_o_=_G_N_U_&_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]
 A cross-platform terminal-based termux-oriented file manager *(and component)*,
 meant to be used with a [Uni-Curses](https://github.com/unicurses/unicurses)
 project or as is. This project is mainly an attempt to get more attention to
-the [Uni-Curses](https://github.com/unicurses/unicurses) project. # âï¸
-Installation ```terminal sudo pip3 install tuifimanager --upgrade ```
+the [Uni-Curses](https://github.com/unicurses/unicurses) project. ##
+                                 [./Peek.gif]
+                              FONT: Cartograph CF
+# âï¸ Installation ```terminal sudo pip3 install tuifimanager --upgrade ```
 ```terminal pip3 install TUIFIManager --upgrade ``` or just ^^^ if it works for
 you. *(eg. on termux?)* # ð¥ Usage Run `tuifi` in your terminal to use it as
 is or import it in one of your [Uni-Curses](https://github.com/unicurses/
 unicurses) project as a component like: ```python from TUIFIManager import *
-``` for more details look into the `__main__.py` [./Peek.gif]FONT: Cartograph
-CF # ð¦ Features ### â¢ ð *Current:* - Supports most of the common mouse
-events so far - It is somewhat fully customizable? - Can be used as a component
-- Uses only ~30MB of RAM - It is pretty snappy - Supports [Termux](https://
-github.com/termux) - Cross Platform - and more ### â¢ ð® *Desired:* -
-Undo\Redo - tool-tips - Scroll bar - [Sixel support](https://github.com/
-GiorgosXou/TUIFIManager/issues/86) - Multiple tabs - Better performance -
-Effect on cutted Files - [Drop files into GUI apps](https://github.com/
-GiorgosXou/TUIFIManager/issues/21) # â¨ï¸ Keybindings In `vim_mode` both
-normal and vim shortcuts work | Normal | vim_mode | Action | |---- | ---- |:---
-- | |`SHIFT + TAB` | |Moves selected file to the previous directory |
-|`KEY_BACKSPACE`| `J` |Opens\Goes to the previous directory | |`ALT + DOWN` |
-|Opens\Closes the "right-click menu" | |`KEY_HOME` | `H` |Navigates to the
-$HOME directory | |`KEY_F5` | |Reload\Refresh current directory | |`CTRL + V` |
-`p` |Pastes the Copied or Cuted files | |`DEL` | `CTRL+d` |Deletes the selected
+``` for more details look into the `__main__.py` # ð¦ Features ### â¢ ð
+*Current:* - [Supports X11 Drag&Drop from terminals](#-customization 'set
+`tuifi_synth_dnd` enviroment variable to `True`. `pip install pynput PySide6
+python-xlib`...') - Supports most common mouse events - Can be used as a
+component - Uses about [~30MB](## '80mb with synthetic xdnd') of RAM - Strong
+[C TUI backend](https://github.com/unicurses/unicurses 'Via Uni-Curses, a
+NCurses\\PDCurses wrapper') - It is pretty snappy - Supports [Termux](https://
+github.com/termux) - Cross Platform - and more ### â¢ ð® *Desired:* - Macros
+- [Treeview](## 'Via a `WindowPad`') - Undo\Redo - Improved UI - Multiple tabs
+- [Sixel support](https://github.com/GiorgosXou/TUIFIManager/issues/
+86#issuecomment-2016846146) - Effect on cutted Files - Multithread performance
+# â¨ï¸ Keybindings In `vim_mode` both normal and vim shortcuts work | Normal
+| vim_mode | Action | |---- | ---- |---- | |`SHIFT + TAB` | |Moves selected
+file to the previous directory | |`KEY_BACKSPACE`| `J` |Opens\Goes to the
+previous directory | |`ALT + DOWN` | |Opens\Closes the "right-click menu" |
+|`KEY_HOME` | `H` |Navigates to the $HOME directory | |`KEY_F5` |
+|Reload\Refresh current directory | |`KEY_F3` | `o` |(descending) order-type
+switch| |`KEY_F1` | `O` |(ascending) order-type switch| |`CTRL + V` | `p`
+|Pastes the Copied or Cuted files | |`DEL` | `CTRL+d` |Deletes the selected
 files | |`CTRL + F` | `i` |Find Files *(if not auto_find_on_typing)* | |`CTRL +
-O` | `O` |Open whole directory in editor | |`CTRL + A` | |Select all files in
+O` | |Open whole directory in editor | |`CTRL + A` | |Select all files in
 current folder| |`CTRL + C` | `yy` |Copies the selected files | |`CTRL + K` |
 |Copies the selected files | |`CTRL + X` | `c` |Cuts the selected files |
 |`CTRL + R` | `r` |Rename selected file | |`CTRL + T` | | Toggle hidden files|
 |`CTRL + N` | `W` |Create new folder | |`CTRL + W` | `w` |Create new file |
 |`ARROW KEYS` | `l` `k` `j` `h` |Navigates files | |`KEY_ENTER` | `K`|Opens
 files | |`CTRL + E` | `e` |Exit with `cd` | |`ESCAPE` | |Exit | **(*TIP:** ð
 use `ALT + CLICK` for multiple mouse selection if `SHIFT` not working)*
@@ -58,45 +64,57 @@
 the selected file(s) | |`CTRL + UP` | Same as `CTRL + V`, Pastes the Copied or
 Cuted files | |`END` | Deletes selected files | # ð¨âð» Commands **
 (Default & Custom Comands)** - To perform a command under the normal-mode, you
 first have to press the space-bar and then type the command. Alternatively, use
 `vim_mode` or enable the `tuifi_auto_command_on_typing` env-variable *(notice:
 it disables `tuifi_auto_find_on_typing`)*. **The default commands can be seen
 below and can be found under the `~/.config/tuifi/cmds.conf` where you can add
-your custom ones too:** | Cmd | Type | Attributes | Label Comment| |---|---|---
-|---| |`gt` | open | 'directory':'~/.config/tuifi' | - tuifi -| |`gh` | open |
-'directory':'~/' | - Home -| |`owv` | open | 'directory':None,'\_with':'vim'
-|Opened With Vim| |`yat` | copy | 'pattern':'.+\.txt' || |`yy` | copy |
-'pattern':None || There are also some "static" ones like the `m`+character
-which marks the current directory into the character, so you can navigate back
-to it by using \` or `;`+that_character # ð Documentation Work in progress
-ð ï¸ð ... # ð­ Customization *How do I enable vim_mode?* > Set
-`tuifi_vim_mode` enviroment variable to `True` *How do I change the default
-keys (besides commands)?* > This is not possible right now althought you could
-play around with the content of `toggle_vim_mode` function under `__init__.py`
-*How do I set the default editor?* > Set `tuifi_default_editor` enviroment
-variable to `vim` or whatever you prefer *How do I disable the auto-find-mode?*
-> You can just set `tuifi_auto_find_on_typing` enviroment variable to `False`
-*How do I change the scroll sensitivity?* > You can set either or both
+your custom ones too:** | Cmd | Type | Attributes | Label Information| |---|---
+|---|---| |`gt` | open | 'directory':'~/.config/tuifi' | - tuifi -| |`gh` |
+open | 'directory':'~/' | - Home -| |`owv` | open | 'directory':None,'\_with':
+'vim' |Opened With Vim| |`yat` | copy | 'pattern':'.+\.txt' || |`yy` | copy |
+'pattern':None || **Available Type-keywords:** `open`, `copy`, `cut`, [`find`]
+(## 'Attributes: `filename`') **important note:** `o` is also used for ordering
+in `vim_mode`. In this case you can first press space-bar before proceeding
+with `owv` or with any other already reserved starting key, or just change it.
+**Additionally** there are also some "static" ones like the `m`+character which
+marks the current directory into the character, so you can navigate back to it
+by using \` or `;`+that_character # ð Documentation Work in progress
+ð ï¸ð ... # ð­ Customization How do I enable vim_mode? > Set
+`tuifi_vim_mode` enviroment variable to `True` How do I enable synthetic XDND?
+> set `tuifi_synth_dnd` enviroment variable to `True`. `pip install pynput
+PySide6 python-xlib`. Know it's expirimental! You'll need to adapt to it
+slightly, **use it as: Drag&drop + click afterwords where you want the file to
+be dropped.** [See also](https://github.com/GiorgosXou/TUIFIManager/
+discussions/92) and [this issue](https://github.com/GiorgosXou/TUIFIManager/
+issues/21) How do I set the default editor? > Set `tuifi_default_editor`
+enviroment variable to `vim` or whatever you prefer How do I disable the auto-
+find-mode? > You can just set `tuifi_auto_find_on_typing` enviroment variable
+to `False` How do I change the scroll sensitivity? > You can set either or both
 `tuifi_scroll_sensitivity`, `tuifi_ctrl_scroll_sensitivity` enviromental
 variables, to the disered number of characters per scroll action *(they default
-to 1 and 7)* How do I change the number of visible lines of filenames that are
-visible? > You can set how mnay lines you want using
-`tuifi_visible_filename_lines` *(Defaults to 4)* *How do I change the default
-configuration path?* > Set `tuifi_config_path` enviroment variable to whatever
-you prefer most *How do I toggle hidden files/folders?* > You can either `CTRL
-+ T` or set `tuifi_show_hidden` enviroment variable to `True` *How do I change
-the default colors?* > [look here for more informations](https://github.com/
-GiorgosXou/TUIFIManager/issues/38) # ð Donation I do really need money to
-survive, I have no job, living in a basement, making things for free, because I
-love to. - [***Paypal Address***](https://www.paypal.com/donate/
+to 1 and 7)* How do I change the default keys (besides commands)? > This is not
+possible right now althought you could play around with the content of
+`toggle_vim_mode` function under `__init__.py` How do I change the number of
+visible lines of filenames that are visible? > You can set how mnay lines you
+want using `tuifi_visible_filename_lines` *(Defaults to 4)* How do I change the
+default configuration path? > Set `tuifi_config_path` enviroment variable to
+whatever you prefer most How do I toggle hidden files/folders? > You can either
+`CTRL + T` or set `tuifi_show_hidden` enviroment variable to `True` How do I
+change the default colors? > [look here for more informations](https://
+github.com/GiorgosXou/TUIFIManager/issues/38) # ð Donation I do really need
+money to survive, I have no job, living in a basement, making things for free,
+because I love to. - [***Paypal Address***](https://www.paypal.com/donate/
 ?hosted_button_id=QNQN23M55EJVS) - ***Monero Address:***
 `897ehhSQJQpGF7tYDhQM51jiX7nnHmzuYAW4q8JGwJxu8JKXvaK6AivCzatuJxnifjZ2qy98ks2g2PhmTaYCMMta2Ga2LJx`
                                  [./TUIFI.png]
-# ð«¶ Special thanks to - [Bryan Lunduke for this article](https://
+# ð«¶ Special thanks to - [@KORBEN for this article](https://korben.info/
+gestionnaire-fichiers-terminal-tuifimanager-multiplateforme-leger-
+personnalisable.html) - [Bryan Lunduke for this article](https://
 lunduke.substack.com/p/tuifi-manager-a-file-manager-in-the) - [Brodie Robertson
 for this video](https://youtu.be/9laxdMKTZLA) - [r/linux community for their
 comments](https://www.reddit.com/r/linux/comments/zzf5rx) - [r/cyberDeck
 community for their comments](https://www.reddit.com/r/cyberDeck/comments/
 zttur0) - [r/commandline community for their comments](https://www.reddit.com/
-r/commandline/comments/zt30v9) # ð³ï¸ Help Any Idea with this issue https://
-github.com/unicurses/unicurses/issues/21 ?
+r/commandline/comments/zt30v9) # ð³ï¸ Outro - Any Idea with this issue
+https://github.com/unicurses/unicurses/issues/21 ? - Btw I use TUIFI in a daily
+basis. As crazy as it might sound: It's my primary file manager.
```

### Comparing `TUIFIManager-3.3.5/TUIFIManager.egg-info/SOURCES.txt` & `TUIFIManager-4.0.0/TUIFIManager.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 setup.py
 .github/ISSUE_TEMPLATE/bug_report.md
 .github/ISSUE_TEMPLATE/feature_request.md
 .github/workflows/nox_ci.yml
 TUIFIManager/TUIFIProfile.py
 TUIFIManager/TUIFile.py
 TUIFIManager/TUIMenu.py
+TUIFIManager/TUISynthXDND.py
 TUIFIManager/TUItilities.py
 TUIFIManager/__init__.py
 TUIFIManager/__main__.py
 TUIFIManager.egg-info/PKG-INFO
 TUIFIManager.egg-info/SOURCES.txt
 TUIFIManager.egg-info/dependency_links.txt
 TUIFIManager.egg-info/entry_points.txt
```

### Comparing `TUIFIManager-3.3.5/pyproject.toml` & `TUIFIManager-4.0.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "TUIFIManager"
-version = "3.3.5"
+version = "4.0.0"
 
 description = "A cross-platform terminal-based termux-oriented file manager."
 requires-python = ">=3.8"
 readme = "README.md"
 
 dependencies = [
     "uni-curses >= 2.1.3",
-    "Send2Trash == 1.8.0",
+    "Send2Trash >= 1.8.0",
 ]
 
 license = {text = "General Public License v3.0"}
 classifiers = [
     "Intended Audience :: Developers",
     "Intended Audience :: End Users/Desktop",
     "License :: OSI Approved :: MIT License",
```

### Comparing `TUIFIManager-3.3.5/setup.cfg` & `TUIFIManager-4.0.0/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = TUIFIManager
-version = 3.3.5
+version = 4.0.0
 description = A cross-platform terminal-based termux-oriented file manager
 long_description = file: docs/README.md
 long_description_content_type = text/markdown
 author = George Chousos
 author_email = gxousos@gmail.com
 keywords = file-manager, terminal, tui, ncurses, pdcurses, uni-curses, termux, vim, vim-motions, cross-platform
 license = GPL-3.0
```

