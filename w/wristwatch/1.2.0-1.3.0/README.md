# Comparing `tmp/wristwatch-1.2.0.tar.gz` & `tmp/wristwatch-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wristwatch-1.2.0.tar", last modified: Wed Apr 17 16:39:32 2024, max compression
+gzip compressed data, was "wristwatch-1.3.0.tar", last modified: Sat Apr 20 10:16:34 2024, max compression
```

## Comparing `wristwatch-1.2.0.tar` & `wristwatch-1.3.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 zwolfrost  (1000) zwolfrost  (1000)        0 2024-04-17 16:39:32.340575 wristwatch-1.2.0/
--rwxrwxrwx   0 zwolfrost  (1000) zwolfrost  (1000)     1086 2022-12-24 08:05:26.000000 wristwatch-1.2.0/LICENSE
--rw-rw-r--   0 zwolfrost  (1000) zwolfrost  (1000)     3294 2024-04-17 16:39:32.336575 wristwatch-1.2.0/PKG-INFO
--rwxrwxrwx   0 zwolfrost  (1000) zwolfrost  (1000)     3081 2024-04-17 16:39:26.000000 wristwatch-1.2.0/README.md
--rw-rw-r--   0 zwolfrost  (1000) zwolfrost  (1000)       38 2024-04-17 16:39:32.340575 wristwatch-1.2.0/setup.cfg
--rw-rw-r--   0 zwolfrost  (1000) zwolfrost  (1000)      554 2024-04-17 16:26:06.000000 wristwatch-1.2.0/setup.py
-drwxrwxr-x   0 zwolfrost  (1000) zwolfrost  (1000)        0 2024-04-17 16:39:32.336575 wristwatch-1.2.0/wristwatch/
--rw-rw-r--   0 zwolfrost  (1000) zwolfrost  (1000)       36 2024-04-17 16:36:04.000000 wristwatch-1.2.0/wristwatch/__init__.py
--rw-rw-r--   0 zwolfrost  (1000) zwolfrost  (1000)     9213 2024-04-17 16:33:46.000000 wristwatch-1.2.0/wristwatch/wristwatch.py
-drwxrwxr-x   0 zwolfrost  (1000) zwolfrost  (1000)        0 2024-04-17 16:39:32.336575 wristwatch-1.2.0/wristwatch.egg-info/
--rw-rw-r--   0 zwolfrost  (1000) zwolfrost  (1000)     3294 2024-04-17 16:39:32.000000 wristwatch-1.2.0/wristwatch.egg-info/PKG-INFO
--rw-rw-r--   0 zwolfrost  (1000) zwolfrost  (1000)      280 2024-04-17 16:39:32.000000 wristwatch-1.2.0/wristwatch.egg-info/SOURCES.txt
--rw-rw-r--   0 zwolfrost  (1000) zwolfrost  (1000)        1 2024-04-17 16:39:32.000000 wristwatch-1.2.0/wristwatch.egg-info/dependency_links.txt
--rw-rw-r--   0 zwolfrost  (1000) zwolfrost  (1000)       59 2024-04-17 16:39:32.000000 wristwatch-1.2.0/wristwatch.egg-info/entry_points.txt
--rw-rw-r--   0 zwolfrost  (1000) zwolfrost  (1000)       77 2024-04-17 16:39:32.000000 wristwatch-1.2.0/wristwatch.egg-info/requires.txt
--rw-rw-r--   0 zwolfrost  (1000) zwolfrost  (1000)       11 2024-04-17 16:39:32.000000 wristwatch-1.2.0/wristwatch.egg-info/top_level.txt
+drwxrwxr-x   0 zwolfrost  (1000) zwolfrost  (1000)        0 2024-04-20 10:16:34.398219 wristwatch-1.3.0/
+-rwxrwxrwx   0 zwolfrost  (1000) zwolfrost  (1000)     1086 2022-12-24 08:05:26.000000 wristwatch-1.3.0/LICENSE
+-rw-rw-r--   0 zwolfrost  (1000) zwolfrost  (1000)     3574 2024-04-20 10:16:34.398219 wristwatch-1.3.0/PKG-INFO
+-rwxrwxrwx   0 zwolfrost  (1000) zwolfrost  (1000)     3366 2024-04-20 09:52:50.000000 wristwatch-1.3.0/README.md
+-rw-rw-r--   0 zwolfrost  (1000) zwolfrost  (1000)       38 2024-04-20 10:16:34.398219 wristwatch-1.3.0/setup.cfg
+-rw-rw-r--   0 zwolfrost  (1000) zwolfrost  (1000)      554 2024-04-20 07:42:03.000000 wristwatch-1.3.0/setup.py
+drwxrwxr-x   0 zwolfrost  (1000) zwolfrost  (1000)        0 2024-04-20 10:16:34.398219 wristwatch-1.3.0/wristwatch/
+-rw-rw-r--   0 zwolfrost  (1000) zwolfrost  (1000)        0 2024-04-20 08:15:23.000000 wristwatch-1.3.0/wristwatch/__init__.py
+-rw-rw-r--   0 zwolfrost  (1000) zwolfrost  (1000)    10153 2024-04-20 09:58:15.000000 wristwatch-1.3.0/wristwatch/wristwatch.py
+drwxrwxr-x   0 zwolfrost  (1000) zwolfrost  (1000)        0 2024-04-20 10:16:34.398219 wristwatch-1.3.0/wristwatch.egg-info/
+-rw-rw-r--   0 zwolfrost  (1000) zwolfrost  (1000)     3574 2024-04-20 10:16:34.000000 wristwatch-1.3.0/wristwatch.egg-info/PKG-INFO
+-rw-rw-r--   0 zwolfrost  (1000) zwolfrost  (1000)      280 2024-04-20 10:16:34.000000 wristwatch-1.3.0/wristwatch.egg-info/SOURCES.txt
+-rw-rw-r--   0 zwolfrost  (1000) zwolfrost  (1000)        1 2024-04-20 10:16:34.000000 wristwatch-1.3.0/wristwatch.egg-info/dependency_links.txt
+-rw-rw-r--   0 zwolfrost  (1000) zwolfrost  (1000)       59 2024-04-20 10:16:34.000000 wristwatch-1.3.0/wristwatch.egg-info/entry_points.txt
+-rw-rw-r--   0 zwolfrost  (1000) zwolfrost  (1000)       77 2024-04-20 10:16:34.000000 wristwatch-1.3.0/wristwatch.egg-info/requires.txt
+-rw-rw-r--   0 zwolfrost  (1000) zwolfrost  (1000)       11 2024-04-20 10:16:34.000000 wristwatch-1.3.0/wristwatch.egg-info/top_level.txt
```

### Comparing `wristwatch-1.2.0/LICENSE` & `wristwatch-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wristwatch-1.2.0/PKG-INFO` & `wristwatch-1.3.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,80 +1,73 @@
-Metadata-Version: 2.1
-Name: wristwatch
-Version: 1.2.0
-Summary: Yet another Python watcher for website updates.
-Home-page: https://github.com/zWolfrost/wristwatch
-Author: zWolfrost
-License: UNKNOWN
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# wristwatch
-[![PyPI version](https://img.shields.io/pypi/v/wristwatch)](https://pypi.org/project/wristwatch/)
-[![PyPI downloads](https://img.shields.io/pypi/dm/wristwatch)](https://pypi.org/project/wristwatch/)
-[![GitHub license](https://img.shields.io/github/license/zWolfrost/wristwatch)](LICENSE)
-
-Yet another Python watcher for website updates.
-
-&nbsp;
-## Features
-- Selecting elements to watch with CSS selectors.
-- Automatic importing of cookies from many browsers.
-- Emailing the changes to yourself.
-- Other features...
-
-You can safely quit watching at any time by pressing `Ctrl+C`.
-
-&nbsp;
-## Installation
-After having installed [Python 3](https://www.python.org/downloads/) with pip, you can install wristwatch using the following command:
-```bash
-pip install wristwatch
-```
-
-&nbsp;
-## Arguments
-| Command       | Shorthand | Example                  | Description
-|:-:            |:-:        | :-:                      |:-
-|               |           | `https://example.com/`   | The URL of the webpage to scrape.
-| `--browser`   | `-b`      | `-b chrome`              | Name of the browser to get cookies from (by default, any browser possible). See `--help` for supported browsers.
-| `--frequency` | `-f`      | `-f 60`                  | Frequency of fetches in seconds (default: 60).
-| `--selector`  | `-s`      | `-s #minutes -s #hours`  | CSS selector of element(s) to scrape. Can be used multiple times.
-| `--email`     | `-e`      | `-e example@gmail.com`   | Email address to self-send the changes to.
-| `--password`  | `-p`      | `-p aaaa bbbb cccc dddd` | Email "app" password. [Here's a guide on how to generate one](https://support.google.com/accounts/answer/185833#app-passwords).
-| `--quiet`     | `-q`      | `-q`                     | Decrease output verbosity.
-| `--loop`      | `-l`      | `-l`                     | Keep watching for changes even after the first one.
-| `--output`    | `-o`      | `-o output.txt`          | Save the last fetch to a file.
-| `--input`     | `-i`      | `-i input.txt`           | Load the first fetch from a file.
-| `--alert`     | `-a`      | `-a`                     | Play a sound when changes are detected.
-| `--version`   | `-v`      | `-v`                     | Show the program's version.
-| `--help`      | `-h`      | `-h`                     | Show the help message on how to use the program.
-
-&nbsp;
-## Examples
-```bash
-wristwatch "https://relaxingclock.com" -s "#minutes" -f 5 -a -l
-```
-
-&nbsp;
-## Screenshots
-
-![Enter commands](screenshots/1.png)
-
-&nbsp;
-## Changelog
-*This changelog only includes changes that are worth mentioning.*
-
-- **1.0.0**:
-<br>- Initial release.
-	- 1.0.1
-	<br>-Specified dependencies version requirements
-	- 1.0.2
-	<br>-Fixed `--loop` argument not working
-- **1.1.0**:
-<br>- Added `--alert` argument to play a sound when changes are detected.
-- **1.2.0**:
-<br>- Added `--debug` argument to show debug info & error messages.
-<br>- Changed "rookiepy" dependency for "browser-cookie3"
-<br>- Better error handling.
-
+# wristwatch
+[![PyPI version](https://img.shields.io/pypi/v/wristwatch)](https://pypi.org/project/wristwatch/)
+[![PyPI downloads](https://img.shields.io/pypi/dm/wristwatch)](https://pypi.org/project/wristwatch/)
+[![GitHub license](https://img.shields.io/github/license/zWolfrost/wristwatch)](LICENSE)
+
+Yet another Python watcher for website updates.
+
+&nbsp;
+## Features
+- Selecting elements to watch with CSS selectors.
+- Automatic importing of cookies from many browsers.
+- Emailing the changes to yourself.
+- Other features...
+
+You can safely quit watching at any time by pressing `Ctrl+C`.
+
+&nbsp;
+## Installation
+After having installed [Python 3](https://www.python.org/downloads/) with pip, you can install wristwatch using the following command:
+```bash
+pip install wristwatch
+```
+
+&nbsp;
+## Arguments
+| Command            | Example                     | Description
+|:-:                 | :-:                         |:-
+|                    | `"https://example.com/"`    | The URL of the webpage to scrape.
+| `-b` `--browser`   | `-b "chrome"`               | Name of the browser to get cookies from (by default, any<br>browser possible). See `--help` for supported browsers.
+| `-f` `--frequency` | `-f 60`                     | Frequency of fetches in seconds (default: 60).
+| `-s` `--selector`  | `-s "#minutes" -s "#hours"` | CSS selector of element(s) to scrape. Can be used multiple times.
+| `-a` `--attribute` | `-a "href" -a "title"`      | Attribute of the element(s) to scrape. Can be used multiple times.<br>Can also be "text" to scrape the text content.
+| `-e` `--email`     | `-e "example@gmail.com"`    | Email address to self-send the changes to.
+| `-p` `--password`  | `-p "aaaa bbbb cccc dddd"`  | Email "app" password. [Here's a guide on how to generate one](https://support.google.com/accounts/answer/185833#app-passwords).
+| `-i` `--input`     | `-i "input.txt"`            | Load the first fetch from a file.
+| `-o` `--output`    | `-o "output.txt"`           | Save the last fetch to a file.
+| `-q` `--quiet`     | `-q`                        | Decrease output verbosity.
+| `-l` `--loop`      | `-l`                        | Keep watching for changes even after the first one.
+| `-c` `--chime`     | `-c`                        | Play a sound when changes are detected.
+| `-v` `--version`   | `-v`                        | Show the program's version.
+| `-h` `--help`      | `-h`                        | Show the help message on how to use the program.
+
+&nbsp;
+## Examples
+```bash
+wristwatch "https://relaxingclock.com" -s "#minutes" -f 5 -a -l
+```
+
+&nbsp;
+## Screenshots
+
+![Enter commands](screenshots/1.png)
+
+&nbsp;
+## Changelog
+*This changelog only includes changes that are worth mentioning.*
+
+- **1.0.0**:
+<br>- Initial release.
+	- 1.0.1
+	<br>-Specified dependencies version requirements
+	- 1.0.2
+	<br>-Fixed `--loop` argument not working
+- **1.1.0**:
+<br>- Added `--alert` argument to play a sound when changes are detected.
+- **1.2.0**:
+<br>- Added `--debug` argument to show debug info & error messages.
+<br>- Changed "rookiepy" dependency for "browser-cookie3"
+<br>- Better error handling.
+- **1.3.0**:
+<br>- Added `--attribute` argument to scrape attributes and text content.
+<br>- Changed `--alert` argument name to `--chime`
+<br>- Better error handling.
```

### Comparing `wristwatch-1.2.0/setup.py` & `wristwatch-1.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
 	name="wristwatch",
 	author="zWolfrost",
-	version="1.2.0",
+	version="1.3.0",
 	description="Yet another Python watcher for website updates.",
 	long_description=open("README.md").read(),
 	long_description_content_type="text/markdown",
 	url="https://github.com/zWolfrost/wristwatch",
 	packages=find_packages(),
 	install_requires=[
 		"beautifulsoup4>=4.11.0",
```

### Comparing `wristwatch-1.2.0/wristwatch/wristwatch.py` & `wristwatch-1.3.0/wristwatch/wristwatch.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 #! venv/bin/python 
 
 import time, os, sys, argparse, difflib
 from urllib.parse import urlparse
 
 from selenium.webdriver.chrome.options import Options
 from selenium.webdriver import Chrome
+
 from bs4 import BeautifulSoup
 from bs4.formatter import HTMLFormatter
+from soupsieve.util import SelectorSyntaxError
+
 import browser_cookie3, chime
 
 import smtplib, ssl
 from email.message import EmailMessage
 
 
 debug_mode = False
@@ -21,27 +24,27 @@
 	parser = argparse.ArgumentParser(prog="wristwatch", description="Yet another Python watcher for website updates.")
 
 	parser.add_argument("webpage", type=str, help="The URL of the webpage to scrape.", metavar="URL")
 
 	parser.add_argument("-b", "--browser", type=str, help="Name of the browser to get cookies from (by default, any browser possible).", default="load", choices=["brave", "chrome", "chromium", "edge", "firefox", "librewolf", "opera", "opera_gx", "safari", "vivaldi"])
 	parser.add_argument("-f", "--frequency", type=int, help="Frequency of fetches in seconds (default: 60).", default=60, metavar="SECONDS")
 	parser.add_argument("-s", "--selector", type=str, help="CSS selector of element(s) to scrape. Can be used multiple times.", action="extend", nargs="+")
+	parser.add_argument("-a", "--attribute", type=str, help="Attribute of the element(s) to scrape. Can be used multiple times. Can also be \"text\" to scrape the text content.", action="extend", nargs="+")
 
 	parser.add_argument("-e", "--email", type=str, help="Email address to self-send the changes to.", required=("-p" in sys.argv or "--password" in sys.argv))
 	parser.add_argument("-p", "--password", type=str, help="Email \"app\" password. Here's a guide on how to generate one: https://support.google.com/accounts/answer/185833", required=("-e" in sys.argv or "--email" in sys.argv))
 
-	parser.add_argument("-q", "--quiet", help="Decrease output verbosity.", action="store_true")
-	parser.add_argument("-l", "--loop", help="Keep watching for changes even after the first one.", action="store_true")
-
-	parser.add_argument("-o", "--output", type=str, help="Save the last fetch to a file.", metavar="FILE")
 	parser.add_argument("-i", "--input", type=str, help="Load the first fetch from a file.", metavar="FILE")
+	parser.add_argument("-o", "--output", type=str, help="Save the last fetch to a file.", metavar="FILE")
 
-	parser.add_argument("-a", "--alert", help="Play a sound when changes are detected.", action="store_true")
+	parser.add_argument("-q", "--quiet", help="Decrease output verbosity.", action="store_true")
+	parser.add_argument("-l", "--loop", help="Keep watching for changes even after the first one.", action="store_true")
+	parser.add_argument("-c", "--chime", help="Play a sound when changes are detected.", action="store_true")
 
-	parser.add_argument("-v", "--version", action="version", version="%(prog)s 1.2.0")
+	parser.add_argument("-v", "--version", action="version", version="%(prog)s 1.3.0")
 	parser.add_argument("-d", "--debug", help="Enable debug mode.", action="store_true")
 
 	return vars(parser.parse_args())
 
 
 def cookie_to_dict(cookie) -> dict:
 	cookie_dict = {
@@ -75,28 +78,44 @@
 				if (debug_mode):
 					print(f"COOKIE NO. {i + 1}")
 					print(e)
 				errorCookies += 1
 
 		return len(cookies) - errorCookies
 
-def fetch_driver(driver: Chrome, selectors: str = None) -> str:
+def fetch_driver(driver: Chrome, selectors: list = None, attributes: list = None) -> str:
 	formatter = HTMLFormatter(indent=3)
 	soup = BeautifulSoup(driver.page_source, "html.parser")
 
 	if (selectors is None):
 		return str(soup.prettify(formatter=formatter))
 	else:
 		fetch = ""
 
 		for selector in selectors:
-			for i, element in enumerate(soup.select(selector)):
-				fetch += str(element.prettify(formatter=formatter))
-				if (i < len(soup.select(selector)) - 1):
-					fetch += "\n"
+
+			elements = soup.select(selector)
+
+			for i, el in enumerate(elements):
+				if (attributes):
+					for attributeName in attributes:
+						if (attributeName == "text"):
+							fetch += el.get_text() + "\n"
+						else:
+							attributeValue = el.get(attributeName, None)
+							if (attributeValue is not None):
+								if (isinstance(attributeValue, list)):
+									attributeValue = " ".join(attributeValue)
+								fetch += attributeValue + "\n"
+				else:
+					fetch += str(el.prettify(formatter=formatter))
+					if (i < len(elements) - 1):
+						fetch += "\n"
+
+		fetch = fetch.strip()
 
 		return fetch
 
 
 def print_text(text: str, line_numbers: bool = False, prefix: str = ""):
 	if (text == ""):
 		print("<empty>")
@@ -116,19 +135,23 @@
 
 		if (max_length and len(full_line) > max_length):
 			full_line = full_line[:max_length - len(break_line)] + break_line
 
 		print(full_line)
 
 def print_sleep(string: str, seconds: int = 0):
-	padding = len(string.format(seconds))
-	for i in range(seconds, 0, -1):
-		print("\r" + (string.format(i)).ljust(padding), end="")
-		time.sleep(1)
-	print("\r" + " " * padding + "\r", end="")
+	try:
+		padding = len(string.format(seconds))
+		for i in range(seconds, 0, -1):
+			print("\r" + (string.format(i)).ljust(padding), end="")
+			time.sleep(1)
+		print("\r" + " " * padding + "\r", end="")
+	except KeyboardInterrupt:
+		print("\b\b  ")
+		sys.exit()
 
 
 def send_email(from_email: str, to_email: str, password: str, subject="", body="", attachments=[]):
 	msg = EmailMessage()
 	msg["From"] = from_email
 	msg["To"] = to_email
 	msg["Subject"] = subject
@@ -179,15 +202,15 @@
 	try:
 		####
 		## Load the webpage
 		####
 
 		try:
 			driver.get(ARGS["webpage"])
-		except:
+		except Exception:
 			print("Failed to load the webpage. Please check the URL and ensure that your internet connection is working.")
 			sys.exit()
 
 
 
 		####
 		## Get cookies and apply them
@@ -218,15 +241,20 @@
 			else:
 				with open(ARGS["input"], "r") as f:
 					first_fetch = f.read()
 				print(f"First fetch loaded from \"{ARGS['input']}\".")
 		else:
 			driver.refresh()
 			print_sleep("Waiting before the first fetch. {} seconds remaining...", ARGS["frequency"])
-			first_fetch = fetch_driver(driver, ARGS["selector"])
+
+			try:
+				first_fetch = fetch_driver(driver, ARGS["selector"], ARGS["attribute"])
+			except SelectorSyntaxError as e:
+				print(f"\n{e.__class__.__name__}: {e}")
+				sys.exit()
 
 			if (ARGS["quiet"]):
 				print("First fetch done. Waiting for changes...")
 			else:
 				print("\n#### First fetch: ####")
 				print_text(first_fetch, line_numbers=True)
 				print()
@@ -248,22 +276,22 @@
 		fetches = 0
 
 		while True:
 			driver.refresh()
 			print_sleep(f"No changes detected ({fetches} fetches). Waiting {{}} seconds before the next fetch...", ARGS["frequency"])
 			print("\rFetching...", end="")
 
-			current_fetch = fetch_driver(driver, ARGS["selector"])
+			current_fetch = fetch_driver(driver, ARGS["selector"], ARGS["attribute"])
 
 			fetches += 1
 
 			if (first_fetch != current_fetch):
 				diff = "\n".join(difflib.unified_diff(first_fetch.splitlines(), current_fetch.splitlines(), lineterm=""))
 
-				if (ARGS["alert"]):
+				if (ARGS["chime"]):
 					chime.info()
 
 				print("\r", end="")
 				if (ARGS["quiet"]):
 					print(f"Changes detected after {fetches} fetches!")
 				else:
 					print(f"#### Changes detected after {fetches} fetches! Diff: ####")
@@ -282,16 +310,16 @@
 
 				if (ARGS["loop"]):
 					first_fetch = current_fetch
 					fetches = 0
 				else:
 					break
 
-	except BaseException as e:
-		if (e.__class__ in (KeyboardInterrupt, SystemExit) and not debug_mode):
-			print(f"\nStopped watching.")
+	except () if debug_mode else BaseException as e:
+		if (e.__class__ in (KeyboardInterrupt, SystemExit)):
+			print(f"Stopped watching.")
 		else:
-			print(f"\n\"{e.__class__.__name__}\" Exception")
+			print(f"\"{e.__class__.__name__}\" Exception")
 
 	finally:
 		print(f"Closing drivers...")
 		driver.quit()
```

