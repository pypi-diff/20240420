# Comparing `tmp/PerplexiPy-0.4.1-py3-none-any.whl.zip` & `tmp/PerplexiPy-1.0.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 11285 bytes, number of entries: 10
--rw-r--r--  2.0 unx     9067 b- defN 24-Apr-16 02:09 perplexipy/__init__.py
--rw-r--r--  2.0 unx     8834 b- defN 24-Apr-17 00:34 perplexipy/codex.py
+Zip file size: 11533 bytes, number of entries: 10
+-rw-r--r--  2.0 unx     9253 b- defN 24-Apr-20 02:08 perplexipy/__init__.py
+-rw-r--r--  2.0 unx     8842 b- defN 24-Apr-19 14:23 perplexipy/codex.py
 -rw-r--r--  2.0 unx      283 b- defN 24-Mar-01 20:13 perplexipy/errors.py
 -rw-r--r--  2.0 unx      684 b- defN 24-Apr-13 17:06 perplexipy/responses.py
--rw-r--r--  2.0 unx     1514 b- defN 24-Apr-17 00:40 PerplexiPy-0.4.1.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx     6334 b- defN 24-Apr-17 00:40 PerplexiPy-0.4.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-17 00:40 PerplexiPy-0.4.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       49 b- defN 24-Apr-17 00:40 PerplexiPy-0.4.1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       11 b- defN 24-Apr-17 00:40 PerplexiPy-0.4.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      813 b- defN 24-Apr-17 00:40 PerplexiPy-0.4.1.dist-info/RECORD
-10 files, 27681 bytes uncompressed, 9893 bytes compressed:  64.3%
+-rw-r--r--  2.0 unx     1514 b- defN 24-Apr-20 02:09 PerplexiPy-1.0.1.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx     6833 b- defN 24-Apr-20 02:09 PerplexiPy-1.0.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-20 02:09 PerplexiPy-1.0.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       49 b- defN 24-Apr-20 02:09 PerplexiPy-1.0.1.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       11 b- defN 24-Apr-20 02:09 PerplexiPy-1.0.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      813 b- defN 24-Apr-20 02:09 PerplexiPy-1.0.1.dist-info/RECORD
+10 files, 28374 bytes uncompressed, 10141 bytes compressed:  64.3%
```

## zipnote {}

```diff
@@ -6,26 +6,26 @@
 
 Filename: perplexipy/errors.py
 Comment: 
 
 Filename: perplexipy/responses.py
 Comment: 
 
-Filename: PerplexiPy-0.4.1.dist-info/LICENSE.txt
+Filename: PerplexiPy-1.0.1.dist-info/LICENSE.txt
 Comment: 
 
-Filename: PerplexiPy-0.4.1.dist-info/METADATA
+Filename: PerplexiPy-1.0.1.dist-info/METADATA
 Comment: 
 
-Filename: PerplexiPy-0.4.1.dist-info/WHEEL
+Filename: PerplexiPy-1.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: PerplexiPy-0.4.1.dist-info/entry_points.txt
+Filename: PerplexiPy-1.0.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: PerplexiPy-0.4.1.dist-info/top_level.txt
+Filename: PerplexiPy-1.0.1.dist-info/top_level.txt
 Comment: 
 
-Filename: PerplexiPy-0.4.1.dist-info/RECORD
+Filename: PerplexiPy-1.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## perplexipy/__init__.py

```diff
@@ -248,14 +248,16 @@
         - `parameterCount`
         - `contextLength`
         - `modelType`
         - `availability`
         """
         supportedModels = OrderedDict({
             'codellama-70b-instruct': ModelInfo('70B', 16384, 'chat completion', 'open source',),
+            'llama-3-8b-instruct': ModelInfo('8B', 8192, 'chat completion', 'open source'),
+            'llama-3-70b-instruct': ModelInfo('70B', 8192, 'chat completion', 'open source'),
             'mistral-7b-instruct': ModelInfo('7B', 16384, 'chat completion', 'open source',),
             'mixtral-8x7b-instruct': ModelInfo('8x7B', 16384, 'chat completion', 'open source',),
             'sonar-medium-chat': ModelInfo('8x7B', 16348, 'chat completion', 'Perplexity',),
             'sonar-medium-online': ModelInfo('8x7B', 12000, 'chat completion', 'Perplexity',),
             'sonar-small-chat': ModelInfo('7B', 16384, 'chat completion', 'Perplexity',),
             'sonar-small-online': ModelInfo('7B', 12000, 'chat completion', 'Perplexity',),
         })
```

## perplexipy/codex.py

```diff
@@ -172,15 +172,15 @@
     return session
 
 
 def _queryStyle(newStyle: str = None):
     global _queryCodeStyle
 
     if newStyle:
-        _queryCodeStyle = not 'human'
+        _queryCodeStyle = newStyle != 'human'
     click.secho('Coding query style = %s' % _queryCodeStyle, fg = 'bright_blue')
     return _queryCodeStyle
 
 
 def _makeQuery(userQuery: str) -> str:
     if _queryCodeStyle:
         userQuery = QUERY_DETAILED+userQuery
```

## Comparing `PerplexiPy-0.4.1.dist-info/LICENSE.txt` & `PerplexiPy-1.0.1.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `PerplexiPy-0.4.1.dist-info/METADATA` & `PerplexiPy-1.0.1.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PerplexiPy
-Version: 0.4.1
+Version: 1.0.1
 Summary: PerplexiPy - A robust Perplexity AI API client
 Author-email: CIME Software Ltd <perplexipy@cime.net>
 License: BSD-3
 Project-URL: homepage, https://cime-software.github.io/perplexipy/
 Project-URL: Documentation, https://cime-software.github.io/perplexipy/
 Project-URL: Bug Tracker, https://github.com/CIME-Software/perplexipy/issues
 Project-URL: Source, https://github.com/CIME-Software/perplexipy
@@ -22,22 +22,25 @@
 Requires-Dist: appdirs
 Requires-Dist: click
 Requires-Dist: openai (>=1.12.0)
 Requires-Dist: prompt-toolkit
 Requires-Dist: python-dotenv
 Requires-Dist: pyyaml
 
-% perplexipy(3) Version 0.4.1 | Perplexity AI high level API documentation
+% perplexipy(3) Version 1.0.1 | Perplexity AI high level API documentation
 
 Name
 ====
 
 **PerplexiPy** - Perplexity AI high level library
 
 
+<img src='https://images2.imgbox.com/57/94/AsI1WSfy_o.png'>
+
+
 Synopsis
 ========
 ```python
 client = PerplexityClient() \
 print(client.query('What is the meaning of 42?') \
 for result in client.queryStreamable('List of all US presidents'): \
     print(result)
@@ -155,14 +158,30 @@
 
 
 Async usage
 ===========
 Not supported at this time.
 
 
+Interactive usage
+=================
+PerplexiPy ships with the Codex Playground, an interactive REPL console.  To
+run it:
+
+```bash
+# In a virtualenv:
+pip install -U perplexipy
+export PERPLEXITY_API_KEY="your-key-goes-here"
+codex repl
+```
+
+Full description of Codex Playground and other use cases like streaming API and
+CLI argument passing in the [Codex README](https://github.com/CIME-Software/perplexipy/blob/master/codex-README.md).
+
+
 License
 =======
 The **PerplexiPy** package, documentation and examples are licensed under the
 [BSD-3 open source license](https://github.com/CIME-Software/perplexipy/blob/master/LICENSE.txt).
 
 
 See also
```

### html2text {}

```diff
@@ -1,74 +1,81 @@
-Metadata-Version: 2.1 Name: PerplexiPy Version: 0.4.1 Summary: PerplexiPy - A
+Metadata-Version: 2.1 Name: PerplexiPy Version: 1.0.1 Summary: PerplexiPy - A
 robust Perplexity AI API client Author-email: CIME Software Ltd
 cime.net> License: BSD-3 Project-URL: homepage, https://cime-
 software.github.io/perplexipy/ Project-URL: Documentation, https://cime-
 software.github.io/perplexipy/ Project-URL: Bug Tracker, https://github.com/
 CIME-Software/perplexipy/issues Project-URL: Source, https://github.com/CIME-
 Software/perplexipy Classifier: Development Status :: 4 - Beta Classifier:
 Intended Audience :: Developers Classifier: License :: OSI Approved :: BSD
 License Classifier: Operating System :: OS Independent Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.9 Description-Content-Type: text/markdown License-File:
 LICENSE.txt Requires-Dist: appdirs Requires-Dist: click Requires-Dist: openai
 (>=1.12.0) Requires-Dist: prompt-toolkit Requires-Dist: python-dotenv Requires-
-Dist: pyyaml % perplexipy(3) Version 0.4.1 | Perplexity AI high level API
+Dist: pyyaml % perplexipy(3) Version 1.0.1 | Perplexity AI high level API
 documentation Name ==== **PerplexiPy** - Perplexity AI high level library
-Synopsis ======== ```python client = PerplexityClient() \ print(client.query
-('What is the meaning of 42?') \ for result in client.queryStreamable('List of
-all US presidents'): \ print(result) ``` Description =========== **PerplexiPy**
-is a high-level, convenience library for interacting with the Perplexity API
-from any Python 3.9+ application. The library aims to simplify interactions
-with Perplexity models by encapsulating all the implementation details of the
-lower level OpenAI API. All interaction between the code and this library
-occurs in the form of string and native Python objects, not OpenAPI / Swagger
-mapped objects. **PerplexiPy** implements a combination of the Perplexity AI
-and the OpenAI outputs. API semantics follow the "literate programming"
-workflow, and attempt to make the resulting code as simple to follow as
-possible. _P_e_r_p_l_e_x_i_t_y_ _A_I is an AI-powered search engine that uses natural
-language processing and machine learning to provide accurate and comprehensive
-answers to end-user queries. It can be argued that it outperforms OpenAI's
-offerings in accuracy and responsiveness. **PerplexiPy** enables the creation
-of Python programs and tools that leverage the power of Perplexity AI.
-Documentation ============= These documents encompass all information about
-**PerplexiPy**: - This README file, hosted in the **[perplexipy](https://
-github.com/CIME-Software/perplexipy)** GitHub repository project on GitHub and
-exported to the PyPI project page - A `man` page autogenerated from this README
-file, `perplexipy.3` - The complete **PerplexiPy API reference** on GitHub
-Pages - https://cime-software.github.io/perplexipy/perplexipy.html - The
-_P_e_r_p_l_e_x_i_P_y_-_t_u_t_o_r_i_a_l_._i_p_y_n_b tutorial notebook The `man` page can be generated
-from the source distribution using this command: ```bash make manpage ``` The
-output will reside in: `./manpages/perplexipy.3`. The `man` page isn't included
-in the Python package wheel because there's no accepted standard installation
-that's cross-compatible among all supported operating systems and
-distributions. Installation ============ ```bash pip install perplexipy ```
-Package information: https://pypi.org/project/perplexipy API key ======= Access
-to the Perplexity API requires a paid subscription and an API key. Use of
-`.env` is recommended for storing the private key. There is an automatic
-constant `PERPLEXITY_API_KEY` that gets initialized to the value of a `.env`
-key of the same name via the `dotenv` API. Otherwise, `PERPLEXITY_API_KEY` may
-be handled like any other secret by the implementing team. This module provides
-no other tools or services for handling the API key. This key is used only
-during `PerplexityClient` instantiation: ```python import os key = os.environ
+[https://images2.imgbox.com/57/94/AsI1WSfy_o.png]Synopsis ======== ```python
+client = PerplexityClient() \ print(client.query('What is the meaning of 42?')
+\ for result in client.queryStreamable('List of all US presidents'): \ print
+(result) ``` Description =========== **PerplexiPy** is a high-level,
+convenience library for interacting with the Perplexity API from any Python
+3.9+ application. The library aims to simplify interactions with Perplexity
+models by encapsulating all the implementation details of the lower level
+OpenAI API. All interaction between the code and this library occurs in the
+form of string and native Python objects, not OpenAPI / Swagger mapped objects.
+**PerplexiPy** implements a combination of the Perplexity AI and the OpenAI
+outputs. API semantics follow the "literate programming" workflow, and attempt
+to make the resulting code as simple to follow as possible. _P_e_r_p_l_e_x_i_t_y_ _A_I is an
+AI-powered search engine that uses natural language processing and machine
+learning to provide accurate and comprehensive answers to end-user queries. It
+can be argued that it outperforms OpenAI's offerings in accuracy and
+responsiveness. **PerplexiPy** enables the creation of Python programs and
+tools that leverage the power of Perplexity AI. Documentation =============
+These documents encompass all information about **PerplexiPy**: - This README
+file, hosted in the **[perplexipy](https://github.com/CIME-Software/
+perplexipy)** GitHub repository project on GitHub and exported to the PyPI
+project page - A `man` page autogenerated from this README file, `perplexipy.3`
+- The complete **PerplexiPy API reference** on GitHub Pages - https://cime-
+software.github.io/perplexipy/perplexipy.html - The _P_e_r_p_l_e_x_i_P_y_-_t_u_t_o_r_i_a_l_._i_p_y_n_b
+tutorial notebook The `man` page can be generated from the source distribution
+using this command: ```bash make manpage ``` The output will reside in: `./
+manpages/perplexipy.3`. The `man` page isn't included in the Python package
+wheel because there's no accepted standard installation that's cross-compatible
+among all supported operating systems and distributions. Installation
+============ ```bash pip install perplexipy ``` Package information: https://
+pypi.org/project/perplexipy API key ======= Access to the Perplexity API
+requires a paid subscription and an API key. Use of `.env` is recommended for
+storing the private key. There is an automatic constant `PERPLEXITY_API_KEY`
+that gets initialized to the value of a `.env` key of the same name via the
+`dotenv` API. Otherwise, `PERPLEXITY_API_KEY` may be handled like any other
+secret by the implementing team. This module provides no other tools or
+services for handling the API key. This key is used only during
+`PerplexityClient` instantiation: ```python import os key = os.environ
 ['PERPLEXITY_API_KEY'] client = PerplexityClient(key = key) print(client.query
 ('Brief answer: greet the world in Swedish.')) ``` Usage ===== See the
 _P_e_r_p_l_e_x_i_P_y_-_t_u_t_o_r_i_a_l_._i_p_y_n_b notebook for a richer example of the API's
 capabilities. In general: ```python client = PerplexityClient() result =
 client.query('Show me how to declare a list in Python') # result is a string
 results = client.queryBatch('Show me different ways of declaring a Python
 list') for result in results: print(result) # results is a tuple of one or more
 results results = client.queryStreamable('Tell me why lists are important in
 programming') for result in results: print(result) # results is a long stream
 of data, served over time. models = client.models # lists all models supported
 by Perplexity AI print('Model names:') for model in models.keys(): print(' -
 %s' % model) try: client.model = 'bogus-LLM-7b' except PerplexityClientError as
 e: print(e) client.model = models.keys()[0] # OK ``` Async usage ===========
-Not supported at this time. License ======= The **PerplexiPy** package,
+Not supported at this time. Interactive usage ================= PerplexiPy
+ships with the Codex Playground, an interactive REPL console. To run it:
+```bash # In a virtualenv: pip install -U perplexipy export
+PERPLEXITY_API_KEY="your-key-goes-here" codex repl ``` Full description of
+Codex Playground and other use cases like streaming API and CLI argument
+passing in the [Codex README](https://github.com/CIME-Software/perplexipy/blob/
+master/codex-README.md). License ======= The **PerplexiPy** package,
 documentation and examples are licensed under the [BSD-3 open source license]
 (https://github.com/CIME-Software/perplexipy/blob/master/LICENSE.txt). See also
 ======== - **codex** - a PerplexiPy command line code explainer - API
 documentation: https://cime-software.github.io/perplexipy - _P_e_r_p_l_e_x_i_t_y_ _A_I -
 m0toko: a Sopel bot plug-in that uses PerplexiPy for providing AI-enhanced
 chatbot functionality: https://github.com/pr3d4t0r/m0toko - PyPI: _o_p_e_n_a_i
 Caveats ======= The code should work with Python 3.7 or later, but it was only
```

## Comparing `PerplexiPy-0.4.1.dist-info/RECORD` & `PerplexiPy-1.0.1.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-perplexipy/__init__.py,sha256=YHI3TDJUnV8BIKHKojbwSo75NKX9i9xq4jmChr2EZH4,9067
-perplexipy/codex.py,sha256=jFk2CZ-ic2TT4Tqhmq4EvpVTqn9qERaCrrkx2_rjKYg,8834
+perplexipy/__init__.py,sha256=jex9IfNCEyLV3rtpq7L3VEfs75NmHXZki8l6wD-wohA,9253
+perplexipy/codex.py,sha256=teupcZ85_UxAcdOFYILs3KPCVdDU9BUa2z3rtoLNwYs,8842
 perplexipy/errors.py,sha256=YM4dVV9q2aLm_ZJdhyCjhejLXdo8mEffx93zlP_7lOs,283
 perplexipy/responses.py,sha256=1OrBpZxGHaVvlE5x9ZtdQhoXP5RbmKOXtHGt6Nm7g2I,684
-PerplexiPy-0.4.1.dist-info/LICENSE.txt,sha256=j9TykfeJa2xvP5Wmggfxaz8pTnedQO9BQX5PbJkh8Yc,1514
-PerplexiPy-0.4.1.dist-info/METADATA,sha256=jaIzzXOzz31rWv0uUipRNEYnZM2bMRAVdLQHetBiRrY,6334
-PerplexiPy-0.4.1.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-PerplexiPy-0.4.1.dist-info/entry_points.txt,sha256=tRB7D5Ao_Rptera8eLiPoF9ecAvHbf5lFSYYaGs9Cfw,49
-PerplexiPy-0.4.1.dist-info/top_level.txt,sha256=JS_DtYqartG2-vkrCiFr0aeoy4Dg6my7DlmUA90wKhA,11
-PerplexiPy-0.4.1.dist-info/RECORD,,
+PerplexiPy-1.0.1.dist-info/LICENSE.txt,sha256=j9TykfeJa2xvP5Wmggfxaz8pTnedQO9BQX5PbJkh8Yc,1514
+PerplexiPy-1.0.1.dist-info/METADATA,sha256=GPA1H9J62pJIOmndFDPB3CapduQI5L442vqgGD5gFoU,6833
+PerplexiPy-1.0.1.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+PerplexiPy-1.0.1.dist-info/entry_points.txt,sha256=tRB7D5Ao_Rptera8eLiPoF9ecAvHbf5lFSYYaGs9Cfw,49
+PerplexiPy-1.0.1.dist-info/top_level.txt,sha256=JS_DtYqartG2-vkrCiFr0aeoy4Dg6my7DlmUA90wKhA,11
+PerplexiPy-1.0.1.dist-info/RECORD,,
```

