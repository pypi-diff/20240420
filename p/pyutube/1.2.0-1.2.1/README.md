# Comparing `tmp/pyutube-1.2.0.tar.gz` & `tmp/pyutube-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyutube-1.2.0.tar", last modified: Thu Apr 11 14:09:10 2024, max compression
+gzip compressed data, was "pyutube-1.2.1.tar", last modified: Sat Apr 20 10:05:55 2024, max compression
```

## Comparing `pyutube-1.2.0.tar` & `pyutube-1.2.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0 brhoom    (1000) brhoom    (1000)        0 2024-04-11 14:09:10.256730 pyutube-1.2.0/
--rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)     1078 2024-03-05 00:46:11.000000 pyutube-1.2.0/LICENSE.md
--rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)     7025 2024-04-11 14:09:10.255784 pyutube-1.2.0/PKG-INFO
--rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)     6204 2024-04-11 14:08:03.000000 pyutube-1.2.0/README.md
-drwxrwxrwx   0 brhoom    (1000) brhoom    (1000)        0 2024-04-11 14:09:10.243337 pyutube-1.2.0/pyutube/
--rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)      399 2024-04-07 04:16:19.000000 pyutube-1.2.0/pyutube/__init__.py
--rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)      184 2024-03-31 03:14:16.000000 pyutube-1.2.0/pyutube/__main__.py
--rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)     6690 2024-04-11 14:08:48.000000 pyutube-1.2.0/pyutube/cli.py
--rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)    13801 2024-04-11 12:47:00.000000 pyutube-1.2.0/pyutube/downloader.py
-drwxrwxrwx   0 brhoom    (1000) brhoom    (1000)        0 2024-04-11 14:09:10.253182 pyutube-1.2.0/pyutube/tests/
--rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)       30 2024-02-14 23:03:00.000000 pyutube-1.2.0/pyutube/tests/__init__.py
--rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)     4676 2024-04-06 03:28:26.000000 pyutube-1.2.0/pyutube/tests/test_utils.py
--rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)    10206 2024-04-11 13:48:28.000000 pyutube-1.2.0/pyutube/utils.py
-drwxrwxrwx   0 brhoom    (1000) brhoom    (1000)        0 2024-04-11 14:09:10.254718 pyutube-1.2.0/pyutube.egg-info/
--rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)     7025 2024-04-11 14:09:10.000000 pyutube-1.2.0/pyutube.egg-info/PKG-INFO
--rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)      365 2024-04-11 14:09:10.000000 pyutube-1.2.0/pyutube.egg-info/SOURCES.txt
--rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)        1 2024-04-11 14:09:10.000000 pyutube-1.2.0/pyutube.egg-info/dependency_links.txt
--rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)       44 2024-04-11 14:09:10.000000 pyutube-1.2.0/pyutube.egg-info/entry_points.txt
--rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)       70 2024-04-11 14:09:10.000000 pyutube-1.2.0/pyutube.egg-info/requires.txt
--rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)        8 2024-04-11 14:09:10.000000 pyutube-1.2.0/pyutube.egg-info/top_level.txt
--rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)       38 2024-04-11 14:09:10.256867 pyutube-1.2.0/setup.cfg
--rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)     1436 2024-04-07 04:18:59.000000 pyutube-1.2.0/setup.py
+drwxrwxrwx   0 brhoom    (1000) brhoom    (1000)        0 2024-04-20 10:05:55.009515 pyutube-1.2.1/
+-rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)     1078 2024-03-05 00:46:11.000000 pyutube-1.2.1/LICENSE.md
+-rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)     8304 2024-04-20 10:05:55.008246 pyutube-1.2.1/PKG-INFO
+-rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)     7483 2024-04-20 10:02:00.000000 pyutube-1.2.1/README.md
+drwxrwxrwx   0 brhoom    (1000) brhoom    (1000)        0 2024-04-20 10:05:54.982750 pyutube-1.2.1/pyutube/
+-rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)      399 2024-04-07 04:16:19.000000 pyutube-1.2.1/pyutube/__init__.py
+-rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)      184 2024-03-31 03:14:16.000000 pyutube-1.2.1/pyutube/__main__.py
+-rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)     6749 2024-04-20 09:57:31.000000 pyutube-1.2.1/pyutube/cli.py
+-rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)    13717 2024-04-20 09:52:41.000000 pyutube-1.2.1/pyutube/downloader.py
+drwxrwxrwx   0 brhoom    (1000) brhoom    (1000)        0 2024-04-20 10:05:55.005206 pyutube-1.2.1/pyutube/tests/
+-rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)       30 2024-02-14 23:03:00.000000 pyutube-1.2.1/pyutube/tests/__init__.py
+-rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)     4676 2024-04-12 09:09:48.000000 pyutube-1.2.1/pyutube/tests/test_utils.py
+-rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)    11817 2024-04-20 09:59:18.000000 pyutube-1.2.1/pyutube/utils.py
+drwxrwxrwx   0 brhoom    (1000) brhoom    (1000)        0 2024-04-20 10:05:55.006933 pyutube-1.2.1/pyutube.egg-info/
+-rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)     8304 2024-04-20 10:05:54.000000 pyutube-1.2.1/pyutube.egg-info/PKG-INFO
+-rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)      365 2024-04-20 10:05:54.000000 pyutube-1.2.1/pyutube.egg-info/SOURCES.txt
+-rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)        1 2024-04-20 10:05:54.000000 pyutube-1.2.1/pyutube.egg-info/dependency_links.txt
+-rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)       44 2024-04-20 10:05:54.000000 pyutube-1.2.1/pyutube.egg-info/entry_points.txt
+-rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)       70 2024-04-20 10:05:54.000000 pyutube-1.2.1/pyutube.egg-info/requires.txt
+-rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)        8 2024-04-20 10:05:54.000000 pyutube-1.2.1/pyutube.egg-info/top_level.txt
+-rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)       38 2024-04-20 10:05:55.009672 pyutube-1.2.1/setup.cfg
+-rwxrwxrwx   0 brhoom    (1000) brhoom    (1000)     1436 2024-04-07 04:18:59.000000 pyutube-1.2.1/setup.py
```

### Comparing `pyutube-1.2.0/LICENSE.md` & `pyutube-1.2.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyutube-1.2.0/README.md` & `pyutube-1.2.1/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,92 +1,123 @@
 # 📹 YouTube Downloader CLI
 
-## Enjoying my project? Please show your appreciation by starring it on GitHub! ⭐
+### Enjoying my project? Please show your appreciation by starring it on GitHub! ⭐
 
-> [!NOTE] Help me to improve this tool!
-> I tested it on Windows, Mac, and Linux, and it works fine, but if there is any issue, please open an issue on [GitHub](https://github.com/Hetari/pyutube/issues/new) and I'll fix it.
->
+[![Version](https://img.shields.io/pypi/v/pyutube.svg?style=flat)](https://pypi.org/project/pyutube/)
+[![Downloads](https://static.pepy.tech/badge/pyutube)](https://pepy.tech/project/pyutube)
+
+> [!NOTE]
 > Have a new feature? Please don't hesitate to [tell me](https://github.com/Hetari/pyutube/issues/new)!
 
 <a href="https://ibb.co/27wcFYN">
    <img src="https://i.ibb.co/MDbPg56/Screenshot-from-2024-04-08-21-38-02-transformed.png" alt="Pyutube" style="width: 100%;">
 </a>
 
+<!-- <a href="https://ibb.co/27wcFYN">
+   <img src="images/pyutube.png" alt="Pyutube" style="width: 100%;">
+</a> -->
+
 ## 📓 Description
 
 This command-line tool downloads YouTube videos from the `Terminal`, written under [Pytube](https://pytube.io/).
 
 it is cross-platform (Windows, Mac, Linux) and can be used in any terminal.
 
-## 💎 Features
-
 - User-friendly CLI interface.
 - Download a single YouTube video format or audio.
 - Download YouTube shorts.
 - Download YouTube playlists.
 
-## Upgrade
+## :why: why `pyutube`?
 
-All the latest updates will be posted on [GitHub](https://github.com/Hetari/pyutube), you can also upgrade the tool via [PyPI](https://pypi.org/project/pyutube/) with this command:
-
-```bash
-pip install --upgrade pyutube
-```
-
-## Installation
+## 🛠️ Installation
 
 it is easy to install Pyutube, make sure that you have [Python](https://www.python.org) installed. To check if you have it installed, type `python --version` in your terminal. You should see something like `Python 3. x ` otherwise, download and install it from [Python](https://www.python.org/downloads/).
 
 after that, you can install it with the following command:
 
 ```bash
 pip install pyutube
 ```
 
+## 📈 Upgrade
+
+All the latest updates will be posted on [GitHub](https://github.com/Hetari/pyutube), you can also upgrade the tool via [PyPI](https://pypi.org/project/pyutube/) with this command:
+
+```bash
+pip install --upgrade pyutube
+```
+
 Then you can use it in your `Terminal` 🥳.
 
-## Usage
+## 🦸 Quick Start
 
 Pyutube is very easy to use, here are examples of its uses:
 
 ```bash
 pyutube YOUTUBE_LINK [PATH]
 ```
 
-> [!NOTE] > `[PATH]` is an optional input, the default value is the `terminal` path where the CLI is running (the current working directory).
+> [!NOTE] > `[PATH]` is an optional input, the default value is the `terminal` path where the CLI is running (the current working directory in your terminal).
+
+## 🦸 Usage
 
 <div style="text-align: center;">
    <p>Download video with specify the save location</p>
    <a href="https://ibb.co/0JkdkQy">
       <img src="https://i.ibb.co/7yH6Hbt/image1.png" alt="Download video with specify the save location">
    </a>
-
    <p>Chose what type you want to download</p>
    <a href="https://ibb.co/Kb6qjmg">
       <img src="https://i.ibb.co/sbjwvt4/image2.png" alt="Chose what type you want to download">
    </a>
-
    <p>Chose what what resolution you want to download(if the type is video)</p>
    <a href="https://ibb.co/7ymCS79">
       <img src="https://i.ibb.co/h8z9gpq/image4.png" alt="Chose what what resolution you want to download">
    </a>
-
    <p>If you download a playlist, you can chose what video you want to download, or even all of them</p>
    <a href="https://ibb.co/0qwkQNm">
       <img src="https://i.ibb.co/1ZS3bV7/Screenshot-from-2024-04-11-16-42-29.png" alt="If you download a playlist, you can chose what video you want to download, or even all of them"/>
    </a>
-
 <br /><br />
-<a href="https://ibb.co/LhT6r3r">
-
-   <p>Do not know how to use it? just type <code>pyutube --help</code></p>
+ <p>Do not know how to use it? just type <code>pyutube --help</code></p>
+  <a href="https://ibb.co/LhT6r3r">
       <img src="https://i.ibb.co/WprF0L0/image5.png" alt="image5">
    </a>
 </div>
 
+<!-- <div style="text-align: center;">
+   <p>Download video with specify the save location</p>
+   <a href="https://ibb.co/0JkdkQy">
+      <img src="images/image1.png" alt="Download video with specify the save location">
+   </a>
+
+   <p>Chose what type you want to download</p>
+   <a href="https://ibb.co/Kb6qjmg">
+      <img src="images/image2.png" alt="Chose what type you want to download">
+   </a>
+
+   <p>Chose what what resolution you want to download(if the type is video)</p>
+   <a href="https://ibb.co/7ymCS79">
+      <img src="images/image3.png" alt="Chose what what resolution you want to download">
+   </a>
+
+   <p>If you download a playlist, you can chose what video you want to download, or even all of them</p>
+   <a href="https://ibb.co/0qwkQNm">
+      <img src="images/image4.png" alt="If you download a playlist, you can chose what video you want to download, or even all of them"/>
+   </a>
+
+<br /><br />
+
+ <p>Do not know how to use it? just type <code>pyutube --help</code></p>
+  <a href="https://ibb.co/LhT6r3r">
+      <img src="images/image5.png" alt="image5">
+   </a>
+</div> -->
+
 #### Arguments
 
 | Arguments | Description                                                                                                          |
 | --------- | -------------------------------------------------------------------------------------------------------------------- |
 | `URL`     | The `URL` of the YouTube video. This argument is <span style="color:red">[Required]</span>.                          |
 | `PATH`    | The `path` to save the video. Defaults to the current working directory. <span style="color:green">[Optional]</span> |
 
@@ -94,15 +125,15 @@
 
 | Option                                              | Description                                                      |
 | --------------------------------------------------- | ---------------------------------------------------------------- |
 | `-v` <span style="color:cyan">or</span> `--version` | Show the version number.                                         |
 | `-a` <span style="color:cyan">or</span> `--audio`   | Download only audio immediately without asking (video or audio). |
 | `-f` <span style="color:cyan">or</span> `--footage` | Download only video immediately without asking (video or audio). |
 
-## Examples
+## 🕵️‍♂️ Examples
 
 ### **- Show version:**
 
 ```bash
 pyutube -v
 ```
 
@@ -163,15 +194,15 @@
 
 ```bash
 pyutube -f youtu.be/cMPnY7EuZvo
 ```
 
 see the video and relax 🎉.
 
-## Contributing
+## 🥰 Contributing
 
 Pull requests are welcome. For major changes, please open an issue first to discuss what you want to change.
 please follow the [contributing guidelines](https://github.com/Hetari/pyutube/blob/main/CONTRIBUTING.md)
 
-## License
+## 📎 License
 
 This project is licensed under the [MIT License](https://github.com/Hetari/pyutube/blob/main/LICENSE.md).
```

#### html2text {}

```diff
@@ -1,55 +1,55 @@
-# ð¹ YouTube Downloader CLI ## Enjoying my project? Please show your
-appreciation by starring it on GitHub! â­ > [!NOTE] Help me to improve this
-tool! > I tested it on Windows, Mac, and Linux, and it works fine, but if there
-is any issue, please open an issue on [GitHub](https://github.com/Hetari/
-pyutube/issues/new) and I'll fix it. > > Have a new feature? Please don't
-hesitate to [tell me](https://github.com/Hetari/pyutube/issues/new)!
-_[_P_y_u_t_u_b_e_]## ð Description This command-line tool downloads YouTube videos
-from the `Terminal`, written under [Pytube](https://pytube.io/). it is cross-
-platform (Windows, Mac, Linux) and can be used in any terminal. ## ð
-Features - User-friendly CLI interface. - Download a single YouTube video
-format or audio. - Download YouTube shorts. - Download YouTube playlists. ##
-Upgrade All the latest updates will be posted on [GitHub](https://github.com/
-Hetari/pyutube), you can also upgrade the tool via [PyPI](https://pypi.org/
-project/pyutube/) with this command: ```bash pip install --upgrade pyutube ```
-## Installation it is easy to install Pyutube, make sure that you have [Python]
-(https://www.python.org) installed. To check if you have it installed, type
-`python --version` in your terminal. You should see something like `Python 3. x
-` otherwise, download and install it from [Python](https://www.python.org/
-downloads/). after that, you can install it with the following command: ```bash
-pip install pyutube ``` Then you can use it in your `Terminal` ð¥³. ## Usage
+# ð¹ YouTube Downloader CLI ### Enjoying my project? Please show your
+appreciation by starring it on GitHub! â­ [![Version](https://img.shields.io/
+pypi/v/pyutube.svg?style=flat)](https://pypi.org/project/pyutube/) [!
+[Downloads](https://static.pepy.tech/badge/pyutube)](https://pepy.tech/project/
+pyutube) > [!NOTE] > Have a new feature? Please don't hesitate to [tell me]
+(https://github.com/Hetari/pyutube/issues/new)! _[_P_y_u_t_u_b_e_]## ð Description
+This command-line tool downloads YouTube videos from the `Terminal`, written
+under [Pytube](https://pytube.io/). it is cross-platform (Windows, Mac, Linux)
+and can be used in any terminal. - User-friendly CLI interface. - Download a
+single YouTube video format or audio. - Download YouTube shorts. - Download
+YouTube playlists. ## :why: why `pyutube`? ## ð ï¸ Installation it is easy
+to install Pyutube, make sure that you have [Python](https://www.python.org)
+installed. To check if you have it installed, type `python --version` in your
+terminal. You should see something like `Python 3. x ` otherwise, download and
+install it from [Python](https://www.python.org/downloads/). after that, you
+can install it with the following command: ```bash pip install pyutube ``` ##
+ð Upgrade All the latest updates will be posted on [GitHub](https://
+github.com/Hetari/pyutube), you can also upgrade the tool via [PyPI](https://
+pypi.org/project/pyutube/) with this command: ```bash pip install --upgrade
+pyutube ``` Then you can use it in your `Terminal` ð¥³. ## ð¦¸ Quick Start
 Pyutube is very easy to use, here are examples of its uses: ```bash pyutube
 YOUTUBE_LINK [PATH] ``` > [!NOTE] > `[PATH]` is an optional input, the default
 value is the `terminal` path where the CLI is running (the current working
-directory).
+directory in your terminal). ## ð¦¸ Usage
 Download video with specify the save location
 _[_D_o_w_n_l_o_a_d_ _v_i_d_e_o_ _w_i_t_h_ _s_p_e_c_i_f_y_ _t_h_e_ _s_a_v_e_ _l_o_c_a_t_i_o_n_]
 Chose what type you want to download
 _[_C_h_o_s_e_ _w_h_a_t_ _t_y_p_e_ _y_o_u_ _w_a_n_t_ _t_o_ _d_o_w_n_l_o_a_d_]
 Chose what what resolution you want to download(if the type is video)
 _[_C_h_o_s_e_ _w_h_a_t_ _w_h_a_t_ _r_e_s_o_l_u_t_i_o_n_ _y_o_u_ _w_a_n_t_ _t_o_ _d_o_w_n_l_o_a_d_]
 If you download a playlist, you can chose what video you want to download, or
 even all of them
 _[_I_f_ _y_o_u_ _d_o_w_n_l_o_a_d_ _a_ _p_l_a_y_l_i_s_t_,_ _y_o_u_ _c_a_n_ _c_h_o_s_e_ _w_h_a_t_ _v_i_d_e_o_ _y_o_u_ _w_a_n_t_ _t_o_ _d_o_w_n_l_o_a_d_,_ _o_r
 _e_v_e_n_ _a_l_l_ _o_f_ _t_h_e_m_]
 
-_D_o_ _n_o_t_ _k_n_o_w_ _h_o_w_ _t_o_ _u_s_e_ _i_t_?_ _j_u_s_t_ _t_y_p_e_ _p_y_u_t_u_b_e_ _-_-_h_e_l_p
+Do not know how to use it? just type pyutube --help
 _[_i_m_a_g_e_5_]
 #### Arguments | Arguments | Description | | --------- | ----------------------
 -------------------------------------------------------------------------------
 --------------- | | `URL` | The `URL` of the YouTube video. This argument is
 [Required]. | | `PATH` | The `path` to save the video. Defaults to the current
 working directory. [Optional] | #### Options | Option | Description | | -------
 -------------------------------------------- | --------------------------------
 -------------------------------- | | `-v` or `--version` | Show the version
 number. | | `-a` or `--audio` | Download only audio immediately without asking
 (video or audio). | | `-f` or `--footage` | Download only video immediately
-without asking (video or audio). | ## Examples ### **- Show version:** ```bash
-pyutube -v ``` ### **- Download playlists:** 1. `pyutube
+without asking (video or audio). | ## ðµï¸ââï¸ Examples ### **- Show
+version:** ```bash pyutube -v ``` ### **- Download playlists:** 1. `pyutube
 PLAYLIST_ID> [the_download_path*]` > [!NOTE] > Don't forget, the path is
 optional. 2. Then choose the format of the download, video or audio. 3. Choose
 the resolution if it is a video you want to download, otherwise, choose audio
 and it will download it all immediately ð¥. > [!NOTE] > It will check all
 resolutions available in the first video in the playlist, then it will download
 all of them in the same resolution ð. ### **- Download shorts, videos, or
 audio:** 1. `pyutube
@@ -60,12 +60,13 @@
 pyutube youtu.be/cMPnY7EuZvo pyutube https://youtube.com/watch?v=cMPnY7EuZvo
 ``` ### **- Download audio immediately:** 1. `pyutube
 VIDEO_ID | SHORT_LINK> [the_download_path*] -a` ```bash pyutube cMPnY7EuZvo -
 a ``` or ```bash pyutube -a youtu.be/cMPnY7EuZvo ``` and that's it ð. ###
 **- Download videos immediately:** 1. `pyutube
 VIDEO_ID | SHORT_LINK> [the_download_path*] -f` 2. Choose the resolution.
 ```bash pyutube cMPnY7EuZvo -f ``` or ```bash pyutube -f youtu.be/cMPnY7EuZvo
-``` see the video and relax ð. ## Contributing Pull requests are welcome.
-For major changes, please open an issue first to discuss what you want to
-change. please follow the [contributing guidelines](https://github.com/Hetari/
-pyutube/blob/main/CONTRIBUTING.md) ## License This project is licensed under
-the [MIT License](https://github.com/Hetari/pyutube/blob/main/LICENSE.md).
+``` see the video and relax ð. ## ð¥° Contributing Pull requests are
+welcome. For major changes, please open an issue first to discuss what you want
+to change. please follow the [contributing guidelines](https://github.com/
+Hetari/pyutube/blob/main/CONTRIBUTING.md) ## ð License This project is
+licensed under the [MIT License](https://github.com/Hetari/pyutube/blob/main/
+LICENSE.md).
```

### Comparing `pyutube-1.2.0/pyutube/cli.py` & `pyutube-1.2.1/pyutube/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -41,22 +41,24 @@
 import sys
 
 import typer
 import threading
 
 from pyutube.utils import (
     __version__,
+    __app__,
     clear,
     error_console,
     console,
     check_internet_connection,
     is_youtube_video_id,
     validate_link,
     handle_video_link,
     ask_playlist_video_names,
+    check_for_updates
 )
 from pyutube.downloader import download
 
 
 # Create CLI app
 app = typer.Typer(
     name="pyutube",
@@ -149,14 +151,15 @@
     elif link_type == "playlist":
         handle_playlist(url, path)
 
     else:
         error_console.print("❗ Unsupported link type.")
         sys.exit()
 
+    check_for_updates()
     sys.exit()
 
 
 def handle_video(url, path):
     """
     Downloads a video from the given URL and saves it to the specified path.
```

### Comparing `pyutube-1.2.0/pyutube/downloader.py` & `pyutube-1.2.1/pyutube/downloader.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     console,
     error_console,
     sanitize_filename,
     ask_rename_file,
     ask_resolution,
     rename_file,
     is_file_exists,
+    has_audio
 )
 
 import os
 import sys
 
 
 from yaspin import yaspin
@@ -74,16 +75,15 @@
             url,
             use_oauth=False,
             allow_oauth_cache=True,
             on_progress_callback=on_progress,
         )
 
     @yaspin(
-        text=colored("getting video headers ", "green") +
-        colored("(means the video won't be fully downloaded)", "yellow"),
+        text=colored("getting video streams", "green"),
         spinner=Spinners.point
     )
     def get_available_resolutions(self, video: YouTube) -> set:
         """
         Get a set of all available resolutions for the video.
 
         Args:
@@ -148,18 +148,14 @@
             video: The video for which audio streams are to be obtained.
 
         Returns:
             The first audio stream found in the video.
         """
         return video.streams.filter(only_audio=True).order_by('mime_type').first()
 
-    @yaspin(
-        text=colored("Saving the file...", "cyan"),
-        spinner=Spinners.smiley
-    )
     def save_file(self, video: YouTube, path: str, filename: str) -> None:
         """
         Save the file to the specified path with the given filename.
 
         Args:
             video: The video to be saved.
             path: The path where the video will be saved.
@@ -384,23 +380,23 @@
         # If file with the same name already exists in the path
         if is_file_exists(self.path, video_filename):
             video_filename = self.handle_existing_file(video_filename)
             if not video_filename:
                 sys.exit()
         try:
             self.save_file(footage, self.path, video_filename)
-            if not self.is_audio:
+            if not self.is_audio and not has_audio(video_filename, os.path.join(self.path, audio_filename)):
                 self.save_file(video_audio, self.path, audio_filename)
                 self.merging(video_filename, audio_filename)
 
         except Exception as error:
             error_console.print(f"Error: {error}")
             sys.exit()
 
-        console.print("✅ Download completed", style="info")
+        console.print("\n\n\n✅ Download completed", style="info")
         return True
 
     def get_playlist_links(self):
         """
         Get the playlist links from the URL.
 
         Args:
```

### Comparing `pyutube-1.2.0/pyutube/tests/test_utils.py` & `pyutube-1.2.1/pyutube/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `pyutube-1.2.0/pyutube/utils.py` & `pyutube-1.2.1/pyutube/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,17 +9,20 @@
 import inquirer
 import requests
 from yaspin import yaspin
 from yaspin.spinners import Spinners
 from rich.console import Console
 from rich.theme import Theme
 from termcolor import colored
+from moviepy.tools import subprocess_call
+from moviepy.config import get_setting
 
 
-__version__ = "1.2.0"
+__version__ = "1.2.1"
+__app__ = "pyutube"
 ABORTED_PREFIX = "aborted"
 CANCEL_PREFIX = "cancel"
 
 # Set up the console
 custom_theme = Theme({
     "info": "#64b0f2",
     "warning": "color(3)",
@@ -378,7 +381,60 @@
     if file_type_choice.startswith(CANCEL_PREFIX):
         error_console.print("❗ Cancel the download...")
         sys.exit()
     elif file_type_choice.startswith(ABORTED_PREFIX):
         sys.exit()
 
     return is_audio
+
+
+def has_audio(input_file, output, bitrate=3000, fps=44100):
+    """ extract the sound from a video file and save it in ``output`` """
+
+    try:
+        cmd = [
+            get_setting("FFMPEG_BINARY"),
+            "-y",
+            "-i",
+            input_file,
+            "-ab",
+            "%dk" % bitrate,
+            "-ar",
+            "%d" % fps,
+            output
+        ]
+        subprocess_call(cmd, logger=None)
+    except Exception as error:
+        return False
+
+    os.remove(output)
+    return True
+
+
+def check_for_updates() -> None:
+    """
+    A function to check for updates of a given package.
+
+    Returns:
+        None
+    """
+    try:
+        r = requests.get(
+            f'https://pypi.org/pypi/{__app__}/json', headers={'Accept': 'application/json'})
+    except Exception as error:
+        error_console.print(f"❗ Error checking for updates: {error}")
+    else:
+        if r.status_code == 200:
+            latest_version = r.json()['info']['version']
+            if latest_version != __version__:
+                console.print(
+                    f"👉 A new version of {__app__} is available: {latest_version}. Update it by running [bold red link=https://github.com/Hetari/pyutube]pip install --upgrade {__app__}[/bold red link]",
+                    style="warning"
+                )
+        else:
+            error_console.print(
+                f"❗ Error checking for updates: {r.status_code}")
+            sys.exit()
+
+
+if __name__ == "__main__":
+    check_for_updates()
```

### Comparing `pyutube-1.2.0/setup.py` & `pyutube-1.2.1/setup.py`

 * *Files identical despite different names*

