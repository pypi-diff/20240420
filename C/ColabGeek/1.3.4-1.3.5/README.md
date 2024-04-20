# Comparing `tmp/ColabGeek-1.3.4.tar.gz` & `tmp/colabgeek-1.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ColabGeek-1.3.4.tar", last modified: Fri Apr 12 03:16:51 2024, max compression
+gzip compressed data, was "colabgeek-1.3.5.tar", last modified: Sat Apr 20 08:11:11 2024, max compression
```

## Comparing `ColabGeek-1.3.4.tar` & `colabgeek-1.3.5.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxrwxr-x   0 sunym     (1000) sunym     (1000)        0 2024-04-12 03:16:51.252305 ColabGeek-1.3.4/
--rw-rw-r--   0 sunym     (1000) sunym     (1000)     1067 2024-04-12 03:12:54.000000 ColabGeek-1.3.4/LICENSE
--rw-r--r--   0 sunym     (1000) sunym     (1000)     8758 2024-04-12 03:16:51.251305 ColabGeek-1.3.4/PKG-INFO
--rw-rw-r--   0 sunym     (1000) sunym     (1000)     8022 2024-04-12 03:12:54.000000 ColabGeek-1.3.4/README.md
--rw-rw-r--   0 sunym     (1000) sunym     (1000)      940 2024-04-12 03:12:54.000000 ColabGeek-1.3.4/pyproject.toml
--rw-rw-r--   0 sunym     (1000) sunym     (1000)       38 2024-04-12 03:16:51.252305 ColabGeek-1.3.4/setup.cfg
-drwxrwxr-x   0 sunym     (1000) sunym     (1000)        0 2024-04-12 03:16:51.247305 ColabGeek-1.3.4/src/
-drwxrwxr-x   0 sunym     (1000) sunym     (1000)        0 2024-04-12 03:16:51.248305 ColabGeek-1.3.4/src/ColabGeek/
--rw-rw-r--   0 sunym     (1000) sunym     (1000)    28805 2024-04-12 03:12:54.000000 ColabGeek-1.3.4/src/ColabGeek/ColabGeek.py
--rw-rw-r--   0 sunym     (1000) sunym     (1000)       25 2024-04-12 03:12:54.000000 ColabGeek-1.3.4/src/ColabGeek/__init__.py
-drwxrwxr-x   0 sunym     (1000) sunym     (1000)        0 2024-04-12 03:16:51.251305 ColabGeek-1.3.4/src/ColabGeek/shell_scripts/
--rw-rw-r--   0 sunym     (1000) sunym     (1000)      817 2024-04-12 03:12:54.000000 ColabGeek-1.3.4/src/ColabGeek/shell_scripts/Install_Homebrew.exp
--rw-rw-r--   0 sunym     (1000) sunym     (1000)      325 2024-04-12 03:12:54.000000 ColabGeek-1.3.4/src/ColabGeek/shell_scripts/Install_Jekyll.exp
--rw-rw-r--   0 sunym     (1000) sunym     (1000)      621 2024-04-12 03:12:54.000000 ColabGeek-1.3.4/src/ColabGeek/shell_scripts/Install_Miniconda.sh
--rw-rw-r--   0 sunym     (1000) sunym     (1000)      486 2024-04-12 03:12:54.000000 ColabGeek-1.3.4/src/ColabGeek/shell_scripts/Install_Ruby.exp
--rw-rw-r--   0 sunym     (1000) sunym     (1000)      443 2024-04-12 03:12:54.000000 ColabGeek-1.3.4/src/ColabGeek/shell_scripts/Install_rbenv.exp
--rw-rw-r--   0 sunym     (1000) sunym     (1000)      382 2024-04-12 03:12:54.000000 ColabGeek-1.3.4/src/ColabGeek/shell_scripts/Run_Rstudio_server.sh
--rw-rw-r--   0 sunym     (1000) sunym     (1000)     1193 2024-04-12 03:12:54.000000 ColabGeek-1.3.4/src/ColabGeek/shell_scripts/Run_code_server.exp
-drwxrwxr-x   0 sunym     (1000) sunym     (1000)        0 2024-04-12 03:16:51.251305 ColabGeek-1.3.4/src/ColabGeek.egg-info/
--rw-r--r--   0 sunym     (1000) sunym     (1000)     8758 2024-04-12 03:16:51.000000 ColabGeek-1.3.4/src/ColabGeek.egg-info/PKG-INFO
--rw-rw-r--   0 sunym     (1000) sunym     (1000)      567 2024-04-12 03:16:51.000000 ColabGeek-1.3.4/src/ColabGeek.egg-info/SOURCES.txt
--rw-rw-r--   0 sunym     (1000) sunym     (1000)        1 2024-04-12 03:16:51.000000 ColabGeek-1.3.4/src/ColabGeek.egg-info/dependency_links.txt
--rw-rw-r--   0 sunym     (1000) sunym     (1000)       10 2024-04-12 03:16:51.000000 ColabGeek-1.3.4/src/ColabGeek.egg-info/top_level.txt
+drwxrwxr-x   0 sunym     (1000) sunym     (1000)        0 2024-04-20 08:11:11.810792 colabgeek-1.3.5/
+-rw-rw-r--   0 sunym     (1000) sunym     (1000)     1067 2024-04-20 06:51:09.000000 colabgeek-1.3.5/LICENSE
+-rw-r--r--   0 sunym     (1000) sunym     (1000)     9955 2024-04-20 08:11:11.809792 colabgeek-1.3.5/PKG-INFO
+-rw-rw-r--   0 sunym     (1000) sunym     (1000)     9151 2024-04-20 07:59:49.000000 colabgeek-1.3.5/README.md
+-rw-rw-r--   0 sunym     (1000) sunym     (1000)      999 2024-04-20 07:59:49.000000 colabgeek-1.3.5/pyproject.toml
+-rw-rw-r--   0 sunym     (1000) sunym     (1000)       38 2024-04-20 08:11:11.810792 colabgeek-1.3.5/setup.cfg
+drwxrwxr-x   0 sunym     (1000) sunym     (1000)        0 2024-04-20 08:11:11.806792 colabgeek-1.3.5/src/
+drwxrwxr-x   0 sunym     (1000) sunym     (1000)        0 2024-04-20 08:11:11.807792 colabgeek-1.3.5/src/ColabGeek/
+-rw-rw-r--   0 sunym     (1000) sunym     (1000)    34654 2024-04-20 07:59:49.000000 colabgeek-1.3.5/src/ColabGeek/ColabGeek.py
+-rw-rw-r--   0 sunym     (1000) sunym     (1000)       25 2024-04-20 06:51:09.000000 colabgeek-1.3.5/src/ColabGeek/__init__.py
+drwxrwxr-x   0 sunym     (1000) sunym     (1000)        0 2024-04-20 08:11:11.809792 colabgeek-1.3.5/src/ColabGeek/shell_scripts/
+-rw-rw-r--   0 sunym     (1000) sunym     (1000)      817 2024-04-20 06:51:09.000000 colabgeek-1.3.5/src/ColabGeek/shell_scripts/Install_Homebrew.exp
+-rw-rw-r--   0 sunym     (1000) sunym     (1000)      325 2024-04-20 06:51:09.000000 colabgeek-1.3.5/src/ColabGeek/shell_scripts/Install_Jekyll.exp
+-rw-rw-r--   0 sunym     (1000) sunym     (1000)      621 2024-04-20 06:51:09.000000 colabgeek-1.3.5/src/ColabGeek/shell_scripts/Install_Miniconda.sh
+-rw-rw-r--   0 sunym     (1000) sunym     (1000)      486 2024-04-20 06:51:09.000000 colabgeek-1.3.5/src/ColabGeek/shell_scripts/Install_Ruby.exp
+-rw-rw-r--   0 sunym     (1000) sunym     (1000)      443 2024-04-20 06:51:09.000000 colabgeek-1.3.5/src/ColabGeek/shell_scripts/Install_rbenv.exp
+-rw-rw-r--   0 sunym     (1000) sunym     (1000)      382 2024-04-20 06:51:09.000000 colabgeek-1.3.5/src/ColabGeek/shell_scripts/Run_Rstudio_server.sh
+-rw-rw-r--   0 sunym     (1000) sunym     (1000)     1193 2024-04-20 06:51:09.000000 colabgeek-1.3.5/src/ColabGeek/shell_scripts/Run_code_server.exp
+drwxrwxr-x   0 sunym     (1000) sunym     (1000)        0 2024-04-20 08:11:11.809792 colabgeek-1.3.5/src/ColabGeek.egg-info/
+-rw-r--r--   0 sunym     (1000) sunym     (1000)     9955 2024-04-20 08:11:11.000000 colabgeek-1.3.5/src/ColabGeek.egg-info/PKG-INFO
+-rw-rw-r--   0 sunym     (1000) sunym     (1000)      603 2024-04-20 08:11:11.000000 colabgeek-1.3.5/src/ColabGeek.egg-info/SOURCES.txt
+-rw-rw-r--   0 sunym     (1000) sunym     (1000)        1 2024-04-20 08:11:11.000000 colabgeek-1.3.5/src/ColabGeek.egg-info/dependency_links.txt
+-rw-rw-r--   0 sunym     (1000) sunym     (1000)       23 2024-04-20 08:11:11.000000 colabgeek-1.3.5/src/ColabGeek.egg-info/requires.txt
+-rw-rw-r--   0 sunym     (1000) sunym     (1000)       10 2024-04-20 08:11:11.000000 colabgeek-1.3.5/src/ColabGeek.egg-info/top_level.txt
```

### Comparing `ColabGeek-1.3.4/LICENSE` & `colabgeek-1.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ColabGeek-1.3.4/PKG-INFO` & `colabgeek-1.3.5/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: ColabGeek
-Version: 1.3.4
-Summary: ColabGeek is designed to help run useful tools on Google Colab, including port forwarding, web IDE and so on. It is worth noting that this package is also compatible with other Ubuntu operating system servers, so try on other platforms as well.
-Author-email: Yiming Sun <yiming.sun12138@gmail.com>
-Project-URL: Homepage, https://github.com/yimingsun12138/ColabGeek
-Project-URL: Bug Tracker, https://github.com/yimingsun12138/ColabGeek/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: POSIX :: Linux
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # ColabGeek
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://github.com/yimingsun12138/ColabGeek/blob/main/LICENSE)
 [![PyPI version](https://badge.fury.io/py/ColabGeek.svg)](https://badge.fury.io/py/ColabGeek)
 
 ColabGeek Python package is designed to help run useful tools on Google Colab, including web IDE, port forwarding and so on. It is worth noting that this package is also compatible with other Ubuntu operating system based servers, so try this package on other platforms as well.
 
@@ -87,14 +73,27 @@
 # ColabGeek.Run_Rstudio_server has the following parameters:
 # - port The port you want to run Rstudio on, set to None to use the default port.
 # - verbose Show the running logs.
 
 main.Run_Rstudio_server()
 ```
 
+### Run JupyterLab
+[JupyterLab](https://jupyterlab.readthedocs.io/en/stable/index.html) is an interactive web IDE for working with Jupyter notebooks, code, and data. It is a flexible and extensible platform designed to support the entire workflow in data science, scientific computing, and machine learning projects. ColabGeek pulls the [mrdoge/jupyterlab docker image](https://hub.docker.com/r/mrdoge/jupyterlab) from Docker Hub and execute the docker container using [udocker](https://github.com/indigo-dc/udocker). Notice that it is not recommended to run udocker and JupyterLab under user root.
+
+```python
+# ColabGeek.Run_JupyterLab has the following parameters:
+# - port The port you want to run JupyterLab on, set to None to use the default port.
+# - password The JupyterLab login password, set to None and use the linux user password by default.
+# - mount_Colab Whether map the Colab /content directory to the JupyterLab container /content directory.
+# - verbose Show the running logs.
+
+main.Run_JupyterLab()
+```
+
 Google Colab does not allow any internet connections to their servers except the official web interface. So, port forwarding methods are required to proxy the web IDE installed.
 
 ### localtunnel
 
 ```python
 # ColabGeek.Run_localtunnel has the following parameters:
 # - port The port you want to expose to localtunnel, set to None and you will use the default port.
@@ -113,19 +112,27 @@
 # - port The port you want to expose to ngrok, set to None and you will use the default port.
 # - domain The customized ngrok URL, check the ngrok document.
 # - verbose Show the running logs.
 
 main.Run_ngrok()
 ```
 
-For now, all the port forwarding methods built in ColabGeek only accept http protocal. I am still tring to add TCP forwarding methods to ColabGeek. If you have any good ideas and advices, leave an issue.
+### Cloudflare Tunnel
+
+```python
+# ColabGeek.Run_Cloudflare_Tunnel has the following parameters:
+# - token The token of your tunnels created on Cloudflare.
+# - verbose Show the running logs.
+
+main.Run_Cloudflare_Tunnel(token = 'replace with your own tunnel token!')
+```
 
 ### shadowsocks
 
-Although not allowed by Google and not recommended by myself, building a proxy server using Colab sounds pretty 'Geek'. However, due to the lack of TCP forwarding method, ColabGeek can now only install shadowsocks on Colab but have no method to help to connect it. Just use this method on your own Ubuntu servers, that should work.
+Although not allowed by Google and not recommended by myself, building a proxy server using Colab sounds pretty 'Geek'. However, this function only helps to install and run shadowsocks on Colab, and I have no clue how to connect to the shadowsocks server. Just use this method on your own Ubuntu servers, that should work. If you have any good ideas, leave an issue please!
 
 ```python
 # ColabGeek.Run_shadowsocks has the following parameters:
 # - port The server port of shadowsocks, set to None and you will use the default port.
 # - password The shadowsocks password.
 # - encrypt The shadowsocks encrypt method.
 # - verbose Show the running logs.
```

### Comparing `ColabGeek-1.3.4/README.md` & `colabgeek-1.3.5/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,23 @@
+Metadata-Version: 2.1
+Name: ColabGeek
+Version: 1.3.5
+Summary: ColabGeek is designed to help run useful tools on Google Colab, including port forwarding, web IDE and so on. It is worth noting that this package is also compatible with other Ubuntu operating system servers, so try on other platforms as well.
+Author-email: Yiming Sun <yiming.sun12138@gmail.com>
+Project-URL: Homepage, https://github.com/yimingsun12138/ColabGeek
+Project-URL: Bug Tracker, https://github.com/yimingsun12138/ColabGeek/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: POSIX :: Linux
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Provides-Extra: full
+Requires-Dist: jupyter_server; extra == "full"
+
 # ColabGeek
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://github.com/yimingsun12138/ColabGeek/blob/main/LICENSE)
 [![PyPI version](https://badge.fury.io/py/ColabGeek.svg)](https://badge.fury.io/py/ColabGeek)
 
 ColabGeek Python package is designed to help run useful tools on Google Colab, including web IDE, port forwarding and so on. It is worth noting that this package is also compatible with other Ubuntu operating system based servers, so try this package on other platforms as well.
 
@@ -73,14 +89,27 @@
 # ColabGeek.Run_Rstudio_server has the following parameters:
 # - port The port you want to run Rstudio on, set to None to use the default port.
 # - verbose Show the running logs.
 
 main.Run_Rstudio_server()
 ```
 
+### Run JupyterLab
+[JupyterLab](https://jupyterlab.readthedocs.io/en/stable/index.html) is an interactive web IDE for working with Jupyter notebooks, code, and data. It is a flexible and extensible platform designed to support the entire workflow in data science, scientific computing, and machine learning projects. ColabGeek pulls the [mrdoge/jupyterlab docker image](https://hub.docker.com/r/mrdoge/jupyterlab) from Docker Hub and execute the docker container using [udocker](https://github.com/indigo-dc/udocker). Notice that it is not recommended to run udocker and JupyterLab under user root.
+
+```python
+# ColabGeek.Run_JupyterLab has the following parameters:
+# - port The port you want to run JupyterLab on, set to None to use the default port.
+# - password The JupyterLab login password, set to None and use the linux user password by default.
+# - mount_Colab Whether map the Colab /content directory to the JupyterLab container /content directory.
+# - verbose Show the running logs.
+
+main.Run_JupyterLab()
+```
+
 Google Colab does not allow any internet connections to their servers except the official web interface. So, port forwarding methods are required to proxy the web IDE installed.
 
 ### localtunnel
 
 ```python
 # ColabGeek.Run_localtunnel has the following parameters:
 # - port The port you want to expose to localtunnel, set to None and you will use the default port.
@@ -99,19 +128,27 @@
 # - port The port you want to expose to ngrok, set to None and you will use the default port.
 # - domain The customized ngrok URL, check the ngrok document.
 # - verbose Show the running logs.
 
 main.Run_ngrok()
 ```
 
-For now, all the port forwarding methods built in ColabGeek only accept http protocal. I am still tring to add TCP forwarding methods to ColabGeek. If you have any good ideas and advices, leave an issue.
+### Cloudflare Tunnel
+
+```python
+# ColabGeek.Run_Cloudflare_Tunnel has the following parameters:
+# - token The token of your tunnels created on Cloudflare.
+# - verbose Show the running logs.
+
+main.Run_Cloudflare_Tunnel(token = 'replace with your own tunnel token!')
+```
 
 ### shadowsocks
 
-Although not allowed by Google and not recommended by myself, building a proxy server using Colab sounds pretty 'Geek'. However, due to the lack of TCP forwarding method, ColabGeek can now only install shadowsocks on Colab but have no method to help to connect it. Just use this method on your own Ubuntu servers, that should work.
+Although not allowed by Google and not recommended by myself, building a proxy server using Colab sounds pretty 'Geek'. However, this function only helps to install and run shadowsocks on Colab, and I have no clue how to connect to the shadowsocks server. Just use this method on your own Ubuntu servers, that should work. If you have any good ideas, leave an issue please!
 
 ```python
 # ColabGeek.Run_shadowsocks has the following parameters:
 # - port The server port of shadowsocks, set to None and you will use the default port.
 # - password The shadowsocks password.
 # - encrypt The shadowsocks encrypt method.
 # - verbose Show the running logs.
```

### Comparing `ColabGeek-1.3.4/pyproject.toml` & `colabgeek-1.3.5/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -7,23 +7,26 @@
 where = ["src"]
 
 [tool.setuptools.package-data]
 "ColabGeek.shell_scripts" = ["*"]
 
 [project]
 name = "ColabGeek"
-version = "1.3.4"
+version = "1.3.5"
 authors = [
     {name = "Yiming Sun",email = "yiming.sun12138@gmail.com"},
 ]
 description = "ColabGeek is designed to help run useful tools on Google Colab, including port forwarding, web IDE and so on. It is worth noting that this package is also compatible with other Ubuntu operating system servers, so try on other platforms as well."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: POSIX :: Linux",
 ]
 
+[project.optional-dependencies]
+full = ["jupyter_server"]
+
 [project.urls]
 "Homepage" = "https://github.com/yimingsun12138/ColabGeek"
 "Bug Tracker" = "https://github.com/yimingsun12138/ColabGeek/issues"
```

### Comparing `ColabGeek-1.3.4/src/ColabGeek/ColabGeek.py` & `colabgeek-1.3.5/src/ColabGeek/ColabGeek.py`

 * *Files 10% similar despite different names*

```diff
@@ -53,22 +53,26 @@
         Mount Google Drive if mount_GD is set to True.
     tmp_path()
         Create a temporary directory in /tmp.
     Run_localtunnel(port = None,host = "https://localtunnel.me",subdomain = None,verbose = True)
         Install and run localtunnel for tunnelling.
     Run_ngrok(token = None,port = None,domain = None,verbose = True)
         Install and run ngrok for tunnelling.
+    Run_Cloudflare_Tunnel(token = None,verbose = True)
+        Install and run cloudflared for tunnelling.
     Run_Rstudio_server(port = None,verbose = True)
         Install and run Rstudio Server on Colab.
     Run_code_server(port = None,password = None,verbose = True)
         Install and run code server on Colab.
     Install_code_server_extension(extension,verbose = True)
         Install code server extensions.
     Config_code_server(property,value)
         Configure code server.
+    Run_JupyterLab(port = None,password = None,mount_Colab = True,verbose = True)
+        Install and run JupyterLab on Colab.
     Run_shadowsocks(port = None,password = None,encrypt = 'aes-256-gcm',verbose = True)
         Install and run shadowsocks on Colab.
     Install_Homebrew(verbose = True)
         Install Homebrew on Colab.
     Install_rbenv(verbose = True)
         Install rbenv on Colab.
     Install_Ruby(version = None,verbose = True)
@@ -77,14 +81,16 @@
         Install and run Jekyll on Colab.
     Run_stable_diffusion_webui(path = None,port = None,verbose = True,args = None,**kwargs)
         Install and run Stable Diffusion WebUI on Colab.
     busy_session(busy = None)
         Keep the Colab session active.
     Install_Miniconda(path = None,verbose = True)
         Install Miniconda on Colab.
+    Install_udocker(verbose = True)
+        Install udocker on Colab.
     """
     
     def __init__(self,user,password,sudo = True,port = 8787,mount_GD = False,keep_busy = True):
         """
         Initialize the ColabSession object.
 
         Initialize the ColabSession object by adding the system user, mounting Google Drive and setting temp directory.
@@ -282,14 +288,58 @@
         os.system("sleep 10")
 
         # return
         ngrok_url = os.popen("cat" + " " + "/tmp/" + str(self.path) + "/ngrok.log" + " " + "|" + " " + "grep 'started tunnel'")
         ngrok_url = ((ngrok_url.readlines())[0]).replace("\n","")
         return(ngrok_url)
 
+    # tunnelling with cloudflared
+    def Run_Cloudflare_Tunnel(self,token = None,verbose = True):
+        """
+        Install and run cloudflared for tunnelling.
+
+        Apart from the Colab notebook, Google Colab prohibits any network connections to the host server.
+        Therefore, a tunnelling method is required to access services installed on Colab.
+        This function helps to install and run cloudflared, which is a server-side daemon for Cloudflare Tunnel.
+
+        Parameters
+        ----------
+        token : str, optional
+            The token of your tunnels created on Cloudflare.
+        verbose : bool, optional
+            Whether to show the running logs.
+        """
+
+        # check param
+        if (token is None):
+            token = input("Input your tunnel token: ")
+
+        # install cloudflared
+        char_cmd = "curl -L --output" + " " + "/tmp/" + str(self.path) + "/cloudflared.deb" + " " + "https://github.com/cloudflare/cloudflared/releases/latest/download/cloudflared-linux-amd64.deb"
+        char_cmd = char_cmd + " " + "&&" + " " + "dpkg -i" + " " + "/tmp/" + str(self.path) + "/cloudflared.deb"
+        exec_logging = os.popen(char_cmd)
+        exec_logging = ''.join(exec_logging.readlines())
+        if verbose:
+            print("Install cloudflared: \n")
+            print(exec_logging)
+
+        # exec cmd
+        char_cmd = "cloudflared service install" + " " + str(token)
+        char_cmd = "nohup" + " " + char_cmd + " " + "> /tmp/" + str(self.path) + "/cloudflared.log 2>&1 &"
+
+        # exec
+        os.system(char_cmd)
+        os.system("sleep 30")
+        char_cmd = "cat" + " " + "/tmp/" + str(self.path) + "/cloudflared.log"
+        exec_logging = os.popen(char_cmd)
+        exec_logging = ''.join(exec_logging.readlines())
+        if verbose:
+            print("Run cloudflared: \n")
+            print(exec_logging)
+
     #####################
     ## web IDE methods ##
     #####################
 
     # run Rstudio server
     def Run_Rstudio_server(self,port = None,verbose = True):
         """
@@ -428,14 +478,81 @@
         # add property
         json_setting[str(property)] = value
 
         # dump settings
         with open(file_path,"w") as json_file:
             json.dump(json_setting,json_file,indent=4)
 
+    # run JupyterLab
+    def Run_JupyterLab(self,port = None,password = None,mount_Colab = True,verbose = True):
+        """
+        Install and run JupyterLab on Colab.
+
+        JupyterLab is a web IDE for working with Jupyter Notebooks, providing a powerful environment for interactive computing.
+        This function helps to install and run mrdoge/jupyterlab container from Docker Hub using udocker.
+
+        Parameters
+        ----------
+        port : int, optional
+            Listening port for JupyterLab.
+        password : str, optional
+            The JupyterLab login password.
+        mount_Colab : bool, optional
+            Whether map the Colab /content directory to the JupyterLab container /content directory.
+        verbose : bool, optional
+            Whether to show the running logs.
+
+        Raises
+        ------
+        ImportError
+            If the jupyter_server.auth module is not installed.
+        """
+
+        # import dependency
+        try:
+            import jupyter_server.auth
+        except ImportError:
+            print("jupyter_server.auth does not exist, try execute `pip install jupyter_server`.")
+            return(None)
+
+        # check param
+        if (str(self.user) == 'root'):
+            warnings.warn(message = "Running udocker and JupyterLab as root may lead to unexpected issues!",category = UserWarning)
+        if (port is None):
+            port = self.port
+        if (password is None):
+            password = self.password
+        password = jupyter_server.auth.passwd(str(password))
+
+        # install udocker
+        self.Install_udocker(verbose = verbose)
+
+        # pull JupyterLab
+        char_cmd = "sudo -u" + " " + str(self.user) + " " + "udocker --allow-root pull mrdoge/jupyterlab"
+        exec_logging = os.popen(char_cmd)
+        exec_logging = ''.join(exec_logging.readlines())
+        if verbose:
+            print("Pull mrdoge/jupyterlab: \n")
+            print(exec_logging)
+
+        # run JupyterLab
+        char_cmd = "sudo -u" + " " + str(self.user) + " " + "udocker --allow-root run -p" + " " + str(port) + ":" + "8888"
+        if mount_Colab:
+            char_cmd = char_cmd + " " + "-v /content:/content"
+        char_cmd = char_cmd + " " + "mrdoge/jupyterlab" + " " + "jupyter lab --allow-root --ip=0.0.0.0 --port=8888 --no-browser" + " " + "--ServerApp.password" + "=" + "'" + str(password) + "'"
+        char_cmd = "nohup" + " " + char_cmd + " " + ">" + " " + "/tmp/" + str(self.path) + "/JupyterLab.log 2>&1 &"
+        os.system(char_cmd)
+        os.system("sleep 120")
+        char_cmd = "cat" + " " + "/tmp/" + str(self.path) + "/JupyterLab.log"
+        exec_logging = os.popen(char_cmd)
+        exec_logging = ''.join(exec_logging.readlines())
+        if verbose:
+            print("JupyterLab log: \n")
+            print(exec_logging)
+
     ###################
     ## proxy methods ##
     ###################
 
     # run shadowsocks
     def Run_shadowsocks(self,port = None,password = None,encrypt = 'aes-256-gcm',verbose = True):
         """
@@ -791,14 +908,36 @@
         char_cmd = "sudo -u" + " " + str(self.user) + " " + "bash" + " " + str(script_path) + " " + str(self.user) + " " + str(path)
         exec_logging = os.popen(char_cmd)
         exec_logging = ''.join(exec_logging.readlines())
         if verbose:
             print("Install Miniconda: \n")
             print(exec_logging)
 
+    # install udocker
+    def Install_udocker(self,verbose = True):
+        """
+        Install udocker on Colab.
+
+        udocker is a basic user tool to execute simple docker containers in user space without requiring root privileges.
+        udocker can also run inside a docker container, making it a perfect tool for executing containers on Colab.
+
+        Parameters
+        ----------
+        verbose : bool, optional
+            Whether to show the running logs.
+        """
+
+        # install udocker
+        char_cmd = "pip install udocker" + " " + "&&" + " " + "sudo -u" + " " + str(self.user) + " " + "udocker --allow-root install"
+        exec_logging = os.popen(char_cmd)
+        exec_logging = ''.join(exec_logging.readlines())
+        if verbose:
+            print("Install udocker: \n")
+            print(exec_logging)
+
 ##########################
 ## define other methods ##
 ##########################
 
 # update environment
 def update_environment(verbose = True):
     """
```

### Comparing `ColabGeek-1.3.4/src/ColabGeek/shell_scripts/Install_Homebrew.exp` & `colabgeek-1.3.5/src/ColabGeek/shell_scripts/Install_Homebrew.exp`

 * *Files identical despite different names*

### Comparing `ColabGeek-1.3.4/src/ColabGeek/shell_scripts/Install_Miniconda.sh` & `colabgeek-1.3.5/src/ColabGeek/shell_scripts/Install_Miniconda.sh`

 * *Files identical despite different names*

### Comparing `ColabGeek-1.3.4/src/ColabGeek/shell_scripts/Run_code_server.exp` & `colabgeek-1.3.5/src/ColabGeek/shell_scripts/Run_code_server.exp`

 * *Files identical despite different names*

### Comparing `ColabGeek-1.3.4/src/ColabGeek.egg-info/PKG-INFO` & `colabgeek-1.3.5/src/ColabGeek.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 Metadata-Version: 2.1
 Name: ColabGeek
-Version: 1.3.4
+Version: 1.3.5
 Summary: ColabGeek is designed to help run useful tools on Google Colab, including port forwarding, web IDE and so on. It is worth noting that this package is also compatible with other Ubuntu operating system servers, so try on other platforms as well.
 Author-email: Yiming Sun <yiming.sun12138@gmail.com>
 Project-URL: Homepage, https://github.com/yimingsun12138/ColabGeek
 Project-URL: Bug Tracker, https://github.com/yimingsun12138/ColabGeek/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Provides-Extra: full
+Requires-Dist: jupyter_server; extra == "full"
 
 # ColabGeek
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://github.com/yimingsun12138/ColabGeek/blob/main/LICENSE)
 [![PyPI version](https://badge.fury.io/py/ColabGeek.svg)](https://badge.fury.io/py/ColabGeek)
 
 ColabGeek Python package is designed to help run useful tools on Google Colab, including web IDE, port forwarding and so on. It is worth noting that this package is also compatible with other Ubuntu operating system based servers, so try this package on other platforms as well.
@@ -87,14 +89,27 @@
 # ColabGeek.Run_Rstudio_server has the following parameters:
 # - port The port you want to run Rstudio on, set to None to use the default port.
 # - verbose Show the running logs.
 
 main.Run_Rstudio_server()
 ```
 
+### Run JupyterLab
+[JupyterLab](https://jupyterlab.readthedocs.io/en/stable/index.html) is an interactive web IDE for working with Jupyter notebooks, code, and data. It is a flexible and extensible platform designed to support the entire workflow in data science, scientific computing, and machine learning projects. ColabGeek pulls the [mrdoge/jupyterlab docker image](https://hub.docker.com/r/mrdoge/jupyterlab) from Docker Hub and execute the docker container using [udocker](https://github.com/indigo-dc/udocker). Notice that it is not recommended to run udocker and JupyterLab under user root.
+
+```python
+# ColabGeek.Run_JupyterLab has the following parameters:
+# - port The port you want to run JupyterLab on, set to None to use the default port.
+# - password The JupyterLab login password, set to None and use the linux user password by default.
+# - mount_Colab Whether map the Colab /content directory to the JupyterLab container /content directory.
+# - verbose Show the running logs.
+
+main.Run_JupyterLab()
+```
+
 Google Colab does not allow any internet connections to their servers except the official web interface. So, port forwarding methods are required to proxy the web IDE installed.
 
 ### localtunnel
 
 ```python
 # ColabGeek.Run_localtunnel has the following parameters:
 # - port The port you want to expose to localtunnel, set to None and you will use the default port.
@@ -113,19 +128,27 @@
 # - port The port you want to expose to ngrok, set to None and you will use the default port.
 # - domain The customized ngrok URL, check the ngrok document.
 # - verbose Show the running logs.
 
 main.Run_ngrok()
 ```
 
-For now, all the port forwarding methods built in ColabGeek only accept http protocal. I am still tring to add TCP forwarding methods to ColabGeek. If you have any good ideas and advices, leave an issue.
+### Cloudflare Tunnel
+
+```python
+# ColabGeek.Run_Cloudflare_Tunnel has the following parameters:
+# - token The token of your tunnels created on Cloudflare.
+# - verbose Show the running logs.
+
+main.Run_Cloudflare_Tunnel(token = 'replace with your own tunnel token!')
+```
 
 ### shadowsocks
 
-Although not allowed by Google and not recommended by myself, building a proxy server using Colab sounds pretty 'Geek'. However, due to the lack of TCP forwarding method, ColabGeek can now only install shadowsocks on Colab but have no method to help to connect it. Just use this method on your own Ubuntu servers, that should work.
+Although not allowed by Google and not recommended by myself, building a proxy server using Colab sounds pretty 'Geek'. However, this function only helps to install and run shadowsocks on Colab, and I have no clue how to connect to the shadowsocks server. Just use this method on your own Ubuntu servers, that should work. If you have any good ideas, leave an issue please!
 
 ```python
 # ColabGeek.Run_shadowsocks has the following parameters:
 # - port The server port of shadowsocks, set to None and you will use the default port.
 # - password The shadowsocks password.
 # - encrypt The shadowsocks encrypt method.
 # - verbose Show the running logs.
```

### Comparing `ColabGeek-1.3.4/src/ColabGeek.egg-info/SOURCES.txt` & `colabgeek-1.3.5/src/ColabGeek.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 README.md
 pyproject.toml
 src/ColabGeek/ColabGeek.py
 src/ColabGeek/__init__.py
 src/ColabGeek.egg-info/PKG-INFO
 src/ColabGeek.egg-info/SOURCES.txt
 src/ColabGeek.egg-info/dependency_links.txt
+src/ColabGeek.egg-info/requires.txt
 src/ColabGeek.egg-info/top_level.txt
 src/ColabGeek/shell_scripts/Install_Homebrew.exp
 src/ColabGeek/shell_scripts/Install_Jekyll.exp
 src/ColabGeek/shell_scripts/Install_Miniconda.sh
 src/ColabGeek/shell_scripts/Install_Ruby.exp
 src/ColabGeek/shell_scripts/Install_rbenv.exp
 src/ColabGeek/shell_scripts/Run_Rstudio_server.sh
```

