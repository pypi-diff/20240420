# Comparing `tmp/thepipe_api-0.2.6.tar.gz` & `tmp/thepipe_api-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thepipe_api-0.2.6.tar", last modified: Wed Apr 17 21:46:04 2024, max compression
+gzip compressed data, was "thepipe_api-0.2.7.tar", last modified: Fri Apr 19 14:53:20 2024, max compression
```

## Comparing `thepipe_api-0.2.6.tar` & `thepipe_api-0.2.7.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-04-17 21:46:04.879906 thepipe_api-0.2.6/
--rw-rw-rw-   0        0        0     1094 2024-03-27 18:15:40.000000 thepipe_api-0.2.6/LICENSE
--rw-rw-rw-   0        0        0    10064 2024-04-17 21:46:04.878898 thepipe_api-0.2.6/PKG-INFO
--rw-rw-rw-   0        0        0     9337 2024-04-17 14:56:48.000000 thepipe_api-0.2.6/README.md
--rw-rw-rw-   0        0        0       42 2024-04-17 21:46:04.879906 thepipe_api-0.2.6/setup.cfg
--rw-rw-rw-   0        0        0      859 2024-04-17 21:43:17.000000 thepipe_api-0.2.6/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-17 21:46:04.825898 thepipe_api-0.2.6/tests/
--rw-rw-rw-   0        0        0        0 2024-03-23 01:45:32.000000 thepipe_api-0.2.6/tests/__init__.py
--rw-rw-rw-   0        0        0     9265 2024-04-16 16:00:52.000000 thepipe_api-0.2.6/tests/test_thepipe.py
-drwxrwxrwx   0        0        0        0 2024-04-17 21:46:04.857899 thepipe_api-0.2.6/thepipe_api/
--rw-rw-rw-   0        0        0       86 2024-04-15 22:46:19.000000 thepipe_api-0.2.6/thepipe_api/__init__.py
--rw-rw-rw-   0        0        0     4821 2024-04-13 20:40:22.000000 thepipe_api-0.2.6/thepipe_api/compressor.py
--rw-rw-rw-   0        0        0     2778 2024-04-16 05:18:22.000000 thepipe_api-0.2.6/thepipe_api/core.py
--rw-rw-rw-   0        0        0    20977 2024-04-17 06:23:20.000000 thepipe_api-0.2.6/thepipe_api/extractor.py
--rw-rw-rw-   0        0        0     3634 2024-04-17 21:42:35.000000 thepipe_api-0.2.6/thepipe_api/thepipe.py
-drwxrwxrwx   0        0        0        0 2024-04-17 21:46:04.877898 thepipe_api-0.2.6/thepipe_api.egg-info/
--rw-rw-rw-   0        0        0    10064 2024-04-17 21:46:04.000000 thepipe_api-0.2.6/thepipe_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      396 2024-04-17 21:46:04.000000 thepipe_api-0.2.6/thepipe_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-17 21:46:04.000000 thepipe_api-0.2.6/thepipe_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2024-04-17 21:46:04.000000 thepipe_api-0.2.6/thepipe_api.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      104 2024-04-17 21:46:04.000000 thepipe_api-0.2.6/thepipe_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-04-17 21:46:04.000000 thepipe_api-0.2.6/thepipe_api.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-19 14:53:20.733883 thepipe_api-0.2.7/
+-rw-rw-rw-   0        0        0     1094 2024-04-18 07:46:31.000000 thepipe_api-0.2.7/LICENSE
+-rw-rw-rw-   0        0        0    10866 2024-04-19 14:53:20.731881 thepipe_api-0.2.7/PKG-INFO
+-rw-rw-rw-   0        0        0    10109 2024-04-18 16:18:13.000000 thepipe_api-0.2.7/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-19 14:53:20.734882 thepipe_api-0.2.7/setup.cfg
+-rw-rw-rw-   0        0        0      859 2024-04-19 14:52:42.000000 thepipe_api-0.2.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-19 14:53:20.690881 thepipe_api-0.2.7/tests/
+-rw-rw-rw-   0        0        0        0 2024-04-18 07:46:31.000000 thepipe_api-0.2.7/tests/__init__.py
+-rw-rw-rw-   0        0        0     9265 2024-04-18 07:46:31.000000 thepipe_api-0.2.7/tests/test_thepipe.py
+drwxrwxrwx   0        0        0        0 2024-04-19 14:53:20.700883 thepipe_api-0.2.7/thepipe_api/
+-rw-rw-rw-   0        0        0       86 2024-04-18 07:46:31.000000 thepipe_api-0.2.7/thepipe_api/__init__.py
+-rw-rw-rw-   0        0        0     4821 2024-04-18 07:46:31.000000 thepipe_api-0.2.7/thepipe_api/compressor.py
+-rw-rw-rw-   0        0        0     2778 2024-04-19 14:45:09.000000 thepipe_api-0.2.7/thepipe_api/core.py
+-rw-rw-rw-   0        0        0    21113 2024-04-19 14:51:46.000000 thepipe_api-0.2.7/thepipe_api/extractor.py
+-rw-rw-rw-   0        0        0     3611 2024-04-19 14:51:46.000000 thepipe_api-0.2.7/thepipe_api/thepipe.py
+drwxrwxrwx   0        0        0        0 2024-04-19 14:53:20.729884 thepipe_api-0.2.7/thepipe_api.egg-info/
+-rw-rw-rw-   0        0        0    10866 2024-04-19 14:53:20.000000 thepipe_api-0.2.7/thepipe_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      396 2024-04-19 14:53:20.000000 thepipe_api-0.2.7/thepipe_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-19 14:53:20.000000 thepipe_api-0.2.7/thepipe_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2024-04-19 14:53:20.000000 thepipe_api-0.2.7/thepipe_api.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      118 2024-04-19 14:53:20.000000 thepipe_api-0.2.7/thepipe_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-04-19 14:53:20.000000 thepipe_api-0.2.7/thepipe_api.egg-info/top_level.txt
```

### Comparing `thepipe_api-0.2.6/LICENSE` & `thepipe_api-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `thepipe_api-0.2.6/PKG-INFO` & `thepipe_api-0.2.7/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,42 +1,18 @@
-Metadata-Version: 2.1
-Name: thepipe_api
-Version: 0.2.6
-Summary: Automate information extraction for multimodal LLMs.
-Home-page: https://github.com/emcf/thepipe
-Author: Emmett McFarlane
-Author-email: emmett@thepi.pe
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: aiohttp
-Requires-Dist: charset-normalizer
-Requires-Dist: Pyarrow
-Requires-Dist: python-magic
-Requires-Dist: colorama
-Requires-Dist: requests
-Requires-Dist: pillow
-Requires-Dist: cssutils
-Requires-Dist: beautifulsoup4
-Requires-Dist: magika
-
 
 # <a href="https://thepi.pe/"><img src="https://rpnutzemutbrumczwvue.supabase.co/storage/v1/object/public/assets/pipeline_small%20(1).png" alt="Pipeline Illustration" style="width:96px; height:72px; vertical-align:middle;"> The Pipe</a>
 <p>
   <a href="https://github.com/emcf/thepipe/blob/main/README.md">English</a> | <a href="https://github.com/emcf/thepipe/blob/main/README_cn.md">中文</a>
 </p>
 
 [![codecov](https://codecov.io/gh/emcf/thepipe/graph/badge.svg?token=OE7CUEFUL9)](https://codecov.io/gh/emcf/thepipe) ![python-gh-action](https://github.com/emcf/thepipe/actions/workflows/python-ci.yml/badge.svg) <a href="https://thepi.pe/">![Website](https://img.shields.io/website?url=https%3A%2F%2Fthepipe.up.railway.app%2F&label=API%20status)</a> <a href="https://thepi.pe/">![get API](https://img.shields.io/badge/API-get%20access-blue)</a>
 
 ### Feed PDFs, word docs, slides, web pages and more into Vision-LLMs with one line of code ⚡
 
-The Pipe is a multimodal-first tool for feeding files and web pages into vision-language models such as GPT-4V. It is best for LLM and RAG applications that require a deep understanding of tricky data sources. The Pipe is available as a hosted API at [thepi.pe](https://thepi.pe), or it can be set up locally.
+The Pipe is a multimodal-first tool for feeding files and web pages into vision-language models such as GPT-4V. It is best for LLM and RAG applications that require a deep understanding of tricky data sources. The Pipe is available as a hosted API at [thepi.pe](https://thepi.pe), or it can be set up locally. 
 
 ![Demo](https://ngrdaaykhfrmtpodlakn.supabase.co/storage/v1/object/public/assets/demo.gif?t=2024-03-24T19%3A13%3A46.695Z)
 
 ## Features 🌟
 
 - Extracts text and visuals from files or web pages 📚
 - Outputs chunks optimized for multimodal LLMs 🖼️
@@ -44,41 +20,44 @@
 - Auto-compress prompts exceeding your chosen token limit 📦
 - Works even with missing file extensions, in-memory data streams 💾
 - Works with codebases, git repos, and custom integrations 🌐
 - Multi-threaded ⚡️
 
 ## Getting Started  🚀
 
+The Pipe handles a wide array of complex filetypes, and thus has many dependencies that must be installed separately. It also requires a strong machine for good response times. For this reason, we host it as an API that works out-of-the-box. 
+
 First, install The Pipe. 
 ```
 pip install thepipe_api
 ```
 
-Ensure the `THEPIPE_API_KEY` environment variable is set. Don't have an API key yet? [Get one here](https://thepi.pe). Alternatively, see the local installation section for the more advanced local setup.
+The Pipe is available as a hosted API, or it can be set up locally. An API key is recommended for out-of-the-box functionality (alternatively, see the local installation section). Ensure the `THEPIPE_API_KEY` environment variable is set. Don't have a key yet? [Get one here](https://thepi.pe).
 
 Now you can extract comprehensive text and visuals from any file:
 ```python
 from thepipe_api import thepipe
-chunks = thepipe.extract("example.pdf")
+messages = thepipe.extract("example.pdf")
 ```
 Or any website:
 ```python
-chunks = thepipe.extract("https://example.com")
+messages = thepipe.extract("https://example.com")
 ```
 Then feed it into GPT-4-Vision:
 ```python
 response = client.chat.completions.create(
     model="gpt-4-vision-preview",
-    messages = chunks,
+    messages = messages,
 )
 ```
-The Pipe's output is a list of sensible "chunks", and thus can be used either for storage in a vector database or for direct use as a prompt. Extra features such as data table extraction, bar chart extraction, custom web authentications and more are available in the [API documentation](https://thepi.pe/docs). [LiteLLM](https://github.com/BerriAI/litellm) can be used to easily integrate The Pipe with any LLM provider.
+
+![Just call OpenAI](https://rpnutzemutbrumczwvue.supabase.co/storage/v1/object/public/assets/IMG_0180.jpg)
 
 You can also use The Pipe from the command line. Here's how to recursively extract from a directory, matching only a specific file type:
-```
+```bash
 thepipe path/to/folder --match *jsx
 ```
 
 ## Supported File Types 📚
 
 | Source Type                           | Input types        | Token Compression 🗜️ | Image Extraction 👁️ | Notes 📌                                                  |
 |---------------------------------------|------------------------------------------|-------------------|------------------|---------------------------------------------------------|
@@ -91,29 +70,45 @@
 | Jupyter Notebook                      | `.ipynb`                                | ❌               | ✔️               | Extracts code, markdown, and images from Jupyter notebooks                                  |
 | Microsoft Word Document               | `.docx`                                 | ✔️               | ✔️               | Extracts text and images from Word documents                                        |
 | Microsoft PowerPoint Presentation     | `.pptx`                                 | ✔️               | ✔️               | Extracts text and images from PowerPoint presentations                              |
 | Website                               | URLs (inputs containing `http`, `https`, `ftp`)             | ✔️                | ✔️    | Extracts text from web page along with image (or images if scrollable); text-only extraction available          |
 | GitHub Repository                     | GitHub repo URLs                         | ✔️               | ✔️                | Extracts from GitHub repositories; supports branch specification         |
 | ZIP File                              | `.zip`                                  | ✔️               | ✔️                | Extracts contents of ZIP files; supports nested directory extraction     |
 
-##  How it works 🛠️
+## How it works 🛠️
 
-The pipe is accessible from the command line or from [Python](https://www.python.org/downloads/). The input source is either a file path, a URL, or a directory. The pipe will extract information from the source and process it for downstream use with [language models](https://en.wikipedia.org/wiki/Large_language_model), [vision transformers](https://en.wikipedia.org/wiki/Vision_transformer), or [vision-language models](https://arxiv.org/abs/2304.00685). The output from the pipe is a sensible text-based (or multimodal) representation of the extracted information, carefully crafted to fit within context windows for any models from [gemma-7b](https://huggingface.co/google/gemma-7b) to [GPT-4](https://openai.com/gpt-4). It uses a variety of heuristics for optimal performance with vision-language models, including AI filetype detection with [filetype detection](https://opensource.googleblog.com/2024/02/magika-ai-powered-fast-and-efficient-file-type-identification.html), AI [PDF extraction](thepi.pe/docs), efficient [token compression](https://arxiv.org/abs/2403.12968), automatic [image encoding](https://en.wikipedia.org/wiki/Base64), [reranking](https://arxiv.org/abs/2310.06839) for [lost-in-the-middle](https://arxiv.org/abs/2307.03172) effects, and more, all pre-built to work out-of-the-box.
+The input source is either a file path, a URL, or a directory. The pipe will extract information from the source and process it for downstream use with [language models](https://en.wikipedia.org/wiki/Large_language_model), [vision transformers](https://en.wikipedia.org/wiki/Vision_transformer), or [vision-language models](https://arxiv.org/abs/2304.00685). The output from the pipe is a sensible list of multimodal messages representing chunks of the extracted information, carefully crafted to fit within context windows for any models from [gemma-7b](https://huggingface.co/google/gemma-7b) to [GPT-4](https://openai.com/gpt-4). The messages returned should look like this:
+```json
+[
+  {
+    "type": "text",
+    "content": "Extracted text here..."
+  },
+  {
+    "type": "image_url",
+    "image_url": {
+      "url": "data:image/jpeg;base64,..."}
+  },
+]
+```
+The text and images from these messages may also be prepared for a vector database with `thepipe.core.create_chunks_from_messages` or for downstream use with RAG frameworks. [LiteLLM](https://github.com/BerriAI/litellm) can be used to easily integrate The Pipe with any LLM provider. 
+
+It uses a variety of heuristics for optimal performance with vision-language models, including AI filetype detection with [filetype detection](https://opensource.googleblog.com/2024/02/magika-ai-powered-fast-and-efficient-file-type-identification.html), opt-in AI [PDF extraction](thepi.pe/docs), efficient [token compression](https://arxiv.org/abs/2403.12968), automatic [image encoding](https://en.wikipedia.org/wiki/Base64), [reranking](https://arxiv.org/abs/2310.06839) for [lost-in-the-middle](https://arxiv.org/abs/2307.03172) effects, and more, all pre-built to work out-of-the-box.
 
 
 ## Local Installation 🛠️
 
-To use The Pipe locally, you will need [playwright](https://github.com/microsoft/playwright), [ctags](https://github.com/universal-ctags/), [pytesseract](https://github.com/h/pytesseract), and the local python requirements, which differ from the more lightweight API requirements. You will also need to use the local version of the requirements file:
+The Pipe handles a wide array of complex filetypes, and thus requires installation of many different packages to function. It also requires a very capable machine for good response times. For this reason, we host it as an API that works out-of-the-box. To use The Pipe locally for free instead, you will need [playwright](https://github.com/microsoft/playwright), [ctags](https://github.com/universal-ctags/), [pytesseract](https://github.com/h/pytesseract), and the local python requirements, which differ from the more lightweight API requirements:
 
 ```bash
 git clone https://github.com/emcf/thepipe
 pip install -r requirements_local.txt
 ```
 
-Tip for windows users: you may need to install the python-libmagic binaries with `pip install python-magic-bin`. You may also need to ensure the tesseract-ocr binaries and the ctags binaries are in your PATH.
+Tip for windows users: Install the python-libmagic binaries with `pip install python-magic-bin`. Ensure the `tesseract-ocr` binaries and the `ctags` binaries are in your PATH.
 
 Now you can use The Pipe with Python:
 ```bash
 from thepipe_api import thepipe
 chunks = thepipe.extract("example.pdf", local=True)
 ```
 
@@ -123,16 +118,16 @@
 ```
 
 Arguments are:
 - `source` (required): can be a file path, a URL, or a directory path.
 - `local` (optional): Use the local version of The Pipe instead of the hosted API.
 - `match` (optional): Regex pattern to match files in the directory.
 - `ignore` (optional): Regex pattern to ignore files in the directory.
-- `limit` (optional): The token limit for the output prompt, defaults to 100K. Prompts exceeding the limit will be compressed.
+- `limit` (optional): The token limit for the output prompt, defaults to 100K. Prompts exceeding the limit will be compressed. This may not work as expected with the API, as it is in active development.
 - `ai_extraction` (optional): Extract tables, figures, and math from PDFs using our extractor. Incurs extra costs.
 - `text_only` (optional): Do not extract images from documents or websites. Additionally, image files will be represented with OCR instead of as images.
 
-<a href="https://cal.com/emmett-mcf/30min"><img alt="Book us with Cal.com" src="https://cal.com/book-with-cal-dark.svg" /></a>
-
 # Sponsors
 
-Thank you to [Cal.com](https://cal.com/) for sponsoring this project. 
+<a href="https://cal.com/emmett-mcf/30min"><img alt="Book us with Cal.com" src="https://cal.com/book-with-cal-dark.svg" /></a>
+
+Thank you to [Cal.com](https://cal.com/) for sponsoring this project. Contact emmett@thepi.pe for sponsorship information.
```

#### html2text {}

```diff
@@ -1,17 +1,8 @@
-Metadata-Version: 2.1 Name: thepipe_api Version: 0.2.6 Summary: Automate
-information extraction for multimodal LLMs. Home-page: https://github.com/emcf/
-thepipe Author: Emmett McFarlane Author-email: emmett@thepi.pe Classifier:
-Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
-License Classifier: Operating System :: OS Independent Requires-Python: >=3.6
-Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
-aiohttp Requires-Dist: charset-normalizer Requires-Dist: Pyarrow Requires-Dist:
-python-magic Requires-Dist: colorama Requires-Dist: requests Requires-Dist:
-pillow Requires-Dist: cssutils Requires-Dist: beautifulsoup4 Requires-Dist:
-magika # _[_P_i_p_e_l_i_n_e_ _I_l_l_u_s_t_r_a_t_i_o_n_]_T_h_e_ _P_i_p_e
+# _[_P_i_p_e_l_i_n_e_ _I_l_l_u_s_t_r_a_t_i_o_n_]_T_h_e_ _P_i_p_e
 _E_n_g_l_i_s_h | _ä_¸_­_æ__
 [![codecov](https://codecov.io/gh/emcf/thepipe/graph/
 badge.svg?token=OE7CUEFUL9)](https://codecov.io/gh/emcf/thepipe) ![python-gh-
 action](https://github.com/emcf/thepipe/actions/workflows/python-ci.yml/
 badge.svg) _!_[_W_e_b_s_i_t_e_]_(_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
 _w_e_b_s_i_t_e_?_u_r_l_=_h_t_t_p_s_%_3_A_%_2_F_%_2_F_t_h_e_p_i_p_e_._u_p_._r_a_i_l_w_a_y_._a_p_p_%_2_F_&_l_a_b_e_l_=_A_P_I_%_2_0_s_t_a_t_u_s_) _!_[_g_e_t
 _A_P_I_]_(_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_A_P_I_-_g_e_t_%_2_0_a_c_c_e_s_s_-_b_l_u_e_) ### Feed PDFs, word
@@ -23,88 +14,97 @@
 [Demo](https://ngrdaaykhfrmtpodlakn.supabase.co/storage/v1/object/public/
 assets/demo.gif?t=2024-03-24T19%3A13%3A46.695Z) ## Features ð - Extracts
 text and visuals from files or web pages ð - Outputs chunks optimized for
 multimodal LLMs ð¼ï¸ - Interpret complex PDFs, web pages, slides, CSVs, and
 more ð§  - Auto-compress prompts exceeding your chosen token limit ð¦ -
 Works even with missing file extensions, in-memory data streams ð¾ - Works
 with codebases, git repos, and custom integrations ð - Multi-threaded â¡ï¸
-## Getting Started ð First, install The Pipe. ``` pip install thepipe_api
-``` Ensure the `THEPIPE_API_KEY` environment variable is set. Don't have an API
-key yet? [Get one here](https://thepi.pe). Alternatively, see the local
-installation section for the more advanced local setup. Now you can extract
-comprehensive text and visuals from any file: ```python from thepipe_api import
-thepipe chunks = thepipe.extract("example.pdf") ``` Or any website: ```python
-chunks = thepipe.extract("https://example.com") ``` Then feed it into GPT-4-
-Vision: ```python response = client.chat.completions.create( model="gpt-4-
-vision-preview", messages = chunks, ) ``` The Pipe's output is a list of
-sensible "chunks", and thus can be used either for storage in a vector database
-or for direct use as a prompt. Extra features such as data table extraction,
-bar chart extraction, custom web authentications and more are available in the
-[API documentation](https://thepi.pe/docs). [LiteLLM](https://github.com/
+## Getting Started ð The Pipe handles a wide array of complex filetypes, and
+thus has many dependencies that must be installed separately. It also requires
+a strong machine for good response times. For this reason, we host it as an API
+that works out-of-the-box. First, install The Pipe. ``` pip install thepipe_api
+``` The Pipe is available as a hosted API, or it can be set up locally. An API
+key is recommended for out-of-the-box functionality (alternatively, see the
+local installation section). Ensure the `THEPIPE_API_KEY` environment variable
+is set. Don't have a key yet? [Get one here](https://thepi.pe). Now you can
+extract comprehensive text and visuals from any file: ```python from
+thepipe_api import thepipe messages = thepipe.extract("example.pdf") ``` Or any
+website: ```python messages = thepipe.extract("https://example.com") ``` Then
+feed it into GPT-4-Vision: ```python response = client.chat.completions.create
+( model="gpt-4-vision-preview", messages = messages, ) ``` ![Just call OpenAI]
+(https://rpnutzemutbrumczwvue.supabase.co/storage/v1/object/public/assets/
+IMG_0180.jpg) You can also use The Pipe from the command line. Here's how to
+recursively extract from a directory, matching only a specific file type:
+```bash thepipe path/to/folder --match *jsx ``` ## Supported File Types ð |
+Source Type | Input types | Token Compression ðï¸ | Image Extraction
+ðï¸ | Notes ð | |---------------------------------------|---------------
+---------------------------|-------------------|------------------|------------
+---------------------------------------------| | Directory | Any `/path/to/
+directory` | âï¸ | âï¸ | Extracts from all files in directory, supports
+match and ignore patterns | | Code | `.py`, `.tsx`, `.js`, `.html`, `.css`,
+`.cpp`, etc | âï¸ (varies) | â | Combines all code files. `.c`, `.cpp`,
+`.py` are compressible with ctags, others are not | | Plaintext | `.txt`,
+`.md`, `.rtf`, etc | âï¸ | â | Regular text files | | PDF | `.pdf` |
+âï¸ | âï¸ | Extracts text and images of each page; can use AI for
+extraction of table data and images within pages | | Image | `.jpg`, `.jpeg`,
+`.png` | â | âï¸ | Extracts images, uses OCR if text_only | | Data Table |
+`.csv`, `.xls`, `.xlsx` | âï¸ | â | Extracts data from spreadsheets;
+converts to text representation. For very large datasets, will only extract
+column names and types | | Jupyter Notebook | `.ipynb` | â | âï¸ |
+Extracts code, markdown, and images from Jupyter notebooks | | Microsoft Word
+Document | `.docx` | âï¸ | âï¸ | Extracts text and images from Word
+documents | | Microsoft PowerPoint Presentation | `.pptx` | âï¸ | âï¸ |
+Extracts text and images from PowerPoint presentations | | Website | URLs
+(inputs containing `http`, `https`, `ftp`) | âï¸ | âï¸ | Extracts text
+from web page along with image (or images if scrollable); text-only extraction
+available | | GitHub Repository | GitHub repo URLs | âï¸ | âï¸ | Extracts
+from GitHub repositories; supports branch specification | | ZIP File | `.zip` |
+âï¸ | âï¸ | Extracts contents of ZIP files; supports nested directory
+extraction | ## How it works ð ï¸ The input source is either a file path, a
+URL, or a directory. The pipe will extract information from the source and
+process it for downstream use with [language models](https://en.wikipedia.org/
+wiki/Large_language_model), [vision transformers](https://en.wikipedia.org/
+wiki/Vision_transformer), or [vision-language models](https://arxiv.org/abs/
+2304.00685). The output from the pipe is a sensible list of multimodal messages
+representing chunks of the extracted information, carefully crafted to fit
+within context windows for any models from [gemma-7b](https://huggingface.co/
+google/gemma-7b) to [GPT-4](https://openai.com/gpt-4). The messages returned
+should look like this: ```json [ { "type": "text", "content": "Extracted text
+here..." }, { "type": "image_url", "image_url": { "url": "data:image/
+jpeg;base64,..."} }, ] ``` The text and images from these messages may also be
+prepared for a vector database with `thepipe.core.create_chunks_from_messages`
+or for downstream use with RAG frameworks. [LiteLLM](https://github.com/
 BerriAI/litellm) can be used to easily integrate The Pipe with any LLM
-provider. You can also use The Pipe from the command line. Here's how to
-recursively extract from a directory, matching only a specific file type: ```
-thepipe path/to/folder --match *jsx ``` ## Supported File Types ð | Source
-Type | Input types | Token Compression ðï¸ | Image Extraction ðï¸ |
-Notes ð | |---------------------------------------|-------------------------
------------------|-------------------|------------------|----------------------
------------------------------------| | Directory | Any `/path/to/directory` |
-âï¸ | âï¸ | Extracts from all files in directory, supports match and
-ignore patterns | | Code | `.py`, `.tsx`, `.js`, `.html`, `.css`, `.cpp`, etc |
-âï¸ (varies) | â | Combines all code files. `.c`, `.cpp`, `.py` are
-compressible with ctags, others are not | | Plaintext | `.txt`, `.md`, `.rtf`,
-etc | âï¸ | â | Regular text files | | PDF | `.pdf` | âï¸ | âï¸ |
-Extracts text and images of each page; can use AI for extraction of table data
-and images within pages | | Image | `.jpg`, `.jpeg`, `.png` | â | âï¸ |
-Extracts images, uses OCR if text_only | | Data Table | `.csv`, `.xls`, `.xlsx`
-| âï¸ | â | Extracts data from spreadsheets; converts to text
-representation. For very large datasets, will only extract column names and
-types | | Jupyter Notebook | `.ipynb` | â | âï¸ | Extracts code, markdown,
-and images from Jupyter notebooks | | Microsoft Word Document | `.docx` |
-âï¸ | âï¸ | Extracts text and images from Word documents | | Microsoft
-PowerPoint Presentation | `.pptx` | âï¸ | âï¸ | Extracts text and images
-from PowerPoint presentations | | Website | URLs (inputs containing `http`,
-`https`, `ftp`) | âï¸ | âï¸ | Extracts text from web page along with
-image (or images if scrollable); text-only extraction available | | GitHub
-Repository | GitHub repo URLs | âï¸ | âï¸ | Extracts from GitHub
-repositories; supports branch specification | | ZIP File | `.zip` | âï¸ |
-âï¸ | Extracts contents of ZIP files; supports nested directory extraction |
-## How it works ð ï¸ The pipe is accessible from the command line or from
-[Python](https://www.python.org/downloads/). The input source is either a file
-path, a URL, or a directory. The pipe will extract information from the source
-and process it for downstream use with [language models](https://
-en.wikipedia.org/wiki/Large_language_model), [vision transformers](https://
-en.wikipedia.org/wiki/Vision_transformer), or [vision-language models](https://
-arxiv.org/abs/2304.00685). The output from the pipe is a sensible text-based
-(or multimodal) representation of the extracted information, carefully crafted
-to fit within context windows for any models from [gemma-7b](https://
-huggingface.co/google/gemma-7b) to [GPT-4](https://openai.com/gpt-4). It uses a
-variety of heuristics for optimal performance with vision-language models,
-including AI filetype detection with [filetype detection](https://
-opensource.googleblog.com/2024/02/magika-ai-powered-fast-and-efficient-file-
-type-identification.html), AI [PDF extraction](thepi.pe/docs), efficient [token
-compression](https://arxiv.org/abs/2403.12968), automatic [image encoding]
-(https://en.wikipedia.org/wiki/Base64), [reranking](https://arxiv.org/abs/
-2310.06839) for [lost-in-the-middle](https://arxiv.org/abs/2307.03172) effects,
-and more, all pre-built to work out-of-the-box. ## Local Installation ð ï¸
-To use The Pipe locally, you will need [playwright](https://github.com/
-microsoft/playwright), [ctags](https://github.com/universal-ctags/),
-[pytesseract](https://github.com/h/pytesseract), and the local python
-requirements, which differ from the more lightweight API requirements. You will
-also need to use the local version of the requirements file: ```bash git clone
-https://github.com/emcf/thepipe pip install -r requirements_local.txt ``` Tip
-for windows users: you may need to install the python-libmagic binaries with
-`pip install python-magic-bin`. You may also need to ensure the tesseract-ocr
-binaries and the ctags binaries are in your PATH. Now you can use The Pipe with
-Python: ```bash from thepipe_api import thepipe chunks = thepipe.extract
-("example.pdf", local=True) ``` or from the command line: ```bash thepipe path/
-to/folder --local ``` Arguments are: - `source` (required): can be a file path,
-a URL, or a directory path. - `local` (optional): Use the local version of The
-Pipe instead of the hosted API. - `match` (optional): Regex pattern to match
-files in the directory. - `ignore` (optional): Regex pattern to ignore files in
-the directory. - `limit` (optional): The token limit for the output prompt,
-defaults to 100K. Prompts exceeding the limit will be compressed. -
-`ai_extraction` (optional): Extract tables, figures, and math from PDFs using
-our extractor. Incurs extra costs. - `text_only` (optional): Do not extract
-images from documents or websites. Additionally, image files will be
-represented with OCR instead of as images. _[_B_o_o_k_ _u_s_ _w_i_t_h_ _C_a_l_._c_o_m_]# Sponsors
-Thank you to [Cal.com](https://cal.com/) for sponsoring this project.
+provider. It uses a variety of heuristics for optimal performance with vision-
+language models, including AI filetype detection with [filetype detection]
+(https://opensource.googleblog.com/2024/02/magika-ai-powered-fast-and-
+efficient-file-type-identification.html), opt-in AI [PDF extraction](thepi.pe/
+docs), efficient [token compression](https://arxiv.org/abs/2403.12968),
+automatic [image encoding](https://en.wikipedia.org/wiki/Base64), [reranking]
+(https://arxiv.org/abs/2310.06839) for [lost-in-the-middle](https://arxiv.org/
+abs/2307.03172) effects, and more, all pre-built to work out-of-the-box. ##
+Local Installation ð ï¸ The Pipe handles a wide array of complex filetypes,
+and thus requires installation of many different packages to function. It also
+requires a very capable machine for good response times. For this reason, we
+host it as an API that works out-of-the-box. To use The Pipe locally for free
+instead, you will need [playwright](https://github.com/microsoft/playwright),
+[ctags](https://github.com/universal-ctags/), [pytesseract](https://github.com/
+h/pytesseract), and the local python requirements, which differ from the more
+lightweight API requirements: ```bash git clone https://github.com/emcf/thepipe
+pip install -r requirements_local.txt ``` Tip for windows users: Install the
+python-libmagic binaries with `pip install python-magic-bin`. Ensure the
+`tesseract-ocr` binaries and the `ctags` binaries are in your PATH. Now you can
+use The Pipe with Python: ```bash from thepipe_api import thepipe chunks =
+thepipe.extract("example.pdf", local=True) ``` or from the command line:
+```bash thepipe path/to/folder --local ``` Arguments are: - `source`
+(required): can be a file path, a URL, or a directory path. - `local`
+(optional): Use the local version of The Pipe instead of the hosted API. -
+`match` (optional): Regex pattern to match files in the directory. - `ignore`
+(optional): Regex pattern to ignore files in the directory. - `limit`
+(optional): The token limit for the output prompt, defaults to 100K. Prompts
+exceeding the limit will be compressed. This may not work as expected with the
+API, as it is in active development. - `ai_extraction` (optional): Extract
+tables, figures, and math from PDFs using our extractor. Incurs extra costs. -
+`text_only` (optional): Do not extract images from documents or websites.
+Additionally, image files will be represented with OCR instead of as images. #
+Sponsors _[_B_o_o_k_ _u_s_ _w_i_t_h_ _C_a_l_._c_o_m_]Thank you to [Cal.com](https://cal.com/) for
+sponsoring this project. Contact emmett@thepi.pe for sponsorship information.
```

### Comparing `thepipe_api-0.2.6/README.md` & `thepipe_api-0.2.7/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,43 @@
+Metadata-Version: 2.1
+Name: thepipe_api
+Version: 0.2.7
+Summary: Automate information extraction for multimodal LLMs.
+Home-page: https://github.com/emcf/thepipe
+Author: Emmett McFarlane
+Author-email: emmett@thepi.pe
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: aiohttp
+Requires-Dist: charset-normalizer
+Requires-Dist: Pyarrow
+Requires-Dist: python-magic
+Requires-Dist: colorama
+Requires-Dist: requests
+Requires-Dist: pillow
+Requires-Dist: cssutils
+Requires-Dist: beautifulsoup4
+Requires-Dist: magika
+Requires-Dist: python-dotenv
+
 
 # <a href="https://thepi.pe/"><img src="https://rpnutzemutbrumczwvue.supabase.co/storage/v1/object/public/assets/pipeline_small%20(1).png" alt="Pipeline Illustration" style="width:96px; height:72px; vertical-align:middle;"> The Pipe</a>
 <p>
   <a href="https://github.com/emcf/thepipe/blob/main/README.md">English</a> | <a href="https://github.com/emcf/thepipe/blob/main/README_cn.md">中文</a>
 </p>
 
 [![codecov](https://codecov.io/gh/emcf/thepipe/graph/badge.svg?token=OE7CUEFUL9)](https://codecov.io/gh/emcf/thepipe) ![python-gh-action](https://github.com/emcf/thepipe/actions/workflows/python-ci.yml/badge.svg) <a href="https://thepi.pe/">![Website](https://img.shields.io/website?url=https%3A%2F%2Fthepipe.up.railway.app%2F&label=API%20status)</a> <a href="https://thepi.pe/">![get API](https://img.shields.io/badge/API-get%20access-blue)</a>
 
 ### Feed PDFs, word docs, slides, web pages and more into Vision-LLMs with one line of code ⚡
 
-The Pipe is a multimodal-first tool for feeding files and web pages into vision-language models such as GPT-4V. It is best for LLM and RAG applications that require a deep understanding of tricky data sources. The Pipe is available as a hosted API at [thepi.pe](https://thepi.pe), or it can be set up locally.
+The Pipe is a multimodal-first tool for feeding files and web pages into vision-language models such as GPT-4V. It is best for LLM and RAG applications that require a deep understanding of tricky data sources. The Pipe is available as a hosted API at [thepi.pe](https://thepi.pe), or it can be set up locally. 
 
 ![Demo](https://ngrdaaykhfrmtpodlakn.supabase.co/storage/v1/object/public/assets/demo.gif?t=2024-03-24T19%3A13%3A46.695Z)
 
 ## Features 🌟
 
 - Extracts text and visuals from files or web pages 📚
 - Outputs chunks optimized for multimodal LLMs 🖼️
@@ -20,41 +45,44 @@
 - Auto-compress prompts exceeding your chosen token limit 📦
 - Works even with missing file extensions, in-memory data streams 💾
 - Works with codebases, git repos, and custom integrations 🌐
 - Multi-threaded ⚡️
 
 ## Getting Started  🚀
 
+The Pipe handles a wide array of complex filetypes, and thus has many dependencies that must be installed separately. It also requires a strong machine for good response times. For this reason, we host it as an API that works out-of-the-box. 
+
 First, install The Pipe. 
 ```
 pip install thepipe_api
 ```
 
-Ensure the `THEPIPE_API_KEY` environment variable is set. Don't have an API key yet? [Get one here](https://thepi.pe). Alternatively, see the local installation section for the more advanced local setup.
+The Pipe is available as a hosted API, or it can be set up locally. An API key is recommended for out-of-the-box functionality (alternatively, see the local installation section). Ensure the `THEPIPE_API_KEY` environment variable is set. Don't have a key yet? [Get one here](https://thepi.pe).
 
 Now you can extract comprehensive text and visuals from any file:
 ```python
 from thepipe_api import thepipe
-chunks = thepipe.extract("example.pdf")
+messages = thepipe.extract("example.pdf")
 ```
 Or any website:
 ```python
-chunks = thepipe.extract("https://example.com")
+messages = thepipe.extract("https://example.com")
 ```
 Then feed it into GPT-4-Vision:
 ```python
 response = client.chat.completions.create(
     model="gpt-4-vision-preview",
-    messages = chunks,
+    messages = messages,
 )
 ```
-The Pipe's output is a list of sensible "chunks", and thus can be used either for storage in a vector database or for direct use as a prompt. Extra features such as data table extraction, bar chart extraction, custom web authentications and more are available in the [API documentation](https://thepi.pe/docs). [LiteLLM](https://github.com/BerriAI/litellm) can be used to easily integrate The Pipe with any LLM provider.
+
+![Just call OpenAI](https://rpnutzemutbrumczwvue.supabase.co/storage/v1/object/public/assets/IMG_0180.jpg)
 
 You can also use The Pipe from the command line. Here's how to recursively extract from a directory, matching only a specific file type:
-```
+```bash
 thepipe path/to/folder --match *jsx
 ```
 
 ## Supported File Types 📚
 
 | Source Type                           | Input types        | Token Compression 🗜️ | Image Extraction 👁️ | Notes 📌                                                  |
 |---------------------------------------|------------------------------------------|-------------------|------------------|---------------------------------------------------------|
@@ -67,29 +95,45 @@
 | Jupyter Notebook                      | `.ipynb`                                | ❌               | ✔️               | Extracts code, markdown, and images from Jupyter notebooks                                  |
 | Microsoft Word Document               | `.docx`                                 | ✔️               | ✔️               | Extracts text and images from Word documents                                        |
 | Microsoft PowerPoint Presentation     | `.pptx`                                 | ✔️               | ✔️               | Extracts text and images from PowerPoint presentations                              |
 | Website                               | URLs (inputs containing `http`, `https`, `ftp`)             | ✔️                | ✔️    | Extracts text from web page along with image (or images if scrollable); text-only extraction available          |
 | GitHub Repository                     | GitHub repo URLs                         | ✔️               | ✔️                | Extracts from GitHub repositories; supports branch specification         |
 | ZIP File                              | `.zip`                                  | ✔️               | ✔️                | Extracts contents of ZIP files; supports nested directory extraction     |
 
-##  How it works 🛠️
+## How it works 🛠️
 
-The pipe is accessible from the command line or from [Python](https://www.python.org/downloads/). The input source is either a file path, a URL, or a directory. The pipe will extract information from the source and process it for downstream use with [language models](https://en.wikipedia.org/wiki/Large_language_model), [vision transformers](https://en.wikipedia.org/wiki/Vision_transformer), or [vision-language models](https://arxiv.org/abs/2304.00685). The output from the pipe is a sensible text-based (or multimodal) representation of the extracted information, carefully crafted to fit within context windows for any models from [gemma-7b](https://huggingface.co/google/gemma-7b) to [GPT-4](https://openai.com/gpt-4). It uses a variety of heuristics for optimal performance with vision-language models, including AI filetype detection with [filetype detection](https://opensource.googleblog.com/2024/02/magika-ai-powered-fast-and-efficient-file-type-identification.html), AI [PDF extraction](thepi.pe/docs), efficient [token compression](https://arxiv.org/abs/2403.12968), automatic [image encoding](https://en.wikipedia.org/wiki/Base64), [reranking](https://arxiv.org/abs/2310.06839) for [lost-in-the-middle](https://arxiv.org/abs/2307.03172) effects, and more, all pre-built to work out-of-the-box.
+The input source is either a file path, a URL, or a directory. The pipe will extract information from the source and process it for downstream use with [language models](https://en.wikipedia.org/wiki/Large_language_model), [vision transformers](https://en.wikipedia.org/wiki/Vision_transformer), or [vision-language models](https://arxiv.org/abs/2304.00685). The output from the pipe is a sensible list of multimodal messages representing chunks of the extracted information, carefully crafted to fit within context windows for any models from [gemma-7b](https://huggingface.co/google/gemma-7b) to [GPT-4](https://openai.com/gpt-4). The messages returned should look like this:
+```json
+[
+  {
+    "type": "text",
+    "content": "Extracted text here..."
+  },
+  {
+    "type": "image_url",
+    "image_url": {
+      "url": "data:image/jpeg;base64,..."}
+  },
+]
+```
+The text and images from these messages may also be prepared for a vector database with `thepipe.core.create_chunks_from_messages` or for downstream use with RAG frameworks. [LiteLLM](https://github.com/BerriAI/litellm) can be used to easily integrate The Pipe with any LLM provider. 
+
+It uses a variety of heuristics for optimal performance with vision-language models, including AI filetype detection with [filetype detection](https://opensource.googleblog.com/2024/02/magika-ai-powered-fast-and-efficient-file-type-identification.html), opt-in AI [PDF extraction](thepi.pe/docs), efficient [token compression](https://arxiv.org/abs/2403.12968), automatic [image encoding](https://en.wikipedia.org/wiki/Base64), [reranking](https://arxiv.org/abs/2310.06839) for [lost-in-the-middle](https://arxiv.org/abs/2307.03172) effects, and more, all pre-built to work out-of-the-box.
 
 
 ## Local Installation 🛠️
 
-To use The Pipe locally, you will need [playwright](https://github.com/microsoft/playwright), [ctags](https://github.com/universal-ctags/), [pytesseract](https://github.com/h/pytesseract), and the local python requirements, which differ from the more lightweight API requirements. You will also need to use the local version of the requirements file:
+The Pipe handles a wide array of complex filetypes, and thus requires installation of many different packages to function. It also requires a very capable machine for good response times. For this reason, we host it as an API that works out-of-the-box. To use The Pipe locally for free instead, you will need [playwright](https://github.com/microsoft/playwright), [ctags](https://github.com/universal-ctags/), [pytesseract](https://github.com/h/pytesseract), and the local python requirements, which differ from the more lightweight API requirements:
 
 ```bash
 git clone https://github.com/emcf/thepipe
 pip install -r requirements_local.txt
 ```
 
-Tip for windows users: you may need to install the python-libmagic binaries with `pip install python-magic-bin`. You may also need to ensure the tesseract-ocr binaries and the ctags binaries are in your PATH.
+Tip for windows users: Install the python-libmagic binaries with `pip install python-magic-bin`. Ensure the `tesseract-ocr` binaries and the `ctags` binaries are in your PATH.
 
 Now you can use The Pipe with Python:
 ```bash
 from thepipe_api import thepipe
 chunks = thepipe.extract("example.pdf", local=True)
 ```
 
@@ -99,16 +143,16 @@
 ```
 
 Arguments are:
 - `source` (required): can be a file path, a URL, or a directory path.
 - `local` (optional): Use the local version of The Pipe instead of the hosted API.
 - `match` (optional): Regex pattern to match files in the directory.
 - `ignore` (optional): Regex pattern to ignore files in the directory.
-- `limit` (optional): The token limit for the output prompt, defaults to 100K. Prompts exceeding the limit will be compressed.
+- `limit` (optional): The token limit for the output prompt, defaults to 100K. Prompts exceeding the limit will be compressed. This may not work as expected with the API, as it is in active development.
 - `ai_extraction` (optional): Extract tables, figures, and math from PDFs using our extractor. Incurs extra costs.
 - `text_only` (optional): Do not extract images from documents or websites. Additionally, image files will be represented with OCR instead of as images.
 
-<a href="https://cal.com/emmett-mcf/30min"><img alt="Book us with Cal.com" src="https://cal.com/book-with-cal-dark.svg" /></a>
-
 # Sponsors
 
-Thank you to [Cal.com](https://cal.com/) for sponsoring this project. 
+<a href="https://cal.com/emmett-mcf/30min"><img alt="Book us with Cal.com" src="https://cal.com/book-with-cal-dark.svg" /></a>
+
+Thank you to [Cal.com](https://cal.com/) for sponsoring this project. Contact emmett@thepi.pe for sponsorship information.
```

#### html2text {}

```diff
@@ -1,8 +1,17 @@
-# _[_P_i_p_e_l_i_n_e_ _I_l_l_u_s_t_r_a_t_i_o_n_]_T_h_e_ _P_i_p_e
+Metadata-Version: 2.1 Name: thepipe_api Version: 0.2.7 Summary: Automate
+information extraction for multimodal LLMs. Home-page: https://github.com/emcf/
+thepipe Author: Emmett McFarlane Author-email: emmett@thepi.pe Classifier:
+Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
+License Classifier: Operating System :: OS Independent Requires-Python: >=3.6
+Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
+aiohttp Requires-Dist: charset-normalizer Requires-Dist: Pyarrow Requires-Dist:
+python-magic Requires-Dist: colorama Requires-Dist: requests Requires-Dist:
+pillow Requires-Dist: cssutils Requires-Dist: beautifulsoup4 Requires-Dist:
+magika Requires-Dist: python-dotenv # _[_P_i_p_e_l_i_n_e_ _I_l_l_u_s_t_r_a_t_i_o_n_]_T_h_e_ _P_i_p_e
 _E_n_g_l_i_s_h | _ä_¸_­_æ__
 [![codecov](https://codecov.io/gh/emcf/thepipe/graph/
 badge.svg?token=OE7CUEFUL9)](https://codecov.io/gh/emcf/thepipe) ![python-gh-
 action](https://github.com/emcf/thepipe/actions/workflows/python-ci.yml/
 badge.svg) _!_[_W_e_b_s_i_t_e_]_(_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
 _w_e_b_s_i_t_e_?_u_r_l_=_h_t_t_p_s_%_3_A_%_2_F_%_2_F_t_h_e_p_i_p_e_._u_p_._r_a_i_l_w_a_y_._a_p_p_%_2_F_&_l_a_b_e_l_=_A_P_I_%_2_0_s_t_a_t_u_s_) _!_[_g_e_t
 _A_P_I_]_(_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_A_P_I_-_g_e_t_%_2_0_a_c_c_e_s_s_-_b_l_u_e_) ### Feed PDFs, word
@@ -14,88 +23,97 @@
 [Demo](https://ngrdaaykhfrmtpodlakn.supabase.co/storage/v1/object/public/
 assets/demo.gif?t=2024-03-24T19%3A13%3A46.695Z) ## Features ð - Extracts
 text and visuals from files or web pages ð - Outputs chunks optimized for
 multimodal LLMs ð¼ï¸ - Interpret complex PDFs, web pages, slides, CSVs, and
 more ð§  - Auto-compress prompts exceeding your chosen token limit ð¦ -
 Works even with missing file extensions, in-memory data streams ð¾ - Works
 with codebases, git repos, and custom integrations ð - Multi-threaded â¡ï¸
-## Getting Started ð First, install The Pipe. ``` pip install thepipe_api
-``` Ensure the `THEPIPE_API_KEY` environment variable is set. Don't have an API
-key yet? [Get one here](https://thepi.pe). Alternatively, see the local
-installation section for the more advanced local setup. Now you can extract
-comprehensive text and visuals from any file: ```python from thepipe_api import
-thepipe chunks = thepipe.extract("example.pdf") ``` Or any website: ```python
-chunks = thepipe.extract("https://example.com") ``` Then feed it into GPT-4-
-Vision: ```python response = client.chat.completions.create( model="gpt-4-
-vision-preview", messages = chunks, ) ``` The Pipe's output is a list of
-sensible "chunks", and thus can be used either for storage in a vector database
-or for direct use as a prompt. Extra features such as data table extraction,
-bar chart extraction, custom web authentications and more are available in the
-[API documentation](https://thepi.pe/docs). [LiteLLM](https://github.com/
+## Getting Started ð The Pipe handles a wide array of complex filetypes, and
+thus has many dependencies that must be installed separately. It also requires
+a strong machine for good response times. For this reason, we host it as an API
+that works out-of-the-box. First, install The Pipe. ``` pip install thepipe_api
+``` The Pipe is available as a hosted API, or it can be set up locally. An API
+key is recommended for out-of-the-box functionality (alternatively, see the
+local installation section). Ensure the `THEPIPE_API_KEY` environment variable
+is set. Don't have a key yet? [Get one here](https://thepi.pe). Now you can
+extract comprehensive text and visuals from any file: ```python from
+thepipe_api import thepipe messages = thepipe.extract("example.pdf") ``` Or any
+website: ```python messages = thepipe.extract("https://example.com") ``` Then
+feed it into GPT-4-Vision: ```python response = client.chat.completions.create
+( model="gpt-4-vision-preview", messages = messages, ) ``` ![Just call OpenAI]
+(https://rpnutzemutbrumczwvue.supabase.co/storage/v1/object/public/assets/
+IMG_0180.jpg) You can also use The Pipe from the command line. Here's how to
+recursively extract from a directory, matching only a specific file type:
+```bash thepipe path/to/folder --match *jsx ``` ## Supported File Types ð |
+Source Type | Input types | Token Compression ðï¸ | Image Extraction
+ðï¸ | Notes ð | |---------------------------------------|---------------
+---------------------------|-------------------|------------------|------------
+---------------------------------------------| | Directory | Any `/path/to/
+directory` | âï¸ | âï¸ | Extracts from all files in directory, supports
+match and ignore patterns | | Code | `.py`, `.tsx`, `.js`, `.html`, `.css`,
+`.cpp`, etc | âï¸ (varies) | â | Combines all code files. `.c`, `.cpp`,
+`.py` are compressible with ctags, others are not | | Plaintext | `.txt`,
+`.md`, `.rtf`, etc | âï¸ | â | Regular text files | | PDF | `.pdf` |
+âï¸ | âï¸ | Extracts text and images of each page; can use AI for
+extraction of table data and images within pages | | Image | `.jpg`, `.jpeg`,
+`.png` | â | âï¸ | Extracts images, uses OCR if text_only | | Data Table |
+`.csv`, `.xls`, `.xlsx` | âï¸ | â | Extracts data from spreadsheets;
+converts to text representation. For very large datasets, will only extract
+column names and types | | Jupyter Notebook | `.ipynb` | â | âï¸ |
+Extracts code, markdown, and images from Jupyter notebooks | | Microsoft Word
+Document | `.docx` | âï¸ | âï¸ | Extracts text and images from Word
+documents | | Microsoft PowerPoint Presentation | `.pptx` | âï¸ | âï¸ |
+Extracts text and images from PowerPoint presentations | | Website | URLs
+(inputs containing `http`, `https`, `ftp`) | âï¸ | âï¸ | Extracts text
+from web page along with image (or images if scrollable); text-only extraction
+available | | GitHub Repository | GitHub repo URLs | âï¸ | âï¸ | Extracts
+from GitHub repositories; supports branch specification | | ZIP File | `.zip` |
+âï¸ | âï¸ | Extracts contents of ZIP files; supports nested directory
+extraction | ## How it works ð ï¸ The input source is either a file path, a
+URL, or a directory. The pipe will extract information from the source and
+process it for downstream use with [language models](https://en.wikipedia.org/
+wiki/Large_language_model), [vision transformers](https://en.wikipedia.org/
+wiki/Vision_transformer), or [vision-language models](https://arxiv.org/abs/
+2304.00685). The output from the pipe is a sensible list of multimodal messages
+representing chunks of the extracted information, carefully crafted to fit
+within context windows for any models from [gemma-7b](https://huggingface.co/
+google/gemma-7b) to [GPT-4](https://openai.com/gpt-4). The messages returned
+should look like this: ```json [ { "type": "text", "content": "Extracted text
+here..." }, { "type": "image_url", "image_url": { "url": "data:image/
+jpeg;base64,..."} }, ] ``` The text and images from these messages may also be
+prepared for a vector database with `thepipe.core.create_chunks_from_messages`
+or for downstream use with RAG frameworks. [LiteLLM](https://github.com/
 BerriAI/litellm) can be used to easily integrate The Pipe with any LLM
-provider. You can also use The Pipe from the command line. Here's how to
-recursively extract from a directory, matching only a specific file type: ```
-thepipe path/to/folder --match *jsx ``` ## Supported File Types ð | Source
-Type | Input types | Token Compression ðï¸ | Image Extraction ðï¸ |
-Notes ð | |---------------------------------------|-------------------------
------------------|-------------------|------------------|----------------------
------------------------------------| | Directory | Any `/path/to/directory` |
-âï¸ | âï¸ | Extracts from all files in directory, supports match and
-ignore patterns | | Code | `.py`, `.tsx`, `.js`, `.html`, `.css`, `.cpp`, etc |
-âï¸ (varies) | â | Combines all code files. `.c`, `.cpp`, `.py` are
-compressible with ctags, others are not | | Plaintext | `.txt`, `.md`, `.rtf`,
-etc | âï¸ | â | Regular text files | | PDF | `.pdf` | âï¸ | âï¸ |
-Extracts text and images of each page; can use AI for extraction of table data
-and images within pages | | Image | `.jpg`, `.jpeg`, `.png` | â | âï¸ |
-Extracts images, uses OCR if text_only | | Data Table | `.csv`, `.xls`, `.xlsx`
-| âï¸ | â | Extracts data from spreadsheets; converts to text
-representation. For very large datasets, will only extract column names and
-types | | Jupyter Notebook | `.ipynb` | â | âï¸ | Extracts code, markdown,
-and images from Jupyter notebooks | | Microsoft Word Document | `.docx` |
-âï¸ | âï¸ | Extracts text and images from Word documents | | Microsoft
-PowerPoint Presentation | `.pptx` | âï¸ | âï¸ | Extracts text and images
-from PowerPoint presentations | | Website | URLs (inputs containing `http`,
-`https`, `ftp`) | âï¸ | âï¸ | Extracts text from web page along with
-image (or images if scrollable); text-only extraction available | | GitHub
-Repository | GitHub repo URLs | âï¸ | âï¸ | Extracts from GitHub
-repositories; supports branch specification | | ZIP File | `.zip` | âï¸ |
-âï¸ | Extracts contents of ZIP files; supports nested directory extraction |
-## How it works ð ï¸ The pipe is accessible from the command line or from
-[Python](https://www.python.org/downloads/). The input source is either a file
-path, a URL, or a directory. The pipe will extract information from the source
-and process it for downstream use with [language models](https://
-en.wikipedia.org/wiki/Large_language_model), [vision transformers](https://
-en.wikipedia.org/wiki/Vision_transformer), or [vision-language models](https://
-arxiv.org/abs/2304.00685). The output from the pipe is a sensible text-based
-(or multimodal) representation of the extracted information, carefully crafted
-to fit within context windows for any models from [gemma-7b](https://
-huggingface.co/google/gemma-7b) to [GPT-4](https://openai.com/gpt-4). It uses a
-variety of heuristics for optimal performance with vision-language models,
-including AI filetype detection with [filetype detection](https://
-opensource.googleblog.com/2024/02/magika-ai-powered-fast-and-efficient-file-
-type-identification.html), AI [PDF extraction](thepi.pe/docs), efficient [token
-compression](https://arxiv.org/abs/2403.12968), automatic [image encoding]
-(https://en.wikipedia.org/wiki/Base64), [reranking](https://arxiv.org/abs/
-2310.06839) for [lost-in-the-middle](https://arxiv.org/abs/2307.03172) effects,
-and more, all pre-built to work out-of-the-box. ## Local Installation ð ï¸
-To use The Pipe locally, you will need [playwright](https://github.com/
-microsoft/playwright), [ctags](https://github.com/universal-ctags/),
-[pytesseract](https://github.com/h/pytesseract), and the local python
-requirements, which differ from the more lightweight API requirements. You will
-also need to use the local version of the requirements file: ```bash git clone
-https://github.com/emcf/thepipe pip install -r requirements_local.txt ``` Tip
-for windows users: you may need to install the python-libmagic binaries with
-`pip install python-magic-bin`. You may also need to ensure the tesseract-ocr
-binaries and the ctags binaries are in your PATH. Now you can use The Pipe with
-Python: ```bash from thepipe_api import thepipe chunks = thepipe.extract
-("example.pdf", local=True) ``` or from the command line: ```bash thepipe path/
-to/folder --local ``` Arguments are: - `source` (required): can be a file path,
-a URL, or a directory path. - `local` (optional): Use the local version of The
-Pipe instead of the hosted API. - `match` (optional): Regex pattern to match
-files in the directory. - `ignore` (optional): Regex pattern to ignore files in
-the directory. - `limit` (optional): The token limit for the output prompt,
-defaults to 100K. Prompts exceeding the limit will be compressed. -
-`ai_extraction` (optional): Extract tables, figures, and math from PDFs using
-our extractor. Incurs extra costs. - `text_only` (optional): Do not extract
-images from documents or websites. Additionally, image files will be
-represented with OCR instead of as images. _[_B_o_o_k_ _u_s_ _w_i_t_h_ _C_a_l_._c_o_m_]# Sponsors
-Thank you to [Cal.com](https://cal.com/) for sponsoring this project.
+provider. It uses a variety of heuristics for optimal performance with vision-
+language models, including AI filetype detection with [filetype detection]
+(https://opensource.googleblog.com/2024/02/magika-ai-powered-fast-and-
+efficient-file-type-identification.html), opt-in AI [PDF extraction](thepi.pe/
+docs), efficient [token compression](https://arxiv.org/abs/2403.12968),
+automatic [image encoding](https://en.wikipedia.org/wiki/Base64), [reranking]
+(https://arxiv.org/abs/2310.06839) for [lost-in-the-middle](https://arxiv.org/
+abs/2307.03172) effects, and more, all pre-built to work out-of-the-box. ##
+Local Installation ð ï¸ The Pipe handles a wide array of complex filetypes,
+and thus requires installation of many different packages to function. It also
+requires a very capable machine for good response times. For this reason, we
+host it as an API that works out-of-the-box. To use The Pipe locally for free
+instead, you will need [playwright](https://github.com/microsoft/playwright),
+[ctags](https://github.com/universal-ctags/), [pytesseract](https://github.com/
+h/pytesseract), and the local python requirements, which differ from the more
+lightweight API requirements: ```bash git clone https://github.com/emcf/thepipe
+pip install -r requirements_local.txt ``` Tip for windows users: Install the
+python-libmagic binaries with `pip install python-magic-bin`. Ensure the
+`tesseract-ocr` binaries and the `ctags` binaries are in your PATH. Now you can
+use The Pipe with Python: ```bash from thepipe_api import thepipe chunks =
+thepipe.extract("example.pdf", local=True) ``` or from the command line:
+```bash thepipe path/to/folder --local ``` Arguments are: - `source`
+(required): can be a file path, a URL, or a directory path. - `local`
+(optional): Use the local version of The Pipe instead of the hosted API. -
+`match` (optional): Regex pattern to match files in the directory. - `ignore`
+(optional): Regex pattern to ignore files in the directory. - `limit`
+(optional): The token limit for the output prompt, defaults to 100K. Prompts
+exceeding the limit will be compressed. This may not work as expected with the
+API, as it is in active development. - `ai_extraction` (optional): Extract
+tables, figures, and math from PDFs using our extractor. Incurs extra costs. -
+`text_only` (optional): Do not extract images from documents or websites.
+Additionally, image files will be represented with OCR instead of as images. #
+Sponsors _[_B_o_o_k_ _u_s_ _w_i_t_h_ _C_a_l_._c_o_m_]Thank you to [Cal.com](https://cal.com/) for
+sponsoring this project. Contact emmett@thepi.pe for sponsorship information.
```

### Comparing `thepipe_api-0.2.6/setup.py` & `thepipe_api-0.2.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='thepipe_api',
-    version='0.2.6',
+    version='0.2.7',
     author='Emmett McFarlane',
     author_email='emmett@thepi.pe',
     description='Automate information extraction for multimodal LLMs.',
     long_description=open('README.md', encoding='utf-8').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/emcf/thepipe',
     packages=find_packages(),
```

### Comparing `thepipe_api-0.2.6/tests/test_thepipe.py` & `thepipe_api-0.2.7/tests/test_thepipe.py`

 * *Files identical despite different names*

### Comparing `thepipe_api-0.2.6/thepipe_api/compressor.py` & `thepipe_api-0.2.7/thepipe_api/compressor.py`

 * *Files identical despite different names*

### Comparing `thepipe_api-0.2.6/thepipe_api/core.py` & `thepipe_api-0.2.7/thepipe_api/core.py`

 * *Files identical despite different names*

### Comparing `thepipe_api-0.2.6/thepipe_api/extractor.py` & `thepipe_api-0.2.7/thepipe_api/extractor.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 import zipfile
 from PIL import Image
 import requests
 import json
 from .core import Chunk, print_status, SourceTypes, create_chunks_from_messages, API_URL
 import tempfile
 import mimetypes
+import dotenv
+dotenv.load_dotenv()
 
 FILES_TO_IGNORE = {'package-lock.json', '.gitignore', '.bin', '.pyc', '.pyo', '.exe', '.bat', '.dll', '.obj', '.o', '.a', '.lib', '.so', '.dylib', '.ncb', '.sdf', '.suo', '.pdb', '.idb', '.pyd', '.ipynb_checkpoints', '.npy', '.pth'} # Files to ignore, please feel free to customize!
 CODE_EXTENSIONS = {'.h', '.json', '.js', '.jsx', '.ts', '.tsx',  '.cs', '.java', '.html', '.css', '.ini', '.xml', '.yaml', '.xaml', '.sh'} # Plaintext files that should not be compressed with LLMLingua
 CTAGS_CODE_EXTENSIONS = {'.c', '.cpp', '.py'} # code files that work with ctags
 PLAINTEXT_EXTENSIONS = {'.txt', '.md', '.rtf'}
 IMAGE_EXTENSIONS = {'.jpg', '.jpeg', '.png'}
 SPREADSHEET_EXTENSIONS = {'.csv', '.xls', '.xlsx'}
@@ -58,14 +60,17 @@
         try:
             response = response.json()
         except json.JSONDecodeError:
             raise ValueError(f"Failed to extract from {file_path}. This may mean our backend couldn't handle this request. Response: {response}.")
         if 'error' in response:
             raise ValueError(f"{response['error']}")
         chunks = create_chunks_from_messages(response['messages'])
+        for c in chunks:
+            c.path = file_path
+            c.source_type = source_type
         return chunks
     try:    
         if source_type == SourceTypes.PDF:
             extraction = extract_pdf(file_path=file_path, ai_extraction=ai_extraction, text_only=text_only, verbose=verbose)
         elif source_type == SourceTypes.DOCX:
             extraction = extract_docx(file_path=file_path, verbose=verbose, text_only=text_only)
         elif source_type == SourceTypes.PPTX:
```

### Comparing `thepipe_api-0.2.6/thepipe_api/thepipe.py` & `thepipe_api-0.2.7/thepipe_api/thepipe.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     # Save the chunks to files
     text = ""
     n_images = 0
     for i, chunk in enumerate(chunks):
         if chunk is None:
             continue
         if chunk.text is not None:
-            text += f"""```\n{chunk.text}\n```\n\n"""
+            text += chunk.text
         if (chunk.image is not None) and (not text_only):
             if chunk.path is None:
                 clean_path = f"image"
             else:
                 clean_path = chunk.path.replace('/', '_').replace('\\', '_')
                 clean_path = re.sub(r"[^a-zA-Z0-9 _]", "", clean_path)
             chunk.image.convert('RGB').save(f'outputs/{clean_path}_{i}.jpg')
```

### Comparing `thepipe_api-0.2.6/thepipe_api.egg-info/PKG-INFO` & `thepipe_api-0.2.7/thepipe_api.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thepipe_api
-Version: 0.2.6
+Version: 0.2.7
 Summary: Automate information extraction for multimodal LLMs.
 Home-page: https://github.com/emcf/thepipe
 Author: Emmett McFarlane
 Author-email: emmett@thepi.pe
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -17,26 +17,27 @@
 Requires-Dist: python-magic
 Requires-Dist: colorama
 Requires-Dist: requests
 Requires-Dist: pillow
 Requires-Dist: cssutils
 Requires-Dist: beautifulsoup4
 Requires-Dist: magika
+Requires-Dist: python-dotenv
 
 
 # <a href="https://thepi.pe/"><img src="https://rpnutzemutbrumczwvue.supabase.co/storage/v1/object/public/assets/pipeline_small%20(1).png" alt="Pipeline Illustration" style="width:96px; height:72px; vertical-align:middle;"> The Pipe</a>
 <p>
   <a href="https://github.com/emcf/thepipe/blob/main/README.md">English</a> | <a href="https://github.com/emcf/thepipe/blob/main/README_cn.md">中文</a>
 </p>
 
 [![codecov](https://codecov.io/gh/emcf/thepipe/graph/badge.svg?token=OE7CUEFUL9)](https://codecov.io/gh/emcf/thepipe) ![python-gh-action](https://github.com/emcf/thepipe/actions/workflows/python-ci.yml/badge.svg) <a href="https://thepi.pe/">![Website](https://img.shields.io/website?url=https%3A%2F%2Fthepipe.up.railway.app%2F&label=API%20status)</a> <a href="https://thepi.pe/">![get API](https://img.shields.io/badge/API-get%20access-blue)</a>
 
 ### Feed PDFs, word docs, slides, web pages and more into Vision-LLMs with one line of code ⚡
 
-The Pipe is a multimodal-first tool for feeding files and web pages into vision-language models such as GPT-4V. It is best for LLM and RAG applications that require a deep understanding of tricky data sources. The Pipe is available as a hosted API at [thepi.pe](https://thepi.pe), or it can be set up locally.
+The Pipe is a multimodal-first tool for feeding files and web pages into vision-language models such as GPT-4V. It is best for LLM and RAG applications that require a deep understanding of tricky data sources. The Pipe is available as a hosted API at [thepi.pe](https://thepi.pe), or it can be set up locally. 
 
 ![Demo](https://ngrdaaykhfrmtpodlakn.supabase.co/storage/v1/object/public/assets/demo.gif?t=2024-03-24T19%3A13%3A46.695Z)
 
 ## Features 🌟
 
 - Extracts text and visuals from files or web pages 📚
 - Outputs chunks optimized for multimodal LLMs 🖼️
@@ -44,41 +45,44 @@
 - Auto-compress prompts exceeding your chosen token limit 📦
 - Works even with missing file extensions, in-memory data streams 💾
 - Works with codebases, git repos, and custom integrations 🌐
 - Multi-threaded ⚡️
 
 ## Getting Started  🚀
 
+The Pipe handles a wide array of complex filetypes, and thus has many dependencies that must be installed separately. It also requires a strong machine for good response times. For this reason, we host it as an API that works out-of-the-box. 
+
 First, install The Pipe. 
 ```
 pip install thepipe_api
 ```
 
-Ensure the `THEPIPE_API_KEY` environment variable is set. Don't have an API key yet? [Get one here](https://thepi.pe). Alternatively, see the local installation section for the more advanced local setup.
+The Pipe is available as a hosted API, or it can be set up locally. An API key is recommended for out-of-the-box functionality (alternatively, see the local installation section). Ensure the `THEPIPE_API_KEY` environment variable is set. Don't have a key yet? [Get one here](https://thepi.pe).
 
 Now you can extract comprehensive text and visuals from any file:
 ```python
 from thepipe_api import thepipe
-chunks = thepipe.extract("example.pdf")
+messages = thepipe.extract("example.pdf")
 ```
 Or any website:
 ```python
-chunks = thepipe.extract("https://example.com")
+messages = thepipe.extract("https://example.com")
 ```
 Then feed it into GPT-4-Vision:
 ```python
 response = client.chat.completions.create(
     model="gpt-4-vision-preview",
-    messages = chunks,
+    messages = messages,
 )
 ```
-The Pipe's output is a list of sensible "chunks", and thus can be used either for storage in a vector database or for direct use as a prompt. Extra features such as data table extraction, bar chart extraction, custom web authentications and more are available in the [API documentation](https://thepi.pe/docs). [LiteLLM](https://github.com/BerriAI/litellm) can be used to easily integrate The Pipe with any LLM provider.
+
+![Just call OpenAI](https://rpnutzemutbrumczwvue.supabase.co/storage/v1/object/public/assets/IMG_0180.jpg)
 
 You can also use The Pipe from the command line. Here's how to recursively extract from a directory, matching only a specific file type:
-```
+```bash
 thepipe path/to/folder --match *jsx
 ```
 
 ## Supported File Types 📚
 
 | Source Type                           | Input types        | Token Compression 🗜️ | Image Extraction 👁️ | Notes 📌                                                  |
 |---------------------------------------|------------------------------------------|-------------------|------------------|---------------------------------------------------------|
@@ -91,29 +95,45 @@
 | Jupyter Notebook                      | `.ipynb`                                | ❌               | ✔️               | Extracts code, markdown, and images from Jupyter notebooks                                  |
 | Microsoft Word Document               | `.docx`                                 | ✔️               | ✔️               | Extracts text and images from Word documents                                        |
 | Microsoft PowerPoint Presentation     | `.pptx`                                 | ✔️               | ✔️               | Extracts text and images from PowerPoint presentations                              |
 | Website                               | URLs (inputs containing `http`, `https`, `ftp`)             | ✔️                | ✔️    | Extracts text from web page along with image (or images if scrollable); text-only extraction available          |
 | GitHub Repository                     | GitHub repo URLs                         | ✔️               | ✔️                | Extracts from GitHub repositories; supports branch specification         |
 | ZIP File                              | `.zip`                                  | ✔️               | ✔️                | Extracts contents of ZIP files; supports nested directory extraction     |
 
-##  How it works 🛠️
+## How it works 🛠️
+
+The input source is either a file path, a URL, or a directory. The pipe will extract information from the source and process it for downstream use with [language models](https://en.wikipedia.org/wiki/Large_language_model), [vision transformers](https://en.wikipedia.org/wiki/Vision_transformer), or [vision-language models](https://arxiv.org/abs/2304.00685). The output from the pipe is a sensible list of multimodal messages representing chunks of the extracted information, carefully crafted to fit within context windows for any models from [gemma-7b](https://huggingface.co/google/gemma-7b) to [GPT-4](https://openai.com/gpt-4). The messages returned should look like this:
+```json
+[
+  {
+    "type": "text",
+    "content": "Extracted text here..."
+  },
+  {
+    "type": "image_url",
+    "image_url": {
+      "url": "data:image/jpeg;base64,..."}
+  },
+]
+```
+The text and images from these messages may also be prepared for a vector database with `thepipe.core.create_chunks_from_messages` or for downstream use with RAG frameworks. [LiteLLM](https://github.com/BerriAI/litellm) can be used to easily integrate The Pipe with any LLM provider. 
 
-The pipe is accessible from the command line or from [Python](https://www.python.org/downloads/). The input source is either a file path, a URL, or a directory. The pipe will extract information from the source and process it for downstream use with [language models](https://en.wikipedia.org/wiki/Large_language_model), [vision transformers](https://en.wikipedia.org/wiki/Vision_transformer), or [vision-language models](https://arxiv.org/abs/2304.00685). The output from the pipe is a sensible text-based (or multimodal) representation of the extracted information, carefully crafted to fit within context windows for any models from [gemma-7b](https://huggingface.co/google/gemma-7b) to [GPT-4](https://openai.com/gpt-4). It uses a variety of heuristics for optimal performance with vision-language models, including AI filetype detection with [filetype detection](https://opensource.googleblog.com/2024/02/magika-ai-powered-fast-and-efficient-file-type-identification.html), AI [PDF extraction](thepi.pe/docs), efficient [token compression](https://arxiv.org/abs/2403.12968), automatic [image encoding](https://en.wikipedia.org/wiki/Base64), [reranking](https://arxiv.org/abs/2310.06839) for [lost-in-the-middle](https://arxiv.org/abs/2307.03172) effects, and more, all pre-built to work out-of-the-box.
+It uses a variety of heuristics for optimal performance with vision-language models, including AI filetype detection with [filetype detection](https://opensource.googleblog.com/2024/02/magika-ai-powered-fast-and-efficient-file-type-identification.html), opt-in AI [PDF extraction](thepi.pe/docs), efficient [token compression](https://arxiv.org/abs/2403.12968), automatic [image encoding](https://en.wikipedia.org/wiki/Base64), [reranking](https://arxiv.org/abs/2310.06839) for [lost-in-the-middle](https://arxiv.org/abs/2307.03172) effects, and more, all pre-built to work out-of-the-box.
 
 
 ## Local Installation 🛠️
 
-To use The Pipe locally, you will need [playwright](https://github.com/microsoft/playwright), [ctags](https://github.com/universal-ctags/), [pytesseract](https://github.com/h/pytesseract), and the local python requirements, which differ from the more lightweight API requirements. You will also need to use the local version of the requirements file:
+The Pipe handles a wide array of complex filetypes, and thus requires installation of many different packages to function. It also requires a very capable machine for good response times. For this reason, we host it as an API that works out-of-the-box. To use The Pipe locally for free instead, you will need [playwright](https://github.com/microsoft/playwright), [ctags](https://github.com/universal-ctags/), [pytesseract](https://github.com/h/pytesseract), and the local python requirements, which differ from the more lightweight API requirements:
 
 ```bash
 git clone https://github.com/emcf/thepipe
 pip install -r requirements_local.txt
 ```
 
-Tip for windows users: you may need to install the python-libmagic binaries with `pip install python-magic-bin`. You may also need to ensure the tesseract-ocr binaries and the ctags binaries are in your PATH.
+Tip for windows users: Install the python-libmagic binaries with `pip install python-magic-bin`. Ensure the `tesseract-ocr` binaries and the `ctags` binaries are in your PATH.
 
 Now you can use The Pipe with Python:
 ```bash
 from thepipe_api import thepipe
 chunks = thepipe.extract("example.pdf", local=True)
 ```
 
@@ -123,16 +143,16 @@
 ```
 
 Arguments are:
 - `source` (required): can be a file path, a URL, or a directory path.
 - `local` (optional): Use the local version of The Pipe instead of the hosted API.
 - `match` (optional): Regex pattern to match files in the directory.
 - `ignore` (optional): Regex pattern to ignore files in the directory.
-- `limit` (optional): The token limit for the output prompt, defaults to 100K. Prompts exceeding the limit will be compressed.
+- `limit` (optional): The token limit for the output prompt, defaults to 100K. Prompts exceeding the limit will be compressed. This may not work as expected with the API, as it is in active development.
 - `ai_extraction` (optional): Extract tables, figures, and math from PDFs using our extractor. Incurs extra costs.
 - `text_only` (optional): Do not extract images from documents or websites. Additionally, image files will be represented with OCR instead of as images.
 
-<a href="https://cal.com/emmett-mcf/30min"><img alt="Book us with Cal.com" src="https://cal.com/book-with-cal-dark.svg" /></a>
-
 # Sponsors
 
-Thank you to [Cal.com](https://cal.com/) for sponsoring this project. 
+<a href="https://cal.com/emmett-mcf/30min"><img alt="Book us with Cal.com" src="https://cal.com/book-with-cal-dark.svg" /></a>
+
+Thank you to [Cal.com](https://cal.com/) for sponsoring this project. Contact emmett@thepi.pe for sponsorship information.
```

#### html2text {}

```diff
@@ -1,17 +1,17 @@
-Metadata-Version: 2.1 Name: thepipe_api Version: 0.2.6 Summary: Automate
+Metadata-Version: 2.1 Name: thepipe_api Version: 0.2.7 Summary: Automate
 information extraction for multimodal LLMs. Home-page: https://github.com/emcf/
 thepipe Author: Emmett McFarlane Author-email: emmett@thepi.pe Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Requires-Python: >=3.6
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 aiohttp Requires-Dist: charset-normalizer Requires-Dist: Pyarrow Requires-Dist:
 python-magic Requires-Dist: colorama Requires-Dist: requests Requires-Dist:
 pillow Requires-Dist: cssutils Requires-Dist: beautifulsoup4 Requires-Dist:
-magika # _[_P_i_p_e_l_i_n_e_ _I_l_l_u_s_t_r_a_t_i_o_n_]_T_h_e_ _P_i_p_e
+magika Requires-Dist: python-dotenv # _[_P_i_p_e_l_i_n_e_ _I_l_l_u_s_t_r_a_t_i_o_n_]_T_h_e_ _P_i_p_e
 _E_n_g_l_i_s_h | _ä_¸_­_æ__
 [![codecov](https://codecov.io/gh/emcf/thepipe/graph/
 badge.svg?token=OE7CUEFUL9)](https://codecov.io/gh/emcf/thepipe) ![python-gh-
 action](https://github.com/emcf/thepipe/actions/workflows/python-ci.yml/
 badge.svg) _!_[_W_e_b_s_i_t_e_]_(_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
 _w_e_b_s_i_t_e_?_u_r_l_=_h_t_t_p_s_%_3_A_%_2_F_%_2_F_t_h_e_p_i_p_e_._u_p_._r_a_i_l_w_a_y_._a_p_p_%_2_F_&_l_a_b_e_l_=_A_P_I_%_2_0_s_t_a_t_u_s_) _!_[_g_e_t
 _A_P_I_]_(_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_A_P_I_-_g_e_t_%_2_0_a_c_c_e_s_s_-_b_l_u_e_) ### Feed PDFs, word
@@ -23,88 +23,97 @@
 [Demo](https://ngrdaaykhfrmtpodlakn.supabase.co/storage/v1/object/public/
 assets/demo.gif?t=2024-03-24T19%3A13%3A46.695Z) ## Features ð - Extracts
 text and visuals from files or web pages ð - Outputs chunks optimized for
 multimodal LLMs ð¼ï¸ - Interpret complex PDFs, web pages, slides, CSVs, and
 more ð§  - Auto-compress prompts exceeding your chosen token limit ð¦ -
 Works even with missing file extensions, in-memory data streams ð¾ - Works
 with codebases, git repos, and custom integrations ð - Multi-threaded â¡ï¸
-## Getting Started ð First, install The Pipe. ``` pip install thepipe_api
-``` Ensure the `THEPIPE_API_KEY` environment variable is set. Don't have an API
-key yet? [Get one here](https://thepi.pe). Alternatively, see the local
-installation section for the more advanced local setup. Now you can extract
-comprehensive text and visuals from any file: ```python from thepipe_api import
-thepipe chunks = thepipe.extract("example.pdf") ``` Or any website: ```python
-chunks = thepipe.extract("https://example.com") ``` Then feed it into GPT-4-
-Vision: ```python response = client.chat.completions.create( model="gpt-4-
-vision-preview", messages = chunks, ) ``` The Pipe's output is a list of
-sensible "chunks", and thus can be used either for storage in a vector database
-or for direct use as a prompt. Extra features such as data table extraction,
-bar chart extraction, custom web authentications and more are available in the
-[API documentation](https://thepi.pe/docs). [LiteLLM](https://github.com/
+## Getting Started ð The Pipe handles a wide array of complex filetypes, and
+thus has many dependencies that must be installed separately. It also requires
+a strong machine for good response times. For this reason, we host it as an API
+that works out-of-the-box. First, install The Pipe. ``` pip install thepipe_api
+``` The Pipe is available as a hosted API, or it can be set up locally. An API
+key is recommended for out-of-the-box functionality (alternatively, see the
+local installation section). Ensure the `THEPIPE_API_KEY` environment variable
+is set. Don't have a key yet? [Get one here](https://thepi.pe). Now you can
+extract comprehensive text and visuals from any file: ```python from
+thepipe_api import thepipe messages = thepipe.extract("example.pdf") ``` Or any
+website: ```python messages = thepipe.extract("https://example.com") ``` Then
+feed it into GPT-4-Vision: ```python response = client.chat.completions.create
+( model="gpt-4-vision-preview", messages = messages, ) ``` ![Just call OpenAI]
+(https://rpnutzemutbrumczwvue.supabase.co/storage/v1/object/public/assets/
+IMG_0180.jpg) You can also use The Pipe from the command line. Here's how to
+recursively extract from a directory, matching only a specific file type:
+```bash thepipe path/to/folder --match *jsx ``` ## Supported File Types ð |
+Source Type | Input types | Token Compression ðï¸ | Image Extraction
+ðï¸ | Notes ð | |---------------------------------------|---------------
+---------------------------|-------------------|------------------|------------
+---------------------------------------------| | Directory | Any `/path/to/
+directory` | âï¸ | âï¸ | Extracts from all files in directory, supports
+match and ignore patterns | | Code | `.py`, `.tsx`, `.js`, `.html`, `.css`,
+`.cpp`, etc | âï¸ (varies) | â | Combines all code files. `.c`, `.cpp`,
+`.py` are compressible with ctags, others are not | | Plaintext | `.txt`,
+`.md`, `.rtf`, etc | âï¸ | â | Regular text files | | PDF | `.pdf` |
+âï¸ | âï¸ | Extracts text and images of each page; can use AI for
+extraction of table data and images within pages | | Image | `.jpg`, `.jpeg`,
+`.png` | â | âï¸ | Extracts images, uses OCR if text_only | | Data Table |
+`.csv`, `.xls`, `.xlsx` | âï¸ | â | Extracts data from spreadsheets;
+converts to text representation. For very large datasets, will only extract
+column names and types | | Jupyter Notebook | `.ipynb` | â | âï¸ |
+Extracts code, markdown, and images from Jupyter notebooks | | Microsoft Word
+Document | `.docx` | âï¸ | âï¸ | Extracts text and images from Word
+documents | | Microsoft PowerPoint Presentation | `.pptx` | âï¸ | âï¸ |
+Extracts text and images from PowerPoint presentations | | Website | URLs
+(inputs containing `http`, `https`, `ftp`) | âï¸ | âï¸ | Extracts text
+from web page along with image (or images if scrollable); text-only extraction
+available | | GitHub Repository | GitHub repo URLs | âï¸ | âï¸ | Extracts
+from GitHub repositories; supports branch specification | | ZIP File | `.zip` |
+âï¸ | âï¸ | Extracts contents of ZIP files; supports nested directory
+extraction | ## How it works ð ï¸ The input source is either a file path, a
+URL, or a directory. The pipe will extract information from the source and
+process it for downstream use with [language models](https://en.wikipedia.org/
+wiki/Large_language_model), [vision transformers](https://en.wikipedia.org/
+wiki/Vision_transformer), or [vision-language models](https://arxiv.org/abs/
+2304.00685). The output from the pipe is a sensible list of multimodal messages
+representing chunks of the extracted information, carefully crafted to fit
+within context windows for any models from [gemma-7b](https://huggingface.co/
+google/gemma-7b) to [GPT-4](https://openai.com/gpt-4). The messages returned
+should look like this: ```json [ { "type": "text", "content": "Extracted text
+here..." }, { "type": "image_url", "image_url": { "url": "data:image/
+jpeg;base64,..."} }, ] ``` The text and images from these messages may also be
+prepared for a vector database with `thepipe.core.create_chunks_from_messages`
+or for downstream use with RAG frameworks. [LiteLLM](https://github.com/
 BerriAI/litellm) can be used to easily integrate The Pipe with any LLM
-provider. You can also use The Pipe from the command line. Here's how to
-recursively extract from a directory, matching only a specific file type: ```
-thepipe path/to/folder --match *jsx ``` ## Supported File Types ð | Source
-Type | Input types | Token Compression ðï¸ | Image Extraction ðï¸ |
-Notes ð | |---------------------------------------|-------------------------
------------------|-------------------|------------------|----------------------
------------------------------------| | Directory | Any `/path/to/directory` |
-âï¸ | âï¸ | Extracts from all files in directory, supports match and
-ignore patterns | | Code | `.py`, `.tsx`, `.js`, `.html`, `.css`, `.cpp`, etc |
-âï¸ (varies) | â | Combines all code files. `.c`, `.cpp`, `.py` are
-compressible with ctags, others are not | | Plaintext | `.txt`, `.md`, `.rtf`,
-etc | âï¸ | â | Regular text files | | PDF | `.pdf` | âï¸ | âï¸ |
-Extracts text and images of each page; can use AI for extraction of table data
-and images within pages | | Image | `.jpg`, `.jpeg`, `.png` | â | âï¸ |
-Extracts images, uses OCR if text_only | | Data Table | `.csv`, `.xls`, `.xlsx`
-| âï¸ | â | Extracts data from spreadsheets; converts to text
-representation. For very large datasets, will only extract column names and
-types | | Jupyter Notebook | `.ipynb` | â | âï¸ | Extracts code, markdown,
-and images from Jupyter notebooks | | Microsoft Word Document | `.docx` |
-âï¸ | âï¸ | Extracts text and images from Word documents | | Microsoft
-PowerPoint Presentation | `.pptx` | âï¸ | âï¸ | Extracts text and images
-from PowerPoint presentations | | Website | URLs (inputs containing `http`,
-`https`, `ftp`) | âï¸ | âï¸ | Extracts text from web page along with
-image (or images if scrollable); text-only extraction available | | GitHub
-Repository | GitHub repo URLs | âï¸ | âï¸ | Extracts from GitHub
-repositories; supports branch specification | | ZIP File | `.zip` | âï¸ |
-âï¸ | Extracts contents of ZIP files; supports nested directory extraction |
-## How it works ð ï¸ The pipe is accessible from the command line or from
-[Python](https://www.python.org/downloads/). The input source is either a file
-path, a URL, or a directory. The pipe will extract information from the source
-and process it for downstream use with [language models](https://
-en.wikipedia.org/wiki/Large_language_model), [vision transformers](https://
-en.wikipedia.org/wiki/Vision_transformer), or [vision-language models](https://
-arxiv.org/abs/2304.00685). The output from the pipe is a sensible text-based
-(or multimodal) representation of the extracted information, carefully crafted
-to fit within context windows for any models from [gemma-7b](https://
-huggingface.co/google/gemma-7b) to [GPT-4](https://openai.com/gpt-4). It uses a
-variety of heuristics for optimal performance with vision-language models,
-including AI filetype detection with [filetype detection](https://
-opensource.googleblog.com/2024/02/magika-ai-powered-fast-and-efficient-file-
-type-identification.html), AI [PDF extraction](thepi.pe/docs), efficient [token
-compression](https://arxiv.org/abs/2403.12968), automatic [image encoding]
-(https://en.wikipedia.org/wiki/Base64), [reranking](https://arxiv.org/abs/
-2310.06839) for [lost-in-the-middle](https://arxiv.org/abs/2307.03172) effects,
-and more, all pre-built to work out-of-the-box. ## Local Installation ð ï¸
-To use The Pipe locally, you will need [playwright](https://github.com/
-microsoft/playwright), [ctags](https://github.com/universal-ctags/),
-[pytesseract](https://github.com/h/pytesseract), and the local python
-requirements, which differ from the more lightweight API requirements. You will
-also need to use the local version of the requirements file: ```bash git clone
-https://github.com/emcf/thepipe pip install -r requirements_local.txt ``` Tip
-for windows users: you may need to install the python-libmagic binaries with
-`pip install python-magic-bin`. You may also need to ensure the tesseract-ocr
-binaries and the ctags binaries are in your PATH. Now you can use The Pipe with
-Python: ```bash from thepipe_api import thepipe chunks = thepipe.extract
-("example.pdf", local=True) ``` or from the command line: ```bash thepipe path/
-to/folder --local ``` Arguments are: - `source` (required): can be a file path,
-a URL, or a directory path. - `local` (optional): Use the local version of The
-Pipe instead of the hosted API. - `match` (optional): Regex pattern to match
-files in the directory. - `ignore` (optional): Regex pattern to ignore files in
-the directory. - `limit` (optional): The token limit for the output prompt,
-defaults to 100K. Prompts exceeding the limit will be compressed. -
-`ai_extraction` (optional): Extract tables, figures, and math from PDFs using
-our extractor. Incurs extra costs. - `text_only` (optional): Do not extract
-images from documents or websites. Additionally, image files will be
-represented with OCR instead of as images. _[_B_o_o_k_ _u_s_ _w_i_t_h_ _C_a_l_._c_o_m_]# Sponsors
-Thank you to [Cal.com](https://cal.com/) for sponsoring this project.
+provider. It uses a variety of heuristics for optimal performance with vision-
+language models, including AI filetype detection with [filetype detection]
+(https://opensource.googleblog.com/2024/02/magika-ai-powered-fast-and-
+efficient-file-type-identification.html), opt-in AI [PDF extraction](thepi.pe/
+docs), efficient [token compression](https://arxiv.org/abs/2403.12968),
+automatic [image encoding](https://en.wikipedia.org/wiki/Base64), [reranking]
+(https://arxiv.org/abs/2310.06839) for [lost-in-the-middle](https://arxiv.org/
+abs/2307.03172) effects, and more, all pre-built to work out-of-the-box. ##
+Local Installation ð ï¸ The Pipe handles a wide array of complex filetypes,
+and thus requires installation of many different packages to function. It also
+requires a very capable machine for good response times. For this reason, we
+host it as an API that works out-of-the-box. To use The Pipe locally for free
+instead, you will need [playwright](https://github.com/microsoft/playwright),
+[ctags](https://github.com/universal-ctags/), [pytesseract](https://github.com/
+h/pytesseract), and the local python requirements, which differ from the more
+lightweight API requirements: ```bash git clone https://github.com/emcf/thepipe
+pip install -r requirements_local.txt ``` Tip for windows users: Install the
+python-libmagic binaries with `pip install python-magic-bin`. Ensure the
+`tesseract-ocr` binaries and the `ctags` binaries are in your PATH. Now you can
+use The Pipe with Python: ```bash from thepipe_api import thepipe chunks =
+thepipe.extract("example.pdf", local=True) ``` or from the command line:
+```bash thepipe path/to/folder --local ``` Arguments are: - `source`
+(required): can be a file path, a URL, or a directory path. - `local`
+(optional): Use the local version of The Pipe instead of the hosted API. -
+`match` (optional): Regex pattern to match files in the directory. - `ignore`
+(optional): Regex pattern to ignore files in the directory. - `limit`
+(optional): The token limit for the output prompt, defaults to 100K. Prompts
+exceeding the limit will be compressed. This may not work as expected with the
+API, as it is in active development. - `ai_extraction` (optional): Extract
+tables, figures, and math from PDFs using our extractor. Incurs extra costs. -
+`text_only` (optional): Do not extract images from documents or websites.
+Additionally, image files will be represented with OCR instead of as images. #
+Sponsors _[_B_o_o_k_ _u_s_ _w_i_t_h_ _C_a_l_._c_o_m_]Thank you to [Cal.com](https://cal.com/) for
+sponsoring this project. Contact emmett@thepi.pe for sponsorship information.
```

